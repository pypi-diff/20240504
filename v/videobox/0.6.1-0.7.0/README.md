# Comparing `tmp/videobox-0.6.1.tar.gz` & `tmp/videobox-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "videobox-0.6.1.tar", last modified: Sun Mar 31 16:10:52 2024, max compression
+gzip compressed data, was "videobox-0.7.0.tar", last modified: Sat May  4 13:38:28 2024, max compression
```

## Comparing `videobox-0.6.1.tar` & `videobox-0.7.0.tar`

### file list

```diff
@@ -1,107 +1,133 @@
-drwxr-xr-x   0 andrea.peltrin (1702769464) 858591763        0 2024-03-31 16:10:52.303230 videobox-0.6.1/
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      457 2023-12-29 17:16:46.000000 videobox-0.6.1/.flake8
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1124 2024-03-31 16:03:36.000000 videobox-0.6.1/.gitignore
-drwxr-xr-x   0 andrea.peltrin (1702769464) 858591763        0 2024-03-31 16:10:52.281968 videobox-0.6.1/.vscode/
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      721 2024-03-31 16:03:36.000000 videobox-0.6.1/.vscode/launch.json
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763       49 2023-12-28 09:45:56.000000 videobox-0.6.1/.vscode/settings.json
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1516 2023-12-28 09:45:56.000000 videobox-0.6.1/LICENSE
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     5629 2024-03-31 16:10:52.302954 videobox-0.6.1/PKG-INFO
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     4745 2024-03-31 16:03:36.000000 videobox-0.6.1/README.md
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763       70 2023-12-29 17:16:46.000000 videobox-0.6.1/Videobox.code-workspace
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      894 2024-03-31 16:03:36.000000 videobox-0.6.1/app.py
-drwxr-xr-x   0 andrea.peltrin (1702769464) 858591763        0 2024-03-31 16:10:52.283864 videobox-0.6.1/assets/
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     5045 2024-03-31 16:03:36.000000 videobox-0.6.1/assets/app.js
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763    13866 2024-03-31 16:03:36.000000 videobox-0.6.1/assets/app.scss
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     7842 2024-02-08 16:51:49.000000 videobox-0.6.1/assets/balloon.css
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1744 2024-03-03 20:13:16.000000 videobox-0.6.1/assets/button.scss
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     3167 2024-03-03 20:13:16.000000 videobox-0.6.1/assets/carousel.js
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1638 2024-03-03 20:13:16.000000 videobox-0.6.1/assets/carousel.scss
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     8128 2024-03-31 16:03:36.000000 videobox-0.6.1/assets/helpers.scss
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     6814 2024-02-08 16:51:49.000000 videobox-0.6.1/assets/normalize.css
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      971 2024-03-03 20:13:16.000000 videobox-0.6.1/assets/select.scss
-drwxr-xr-x   0 andrea.peltrin (1702769464) 858591763        0 2024-03-31 16:10:52.284453 videobox-0.6.1/macos/
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763    16835 2023-12-29 17:16:46.000000 videobox-0.6.1/macos/icon.png
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      538 2023-12-29 17:16:46.000000 videobox-0.6.1/macos/menubar-icon.svg
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1759 2024-03-31 16:03:36.000000 videobox-0.6.1/makefile
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763   130226 2024-03-03 20:13:16.000000 videobox-0.6.1/package-lock.json
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      622 2024-03-03 20:13:16.000000 videobox-0.6.1/package.json
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1171 2024-03-31 16:04:21.000000 videobox-0.6.1/pyproject.toml
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      191 2024-03-31 16:03:37.000000 videobox-0.6.1/requirements.txt
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      761 2024-03-31 16:05:03.000000 videobox-0.6.1/setup-app.py
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763       38 2024-03-31 16:10:52.303284 videobox-0.6.1/setup.cfg
-drwxr-xr-x   0 andrea.peltrin (1702769464) 858591763        0 2024-03-31 16:10:52.285757 videobox-0.6.1/videobox/
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     3004 2024-03-31 16:04:31.000000 videobox-0.6.1/videobox/__init__.py
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1904 2024-03-31 16:05:17.000000 videobox-0.6.1/videobox/api.py
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     2127 2024-03-31 16:03:37.000000 videobox-0.6.1/videobox/filters.py
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     2021 2024-03-31 16:03:37.000000 videobox-0.6.1/videobox/languages.py
-drwxr-xr-x   0 andrea.peltrin (1702769464) 858591763        0 2024-03-31 16:10:52.287397 videobox-0.6.1/videobox/main/
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      183 2023-12-29 17:16:46.000000 videobox-0.6.1/videobox/main/__init__.py
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     6930 2024-03-31 16:03:37.000000 videobox-0.6.1/videobox/main/queries.py
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763    12525 2024-03-31 16:03:37.000000 videobox-0.6.1/videobox/main/routes.py
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     5213 2024-03-31 16:03:37.000000 videobox-0.6.1/videobox/models.py
-drwxr-xr-x   0 andrea.peltrin (1702769464) 858591763        0 2024-03-31 16:10:52.296243 videobox-0.6.1/videobox/static/
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763    32206 2024-03-31 16:07:16.000000 videobox-0.6.1/videobox/static/app.css
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763    88100 2024-03-31 16:07:16.000000 videobox-0.6.1/videobox/static/app.css.map
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     2915 2024-03-31 16:07:17.000000 videobox-0.6.1/videobox/static/app.js
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763    22179 2024-03-31 16:07:17.000000 videobox-0.6.1/videobox/static/app.js.map
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763    34941 2023-12-29 17:16:46.000000 videobox-0.6.1/videobox/static/apple-touch-icon.png
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     8890 2023-12-29 17:16:46.000000 videobox-0.6.1/videobox/static/default-poster.png
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     4090 2023-12-29 17:16:46.000000 videobox-0.6.1/videobox/static/default-still.png
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1109 2023-12-29 17:16:46.000000 videobox-0.6.1/videobox/static/favicon.png
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      540 2023-12-29 17:16:46.000000 videobox-0.6.1/videobox/static/favicon.svg
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      358 2024-03-31 16:03:37.000000 videobox-0.6.1/videobox/static/icon-check-bold.svg
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      363 2024-03-31 16:03:37.000000 videobox-0.6.1/videobox/static/icon-check.svg
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      280 2023-12-29 17:16:46.000000 videobox-0.6.1/videobox/static/icon-close-bold.svg
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      308 2023-12-29 17:16:46.000000 videobox-0.6.1/videobox/static/icon-close.svg
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      570 2023-12-29 17:16:46.000000 videobox-0.6.1/videobox/static/icon-grid-bold.svg
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      576 2023-12-29 17:16:46.000000 videobox-0.6.1/videobox/static/icon-grid.svg
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      581 2024-03-03 20:13:16.000000 videobox-0.6.1/videobox/static/icon-heart-bold.svg
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      624 2024-03-03 20:13:16.000000 videobox-0.6.1/videobox/static/icon-heart-break-bold.svg
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      558 2024-03-03 20:13:16.000000 videobox-0.6.1/videobox/static/icon-heart-break.svg
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      511 2024-03-03 20:13:16.000000 videobox-0.6.1/videobox/static/icon-heart.svg
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      785 2024-03-03 20:13:16.000000 videobox-0.6.1/videobox/static/icon-heartbeat-bold.svg
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      765 2024-03-03 20:13:16.000000 videobox-0.6.1/videobox/static/icon-heartbeat.svg
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      418 2023-12-29 17:16:46.000000 videobox-0.6.1/videobox/static/icon-list-bold.svg
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      400 2023-12-29 17:16:46.000000 videobox-0.6.1/videobox/static/icon-list.svg
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      890 2023-12-29 17:16:46.000000 videobox-0.6.1/videobox/static/icon-magnet-bold.svg
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      863 2023-12-29 17:16:46.000000 videobox-0.6.1/videobox/static/icon-magnet.svg
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      252 2023-12-29 17:16:46.000000 videobox-0.6.1/videobox/static/icon-search-bold.svg
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      267 2023-12-29 17:16:46.000000 videobox-0.6.1/videobox/static/icon-search.svg
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      390 2023-12-29 17:16:46.000000 videobox-0.6.1/videobox/static/icon-tag-bold.svg
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      369 2023-12-29 17:16:46.000000 videobox-0.6.1/videobox/static/icon-tag.svg
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      606 2023-12-29 17:16:46.000000 videobox-0.6.1/videobox/static/icon-update-bold.svg
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      579 2023-12-29 17:16:46.000000 videobox-0.6.1/videobox/static/icon-update.svg
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      618 2023-12-29 17:16:46.000000 videobox-0.6.1/videobox/static/logo.svg
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763    16122 2024-03-31 16:03:37.000000 videobox-0.6.1/videobox/sync.py
-drwxr-xr-x   0 andrea.peltrin (1702769464) 858591763        0 2024-03-31 16:10:52.301374 videobox-0.6.1/videobox/templates/
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      319 2023-12-29 17:16:46.000000 videobox-0.6.1/videobox/templates/404.html
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     3272 2023-12-29 17:16:46.000000 videobox-0.6.1/videobox/templates/_episodes-grid.html
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     3186 2023-12-29 17:16:46.000000 videobox-0.6.1/videobox/templates/_episodes-list.html
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      577 2024-03-03 20:13:16.000000 videobox-0.6.1/videobox/templates/_follow-button.html
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      497 2024-03-03 20:13:16.000000 videobox-0.6.1/videobox/templates/_following.html
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      523 2024-03-03 20:13:16.000000 videobox-0.6.1/videobox/templates/_language-card-grid.html
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      566 2024-03-31 16:03:37.000000 videobox-0.6.1/videobox/templates/_meta.html
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1306 2024-03-31 16:03:37.000000 videobox-0.6.1/videobox/templates/_release_detail.html
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763       79 2023-12-29 17:16:46.000000 videobox-0.6.1/videobox/templates/_suggest.html
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      524 2024-03-03 20:13:16.000000 videobox-0.6.1/videobox/templates/_tag-card-grid.html
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      460 2024-03-31 16:03:37.000000 videobox-0.6.1/videobox/templates/_update-dialog-done.html
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      388 2024-03-31 16:03:37.000000 videobox-0.6.1/videobox/templates/_update-dialog.html
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     2178 2024-03-31 16:03:37.000000 videobox-0.6.1/videobox/templates/base.html
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      697 2024-03-31 16:03:37.000000 videobox-0.6.1/videobox/templates/first-import.html
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      574 2024-03-03 20:13:16.000000 videobox-0.6.1/videobox/templates/following.html
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     5249 2024-03-31 16:03:37.000000 videobox-0.6.1/videobox/templates/home.html
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      416 2024-03-03 20:13:16.000000 videobox-0.6.1/videobox/templates/language_detail.html
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1080 2024-03-31 16:03:37.000000 videobox-0.6.1/videobox/templates/log.html
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     2762 2024-03-03 20:13:16.000000 videobox-0.6.1/videobox/templates/macros.html
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1074 2024-03-03 20:13:16.000000 videobox-0.6.1/videobox/templates/search_results.html
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     4711 2024-03-31 16:03:37.000000 videobox-0.6.1/videobox/templates/series_detail.html
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      421 2024-03-03 20:13:16.000000 videobox-0.6.1/videobox/templates/tag_detail.html
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      952 2024-01-30 13:25:31.000000 videobox-0.6.1/videobox/templates/tags.html
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     3180 2024-03-31 16:10:47.000000 videobox-0.6.1/videobox/trackers.txt
-drwxr-xr-x   0 andrea.peltrin (1702769464) 858591763        0 2024-03-31 16:10:52.302469 videobox-0.6.1/videobox.egg-info/
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     5629 2024-03-31 16:10:52.000000 videobox-0.6.1/videobox.egg-info/PKG-INFO
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763     2668 2024-03-31 16:10:52.000000 videobox-0.6.1/videobox.egg-info/SOURCES.txt
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763        1 2024-03-31 16:10:52.000000 videobox-0.6.1/videobox.egg-info/dependency_links.txt
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763       44 2024-03-31 16:10:52.000000 videobox-0.6.1/videobox.egg-info/entry_points.txt
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763      132 2024-03-31 16:10:52.000000 videobox-0.6.1/videobox.egg-info/requires.txt
--rw-r--r--   0 andrea.peltrin (1702769464) 858591763        9 2024-03-31 16:10:52.000000 videobox-0.6.1/videobox.egg-info/top_level.txt
+drwxr-xr-x   0 andrea.peltrin (1702769464) 858591763        0 2024-05-04 13:38:28.462990 videobox-0.7.0/
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      457 2023-12-29 17:16:46.000000 videobox-0.7.0/.flake8
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1138 2024-05-04 07:56:01.000000 videobox-0.7.0/.gitignore
+drwxr-xr-x   0 andrea.peltrin (1702769464) 858591763        0 2024-05-04 13:38:28.431034 videobox-0.7.0/.vscode/
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1242 2024-05-04 07:55:45.000000 videobox-0.7.0/.vscode/launch.json
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763       49 2023-12-28 09:45:56.000000 videobox-0.7.0/.vscode/settings.json
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1204 2024-05-04 07:55:45.000000 videobox-0.7.0/CONTRIBUTING.md
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1516 2023-12-28 09:45:56.000000 videobox-0.7.0/LICENSE
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     4406 2024-05-04 13:38:28.462661 videobox-0.7.0/PKG-INFO
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     3525 2024-05-04 07:56:48.000000 videobox-0.7.0/README.md
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763       70 2023-12-29 17:16:46.000000 videobox-0.7.0/Videobox.code-workspace
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1655 2024-05-04 07:55:45.000000 videobox-0.7.0/app.py
+drwxr-xr-x   0 andrea.peltrin (1702769464) 858591763        0 2024-05-04 13:38:28.433030 videobox-0.7.0/assets/
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     6744 2024-05-04 08:34:24.000000 videobox-0.7.0/assets/app.js
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763    14546 2024-05-04 07:59:02.000000 videobox-0.7.0/assets/app.scss
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     7842 2024-02-08 16:51:49.000000 videobox-0.7.0/assets/balloon.css
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1744 2024-05-04 07:55:45.000000 videobox-0.7.0/assets/button.scss
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     3167 2024-05-04 07:55:45.000000 videobox-0.7.0/assets/carousel.js
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1638 2024-05-04 07:55:45.000000 videobox-0.7.0/assets/carousel.scss
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     8250 2024-05-04 07:55:45.000000 videobox-0.7.0/assets/helpers.scss
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     6814 2024-02-08 16:51:49.000000 videobox-0.7.0/assets/normalize.css
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      971 2024-05-04 07:55:45.000000 videobox-0.7.0/assets/select.scss
+drwxr-xr-x   0 andrea.peltrin (1702769464) 858591763        0 2024-05-04 13:38:28.433638 videobox-0.7.0/macos/
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763    16835 2023-12-29 17:16:46.000000 videobox-0.7.0/macos/icon.png
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      538 2023-12-29 17:16:46.000000 videobox-0.7.0/macos/menubar-icon.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     2100 2024-05-04 08:34:24.000000 videobox-0.7.0/makefile
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763   131701 2024-05-04 08:34:24.000000 videobox-0.7.0/package-lock.json
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      736 2024-05-04 08:00:03.000000 videobox-0.7.0/package.json
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1241 2024-05-04 08:34:24.000000 videobox-0.7.0/pyproject.toml
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      206 2024-05-04 08:34:24.000000 videobox-0.7.0/requirements.txt
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763   192697 2024-05-04 07:55:45.000000 videobox-0.7.0/screenshot.jpg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      796 2024-05-04 07:55:45.000000 videobox-0.7.0/setup-app.py
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763       38 2024-05-04 13:38:28.463045 videobox-0.7.0/setup.cfg
+drwxr-xr-x   0 andrea.peltrin (1702769464) 858591763        0 2024-05-04 13:38:28.434726 videobox-0.7.0/tests/
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763        0 2024-05-04 07:55:45.000000 videobox-0.7.0/tests/__init__.py
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      335 2024-05-04 07:55:45.000000 videobox-0.7.0/tests/conftest.py
+drwxr-xr-x   0 andrea.peltrin (1702769464) 858591763        0 2024-05-04 13:38:28.436591 videobox-0.7.0/tests/sync/
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     2045 2024-05-04 07:55:45.000000 videobox-0.7.0/tests/sync/episodes.json
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     4494 2024-05-04 07:55:45.000000 videobox-0.7.0/tests/sync/releases.json
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      250 2024-05-04 07:55:45.000000 videobox-0.7.0/tests/sync/series-tags.json
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     2496 2024-05-04 07:55:45.000000 videobox-0.7.0/tests/sync/series.json
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      138 2024-05-04 07:55:45.000000 videobox-0.7.0/tests/sync/tags.json
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763   114073 2024-05-04 07:55:45.000000 videobox-0.7.0/tests/sync/updated.json
+-rwxr-xr-x   0 andrea.peltrin (1702769464) 858591763     2052 2024-05-04 07:55:45.000000 videobox-0.7.0/tests/test_frontend.py
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      565 2024-05-04 07:55:45.000000 videobox-0.7.0/tests/test_iso639.py
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     2108 2024-05-04 07:55:45.000000 videobox-0.7.0/tests/test_sync.py
+drwxr-xr-x   0 andrea.peltrin (1702769464) 858591763        0 2024-05-04 13:38:28.439283 videobox-0.7.0/videobox/
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     4749 2024-05-04 08:34:24.000000 videobox-0.7.0/videobox/__init__.py
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1960 2024-05-04 08:34:24.000000 videobox-0.7.0/videobox/api.py
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     2786 2024-05-04 08:03:33.000000 videobox-0.7.0/videobox/filters.py
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     2659 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/iso639.py
+drwxr-xr-x   0 andrea.peltrin (1702769464) 858591763        0 2024-05-04 13:38:28.441880 videobox-0.7.0/videobox/main/
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      183 2023-12-29 17:16:46.000000 videobox-0.7.0/videobox/main/__init__.py
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      914 2024-03-31 16:40:45.000000 videobox-0.7.0/videobox/main/announcer.py
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     6949 2024-05-04 08:03:59.000000 videobox-0.7.0/videobox/main/queries.py
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763    12015 2024-05-04 08:05:16.000000 videobox-0.7.0/videobox/main/routes.py
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763    11263 2024-05-04 08:34:24.000000 videobox-0.7.0/videobox/models.py
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763    10812 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/scraper.py
+drwxr-xr-x   0 andrea.peltrin (1702769464) 858591763        0 2024-05-04 13:38:28.455692 videobox-0.7.0/videobox/static/
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763    32534 2024-05-04 13:38:23.000000 videobox-0.7.0/videobox/static/app.css
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763    89372 2024-05-04 13:38:23.000000 videobox-0.7.0/videobox/static/app.css.map
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763   214595 2024-05-04 13:38:23.000000 videobox-0.7.0/videobox/static/app.js
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763  2237649 2024-05-04 13:38:23.000000 videobox-0.7.0/videobox/static/app.js.map
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763    34941 2023-12-29 17:16:46.000000 videobox-0.7.0/videobox/static/apple-touch-icon.png
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     8890 2023-12-29 17:16:46.000000 videobox-0.7.0/videobox/static/default-poster.png
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     4090 2023-12-29 17:16:46.000000 videobox-0.7.0/videobox/static/default-still.png
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1109 2023-12-29 17:16:46.000000 videobox-0.7.0/videobox/static/favicon.png
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      540 2023-12-29 17:16:46.000000 videobox-0.7.0/videobox/static/favicon.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      358 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/static/icon-check-bold.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      363 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/static/icon-check.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      280 2023-12-29 17:16:46.000000 videobox-0.7.0/videobox/static/icon-close-bold.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      308 2023-12-29 17:16:46.000000 videobox-0.7.0/videobox/static/icon-close.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      570 2023-12-29 17:16:46.000000 videobox-0.7.0/videobox/static/icon-grid-bold.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      576 2023-12-29 17:16:46.000000 videobox-0.7.0/videobox/static/icon-grid.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      581 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/static/icon-heart-bold.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      624 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/static/icon-heart-break-bold.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      558 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/static/icon-heart-break.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      511 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/static/icon-heart.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      785 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/static/icon-heartbeat-bold.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      765 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/static/icon-heartbeat.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      422 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/static/icon-hourglass-bold.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      445 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/static/icon-hourglass.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      372 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/static/icon-info-bold.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      372 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/static/icon-info.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      418 2023-12-29 17:16:46.000000 videobox-0.7.0/videobox/static/icon-list-bold.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      400 2023-12-29 17:16:46.000000 videobox-0.7.0/videobox/static/icon-list.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      890 2023-12-29 17:16:46.000000 videobox-0.7.0/videobox/static/icon-magnet-bold.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      863 2023-12-29 17:16:46.000000 videobox-0.7.0/videobox/static/icon-magnet.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      252 2023-12-29 17:16:46.000000 videobox-0.7.0/videobox/static/icon-search-bold.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      267 2023-12-29 17:16:46.000000 videobox-0.7.0/videobox/static/icon-search.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      431 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/static/icon-sort-asc.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      409 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/static/icon-sort-desc.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      390 2023-12-29 17:16:46.000000 videobox-0.7.0/videobox/static/icon-tag-bold.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      369 2023-12-29 17:16:46.000000 videobox-0.7.0/videobox/static/icon-tag.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      606 2023-12-29 17:16:46.000000 videobox-0.7.0/videobox/static/icon-update-bold.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      579 2023-12-29 17:16:46.000000 videobox-0.7.0/videobox/static/icon-update.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      563 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/static/icon-warning-bold.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      567 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/static/icon-warning.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      618 2023-12-29 17:16:46.000000 videobox-0.7.0/videobox/static/logo.svg
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763    12195 2024-05-04 08:34:24.000000 videobox-0.7.0/videobox/sync.py
+drwxr-xr-x   0 andrea.peltrin (1702769464) 858591763        0 2024-05-04 13:38:28.461731 videobox-0.7.0/videobox/templates/
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      319 2023-12-29 17:16:46.000000 videobox-0.7.0/videobox/templates/404.html
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      433 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/templates/_chart.html
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     3272 2023-12-29 17:16:46.000000 videobox-0.7.0/videobox/templates/_episodes-grid.html
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     3270 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/templates/_episodes-list.html
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      577 2024-05-04 08:34:24.000000 videobox-0.7.0/videobox/templates/_follow-button.html
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      497 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/templates/_following.html
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      523 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/templates/_language-card-grid.html
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      612 2024-05-04 08:09:02.000000 videobox-0.7.0/videobox/templates/_meta.html
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1773 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/templates/_release_detail.html
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763       79 2023-12-29 17:16:46.000000 videobox-0.7.0/videobox/templates/_suggest.html
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      524 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/templates/_tag-card-grid.html
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      231 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/templates/_update-done.html
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      280 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/templates/_update-progress.html
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1848 2024-05-04 08:10:07.000000 videobox-0.7.0/videobox/templates/base.html
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      588 2024-05-04 08:10:27.000000 videobox-0.7.0/videobox/templates/first-import.html
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      574 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/templates/following.html
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     5706 2024-05-04 08:11:04.000000 videobox-0.7.0/videobox/templates/home.html
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      416 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/templates/language_detail.html
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     2861 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/templates/macros.html
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     1074 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/templates/search_results.html
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     5449 2024-05-04 08:34:24.000000 videobox-0.7.0/videobox/templates/series_detail.html
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     3999 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/templates/status.html
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      421 2024-05-04 07:55:45.000000 videobox-0.7.0/videobox/templates/tag_detail.html
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      952 2024-01-30 13:25:31.000000 videobox-0.7.0/videobox/templates/tags.html
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     3238 2024-05-04 13:38:22.000000 videobox-0.7.0/videobox/trackers.txt
+drwxr-xr-x   0 andrea.peltrin (1702769464) 858591763        0 2024-05-04 13:38:28.462090 videobox-0.7.0/videobox.egg-info/
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     4406 2024-05-04 13:38:28.000000 videobox-0.7.0/videobox.egg-info/PKG-INFO
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763     3297 2024-05-04 13:38:28.000000 videobox-0.7.0/videobox.egg-info/SOURCES.txt
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763        1 2024-05-04 13:38:28.000000 videobox-0.7.0/videobox.egg-info/dependency_links.txt
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763       44 2024-05-04 13:38:28.000000 videobox-0.7.0/videobox.egg-info/entry_points.txt
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763      132 2024-05-04 13:38:28.000000 videobox-0.7.0/videobox.egg-info/requires.txt
+-rw-r--r--   0 andrea.peltrin (1702769464) 858591763        9 2024-05-04 13:38:28.000000 videobox-0.7.0/videobox.egg-info/top_level.txt
```

### Comparing `videobox-0.6.1/.gitignore` & `videobox-0.7.0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -67,7 +67,8 @@
 /site
 
 # Tracker list
 trackers.txt
 
 # NPM
 node_modules
+.parcel-cache
```

### Comparing `videobox-0.6.1/LICENSE` & `videobox-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/README.md` & `videobox-0.7.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,38 @@
+Metadata-Version: 2.1
+Name: videobox
+Version: 0.7.0
+Summary: Easy TV series download
+Author: Andrea Peltrin
+Project-URL: Homepage, https://github.com/passiomatic/videobox
+Project-URL: Bug Tracker, https://github.com/passiomatic/videobox/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Flask
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: peewee<4,>=3.15.4
+Requires-Dist: urllib3<2
+Requires-Dist: requests<3,>=2.31.0
+Requires-Dist: flask<3,>=2.3.3
+Requires-Dist: waitress<3,>=2.1.2
+Requires-Dist: tomli<3,>=2.0.1
+Requires-Dist: tomli-w<2,>=1.0.0
+Requires-Dist: chardet==5.2.0
+
 # Videobox
 
 Videobox is a Python web app that lets you discover and download the latest TV series.
 
-![The Videobox home page](https://videobox.passiomatic.com/screenshot-0.6.jpg?1)
+![The Videobox home page](screenshot.jpg)
 
 ## Prerequisites
 
 Videobox requires the Python 3 programming language to be installed on your machine. If you are not familiar with it please refer to the official Python's [download page][d] for more information. 
 
 To check if you have Python installed type the following after in your terminal prompt (`$`):
 
@@ -17,128 +43,87 @@
 
 Any Python version starting from 3.9 should run Videobox just fine. 
 
 **Note**: currently Videobox requires an external BitTorrent client ([uTorrent](https://www.utorrent.com), [Transmission](https://transmissionbt.com), etc.) to download video files.
 
 ## Installation
 
-You can install Videobox along with the main Python installation of your machine or in so-called "virtual environment", which is the recommended approach, since its dependencies may clash with packages you have already installed. [Learn more about virtual environments here][venv]. 
+You can install Videobox along with the main Python installation of your machine or in so-called "virtual environment", which is the recommended approach, since its dependencies may clash with packages you have already installed. [Learn more about virtual environments][venv]. 
 
-You install Videobox from [PyPI][2] via the Python `pip` utility. Again, type the following command in your terminal:
+Install or update Videobox from [PyPI][2] via the Python `pip` utility. Again, type the following command in your terminal:
 
 ```
-$ python -m pip install videobox
+$ python -m pip install -U videobox
 ```
 
-The install procedure will also create a `videobox` command, available in your terminal. 
-
 ## Quick start
 
-You use Videobox via its web interface. To access it you start the `videobox` command on the terminal and point your web browser to the given URL:
+You use Videobox via its web interface. To access it, start the `videobox` command on the terminal and point the web browser to the given URL:
 
 ```
 $ videobox
-Server started. Point your browser to http://0.0.0.0:8080 to use the web interface.
+Videobox has started. Point your browser to http://localhost:8080 to use the web interface.
 ```
 
-Once the page is loaded Videobox will ask you to update your library by clicking the update button 🔄.
-
-## Additional command-line options
+At startup Videobox updates its library and will attempt to do it again periodically.
 
 Add `--help` to list all the available options:
 
 ```
 $ videobox --help 
 Usage: videobox [OPTIONS]
 
 Options:
-  --host TEXT     Hostname or IP address on which to listen, default is
+  --host TEXT     Hostname or IP address on which to listen. Default is
                   0.0.0.0, which means "all IP addresses on this host".
   --port INTEGER  TCP port on which to listen, default is 8080
   --help          Show this message and exit.
 ```
 
+If your are interested in hacking the source code or contribute to the project see the [contributing document][contrib].
+
 ## Building the macOS app 
 
-If you are using a Mac you can compile Videobox into a menu bar app. 
+If you are on a Mac you can compile Videobox into a menu bar app. 
 
 First, install the necessary dependencies with:
 
 ```
 $ make install-package && make install-build-deps
 ```
 
 Then build the app with:
 
 ```
 $ make build-app
 ```
 
-If everything went fine, you will find the compiled app into the `dist` folder.
-
-The first time you run the app you will need to manually authorise it, please [follow these instructions][1].
+If everything went fine you will find the compiled app into the `dist` folder. The first time you run the app you will need to manually authorise it, please [follow these instructions][1].
 
 The build app process has been tested macOS Mojave (Intel), Ventura (arm64), and Sonoma (arm64). 
 
 
 ## Roadmap
 
 This is a rough plan of what I would like to implement in the upcoming releases:
 
-* **0.7**: Background sync.
-* **0.8**: [libtorrent][l] integration.
+* **0.8**: Support for "complete season" torrents.
+* **0.9**: [libtorrent][l] integration.
 
 ## Motivation 
 
 I've seen too many torrent web sites full of tracking scripts, pop-ups windows and crypto mining to remember. In the past years I've built a number of scripts to scrape such sites and now it's time to put all together in a coherent way. 
 
 ## Credits 
 
 [Phosphor Icons][i] created by Helena Zhang and Tobias Fried.
 
-## Contributing
-
-If you would like to help with the Videobox development these are some essential steps to get you started.
-
-### Setup the environment
-
-Starting from the repo root you might want to create a new virtual environment, to avoid messing up pre-existing Pyhton packages on your machine: 
-
-`$ make venv`
-
-And activate it:
-
-`$ source .venv/bin/activate`
-
-Then, install all project dependencies into the virtual enviroment just created:
-
-`$ make install-deps`
-
-`npm`, the Node Package Manager, is required to install `parcel` to compile CSS styles and JavaScript code:
-
-`$ npm ci && make build-assets`
-
-Finally, run the web interface in debug mode:
-
-`$ make`
-
-When you are done you can exit the virtual enviroment with the `deactivate` command.
-
-### Where to find Videobox data
-
-The Videobox Python package stores local database and configuration settings in `~/.videobox`, while the macOS app uses `~/Library/Application Support/Videobox`. 
-
-### Using the debugger with Visual Studio Code
-
-Debug works just fine under Visual Studio Code once you pick the Python interpreter shown in the `.venv` folder created earlier. 
-
-Place any breakpoint you need, hit F5 and editor will fire up the application.
-
 
 [1]: https://www.funkyspacemonkey.com/how-to-open-applications-from-anywhere-in-macos-sonoma
 [2]: https://pypi.org/project/videobox/
 [3]: https://brew.sh/
 [4]: https://flask.palletsprojects.com/en/2.2.x/cli/
 [i]: https://phosphoricons.com
 [d]: https://www.python.org/downloads/
 [l]: https://github.com/arvidn/libtorrent
 [venv]: https://docs.python.org/3/library/venv.html
+[contrib]: CONTRIBUTING.md
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `videobox-0.6.1/assets/app.scss` & `videobox-0.7.0/assets/app.scss`

 * *Files 3% similar despite different names*

```diff
@@ -23,16 +23,21 @@
 
   --color-body: #dfedf7;
   --color-muted: #a3c1d4;
   --color-background: var(--color-primary-100);
   --anchor-color: #e3ddf0;
   --anchor-color-hover: var(--color-accent-light);
   --border-color: var(--color-primary-300);
+  --border-color-accent: var(--color-accent);
   --balloon-color: var(--color-primary-400);
 
+  --color-success: #59c27c;
+  --color-warning: #f0ee78;
+  --color-danger: #cf4d4a;
+
   --font-size-sm: .875rem;
   --font-size-regular: 1rem;
   --font-size-lg: 1.25rem;
   --font-size-xlg: 2rem;
   --font-size-xxlg: 3rem;
 }
 
@@ -199,19 +204,19 @@
 .badge-480 {
   background: #269ddb;
 }
 
 .torrent-hi {}
 
 .torrent-medium {
-  color: #f0ed60;
+  color: var(--color-warning);
 }
 
 .torrent-low {
-  color: #cf4d4a;
+  color: var(--color-danger);
 }
 
 /* FORMS */
 
 fieldset {
   padding: 0;
   margin: 0;
@@ -241,16 +246,16 @@
 }
 
 .table tr:hover  {
   background-color: #253e52;
 }
 
 .report td {
-  padding: 0.5em 0 0.5em 0;
-  border-bottom: 1px solid var(--color-primary-200);
+  padding: 0.25em 2rem 0.25rem 0;
+  // border-bottom: 1px solid var(--color-primary-200);
 }
 
 .report th,
 .table th {
   padding: 0.375rem 0.5rem 0.375rem 0;
   border-bottom: 1px solid var(--color-primary-200);
   color: var(--color-muted);
@@ -571,45 +576,71 @@
   height: 100vh;
   color: var(--color-body);
   /* transition: transform .3s ease-out, opacity .3s ease-out;
   transform: translate(0%, -5%); */
   /* Reset browser defaults */
   max-width: unset;
   max-height: unset;
+  pointer-events: none;
+}
+
+dialog.in {
+  pointer-events: auto;
+  opacity: 1;
+  transition: opacity .3s ease-out;  
+}
+
+dialog.out {
+  opacity: 0;  
+  /* Wait 2s before disappear */
+  transition: opacity .3s ease-out 2s;
 }
 
+
 .dialog-body {
   width: 30rem;
   background: var(--color-primary-200);
   padding: 2rem;
   border-radius: 1rem;
 }
 
 .dialog-body--small {
   width: 16rem;
 }
 
+// .dialog-body--toast {
+//   position: absolute;
+//   top: 1.5rem;
+//   right: 1.5rem;
+//   width: 16rem;
+//   z-index: 10;
+//   background: var(--color-primary-200);
+//   padding: 1rem;
+//   border-radius: .5rem;
+// }
+
 dialog:modal {
   display: flex;
   align-items: center;
   justify-content: center;
   opacity: 1;
+  pointer-events: auto;
   /* transform: translate(0%, 0%); */
 }
 
 dialog::backdrop {
   background: rgba(21, 29, 39, .75);
 }
 
-dialog button[name="close"] {
+/* dialog button[name="close"] {
   position: absolute;
   top: 0;
   right: 0;
   z-index: 1;
-}
+} */
 
 /* Animations  */
 
 .anim-spin {
   animation-name: spin;
   animation-duration: 4s;
   animation-iteration-count: infinite;
@@ -742,8 +773,14 @@
   border: 0;  
 }
 
 /* Progress  */
 
 progress {
   accent-color: var(--color-accent-light);
+}
+
+/* Chart  */
+
+.chart {
+  max-width: 100%;
 }
```

### Comparing `videobox-0.6.1/assets/balloon.css` & `videobox-0.7.0/assets/balloon.css`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/assets/button.scss` & `videobox-0.7.0/assets/button.scss`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/assets/carousel.js` & `videobox-0.7.0/assets/carousel.js`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/assets/carousel.scss` & `videobox-0.7.0/assets/carousel.scss`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/assets/helpers.scss` & `videobox-0.7.0/assets/helpers.scss`

 * *Files 2% similar despite different names*

```diff
@@ -350,14 +350,18 @@
   font-weight: 900;
 }
 
 .font-style-italic {
   font-style: italic;
 }
 
+.font-small-caps {
+  font-variant: all-small-caps;
+}
+
 .line-height-1 {
   line-height: 1;
 }
 
 .text-decoration-none {
   text-decoration: none;
 }
@@ -410,14 +414,18 @@
 
 // Border 
 
 .border {
   border: 1px solid var(--border-color);
 }
 
+.border-accent {
+  border: 1px solid var(--border-color-accent);
+}
+
 .border-top {
   border-top: 1px solid var(--color-primary-300);
 }
 
 .border-bottom {
   border-bottom: 1px solid var(--color-primary-300);
 }
```

### Comparing `videobox-0.6.1/assets/normalize.css` & `videobox-0.7.0/assets/normalize.css`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/assets/select.scss` & `videobox-0.7.0/assets/select.scss`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/macos/icon.png` & `videobox-0.7.0/macos/icon.png`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/macos/menubar-icon.svg` & `videobox-0.7.0/macos/menubar-icon.svg`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/makefile` & `videobox-0.7.0/makefile`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-default: run
+default: run-debug
 
 # Env. setup
 
 venv:
 	python3 -m venv .venv
 
 install-deps: trackers
@@ -15,15 +15,16 @@
 	pip install -e .
 
 # CSS/JS
 
 watch-assets:
 	npm run watch 
 
-build-assets:
+build-assets: clean
+	rm -r .parcel-cache
 	npm run build
 
 # PyPI support 
 
 build: clean trackers build-assets
 	python -m build
 
@@ -41,32 +42,44 @@
 
 clean:
 	rm -rf dist build
 
 # Development
 
 run:
-	flask --app videobox --debug run 
+	flask --app videobox run
+
+# Disable hot reloader since it multiplies Flask instaces and their threads
+run-debug: 
+	flask --app videobox --debug run --no-reload --with-threads
 
 run-waitress:
 	waitress-serve --host 127.0.0.1 --port 5000 --threads=8 --call videobox:create_app
 
 reset:
 	rm ~/.videobox/library.db
 
 shell:
 	flask --app videobox shell
 
 sql:
 	sqlite3 ~/.videobox/library.db
 
-# macOS app build
+# Tests
+
+create-test-data: export FLASK_DATABASE_URL=sqlite:///tests/library-test.db
 
-build-app-alias: clean build-icon build-assets
-	python setup-app.py py2app -A	
+create-test-data:
+	cp ~/.videobox/library.db ./tests/library-test.db
+	sqlite3 ./tests/library-test.db ".dump" > tests/test-data.sql
+
+test:
+	python -m pytest -s
+
+# macOS app build
 
 build-app: clean build-icon build-assets
 	python setup-app.py py2app
 	open ./dist
 
 run-app:
 	./dist/Videobox.app/Contents/MacOS/Videobox
```

### Comparing `videobox-0.6.1/package-lock.json` & `videobox-0.7.0/package-lock.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9983921568627452%*

 * *Differences: {"'packages'": "{'': {'dependencies': OrderedDict([('chart.js', '4.4.2'), "*

 * *               "('chartjs-adapter-dayjs-4', '1.0.4'), ('dayjs', '1.11.9')])}, "*

 * *               "'node_modules/@kurkle/color': OrderedDict([('version', '0.3.2'), ('resolved', "*

 * *               "'https://registry.npmjs.org/@kurkle/color/-/color-0.3.2.tgz'), ('integrity', "*

 * *               "'sha512-fuscdXJ9G1qb7W8VdHi+IwRqij3lBkosAm4ydQtEmbY58OzHXqQhvlxqEkoz0yssNVn38bcpRWgA9PP+OGoisw==')]), "*

 * *               "'node_modules/chart.js': Orde […]*

```diff
@@ -1,12 +1,17 @@
 {
     "lockfileVersion": 3,
     "name": "videobox",
     "packages": {
         "": {
+            "dependencies": {
+                "chart.js": "4.4.2",
+                "chartjs-adapter-dayjs-4": "1.0.4",
+                "dayjs": "1.11.9"
+            },
             "devDependencies": {
                 "@parcel/transformer-sass": "^2.11.0",
                 "parcel": "^2.11.0"
             },
             "license": "ISC",
             "name": "videobox",
             "version": "0.0.0"
@@ -167,14 +172,19 @@
             "engines": {
                 "node": ">=4"
             },
             "integrity": "sha512-QjVjwdXIt408MIiAqCX4oUKsgU2EqAGzs2Ppkm4aQYbjm+ZEWEcW4SfFNTr4uMNZma0ey4f5lgLrkB0aX0QMow==",
             "resolved": "https://registry.npmjs.org/supports-color/-/supports-color-5.5.0.tgz",
             "version": "5.5.0"
         },
+        "node_modules/@kurkle/color": {
+            "integrity": "sha512-fuscdXJ9G1qb7W8VdHi+IwRqij3lBkosAm4ydQtEmbY58OzHXqQhvlxqEkoz0yssNVn38bcpRWgA9PP+OGoisw==",
+            "resolved": "https://registry.npmjs.org/@kurkle/color/-/color-0.3.2.tgz",
+            "version": "0.3.2"
+        },
         "node_modules/@lezer/common": {
             "dev": true,
             "integrity": "sha512-V+GqBsga5+cQJMfM0GdnHmg4DgWvLzgMWjbldBg0+jC3k9Gu6nJNZDLJxXEBT1Xj8KhRN4jmbC5CY7SIL++sVw==",
             "resolved": "https://registry.npmjs.org/@lezer/common/-/common-1.1.2.tgz",
             "version": "1.1.2"
         },
         "node_modules/@lezer/lr": {
@@ -2255,14 +2265,37 @@
             "funding": {
                 "url": "https://github.com/chalk/chalk?sponsor=1"
             },
             "integrity": "sha512-oKnbhFyRIXpUuez8iBMmyEa4nbj4IOQyuhc/wy9kY7/WVPcwIO9VA668Pu8RkO7+0G76SLROeyw9CpQ061i4mA==",
             "resolved": "https://registry.npmjs.org/chalk/-/chalk-4.1.2.tgz",
             "version": "4.1.2"
         },
+        "node_modules/chart.js": {
+            "dependencies": {
+                "@kurkle/color": "^0.3.0"
+            },
+            "engines": {
+                "pnpm": ">=8"
+            },
+            "integrity": "sha512-6GD7iKwFpP5kbSD4MeRRRlTnQvxfQREy36uEtm1hzHzcOqwWx0YEHuspuoNlslu+nciLIB7fjjsHkUv/FzFcOg==",
+            "resolved": "https://registry.npmjs.org/chart.js/-/chart.js-4.4.2.tgz",
+            "version": "4.4.2"
+        },
+        "node_modules/chartjs-adapter-dayjs-4": {
+            "engines": {
+                "node": ">=10"
+            },
+            "integrity": "sha512-yy9BAYW4aNzPVrCWZetbILegTRb7HokhgospPoC3b5iZ5qdlqNmXts2KdSp6AqnjkPAp/YWyHDxLvIvwt5x81w==",
+            "peerDependencies": {
+                "chart.js": ">=4.0.1",
+                "dayjs": "^1.9.7"
+            },
+            "resolved": "https://registry.npmjs.org/chartjs-adapter-dayjs-4/-/chartjs-adapter-dayjs-4-1.0.4.tgz",
+            "version": "1.0.4"
+        },
         "node_modules/chokidar": {
             "dependencies": {
                 "anymatch": "~3.1.2",
                 "braces": "~3.0.2",
                 "glob-parent": "~5.1.2",
                 "is-binary-path": "~2.1.0",
                 "is-glob": "~4.0.1",
@@ -2512,14 +2545,19 @@
             "dev": true,
             "integrity": "sha512-aylIc7Z9y4yzHYAJNuESG3hfhC+0Ibp/MAMiaOZgNv4pmEdFyfZhhhny4MNiAfWdBQ1RQ2mfDWmM1x8SvGyp8g==",
             "optional": true,
             "peer": true,
             "resolved": "https://registry.npmjs.org/mdn-data/-/mdn-data-2.0.28.tgz",
             "version": "2.0.28"
         },
+        "node_modules/dayjs": {
+            "integrity": "sha512-QvzAURSbQ0pKdIye2txOzNaHmxtUBXerpY0FJsFXUMKbIZeFm5ht1LS/jFsrncjnmtv8HsG0W2g6c0zUjZWmpA==",
+            "resolved": "https://registry.npmjs.org/dayjs/-/dayjs-1.11.9.tgz",
+            "version": "1.11.9"
+        },
         "node_modules/detect-libc": {
             "bin": {
                 "detect-libc": "bin/detect-libc.js"
             },
             "dev": true,
             "engines": {
                 "node": ">=0.10"
```

### Comparing `videobox-0.6.1/package.json` & `videobox-0.7.0/package.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'dependencies'": "OrderedDict([('chart.js', '4.4.2'), ('chartjs-adapter-dayjs-4', '1.0.4'), "*

 * *                   "('dayjs', '1.11.9')])"}*

```diff
@@ -1,12 +1,17 @@
 {
     "author": "",
     "bugs": {
         "url": "https://github.com/passiomatic/videobox/issues"
     },
+    "dependencies": {
+        "chart.js": "4.4.2",
+        "chartjs-adapter-dayjs-4": "1.0.4",
+        "dayjs": "1.11.9"
+    },
     "description": "",
     "devDependencies": {
         "@parcel/transformer-sass": "^2.11.0",
         "parcel": "^2.11.0"
     },
     "homepage": "https://github.com/passiomatic/videobox#readme",
     "license": "ISC",
```

### Comparing `videobox-0.6.1/pyproject.toml` & `videobox-0.7.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "videobox"
-version = "0.6.1"
+dynamic = ["version"]
 authors = [
   { name="Andrea Peltrin" },
 ]
-description = "TV series download web app"
+description = "Easy TV series download"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
   "peewee >= 3.15.4,<4",
   "urllib3<2",
   "requests >= 2.31.0,<3",
   "flask >= 2.3.3,<3",
@@ -39,10 +39,13 @@
 
 [tool.setuptools]
 packages = ["videobox", "videobox.main"]
 
 [tool.setuptools.package-data]
 videobox = ["trackers.txt", "static/*.*", "templates/*.*"]
 
+[tool.setuptools.dynamic]
+version = {attr = "videobox.__version__"}
+
 [tools.py2app.bundle.main]
 build-type = "standalone"
 arch = "universal2"
```

### Comparing `videobox-0.6.1/setup-app.py` & `videobox-0.7.0/setup-app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup
+import videobox
 
 APP = ['app.py']
 DATA_FILES = ['macos/menubar-icon.svg']
 OPTIONS = {
-    # List here specific app packages, skipping those in pyproject.toml
+    # List here specific app packages, in addition tp those in pyproject.toml
     'packages': ['rumps', 'videobox'],
     # Copy these files outside the app bundle lib/python39.zip archive
     'resources': ['./videobox/templates', './videobox/static'], 
     # Tweak app Info.plist file
     'plist': {
         'CFBundleIdentifier': 'com.passiomatic.videobox',
         'LSUIElement': True,
-        'CFBundleShortVersionString': '0.6.1',
+        'CFBundleShortVersionString': videobox.__version__,
         'NSHumanReadableCopyright': '© Andrea Peltrin'
     },
     'iconfile': 'build/icon.icns'
 }
 
 setup(
     name='Videobox',
```

### Comparing `videobox-0.6.1/videobox/api.py` & `videobox-0.7.0/videobox/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,71 @@
 import requests
 from flask import current_app
+from urllib.parse import urljoin
 import videobox
 
 TIMEOUT = 10
 API_VERSION = 3
-API_ENDPOINT_URL = f"https://www.videobox.passiomatic.com/{API_VERSION}"
-USER_AGENT = f"Videobox/{videobox.__version__} (https://videobox.passiomatic.com/)"
+DEFAULT_API_BASE_URL = "https://www.videobox.passiomatic.com/"
+USER_AGENT = f"Videobox/{videobox.__version__} (https://pypi.org/project/videobox/)"
 
 # Full import
 
 
 def get_all_tags(client_id):
-    return get_url(f"{API_ENDPOINT_URL}/tags/all?client={client_id}")
+    return get_url(f"{API_VERSION}/tags/all?client={client_id}")
 
 
 def get_all_series(client_id):
-    return get_url(f"{API_ENDPOINT_URL}/series/all?client={client_id}")
+    return get_url(f"{API_VERSION}/series/all?client={client_id}")
 
 
 def get_all_series_tags(client_id):
-    return get_url(f"{API_ENDPOINT_URL}/series-tags/all?client={client_id}")
+    return get_url(f"{API_VERSION}/series-tags/all?client={client_id}")
 
 
 def get_all_episodes(client_id):
-    return get_url(f"{API_ENDPOINT_URL}/episodes/all?client={client_id}")
+    return get_url(f"{API_VERSION}/episodes/all?client={client_id}")
 
 
 def get_all_releases(client_id):
-    return get_url(f"{API_ENDPOINT_URL}/releases/all?client={client_id}")
+    return get_url(f"{API_VERSION}/releases/all?client={client_id}")
 
 
 # Sync
 
 
 def get_updated_series(client_id, since):
-    return get_url(f"{API_ENDPOINT_URL}/series/updated?since={int(since.timestamp())}&client={client_id}")
+    return get_url(f"{API_VERSION}/series/updated?since={int(since.timestamp())}&client={client_id}")
 
 
 def get_tags_with_ids(client_id, ids):
-    return get_url(f"{API_ENDPOINT_URL}/tags?ids={make_ids(ids)}&client={client_id}")
+    return get_url(f"{API_VERSION}/tags?ids={make_ids(ids)}&client={client_id}")
 
 
 def get_series_with_ids(client_id, ids):
-    return get_url(f"{API_ENDPOINT_URL}/series?ids={make_ids(ids)}&client={client_id}")
+    return get_url(f"{API_VERSION}/series?ids={make_ids(ids)}&client={client_id}")
 
 
 def get_series_tags_for_ids(client_id, ids):
-    return get_url(f"{API_ENDPOINT_URL}/series-tags?ids={make_ids(ids)}&client={client_id}")
+    return get_url(f"{API_VERSION}/series-tags?ids={make_ids(ids)}&client={client_id}")
 
 
 def get_episodes_with_ids(client_id, ids):
-    return get_url(f"{API_ENDPOINT_URL}/episodes?ids={make_ids(ids)}&client={client_id}")
+    return get_url(f"{API_VERSION}/episodes?ids={make_ids(ids)}&client={client_id}")
 
 
 def get_releases_with_ids(client_id, ids):
-    return get_url(f"{API_ENDPOINT_URL}/releases?ids={make_ids(ids)}&client={client_id}")
+    return get_url(f"{API_VERSION}/releases?ids={make_ids(ids)}&client={client_id}")
 
 
 def make_ids(ids):
     return ",".join(map(str, ids))
 
 
-def get_url(url):
+def get_url(path):
     request_headers = {
         'User-Agent': USER_AGENT
     }
+    url = urljoin(current_app.config.get('API_BASE_URL', DEFAULT_API_BASE_URL), path)
     current_app.logger.debug(f"Quering API endpoint {url}...")
     return requests.get(url, timeout=TIMEOUT, headers=request_headers)
```

### Comparing `videobox-0.6.1/videobox/filters.py` & `videobox-0.7.0/videobox/filters.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 '''
 Custom Jinja Filters
 '''
 import operator
 import itertools
-from datetime import datetime
-from videobox import languages
+from urllib.parse import urlparse
+from datetime import datetime, timezone
+from videobox import iso639
 
 MIN_SEEDERS = 1
 
 def human_date(value):
     return value.strftime("%b %d, %Y")
 
 def timeline_date(value):
@@ -22,15 +23,16 @@
 
 def datetime_since(since_value, current_value):
     """
     Returns string representing "time since" e.g.
     3 days ago, 5 hours ago etc.
     """
 
-    diff = current_value - since_value
+    # Make sure we are comparing two TZ-aware values
+    diff = current_value.replace(tzinfo=timezone.utc) - since_value.replace(tzinfo=timezone.utc)
 
     periods = (
         (diff.days // 365, "year", "years"),
         (diff.days // 30, "month", "months"),
         (diff.days // 7, "week", "weeks"),
         (diff.days, "day", "days"),
         (diff.seconds // 3600, "hour", "hours"),
@@ -40,14 +42,28 @@
 
     for period, singular, plural in periods:
         if period:
             return "%d %s ago" % (period, singular if period == 1 else plural)
 
     return "just now"
 
+# def timedelta(days):
+#     periods = (
+#         (days // 365, "year", "years"),
+#         (days // 30, "month", "months"),
+#         (days // 7, "week", "weeks"),
+#         (days // 1, "day", "days"),
+#     )
+
+#     for period, singular, plural in periods:
+#         if period:
+#             return "in %d %s" % (period, singular if period == 1 else plural)
+
+#     return "later today"
+    
 def islice(iterable, stop):
     return itertools.islice(iterable, stop)
 
 def groupby_attrs(iterable, attr, *attrs):
     return itertools.groupby(iterable, key=operator.attrgetter(attr, *attrs))
 
 def networks(value):
@@ -63,31 +79,38 @@
         color = "low"
     elif 4 <= value < 7:
         color = "medium"
     return f'<span class="torrent-{color}">{value}</span>'
 
 def lang(code):
     try:
-        return languages.LANGUAGES[code]
+        return iso639.LANGUAGES_SET_1[code]
     except KeyError:
         return ''
 
 def pluralize(prefix, value):
     return f"{prefix}{'s' if value > 1 else ''}"
 
+
+def nice_url(value): 
+    pieces = urlparse(value)
+    return pieces.netloc 
+
 FILTERS = [
     human_date,
     timeline_date,
     human_date_time,
     torrent_health,
     networks,
     lang,
     islice,
     groupby_attrs,
     to_date,
     datetime_since,
-    pluralize
+    #timedelta,
+    pluralize,
+    nice_url,
 ]
 
 def init_app(app):
     for func in FILTERS:
         app.add_template_filter(func)
```

### Comparing `videobox-0.6.1/videobox/main/queries.py` & `videobox-0.7.0/videobox/main/queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import operator
 from functools import reduce
-from datetime import datetime, date, timedelta
+from datetime import datetime, date, timedelta, timezone
 from peewee import fn
 from videobox.models import Series, Episode, Release, Tag, SeriesTag, SeriesIndex, TAG_GENRE
 
 MAX_SEASONS = 2
 
 def get_series_tags(series):
     return (Tag
@@ -35,41 +35,41 @@
     return (SeriesAlias.select(SeriesAlias.id, fn.Max(Episode.season).alias("max_season"))
             .join(Episode)
             .group_by(SeriesAlias.id))
 
 
 def get_featured_series(exclude_ids, days_interval):
     series_subquery = get_series_subquery()
-    return (Series.select(Series, fn.SUM(Release.completed).alias('total_completed'))
+    return (Series.select(Series, fn.Sum(Release.completed).alias('total_completed'))
             .join(Episode)
             .join(Release)
             .join(series_subquery, on=(
                 series_subquery.c.id == Series.id))
             # Consider episodes from last season only and releases within interval days
             .where(~(Series.id << exclude_ids) & 
                    (Episode.season == series_subquery.c.max_season) &
                    (Release.added_on > (date.today() - timedelta(days=days_interval))))
             .group_by(Series)
-            .order_by(fn.SUM(Release.completed).desc())
+            .order_by(fn.Sum(Release.completed).desc())
             )
 
 
 def get_today_series():
     series_subquery = get_series_subquery()
     return (Series.select(Series, Episode, fn.SUM(Release.completed).alias('total_completed'))
             .join(Episode)
             .join(Release)
             .join(series_subquery, on=(
                 series_subquery.c.id == Series.id))
             # Consider episodes from last season only and releases within the past 24h
             .where((Episode.season == series_subquery.c.max_season) &
                    (Episode.thumbnail_url != '') &
                    # @@TODO do not user current time, figure out max added_on and compute from it
-                   (Release.added_on > (datetime.utcnow() - timedelta(hours=24))))
-            .order_by(fn.SUM(Release.completed).desc())
+                   (Release.added_on > (datetime.now(timezone.utc) - timedelta(hours=24))))
+            .order_by(fn.Sum(Release.completed).desc())
             .group_by(Series.id)
             #.get_or_none()
             .limit(10)
             )
 
 def get_followed_series(days=None):
     series_subquery = get_series_subquery()
```

### Comparing `videobox-0.6.1/videobox/main/routes.py` & `videobox-0.7.0/videobox/main/routes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from datetime import datetime, date
+from datetime import datetime, date, timezone
 from operator import attrgetter
 from itertools import groupby
-import queue
 import flask
-from flask import current_app as app
+# from flask import current_app as app
 from peewee import fn, JOIN
 from playhouse.flask_utils import PaginatedQuery, get_object_or_404
 import videobox
 import videobox.models as models
-from videobox.models import Series, Episode, Release, Tag, SeriesTag, SyncLog
-import videobox.sync as sync
+from videobox.models import Series, Episode, Release, Tag, SeriesTag, SyncLog, Tracker
 from . import bp
+from .announcer import announcer
 from . import queries
 
-MAX_TOP_TAGS = 10
-MAX_SEASONS = 2
+MAX_CHART_DAYS = 30 
+MAX_TOP_TAGS = 8
 MIN_SEEDERS = 1
-MAX_LOG_ROWS = 20
+MAX_SEASONS = 2
+MAX_LOG_ROWS = 3
 SERIES_CARDS_PER_PAGE = 6 * 10
 SERIES_EPISODES_PER_PAGE = 30
 RESOLUTION_OPTIONS = {
     0: "Any",
     480: "480p",
     720: "720p (HD)",
     1080: "1080p (Full HD)",
@@ -32,15 +32,14 @@
     "desc": "Largest",
 }
 
 
 @bp.context_processor
 def inject_template_vars():
     return {
-        "last_sync": models.get_last_log(),
         "version": videobox.__version__
     }
 
 
 @bp.errorhandler(404)
 def page_not_found(e):
     return flask.render_template('404.html'), 404
@@ -51,56 +50,62 @@
 # ---------
 
 last_server_alert = ''
 
 @bp.route('/')
 def home():
     total_series, total_episodes, total_releases = queries.get_library_stats()
-    if total_series:        
-        utc_now = datetime.utcnow()
+    # Make sure library is already filled with data
+    if total_series and total_episodes and total_releases:        
+        last_sync = models.get_last_log()
+        utc_now = datetime.now(timezone.utc)
         today_series = queries.get_today_series()
         # Do not exlude any series for now
         exclude_ids = []
         featured_series = queries.get_featured_series(exclude_ids=exclude_ids, days_interval=2).limit(8)
-        top_tags = queries.get_nav_tags(8)    
+        top_tags = queries.get_nav_tags(MAX_TOP_TAGS)    
         # Show updates within the last week
         followed_series = queries.get_followed_series(days=7)
         return flask.render_template("home.html", 
+                                     last_sync=last_sync,
                                      utc_now=utc_now,
                                      server_alert=last_server_alert,
                                      today_series=today_series,
                                      featured_series=featured_series, 
                                      top_tags=top_tags,
                                      total_series=total_series,
-                                     #total_episodes=total_episodes,
                                      total_releases=total_releases,
                                      followed_series=followed_series)
     else:
         return flask.render_template("first-import.html")
 
 # ---------
 # Search
 # ---------
 
 
 @bp.route('/search')
 def search():
     query = flask.request.args.get("query")
+    if not query:
+        flask.abort(400)
     series_ids = [series.rowid for series in queries.search_series(
         sanitize_query(query))]
     series = queries.get_series_with_ids(series_ids)
     # @@TODO
     # if len(series) == 1:
     #     # Single match, display series detail page
     return flask.render_template("search_results.html", found_series=series, search_query=query)
 
 
 @bp.route('/suggest')
 def suggest():
     query = flask.request.args.get("query")
+    if not query:
+        flask.abort(400)
     sanitized_query = sanitize_query(query)
     search_suggestions = queries.suggest_series(sanitized_query).limit(10)
     return flask.render_template("_suggest.html", search_suggestions=search_suggestions)
 
 
 # ---------
 # Tag
@@ -148,62 +153,66 @@
 
 @bp.route('/series/<int:series_id>')
 def series_detail(series_id):
     #resolution = flask.request.args.get("resolution", type=int, default=0) or flask.request.cookies.get('resolution', type=int, default=0)
     resolution = flask.request.args.get("resolution", type=int, default=0)
     #size_sorting = flask.request.args.get("size", default="") or flask.request.cookies.get('size', default="")
     size_sorting = flask.request.args.get("size", default="")
+    episode_sorting = flask.request.args.get("episode", default="asc")
     view_layout = flask.request.args.get("view", default="grid")
     today = date.today()
     series = get_object_or_404(Series, (Series.id == series_id))
     series_subquery = queries.get_series_subquery()
     release_cte = queries.release_cte(resolution, size_sorting)
     if resolution or size_sorting:
         episodes_query = (Episode.select(Episode, Release.id, Release.name, Release.magnet_uri, Release.resolution, Release.size, Release.seeders, Release.last_updated_on)
                           .join(Release)
                           .switch(Episode)
                           .join(Series)
                           .join(series_subquery, on=(
                               series_subquery.c.id == Series.id))
                           .join(release_cte, on=(Release.id == release_cte.c.release_id))
                           .where((Episode.series == series.id) &
+                                 #(Release.seeders >= MIN_SEEDERS) &
                                  # Episodes from last 2 seasons only
-                                 (series_subquery.c.max_season - Episode.season < MAX_SEASONS) &
-                                 (Episode.aired_on != None)
+                                 (series_subquery.c.max_season - Episode.season < MAX_SEASONS) 
+                                 #& (Episode.aired_on != None)
                                  )
-                          .order_by(Episode.season.desc(), Episode.number)
+                          .order_by(Episode.season.desc(), Episode.number if episode_sorting == "asc" else Episode.number.desc())
                           .with_cte(release_cte))
     else:
         # Unfiltered
         episodes_query = (Episode.select(Episode, Release.id, Release.name, Release.magnet_uri, Release.resolution, Release.size, Release.seeders, Release.last_updated_on)
                           .join(Release, JOIN.LEFT_OUTER)
                           .switch(Episode)
                           .join(Series)
                           .join(series_subquery, on=(
                               series_subquery.c.id == Series.id))
                           .where((Episode.series == series.id) &
+                                 #(Release.seeders >= MIN_SEEDERS) &
                                  # Episodes from last 2 seasons only
-                                 (series_subquery.c.max_season - Episode.season < MAX_SEASONS) &
-                                 (Episode.aired_on != None)
+                                 (series_subquery.c.max_season - Episode.season < MAX_SEASONS) 
+                                 # & (Episode.aired_on != None)
                                  )
-                          .order_by(Episode.season.desc(), Episode.number, Release.seeders.desc()))
+                          .order_by(Episode.season.desc(), Episode.number if episode_sorting == "asc" else Episode.number.desc(), Release.seeders.desc()))
 
     # Group by season number
     seasons_episodes = groupby(episodes_query, key=attrgetter('season'))
     series_tags = queries.get_series_tags(series) 
 
     response = flask.make_response(flask.render_template("series_detail.html", 
                                                          series=series, 
                                                          series_tags=series_tags, 
                                                          seasons_episodes=seasons_episodes, 
                                                          today=today, 
                                                          resolution=resolution, 
                                                          resolution_options=RESOLUTION_OPTIONS, 
                                                          size=size_sorting, 
                                                          size_options=SIZE_OPTIONS,
+                                                         episode_sorting=episode_sorting,
                                                          view_layout=view_layout))
     # Remember filters across requests
     if resolution:
         response.set_cookie('resolution', str(resolution))
     if size_sorting:
         response.set_cookie('size', size_sorting)    
     return response
@@ -217,117 +226,60 @@
     series.save()
 
     # Toggle button
     return flask.render_template("_follow-button.html", series=series)
 
 @bp.route('/release/<int:release_id>')
 def release_detail(release_id):
-    utc_now = datetime.utcnow()
     release = get_object_or_404(Release, (Release.id == release_id))
-    return flask.render_template("_release_detail.html", utc_now=utc_now, release=release)
+    return flask.render_template("_release_detail.html", utc_now=datetime.now(timezone.utc), release=release)
 
 
 @bp.route('/following')
 def following():
     page = flask.request.args.get("page", 1, type=int)
     query = queries.get_followed_series()
     paginated_series = PaginatedQuery(query, paginate_by=SERIES_EPISODES_PER_PAGE, page_var="page")
     if page == 1:
         return flask.render_template("following.html", paginated_series=paginated_series, page=page)
     else:
         # For async requests
         return flask.render_template("_following.html", paginated_series=paginated_series, page=page)
-        
-
     
 # ---------
-# Update database
+# Sync database
 # ---------
 
-close_message = object()
-
-class MessageAnnouncer(object):
-    """
-    Server-sent events in Flask without extra dependencies.
-    See https://maxhalford.github.io/blog/flask-sse-no-deps/
-    """
-
-    def __init__(self):
-        self.listeners = []
-
-    def listen(self):
-        q = queue.Queue(maxsize=5)
-        self.listeners.append(q)
-        return q
-
-    def format_sse(self, data, event=None):
-        msg = f'data: {data}\n\n'
-        if event:
-            msg = f'event: {event}\n{msg}'
-        return msg
-
-    def announce(self, msg):
-        for i in reversed(range(len(self.listeners))):
-            try:
-                self.listeners[i].put_nowait(msg)
-            except queue.Full:
-                del self.listeners[i]
-
-
-announcer = MessageAnnouncer()
-sync_worker = None
-
-@bp.route('/update')
-def update():
-
-    @flask.copy_current_request_context
-    def on_update_progress(message, percent=0):
-        data = flask.render_template(
-            "_update-dialog.html", message=message, percent=percent)
-        msg = announcer.format_sse(data=data, event='updating')
-        announcer.announce(msg)
-
-    @flask.copy_current_request_context
-    def on_update_done(message, alert):
-        data = flask.render_template(
-            "_update-dialog-done.html", message=message, percent=100)
-        msg = announcer.format_sse(data=data, event='done')
-        announcer.announce(msg)
-        announcer.announce(close_message)
-        global last_server_alert
-        last_server_alert = alert
-
-    global sync_worker 
-    if sync_worker and sync_worker.is_alive():
-        app.logger.warning("Sync is already running, request ignored")
-    else:
-        sync_worker = sync.SyncWorker(
-            app.config["API_CLIENT_ID"], progress_callback=on_update_progress, done_callback=on_update_done)
-        sync_worker.start()
-
-    return {}, 200
-
-@bp.route('/update-events')
-def update_events():    
+@bp.route('/sync/events')
+def sync_events():    
     def stream():
-        # Returns a queue.Queue
+        # Return a message queue
         messages = announcer.listen()
         while True:
             # Blocks until a new message arrives
             msg = messages.get()
-            if msg is close_message:
+            if announcer.is_close_message(msg):
                 break
             yield msg
     return flask.Response(stream(), mimetype='text/event-stream')
 
+# ---------
+# System status
+# ---------
 
-@bp.route('/update/history')
-def update_history():
+@bp.route('/status')
+def system_status():
     log_rows = SyncLog.select().order_by(SyncLog.timestamp.desc()).limit(MAX_LOG_ROWS)
-    return flask.render_template("log.html", log_rows=log_rows, max_log_rows=MAX_LOG_ROWS)
+    chart_query = Release.raw(f'SELECT DATE(added_on) AS release_date, COUNT(id) AS release_count FROM `release` GROUP BY release_date ORDER BY release_date DESC LIMIT {MAX_CHART_DAYS}')
+    # Filter out trackers that will likely never reply correctly
+    trackers = Tracker.select().where((Tracker.status << models.TRACKERS_ALIVE)).order_by(Tracker.status, Tracker.url)
+    max_last_scraped_on = Tracker.select(fn.Max(Tracker.last_scraped_on).alias("max_last_scraped_on")).where((Tracker.status << [models.TRACKER_OK, models.TRACKER_TIMED_OUT])).scalar()
+    return flask.render_template("status.html", 
+                                 log_rows=log_rows, trackers=trackers, chart=chart_query, max_chart_days=MAX_CHART_DAYS, max_log_rows=MAX_LOG_ROWS, max_last_scraped_on=max_last_scraped_on)
+
 
 # ---------
 # Helpers
 # ---------
 
 def sanitize_query(query):
     # https://www.sqlite.org/fts5.html
```

### Comparing `videobox-0.6.1/videobox/static/app.css` & `videobox-0.7.0/videobox/static/app.css`

 * *Files 1% similar despite different names*

```diff
@@ -1,3 +1,3 @@
 /*! normalize.css v8.0.1 | MIT License | github.com/necolas/normalize.css */
-html{-webkit-text-size-adjust:100%;line-height:1.15}body{margin:0}main{display:block}h1{margin:.67em 0;font-size:2em}hr{box-sizing:content-box;height:0;overflow:visible}pre{font-family:monospace;font-size:1em}a{background-color:#0000}abbr[title]{border-bottom:none;-webkit-text-decoration:underline dotted;text-decoration:underline dotted}b,strong{font-weight:bolder}code,kbd,samp{font-family:monospace;font-size:1em}small{font-size:80%}sub,sup{vertical-align:baseline;font-size:75%;line-height:0;position:relative}sub{bottom:-.25em}sup{top:-.5em}img{border-style:none}button,input,optgroup,select,textarea{margin:0;font-family:inherit;font-size:100%;line-height:1.15}button,input{overflow:visible}button,select{text-transform:none}button,[type=button],[type=reset],[type=submit]{-webkit-appearance:button}button::-moz-focus-inner{border-style:none;padding:0}[type=button]::-moz-focus-inner{border-style:none;padding:0}[type=reset]::-moz-focus-inner{border-style:none;padding:0}[type=submit]::-moz-focus-inner{border-style:none;padding:0}button:-moz-focusring{outline:1px dotted ButtonText}[type=button]:-moz-focusring{outline:1px dotted ButtonText}[type=reset]:-moz-focusring{outline:1px dotted ButtonText}[type=submit]:-moz-focusring{outline:1px dotted ButtonText}fieldset{padding:.35em .75em .625em}legend{box-sizing:border-box;color:inherit;white-space:normal;max-width:100%;padding:0;display:table}progress{vertical-align:baseline}textarea{overflow:auto}[type=checkbox],[type=radio]{box-sizing:border-box;padding:0}[type=number]::-webkit-inner-spin-button{height:auto}[type=number]::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}[type=search]::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}details{display:block}summary{display:list-item}template,[hidden]{display:none}:root{--balloon-border-radius:2px;--balloon-color:#101010f2;--balloon-text-color:#fff;--balloon-font-size:12px;--balloon-move:4px}button[aria-label][data-balloon-pos]{overflow:visible}[aria-label][data-balloon-pos]{cursor:pointer;position:relative}[aria-label][data-balloon-pos]:after{opacity:0;pointer-events:none;text-indent:0;text-shadow:none;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Oxygen,Ubuntu,Cantarell,Open Sans,Helvetica Neue,sans-serif;font-style:normal;font-weight:400;font-size:var(--balloon-font-size);background:var(--balloon-color);color:var(--balloon-text-color);border-radius:2px;border-radius:var(--balloon-border-radius);content:attr(aria-label);white-space:nowrap;z-index:10;padding:.5em 1em;transition:all .18s ease-out .18s;position:absolute}[aria-label][data-balloon-pos]:before{border:5px solid #0000;border-top-color:var(--balloon-color);opacity:0;pointer-events:none;content:"";z-index:10;width:0;height:0;transition:all .18s ease-out .18s;position:absolute}[aria-label][data-balloon-pos]:hover:before,[aria-label][data-balloon-pos]:hover:after,[aria-label][data-balloon-pos][data-balloon-visible]:before,[aria-label][data-balloon-pos][data-balloon-visible]:after,[aria-label][data-balloon-pos]:not([data-balloon-nofocus]):focus:before,[aria-label][data-balloon-pos]:not([data-balloon-nofocus]):focus:after{opacity:1;pointer-events:none}[aria-label][data-balloon-pos].font-awesome:after{font-family:FontAwesome,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Oxygen,Ubuntu,Cantarell,Open Sans,Helvetica Neue,sans-serif}[aria-label][data-balloon-pos][data-balloon-break]:after{white-space:pre}[aria-label][data-balloon-pos][data-balloon-break][data-balloon-length]:after{white-space:pre-line;word-break:break-word}[aria-label][data-balloon-pos][data-balloon-blunt]:before,[aria-label][data-balloon-pos][data-balloon-blunt]:after{transition:none}[aria-label][data-balloon-pos][data-balloon-pos=up]:hover:after,[aria-label][data-balloon-pos][data-balloon-pos=up][data-balloon-visible]:after,[aria-label][data-balloon-pos][data-balloon-pos=down]:hover:after,[aria-label][data-balloon-pos][data-balloon-pos=down][data-balloon-visible]:after,[aria-label][data-balloon-pos][data-balloon-pos=up]:hover:before,[aria-label][data-balloon-pos][data-balloon-pos=up][data-balloon-visible]:before,[aria-label][data-balloon-pos][data-balloon-pos=down]:hover:before,[aria-label][data-balloon-pos][data-balloon-pos=down][data-balloon-visible]:before{transform:translate(-50%)}[aria-label][data-balloon-pos][data-balloon-pos*=-left]:after{left:0}[aria-label][data-balloon-pos][data-balloon-pos*=-left]:before{left:5px}[aria-label][data-balloon-pos][data-balloon-pos*=-right]:after{right:0}[aria-label][data-balloon-pos][data-balloon-pos*=-right]:before{right:5px}[aria-label][data-balloon-pos][data-balloon-pos*=-left]:hover:after,[aria-label][data-balloon-pos][data-balloon-pos*=-left][data-balloon-visible]:after,[aria-label][data-balloon-pos][data-balloon-pos*=-right]:hover:after,[aria-label][data-balloon-pos][data-balloon-pos*=-right][data-balloon-visible]:after,[aria-label][data-balloon-pos][data-balloon-pos*=-left]:hover:before,[aria-label][data-balloon-pos][data-balloon-pos*=-left][data-balloon-visible]:before,[aria-label][data-balloon-pos][data-balloon-pos*=-right]:hover:before,[aria-label][data-balloon-pos][data-balloon-pos*=-right][data-balloon-visible]:before{transform:translate(0)}[aria-label][data-balloon-pos][data-balloon-pos^=up]:before,[aria-label][data-balloon-pos][data-balloon-pos^=up]:after{transform-origin:top;transform:translate(0,var(--balloon-move));bottom:100%}[aria-label][data-balloon-pos][data-balloon-pos^=up]:after{margin-bottom:10px}[aria-label][data-balloon-pos][data-balloon-pos=up]:before,[aria-label][data-balloon-pos][data-balloon-pos=up]:after{transform:translate(-50%,var(--balloon-move));left:50%}[aria-label][data-balloon-pos][data-balloon-pos^=down]:before,[aria-label][data-balloon-pos][data-balloon-pos^=down]:after{transform:translate(0,calc(var(--balloon-move)*-1));top:100%}[aria-label][data-balloon-pos][data-balloon-pos^=down]:after{margin-top:10px}[aria-label][data-balloon-pos][data-balloon-pos^=down]:before{border:5px solid #0000;border-bottom-color:var(--balloon-color);width:0;height:0}[aria-label][data-balloon-pos][data-balloon-pos=down]:after,[aria-label][data-balloon-pos][data-balloon-pos=down]:before{transform:translate(-50%,calc(var(--balloon-move)*-1));left:50%}[aria-label][data-balloon-pos][data-balloon-pos=left]:hover:after,[aria-label][data-balloon-pos][data-balloon-pos=left][data-balloon-visible]:after,[aria-label][data-balloon-pos][data-balloon-pos=right]:hover:after,[aria-label][data-balloon-pos][data-balloon-pos=right][data-balloon-visible]:after,[aria-label][data-balloon-pos][data-balloon-pos=left]:hover:before,[aria-label][data-balloon-pos][data-balloon-pos=left][data-balloon-visible]:before,[aria-label][data-balloon-pos][data-balloon-pos=right]:hover:before,[aria-label][data-balloon-pos][data-balloon-pos=right][data-balloon-visible]:before{transform:translateY(-50%)}[aria-label][data-balloon-pos][data-balloon-pos=left]:after,[aria-label][data-balloon-pos][data-balloon-pos=left]:before{transform:translate(var(--balloon-move),-50%);top:50%;right:100%}[aria-label][data-balloon-pos][data-balloon-pos=left]:after{margin-right:10px}[aria-label][data-balloon-pos][data-balloon-pos=left]:before{border:5px solid #0000;border-left-color:var(--balloon-color);width:0;height:0}[aria-label][data-balloon-pos][data-balloon-pos=right]:after,[aria-label][data-balloon-pos][data-balloon-pos=right]:before{transform:translate(calc(var(--balloon-move)*-1),-50%);top:50%;left:100%}[aria-label][data-balloon-pos][data-balloon-pos=right]:after{margin-left:10px}[aria-label][data-balloon-pos][data-balloon-pos=right]:before{border:5px solid #0000;border-right-color:var(--balloon-color);width:0;height:0}[aria-label][data-balloon-pos][data-balloon-length]:after{white-space:normal}[aria-label][data-balloon-pos][data-balloon-length=small]:after{width:80px}[aria-label][data-balloon-pos][data-balloon-length=medium]:after{width:150px}[aria-label][data-balloon-pos][data-balloon-length=large]:after{width:260px}[aria-label][data-balloon-pos][data-balloon-length=xlarge]:after{width:380px}@media screen and (width<=768px){[aria-label][data-balloon-pos][data-balloon-length=xlarge]:after{width:90vw}}[aria-label][data-balloon-pos][data-balloon-length=fit]:after{width:100%}:root{--color-primary:#489fd9;--color-primary-light:#abd9f7;--color-primary-400:#3d7da9;--color-primary-300:#315d7c;--color-primary-200:#253e52;--color-primary-100:#151d24;--color-accent:#e37dd7;--color-accent-light:#f794d5;--color-accent-400:#b163a8;--color-accent-300:#824b7b;--color-accent-200:#563351;--color-accent-100:#2d1d2a;--color-body:#dfedf7;--color-muted:#a3c1d4;--color-background:var(--color-primary-100);--anchor-color:#e3ddf0;--anchor-color-hover:var(--color-accent-light);--border-color:var(--color-primary-300);--balloon-color:var(--color-primary-400);--font-size-sm:.875rem;--font-size-regular:1rem;--font-size-lg:1.25rem;--font-size-xlg:2rem;--font-size-xxlg:3rem}.d-none{display:none!important}.d-inline{display:inline!important}.d-inline-block{display:inline-block!important}.d-block{display:block!important}.d-table{display:table!important}.d-table-row{display:table-row!important}.d-table-cell{display:table-cell!important}.d-flex{display:flex!important}.d-inline-flex{display:inline-flex!important}@media (width>=768px){.d-md-none{display:none!important}.d-md-inline{display:inline!important}.d-md-inline-block{display:inline-block!important}.d-md-block{display:block!important}.d-md-table{display:table!important}.d-md-table-row{display:table-row!important}.d-md-table-cell{display:table-cell!important}.d-md-flex{display:flex!important}.d-md-inline-flex{display:inline-flex!important}}.m-0{margin:0!important}.mt-0,.my-0{margin-top:0!important}.mr-0,.mx-0{margin-right:0!important}.mb-0,.my-0{margin-bottom:0!important}.ml-0,.mx-0{margin-left:0!important}.m-1{margin:.25rem!important}.mt-1,.my-1{margin-top:.25rem!important}.mr-1,.mx-1{margin-right:.25rem!important}.mb-1,.my-1{margin-bottom:.25rem!important}.ml-1,.mx-1{margin-left:.25rem!important}.m-2{margin:.5rem!important}.mt-2,.my-2{margin-top:.5rem!important}.mr-2,.mx-2{margin-right:.5rem!important}.mb-2,.my-2{margin-bottom:.5rem!important}.ml-2,.mx-2{margin-left:.5rem!important}.m-3{margin:1rem!important}.mt-3,.my-3{margin-top:1rem!important}.mr-3,.mx-3{margin-right:1rem!important}.mb-3,.my-3{margin-bottom:1rem!important}.ml-3,.mx-3{margin-left:1rem!important}.m-4{margin:1.5rem!important}.mt-4,.my-4{margin-top:1.5rem!important}.mr-4,.mx-4{margin-right:1.5rem!important}.mb-4,.my-4{margin-bottom:1.5rem!important}.ml-4,.mx-4{margin-left:1.5rem!important}.m-5{margin:2.5rem!important}.mt-5,.my-5{margin-top:2.5rem!important}.mr-5,.mx-5{margin-right:2.5rem!important}.mb-5,.my-5{margin-bottom:2.5rem!important}.ml-5,.mx-5{margin-left:2.5rem!important}.p-0{padding:0!important}.pt-0,.py-0{padding-top:0!important}.pr-0,.px-0{padding-right:0!important}.pb-0,.py-0{padding-bottom:0!important}.pl-0,.px-0{padding-left:0!important}.p-1{padding:.25rem!important}.pt-1,.py-1{padding-top:.25rem!important}.pr-1,.px-1{padding-right:.25rem!important}.pb-1,.py-1{padding-bottom:.25rem!important}.pl-1,.px-1{padding-left:.25rem!important}.p-2{padding:.5rem!important}.pt-2,.py-2{padding-top:.5rem!important}.pr-2,.px-2{padding-right:.5rem!important}.pb-2,.py-2{padding-bottom:.5rem!important}.pl-2,.px-2{padding-left:.5rem!important}.p-3{padding:1rem!important}.pt-3,.py-3{padding-top:1rem!important}.pr-3,.px-3{padding-right:1rem!important}.pb-3,.py-3{padding-bottom:1rem!important}.pl-3,.px-3{padding-left:1rem!important}.p-4{padding:1.5rem!important}.pt-4,.py-4{padding-top:1.5rem!important}.pr-4,.px-4{padding-right:1.5rem!important}.pb-4,.py-4{padding-bottom:1.5rem!important}.pl-4,.px-4{padding-left:1.5rem!important}.p-5{padding:2.5rem!important}.pt-5,.py-5{padding-top:2.5rem!important}.pr-5,.px-5{padding-right:2.5rem!important}.pb-5,.py-5{padding-bottom:2.5rem!important}.pl-5,.px-5{padding-left:2.5rem!important}.m-n1{margin:-.25rem!important}.mt-n1,.my-n1{margin-top:-.25rem!important}.mr-n1,.mx-n1{margin-right:-.25rem!important}.mb-n1,.my-n1{margin-bottom:-.25rem!important}.ml-n1,.mx-n1{margin-left:-.25rem!important}.m-n2{margin:-.5rem!important}.mt-n2,.my-n2{margin-top:-.5rem!important}.mr-n2,.mx-n2{margin-right:-.5rem!important}.mb-n2,.my-n2{margin-bottom:-.5rem!important}.ml-n2,.mx-n2{margin-left:-.5rem!important}.m-n3{margin:-1rem!important}.mt-n3,.my-n3{margin-top:-1rem!important}.mr-n3,.mx-n3{margin-right:-1rem!important}.mb-n3,.my-n3{margin-bottom:-1rem!important}.ml-n3,.mx-n3{margin-left:-1rem!important}.m-n4{margin:-1.5rem!important}.mt-n4,.my-n4{margin-top:-1.5rem!important}.mr-n4,.mx-n4{margin-right:-1.5rem!important}.mb-n4,.my-n4{margin-bottom:-1.5rem!important}.ml-n4,.mx-n4{margin-left:-1.5rem!important}.m-n5{margin:-2.5rem!important}.mt-n5,.my-n5{margin-top:-2.5rem!important}.mr-n5,.mx-n5{margin-right:-2.5rem!important}.mb-n5,.my-n5{margin-bottom:-2.5rem!important}.ml-n5,.mx-n5{margin-left:-2.5rem!important}.m-auto{margin:auto!important}.mt-auto,.my-auto{margin-top:auto!important}.mr-auto,.mx-auto{margin-right:auto!important}.mb-auto,.my-auto{margin-bottom:auto!important}.ml-auto,.mx-auto{margin-left:auto!important}@media (width>=768px){.m-md-0{margin:0!important}.mt-md-0,.my-md-0{margin-top:0!important}.mr-md-0,.mx-md-0{margin-right:0!important}.mb-md-0,.my-md-0{margin-bottom:0!important}.ml-md-0,.mx-md-0{margin-left:0!important}.m-md-1{margin:.25rem!important}.mt-md-1,.my-md-1{margin-top:.25rem!important}.mr-md-1,.mx-md-1{margin-right:.25rem!important}.mb-md-1,.my-md-1{margin-bottom:.25rem!important}.ml-md-1,.mx-md-1{margin-left:.25rem!important}.m-md-2{margin:.5rem!important}.mt-md-2,.my-md-2{margin-top:.5rem!important}.mr-md-2,.mx-md-2{margin-right:.5rem!important}.mb-md-2,.my-md-2{margin-bottom:.5rem!important}.ml-md-2,.mx-md-2{margin-left:.5rem!important}.m-md-3{margin:1rem!important}.mt-md-3,.my-md-3{margin-top:1rem!important}.mr-md-3,.mx-md-3{margin-right:1rem!important}.mb-md-3,.my-md-3{margin-bottom:1rem!important}.ml-md-3,.mx-md-3{margin-left:1rem!important}.m-md-4{margin:1.5rem!important}.mt-md-4,.my-md-4{margin-top:1.5rem!important}.mr-md-4,.mx-md-4{margin-right:1.5rem!important}.mb-md-4,.my-md-4{margin-bottom:1.5rem!important}.ml-md-4,.mx-md-4{margin-left:1.5rem!important}.m-md-5{margin:2.5rem!important}.mt-md-5,.my-md-5{margin-top:2.5rem!important}.mr-md-5,.mx-md-5{margin-right:2.5rem!important}.mb-md-5,.my-md-5{margin-bottom:2.5rem!important}.ml-md-5,.mx-md-5{margin-left:2.5rem!important}.p-md-0{padding:0!important}.pt-md-0,.py-md-0{padding-top:0!important}.pr-md-0,.px-md-0{padding-right:0!important}.pb-md-0,.py-md-0{padding-bottom:0!important}.pl-md-0,.px-md-0{padding-left:0!important}.p-md-1{padding:.25rem!important}.pt-md-1,.py-md-1{padding-top:.25rem!important}.pr-md-1,.px-md-1{padding-right:.25rem!important}.pb-md-1,.py-md-1{padding-bottom:.25rem!important}.pl-md-1,.px-md-1{padding-left:.25rem!important}.p-md-2{padding:.5rem!important}.pt-md-2,.py-md-2{padding-top:.5rem!important}.pr-md-2,.px-md-2{padding-right:.5rem!important}.pb-md-2,.py-md-2{padding-bottom:.5rem!important}.pl-md-2,.px-md-2{padding-left:.5rem!important}.p-md-3{padding:1rem!important}.pt-md-3,.py-md-3{padding-top:1rem!important}.pr-md-3,.px-md-3{padding-right:1rem!important}.pb-md-3,.py-md-3{padding-bottom:1rem!important}.pl-md-3,.px-md-3{padding-left:1rem!important}.p-md-4{padding:1.5rem!important}.pt-md-4,.py-md-4{padding-top:1.5rem!important}.pr-md-4,.px-md-4{padding-right:1.5rem!important}.pb-md-4,.py-md-4{padding-bottom:1.5rem!important}.pl-md-4,.px-md-4{padding-left:1.5rem!important}.p-md-5{padding:2.5rem!important}.pt-md-5,.py-md-5{padding-top:2.5rem!important}.pr-md-5,.px-md-5{padding-right:2.5rem!important}.pb-md-5,.py-md-5{padding-bottom:2.5rem!important}.pl-md-5,.px-md-5{padding-left:2.5rem!important}.m-md-n1{margin:-.25rem!important}.mt-md-n1,.my-md-n1{margin-top:-.25rem!important}.mr-md-n1,.mx-md-n1{margin-right:-.25rem!important}.mb-md-n1,.my-md-n1{margin-bottom:-.25rem!important}.ml-md-n1,.mx-md-n1{margin-left:-.25rem!important}.m-md-n2{margin:-.5rem!important}.mt-md-n2,.my-md-n2{margin-top:-.5rem!important}.mr-md-n2,.mx-md-n2{margin-right:-.5rem!important}.mb-md-n2,.my-md-n2{margin-bottom:-.5rem!important}.ml-md-n2,.mx-md-n2{margin-left:-.5rem!important}.m-md-n3{margin:-1rem!important}.mt-md-n3,.my-md-n3{margin-top:-1rem!important}.mr-md-n3,.mx-md-n3{margin-right:-1rem!important}.mb-md-n3,.my-md-n3{margin-bottom:-1rem!important}.ml-md-n3,.mx-md-n3{margin-left:-1rem!important}.m-md-n4{margin:-1.5rem!important}.mt-md-n4,.my-md-n4{margin-top:-1.5rem!important}.mr-md-n4,.mx-md-n4{margin-right:-1.5rem!important}.mb-md-n4,.my-md-n4{margin-bottom:-1.5rem!important}.ml-md-n4,.mx-md-n4{margin-left:-1.5rem!important}.m-md-n5{margin:-2.5rem!important}.mt-md-n5,.my-md-n5{margin-top:-2.5rem!important}.mr-md-n5,.mx-md-n5{margin-right:-2.5rem!important}.mb-md-n5,.my-md-n5{margin-bottom:-2.5rem!important}.ml-md-n5,.mx-md-n5{margin-left:-2.5rem!important}.m-md-auto{margin:auto!important}.mt-md-auto,.my-md-auto{margin-top:auto!important}.mr-md-auto,.mx-md-auto{margin-right:auto!important}.mb-md-auto,.my-md-auto{margin-bottom:auto!important}.ml-md-auto,.mx-md-auto{margin-left:auto!important}}.flex-row{flex-direction:row!important}.flex-column{flex-direction:column!important}.flex-row-reverse{flex-direction:row-reverse!important}.flex-column-reverse{flex-direction:column-reverse!important}.flex-wrap{flex-wrap:wrap!important}.flex-nowrap{flex-wrap:nowrap!important}.flex-wrap-reverse{flex-wrap:wrap-reverse!important}.flex-fill{flex:auto!important}.flex-grow-0{flex-grow:0!important}.flex-grow-1{flex-grow:1!important}.flex-shrink-0{flex-shrink:0!important}.flex-shrink-1{flex-shrink:1!important}.justify-content-start{justify-content:flex-start!important}.justify-content-end{justify-content:flex-end!important}.justify-content-center{justify-content:center!important}.justify-content-between{justify-content:space-between!important}.justify-content-around{justify-content:space-around!important}.align-items-start{align-items:flex-start!important}.align-items-end{align-items:flex-end!important}.align-items-center{align-items:center!important}.align-items-baseline{align-items:baseline!important}.align-items-stretch{align-items:stretch!important}.align-content-start{align-content:flex-start!important}.align-content-end{align-content:flex-end!important}.align-content-center{align-content:center!important}.align-content-between{align-content:space-between!important}.align-content-around{align-content:space-around!important}.align-content-stretch{align-content:stretch!important}.align-self-auto{align-self:auto!important}.align-self-start{align-self:flex-start!important}.align-self-end{align-self:flex-end!important}.align-self-center{align-self:center!important}.align-self-baseline{align-self:baseline!important}.align-self-stretch{align-self:stretch!important}@media (width>=768px){.flex-md-row{flex-direction:row!important}.flex-md-column{flex-direction:column!important}.flex-md-row-reverse{flex-direction:row-reverse!important}.flex-md-column-reverse{flex-direction:column-reverse!important}.flex-md-wrap{flex-wrap:wrap!important}.flex-md-nowrap{flex-wrap:nowrap!important}.flex-md-wrap-reverse{flex-wrap:wrap-reverse!important}.flex-md-fill{flex:auto!important}.flex-md-grow-0{flex-grow:0!important}.flex-md-grow-1{flex-grow:1!important}.flex-md-shrink-0{flex-shrink:0!important}.flex-md-shrink-1{flex-shrink:1!important}.justify-content-md-start{justify-content:flex-start!important}.justify-content-md-end{justify-content:flex-end!important}.justify-content-md-center{justify-content:center!important}.justify-content-md-between{justify-content:space-between!important}.justify-content-md-around{justify-content:space-around!important}.align-items-md-start{align-items:flex-start!important}.align-items-md-end{align-items:flex-end!important}.align-items-md-center{align-items:center!important}.align-items-md-baseline{align-items:baseline!important}.align-items-md-stretch{align-items:stretch!important}.align-content-md-start{align-content:flex-start!important}.align-content-md-end{align-content:flex-end!important}.align-content-md-center{align-content:center!important}.align-content-md-between{align-content:space-between!important}.align-content-md-around{align-content:space-around!important}.align-content-md-stretch{align-content:stretch!important}.align-self-md-auto{align-self:auto!important}.align-self-md-start{align-self:flex-start!important}.align-self-md-end{align-self:flex-end!important}.align-self-md-center{align-self:center!important}.align-self-md-baseline{align-self:baseline!important}.align-self-md-stretch{align-self:stretch!important}}small,.text-sm{font-size:var(--font-size-sm)!important}.text-regular{font-size:var(--font-size-regular)!important}.text-lg{font-size:var(--font-size-lg)!important}.text-xlg{font-size:var(--font-size-xlg)!important}.text-right{text-align:right}.text-left{text-align:left}.text-center{text-align:center}.text-muted{color:var(--color-muted)!important}.text-uppercase{text-transform:uppercase}.font-weight-normal{font-weight:400}.font-weight-bold{font-weight:700}.font-weight-semibold{font-weight:600}.font-weight-black{font-weight:900}.font-style-italic{font-style:italic}.line-height-1{line-height:1}.text-decoration-none{text-decoration:none}.text-break-all{word-break:break-all}.text-nowrap{white-space:nowrap}.position-relative{position:relative}.img-fluid{max-width:100%;height:auto}.zero{margin:0;padding:0}.invisible{visibility:hidden}.h-100{height:100%}.w-100{width:100%}.d-grid{grid-auto-columns:1fr;grid-auto-flow:column;display:grid}.rounded{border-radius:.5rem}.border{border:1px solid var(--border-color)}.border-top{border-top:1px solid var(--color-primary-300)}.border-bottom{border-bottom:1px solid var(--color-primary-300)}.border-right{border-right:1px solid var(--color-primary-300)}.border-left{border-left:1px solid var(--color-primary-300)}.carousel{margin:0 -3rem;position:relative}.carousel__items{scroll-behavior:smooth;-webkit-overflow-scrolling:touch;scroll-snap-type:x mandatory;scroll-snap-align:start;scrollbar-width:none;-ms-overflow-style:none;gap:2rem;width:100%;display:flex;overflow-x:scroll}.carousel-item{flex-shrink:0;max-width:300px}.carousel-item:first-child{padding-left:3rem}.carousel-item:last-child{padding-right:3rem}.carousel__items::-webkit-scrollbar{display:none}.carousel__next,.carousel__prev{z-index:1;position:absolute;top:calc(50% - 12px);left:0}.carousel__next{left:unset;right:0}.btn{text-transform:uppercase;font-size:var(--font-size-sm);letter-spacing:.05rem;cursor:pointer;background:var(--color-background);border:2px solid var(--color-primary-400);color:var(--color-primary-light);border-radius:.5rem;padding:.75rem;font-weight:700;transition:border-color .1s ease-in}.btn-small{text-transform:uppercase;font-size:var(--font-size-sm);cursor:pointer;background:var(--color-background);border:2px solid var(--color-primary-400);color:var(--color-primary-light);border-radius:.5rem;padding:.5rem;font-weight:700}.btn-small:hover,.btn:hover{border-color:var(--anchor-color-hover);color:var(--anchor-color-hover)}.btn img,.btn-small img{filter:invert(77%)sepia(40%)saturate(250%)hue-rotate(164deg)brightness()contrast(94%)}.btn:hover img,.btn-small:hover img{filter:invert(85%)sepia(46%)saturate(3508%)hue-rotate(287deg)brightness(112%)contrast(94%)}.btn-text{color:inherit;font-size:inherit;cursor:pointer;background:0 0;border:0;margin:0;padding:0;transition:color .1s ease-in}.btn-text:hover{color:var(--anchor-color-hover)!important}.btn-icon{cursor:pointer;color:inherit;background:0 0;border:0;align-items:center;transition:color .1s ease-in;display:inline-flex}select{border:2px solid var(--color-primary-400);color:var(--color-primary-light);font-size:var(--font-size-sm);appearance:none;background:var(--color-background)url("data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='100' height='100' fill='%233d8fa9'><polygon points='0,0 100,0 50,50'/></svg>") no-repeat;background-position:right .75em top 65%;background-repeat:no-repeat;background-size:12px;border-radius:.5rem;min-width:20ch;padding:.5rem 2rem .5rem .5rem}select:focus-visible{border:2px solid var(--anchor-color-hover);color:var(--anchor-color-hover);outline:none}h1,h2,h3,h4,h5,h6,p{margin:0}body{color:var(--color-body);background-color:var(--color-background);font:1rem/1.5 system-ui,sans-serif;display:flex}h1,h2,h3,h4,h5,h6{line-height:1.1}a{color:inherit;transition:color .1s ease-in}a:hover{color:var(--anchor-color-hover)}a:visited{-webkit-text-decoration:none;text-decoration:none}:target{color:var(--anchor-color-hover)}code{font-family:ui-monospace,Menlo,Monaco,Courier New,monospace}hr{border-top:1px solid var(--border-color);border-bottom:0}dt{font-size:var(--font-size-sm);text-transform:uppercase;color:var(--color-muted);font-weight:600}dd{font-size:var(--font-size-sm);margin:0 0 1rem}.badge{color:var(--color-muted);background-color:var(--color-primary-300);border-radius:.5rem;padding:.1875rem .375rem;text-decoration:none}.badge--outline{border:2px solid var(--color-primary-300);color:var(--color-muted);border-radius:.5rem;padding:.1875rem .375rem;text-decoration:none;transition:border-color .1s ease-in}.badge--outline:hover{border-color:var(--anchor-color-hover)}.badge--pill{border-radius:1rem}.badge-res{background:var(--color-primary-200);color:#fff;text-shadow:1px 1px #4d5078;border-radius:4px;padding:0 3px;font-size:12px}.badge-2160{background:#b82927}.badge-1080{background:#e0560b}.badge-720{background:var(--color-accent)}.badge-480{background:#269ddb}.torrent-medium{color:#f0ed60}.torrent-low{color:#cf4d4a}fieldset{border:0;margin:0;padding:0}legend{font-size:var(--font-size-sm);text-transform:uppercase;color:var(--color-muted);font-weight:600}.report,.table{border-collapse:collapse}.table td{padding:.1875rem .5rem .1875rem 0}.table tr{transition:background-color .1s ease-out}.table tr:hover{background-color:#253e52}.report td{border-bottom:1px solid var(--color-primary-200);padding:.5em 0}.report th,.table th{border-bottom:1px solid var(--color-primary-200);color:var(--color-muted);text-transform:uppercase;font-weight:600;font-size:var(--font-size-sm);padding:.375rem .5rem .375rem 0}@media screen and (width>=768px){.card-series{max-width:10rem}}.card-series__image{aspect-ratio:500/750;border:2px solid var(--color-primary-200);box-shadow:var(--color-primary-200)0 0;background-color:var(--color-accent-200);background-position:0 0;background-image:linear-gradient(125deg,var(--color-accent-400)25%,transparent 25%);transition:transform .2s ease-out,filter .3s ease-out,box-shadow .2s ease-out}a:hover .card-series__image{filter:brightness(1.25);box-shadow:var(--color-primary-200)7px 7px;transform:translate(-7px,-7px)}.search-query{width:min-content;position:relative}.search-query input{background:var(--color-background);border:2px solid var(--color-primary-400);color:var(--color-primary-light);font-size:var(--font-size-lg);border-radius:.5rem;padding:.75rem .5rem}.search-query input::-webkit-calendar-picker-indicator{display:none!important}@media screen and (width>=768px){.search-query input{width:30rem}}.search-query input:focus-visible{border:2px solid var(--anchor-color-hover);outline:none}input::placeholder{color:var(--color-primary-300)}.search-query button{z-index:1;background:var(--color-background);cursor:pointer;font-size:var(--font-size-lg);background:0 0;border:0;padding:.75rem;position:absolute;top:0;right:0}a:hover .card-episode__poster,a:hover .card-episode__image,.btn-text:hover .card-episode__image{border-color:var(--color-accent);transition:border-color .1s ease-in}.header .btn-icon:hover{background-color:var(--color-primary-300);transition:background-color .2s ease-out}.header{background:var(--color-primary-200);flex-direction:column;gap:.5rem;height:100vh;display:flex;position:sticky;top:0}.header .btn-icon{padding:.75rem}.icon,.header .btn-icon img{filter:invert(88%)sepia(3%)saturate(2496%)hue-rotate(185deg)brightness(106%)contrast(94%)}.header .btn-icon:hover img{filter:invert(78%)sepia(13%)saturate(3097%)hue-rotate(274deg)brightness(96%)contrast(85%)}@media screen and (width>=768px){.header{align-items:center}nav{background:0 0}}main{flex-grow:1;padding:3rem}.footer{color:var(--color-muted)}aside{flex-shrink:0;flex-basis:14rem}.main-column{flex-grow:1}.card-episode{position:relative}.card-episode__image{aspect-ratio:300/170;border:2px solid var(--color-primary-300);background-position:0 0;background-color:var(--color-accent-200);background-image:linear-gradient(125deg,var(--color-accent-400)25%,transparent 25%);transition:transform .2s ease-out,filter .3s ease-out,box-shadow .2s ease-out}.card-episode__poster{z-index:1;border:2px solid var(--color-primary-300);max-width:75px;position:absolute;bottom:-1rem;right:1rem}.series-poster__image{aspect-ratio:500/750;border:2px solid var(--color-primary-200);background-position:0 0;background-color:var(--color-accent-200);background-image:linear-gradient(125deg,var(--color-accent-400)25%,transparent 25%)}@media screen and (width>=768px){.series-poster__image{box-shadow:var(--color-primary-200)7px 7px}}.episode-grid{grid-template-rows:auto;grid-template-columns:repeat(4,1fr);gap:2rem;display:grid}.episode-grid__cell{max-width:300px}.body-copy,.series-overview{max-width:75ch}.fanart{background-blend-mode:multiply;background-position:top;background-repeat:no-repeat;background-size:cover;background-attachment:fixed;background-color:var(--color-accent-100);margin-top:-3rem;margin-left:-3rem;margin-right:-3rem;padding:3rem}@media screen and (width>=768px){.top-series-grid{grid-template-columns:repeat(2,1fr);gap:2rem;display:grid}}.cards-grid{grid-template-columns:repeat(3,1fr);gap:1.5rem;margin-bottom:2rem;display:grid}@media screen and (width>=768px){.cards-grid{grid-template-columns:repeat(6,1fr);gap:2rem}}dialog{opacity:0;color:var(--color-body);max-width:unset;max-height:unset;background:0 0;border:0;width:100vw;height:100vh;margin:0;padding:0}.dialog-body{background:var(--color-primary-200);border-radius:1rem;width:30rem;padding:2rem}.dialog-body--small{width:16rem}dialog:modal{opacity:1;justify-content:center;align-items:center;display:flex}dialog::backdrop{background:#151d27bf}dialog button[name=close]{z-index:1;position:absolute;top:0;right:0}.anim-spin{animation-name:spin;animation-duration:4s;animation-timing-function:linear;animation-iteration-count:infinite}@keyframes spin{0%{transform:rotate(0)}to{transform:rotate(360deg)}}.sr-only{white-space:nowrap;clip:rect(0 0 0 0);clip-path:inset(50%);border:0;width:1px;height:1px;margin:-1px;padding:0;position:absolute;overflow:hidden}.skip-nav a{width:1px;height:1px;position:absolute;top:auto;left:-9999px;overflow:hidden}.skip-nav a:focus{width:auto;height:auto;position:static}.mobile-carousel{gap:1.5rem;display:flex}@media screen and (width<=767.98px){.mobile-carousel{scroll-behavior:smooth;-webkit-overflow-scrolling:touch;scroll-snap-type:x mandatory;margin:0 -1rem 0 0;display:flex;overflow-x:scroll}.mobile-carousel>.mobile-carousel__item{scroll-snap-align:start;flex-shrink:0;flex-basis:50vw}.mobile-carousel::-webkit-scrollbar{display:none}}@media screen and (width>=768px){.mobile-carousel{gap:2rem}}.radio-button-group{border:2px solid var(--color-primary-400);color:var(--color-primary-light);font-size:var(--font-size-sm);background-color:var(--color-primary-100);border-radius:.5rem;display:flex}.radio-button-group__label{color:var(--color-body);cursor:pointer;background-color:#0000;border-radius:.4rem;align-items:center;padding:.5rem;display:inline-flex}.radio-button-group__label:has(input:checked){background-color:var(--color-primary-300)}.radio-button-group__input{clip:rect(0,0,0,0);white-space:nowrap;border:0;width:1px;height:1px;padding:0;position:absolute;overflow:hidden}progress{accent-color:var(--color-accent-light)}
+html{-webkit-text-size-adjust:100%;line-height:1.15}body{margin:0}main{display:block}h1{margin:.67em 0;font-size:2em}hr{box-sizing:content-box;height:0;overflow:visible}pre{font-family:monospace;font-size:1em}a{background-color:#0000}abbr[title]{border-bottom:none;-webkit-text-decoration:underline dotted;text-decoration:underline dotted}b,strong{font-weight:bolder}code,kbd,samp{font-family:monospace;font-size:1em}small{font-size:80%}sub,sup{vertical-align:baseline;font-size:75%;line-height:0;position:relative}sub{bottom:-.25em}sup{top:-.5em}img{border-style:none}button,input,optgroup,select,textarea{margin:0;font-family:inherit;font-size:100%;line-height:1.15}button,input{overflow:visible}button,select{text-transform:none}button,[type=button],[type=reset],[type=submit]{-webkit-appearance:button}button::-moz-focus-inner{border-style:none;padding:0}[type=button]::-moz-focus-inner{border-style:none;padding:0}[type=reset]::-moz-focus-inner{border-style:none;padding:0}[type=submit]::-moz-focus-inner{border-style:none;padding:0}button:-moz-focusring{outline:1px dotted ButtonText}[type=button]:-moz-focusring{outline:1px dotted ButtonText}[type=reset]:-moz-focusring{outline:1px dotted ButtonText}[type=submit]:-moz-focusring{outline:1px dotted ButtonText}fieldset{padding:.35em .75em .625em}legend{box-sizing:border-box;color:inherit;white-space:normal;max-width:100%;padding:0;display:table}progress{vertical-align:baseline}textarea{overflow:auto}[type=checkbox],[type=radio]{box-sizing:border-box;padding:0}[type=number]::-webkit-inner-spin-button{height:auto}[type=number]::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}[type=search]::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}details{display:block}summary{display:list-item}template,[hidden]{display:none}:root{--balloon-border-radius:2px;--balloon-color:#101010f2;--balloon-text-color:#fff;--balloon-font-size:12px;--balloon-move:4px}button[aria-label][data-balloon-pos]{overflow:visible}[aria-label][data-balloon-pos]{cursor:pointer;position:relative}[aria-label][data-balloon-pos]:after{opacity:0;pointer-events:none;text-indent:0;text-shadow:none;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Oxygen,Ubuntu,Cantarell,Open Sans,Helvetica Neue,sans-serif;font-style:normal;font-weight:400;font-size:var(--balloon-font-size);background:var(--balloon-color);color:var(--balloon-text-color);border-radius:2px;border-radius:var(--balloon-border-radius);content:attr(aria-label);white-space:nowrap;z-index:10;padding:.5em 1em;transition:all .18s ease-out .18s;position:absolute}[aria-label][data-balloon-pos]:before{border:5px solid #0000;border-top-color:var(--balloon-color);opacity:0;pointer-events:none;content:"";z-index:10;width:0;height:0;transition:all .18s ease-out .18s;position:absolute}[aria-label][data-balloon-pos]:hover:before,[aria-label][data-balloon-pos]:hover:after,[aria-label][data-balloon-pos][data-balloon-visible]:before,[aria-label][data-balloon-pos][data-balloon-visible]:after,[aria-label][data-balloon-pos]:not([data-balloon-nofocus]):focus:before,[aria-label][data-balloon-pos]:not([data-balloon-nofocus]):focus:after{opacity:1;pointer-events:none}[aria-label][data-balloon-pos].font-awesome:after{font-family:FontAwesome,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Oxygen,Ubuntu,Cantarell,Open Sans,Helvetica Neue,sans-serif}[aria-label][data-balloon-pos][data-balloon-break]:after{white-space:pre}[aria-label][data-balloon-pos][data-balloon-break][data-balloon-length]:after{white-space:pre-line;word-break:break-word}[aria-label][data-balloon-pos][data-balloon-blunt]:before,[aria-label][data-balloon-pos][data-balloon-blunt]:after{transition:none}[aria-label][data-balloon-pos][data-balloon-pos=up]:hover:after,[aria-label][data-balloon-pos][data-balloon-pos=up][data-balloon-visible]:after,[aria-label][data-balloon-pos][data-balloon-pos=down]:hover:after,[aria-label][data-balloon-pos][data-balloon-pos=down][data-balloon-visible]:after,[aria-label][data-balloon-pos][data-balloon-pos=up]:hover:before,[aria-label][data-balloon-pos][data-balloon-pos=up][data-balloon-visible]:before,[aria-label][data-balloon-pos][data-balloon-pos=down]:hover:before,[aria-label][data-balloon-pos][data-balloon-pos=down][data-balloon-visible]:before{transform:translate(-50%)}[aria-label][data-balloon-pos][data-balloon-pos*=-left]:after{left:0}[aria-label][data-balloon-pos][data-balloon-pos*=-left]:before{left:5px}[aria-label][data-balloon-pos][data-balloon-pos*=-right]:after{right:0}[aria-label][data-balloon-pos][data-balloon-pos*=-right]:before{right:5px}[aria-label][data-balloon-pos][data-balloon-pos*=-left]:hover:after,[aria-label][data-balloon-pos][data-balloon-pos*=-left][data-balloon-visible]:after,[aria-label][data-balloon-pos][data-balloon-pos*=-right]:hover:after,[aria-label][data-balloon-pos][data-balloon-pos*=-right][data-balloon-visible]:after,[aria-label][data-balloon-pos][data-balloon-pos*=-left]:hover:before,[aria-label][data-balloon-pos][data-balloon-pos*=-left][data-balloon-visible]:before,[aria-label][data-balloon-pos][data-balloon-pos*=-right]:hover:before,[aria-label][data-balloon-pos][data-balloon-pos*=-right][data-balloon-visible]:before{transform:translate(0)}[aria-label][data-balloon-pos][data-balloon-pos^=up]:before,[aria-label][data-balloon-pos][data-balloon-pos^=up]:after{transform-origin:top;transform:translate(0,var(--balloon-move));bottom:100%}[aria-label][data-balloon-pos][data-balloon-pos^=up]:after{margin-bottom:10px}[aria-label][data-balloon-pos][data-balloon-pos=up]:before,[aria-label][data-balloon-pos][data-balloon-pos=up]:after{transform:translate(-50%,var(--balloon-move));left:50%}[aria-label][data-balloon-pos][data-balloon-pos^=down]:before,[aria-label][data-balloon-pos][data-balloon-pos^=down]:after{transform:translate(0,calc(var(--balloon-move)*-1));top:100%}[aria-label][data-balloon-pos][data-balloon-pos^=down]:after{margin-top:10px}[aria-label][data-balloon-pos][data-balloon-pos^=down]:before{border:5px solid #0000;border-bottom-color:var(--balloon-color);width:0;height:0}[aria-label][data-balloon-pos][data-balloon-pos=down]:after,[aria-label][data-balloon-pos][data-balloon-pos=down]:before{transform:translate(-50%,calc(var(--balloon-move)*-1));left:50%}[aria-label][data-balloon-pos][data-balloon-pos=left]:hover:after,[aria-label][data-balloon-pos][data-balloon-pos=left][data-balloon-visible]:after,[aria-label][data-balloon-pos][data-balloon-pos=right]:hover:after,[aria-label][data-balloon-pos][data-balloon-pos=right][data-balloon-visible]:after,[aria-label][data-balloon-pos][data-balloon-pos=left]:hover:before,[aria-label][data-balloon-pos][data-balloon-pos=left][data-balloon-visible]:before,[aria-label][data-balloon-pos][data-balloon-pos=right]:hover:before,[aria-label][data-balloon-pos][data-balloon-pos=right][data-balloon-visible]:before{transform:translateY(-50%)}[aria-label][data-balloon-pos][data-balloon-pos=left]:after,[aria-label][data-balloon-pos][data-balloon-pos=left]:before{transform:translate(var(--balloon-move),-50%);top:50%;right:100%}[aria-label][data-balloon-pos][data-balloon-pos=left]:after{margin-right:10px}[aria-label][data-balloon-pos][data-balloon-pos=left]:before{border:5px solid #0000;border-left-color:var(--balloon-color);width:0;height:0}[aria-label][data-balloon-pos][data-balloon-pos=right]:after,[aria-label][data-balloon-pos][data-balloon-pos=right]:before{transform:translate(calc(var(--balloon-move)*-1),-50%);top:50%;left:100%}[aria-label][data-balloon-pos][data-balloon-pos=right]:after{margin-left:10px}[aria-label][data-balloon-pos][data-balloon-pos=right]:before{border:5px solid #0000;border-right-color:var(--balloon-color);width:0;height:0}[aria-label][data-balloon-pos][data-balloon-length]:after{white-space:normal}[aria-label][data-balloon-pos][data-balloon-length=small]:after{width:80px}[aria-label][data-balloon-pos][data-balloon-length=medium]:after{width:150px}[aria-label][data-balloon-pos][data-balloon-length=large]:after{width:260px}[aria-label][data-balloon-pos][data-balloon-length=xlarge]:after{width:380px}@media screen and (width<=768px){[aria-label][data-balloon-pos][data-balloon-length=xlarge]:after{width:90vw}}[aria-label][data-balloon-pos][data-balloon-length=fit]:after{width:100%}:root{--color-primary:#489fd9;--color-primary-light:#abd9f7;--color-primary-400:#3d7da9;--color-primary-300:#315d7c;--color-primary-200:#253e52;--color-primary-100:#151d24;--color-accent:#e37dd7;--color-accent-light:#f794d5;--color-accent-400:#b163a8;--color-accent-300:#824b7b;--color-accent-200:#563351;--color-accent-100:#2d1d2a;--color-body:#dfedf7;--color-muted:#a3c1d4;--color-background:var(--color-primary-100);--anchor-color:#e3ddf0;--anchor-color-hover:var(--color-accent-light);--border-color:var(--color-primary-300);--border-color-accent:var(--color-accent);--balloon-color:var(--color-primary-400);--color-success:#59c27c;--color-warning:#f0ee78;--color-danger:#cf4d4a;--font-size-sm:.875rem;--font-size-regular:1rem;--font-size-lg:1.25rem;--font-size-xlg:2rem;--font-size-xxlg:3rem}.d-none{display:none!important}.d-inline{display:inline!important}.d-inline-block{display:inline-block!important}.d-block{display:block!important}.d-table{display:table!important}.d-table-row{display:table-row!important}.d-table-cell{display:table-cell!important}.d-flex{display:flex!important}.d-inline-flex{display:inline-flex!important}@media (width>=768px){.d-md-none{display:none!important}.d-md-inline{display:inline!important}.d-md-inline-block{display:inline-block!important}.d-md-block{display:block!important}.d-md-table{display:table!important}.d-md-table-row{display:table-row!important}.d-md-table-cell{display:table-cell!important}.d-md-flex{display:flex!important}.d-md-inline-flex{display:inline-flex!important}}.m-0{margin:0!important}.mt-0,.my-0{margin-top:0!important}.mr-0,.mx-0{margin-right:0!important}.mb-0,.my-0{margin-bottom:0!important}.ml-0,.mx-0{margin-left:0!important}.m-1{margin:.25rem!important}.mt-1,.my-1{margin-top:.25rem!important}.mr-1,.mx-1{margin-right:.25rem!important}.mb-1,.my-1{margin-bottom:.25rem!important}.ml-1,.mx-1{margin-left:.25rem!important}.m-2{margin:.5rem!important}.mt-2,.my-2{margin-top:.5rem!important}.mr-2,.mx-2{margin-right:.5rem!important}.mb-2,.my-2{margin-bottom:.5rem!important}.ml-2,.mx-2{margin-left:.5rem!important}.m-3{margin:1rem!important}.mt-3,.my-3{margin-top:1rem!important}.mr-3,.mx-3{margin-right:1rem!important}.mb-3,.my-3{margin-bottom:1rem!important}.ml-3,.mx-3{margin-left:1rem!important}.m-4{margin:1.5rem!important}.mt-4,.my-4{margin-top:1.5rem!important}.mr-4,.mx-4{margin-right:1.5rem!important}.mb-4,.my-4{margin-bottom:1.5rem!important}.ml-4,.mx-4{margin-left:1.5rem!important}.m-5{margin:2.5rem!important}.mt-5,.my-5{margin-top:2.5rem!important}.mr-5,.mx-5{margin-right:2.5rem!important}.mb-5,.my-5{margin-bottom:2.5rem!important}.ml-5,.mx-5{margin-left:2.5rem!important}.p-0{padding:0!important}.pt-0,.py-0{padding-top:0!important}.pr-0,.px-0{padding-right:0!important}.pb-0,.py-0{padding-bottom:0!important}.pl-0,.px-0{padding-left:0!important}.p-1{padding:.25rem!important}.pt-1,.py-1{padding-top:.25rem!important}.pr-1,.px-1{padding-right:.25rem!important}.pb-1,.py-1{padding-bottom:.25rem!important}.pl-1,.px-1{padding-left:.25rem!important}.p-2{padding:.5rem!important}.pt-2,.py-2{padding-top:.5rem!important}.pr-2,.px-2{padding-right:.5rem!important}.pb-2,.py-2{padding-bottom:.5rem!important}.pl-2,.px-2{padding-left:.5rem!important}.p-3{padding:1rem!important}.pt-3,.py-3{padding-top:1rem!important}.pr-3,.px-3{padding-right:1rem!important}.pb-3,.py-3{padding-bottom:1rem!important}.pl-3,.px-3{padding-left:1rem!important}.p-4{padding:1.5rem!important}.pt-4,.py-4{padding-top:1.5rem!important}.pr-4,.px-4{padding-right:1.5rem!important}.pb-4,.py-4{padding-bottom:1.5rem!important}.pl-4,.px-4{padding-left:1.5rem!important}.p-5{padding:2.5rem!important}.pt-5,.py-5{padding-top:2.5rem!important}.pr-5,.px-5{padding-right:2.5rem!important}.pb-5,.py-5{padding-bottom:2.5rem!important}.pl-5,.px-5{padding-left:2.5rem!important}.m-n1{margin:-.25rem!important}.mt-n1,.my-n1{margin-top:-.25rem!important}.mr-n1,.mx-n1{margin-right:-.25rem!important}.mb-n1,.my-n1{margin-bottom:-.25rem!important}.ml-n1,.mx-n1{margin-left:-.25rem!important}.m-n2{margin:-.5rem!important}.mt-n2,.my-n2{margin-top:-.5rem!important}.mr-n2,.mx-n2{margin-right:-.5rem!important}.mb-n2,.my-n2{margin-bottom:-.5rem!important}.ml-n2,.mx-n2{margin-left:-.5rem!important}.m-n3{margin:-1rem!important}.mt-n3,.my-n3{margin-top:-1rem!important}.mr-n3,.mx-n3{margin-right:-1rem!important}.mb-n3,.my-n3{margin-bottom:-1rem!important}.ml-n3,.mx-n3{margin-left:-1rem!important}.m-n4{margin:-1.5rem!important}.mt-n4,.my-n4{margin-top:-1.5rem!important}.mr-n4,.mx-n4{margin-right:-1.5rem!important}.mb-n4,.my-n4{margin-bottom:-1.5rem!important}.ml-n4,.mx-n4{margin-left:-1.5rem!important}.m-n5{margin:-2.5rem!important}.mt-n5,.my-n5{margin-top:-2.5rem!important}.mr-n5,.mx-n5{margin-right:-2.5rem!important}.mb-n5,.my-n5{margin-bottom:-2.5rem!important}.ml-n5,.mx-n5{margin-left:-2.5rem!important}.m-auto{margin:auto!important}.mt-auto,.my-auto{margin-top:auto!important}.mr-auto,.mx-auto{margin-right:auto!important}.mb-auto,.my-auto{margin-bottom:auto!important}.ml-auto,.mx-auto{margin-left:auto!important}@media (width>=768px){.m-md-0{margin:0!important}.mt-md-0,.my-md-0{margin-top:0!important}.mr-md-0,.mx-md-0{margin-right:0!important}.mb-md-0,.my-md-0{margin-bottom:0!important}.ml-md-0,.mx-md-0{margin-left:0!important}.m-md-1{margin:.25rem!important}.mt-md-1,.my-md-1{margin-top:.25rem!important}.mr-md-1,.mx-md-1{margin-right:.25rem!important}.mb-md-1,.my-md-1{margin-bottom:.25rem!important}.ml-md-1,.mx-md-1{margin-left:.25rem!important}.m-md-2{margin:.5rem!important}.mt-md-2,.my-md-2{margin-top:.5rem!important}.mr-md-2,.mx-md-2{margin-right:.5rem!important}.mb-md-2,.my-md-2{margin-bottom:.5rem!important}.ml-md-2,.mx-md-2{margin-left:.5rem!important}.m-md-3{margin:1rem!important}.mt-md-3,.my-md-3{margin-top:1rem!important}.mr-md-3,.mx-md-3{margin-right:1rem!important}.mb-md-3,.my-md-3{margin-bottom:1rem!important}.ml-md-3,.mx-md-3{margin-left:1rem!important}.m-md-4{margin:1.5rem!important}.mt-md-4,.my-md-4{margin-top:1.5rem!important}.mr-md-4,.mx-md-4{margin-right:1.5rem!important}.mb-md-4,.my-md-4{margin-bottom:1.5rem!important}.ml-md-4,.mx-md-4{margin-left:1.5rem!important}.m-md-5{margin:2.5rem!important}.mt-md-5,.my-md-5{margin-top:2.5rem!important}.mr-md-5,.mx-md-5{margin-right:2.5rem!important}.mb-md-5,.my-md-5{margin-bottom:2.5rem!important}.ml-md-5,.mx-md-5{margin-left:2.5rem!important}.p-md-0{padding:0!important}.pt-md-0,.py-md-0{padding-top:0!important}.pr-md-0,.px-md-0{padding-right:0!important}.pb-md-0,.py-md-0{padding-bottom:0!important}.pl-md-0,.px-md-0{padding-left:0!important}.p-md-1{padding:.25rem!important}.pt-md-1,.py-md-1{padding-top:.25rem!important}.pr-md-1,.px-md-1{padding-right:.25rem!important}.pb-md-1,.py-md-1{padding-bottom:.25rem!important}.pl-md-1,.px-md-1{padding-left:.25rem!important}.p-md-2{padding:.5rem!important}.pt-md-2,.py-md-2{padding-top:.5rem!important}.pr-md-2,.px-md-2{padding-right:.5rem!important}.pb-md-2,.py-md-2{padding-bottom:.5rem!important}.pl-md-2,.px-md-2{padding-left:.5rem!important}.p-md-3{padding:1rem!important}.pt-md-3,.py-md-3{padding-top:1rem!important}.pr-md-3,.px-md-3{padding-right:1rem!important}.pb-md-3,.py-md-3{padding-bottom:1rem!important}.pl-md-3,.px-md-3{padding-left:1rem!important}.p-md-4{padding:1.5rem!important}.pt-md-4,.py-md-4{padding-top:1.5rem!important}.pr-md-4,.px-md-4{padding-right:1.5rem!important}.pb-md-4,.py-md-4{padding-bottom:1.5rem!important}.pl-md-4,.px-md-4{padding-left:1.5rem!important}.p-md-5{padding:2.5rem!important}.pt-md-5,.py-md-5{padding-top:2.5rem!important}.pr-md-5,.px-md-5{padding-right:2.5rem!important}.pb-md-5,.py-md-5{padding-bottom:2.5rem!important}.pl-md-5,.px-md-5{padding-left:2.5rem!important}.m-md-n1{margin:-.25rem!important}.mt-md-n1,.my-md-n1{margin-top:-.25rem!important}.mr-md-n1,.mx-md-n1{margin-right:-.25rem!important}.mb-md-n1,.my-md-n1{margin-bottom:-.25rem!important}.ml-md-n1,.mx-md-n1{margin-left:-.25rem!important}.m-md-n2{margin:-.5rem!important}.mt-md-n2,.my-md-n2{margin-top:-.5rem!important}.mr-md-n2,.mx-md-n2{margin-right:-.5rem!important}.mb-md-n2,.my-md-n2{margin-bottom:-.5rem!important}.ml-md-n2,.mx-md-n2{margin-left:-.5rem!important}.m-md-n3{margin:-1rem!important}.mt-md-n3,.my-md-n3{margin-top:-1rem!important}.mr-md-n3,.mx-md-n3{margin-right:-1rem!important}.mb-md-n3,.my-md-n3{margin-bottom:-1rem!important}.ml-md-n3,.mx-md-n3{margin-left:-1rem!important}.m-md-n4{margin:-1.5rem!important}.mt-md-n4,.my-md-n4{margin-top:-1.5rem!important}.mr-md-n4,.mx-md-n4{margin-right:-1.5rem!important}.mb-md-n4,.my-md-n4{margin-bottom:-1.5rem!important}.ml-md-n4,.mx-md-n4{margin-left:-1.5rem!important}.m-md-n5{margin:-2.5rem!important}.mt-md-n5,.my-md-n5{margin-top:-2.5rem!important}.mr-md-n5,.mx-md-n5{margin-right:-2.5rem!important}.mb-md-n5,.my-md-n5{margin-bottom:-2.5rem!important}.ml-md-n5,.mx-md-n5{margin-left:-2.5rem!important}.m-md-auto{margin:auto!important}.mt-md-auto,.my-md-auto{margin-top:auto!important}.mr-md-auto,.mx-md-auto{margin-right:auto!important}.mb-md-auto,.my-md-auto{margin-bottom:auto!important}.ml-md-auto,.mx-md-auto{margin-left:auto!important}}.flex-row{flex-direction:row!important}.flex-column{flex-direction:column!important}.flex-row-reverse{flex-direction:row-reverse!important}.flex-column-reverse{flex-direction:column-reverse!important}.flex-wrap{flex-wrap:wrap!important}.flex-nowrap{flex-wrap:nowrap!important}.flex-wrap-reverse{flex-wrap:wrap-reverse!important}.flex-fill{flex:auto!important}.flex-grow-0{flex-grow:0!important}.flex-grow-1{flex-grow:1!important}.flex-shrink-0{flex-shrink:0!important}.flex-shrink-1{flex-shrink:1!important}.justify-content-start{justify-content:flex-start!important}.justify-content-end{justify-content:flex-end!important}.justify-content-center{justify-content:center!important}.justify-content-between{justify-content:space-between!important}.justify-content-around{justify-content:space-around!important}.align-items-start{align-items:flex-start!important}.align-items-end{align-items:flex-end!important}.align-items-center{align-items:center!important}.align-items-baseline{align-items:baseline!important}.align-items-stretch{align-items:stretch!important}.align-content-start{align-content:flex-start!important}.align-content-end{align-content:flex-end!important}.align-content-center{align-content:center!important}.align-content-between{align-content:space-between!important}.align-content-around{align-content:space-around!important}.align-content-stretch{align-content:stretch!important}.align-self-auto{align-self:auto!important}.align-self-start{align-self:flex-start!important}.align-self-end{align-self:flex-end!important}.align-self-center{align-self:center!important}.align-self-baseline{align-self:baseline!important}.align-self-stretch{align-self:stretch!important}@media (width>=768px){.flex-md-row{flex-direction:row!important}.flex-md-column{flex-direction:column!important}.flex-md-row-reverse{flex-direction:row-reverse!important}.flex-md-column-reverse{flex-direction:column-reverse!important}.flex-md-wrap{flex-wrap:wrap!important}.flex-md-nowrap{flex-wrap:nowrap!important}.flex-md-wrap-reverse{flex-wrap:wrap-reverse!important}.flex-md-fill{flex:auto!important}.flex-md-grow-0{flex-grow:0!important}.flex-md-grow-1{flex-grow:1!important}.flex-md-shrink-0{flex-shrink:0!important}.flex-md-shrink-1{flex-shrink:1!important}.justify-content-md-start{justify-content:flex-start!important}.justify-content-md-end{justify-content:flex-end!important}.justify-content-md-center{justify-content:center!important}.justify-content-md-between{justify-content:space-between!important}.justify-content-md-around{justify-content:space-around!important}.align-items-md-start{align-items:flex-start!important}.align-items-md-end{align-items:flex-end!important}.align-items-md-center{align-items:center!important}.align-items-md-baseline{align-items:baseline!important}.align-items-md-stretch{align-items:stretch!important}.align-content-md-start{align-content:flex-start!important}.align-content-md-end{align-content:flex-end!important}.align-content-md-center{align-content:center!important}.align-content-md-between{align-content:space-between!important}.align-content-md-around{align-content:space-around!important}.align-content-md-stretch{align-content:stretch!important}.align-self-md-auto{align-self:auto!important}.align-self-md-start{align-self:flex-start!important}.align-self-md-end{align-self:flex-end!important}.align-self-md-center{align-self:center!important}.align-self-md-baseline{align-self:baseline!important}.align-self-md-stretch{align-self:stretch!important}}small,.text-sm{font-size:var(--font-size-sm)!important}.text-regular{font-size:var(--font-size-regular)!important}.text-lg{font-size:var(--font-size-lg)!important}.text-xlg{font-size:var(--font-size-xlg)!important}.text-right{text-align:right}.text-left{text-align:left}.text-center{text-align:center}.text-muted{color:var(--color-muted)!important}.text-uppercase{text-transform:uppercase}.font-weight-normal{font-weight:400}.font-weight-bold{font-weight:700}.font-weight-semibold{font-weight:600}.font-weight-black{font-weight:900}.font-style-italic{font-style:italic}.font-small-caps{font-variant:all-small-caps}.line-height-1{line-height:1}.text-decoration-none{text-decoration:none}.text-break-all{word-break:break-all}.text-nowrap{white-space:nowrap}.position-relative{position:relative}.img-fluid{max-width:100%;height:auto}.zero{margin:0;padding:0}.invisible{visibility:hidden}.h-100{height:100%}.w-100{width:100%}.d-grid{grid-auto-columns:1fr;grid-auto-flow:column;display:grid}.rounded{border-radius:.5rem}.border{border:1px solid var(--border-color)}.border-accent{border:1px solid var(--border-color-accent)}.border-top{border-top:1px solid var(--color-primary-300)}.border-bottom{border-bottom:1px solid var(--color-primary-300)}.border-right{border-right:1px solid var(--color-primary-300)}.border-left{border-left:1px solid var(--color-primary-300)}.carousel{margin:0 -3rem;position:relative}.carousel__items{scroll-behavior:smooth;-webkit-overflow-scrolling:touch;scroll-snap-type:x mandatory;scroll-snap-align:start;scrollbar-width:none;-ms-overflow-style:none;gap:2rem;width:100%;display:flex;overflow-x:scroll}.carousel-item{flex-shrink:0;max-width:300px}.carousel-item:first-child{padding-left:3rem}.carousel-item:last-child{padding-right:3rem}.carousel__items::-webkit-scrollbar{display:none}.carousel__next,.carousel__prev{z-index:1;position:absolute;top:calc(50% - 12px);left:0}.carousel__next{left:unset;right:0}.btn{text-transform:uppercase;font-size:var(--font-size-sm);letter-spacing:.05rem;cursor:pointer;background:var(--color-background);border:2px solid var(--color-primary-400);color:var(--color-primary-light);border-radius:.5rem;padding:.75rem;font-weight:700;transition:border-color .1s ease-in}.btn-small{text-transform:uppercase;font-size:var(--font-size-sm);cursor:pointer;background:var(--color-background);border:2px solid var(--color-primary-400);color:var(--color-primary-light);border-radius:.5rem;padding:.5rem;font-weight:700}.btn-small:hover,.btn:hover{border-color:var(--anchor-color-hover);color:var(--anchor-color-hover)}.btn img,.btn-small img{filter:invert(77%)sepia(40%)saturate(250%)hue-rotate(164deg)brightness()contrast(94%)}.btn:hover img,.btn-small:hover img{filter:invert(85%)sepia(46%)saturate(3508%)hue-rotate(287deg)brightness(112%)contrast(94%)}.btn-text{color:inherit;font-size:inherit;cursor:pointer;background:0 0;border:0;margin:0;padding:0;transition:color .1s ease-in}.btn-text:hover{color:var(--anchor-color-hover)!important}.btn-icon{cursor:pointer;color:inherit;background:0 0;border:0;align-items:center;transition:color .1s ease-in;display:inline-flex}select{border:2px solid var(--color-primary-400);color:var(--color-primary-light);font-size:var(--font-size-sm);appearance:none;background:var(--color-background)url("data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='100' height='100' fill='%233d8fa9'><polygon points='0,0 100,0 50,50'/></svg>") no-repeat;background-position:right .75em top 65%;background-repeat:no-repeat;background-size:12px;border-radius:.5rem;min-width:20ch;padding:.5rem 2rem .5rem .5rem}select:focus-visible{border:2px solid var(--anchor-color-hover);color:var(--anchor-color-hover);outline:none}h1,h2,h3,h4,h5,h6,p{margin:0}body{color:var(--color-body);background-color:var(--color-background);font:1rem/1.5 system-ui,sans-serif;display:flex}h1,h2,h3,h4,h5,h6{line-height:1.1}a{color:inherit;transition:color .1s ease-in}a:hover{color:var(--anchor-color-hover)}a:visited{-webkit-text-decoration:none;text-decoration:none}:target{color:var(--anchor-color-hover)}code{font-family:ui-monospace,Menlo,Monaco,Courier New,monospace}hr{border-top:1px solid var(--border-color);border-bottom:0}dt{font-size:var(--font-size-sm);text-transform:uppercase;color:var(--color-muted);font-weight:600}dd{font-size:var(--font-size-sm);margin:0 0 1rem}.badge{color:var(--color-muted);background-color:var(--color-primary-300);border-radius:.5rem;padding:.1875rem .375rem;text-decoration:none}.badge--outline{border:2px solid var(--color-primary-300);color:var(--color-muted);border-radius:.5rem;padding:.1875rem .375rem;text-decoration:none;transition:border-color .1s ease-in}.badge--outline:hover{border-color:var(--anchor-color-hover)}.badge--pill{border-radius:1rem}.badge-res{background:var(--color-primary-200);color:#fff;text-shadow:1px 1px #4d5078;border-radius:4px;padding:0 3px;font-size:12px}.badge-2160{background:#b82927}.badge-1080{background:#e0560b}.badge-720{background:var(--color-accent)}.badge-480{background:#269ddb}.torrent-medium{color:var(--color-warning)}.torrent-low{color:var(--color-danger)}fieldset{border:0;margin:0;padding:0}legend{font-size:var(--font-size-sm);text-transform:uppercase;color:var(--color-muted);font-weight:600}.report,.table{border-collapse:collapse}.table td{padding:.1875rem .5rem .1875rem 0}.table tr{transition:background-color .1s ease-out}.table tr:hover{background-color:#253e52}.report td{padding:.25em 2rem .25rem 0}.report th,.table th{border-bottom:1px solid var(--color-primary-200);color:var(--color-muted);text-transform:uppercase;font-weight:600;font-size:var(--font-size-sm);padding:.375rem .5rem .375rem 0}@media screen and (width>=768px){.card-series{max-width:10rem}}.card-series__image{aspect-ratio:500/750;border:2px solid var(--color-primary-200);box-shadow:var(--color-primary-200)0 0;background-color:var(--color-accent-200);background-position:0 0;background-image:linear-gradient(125deg,var(--color-accent-400)25%,transparent 25%);transition:transform .2s ease-out,filter .3s ease-out,box-shadow .2s ease-out}a:hover .card-series__image{filter:brightness(1.25);box-shadow:var(--color-primary-200)7px 7px;transform:translate(-7px,-7px)}.search-query{width:min-content;position:relative}.search-query input{background:var(--color-background);border:2px solid var(--color-primary-400);color:var(--color-primary-light);font-size:var(--font-size-lg);border-radius:.5rem;padding:.75rem .5rem}.search-query input::-webkit-calendar-picker-indicator{display:none!important}@media screen and (width>=768px){.search-query input{width:30rem}}.search-query input:focus-visible{border:2px solid var(--anchor-color-hover);outline:none}input::placeholder{color:var(--color-primary-300)}.search-query button{z-index:1;background:var(--color-background);cursor:pointer;font-size:var(--font-size-lg);background:0 0;border:0;padding:.75rem;position:absolute;top:0;right:0}a:hover .card-episode__poster,a:hover .card-episode__image,.btn-text:hover .card-episode__image{border-color:var(--color-accent);transition:border-color .1s ease-in}.header .btn-icon:hover{background-color:var(--color-primary-300);transition:background-color .2s ease-out}.header{background:var(--color-primary-200);flex-direction:column;gap:.5rem;height:100vh;display:flex;position:sticky;top:0}.header .btn-icon{padding:.75rem}.icon,.header .btn-icon img{filter:invert(88%)sepia(3%)saturate(2496%)hue-rotate(185deg)brightness(106%)contrast(94%)}.header .btn-icon:hover img{filter:invert(78%)sepia(13%)saturate(3097%)hue-rotate(274deg)brightness(96%)contrast(85%)}@media screen and (width>=768px){.header{align-items:center}nav{background:0 0}}main{flex-grow:1;padding:3rem}.footer{color:var(--color-muted)}aside{flex-shrink:0;flex-basis:14rem}.main-column{flex-grow:1}.card-episode{position:relative}.card-episode__image{aspect-ratio:300/170;border:2px solid var(--color-primary-300);background-position:0 0;background-color:var(--color-accent-200);background-image:linear-gradient(125deg,var(--color-accent-400)25%,transparent 25%);transition:transform .2s ease-out,filter .3s ease-out,box-shadow .2s ease-out}.card-episode__poster{z-index:1;border:2px solid var(--color-primary-300);max-width:75px;position:absolute;bottom:-1rem;right:1rem}.series-poster__image{aspect-ratio:500/750;border:2px solid var(--color-primary-200);background-position:0 0;background-color:var(--color-accent-200);background-image:linear-gradient(125deg,var(--color-accent-400)25%,transparent 25%)}@media screen and (width>=768px){.series-poster__image{box-shadow:var(--color-primary-200)7px 7px}}.episode-grid{grid-template-rows:auto;grid-template-columns:repeat(4,1fr);gap:2rem;display:grid}.episode-grid__cell{max-width:300px}.body-copy,.series-overview{max-width:75ch}.fanart{background-blend-mode:multiply;background-position:top;background-repeat:no-repeat;background-size:cover;background-attachment:fixed;background-color:var(--color-accent-100);margin-top:-3rem;margin-left:-3rem;margin-right:-3rem;padding:3rem}@media screen and (width>=768px){.top-series-grid{grid-template-columns:repeat(2,1fr);gap:2rem;display:grid}}.cards-grid{grid-template-columns:repeat(3,1fr);gap:1.5rem;margin-bottom:2rem;display:grid}@media screen and (width>=768px){.cards-grid{grid-template-columns:repeat(6,1fr);gap:2rem}}dialog{opacity:0;color:var(--color-body);max-width:unset;max-height:unset;pointer-events:none;background:0 0;border:0;width:100vw;height:100vh;margin:0;padding:0}dialog.in{pointer-events:auto;opacity:1;transition:opacity .3s ease-out}dialog.out{opacity:0;transition:opacity .3s ease-out 2s}.dialog-body{background:var(--color-primary-200);border-radius:1rem;width:30rem;padding:2rem}.dialog-body--small{width:16rem}dialog:modal{opacity:1;pointer-events:auto;justify-content:center;align-items:center;display:flex}dialog::backdrop{background:#151d27bf}.anim-spin{animation-name:spin;animation-duration:4s;animation-timing-function:linear;animation-iteration-count:infinite}@keyframes spin{0%{transform:rotate(0)}to{transform:rotate(360deg)}}.sr-only{white-space:nowrap;clip:rect(0 0 0 0);clip-path:inset(50%);border:0;width:1px;height:1px;margin:-1px;padding:0;position:absolute;overflow:hidden}.skip-nav a{width:1px;height:1px;position:absolute;top:auto;left:-9999px;overflow:hidden}.skip-nav a:focus{width:auto;height:auto;position:static}.mobile-carousel{gap:1.5rem;display:flex}@media screen and (width<=767.98px){.mobile-carousel{scroll-behavior:smooth;-webkit-overflow-scrolling:touch;scroll-snap-type:x mandatory;margin:0 -1rem 0 0;display:flex;overflow-x:scroll}.mobile-carousel>.mobile-carousel__item{scroll-snap-align:start;flex-shrink:0;flex-basis:50vw}.mobile-carousel::-webkit-scrollbar{display:none}}@media screen and (width>=768px){.mobile-carousel{gap:2rem}}.radio-button-group{border:2px solid var(--color-primary-400);color:var(--color-primary-light);font-size:var(--font-size-sm);background-color:var(--color-primary-100);border-radius:.5rem;display:flex}.radio-button-group__label{color:var(--color-body);cursor:pointer;background-color:#0000;border-radius:.4rem;align-items:center;padding:.5rem;display:inline-flex}.radio-button-group__label:has(input:checked){background-color:var(--color-primary-300)}.radio-button-group__input{clip:rect(0,0,0,0);white-space:nowrap;border:0;width:1px;height:1px;padding:0;position:absolute;overflow:hidden}progress{accent-color:var(--color-accent-light)}.chart{max-width:100%}
 /*# sourceMappingURL=app.css.map */
```

### Comparing `videobox-0.6.1/videobox/static/app.css.map` & `videobox-0.7.0/videobox/static/app.css.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8712121212121212%*

 * *Differences: {"'mappings'": "'6E,oD,c,mB,gC,oD,wC,yB,yG,4B,kD,oB,8E,kB,c,sB,mG,8B,kC,0E,qD,4D,2D,4D,oD,2D,0D,2D,oC,qG,iC,uB,6D,qD,qD,+D,iE,oE,sB,0B,+BEAA,kIAOE,sDAGA,gEAGE,yhBAmBA,4NAWA,2XAGA,uLAEA,yEAEA,yHAGA,mIAEA,smBAIA,qEAEA,wEAEA,uEAEA,0EAEA,+nBAIA,mMAIA,8EAEA,4KAGA,wLAGA,6EAEA,+IAKA,yLAGA,mnBAIA,0LAIA,8EAEA,4IAKA,oMAIA,8EAEA,8IAKA,6EAEA,2EAEA,6EAEA,4EAEA,6EAEE,iCACE,6EAEJ,yEC3HJ,6xBC+CM,+BAAA,mCAAA,+CAAA,iCAAA,iCAAA,yCAAA,2CAAA,+BAAA,6CA/BF,sBA+BE,kCAAA,sCAAA,kDAAA,oCAAA,oCAAA,4CAAA,8CAAA,kCAAA,iDAeE,wBAIA,mCAKA,q […]*

```diff
@@ -1,26 +1,26 @@
 {
     "file": "app.css.map",
-    "mappings": "6E,oD,c,mB,gC,oD,wC,yB,yG,4B,kD,oB,8E,kB,c,sB,mG,8B,kC,0E,qD,4D,2D,4D,oD,2D,0D,2D,oC,qG,iC,uB,6D,qD,qD,+D,iE,oE,sB,0B,+BEAA,kIAOE,sDAGA,gEAGE,yhBAmBA,4NAWA,2XAGA,uLAEA,yEAEA,yHAGA,mIAEA,smBAIA,qEAEA,wEAEA,uEAEA,0EAEA,+nBAIA,mMAIA,8EAEA,4KAGA,wLAGA,6EAEA,+IAKA,yLAGA,mnBAIA,0LAIA,8EAEA,4IAKA,oMAIA,8EAEA,8IAKA,6EAEA,2EAEA,6EAEA,4EAEA,6EAEE,iCACE,6EAEJ,yEC3HJ,4qBC+CM,+BAAA,mCAAA,+CAAA,iCAAA,iCAAA,yCAAA,2CAAA,+BAAA,6CA/BF,sBA+BE,kCAAA,sCAAA,kDAAA,oCAAA,oCAAA,4CAAA,8CAAA,kCAAA,iDAeE,wBAIA,mCAKA,qCAKA,sCAKA,oCAnBA,6BAIA,wCAKA,0CAKA,2CAKA,yCAnBA,4BAIA,uCAKA,yCAKA,0CAKA,wCAnBA,2BAIA,sCAKA,wCAKA,yCAKA,uCAnBA,6BAIA,wCAKA,0CAKA,2CAKA,yCAnBA,6BAIA,wCAKA,0CAKA,2CAKA,yCAnBA,yBAIA,oCAKA,sCAKA,uCAKA,qCAnBA,8BAIA,yCAKA,2CAKA,4CAKA,0CAnBA,6BAIA,wCAKA,0CAKA,2CAKA,yCAnBA,4BAIA,uCAKA,yCAKA,0CAKA,wCAnBA,8BAIA,yCAKA,2CAKA,4CAKA,0CAnBA,8BAIA,yCAKA,2CAKA,4CAKA,0CAUA,+BAIA,2CAKA,6CAKA,8CAKA,4CAnBA,8BAIA,0CAKA,4CAKA,6CAKA,2CAnBA,6BAIA,yCAKA,2CAKA,4CAKA,0CAnBA,+BAIA,2CAKA,6CAKA,8CAKA,4CAnBA,+BAIA,2CAKA,6CAKA,8CAKA,4CAQJ,8BAIA,4CAKA,8CAKA,+CAKA,6CAzHA,sBA8CI,2BAIA,yCAKA,2CAKA,4CAKA,0CAnBA,gCAIA,8CAKA,gDAKA,iDAKA,+CAnBA,+BAIA,6CAKA,+CAKA,gDAKA,8CAnBA,8BAIA,4CAKA,8CAKA,+CAKA,6CAnBA,gCAIA,8CAKA,gDAKA,iDAKA,+CAnBA,gCAIA,8CAKA,gDAKA,iDAKA,+CAnBA,4BAIA,0CAKA,4CAKA,6CAKA,2CAnBA,iCAIA,+CAKA,iDAKA,kDAKA,gDAnBA,gCAIA,8CAKA,gDAKA,iDAKA,+CAnBA,+BAIA,6CAKA,+CAKA,gDAKA,8CAnBA,iCAIA,+CAKA,iDAKA,kDAKA,gDAnBA,iCAIA,+CAKA,iDAKA,kDAKA,gDAUA,kCAIA,iDAKA,mDAKA,oDAKA,kDAnBA,iCAIA,gDAKA,kDAKA,mDAKA,iDAnBA,gCAIA,+CAKA,iDAKA,kDAKA,gDAnBA,kCAIA,iDAKA,mDAKA,oDAKA,kDAnBA,kCAIA,iDAKA,mDAKA,oDAKA,kDAQJ,iCAIA,kDAKA,oDAKA,qDAKA,oDAaA,uCAIA,6CAIA,uDAIA,6DAIA,oCAIA,wCAIA,oDAIA,+BAIA,mCAIA,mCAIA,uCAIA,uCAIA,4DAIA,wDAIA,yDAIA,iEAIA,+DAIA,oDAIA,gDAIA,iDAIA,qDAIA,mDAIA,wDAIA,oDAIA,qDAIA,6DAIA,2DAIA,uDAIA,2CAIA,kDAIA,8CAIA,+CAIA,mDAIA,iDA1QA,sBAsIA,0CAIA,gDAIA,0DAIA,gEAIA,uCAIA,2CAIA,uDAIA,kCAIA,sCAIA,sCAIA,0CAIA,0CAIA,+DAIA,2DAIA,4DAIA,oEAIA,kEAIA,uDAIA,mDAIA,oDAIA,wDAIA,sDAIA,2DAIA,uDAIA,wDAIA,gEAIA,8DAIA,0DAIA,8CAIA,qDAIA,iDAIA,kDAIA,sDAIA,qDAQJ,uDAKA,2DAIA,iDAIA,mDAIA,6BAIA,2BAIA,+BAIA,+CAIA,yCAIA,oCAIA,kCAIA,sCAIA,mCAIA,qCAIA,6BAIA,2CAIA,qCAIA,gCAMA,qCAIA,sCAKA,yBAKA,6BAIA,mBAIA,kBAIA,iEAMA,6BAMA,6CAIA,0DAIA,gEAIA,8DAIA,4DClZA,2CASA,8NAiBA,6CAIE,6CAIA,6CAUF,iDAQA,wFAQA,mCClFA,sSAcA,iPAYA,mGAQI,8GAIA,+HAUJ,iIAYA,0DAQA,mICxEA,keAkBA,6GJgEA,6BAUA,sHAOA,kCASA,6CAKA,wCAIA,4DAIA,wCAIA,iEAIA,4DASA,mGAOA,iDAKA,4IASA,yLASA,6DAKA,gCAIA,qIASA,+BAIA,+BAIA,0CAIA,8BAMA,8BAIA,2BAMA,qCAMA,uGASA,wCAKA,4CAIA,mDAIA,yCAIA,2EAKA,sMAYA,iCACE,8BAKF,6VAUA,8HAcA,kDAKA,yMAWA,8EAKA,iCACE,iCAKF,0FAMA,kDAIA,sLA0BA,qKAQA,2GAKA,4HAUA,iCAKA,sHAKA,sHAIA,iCACE,2BAQA,oBAWF,8BAKA,iCAIA,qCAKA,yBAWA,gCAIA,uTAUA,mIAeA,0OAQA,iCACE,kEAKF,gGAOA,oCAkCA,2CAKA,yPAcA,iCACE,4EAOF,2FAOA,iCACE,0DAMF,8IAgBA,6FAOA,gCAIA,8EAQA,sCAIA,oEASA,yHAOA,oEAYA,0JAaA,yFASA,yDAaA,yCAKA,oCACE,wJASA,8FAQA,kDAKF,iCACE,2BAQF,wMAUA,kKAeA,wFAMA,2IAaA",
+    "mappings": "6E,oD,c,mB,gC,oD,wC,yB,yG,4B,kD,oB,8E,kB,c,sB,mG,8B,kC,0E,qD,4D,2D,4D,oD,2D,0D,2D,oC,qG,iC,uB,6D,qD,qD,+D,iE,oE,sB,0B,+BEAA,kIAOE,sDAGA,gEAGE,yhBAmBA,4NAWA,2XAGA,uLAEA,yEAEA,yHAGA,mIAEA,smBAIA,qEAEA,wEAEA,uEAEA,0EAEA,+nBAIA,mMAIA,8EAEA,4KAGA,wLAGA,6EAEA,+IAKA,yLAGA,mnBAIA,0LAIA,8EAEA,4IAKA,oMAIA,8EAEA,8IAKA,6EAEA,2EAEA,6EAEA,4EAEA,6EAEE,iCACE,6EAEJ,yEC3HJ,6xBC+CM,+BAAA,mCAAA,+CAAA,iCAAA,iCAAA,yCAAA,2CAAA,+BAAA,6CA/BF,sBA+BE,kCAAA,sCAAA,kDAAA,oCAAA,oCAAA,4CAAA,8CAAA,kCAAA,iDAeE,wBAIA,mCAKA,qCAKA,sCAKA,oCAnBA,6BAIA,wCAKA,0CAKA,2CAKA,yCAnBA,4BAIA,uCAKA,yCAKA,0CAKA,wCAnBA,2BAIA,sCAKA,wCAKA,yCAKA,uCAnBA,6BAIA,wCAKA,0CAKA,2CAKA,yCAnBA,6BAIA,wCAKA,0CAKA,2CAKA,yCAnBA,yBAIA,oCAKA,sCAKA,uCAKA,qCAnBA,8BAIA,yCAKA,2CAKA,4CAKA,0CAnBA,6BAIA,wCAKA,0CAKA,2CAKA,yCAnBA,4BAIA,uCAKA,yCAKA,0CAKA,wCAnBA,8BAIA,yCAKA,2CAKA,4CAKA,0CAnBA,8BAIA,yCAKA,2CAKA,4CAKA,0CAUA,+BAIA,2CAKA,6CAKA,8CAKA,4CAnBA,8BAIA,0CAKA,4CAKA,6CAKA,2CAnBA,6BAIA,yCAKA,2CAKA,4CAKA,0CAnBA,+BAIA,2CAKA,6CAKA,8CAKA,4CAnBA,+BAIA,2CAKA,6CAKA,8CAKA,4CAQJ,8BAIA,4CAKA,8CAKA,+CAKA,6CAzHA,sBA8CI,2BAIA,yCAKA,2CAKA,4CAKA,0CAnBA,gCAIA,8CAKA,gDAKA,iDAKA,+CAnBA,+BAIA,6CAKA,+CAKA,gDAKA,8CAnBA,8BAIA,4CAKA,8CAKA,+CAKA,6CAnBA,gCAIA,8CAKA,gDAKA,iDAKA,+CAnBA,gCAIA,8CAKA,gDAKA,iDAKA,+CAnBA,4BAIA,0CAKA,4CAKA,6CAKA,2CAnBA,iCAIA,+CAKA,iDAKA,kDAKA,gDAnBA,gCAIA,8CAKA,gDAKA,iDAKA,+CAnBA,+BAIA,6CAKA,+CAKA,gDAKA,8CAnBA,iCAIA,+CAKA,iDAKA,kDAKA,gDAnBA,iCAIA,+CAKA,iDAKA,kDAKA,gDAUA,kCAIA,iDAKA,mDAKA,oDAKA,kDAnBA,iCAIA,gDAKA,kDAKA,mDAKA,iDAnBA,gCAIA,+CAKA,iDAKA,kDAKA,gDAnBA,kCAIA,iDAKA,mDAKA,oDAKA,kDAnBA,kCAIA,iDAKA,mDAKA,oDAKA,kDAQJ,iCAIA,kDAKA,oDAKA,qDAKA,oDAaA,uCAIA,6CAIA,uDAIA,6DAIA,oCAIA,wCAIA,oDAIA,+BAIA,mCAIA,mCAIA,uCAIA,uCAIA,4DAIA,wDAIA,yDAIA,iEAIA,+DAIA,oDAIA,gDAIA,iDAIA,qDAIA,mDAIA,wDAIA,oDAIA,qDAIA,6DAIA,2DAIA,uDAIA,2CAIA,kDAIA,8CAIA,+CAIA,mDAIA,iDA1QA,sBAsIA,0CAIA,gDAIA,0DAIA,gEAIA,uCAIA,2CAIA,uDAIA,kCAIA,sCAIA,sCAIA,0CAIA,0CAIA,+DAIA,2DAIA,4DAIA,oEAIA,kEAIA,uDAIA,mDAIA,oDAIA,wDAIA,sDAIA,2DAIA,uDAIA,wDAIA,gEAIA,8DAIA,0DAIA,8CAIA,qDAIA,iDAIA,kDAIA,sDAIA,qDAQJ,uDAKA,2DAIA,iDAIA,mDAIA,6BAIA,2BAIA,+BAIA,+CAIA,yCAIA,oCAIA,kCAIA,sCAIA,mCAIA,qCAIA,6CAIA,6BAIA,2CAIA,qCAIA,gCAMA,qCAIA,sCAKA,yBAKA,6BAIA,mBAIA,kBAIA,iEAMA,6BAMA,6CAIA,2DAIA,0DAIA,gEAIA,8DAIA,4DC1ZA,2CASA,8NAiBA,6CAIE,6CAIA,6CAUF,iDAQA,wFAQA,mCClFA,sSAcA,iPAYA,mGAQI,8GAIA,+HAUJ,iIAYA,0DAQA,mICxEA,keAkBA,6GJqEA,6BAUA,sHAOA,kCASA,6CAKA,wCAIA,4DAIA,wCAIA,iEAIA,4DASA,mGAOA,iDAKA,4IASA,yLASA,6DAKA,gCAIA,qIASA,+BAIA,+BAIA,0CAIA,8BAMA,2CAIA,uCAMA,qCAMA,uGASA,wCAKA,4CAIA,mDAIA,yCAIA,uCAKA,sMAYA,iCACE,8BAKF,6VAUA,8HAcA,kDAKA,yMAWA,8EAKA,iCACE,iCAKF,0FAMA,kDAIA,sLA0BA,qKAQA,2GAKA,4HAUA,iCAKA,sHAKA,sHAIA,iCACE,2BAQA,oBAWF,8BAKA,iCAIA,qCAKA,yBAWA,gCAIA,uTAUA,mIAeA,0OAQA,iCACE,kEAKF,gGAOA,oCAkCA,2CAKA,yPAcA,iCACE,4EAOF,2FAOA,iCACE,0DAMF,kKAiBA,wEAMA,wDAOA,6FAOA,gCAeA,kGASA,sCAaA,yHAOA,oEAYA,0JAaA,yFASA,yDAaA,yCAKA,oCACE,wJASA,8FAQA,kDAKF,iCACE,2BAQF,wMAUA,kKAeA,wFAMA,2IAaA,gDAMA",
     "names": [],
     "sources": [
         "app.css",
         "assets/normalize.css",
         "assets/balloon.css",
         "assets/app.scss",
         "assets/helpers.scss",
         "assets/carousel.scss",
         "assets/button.scss",
         "assets/select.scss"
     ],
     "sourcesContent": [
-        "/*! normalize.css v8.0.1 | MIT License | github.com/necolas/normalize.css */\nhtml {\n  -webkit-text-size-adjust: 100%;\n  line-height: 1.15;\n}\n\nbody {\n  margin: 0;\n}\n\nmain {\n  display: block;\n}\n\nh1 {\n  margin: .67em 0;\n  font-size: 2em;\n}\n\nhr {\n  box-sizing: content-box;\n  height: 0;\n  overflow: visible;\n}\n\npre {\n  font-family: monospace;\n  font-size: 1em;\n}\n\na {\n  background-color: #0000;\n}\n\nabbr[title] {\n  border-bottom: none;\n  -webkit-text-decoration: underline dotted;\n  text-decoration: underline dotted;\n}\n\nb, strong {\n  font-weight: bolder;\n}\n\ncode, kbd, samp {\n  font-family: monospace;\n  font-size: 1em;\n}\n\nsmall {\n  font-size: 80%;\n}\n\nsub, sup {\n  vertical-align: baseline;\n  font-size: 75%;\n  line-height: 0;\n  position: relative;\n}\n\nsub {\n  bottom: -.25em;\n}\n\nsup {\n  top: -.5em;\n}\n\nimg {\n  border-style: none;\n}\n\nbutton, input, optgroup, select, textarea {\n  margin: 0;\n  font-family: inherit;\n  font-size: 100%;\n  line-height: 1.15;\n}\n\nbutton, input {\n  overflow: visible;\n}\n\nbutton, select {\n  text-transform: none;\n}\n\nbutton, [type=\"button\"], [type=\"reset\"], [type=\"submit\"] {\n  -webkit-appearance: button;\n}\n\nbutton::-moz-focus-inner {\n  border-style: none;\n  padding: 0;\n}\n\n[type=\"button\"]::-moz-focus-inner {\n  border-style: none;\n  padding: 0;\n}\n\n[type=\"reset\"]::-moz-focus-inner {\n  border-style: none;\n  padding: 0;\n}\n\n[type=\"submit\"]::-moz-focus-inner {\n  border-style: none;\n  padding: 0;\n}\n\nbutton:-moz-focusring {\n  outline: 1px dotted ButtonText;\n}\n\n[type=\"button\"]:-moz-focusring {\n  outline: 1px dotted ButtonText;\n}\n\n[type=\"reset\"]:-moz-focusring {\n  outline: 1px dotted ButtonText;\n}\n\n[type=\"submit\"]:-moz-focusring {\n  outline: 1px dotted ButtonText;\n}\n\nfieldset {\n  padding: .35em .75em .625em;\n}\n\nlegend {\n  box-sizing: border-box;\n  color: inherit;\n  white-space: normal;\n  max-width: 100%;\n  padding: 0;\n  display: table;\n}\n\nprogress {\n  vertical-align: baseline;\n}\n\ntextarea {\n  overflow: auto;\n}\n\n[type=\"checkbox\"], [type=\"radio\"] {\n  box-sizing: border-box;\n  padding: 0;\n}\n\n[type=\"number\"]::-webkit-inner-spin-button {\n  height: auto;\n}\n\n[type=\"number\"]::-webkit-outer-spin-button {\n  height: auto;\n}\n\n[type=\"search\"] {\n  -webkit-appearance: textfield;\n  outline-offset: -2px;\n}\n\n[type=\"search\"]::-webkit-search-decoration {\n  -webkit-appearance: none;\n}\n\n::-webkit-file-upload-button {\n  -webkit-appearance: button;\n  font: inherit;\n}\n\ndetails {\n  display: block;\n}\n\nsummary {\n  display: list-item;\n}\n\ntemplate, [hidden] {\n  display: none;\n}\n\n:root {\n  --balloon-border-radius: 2px;\n  --balloon-color: #101010f2;\n  --balloon-text-color: #fff;\n  --balloon-font-size: 12px;\n  --balloon-move: 4px;\n}\n\nbutton[aria-label][data-balloon-pos] {\n  overflow: visible;\n}\n\n[aria-label][data-balloon-pos] {\n  cursor: pointer;\n  position: relative;\n}\n\n[aria-label][data-balloon-pos]:after {\n  opacity: 0;\n  pointer-events: none;\n  text-indent: 0;\n  text-shadow: none;\n  font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Oxygen, Ubuntu, Cantarell, Open Sans, Helvetica Neue, sans-serif;\n  font-style: normal;\n  font-weight: normal;\n  font-size: var(--balloon-font-size);\n  background: var(--balloon-color);\n  color: var(--balloon-text-color);\n  border-radius: 2px;\n  border-radius: var(--balloon-border-radius);\n  content: attr(aria-label);\n  white-space: nowrap;\n  z-index: 10;\n  padding: .5em 1em;\n  transition: all .18s ease-out .18s;\n  position: absolute;\n}\n\n[aria-label][data-balloon-pos]:before {\n  border: 5px solid #0000;\n  border-top-color: var(--balloon-color);\n  opacity: 0;\n  pointer-events: none;\n  content: \"\";\n  z-index: 10;\n  width: 0;\n  height: 0;\n  transition: all .18s ease-out .18s;\n  position: absolute;\n}\n\n[aria-label][data-balloon-pos]:hover:before, [aria-label][data-balloon-pos]:hover:after, [aria-label][data-balloon-pos][data-balloon-visible]:before, [aria-label][data-balloon-pos][data-balloon-visible]:after, [aria-label][data-balloon-pos]:not([data-balloon-nofocus]):focus:before, [aria-label][data-balloon-pos]:not([data-balloon-nofocus]):focus:after {\n  opacity: 1;\n  pointer-events: none;\n}\n\n[aria-label][data-balloon-pos].font-awesome:after {\n  font-family: FontAwesome, -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Oxygen, Ubuntu, Cantarell, Open Sans, Helvetica Neue, sans-serif;\n}\n\n[aria-label][data-balloon-pos][data-balloon-break]:after {\n  white-space: pre;\n}\n\n[aria-label][data-balloon-pos][data-balloon-break][data-balloon-length]:after {\n  white-space: pre-line;\n  word-break: break-word;\n}\n\n[aria-label][data-balloon-pos][data-balloon-blunt]:before, [aria-label][data-balloon-pos][data-balloon-blunt]:after {\n  transition: none;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos=\"up\"]:hover:after, [aria-label][data-balloon-pos][data-balloon-pos=\"up\"][data-balloon-visible]:after, [aria-label][data-balloon-pos][data-balloon-pos=\"down\"]:hover:after, [aria-label][data-balloon-pos][data-balloon-pos=\"down\"][data-balloon-visible]:after, [aria-label][data-balloon-pos][data-balloon-pos=\"up\"]:hover:before, [aria-label][data-balloon-pos][data-balloon-pos=\"up\"][data-balloon-visible]:before, [aria-label][data-balloon-pos][data-balloon-pos=\"down\"]:hover:before, [aria-label][data-balloon-pos][data-balloon-pos=\"down\"][data-balloon-visible]:before {\n  transform: translate(-50%);\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos*=\"-left\"]:after {\n  left: 0;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos*=\"-left\"]:before {\n  left: 5px;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos*=\"-right\"]:after {\n  right: 0;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos*=\"-right\"]:before {\n  right: 5px;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos*=\"-left\"]:hover:after, [aria-label][data-balloon-pos][data-balloon-pos*=\"-left\"][data-balloon-visible]:after, [aria-label][data-balloon-pos][data-balloon-pos*=\"-right\"]:hover:after, [aria-label][data-balloon-pos][data-balloon-pos*=\"-right\"][data-balloon-visible]:after, [aria-label][data-balloon-pos][data-balloon-pos*=\"-left\"]:hover:before, [aria-label][data-balloon-pos][data-balloon-pos*=\"-left\"][data-balloon-visible]:before, [aria-label][data-balloon-pos][data-balloon-pos*=\"-right\"]:hover:before, [aria-label][data-balloon-pos][data-balloon-pos*=\"-right\"][data-balloon-visible]:before {\n  transform: translate(0);\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos^=\"up\"]:before, [aria-label][data-balloon-pos][data-balloon-pos^=\"up\"]:after {\n  transform-origin: top;\n  transform: translate(0, var(--balloon-move));\n  bottom: 100%;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos^=\"up\"]:after {\n  margin-bottom: 10px;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos=\"up\"]:before, [aria-label][data-balloon-pos][data-balloon-pos=\"up\"]:after {\n  transform: translate(-50%, var(--balloon-move));\n  left: 50%;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos^=\"down\"]:before, [aria-label][data-balloon-pos][data-balloon-pos^=\"down\"]:after {\n  transform: translate(0, calc(var(--balloon-move) * -1));\n  top: 100%;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos^=\"down\"]:after {\n  margin-top: 10px;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos^=\"down\"]:before {\n  border: 5px solid #0000;\n  border-bottom-color: var(--balloon-color);\n  width: 0;\n  height: 0;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos=\"down\"]:after, [aria-label][data-balloon-pos][data-balloon-pos=\"down\"]:before {\n  transform: translate(-50%, calc(var(--balloon-move) * -1));\n  left: 50%;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos=\"left\"]:hover:after, [aria-label][data-balloon-pos][data-balloon-pos=\"left\"][data-balloon-visible]:after, [aria-label][data-balloon-pos][data-balloon-pos=\"right\"]:hover:after, [aria-label][data-balloon-pos][data-balloon-pos=\"right\"][data-balloon-visible]:after, [aria-label][data-balloon-pos][data-balloon-pos=\"left\"]:hover:before, [aria-label][data-balloon-pos][data-balloon-pos=\"left\"][data-balloon-visible]:before, [aria-label][data-balloon-pos][data-balloon-pos=\"right\"]:hover:before, [aria-label][data-balloon-pos][data-balloon-pos=\"right\"][data-balloon-visible]:before {\n  transform: translate(0, -50%);\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos=\"left\"]:after, [aria-label][data-balloon-pos][data-balloon-pos=\"left\"]:before {\n  transform: translate(var(--balloon-move), -50%);\n  top: 50%;\n  right: 100%;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos=\"left\"]:after {\n  margin-right: 10px;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos=\"left\"]:before {\n  border: 5px solid #0000;\n  border-left-color: var(--balloon-color);\n  width: 0;\n  height: 0;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos=\"right\"]:after, [aria-label][data-balloon-pos][data-balloon-pos=\"right\"]:before {\n  transform: translate(calc(var(--balloon-move) * -1), -50%);\n  top: 50%;\n  left: 100%;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos=\"right\"]:after {\n  margin-left: 10px;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos=\"right\"]:before {\n  border: 5px solid #0000;\n  border-right-color: var(--balloon-color);\n  width: 0;\n  height: 0;\n}\n\n[aria-label][data-balloon-pos][data-balloon-length]:after {\n  white-space: normal;\n}\n\n[aria-label][data-balloon-pos][data-balloon-length=\"small\"]:after {\n  width: 80px;\n}\n\n[aria-label][data-balloon-pos][data-balloon-length=\"medium\"]:after {\n  width: 150px;\n}\n\n[aria-label][data-balloon-pos][data-balloon-length=\"large\"]:after {\n  width: 260px;\n}\n\n[aria-label][data-balloon-pos][data-balloon-length=\"xlarge\"]:after {\n  width: 380px;\n}\n\n@media screen and (width <= 768px) {\n  [aria-label][data-balloon-pos][data-balloon-length=\"xlarge\"]:after {\n    width: 90vw;\n  }\n}\n\n[aria-label][data-balloon-pos][data-balloon-length=\"fit\"]:after {\n  width: 100%;\n}\n\n:root {\n  --color-primary: #489fd9;\n  --color-primary-light: #abd9f7;\n  --color-primary-400: #3d7da9;\n  --color-primary-300: #315d7c;\n  --color-primary-200: #253e52;\n  --color-primary-100: #151d24;\n  --color-accent: #e37dd7;\n  --color-accent-light: #f794d5;\n  --color-accent-400: #b163a8;\n  --color-accent-300: #824b7b;\n  --color-accent-200: #563351;\n  --color-accent-100: #2d1d2a;\n  --color-body: #dfedf7;\n  --color-muted: #a3c1d4;\n  --color-background: var(--color-primary-100);\n  --anchor-color: #e3ddf0;\n  --anchor-color-hover: var(--color-accent-light);\n  --border-color: var(--color-primary-300);\n  --balloon-color: var(--color-primary-400);\n  --font-size-sm: .875rem;\n  --font-size-regular: 1rem;\n  --font-size-lg: 1.25rem;\n  --font-size-xlg: 2rem;\n  --font-size-xxlg: 3rem;\n}\n\n.d-none {\n  display: none !important;\n}\n\n.d-inline {\n  display: inline !important;\n}\n\n.d-inline-block {\n  display: inline-block !important;\n}\n\n.d-block {\n  display: block !important;\n}\n\n.d-table {\n  display: table !important;\n}\n\n.d-table-row {\n  display: table-row !important;\n}\n\n.d-table-cell {\n  display: table-cell !important;\n}\n\n.d-flex {\n  display: flex !important;\n}\n\n.d-inline-flex {\n  display: inline-flex !important;\n}\n\n@media (width >= 768px) {\n  .d-md-none {\n    display: none !important;\n  }\n\n  .d-md-inline {\n    display: inline !important;\n  }\n\n  .d-md-inline-block {\n    display: inline-block !important;\n  }\n\n  .d-md-block {\n    display: block !important;\n  }\n\n  .d-md-table {\n    display: table !important;\n  }\n\n  .d-md-table-row {\n    display: table-row !important;\n  }\n\n  .d-md-table-cell {\n    display: table-cell !important;\n  }\n\n  .d-md-flex {\n    display: flex !important;\n  }\n\n  .d-md-inline-flex {\n    display: inline-flex !important;\n  }\n}\n\n.m-0 {\n  margin: 0 !important;\n}\n\n.mt-0, .my-0 {\n  margin-top: 0 !important;\n}\n\n.mr-0, .mx-0 {\n  margin-right: 0 !important;\n}\n\n.mb-0, .my-0 {\n  margin-bottom: 0 !important;\n}\n\n.ml-0, .mx-0 {\n  margin-left: 0 !important;\n}\n\n.m-1 {\n  margin: .25rem !important;\n}\n\n.mt-1, .my-1 {\n  margin-top: .25rem !important;\n}\n\n.mr-1, .mx-1 {\n  margin-right: .25rem !important;\n}\n\n.mb-1, .my-1 {\n  margin-bottom: .25rem !important;\n}\n\n.ml-1, .mx-1 {\n  margin-left: .25rem !important;\n}\n\n.m-2 {\n  margin: .5rem !important;\n}\n\n.mt-2, .my-2 {\n  margin-top: .5rem !important;\n}\n\n.mr-2, .mx-2 {\n  margin-right: .5rem !important;\n}\n\n.mb-2, .my-2 {\n  margin-bottom: .5rem !important;\n}\n\n.ml-2, .mx-2 {\n  margin-left: .5rem !important;\n}\n\n.m-3 {\n  margin: 1rem !important;\n}\n\n.mt-3, .my-3 {\n  margin-top: 1rem !important;\n}\n\n.mr-3, .mx-3 {\n  margin-right: 1rem !important;\n}\n\n.mb-3, .my-3 {\n  margin-bottom: 1rem !important;\n}\n\n.ml-3, .mx-3 {\n  margin-left: 1rem !important;\n}\n\n.m-4 {\n  margin: 1.5rem !important;\n}\n\n.mt-4, .my-4 {\n  margin-top: 1.5rem !important;\n}\n\n.mr-4, .mx-4 {\n  margin-right: 1.5rem !important;\n}\n\n.mb-4, .my-4 {\n  margin-bottom: 1.5rem !important;\n}\n\n.ml-4, .mx-4 {\n  margin-left: 1.5rem !important;\n}\n\n.m-5 {\n  margin: 2.5rem !important;\n}\n\n.mt-5, .my-5 {\n  margin-top: 2.5rem !important;\n}\n\n.mr-5, .mx-5 {\n  margin-right: 2.5rem !important;\n}\n\n.mb-5, .my-5 {\n  margin-bottom: 2.5rem !important;\n}\n\n.ml-5, .mx-5 {\n  margin-left: 2.5rem !important;\n}\n\n.p-0 {\n  padding: 0 !important;\n}\n\n.pt-0, .py-0 {\n  padding-top: 0 !important;\n}\n\n.pr-0, .px-0 {\n  padding-right: 0 !important;\n}\n\n.pb-0, .py-0 {\n  padding-bottom: 0 !important;\n}\n\n.pl-0, .px-0 {\n  padding-left: 0 !important;\n}\n\n.p-1 {\n  padding: .25rem !important;\n}\n\n.pt-1, .py-1 {\n  padding-top: .25rem !important;\n}\n\n.pr-1, .px-1 {\n  padding-right: .25rem !important;\n}\n\n.pb-1, .py-1 {\n  padding-bottom: .25rem !important;\n}\n\n.pl-1, .px-1 {\n  padding-left: .25rem !important;\n}\n\n.p-2 {\n  padding: .5rem !important;\n}\n\n.pt-2, .py-2 {\n  padding-top: .5rem !important;\n}\n\n.pr-2, .px-2 {\n  padding-right: .5rem !important;\n}\n\n.pb-2, .py-2 {\n  padding-bottom: .5rem !important;\n}\n\n.pl-2, .px-2 {\n  padding-left: .5rem !important;\n}\n\n.p-3 {\n  padding: 1rem !important;\n}\n\n.pt-3, .py-3 {\n  padding-top: 1rem !important;\n}\n\n.pr-3, .px-3 {\n  padding-right: 1rem !important;\n}\n\n.pb-3, .py-3 {\n  padding-bottom: 1rem !important;\n}\n\n.pl-3, .px-3 {\n  padding-left: 1rem !important;\n}\n\n.p-4 {\n  padding: 1.5rem !important;\n}\n\n.pt-4, .py-4 {\n  padding-top: 1.5rem !important;\n}\n\n.pr-4, .px-4 {\n  padding-right: 1.5rem !important;\n}\n\n.pb-4, .py-4 {\n  padding-bottom: 1.5rem !important;\n}\n\n.pl-4, .px-4 {\n  padding-left: 1.5rem !important;\n}\n\n.p-5 {\n  padding: 2.5rem !important;\n}\n\n.pt-5, .py-5 {\n  padding-top: 2.5rem !important;\n}\n\n.pr-5, .px-5 {\n  padding-right: 2.5rem !important;\n}\n\n.pb-5, .py-5 {\n  padding-bottom: 2.5rem !important;\n}\n\n.pl-5, .px-5 {\n  padding-left: 2.5rem !important;\n}\n\n.m-n1 {\n  margin: -.25rem !important;\n}\n\n.mt-n1, .my-n1 {\n  margin-top: -.25rem !important;\n}\n\n.mr-n1, .mx-n1 {\n  margin-right: -.25rem !important;\n}\n\n.mb-n1, .my-n1 {\n  margin-bottom: -.25rem !important;\n}\n\n.ml-n1, .mx-n1 {\n  margin-left: -.25rem !important;\n}\n\n.m-n2 {\n  margin: -.5rem !important;\n}\n\n.mt-n2, .my-n2 {\n  margin-top: -.5rem !important;\n}\n\n.mr-n2, .mx-n2 {\n  margin-right: -.5rem !important;\n}\n\n.mb-n2, .my-n2 {\n  margin-bottom: -.5rem !important;\n}\n\n.ml-n2, .mx-n2 {\n  margin-left: -.5rem !important;\n}\n\n.m-n3 {\n  margin: -1rem !important;\n}\n\n.mt-n3, .my-n3 {\n  margin-top: -1rem !important;\n}\n\n.mr-n3, .mx-n3 {\n  margin-right: -1rem !important;\n}\n\n.mb-n3, .my-n3 {\n  margin-bottom: -1rem !important;\n}\n\n.ml-n3, .mx-n3 {\n  margin-left: -1rem !important;\n}\n\n.m-n4 {\n  margin: -1.5rem !important;\n}\n\n.mt-n4, .my-n4 {\n  margin-top: -1.5rem !important;\n}\n\n.mr-n4, .mx-n4 {\n  margin-right: -1.5rem !important;\n}\n\n.mb-n4, .my-n4 {\n  margin-bottom: -1.5rem !important;\n}\n\n.ml-n4, .mx-n4 {\n  margin-left: -1.5rem !important;\n}\n\n.m-n5 {\n  margin: -2.5rem !important;\n}\n\n.mt-n5, .my-n5 {\n  margin-top: -2.5rem !important;\n}\n\n.mr-n5, .mx-n5 {\n  margin-right: -2.5rem !important;\n}\n\n.mb-n5, .my-n5 {\n  margin-bottom: -2.5rem !important;\n}\n\n.ml-n5, .mx-n5 {\n  margin-left: -2.5rem !important;\n}\n\n.m-auto {\n  margin: auto !important;\n}\n\n.mt-auto, .my-auto {\n  margin-top: auto !important;\n}\n\n.mr-auto, .mx-auto {\n  margin-right: auto !important;\n}\n\n.mb-auto, .my-auto {\n  margin-bottom: auto !important;\n}\n\n.ml-auto, .mx-auto {\n  margin-left: auto !important;\n}\n\n@media (width >= 768px) {\n  .m-md-0 {\n    margin: 0 !important;\n  }\n\n  .mt-md-0, .my-md-0 {\n    margin-top: 0 !important;\n  }\n\n  .mr-md-0, .mx-md-0 {\n    margin-right: 0 !important;\n  }\n\n  .mb-md-0, .my-md-0 {\n    margin-bottom: 0 !important;\n  }\n\n  .ml-md-0, .mx-md-0 {\n    margin-left: 0 !important;\n  }\n\n  .m-md-1 {\n    margin: .25rem !important;\n  }\n\n  .mt-md-1, .my-md-1 {\n    margin-top: .25rem !important;\n  }\n\n  .mr-md-1, .mx-md-1 {\n    margin-right: .25rem !important;\n  }\n\n  .mb-md-1, .my-md-1 {\n    margin-bottom: .25rem !important;\n  }\n\n  .ml-md-1, .mx-md-1 {\n    margin-left: .25rem !important;\n  }\n\n  .m-md-2 {\n    margin: .5rem !important;\n  }\n\n  .mt-md-2, .my-md-2 {\n    margin-top: .5rem !important;\n  }\n\n  .mr-md-2, .mx-md-2 {\n    margin-right: .5rem !important;\n  }\n\n  .mb-md-2, .my-md-2 {\n    margin-bottom: .5rem !important;\n  }\n\n  .ml-md-2, .mx-md-2 {\n    margin-left: .5rem !important;\n  }\n\n  .m-md-3 {\n    margin: 1rem !important;\n  }\n\n  .mt-md-3, .my-md-3 {\n    margin-top: 1rem !important;\n  }\n\n  .mr-md-3, .mx-md-3 {\n    margin-right: 1rem !important;\n  }\n\n  .mb-md-3, .my-md-3 {\n    margin-bottom: 1rem !important;\n  }\n\n  .ml-md-3, .mx-md-3 {\n    margin-left: 1rem !important;\n  }\n\n  .m-md-4 {\n    margin: 1.5rem !important;\n  }\n\n  .mt-md-4, .my-md-4 {\n    margin-top: 1.5rem !important;\n  }\n\n  .mr-md-4, .mx-md-4 {\n    margin-right: 1.5rem !important;\n  }\n\n  .mb-md-4, .my-md-4 {\n    margin-bottom: 1.5rem !important;\n  }\n\n  .ml-md-4, .mx-md-4 {\n    margin-left: 1.5rem !important;\n  }\n\n  .m-md-5 {\n    margin: 2.5rem !important;\n  }\n\n  .mt-md-5, .my-md-5 {\n    margin-top: 2.5rem !important;\n  }\n\n  .mr-md-5, .mx-md-5 {\n    margin-right: 2.5rem !important;\n  }\n\n  .mb-md-5, .my-md-5 {\n    margin-bottom: 2.5rem !important;\n  }\n\n  .ml-md-5, .mx-md-5 {\n    margin-left: 2.5rem !important;\n  }\n\n  .p-md-0 {\n    padding: 0 !important;\n  }\n\n  .pt-md-0, .py-md-0 {\n    padding-top: 0 !important;\n  }\n\n  .pr-md-0, .px-md-0 {\n    padding-right: 0 !important;\n  }\n\n  .pb-md-0, .py-md-0 {\n    padding-bottom: 0 !important;\n  }\n\n  .pl-md-0, .px-md-0 {\n    padding-left: 0 !important;\n  }\n\n  .p-md-1 {\n    padding: .25rem !important;\n  }\n\n  .pt-md-1, .py-md-1 {\n    padding-top: .25rem !important;\n  }\n\n  .pr-md-1, .px-md-1 {\n    padding-right: .25rem !important;\n  }\n\n  .pb-md-1, .py-md-1 {\n    padding-bottom: .25rem !important;\n  }\n\n  .pl-md-1, .px-md-1 {\n    padding-left: .25rem !important;\n  }\n\n  .p-md-2 {\n    padding: .5rem !important;\n  }\n\n  .pt-md-2, .py-md-2 {\n    padding-top: .5rem !important;\n  }\n\n  .pr-md-2, .px-md-2 {\n    padding-right: .5rem !important;\n  }\n\n  .pb-md-2, .py-md-2 {\n    padding-bottom: .5rem !important;\n  }\n\n  .pl-md-2, .px-md-2 {\n    padding-left: .5rem !important;\n  }\n\n  .p-md-3 {\n    padding: 1rem !important;\n  }\n\n  .pt-md-3, .py-md-3 {\n    padding-top: 1rem !important;\n  }\n\n  .pr-md-3, .px-md-3 {\n    padding-right: 1rem !important;\n  }\n\n  .pb-md-3, .py-md-3 {\n    padding-bottom: 1rem !important;\n  }\n\n  .pl-md-3, .px-md-3 {\n    padding-left: 1rem !important;\n  }\n\n  .p-md-4 {\n    padding: 1.5rem !important;\n  }\n\n  .pt-md-4, .py-md-4 {\n    padding-top: 1.5rem !important;\n  }\n\n  .pr-md-4, .px-md-4 {\n    padding-right: 1.5rem !important;\n  }\n\n  .pb-md-4, .py-md-4 {\n    padding-bottom: 1.5rem !important;\n  }\n\n  .pl-md-4, .px-md-4 {\n    padding-left: 1.5rem !important;\n  }\n\n  .p-md-5 {\n    padding: 2.5rem !important;\n  }\n\n  .pt-md-5, .py-md-5 {\n    padding-top: 2.5rem !important;\n  }\n\n  .pr-md-5, .px-md-5 {\n    padding-right: 2.5rem !important;\n  }\n\n  .pb-md-5, .py-md-5 {\n    padding-bottom: 2.5rem !important;\n  }\n\n  .pl-md-5, .px-md-5 {\n    padding-left: 2.5rem !important;\n  }\n\n  .m-md-n1 {\n    margin: -.25rem !important;\n  }\n\n  .mt-md-n1, .my-md-n1 {\n    margin-top: -.25rem !important;\n  }\n\n  .mr-md-n1, .mx-md-n1 {\n    margin-right: -.25rem !important;\n  }\n\n  .mb-md-n1, .my-md-n1 {\n    margin-bottom: -.25rem !important;\n  }\n\n  .ml-md-n1, .mx-md-n1 {\n    margin-left: -.25rem !important;\n  }\n\n  .m-md-n2 {\n    margin: -.5rem !important;\n  }\n\n  .mt-md-n2, .my-md-n2 {\n    margin-top: -.5rem !important;\n  }\n\n  .mr-md-n2, .mx-md-n2 {\n    margin-right: -.5rem !important;\n  }\n\n  .mb-md-n2, .my-md-n2 {\n    margin-bottom: -.5rem !important;\n  }\n\n  .ml-md-n2, .mx-md-n2 {\n    margin-left: -.5rem !important;\n  }\n\n  .m-md-n3 {\n    margin: -1rem !important;\n  }\n\n  .mt-md-n3, .my-md-n3 {\n    margin-top: -1rem !important;\n  }\n\n  .mr-md-n3, .mx-md-n3 {\n    margin-right: -1rem !important;\n  }\n\n  .mb-md-n3, .my-md-n3 {\n    margin-bottom: -1rem !important;\n  }\n\n  .ml-md-n3, .mx-md-n3 {\n    margin-left: -1rem !important;\n  }\n\n  .m-md-n4 {\n    margin: -1.5rem !important;\n  }\n\n  .mt-md-n4, .my-md-n4 {\n    margin-top: -1.5rem !important;\n  }\n\n  .mr-md-n4, .mx-md-n4 {\n    margin-right: -1.5rem !important;\n  }\n\n  .mb-md-n4, .my-md-n4 {\n    margin-bottom: -1.5rem !important;\n  }\n\n  .ml-md-n4, .mx-md-n4 {\n    margin-left: -1.5rem !important;\n  }\n\n  .m-md-n5 {\n    margin: -2.5rem !important;\n  }\n\n  .mt-md-n5, .my-md-n5 {\n    margin-top: -2.5rem !important;\n  }\n\n  .mr-md-n5, .mx-md-n5 {\n    margin-right: -2.5rem !important;\n  }\n\n  .mb-md-n5, .my-md-n5 {\n    margin-bottom: -2.5rem !important;\n  }\n\n  .ml-md-n5, .mx-md-n5 {\n    margin-left: -2.5rem !important;\n  }\n\n  .m-md-auto {\n    margin: auto !important;\n  }\n\n  .mt-md-auto, .my-md-auto {\n    margin-top: auto !important;\n  }\n\n  .mr-md-auto, .mx-md-auto {\n    margin-right: auto !important;\n  }\n\n  .mb-md-auto, .my-md-auto {\n    margin-bottom: auto !important;\n  }\n\n  .ml-md-auto, .mx-md-auto {\n    margin-left: auto !important;\n  }\n}\n\n.flex-row {\n  flex-direction: row !important;\n}\n\n.flex-column {\n  flex-direction: column !important;\n}\n\n.flex-row-reverse {\n  flex-direction: row-reverse !important;\n}\n\n.flex-column-reverse {\n  flex-direction: column-reverse !important;\n}\n\n.flex-wrap {\n  flex-wrap: wrap !important;\n}\n\n.flex-nowrap {\n  flex-wrap: nowrap !important;\n}\n\n.flex-wrap-reverse {\n  flex-wrap: wrap-reverse !important;\n}\n\n.flex-fill {\n  flex: auto !important;\n}\n\n.flex-grow-0 {\n  flex-grow: 0 !important;\n}\n\n.flex-grow-1 {\n  flex-grow: 1 !important;\n}\n\n.flex-shrink-0 {\n  flex-shrink: 0 !important;\n}\n\n.flex-shrink-1 {\n  flex-shrink: 1 !important;\n}\n\n.justify-content-start {\n  justify-content: flex-start !important;\n}\n\n.justify-content-end {\n  justify-content: flex-end !important;\n}\n\n.justify-content-center {\n  justify-content: center !important;\n}\n\n.justify-content-between {\n  justify-content: space-between !important;\n}\n\n.justify-content-around {\n  justify-content: space-around !important;\n}\n\n.align-items-start {\n  align-items: flex-start !important;\n}\n\n.align-items-end {\n  align-items: flex-end !important;\n}\n\n.align-items-center {\n  align-items: center !important;\n}\n\n.align-items-baseline {\n  align-items: baseline !important;\n}\n\n.align-items-stretch {\n  align-items: stretch !important;\n}\n\n.align-content-start {\n  align-content: flex-start !important;\n}\n\n.align-content-end {\n  align-content: flex-end !important;\n}\n\n.align-content-center {\n  align-content: center !important;\n}\n\n.align-content-between {\n  align-content: space-between !important;\n}\n\n.align-content-around {\n  align-content: space-around !important;\n}\n\n.align-content-stretch {\n  align-content: stretch !important;\n}\n\n.align-self-auto {\n  align-self: auto !important;\n}\n\n.align-self-start {\n  align-self: flex-start !important;\n}\n\n.align-self-end {\n  align-self: flex-end !important;\n}\n\n.align-self-center {\n  align-self: center !important;\n}\n\n.align-self-baseline {\n  align-self: baseline !important;\n}\n\n.align-self-stretch {\n  align-self: stretch !important;\n}\n\n@media (width >= 768px) {\n  .flex-md-row {\n    flex-direction: row !important;\n  }\n\n  .flex-md-column {\n    flex-direction: column !important;\n  }\n\n  .flex-md-row-reverse {\n    flex-direction: row-reverse !important;\n  }\n\n  .flex-md-column-reverse {\n    flex-direction: column-reverse !important;\n  }\n\n  .flex-md-wrap {\n    flex-wrap: wrap !important;\n  }\n\n  .flex-md-nowrap {\n    flex-wrap: nowrap !important;\n  }\n\n  .flex-md-wrap-reverse {\n    flex-wrap: wrap-reverse !important;\n  }\n\n  .flex-md-fill {\n    flex: auto !important;\n  }\n\n  .flex-md-grow-0 {\n    flex-grow: 0 !important;\n  }\n\n  .flex-md-grow-1 {\n    flex-grow: 1 !important;\n  }\n\n  .flex-md-shrink-0 {\n    flex-shrink: 0 !important;\n  }\n\n  .flex-md-shrink-1 {\n    flex-shrink: 1 !important;\n  }\n\n  .justify-content-md-start {\n    justify-content: flex-start !important;\n  }\n\n  .justify-content-md-end {\n    justify-content: flex-end !important;\n  }\n\n  .justify-content-md-center {\n    justify-content: center !important;\n  }\n\n  .justify-content-md-between {\n    justify-content: space-between !important;\n  }\n\n  .justify-content-md-around {\n    justify-content: space-around !important;\n  }\n\n  .align-items-md-start {\n    align-items: flex-start !important;\n  }\n\n  .align-items-md-end {\n    align-items: flex-end !important;\n  }\n\n  .align-items-md-center {\n    align-items: center !important;\n  }\n\n  .align-items-md-baseline {\n    align-items: baseline !important;\n  }\n\n  .align-items-md-stretch {\n    align-items: stretch !important;\n  }\n\n  .align-content-md-start {\n    align-content: flex-start !important;\n  }\n\n  .align-content-md-end {\n    align-content: flex-end !important;\n  }\n\n  .align-content-md-center {\n    align-content: center !important;\n  }\n\n  .align-content-md-between {\n    align-content: space-between !important;\n  }\n\n  .align-content-md-around {\n    align-content: space-around !important;\n  }\n\n  .align-content-md-stretch {\n    align-content: stretch !important;\n  }\n\n  .align-self-md-auto {\n    align-self: auto !important;\n  }\n\n  .align-self-md-start {\n    align-self: flex-start !important;\n  }\n\n  .align-self-md-end {\n    align-self: flex-end !important;\n  }\n\n  .align-self-md-center {\n    align-self: center !important;\n  }\n\n  .align-self-md-baseline {\n    align-self: baseline !important;\n  }\n\n  .align-self-md-stretch {\n    align-self: stretch !important;\n  }\n}\n\nsmall, .text-sm {\n  font-size: var(--font-size-sm) !important;\n}\n\n.text-regular {\n  font-size: var(--font-size-regular) !important;\n}\n\n.text-lg {\n  font-size: var(--font-size-lg) !important;\n}\n\n.text-xlg {\n  font-size: var(--font-size-xlg) !important;\n}\n\n.text-right {\n  text-align: right;\n}\n\n.text-left {\n  text-align: left;\n}\n\n.text-center {\n  text-align: center;\n}\n\n.text-muted {\n  color: var(--color-muted) !important;\n}\n\n.text-uppercase {\n  text-transform: uppercase;\n}\n\n.font-weight-normal {\n  font-weight: normal;\n}\n\n.font-weight-bold {\n  font-weight: bold;\n}\n\n.font-weight-semibold {\n  font-weight: 600;\n}\n\n.font-weight-black {\n  font-weight: 900;\n}\n\n.font-style-italic {\n  font-style: italic;\n}\n\n.line-height-1 {\n  line-height: 1;\n}\n\n.text-decoration-none {\n  text-decoration: none;\n}\n\n.text-break-all {\n  word-break: break-all;\n}\n\n.text-nowrap {\n  white-space: nowrap;\n}\n\n.position-relative {\n  position: relative;\n}\n\n.img-fluid {\n  max-width: 100%;\n  height: auto;\n}\n\n.zero {\n  margin: 0;\n  padding: 0;\n}\n\n.invisible {\n  visibility: hidden;\n}\n\n.h-100 {\n  height: 100%;\n}\n\n.w-100 {\n  width: 100%;\n}\n\n.d-grid {\n  grid-auto-columns: 1fr;\n  grid-auto-flow: column;\n  display: grid;\n}\n\n.rounded {\n  border-radius: .5rem;\n}\n\n.border {\n  border: 1px solid var(--border-color);\n}\n\n.border-top {\n  border-top: 1px solid var(--color-primary-300);\n}\n\n.border-bottom {\n  border-bottom: 1px solid var(--color-primary-300);\n}\n\n.border-right {\n  border-right: 1px solid var(--color-primary-300);\n}\n\n.border-left {\n  border-left: 1px solid var(--color-primary-300);\n}\n\n.carousel {\n  margin: 0 -3rem;\n  position: relative;\n}\n\n.carousel__items {\n  scroll-behavior: smooth;\n  -webkit-overflow-scrolling: touch;\n  scroll-snap-type: x mandatory;\n  scroll-snap-align: start;\n  scrollbar-width: none;\n  -ms-overflow-style: none;\n  gap: 2rem;\n  width: 100%;\n  display: flex;\n  overflow-x: scroll;\n}\n\n.carousel-item {\n  flex-shrink: 0;\n  max-width: 300px;\n}\n\n.carousel-item:first-child {\n  padding-left: 3rem;\n}\n\n.carousel-item:last-child {\n  padding-right: 3rem;\n}\n\n.carousel__items::-webkit-scrollbar {\n  display: none;\n}\n\n.carousel__next, .carousel__prev {\n  z-index: 1;\n  position: absolute;\n  top: calc(50% - 12px);\n  left: 0;\n}\n\n.carousel__next {\n  left: unset;\n  right: 0;\n}\n\n.btn {\n  text-transform: uppercase;\n  font-size: var(--font-size-sm);\n  letter-spacing: .05rem;\n  cursor: pointer;\n  background: var(--color-background);\n  border: 2px solid var(--color-primary-400);\n  color: var(--color-primary-light);\n  border-radius: .5rem;\n  padding: .75rem;\n  font-weight: bold;\n  transition: border-color .1s ease-in;\n}\n\n.btn-small {\n  text-transform: uppercase;\n  font-size: var(--font-size-sm);\n  cursor: pointer;\n  background: var(--color-background);\n  border: 2px solid var(--color-primary-400);\n  color: var(--color-primary-light);\n  border-radius: .5rem;\n  padding: .5rem;\n  font-weight: bold;\n}\n\n.btn-small:hover, .btn:hover {\n  border-color: var(--anchor-color-hover);\n  color: var(--anchor-color-hover);\n}\n\n.btn img, .btn-small img {\n  filter: invert(77%) sepia(40%) saturate(250%) hue-rotate(164deg) brightness() contrast(94%);\n}\n\n.btn:hover img, .btn-small:hover img {\n  filter: invert(85%) sepia(46%) saturate(3508%) hue-rotate(287deg) brightness(112%) contrast(94%);\n}\n\n.btn-text {\n  color: inherit;\n  font-size: inherit;\n  cursor: pointer;\n  background: none;\n  border: 0;\n  margin: 0;\n  padding: 0;\n  transition: color .1s ease-in;\n}\n\n.btn-text:hover {\n  color: var(--anchor-color-hover) !important;\n}\n\n.btn-icon {\n  cursor: pointer;\n  color: inherit;\n  background: none;\n  border: 0;\n  align-items: center;\n  transition: color .1s ease-in;\n  display: inline-flex;\n}\n\nselect {\n  border: 2px solid var(--color-primary-400);\n  color: var(--color-primary-light);\n  font-size: var(--font-size-sm);\n  appearance: none;\n  background: var(--color-background) url(\"data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='100' height='100' fill='%233d8fa9'><polygon points='0,0 100,0 50,50'/></svg>\") no-repeat;\n  background-position: right .75em top 65%;\n  background-repeat: no-repeat;\n  background-size: 12px;\n  border-radius: .5rem;\n  min-width: 20ch;\n  padding: .5rem 2rem .5rem .5rem;\n}\n\nselect:focus-visible {\n  border: 2px solid var(--anchor-color-hover);\n  color: var(--anchor-color-hover);\n  outline: none;\n}\n\nh1, h2, h3, h4, h5, h6, p {\n  margin: 0;\n}\n\nbody {\n  color: var(--color-body);\n  background-color: var(--color-background);\n  font: 1rem / 1.5 system-ui, sans-serif;\n  display: flex;\n}\n\nh1, h2, h3, h4, h5, h6 {\n  line-height: 1.1;\n}\n\na {\n  color: inherit;\n  transition: color .1s ease-in;\n}\n\na:hover {\n  color: var(--anchor-color-hover);\n}\n\na:visited {\n  -webkit-text-decoration: none;\n  text-decoration: none;\n}\n\n:target {\n  color: var(--anchor-color-hover);\n}\n\ncode {\n  font-family: ui-monospace, Menlo, Monaco, Courier New, monospace;\n}\n\nhr {\n  border-top: 1px solid var(--border-color);\n  border-bottom: 0;\n}\n\ndt {\n  font-size: var(--font-size-sm);\n  text-transform: uppercase;\n  color: var(--color-muted);\n  font-weight: 600;\n}\n\ndd {\n  font-size: var(--font-size-sm);\n  margin: 0 0 1rem;\n}\n\n.badge {\n  color: var(--color-muted);\n  background-color: var(--color-primary-300);\n  border-radius: .5rem;\n  padding: .1875rem .375rem;\n  text-decoration: none;\n}\n\n.badge--outline {\n  border: 2px solid var(--color-primary-300);\n  color: var(--color-muted);\n  border-radius: .5rem;\n  padding: .1875rem .375rem;\n  text-decoration: none;\n  transition: border-color .1s ease-in;\n}\n\n.badge--outline:hover {\n  border-color: var(--anchor-color-hover);\n}\n\n.badge--pill {\n  border-radius: 1rem;\n}\n\n.badge-res {\n  background: var(--color-primary-200);\n  color: #fff;\n  text-shadow: 1px 1px #4d5078;\n  border-radius: 4px;\n  padding: 0 3px;\n  font-size: 12px;\n}\n\n.badge-2160 {\n  background: #b82927;\n}\n\n.badge-1080 {\n  background: #e0560b;\n}\n\n.badge-720 {\n  background: var(--color-accent);\n}\n\n.badge-480 {\n  background: #269ddb;\n}\n\n.torrent-medium {\n  color: #f0ed60;\n}\n\n.torrent-low {\n  color: #cf4d4a;\n}\n\nfieldset {\n  border: 0;\n  margin: 0;\n  padding: 0;\n}\n\nlegend {\n  font-size: var(--font-size-sm);\n  text-transform: uppercase;\n  color: var(--color-muted);\n  font-weight: 600;\n}\n\n.report, .table {\n  border-collapse: collapse;\n}\n\n.table td {\n  padding: .1875rem .5rem .1875rem 0;\n}\n\n.table tr {\n  transition: background-color .1s ease-out;\n}\n\n.table tr:hover {\n  background-color: #253e52;\n}\n\n.report td {\n  border-bottom: 1px solid var(--color-primary-200);\n  padding: .5em 0;\n}\n\n.report th, .table th {\n  border-bottom: 1px solid var(--color-primary-200);\n  color: var(--color-muted);\n  text-transform: uppercase;\n  font-weight: 600;\n  font-size: var(--font-size-sm);\n  padding: .375rem .5rem .375rem 0;\n}\n\n@media screen and (width >= 768px) {\n  .card-series {\n    max-width: 10rem;\n  }\n}\n\n.card-series__image {\n  aspect-ratio: 500 / 750;\n  border: 2px solid var(--color-primary-200);\n  box-shadow: var(--color-primary-200) 0 0;\n  background-color: var(--color-accent-200);\n  background-position: 0 0;\n  background-image: linear-gradient(125deg, var(--color-accent-400) 25%, transparent 25%);\n  transition: transform .2s ease-out, filter .3s ease-out, box-shadow .2s ease-out;\n}\n\na:hover .card-series__image {\n  filter: brightness(1.25);\n  box-shadow: var(--color-primary-200) 7px 7px;\n  transform: translate(-7px, -7px);\n}\n\n.search-query {\n  width: min-content;\n  position: relative;\n}\n\n.search-query input {\n  background: var(--color-background);\n  border: 2px solid var(--color-primary-400);\n  color: var(--color-primary-light);\n  font-size: var(--font-size-lg);\n  border-radius: .5rem;\n  padding: .75rem .5rem;\n}\n\n.search-query input::-webkit-calendar-picker-indicator {\n  display: none !important;\n}\n\n@media screen and (width >= 768px) {\n  .search-query input {\n    width: 30rem;\n  }\n}\n\n.search-query input:focus-visible {\n  border: 2px solid var(--anchor-color-hover);\n  outline: none;\n}\n\ninput::placeholder {\n  color: var(--color-primary-300);\n}\n\n.search-query button {\n  z-index: 1;\n  background: var(--color-background);\n  cursor: pointer;\n  font-size: var(--font-size-lg);\n  background: none;\n  border: 0;\n  padding: .75rem;\n  position: absolute;\n  top: 0;\n  right: 0;\n}\n\na:hover .card-episode__poster, a:hover .card-episode__image, .btn-text:hover .card-episode__image {\n  border-color: var(--color-accent);\n  transition: border-color .1s ease-in;\n}\n\n.header .btn-icon:hover {\n  background-color: var(--color-primary-300);\n  transition: background-color .2s ease-out;\n}\n\n.header {\n  background: var(--color-primary-200);\n  flex-direction: column;\n  gap: .5rem;\n  height: 100vh;\n  display: flex;\n  position: sticky;\n  top: 0;\n}\n\n.header .btn-icon {\n  padding: .75rem;\n}\n\n.icon, .header .btn-icon img {\n  filter: invert(88%) sepia(3%) saturate(2496%) hue-rotate(185deg) brightness(106%) contrast(94%);\n}\n\n.header .btn-icon:hover img {\n  filter: invert(78%) sepia(13%) saturate(3097%) hue-rotate(274deg) brightness(96%) contrast(85%);\n}\n\n@media screen and (width >= 768px) {\n  .header {\n    align-items: center;\n  }\n\n  nav {\n    background: none;\n  }\n}\n\nmain {\n  flex-grow: 1;\n  padding: 3rem;\n}\n\n.footer {\n  color: var(--color-muted);\n}\n\naside {\n  flex-shrink: 0;\n  flex-basis: 14rem;\n}\n\n.main-column {\n  flex-grow: 1;\n}\n\n.card-episode {\n  position: relative;\n}\n\n.card-episode__image {\n  aspect-ratio: 300 / 170;\n  border: 2px solid var(--color-primary-300);\n  background-position: 0 0;\n  background-color: var(--color-accent-200);\n  background-image: linear-gradient(125deg, var(--color-accent-400) 25%, transparent 25%);\n  transition: transform .2s ease-out, filter .3s ease-out, box-shadow .2s ease-out;\n}\n\n.card-episode__poster {\n  z-index: 1;\n  border: 2px solid var(--color-primary-300);\n  max-width: 75px;\n  position: absolute;\n  bottom: -1rem;\n  right: 1rem;\n}\n\n.series-poster__image {\n  aspect-ratio: 500 / 750;\n  border: 2px solid var(--color-primary-200);\n  background-position: 0 0;\n  background-color: var(--color-accent-200);\n  background-image: linear-gradient(125deg, var(--color-accent-400) 25%, transparent 25%);\n}\n\n@media screen and (width >= 768px) {\n  .series-poster__image {\n    box-shadow: var(--color-primary-200) 7px 7px;\n  }\n}\n\n.episode-grid {\n  grid-template-rows: auto;\n  grid-template-columns: repeat(4, 1fr);\n  gap: 2rem;\n  display: grid;\n}\n\n.episode-grid__cell {\n  max-width: 300px;\n}\n\n.body-copy, .series-overview {\n  max-width: 75ch;\n}\n\n.fanart {\n  background-blend-mode: multiply;\n  background-position: top;\n  background-repeat: no-repeat;\n  background-size: cover;\n  background-attachment: fixed;\n  background-color: var(--color-accent-100);\n  margin-top: -3rem;\n  margin-left: -3rem;\n  margin-right: -3rem;\n  padding: 3rem;\n}\n\n@media screen and (width >= 768px) {\n  .top-series-grid {\n    grid-template-columns: repeat(2, 1fr);\n    gap: 2rem;\n    display: grid;\n  }\n}\n\n.cards-grid {\n  grid-template-columns: repeat(3, 1fr);\n  gap: 1.5rem;\n  margin-bottom: 2rem;\n  display: grid;\n}\n\n@media screen and (width >= 768px) {\n  .cards-grid {\n    grid-template-columns: repeat(6, 1fr);\n    gap: 2rem;\n  }\n}\n\ndialog {\n  opacity: 0;\n  color: var(--color-body);\n  max-width: unset;\n  max-height: unset;\n  background: none;\n  border: 0;\n  width: 100vw;\n  height: 100vh;\n  margin: 0;\n  padding: 0;\n}\n\n.dialog-body {\n  background: var(--color-primary-200);\n  border-radius: 1rem;\n  width: 30rem;\n  padding: 2rem;\n}\n\n.dialog-body--small {\n  width: 16rem;\n}\n\ndialog:modal {\n  opacity: 1;\n  justify-content: center;\n  align-items: center;\n  display: flex;\n}\n\ndialog::backdrop {\n  background: #151d27bf;\n}\n\ndialog button[name=\"close\"] {\n  z-index: 1;\n  position: absolute;\n  top: 0;\n  right: 0;\n}\n\n.anim-spin {\n  animation-name: spin;\n  animation-duration: 4s;\n  animation-timing-function: linear;\n  animation-iteration-count: infinite;\n}\n\n@keyframes spin {\n  from {\n    transform: rotate(0);\n  }\n\n  to {\n    transform: rotate(360deg);\n  }\n}\n\n.sr-only {\n  white-space: nowrap;\n  clip: rect(0 0 0 0);\n  clip-path: inset(50%);\n  border: 0;\n  width: 1px;\n  height: 1px;\n  margin: -1px;\n  padding: 0;\n  position: absolute;\n  overflow: hidden;\n}\n\n.skip-nav a {\n  width: 1px;\n  height: 1px;\n  position: absolute;\n  top: auto;\n  left: -9999px;\n  overflow: hidden;\n}\n\n.skip-nav a:focus {\n  width: auto;\n  height: auto;\n  position: static;\n}\n\n.mobile-carousel {\n  gap: 1.5rem;\n  display: flex;\n}\n\n@media screen and (width <= 767.98px) {\n  .mobile-carousel {\n    scroll-behavior: smooth;\n    -webkit-overflow-scrolling: touch;\n    scroll-snap-type: x mandatory;\n    margin: 0 -1rem 0 0;\n    display: flex;\n    overflow-x: scroll;\n  }\n\n  .mobile-carousel > .mobile-carousel__item {\n    scroll-snap-align: start;\n    flex-shrink: 0;\n    flex-basis: 50vw;\n  }\n\n  .mobile-carousel::-webkit-scrollbar {\n    display: none;\n  }\n}\n\n@media screen and (width >= 768px) {\n  .mobile-carousel {\n    gap: 2rem;\n  }\n}\n\n.radio-button-group {\n  border: 2px solid var(--color-primary-400);\n  color: var(--color-primary-light);\n  font-size: var(--font-size-sm);\n  background-color: var(--color-primary-100);\n  border-radius: .5rem;\n  display: flex;\n}\n\n.radio-button-group__label {\n  color: var(--color-body);\n  cursor: pointer;\n  background-color: #0000;\n  border-radius: .4rem;\n  align-items: center;\n  padding: .5rem;\n  display: inline-flex;\n}\n\n.radio-button-group__label:has(input:checked) {\n  background-color: var(--color-primary-300);\n}\n\n.radio-button-group__input {\n  clip: rect(0, 0, 0, 0);\n  white-space: nowrap;\n  border: 0;\n  width: 1px;\n  height: 1px;\n  padding: 0;\n  position: absolute;\n  overflow: hidden;\n}\n\nprogress {\n  accent-color: var(--color-accent-light);\n}\n\n/*# sourceMappingURL=app.css.map */\n",
+        "/*! normalize.css v8.0.1 | MIT License | github.com/necolas/normalize.css */\nhtml {\n  -webkit-text-size-adjust: 100%;\n  line-height: 1.15;\n}\n\nbody {\n  margin: 0;\n}\n\nmain {\n  display: block;\n}\n\nh1 {\n  margin: .67em 0;\n  font-size: 2em;\n}\n\nhr {\n  box-sizing: content-box;\n  height: 0;\n  overflow: visible;\n}\n\npre {\n  font-family: monospace;\n  font-size: 1em;\n}\n\na {\n  background-color: #0000;\n}\n\nabbr[title] {\n  border-bottom: none;\n  -webkit-text-decoration: underline dotted;\n  text-decoration: underline dotted;\n}\n\nb, strong {\n  font-weight: bolder;\n}\n\ncode, kbd, samp {\n  font-family: monospace;\n  font-size: 1em;\n}\n\nsmall {\n  font-size: 80%;\n}\n\nsub, sup {\n  vertical-align: baseline;\n  font-size: 75%;\n  line-height: 0;\n  position: relative;\n}\n\nsub {\n  bottom: -.25em;\n}\n\nsup {\n  top: -.5em;\n}\n\nimg {\n  border-style: none;\n}\n\nbutton, input, optgroup, select, textarea {\n  margin: 0;\n  font-family: inherit;\n  font-size: 100%;\n  line-height: 1.15;\n}\n\nbutton, input {\n  overflow: visible;\n}\n\nbutton, select {\n  text-transform: none;\n}\n\nbutton, [type=\"button\"], [type=\"reset\"], [type=\"submit\"] {\n  -webkit-appearance: button;\n}\n\nbutton::-moz-focus-inner {\n  border-style: none;\n  padding: 0;\n}\n\n[type=\"button\"]::-moz-focus-inner {\n  border-style: none;\n  padding: 0;\n}\n\n[type=\"reset\"]::-moz-focus-inner {\n  border-style: none;\n  padding: 0;\n}\n\n[type=\"submit\"]::-moz-focus-inner {\n  border-style: none;\n  padding: 0;\n}\n\nbutton:-moz-focusring {\n  outline: 1px dotted ButtonText;\n}\n\n[type=\"button\"]:-moz-focusring {\n  outline: 1px dotted ButtonText;\n}\n\n[type=\"reset\"]:-moz-focusring {\n  outline: 1px dotted ButtonText;\n}\n\n[type=\"submit\"]:-moz-focusring {\n  outline: 1px dotted ButtonText;\n}\n\nfieldset {\n  padding: .35em .75em .625em;\n}\n\nlegend {\n  box-sizing: border-box;\n  color: inherit;\n  white-space: normal;\n  max-width: 100%;\n  padding: 0;\n  display: table;\n}\n\nprogress {\n  vertical-align: baseline;\n}\n\ntextarea {\n  overflow: auto;\n}\n\n[type=\"checkbox\"], [type=\"radio\"] {\n  box-sizing: border-box;\n  padding: 0;\n}\n\n[type=\"number\"]::-webkit-inner-spin-button {\n  height: auto;\n}\n\n[type=\"number\"]::-webkit-outer-spin-button {\n  height: auto;\n}\n\n[type=\"search\"] {\n  -webkit-appearance: textfield;\n  outline-offset: -2px;\n}\n\n[type=\"search\"]::-webkit-search-decoration {\n  -webkit-appearance: none;\n}\n\n::-webkit-file-upload-button {\n  -webkit-appearance: button;\n  font: inherit;\n}\n\ndetails {\n  display: block;\n}\n\nsummary {\n  display: list-item;\n}\n\ntemplate, [hidden] {\n  display: none;\n}\n\n:root {\n  --balloon-border-radius: 2px;\n  --balloon-color: #101010f2;\n  --balloon-text-color: #fff;\n  --balloon-font-size: 12px;\n  --balloon-move: 4px;\n}\n\nbutton[aria-label][data-balloon-pos] {\n  overflow: visible;\n}\n\n[aria-label][data-balloon-pos] {\n  cursor: pointer;\n  position: relative;\n}\n\n[aria-label][data-balloon-pos]:after {\n  opacity: 0;\n  pointer-events: none;\n  text-indent: 0;\n  text-shadow: none;\n  font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Oxygen, Ubuntu, Cantarell, Open Sans, Helvetica Neue, sans-serif;\n  font-style: normal;\n  font-weight: normal;\n  font-size: var(--balloon-font-size);\n  background: var(--balloon-color);\n  color: var(--balloon-text-color);\n  border-radius: 2px;\n  border-radius: var(--balloon-border-radius);\n  content: attr(aria-label);\n  white-space: nowrap;\n  z-index: 10;\n  padding: .5em 1em;\n  transition: all .18s ease-out .18s;\n  position: absolute;\n}\n\n[aria-label][data-balloon-pos]:before {\n  border: 5px solid #0000;\n  border-top-color: var(--balloon-color);\n  opacity: 0;\n  pointer-events: none;\n  content: \"\";\n  z-index: 10;\n  width: 0;\n  height: 0;\n  transition: all .18s ease-out .18s;\n  position: absolute;\n}\n\n[aria-label][data-balloon-pos]:hover:before, [aria-label][data-balloon-pos]:hover:after, [aria-label][data-balloon-pos][data-balloon-visible]:before, [aria-label][data-balloon-pos][data-balloon-visible]:after, [aria-label][data-balloon-pos]:not([data-balloon-nofocus]):focus:before, [aria-label][data-balloon-pos]:not([data-balloon-nofocus]):focus:after {\n  opacity: 1;\n  pointer-events: none;\n}\n\n[aria-label][data-balloon-pos].font-awesome:after {\n  font-family: FontAwesome, -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Oxygen, Ubuntu, Cantarell, Open Sans, Helvetica Neue, sans-serif;\n}\n\n[aria-label][data-balloon-pos][data-balloon-break]:after {\n  white-space: pre;\n}\n\n[aria-label][data-balloon-pos][data-balloon-break][data-balloon-length]:after {\n  white-space: pre-line;\n  word-break: break-word;\n}\n\n[aria-label][data-balloon-pos][data-balloon-blunt]:before, [aria-label][data-balloon-pos][data-balloon-blunt]:after {\n  transition: none;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos=\"up\"]:hover:after, [aria-label][data-balloon-pos][data-balloon-pos=\"up\"][data-balloon-visible]:after, [aria-label][data-balloon-pos][data-balloon-pos=\"down\"]:hover:after, [aria-label][data-balloon-pos][data-balloon-pos=\"down\"][data-balloon-visible]:after, [aria-label][data-balloon-pos][data-balloon-pos=\"up\"]:hover:before, [aria-label][data-balloon-pos][data-balloon-pos=\"up\"][data-balloon-visible]:before, [aria-label][data-balloon-pos][data-balloon-pos=\"down\"]:hover:before, [aria-label][data-balloon-pos][data-balloon-pos=\"down\"][data-balloon-visible]:before {\n  transform: translate(-50%);\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos*=\"-left\"]:after {\n  left: 0;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos*=\"-left\"]:before {\n  left: 5px;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos*=\"-right\"]:after {\n  right: 0;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos*=\"-right\"]:before {\n  right: 5px;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos*=\"-left\"]:hover:after, [aria-label][data-balloon-pos][data-balloon-pos*=\"-left\"][data-balloon-visible]:after, [aria-label][data-balloon-pos][data-balloon-pos*=\"-right\"]:hover:after, [aria-label][data-balloon-pos][data-balloon-pos*=\"-right\"][data-balloon-visible]:after, [aria-label][data-balloon-pos][data-balloon-pos*=\"-left\"]:hover:before, [aria-label][data-balloon-pos][data-balloon-pos*=\"-left\"][data-balloon-visible]:before, [aria-label][data-balloon-pos][data-balloon-pos*=\"-right\"]:hover:before, [aria-label][data-balloon-pos][data-balloon-pos*=\"-right\"][data-balloon-visible]:before {\n  transform: translate(0);\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos^=\"up\"]:before, [aria-label][data-balloon-pos][data-balloon-pos^=\"up\"]:after {\n  transform-origin: top;\n  transform: translate(0, var(--balloon-move));\n  bottom: 100%;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos^=\"up\"]:after {\n  margin-bottom: 10px;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos=\"up\"]:before, [aria-label][data-balloon-pos][data-balloon-pos=\"up\"]:after {\n  transform: translate(-50%, var(--balloon-move));\n  left: 50%;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos^=\"down\"]:before, [aria-label][data-balloon-pos][data-balloon-pos^=\"down\"]:after {\n  transform: translate(0, calc(var(--balloon-move) * -1));\n  top: 100%;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos^=\"down\"]:after {\n  margin-top: 10px;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos^=\"down\"]:before {\n  border: 5px solid #0000;\n  border-bottom-color: var(--balloon-color);\n  width: 0;\n  height: 0;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos=\"down\"]:after, [aria-label][data-balloon-pos][data-balloon-pos=\"down\"]:before {\n  transform: translate(-50%, calc(var(--balloon-move) * -1));\n  left: 50%;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos=\"left\"]:hover:after, [aria-label][data-balloon-pos][data-balloon-pos=\"left\"][data-balloon-visible]:after, [aria-label][data-balloon-pos][data-balloon-pos=\"right\"]:hover:after, [aria-label][data-balloon-pos][data-balloon-pos=\"right\"][data-balloon-visible]:after, [aria-label][data-balloon-pos][data-balloon-pos=\"left\"]:hover:before, [aria-label][data-balloon-pos][data-balloon-pos=\"left\"][data-balloon-visible]:before, [aria-label][data-balloon-pos][data-balloon-pos=\"right\"]:hover:before, [aria-label][data-balloon-pos][data-balloon-pos=\"right\"][data-balloon-visible]:before {\n  transform: translate(0, -50%);\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos=\"left\"]:after, [aria-label][data-balloon-pos][data-balloon-pos=\"left\"]:before {\n  transform: translate(var(--balloon-move), -50%);\n  top: 50%;\n  right: 100%;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos=\"left\"]:after {\n  margin-right: 10px;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos=\"left\"]:before {\n  border: 5px solid #0000;\n  border-left-color: var(--balloon-color);\n  width: 0;\n  height: 0;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos=\"right\"]:after, [aria-label][data-balloon-pos][data-balloon-pos=\"right\"]:before {\n  transform: translate(calc(var(--balloon-move) * -1), -50%);\n  top: 50%;\n  left: 100%;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos=\"right\"]:after {\n  margin-left: 10px;\n}\n\n[aria-label][data-balloon-pos][data-balloon-pos=\"right\"]:before {\n  border: 5px solid #0000;\n  border-right-color: var(--balloon-color);\n  width: 0;\n  height: 0;\n}\n\n[aria-label][data-balloon-pos][data-balloon-length]:after {\n  white-space: normal;\n}\n\n[aria-label][data-balloon-pos][data-balloon-length=\"small\"]:after {\n  width: 80px;\n}\n\n[aria-label][data-balloon-pos][data-balloon-length=\"medium\"]:after {\n  width: 150px;\n}\n\n[aria-label][data-balloon-pos][data-balloon-length=\"large\"]:after {\n  width: 260px;\n}\n\n[aria-label][data-balloon-pos][data-balloon-length=\"xlarge\"]:after {\n  width: 380px;\n}\n\n@media screen and (width <= 768px) {\n  [aria-label][data-balloon-pos][data-balloon-length=\"xlarge\"]:after {\n    width: 90vw;\n  }\n}\n\n[aria-label][data-balloon-pos][data-balloon-length=\"fit\"]:after {\n  width: 100%;\n}\n\n:root {\n  --color-primary: #489fd9;\n  --color-primary-light: #abd9f7;\n  --color-primary-400: #3d7da9;\n  --color-primary-300: #315d7c;\n  --color-primary-200: #253e52;\n  --color-primary-100: #151d24;\n  --color-accent: #e37dd7;\n  --color-accent-light: #f794d5;\n  --color-accent-400: #b163a8;\n  --color-accent-300: #824b7b;\n  --color-accent-200: #563351;\n  --color-accent-100: #2d1d2a;\n  --color-body: #dfedf7;\n  --color-muted: #a3c1d4;\n  --color-background: var(--color-primary-100);\n  --anchor-color: #e3ddf0;\n  --anchor-color-hover: var(--color-accent-light);\n  --border-color: var(--color-primary-300);\n  --border-color-accent: var(--color-accent);\n  --balloon-color: var(--color-primary-400);\n  --color-success: #59c27c;\n  --color-warning: #f0ee78;\n  --color-danger: #cf4d4a;\n  --font-size-sm: .875rem;\n  --font-size-regular: 1rem;\n  --font-size-lg: 1.25rem;\n  --font-size-xlg: 2rem;\n  --font-size-xxlg: 3rem;\n}\n\n.d-none {\n  display: none !important;\n}\n\n.d-inline {\n  display: inline !important;\n}\n\n.d-inline-block {\n  display: inline-block !important;\n}\n\n.d-block {\n  display: block !important;\n}\n\n.d-table {\n  display: table !important;\n}\n\n.d-table-row {\n  display: table-row !important;\n}\n\n.d-table-cell {\n  display: table-cell !important;\n}\n\n.d-flex {\n  display: flex !important;\n}\n\n.d-inline-flex {\n  display: inline-flex !important;\n}\n\n@media (width >= 768px) {\n  .d-md-none {\n    display: none !important;\n  }\n\n  .d-md-inline {\n    display: inline !important;\n  }\n\n  .d-md-inline-block {\n    display: inline-block !important;\n  }\n\n  .d-md-block {\n    display: block !important;\n  }\n\n  .d-md-table {\n    display: table !important;\n  }\n\n  .d-md-table-row {\n    display: table-row !important;\n  }\n\n  .d-md-table-cell {\n    display: table-cell !important;\n  }\n\n  .d-md-flex {\n    display: flex !important;\n  }\n\n  .d-md-inline-flex {\n    display: inline-flex !important;\n  }\n}\n\n.m-0 {\n  margin: 0 !important;\n}\n\n.mt-0, .my-0 {\n  margin-top: 0 !important;\n}\n\n.mr-0, .mx-0 {\n  margin-right: 0 !important;\n}\n\n.mb-0, .my-0 {\n  margin-bottom: 0 !important;\n}\n\n.ml-0, .mx-0 {\n  margin-left: 0 !important;\n}\n\n.m-1 {\n  margin: .25rem !important;\n}\n\n.mt-1, .my-1 {\n  margin-top: .25rem !important;\n}\n\n.mr-1, .mx-1 {\n  margin-right: .25rem !important;\n}\n\n.mb-1, .my-1 {\n  margin-bottom: .25rem !important;\n}\n\n.ml-1, .mx-1 {\n  margin-left: .25rem !important;\n}\n\n.m-2 {\n  margin: .5rem !important;\n}\n\n.mt-2, .my-2 {\n  margin-top: .5rem !important;\n}\n\n.mr-2, .mx-2 {\n  margin-right: .5rem !important;\n}\n\n.mb-2, .my-2 {\n  margin-bottom: .5rem !important;\n}\n\n.ml-2, .mx-2 {\n  margin-left: .5rem !important;\n}\n\n.m-3 {\n  margin: 1rem !important;\n}\n\n.mt-3, .my-3 {\n  margin-top: 1rem !important;\n}\n\n.mr-3, .mx-3 {\n  margin-right: 1rem !important;\n}\n\n.mb-3, .my-3 {\n  margin-bottom: 1rem !important;\n}\n\n.ml-3, .mx-3 {\n  margin-left: 1rem !important;\n}\n\n.m-4 {\n  margin: 1.5rem !important;\n}\n\n.mt-4, .my-4 {\n  margin-top: 1.5rem !important;\n}\n\n.mr-4, .mx-4 {\n  margin-right: 1.5rem !important;\n}\n\n.mb-4, .my-4 {\n  margin-bottom: 1.5rem !important;\n}\n\n.ml-4, .mx-4 {\n  margin-left: 1.5rem !important;\n}\n\n.m-5 {\n  margin: 2.5rem !important;\n}\n\n.mt-5, .my-5 {\n  margin-top: 2.5rem !important;\n}\n\n.mr-5, .mx-5 {\n  margin-right: 2.5rem !important;\n}\n\n.mb-5, .my-5 {\n  margin-bottom: 2.5rem !important;\n}\n\n.ml-5, .mx-5 {\n  margin-left: 2.5rem !important;\n}\n\n.p-0 {\n  padding: 0 !important;\n}\n\n.pt-0, .py-0 {\n  padding-top: 0 !important;\n}\n\n.pr-0, .px-0 {\n  padding-right: 0 !important;\n}\n\n.pb-0, .py-0 {\n  padding-bottom: 0 !important;\n}\n\n.pl-0, .px-0 {\n  padding-left: 0 !important;\n}\n\n.p-1 {\n  padding: .25rem !important;\n}\n\n.pt-1, .py-1 {\n  padding-top: .25rem !important;\n}\n\n.pr-1, .px-1 {\n  padding-right: .25rem !important;\n}\n\n.pb-1, .py-1 {\n  padding-bottom: .25rem !important;\n}\n\n.pl-1, .px-1 {\n  padding-left: .25rem !important;\n}\n\n.p-2 {\n  padding: .5rem !important;\n}\n\n.pt-2, .py-2 {\n  padding-top: .5rem !important;\n}\n\n.pr-2, .px-2 {\n  padding-right: .5rem !important;\n}\n\n.pb-2, .py-2 {\n  padding-bottom: .5rem !important;\n}\n\n.pl-2, .px-2 {\n  padding-left: .5rem !important;\n}\n\n.p-3 {\n  padding: 1rem !important;\n}\n\n.pt-3, .py-3 {\n  padding-top: 1rem !important;\n}\n\n.pr-3, .px-3 {\n  padding-right: 1rem !important;\n}\n\n.pb-3, .py-3 {\n  padding-bottom: 1rem !important;\n}\n\n.pl-3, .px-3 {\n  padding-left: 1rem !important;\n}\n\n.p-4 {\n  padding: 1.5rem !important;\n}\n\n.pt-4, .py-4 {\n  padding-top: 1.5rem !important;\n}\n\n.pr-4, .px-4 {\n  padding-right: 1.5rem !important;\n}\n\n.pb-4, .py-4 {\n  padding-bottom: 1.5rem !important;\n}\n\n.pl-4, .px-4 {\n  padding-left: 1.5rem !important;\n}\n\n.p-5 {\n  padding: 2.5rem !important;\n}\n\n.pt-5, .py-5 {\n  padding-top: 2.5rem !important;\n}\n\n.pr-5, .px-5 {\n  padding-right: 2.5rem !important;\n}\n\n.pb-5, .py-5 {\n  padding-bottom: 2.5rem !important;\n}\n\n.pl-5, .px-5 {\n  padding-left: 2.5rem !important;\n}\n\n.m-n1 {\n  margin: -.25rem !important;\n}\n\n.mt-n1, .my-n1 {\n  margin-top: -.25rem !important;\n}\n\n.mr-n1, .mx-n1 {\n  margin-right: -.25rem !important;\n}\n\n.mb-n1, .my-n1 {\n  margin-bottom: -.25rem !important;\n}\n\n.ml-n1, .mx-n1 {\n  margin-left: -.25rem !important;\n}\n\n.m-n2 {\n  margin: -.5rem !important;\n}\n\n.mt-n2, .my-n2 {\n  margin-top: -.5rem !important;\n}\n\n.mr-n2, .mx-n2 {\n  margin-right: -.5rem !important;\n}\n\n.mb-n2, .my-n2 {\n  margin-bottom: -.5rem !important;\n}\n\n.ml-n2, .mx-n2 {\n  margin-left: -.5rem !important;\n}\n\n.m-n3 {\n  margin: -1rem !important;\n}\n\n.mt-n3, .my-n3 {\n  margin-top: -1rem !important;\n}\n\n.mr-n3, .mx-n3 {\n  margin-right: -1rem !important;\n}\n\n.mb-n3, .my-n3 {\n  margin-bottom: -1rem !important;\n}\n\n.ml-n3, .mx-n3 {\n  margin-left: -1rem !important;\n}\n\n.m-n4 {\n  margin: -1.5rem !important;\n}\n\n.mt-n4, .my-n4 {\n  margin-top: -1.5rem !important;\n}\n\n.mr-n4, .mx-n4 {\n  margin-right: -1.5rem !important;\n}\n\n.mb-n4, .my-n4 {\n  margin-bottom: -1.5rem !important;\n}\n\n.ml-n4, .mx-n4 {\n  margin-left: -1.5rem !important;\n}\n\n.m-n5 {\n  margin: -2.5rem !important;\n}\n\n.mt-n5, .my-n5 {\n  margin-top: -2.5rem !important;\n}\n\n.mr-n5, .mx-n5 {\n  margin-right: -2.5rem !important;\n}\n\n.mb-n5, .my-n5 {\n  margin-bottom: -2.5rem !important;\n}\n\n.ml-n5, .mx-n5 {\n  margin-left: -2.5rem !important;\n}\n\n.m-auto {\n  margin: auto !important;\n}\n\n.mt-auto, .my-auto {\n  margin-top: auto !important;\n}\n\n.mr-auto, .mx-auto {\n  margin-right: auto !important;\n}\n\n.mb-auto, .my-auto {\n  margin-bottom: auto !important;\n}\n\n.ml-auto, .mx-auto {\n  margin-left: auto !important;\n}\n\n@media (width >= 768px) {\n  .m-md-0 {\n    margin: 0 !important;\n  }\n\n  .mt-md-0, .my-md-0 {\n    margin-top: 0 !important;\n  }\n\n  .mr-md-0, .mx-md-0 {\n    margin-right: 0 !important;\n  }\n\n  .mb-md-0, .my-md-0 {\n    margin-bottom: 0 !important;\n  }\n\n  .ml-md-0, .mx-md-0 {\n    margin-left: 0 !important;\n  }\n\n  .m-md-1 {\n    margin: .25rem !important;\n  }\n\n  .mt-md-1, .my-md-1 {\n    margin-top: .25rem !important;\n  }\n\n  .mr-md-1, .mx-md-1 {\n    margin-right: .25rem !important;\n  }\n\n  .mb-md-1, .my-md-1 {\n    margin-bottom: .25rem !important;\n  }\n\n  .ml-md-1, .mx-md-1 {\n    margin-left: .25rem !important;\n  }\n\n  .m-md-2 {\n    margin: .5rem !important;\n  }\n\n  .mt-md-2, .my-md-2 {\n    margin-top: .5rem !important;\n  }\n\n  .mr-md-2, .mx-md-2 {\n    margin-right: .5rem !important;\n  }\n\n  .mb-md-2, .my-md-2 {\n    margin-bottom: .5rem !important;\n  }\n\n  .ml-md-2, .mx-md-2 {\n    margin-left: .5rem !important;\n  }\n\n  .m-md-3 {\n    margin: 1rem !important;\n  }\n\n  .mt-md-3, .my-md-3 {\n    margin-top: 1rem !important;\n  }\n\n  .mr-md-3, .mx-md-3 {\n    margin-right: 1rem !important;\n  }\n\n  .mb-md-3, .my-md-3 {\n    margin-bottom: 1rem !important;\n  }\n\n  .ml-md-3, .mx-md-3 {\n    margin-left: 1rem !important;\n  }\n\n  .m-md-4 {\n    margin: 1.5rem !important;\n  }\n\n  .mt-md-4, .my-md-4 {\n    margin-top: 1.5rem !important;\n  }\n\n  .mr-md-4, .mx-md-4 {\n    margin-right: 1.5rem !important;\n  }\n\n  .mb-md-4, .my-md-4 {\n    margin-bottom: 1.5rem !important;\n  }\n\n  .ml-md-4, .mx-md-4 {\n    margin-left: 1.5rem !important;\n  }\n\n  .m-md-5 {\n    margin: 2.5rem !important;\n  }\n\n  .mt-md-5, .my-md-5 {\n    margin-top: 2.5rem !important;\n  }\n\n  .mr-md-5, .mx-md-5 {\n    margin-right: 2.5rem !important;\n  }\n\n  .mb-md-5, .my-md-5 {\n    margin-bottom: 2.5rem !important;\n  }\n\n  .ml-md-5, .mx-md-5 {\n    margin-left: 2.5rem !important;\n  }\n\n  .p-md-0 {\n    padding: 0 !important;\n  }\n\n  .pt-md-0, .py-md-0 {\n    padding-top: 0 !important;\n  }\n\n  .pr-md-0, .px-md-0 {\n    padding-right: 0 !important;\n  }\n\n  .pb-md-0, .py-md-0 {\n    padding-bottom: 0 !important;\n  }\n\n  .pl-md-0, .px-md-0 {\n    padding-left: 0 !important;\n  }\n\n  .p-md-1 {\n    padding: .25rem !important;\n  }\n\n  .pt-md-1, .py-md-1 {\n    padding-top: .25rem !important;\n  }\n\n  .pr-md-1, .px-md-1 {\n    padding-right: .25rem !important;\n  }\n\n  .pb-md-1, .py-md-1 {\n    padding-bottom: .25rem !important;\n  }\n\n  .pl-md-1, .px-md-1 {\n    padding-left: .25rem !important;\n  }\n\n  .p-md-2 {\n    padding: .5rem !important;\n  }\n\n  .pt-md-2, .py-md-2 {\n    padding-top: .5rem !important;\n  }\n\n  .pr-md-2, .px-md-2 {\n    padding-right: .5rem !important;\n  }\n\n  .pb-md-2, .py-md-2 {\n    padding-bottom: .5rem !important;\n  }\n\n  .pl-md-2, .px-md-2 {\n    padding-left: .5rem !important;\n  }\n\n  .p-md-3 {\n    padding: 1rem !important;\n  }\n\n  .pt-md-3, .py-md-3 {\n    padding-top: 1rem !important;\n  }\n\n  .pr-md-3, .px-md-3 {\n    padding-right: 1rem !important;\n  }\n\n  .pb-md-3, .py-md-3 {\n    padding-bottom: 1rem !important;\n  }\n\n  .pl-md-3, .px-md-3 {\n    padding-left: 1rem !important;\n  }\n\n  .p-md-4 {\n    padding: 1.5rem !important;\n  }\n\n  .pt-md-4, .py-md-4 {\n    padding-top: 1.5rem !important;\n  }\n\n  .pr-md-4, .px-md-4 {\n    padding-right: 1.5rem !important;\n  }\n\n  .pb-md-4, .py-md-4 {\n    padding-bottom: 1.5rem !important;\n  }\n\n  .pl-md-4, .px-md-4 {\n    padding-left: 1.5rem !important;\n  }\n\n  .p-md-5 {\n    padding: 2.5rem !important;\n  }\n\n  .pt-md-5, .py-md-5 {\n    padding-top: 2.5rem !important;\n  }\n\n  .pr-md-5, .px-md-5 {\n    padding-right: 2.5rem !important;\n  }\n\n  .pb-md-5, .py-md-5 {\n    padding-bottom: 2.5rem !important;\n  }\n\n  .pl-md-5, .px-md-5 {\n    padding-left: 2.5rem !important;\n  }\n\n  .m-md-n1 {\n    margin: -.25rem !important;\n  }\n\n  .mt-md-n1, .my-md-n1 {\n    margin-top: -.25rem !important;\n  }\n\n  .mr-md-n1, .mx-md-n1 {\n    margin-right: -.25rem !important;\n  }\n\n  .mb-md-n1, .my-md-n1 {\n    margin-bottom: -.25rem !important;\n  }\n\n  .ml-md-n1, .mx-md-n1 {\n    margin-left: -.25rem !important;\n  }\n\n  .m-md-n2 {\n    margin: -.5rem !important;\n  }\n\n  .mt-md-n2, .my-md-n2 {\n    margin-top: -.5rem !important;\n  }\n\n  .mr-md-n2, .mx-md-n2 {\n    margin-right: -.5rem !important;\n  }\n\n  .mb-md-n2, .my-md-n2 {\n    margin-bottom: -.5rem !important;\n  }\n\n  .ml-md-n2, .mx-md-n2 {\n    margin-left: -.5rem !important;\n  }\n\n  .m-md-n3 {\n    margin: -1rem !important;\n  }\n\n  .mt-md-n3, .my-md-n3 {\n    margin-top: -1rem !important;\n  }\n\n  .mr-md-n3, .mx-md-n3 {\n    margin-right: -1rem !important;\n  }\n\n  .mb-md-n3, .my-md-n3 {\n    margin-bottom: -1rem !important;\n  }\n\n  .ml-md-n3, .mx-md-n3 {\n    margin-left: -1rem !important;\n  }\n\n  .m-md-n4 {\n    margin: -1.5rem !important;\n  }\n\n  .mt-md-n4, .my-md-n4 {\n    margin-top: -1.5rem !important;\n  }\n\n  .mr-md-n4, .mx-md-n4 {\n    margin-right: -1.5rem !important;\n  }\n\n  .mb-md-n4, .my-md-n4 {\n    margin-bottom: -1.5rem !important;\n  }\n\n  .ml-md-n4, .mx-md-n4 {\n    margin-left: -1.5rem !important;\n  }\n\n  .m-md-n5 {\n    margin: -2.5rem !important;\n  }\n\n  .mt-md-n5, .my-md-n5 {\n    margin-top: -2.5rem !important;\n  }\n\n  .mr-md-n5, .mx-md-n5 {\n    margin-right: -2.5rem !important;\n  }\n\n  .mb-md-n5, .my-md-n5 {\n    margin-bottom: -2.5rem !important;\n  }\n\n  .ml-md-n5, .mx-md-n5 {\n    margin-left: -2.5rem !important;\n  }\n\n  .m-md-auto {\n    margin: auto !important;\n  }\n\n  .mt-md-auto, .my-md-auto {\n    margin-top: auto !important;\n  }\n\n  .mr-md-auto, .mx-md-auto {\n    margin-right: auto !important;\n  }\n\n  .mb-md-auto, .my-md-auto {\n    margin-bottom: auto !important;\n  }\n\n  .ml-md-auto, .mx-md-auto {\n    margin-left: auto !important;\n  }\n}\n\n.flex-row {\n  flex-direction: row !important;\n}\n\n.flex-column {\n  flex-direction: column !important;\n}\n\n.flex-row-reverse {\n  flex-direction: row-reverse !important;\n}\n\n.flex-column-reverse {\n  flex-direction: column-reverse !important;\n}\n\n.flex-wrap {\n  flex-wrap: wrap !important;\n}\n\n.flex-nowrap {\n  flex-wrap: nowrap !important;\n}\n\n.flex-wrap-reverse {\n  flex-wrap: wrap-reverse !important;\n}\n\n.flex-fill {\n  flex: auto !important;\n}\n\n.flex-grow-0 {\n  flex-grow: 0 !important;\n}\n\n.flex-grow-1 {\n  flex-grow: 1 !important;\n}\n\n.flex-shrink-0 {\n  flex-shrink: 0 !important;\n}\n\n.flex-shrink-1 {\n  flex-shrink: 1 !important;\n}\n\n.justify-content-start {\n  justify-content: flex-start !important;\n}\n\n.justify-content-end {\n  justify-content: flex-end !important;\n}\n\n.justify-content-center {\n  justify-content: center !important;\n}\n\n.justify-content-between {\n  justify-content: space-between !important;\n}\n\n.justify-content-around {\n  justify-content: space-around !important;\n}\n\n.align-items-start {\n  align-items: flex-start !important;\n}\n\n.align-items-end {\n  align-items: flex-end !important;\n}\n\n.align-items-center {\n  align-items: center !important;\n}\n\n.align-items-baseline {\n  align-items: baseline !important;\n}\n\n.align-items-stretch {\n  align-items: stretch !important;\n}\n\n.align-content-start {\n  align-content: flex-start !important;\n}\n\n.align-content-end {\n  align-content: flex-end !important;\n}\n\n.align-content-center {\n  align-content: center !important;\n}\n\n.align-content-between {\n  align-content: space-between !important;\n}\n\n.align-content-around {\n  align-content: space-around !important;\n}\n\n.align-content-stretch {\n  align-content: stretch !important;\n}\n\n.align-self-auto {\n  align-self: auto !important;\n}\n\n.align-self-start {\n  align-self: flex-start !important;\n}\n\n.align-self-end {\n  align-self: flex-end !important;\n}\n\n.align-self-center {\n  align-self: center !important;\n}\n\n.align-self-baseline {\n  align-self: baseline !important;\n}\n\n.align-self-stretch {\n  align-self: stretch !important;\n}\n\n@media (width >= 768px) {\n  .flex-md-row {\n    flex-direction: row !important;\n  }\n\n  .flex-md-column {\n    flex-direction: column !important;\n  }\n\n  .flex-md-row-reverse {\n    flex-direction: row-reverse !important;\n  }\n\n  .flex-md-column-reverse {\n    flex-direction: column-reverse !important;\n  }\n\n  .flex-md-wrap {\n    flex-wrap: wrap !important;\n  }\n\n  .flex-md-nowrap {\n    flex-wrap: nowrap !important;\n  }\n\n  .flex-md-wrap-reverse {\n    flex-wrap: wrap-reverse !important;\n  }\n\n  .flex-md-fill {\n    flex: auto !important;\n  }\n\n  .flex-md-grow-0 {\n    flex-grow: 0 !important;\n  }\n\n  .flex-md-grow-1 {\n    flex-grow: 1 !important;\n  }\n\n  .flex-md-shrink-0 {\n    flex-shrink: 0 !important;\n  }\n\n  .flex-md-shrink-1 {\n    flex-shrink: 1 !important;\n  }\n\n  .justify-content-md-start {\n    justify-content: flex-start !important;\n  }\n\n  .justify-content-md-end {\n    justify-content: flex-end !important;\n  }\n\n  .justify-content-md-center {\n    justify-content: center !important;\n  }\n\n  .justify-content-md-between {\n    justify-content: space-between !important;\n  }\n\n  .justify-content-md-around {\n    justify-content: space-around !important;\n  }\n\n  .align-items-md-start {\n    align-items: flex-start !important;\n  }\n\n  .align-items-md-end {\n    align-items: flex-end !important;\n  }\n\n  .align-items-md-center {\n    align-items: center !important;\n  }\n\n  .align-items-md-baseline {\n    align-items: baseline !important;\n  }\n\n  .align-items-md-stretch {\n    align-items: stretch !important;\n  }\n\n  .align-content-md-start {\n    align-content: flex-start !important;\n  }\n\n  .align-content-md-end {\n    align-content: flex-end !important;\n  }\n\n  .align-content-md-center {\n    align-content: center !important;\n  }\n\n  .align-content-md-between {\n    align-content: space-between !important;\n  }\n\n  .align-content-md-around {\n    align-content: space-around !important;\n  }\n\n  .align-content-md-stretch {\n    align-content: stretch !important;\n  }\n\n  .align-self-md-auto {\n    align-self: auto !important;\n  }\n\n  .align-self-md-start {\n    align-self: flex-start !important;\n  }\n\n  .align-self-md-end {\n    align-self: flex-end !important;\n  }\n\n  .align-self-md-center {\n    align-self: center !important;\n  }\n\n  .align-self-md-baseline {\n    align-self: baseline !important;\n  }\n\n  .align-self-md-stretch {\n    align-self: stretch !important;\n  }\n}\n\nsmall, .text-sm {\n  font-size: var(--font-size-sm) !important;\n}\n\n.text-regular {\n  font-size: var(--font-size-regular) !important;\n}\n\n.text-lg {\n  font-size: var(--font-size-lg) !important;\n}\n\n.text-xlg {\n  font-size: var(--font-size-xlg) !important;\n}\n\n.text-right {\n  text-align: right;\n}\n\n.text-left {\n  text-align: left;\n}\n\n.text-center {\n  text-align: center;\n}\n\n.text-muted {\n  color: var(--color-muted) !important;\n}\n\n.text-uppercase {\n  text-transform: uppercase;\n}\n\n.font-weight-normal {\n  font-weight: normal;\n}\n\n.font-weight-bold {\n  font-weight: bold;\n}\n\n.font-weight-semibold {\n  font-weight: 600;\n}\n\n.font-weight-black {\n  font-weight: 900;\n}\n\n.font-style-italic {\n  font-style: italic;\n}\n\n.font-small-caps {\n  font-variant: all-small-caps;\n}\n\n.line-height-1 {\n  line-height: 1;\n}\n\n.text-decoration-none {\n  text-decoration: none;\n}\n\n.text-break-all {\n  word-break: break-all;\n}\n\n.text-nowrap {\n  white-space: nowrap;\n}\n\n.position-relative {\n  position: relative;\n}\n\n.img-fluid {\n  max-width: 100%;\n  height: auto;\n}\n\n.zero {\n  margin: 0;\n  padding: 0;\n}\n\n.invisible {\n  visibility: hidden;\n}\n\n.h-100 {\n  height: 100%;\n}\n\n.w-100 {\n  width: 100%;\n}\n\n.d-grid {\n  grid-auto-columns: 1fr;\n  grid-auto-flow: column;\n  display: grid;\n}\n\n.rounded {\n  border-radius: .5rem;\n}\n\n.border {\n  border: 1px solid var(--border-color);\n}\n\n.border-accent {\n  border: 1px solid var(--border-color-accent);\n}\n\n.border-top {\n  border-top: 1px solid var(--color-primary-300);\n}\n\n.border-bottom {\n  border-bottom: 1px solid var(--color-primary-300);\n}\n\n.border-right {\n  border-right: 1px solid var(--color-primary-300);\n}\n\n.border-left {\n  border-left: 1px solid var(--color-primary-300);\n}\n\n.carousel {\n  margin: 0 -3rem;\n  position: relative;\n}\n\n.carousel__items {\n  scroll-behavior: smooth;\n  -webkit-overflow-scrolling: touch;\n  scroll-snap-type: x mandatory;\n  scroll-snap-align: start;\n  scrollbar-width: none;\n  -ms-overflow-style: none;\n  gap: 2rem;\n  width: 100%;\n  display: flex;\n  overflow-x: scroll;\n}\n\n.carousel-item {\n  flex-shrink: 0;\n  max-width: 300px;\n}\n\n.carousel-item:first-child {\n  padding-left: 3rem;\n}\n\n.carousel-item:last-child {\n  padding-right: 3rem;\n}\n\n.carousel__items::-webkit-scrollbar {\n  display: none;\n}\n\n.carousel__next, .carousel__prev {\n  z-index: 1;\n  position: absolute;\n  top: calc(50% - 12px);\n  left: 0;\n}\n\n.carousel__next {\n  left: unset;\n  right: 0;\n}\n\n.btn {\n  text-transform: uppercase;\n  font-size: var(--font-size-sm);\n  letter-spacing: .05rem;\n  cursor: pointer;\n  background: var(--color-background);\n  border: 2px solid var(--color-primary-400);\n  color: var(--color-primary-light);\n  border-radius: .5rem;\n  padding: .75rem;\n  font-weight: bold;\n  transition: border-color .1s ease-in;\n}\n\n.btn-small {\n  text-transform: uppercase;\n  font-size: var(--font-size-sm);\n  cursor: pointer;\n  background: var(--color-background);\n  border: 2px solid var(--color-primary-400);\n  color: var(--color-primary-light);\n  border-radius: .5rem;\n  padding: .5rem;\n  font-weight: bold;\n}\n\n.btn-small:hover, .btn:hover {\n  border-color: var(--anchor-color-hover);\n  color: var(--anchor-color-hover);\n}\n\n.btn img, .btn-small img {\n  filter: invert(77%) sepia(40%) saturate(250%) hue-rotate(164deg) brightness() contrast(94%);\n}\n\n.btn:hover img, .btn-small:hover img {\n  filter: invert(85%) sepia(46%) saturate(3508%) hue-rotate(287deg) brightness(112%) contrast(94%);\n}\n\n.btn-text {\n  color: inherit;\n  font-size: inherit;\n  cursor: pointer;\n  background: none;\n  border: 0;\n  margin: 0;\n  padding: 0;\n  transition: color .1s ease-in;\n}\n\n.btn-text:hover {\n  color: var(--anchor-color-hover) !important;\n}\n\n.btn-icon {\n  cursor: pointer;\n  color: inherit;\n  background: none;\n  border: 0;\n  align-items: center;\n  transition: color .1s ease-in;\n  display: inline-flex;\n}\n\nselect {\n  border: 2px solid var(--color-primary-400);\n  color: var(--color-primary-light);\n  font-size: var(--font-size-sm);\n  appearance: none;\n  background: var(--color-background) url(\"data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='100' height='100' fill='%233d8fa9'><polygon points='0,0 100,0 50,50'/></svg>\") no-repeat;\n  background-position: right .75em top 65%;\n  background-repeat: no-repeat;\n  background-size: 12px;\n  border-radius: .5rem;\n  min-width: 20ch;\n  padding: .5rem 2rem .5rem .5rem;\n}\n\nselect:focus-visible {\n  border: 2px solid var(--anchor-color-hover);\n  color: var(--anchor-color-hover);\n  outline: none;\n}\n\nh1, h2, h3, h4, h5, h6, p {\n  margin: 0;\n}\n\nbody {\n  color: var(--color-body);\n  background-color: var(--color-background);\n  font: 1rem / 1.5 system-ui, sans-serif;\n  display: flex;\n}\n\nh1, h2, h3, h4, h5, h6 {\n  line-height: 1.1;\n}\n\na {\n  color: inherit;\n  transition: color .1s ease-in;\n}\n\na:hover {\n  color: var(--anchor-color-hover);\n}\n\na:visited {\n  -webkit-text-decoration: none;\n  text-decoration: none;\n}\n\n:target {\n  color: var(--anchor-color-hover);\n}\n\ncode {\n  font-family: ui-monospace, Menlo, Monaco, Courier New, monospace;\n}\n\nhr {\n  border-top: 1px solid var(--border-color);\n  border-bottom: 0;\n}\n\ndt {\n  font-size: var(--font-size-sm);\n  text-transform: uppercase;\n  color: var(--color-muted);\n  font-weight: 600;\n}\n\ndd {\n  font-size: var(--font-size-sm);\n  margin: 0 0 1rem;\n}\n\n.badge {\n  color: var(--color-muted);\n  background-color: var(--color-primary-300);\n  border-radius: .5rem;\n  padding: .1875rem .375rem;\n  text-decoration: none;\n}\n\n.badge--outline {\n  border: 2px solid var(--color-primary-300);\n  color: var(--color-muted);\n  border-radius: .5rem;\n  padding: .1875rem .375rem;\n  text-decoration: none;\n  transition: border-color .1s ease-in;\n}\n\n.badge--outline:hover {\n  border-color: var(--anchor-color-hover);\n}\n\n.badge--pill {\n  border-radius: 1rem;\n}\n\n.badge-res {\n  background: var(--color-primary-200);\n  color: #fff;\n  text-shadow: 1px 1px #4d5078;\n  border-radius: 4px;\n  padding: 0 3px;\n  font-size: 12px;\n}\n\n.badge-2160 {\n  background: #b82927;\n}\n\n.badge-1080 {\n  background: #e0560b;\n}\n\n.badge-720 {\n  background: var(--color-accent);\n}\n\n.badge-480 {\n  background: #269ddb;\n}\n\n.torrent-medium {\n  color: var(--color-warning);\n}\n\n.torrent-low {\n  color: var(--color-danger);\n}\n\nfieldset {\n  border: 0;\n  margin: 0;\n  padding: 0;\n}\n\nlegend {\n  font-size: var(--font-size-sm);\n  text-transform: uppercase;\n  color: var(--color-muted);\n  font-weight: 600;\n}\n\n.report, .table {\n  border-collapse: collapse;\n}\n\n.table td {\n  padding: .1875rem .5rem .1875rem 0;\n}\n\n.table tr {\n  transition: background-color .1s ease-out;\n}\n\n.table tr:hover {\n  background-color: #253e52;\n}\n\n.report td {\n  padding: .25em 2rem .25rem 0;\n}\n\n.report th, .table th {\n  border-bottom: 1px solid var(--color-primary-200);\n  color: var(--color-muted);\n  text-transform: uppercase;\n  font-weight: 600;\n  font-size: var(--font-size-sm);\n  padding: .375rem .5rem .375rem 0;\n}\n\n@media screen and (width >= 768px) {\n  .card-series {\n    max-width: 10rem;\n  }\n}\n\n.card-series__image {\n  aspect-ratio: 500 / 750;\n  border: 2px solid var(--color-primary-200);\n  box-shadow: var(--color-primary-200) 0 0;\n  background-color: var(--color-accent-200);\n  background-position: 0 0;\n  background-image: linear-gradient(125deg, var(--color-accent-400) 25%, transparent 25%);\n  transition: transform .2s ease-out, filter .3s ease-out, box-shadow .2s ease-out;\n}\n\na:hover .card-series__image {\n  filter: brightness(1.25);\n  box-shadow: var(--color-primary-200) 7px 7px;\n  transform: translate(-7px, -7px);\n}\n\n.search-query {\n  width: min-content;\n  position: relative;\n}\n\n.search-query input {\n  background: var(--color-background);\n  border: 2px solid var(--color-primary-400);\n  color: var(--color-primary-light);\n  font-size: var(--font-size-lg);\n  border-radius: .5rem;\n  padding: .75rem .5rem;\n}\n\n.search-query input::-webkit-calendar-picker-indicator {\n  display: none !important;\n}\n\n@media screen and (width >= 768px) {\n  .search-query input {\n    width: 30rem;\n  }\n}\n\n.search-query input:focus-visible {\n  border: 2px solid var(--anchor-color-hover);\n  outline: none;\n}\n\ninput::placeholder {\n  color: var(--color-primary-300);\n}\n\n.search-query button {\n  z-index: 1;\n  background: var(--color-background);\n  cursor: pointer;\n  font-size: var(--font-size-lg);\n  background: none;\n  border: 0;\n  padding: .75rem;\n  position: absolute;\n  top: 0;\n  right: 0;\n}\n\na:hover .card-episode__poster, a:hover .card-episode__image, .btn-text:hover .card-episode__image {\n  border-color: var(--color-accent);\n  transition: border-color .1s ease-in;\n}\n\n.header .btn-icon:hover {\n  background-color: var(--color-primary-300);\n  transition: background-color .2s ease-out;\n}\n\n.header {\n  background: var(--color-primary-200);\n  flex-direction: column;\n  gap: .5rem;\n  height: 100vh;\n  display: flex;\n  position: sticky;\n  top: 0;\n}\n\n.header .btn-icon {\n  padding: .75rem;\n}\n\n.icon, .header .btn-icon img {\n  filter: invert(88%) sepia(3%) saturate(2496%) hue-rotate(185deg) brightness(106%) contrast(94%);\n}\n\n.header .btn-icon:hover img {\n  filter: invert(78%) sepia(13%) saturate(3097%) hue-rotate(274deg) brightness(96%) contrast(85%);\n}\n\n@media screen and (width >= 768px) {\n  .header {\n    align-items: center;\n  }\n\n  nav {\n    background: none;\n  }\n}\n\nmain {\n  flex-grow: 1;\n  padding: 3rem;\n}\n\n.footer {\n  color: var(--color-muted);\n}\n\naside {\n  flex-shrink: 0;\n  flex-basis: 14rem;\n}\n\n.main-column {\n  flex-grow: 1;\n}\n\n.card-episode {\n  position: relative;\n}\n\n.card-episode__image {\n  aspect-ratio: 300 / 170;\n  border: 2px solid var(--color-primary-300);\n  background-position: 0 0;\n  background-color: var(--color-accent-200);\n  background-image: linear-gradient(125deg, var(--color-accent-400) 25%, transparent 25%);\n  transition: transform .2s ease-out, filter .3s ease-out, box-shadow .2s ease-out;\n}\n\n.card-episode__poster {\n  z-index: 1;\n  border: 2px solid var(--color-primary-300);\n  max-width: 75px;\n  position: absolute;\n  bottom: -1rem;\n  right: 1rem;\n}\n\n.series-poster__image {\n  aspect-ratio: 500 / 750;\n  border: 2px solid var(--color-primary-200);\n  background-position: 0 0;\n  background-color: var(--color-accent-200);\n  background-image: linear-gradient(125deg, var(--color-accent-400) 25%, transparent 25%);\n}\n\n@media screen and (width >= 768px) {\n  .series-poster__image {\n    box-shadow: var(--color-primary-200) 7px 7px;\n  }\n}\n\n.episode-grid {\n  grid-template-rows: auto;\n  grid-template-columns: repeat(4, 1fr);\n  gap: 2rem;\n  display: grid;\n}\n\n.episode-grid__cell {\n  max-width: 300px;\n}\n\n.body-copy, .series-overview {\n  max-width: 75ch;\n}\n\n.fanart {\n  background-blend-mode: multiply;\n  background-position: top;\n  background-repeat: no-repeat;\n  background-size: cover;\n  background-attachment: fixed;\n  background-color: var(--color-accent-100);\n  margin-top: -3rem;\n  margin-left: -3rem;\n  margin-right: -3rem;\n  padding: 3rem;\n}\n\n@media screen and (width >= 768px) {\n  .top-series-grid {\n    grid-template-columns: repeat(2, 1fr);\n    gap: 2rem;\n    display: grid;\n  }\n}\n\n.cards-grid {\n  grid-template-columns: repeat(3, 1fr);\n  gap: 1.5rem;\n  margin-bottom: 2rem;\n  display: grid;\n}\n\n@media screen and (width >= 768px) {\n  .cards-grid {\n    grid-template-columns: repeat(6, 1fr);\n    gap: 2rem;\n  }\n}\n\ndialog {\n  opacity: 0;\n  color: var(--color-body);\n  max-width: unset;\n  max-height: unset;\n  pointer-events: none;\n  background: none;\n  border: 0;\n  width: 100vw;\n  height: 100vh;\n  margin: 0;\n  padding: 0;\n}\n\ndialog.in {\n  pointer-events: auto;\n  opacity: 1;\n  transition: opacity .3s ease-out;\n}\n\ndialog.out {\n  opacity: 0;\n  transition: opacity .3s ease-out 2s;\n}\n\n.dialog-body {\n  background: var(--color-primary-200);\n  border-radius: 1rem;\n  width: 30rem;\n  padding: 2rem;\n}\n\n.dialog-body--small {\n  width: 16rem;\n}\n\ndialog:modal {\n  opacity: 1;\n  pointer-events: auto;\n  justify-content: center;\n  align-items: center;\n  display: flex;\n}\n\ndialog::backdrop {\n  background: #151d27bf;\n}\n\n.anim-spin {\n  animation-name: spin;\n  animation-duration: 4s;\n  animation-timing-function: linear;\n  animation-iteration-count: infinite;\n}\n\n@keyframes spin {\n  from {\n    transform: rotate(0);\n  }\n\n  to {\n    transform: rotate(360deg);\n  }\n}\n\n.sr-only {\n  white-space: nowrap;\n  clip: rect(0 0 0 0);\n  clip-path: inset(50%);\n  border: 0;\n  width: 1px;\n  height: 1px;\n  margin: -1px;\n  padding: 0;\n  position: absolute;\n  overflow: hidden;\n}\n\n.skip-nav a {\n  width: 1px;\n  height: 1px;\n  position: absolute;\n  top: auto;\n  left: -9999px;\n  overflow: hidden;\n}\n\n.skip-nav a:focus {\n  width: auto;\n  height: auto;\n  position: static;\n}\n\n.mobile-carousel {\n  gap: 1.5rem;\n  display: flex;\n}\n\n@media screen and (width <= 767.98px) {\n  .mobile-carousel {\n    scroll-behavior: smooth;\n    -webkit-overflow-scrolling: touch;\n    scroll-snap-type: x mandatory;\n    margin: 0 -1rem 0 0;\n    display: flex;\n    overflow-x: scroll;\n  }\n\n  .mobile-carousel > .mobile-carousel__item {\n    scroll-snap-align: start;\n    flex-shrink: 0;\n    flex-basis: 50vw;\n  }\n\n  .mobile-carousel::-webkit-scrollbar {\n    display: none;\n  }\n}\n\n@media screen and (width >= 768px) {\n  .mobile-carousel {\n    gap: 2rem;\n  }\n}\n\n.radio-button-group {\n  border: 2px solid var(--color-primary-400);\n  color: var(--color-primary-light);\n  font-size: var(--font-size-sm);\n  background-color: var(--color-primary-100);\n  border-radius: .5rem;\n  display: flex;\n}\n\n.radio-button-group__label {\n  color: var(--color-body);\n  cursor: pointer;\n  background-color: #0000;\n  border-radius: .4rem;\n  align-items: center;\n  padding: .5rem;\n  display: inline-flex;\n}\n\n.radio-button-group__label:has(input:checked) {\n  background-color: var(--color-primary-300);\n}\n\n.radio-button-group__input {\n  clip: rect(0, 0, 0, 0);\n  white-space: nowrap;\n  border: 0;\n  width: 1px;\n  height: 1px;\n  padding: 0;\n  position: absolute;\n  overflow: hidden;\n}\n\nprogress {\n  accent-color: var(--color-accent-light);\n}\n\n.chart {\n  max-width: 100%;\n}\n\n/*# sourceMappingURL=app.css.map */\n",
         "/*! normalize.css v8.0.1 | MIT License | github.com/necolas/normalize.css */\n\n/* Document\n   ========================================================================== */\n\n/**\n * 1. Correct the line height in all browsers.\n * 2. Prevent adjustments of font size after orientation changes in iOS.\n */\n\n html {\n    line-height: 1.15; /* 1 */\n    -webkit-text-size-adjust: 100%; /* 2 */\n  }\n  \n  /* Sections\n     ========================================================================== */\n  \n  /**\n   * Remove the margin in all browsers.\n   */\n  \n  body {\n    margin: 0;\n  }\n  \n  /**\n   * Render the `main` element consistently in IE.\n   */\n  \n  main {\n    display: block;\n  }\n  \n  /**\n   * Correct the font size and margin on `h1` elements within `section` and\n   * `article` contexts in Chrome, Firefox, and Safari.\n   */\n  \n  h1 {\n    font-size: 2em;\n    margin: 0.67em 0;\n  }\n  \n  /* Grouping content\n     ========================================================================== */\n  \n  /**\n   * 1. Add the correct box sizing in Firefox.\n   * 2. Show the overflow in Edge and IE.\n   */\n  \n  hr {\n    box-sizing: content-box; /* 1 */\n    height: 0; /* 1 */\n    overflow: visible; /* 2 */\n  }\n  \n  /**\n   * 1. Correct the inheritance and scaling of font size in all browsers.\n   * 2. Correct the odd `em` font sizing in all browsers.\n   */\n  \n  pre {\n    font-family: monospace, monospace; /* 1 */\n    font-size: 1em; /* 2 */\n  }\n  \n  /* Text-level semantics\n     ========================================================================== */\n  \n  /**\n   * Remove the gray background on active links in IE 10.\n   */\n  \n  a {\n    background-color: transparent;\n  }\n  \n  /**\n   * 1. Remove the bottom border in Chrome 57-\n   * 2. Add the correct text decoration in Chrome, Edge, IE, Opera, and Safari.\n   */\n  \n  abbr[title] {\n    border-bottom: none; /* 1 */\n    text-decoration: underline; /* 2 */\n    text-decoration: underline dotted; /* 2 */\n  }\n  \n  /**\n   * Add the correct font weight in Chrome, Edge, and Safari.\n   */\n  \n  b,\n  strong {\n    font-weight: bolder;\n  }\n  \n  /**\n   * 1. Correct the inheritance and scaling of font size in all browsers.\n   * 2. Correct the odd `em` font sizing in all browsers.\n   */\n  \n  code,\n  kbd,\n  samp {\n    font-family: monospace, monospace; /* 1 */\n    font-size: 1em; /* 2 */\n  }\n  \n  /**\n   * Add the correct font size in all browsers.\n   */\n  \n  small {\n    font-size: 80%;\n  }\n  \n  /**\n   * Prevent `sub` and `sup` elements from affecting the line height in\n   * all browsers.\n   */\n  \n  sub,\n  sup {\n    font-size: 75%;\n    line-height: 0;\n    position: relative;\n    vertical-align: baseline;\n  }\n  \n  sub {\n    bottom: -0.25em;\n  }\n  \n  sup {\n    top: -0.5em;\n  }\n  \n  /* Embedded content\n     ========================================================================== */\n  \n  /**\n   * Remove the border on images inside links in IE 10.\n   */\n  \n  img {\n    border-style: none;\n  }\n  \n  /* Forms\n     ========================================================================== */\n  \n  /**\n   * 1. Change the font styles in all browsers.\n   * 2. Remove the margin in Firefox and Safari.\n   */\n  \n  button,\n  input,\n  optgroup,\n  select,\n  textarea {\n    font-family: inherit; /* 1 */\n    font-size: 100%; /* 1 */\n    line-height: 1.15; /* 1 */\n    margin: 0; /* 2 */\n  }\n  \n  /**\n   * Show the overflow in IE.\n   * 1. Show the overflow in Edge.\n   */\n  \n  button,\n  input { /* 1 */\n    overflow: visible;\n  }\n  \n  /**\n   * Remove the inheritance of text transform in Edge, Firefox, and IE.\n   * 1. Remove the inheritance of text transform in Firefox.\n   */\n  \n  button,\n  select { /* 1 */\n    text-transform: none;\n  }\n  \n  /**\n   * Correct the inability to style clickable types in iOS and Safari.\n   */\n  \n  button,\n  [type=\"button\"],\n  [type=\"reset\"],\n  [type=\"submit\"] {\n    -webkit-appearance: button;\n  }\n  \n  /**\n   * Remove the inner border and padding in Firefox.\n   */\n  \n  button::-moz-focus-inner,\n  [type=\"button\"]::-moz-focus-inner,\n  [type=\"reset\"]::-moz-focus-inner,\n  [type=\"submit\"]::-moz-focus-inner {\n    border-style: none;\n    padding: 0;\n  }\n  \n  /**\n   * Restore the focus styles unset by the previous rule.\n   */\n  \n  button:-moz-focusring,\n  [type=\"button\"]:-moz-focusring,\n  [type=\"reset\"]:-moz-focusring,\n  [type=\"submit\"]:-moz-focusring {\n    outline: 1px dotted ButtonText;\n  }\n  \n  /**\n   * Correct the padding in Firefox.\n   */\n  \n  fieldset {\n    padding: 0.35em 0.75em 0.625em;\n  }\n  \n  /**\n   * 1. Correct the text wrapping in Edge and IE.\n   * 2. Correct the color inheritance from `fieldset` elements in IE.\n   * 3. Remove the padding so developers are not caught out when they zero out\n   *    `fieldset` elements in all browsers.\n   */\n  \n  legend {\n    box-sizing: border-box; /* 1 */\n    color: inherit; /* 2 */\n    display: table; /* 1 */\n    max-width: 100%; /* 1 */\n    padding: 0; /* 3 */\n    white-space: normal; /* 1 */\n  }\n  \n  /**\n   * Add the correct vertical alignment in Chrome, Firefox, and Opera.\n   */\n  \n  progress {\n    vertical-align: baseline;\n  }\n  \n  /**\n   * Remove the default vertical scrollbar in IE 10+.\n   */\n  \n  textarea {\n    overflow: auto;\n  }\n  \n  /**\n   * 1. Add the correct box sizing in IE 10.\n   * 2. Remove the padding in IE 10.\n   */\n  \n  [type=\"checkbox\"],\n  [type=\"radio\"] {\n    box-sizing: border-box; /* 1 */\n    padding: 0; /* 2 */\n  }\n  \n  /**\n   * Correct the cursor style of increment and decrement buttons in Chrome.\n   */\n  \n  [type=\"number\"]::-webkit-inner-spin-button,\n  [type=\"number\"]::-webkit-outer-spin-button {\n    height: auto;\n  }\n  \n  /**\n   * 1. Correct the odd appearance in Chrome and Safari.\n   * 2. Correct the outline style in Safari.\n   */\n  \n  [type=\"search\"] {\n    -webkit-appearance: textfield; /* 1 */\n    outline-offset: -2px; /* 2 */\n  }\n  \n  /**\n   * Remove the inner padding in Chrome and Safari on macOS.\n   */\n  \n  [type=\"search\"]::-webkit-search-decoration {\n    -webkit-appearance: none;\n  }\n  \n  /**\n   * 1. Correct the inability to style clickable types in iOS and Safari.\n   * 2. Change font properties to `inherit` in Safari.\n   */\n  \n  ::-webkit-file-upload-button {\n    -webkit-appearance: button; /* 1 */\n    font: inherit; /* 2 */\n  }\n  \n  /* Interactive\n     ========================================================================== */\n  \n  /*\n   * Add the correct display in Edge, IE 10+, and Firefox.\n   */\n  \n  details {\n    display: block;\n  }\n  \n  /*\n   * Add the correct display in all browsers.\n   */\n  \n  summary {\n    display: list-item;\n  }\n  \n  /* Misc\n     ========================================================================== */\n  \n  /**\n   * Add the correct display in IE 10+.\n   */\n  \n  template {\n    display: none;\n  }\n  \n  /**\n   * Add the correct display in IE 10.\n   */\n  \n  [hidden] {\n    display: none;\n  }",
         ":root {\n    --balloon-border-radius: 2px;\n    --balloon-color: rgba(16, 16, 16, 0.95);\n    --balloon-text-color: #fff;\n    --balloon-font-size: 12px;\n    --balloon-move: 4px; }\n  \n  button[aria-label][data-balloon-pos] {\n    overflow: visible; }\n  \n  [aria-label][data-balloon-pos] {\n    position: relative;\n    cursor: pointer; }\n    [aria-label][data-balloon-pos]:after {\n      opacity: 0;\n      pointer-events: none;\n      transition: all 0.18s ease-out 0.18s;\n      text-indent: 0;\n      font-family: -apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, Oxygen, Ubuntu, Cantarell, \"Open Sans\", \"Helvetica Neue\", sans-serif;\n      font-weight: normal;\n      font-style: normal;\n      text-shadow: none;\n      font-size: var(--balloon-font-size);\n      background: var(--balloon-color);\n      border-radius: 2px;\n      color: var(--balloon-text-color);\n      border-radius: var(--balloon-border-radius);\n      content: attr(aria-label);\n      padding: .5em 1em;\n      position: absolute;\n      white-space: nowrap;\n      z-index: 10; }\n    [aria-label][data-balloon-pos]:before {\n      width: 0;\n      height: 0;\n      border: 5px solid transparent;\n      border-top-color: var(--balloon-color);\n      opacity: 0;\n      pointer-events: none;\n      transition: all 0.18s ease-out 0.18s;\n      content: \"\";\n      position: absolute;\n      z-index: 10; }\n    [aria-label][data-balloon-pos]:hover:before, [aria-label][data-balloon-pos]:hover:after, [aria-label][data-balloon-pos][data-balloon-visible]:before, [aria-label][data-balloon-pos][data-balloon-visible]:after, [aria-label][data-balloon-pos]:not([data-balloon-nofocus]):focus:before, [aria-label][data-balloon-pos]:not([data-balloon-nofocus]):focus:after {\n      opacity: 1;\n      pointer-events: none; }\n    [aria-label][data-balloon-pos].font-awesome:after {\n      font-family: FontAwesome, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif; }\n    [aria-label][data-balloon-pos][data-balloon-break]:after {\n      white-space: pre; }\n    [aria-label][data-balloon-pos][data-balloon-break][data-balloon-length]:after {\n      white-space: pre-line;\n      word-break: break-word; }\n    [aria-label][data-balloon-pos][data-balloon-blunt]:before, [aria-label][data-balloon-pos][data-balloon-blunt]:after {\n      transition: none; }\n    [aria-label][data-balloon-pos][data-balloon-pos=\"up\"]:hover:after, [aria-label][data-balloon-pos][data-balloon-pos=\"up\"][data-balloon-visible]:after, [aria-label][data-balloon-pos][data-balloon-pos=\"down\"]:hover:after, [aria-label][data-balloon-pos][data-balloon-pos=\"down\"][data-balloon-visible]:after {\n      transform: translate(-50%, 0); }\n    [aria-label][data-balloon-pos][data-balloon-pos=\"up\"]:hover:before, [aria-label][data-balloon-pos][data-balloon-pos=\"up\"][data-balloon-visible]:before, [aria-label][data-balloon-pos][data-balloon-pos=\"down\"]:hover:before, [aria-label][data-balloon-pos][data-balloon-pos=\"down\"][data-balloon-visible]:before {\n      transform: translate(-50%, 0); }\n    [aria-label][data-balloon-pos][data-balloon-pos*=\"-left\"]:after {\n      left: 0; }\n    [aria-label][data-balloon-pos][data-balloon-pos*=\"-left\"]:before {\n      left: 5px; }\n    [aria-label][data-balloon-pos][data-balloon-pos*=\"-right\"]:after {\n      right: 0; }\n    [aria-label][data-balloon-pos][data-balloon-pos*=\"-right\"]:before {\n      right: 5px; }\n    [aria-label][data-balloon-pos][data-balloon-pos*=\"-left\"]:hover:after, [aria-label][data-balloon-pos][data-balloon-pos*=\"-left\"][data-balloon-visible]:after, [aria-label][data-balloon-pos][data-balloon-pos*=\"-right\"]:hover:after, [aria-label][data-balloon-pos][data-balloon-pos*=\"-right\"][data-balloon-visible]:after {\n      transform: translate(0, 0); }\n    [aria-label][data-balloon-pos][data-balloon-pos*=\"-left\"]:hover:before, [aria-label][data-balloon-pos][data-balloon-pos*=\"-left\"][data-balloon-visible]:before, [aria-label][data-balloon-pos][data-balloon-pos*=\"-right\"]:hover:before, [aria-label][data-balloon-pos][data-balloon-pos*=\"-right\"][data-balloon-visible]:before {\n      transform: translate(0, 0); }\n    [aria-label][data-balloon-pos][data-balloon-pos^=\"up\"]:before, [aria-label][data-balloon-pos][data-balloon-pos^=\"up\"]:after {\n      bottom: 100%;\n      transform-origin: top;\n      transform: translate(0, var(--balloon-move)); }\n    [aria-label][data-balloon-pos][data-balloon-pos^=\"up\"]:after {\n      margin-bottom: 10px; }\n    [aria-label][data-balloon-pos][data-balloon-pos=\"up\"]:before, [aria-label][data-balloon-pos][data-balloon-pos=\"up\"]:after {\n      left: 50%;\n      transform: translate(-50%, var(--balloon-move)); }\n    [aria-label][data-balloon-pos][data-balloon-pos^=\"down\"]:before, [aria-label][data-balloon-pos][data-balloon-pos^=\"down\"]:after {\n      top: 100%;\n      transform: translate(0, calc(var(--balloon-move) * -1)); }\n    [aria-label][data-balloon-pos][data-balloon-pos^=\"down\"]:after {\n      margin-top: 10px; }\n    [aria-label][data-balloon-pos][data-balloon-pos^=\"down\"]:before {\n      width: 0;\n      height: 0;\n      border: 5px solid transparent;\n      border-bottom-color: var(--balloon-color); }\n    [aria-label][data-balloon-pos][data-balloon-pos=\"down\"]:after, [aria-label][data-balloon-pos][data-balloon-pos=\"down\"]:before {\n      left: 50%;\n      transform: translate(-50%, calc(var(--balloon-move) * -1)); }\n    [aria-label][data-balloon-pos][data-balloon-pos=\"left\"]:hover:after, [aria-label][data-balloon-pos][data-balloon-pos=\"left\"][data-balloon-visible]:after, [aria-label][data-balloon-pos][data-balloon-pos=\"right\"]:hover:after, [aria-label][data-balloon-pos][data-balloon-pos=\"right\"][data-balloon-visible]:after {\n      transform: translate(0, -50%); }\n    [aria-label][data-balloon-pos][data-balloon-pos=\"left\"]:hover:before, [aria-label][data-balloon-pos][data-balloon-pos=\"left\"][data-balloon-visible]:before, [aria-label][data-balloon-pos][data-balloon-pos=\"right\"]:hover:before, [aria-label][data-balloon-pos][data-balloon-pos=\"right\"][data-balloon-visible]:before {\n      transform: translate(0, -50%); }\n    [aria-label][data-balloon-pos][data-balloon-pos=\"left\"]:after, [aria-label][data-balloon-pos][data-balloon-pos=\"left\"]:before {\n      right: 100%;\n      top: 50%;\n      transform: translate(var(--balloon-move), -50%); }\n    [aria-label][data-balloon-pos][data-balloon-pos=\"left\"]:after {\n      margin-right: 10px; }\n    [aria-label][data-balloon-pos][data-balloon-pos=\"left\"]:before {\n      width: 0;\n      height: 0;\n      border: 5px solid transparent;\n      border-left-color: var(--balloon-color); }\n    [aria-label][data-balloon-pos][data-balloon-pos=\"right\"]:after, [aria-label][data-balloon-pos][data-balloon-pos=\"right\"]:before {\n      left: 100%;\n      top: 50%;\n      transform: translate(calc(var(--balloon-move) * -1), -50%); }\n    [aria-label][data-balloon-pos][data-balloon-pos=\"right\"]:after {\n      margin-left: 10px; }\n    [aria-label][data-balloon-pos][data-balloon-pos=\"right\"]:before {\n      width: 0;\n      height: 0;\n      border: 5px solid transparent;\n      border-right-color: var(--balloon-color); }\n    [aria-label][data-balloon-pos][data-balloon-length]:after {\n      white-space: normal; }\n    [aria-label][data-balloon-pos][data-balloon-length=\"small\"]:after {\n      width: 80px; }\n    [aria-label][data-balloon-pos][data-balloon-length=\"medium\"]:after {\n      width: 150px; }\n    [aria-label][data-balloon-pos][data-balloon-length=\"large\"]:after {\n      width: 260px; }\n    [aria-label][data-balloon-pos][data-balloon-length=\"xlarge\"]:after {\n      width: 380px; }\n      @media screen and (max-width: 768px) {\n        [aria-label][data-balloon-pos][data-balloon-length=\"xlarge\"]:after {\n          width: 90vw; } }\n    [aria-label][data-balloon-pos][data-balloon-length=\"fit\"]:after {\n      width: 100%; }",
-        "@import \"normalize.css\";\n@import \"balloon.css\";\n\n/**\n=========\nVars\n=========\n*/\n\n:root {\n  --color-primary: #489fd9;\n  --color-primary-light: #abd9f7;\n  --color-primary-400: #3d7da9;\n  --color-primary-300: #315d7c;\n  --color-primary-200: #253e52;\n  --color-primary-100: #151d24;\n  --color-accent: #e37dd7;\n  --color-accent-light: #f794d5;\n  --color-accent-400: #b163a8;\n  --color-accent-300: #824b7b;\n  --color-accent-200: #563351;\n  --color-accent-100: #2d1d2a;\n\n  --color-body: #dfedf7;\n  --color-muted: #a3c1d4;\n  --color-background: var(--color-primary-100);\n  --anchor-color: #e3ddf0;\n  --anchor-color-hover: var(--color-accent-light);\n  --border-color: var(--color-primary-300);\n  --balloon-color: var(--color-primary-400);\n\n  --font-size-sm: .875rem;\n  --font-size-regular: 1rem;\n  --font-size-lg: 1.25rem;\n  --font-size-xlg: 2rem;\n  --font-size-xxlg: 3rem;\n}\n\n\n$displays: none, inline, inline-block, block, table, table-row, table-cell, flex, inline-flex !default;\n\n$spacer: 1rem !default;\n$spacers: () !default;\n$spacers: map-merge(\n  (\n    0: 0,\n    1: (\n      $spacer * 0.25\n    ),\n    2: (\n      $spacer * 0.5\n    ),\n    3: $spacer,\n    4: (\n      $spacer * 1.5\n    ),\n    5: (\n      $spacer * 2.5\n    ),\n  ),\n  $spacers\n);\n\n$grid-breakpoints: (\n  xs: 0,\n  // sm: 576px,\n  md: 768px,\n  // lg: 992px,\n  // xl: 1280px\n) !default;\n\n@import \"helpers.scss\";\n@import \"carousel.scss\";\n@import \"button.scss\";\n@import \"select.scss\";\n\n/**\n=========\nElemens\n=========\n*/\n\nh1,\nh2,\nh3,\nh4,\nh5,\nh6,\np {\n  margin: 0;\n}\n\nbody {\n  display: flex;\n  font: normal 1rem/1.5 system-ui, sans-serif;\n  color: var(--color-body);\n  background-color: var(--color-background);\n}\n\nh1,\nh2,\nh3,\nh4,\nh5,\nh6 {\n    line-height: 1.1;\n}\n\na {\n  color: inherit;\n  transition: color .1s ease-in;\n}\n\na:hover {\n  color: var(--anchor-color-hover);\n}\n\na:visited {\n  text-decoration: dotted;\n}\n\n:target {\n  color: var(--anchor-color-hover);\n}\n\ncode {\n  font-family: ui-monospace, Menlo, Monaco, Courier New, monospace;\n}\n\nhr {\n  border-top: 1px solid var(--border-color);\n  border-bottom: 0;\n}\n\ndl {\n\n}\n\ndt {\n  font-size: var(--font-size-sm);\n  text-transform: uppercase;\n  font-weight: 600;\n  color: var(--color-muted);\n}\n\ndd {\n  margin: 0 0 1rem 0;\n  font-size: var(--font-size-sm);\n}\n\n.badge {\n  padding: .1875rem .375rem;\n  border-radius: .5rem;\n  text-decoration: none;\n  color: var(--color-muted);\n  background-color: var(--color-primary-300);\n  /* transition: border-color .1s ease-in; */\n}\n\n.badge--outline {\n  padding: .1875rem .375rem;\n  border: 2px solid var(--color-primary-300);\n  border-radius: .5rem;\n  text-decoration: none;\n  color: var(--color-muted);\n  transition: border-color .1s ease-in;\n}\n\n.badge--outline:hover {\n  border-color: var(--anchor-color-hover);\n}\n\n\n.badge--pill {\n  border-radius: 1rem;\n}\n\n.badge-res {\n  background: var(--color-primary-200);\n  color: #fff;\n  padding: 0 3px;\n  border-radius: 4px;\n  font-size: 12px;\n  text-shadow: 1px 1px 0 #4d5078;\n}\n\n.badge-2160 {\n  background: #b82927;\n}\n\n.badge-1080 {\n  background: #e0560b;\n}\n\n.badge-720 {\n  background: var(--color-accent);\n}\n\n.badge-480 {\n  background: #269ddb;\n}\n\n.torrent-hi {}\n\n.torrent-medium {\n  color: #f0ed60;\n}\n\n.torrent-low {\n  color: #cf4d4a;\n}\n\n/* FORMS */\n\nfieldset {\n  padding: 0;\n  margin: 0;\n  border: 0;  \n}\n\nlegend {\n  font-size: var(--font-size-sm);\n  text-transform: uppercase;\n  font-weight: 600;\n  color: var(--color-muted);\n}\n\n/* TABLES */\n\n.report,\n.table {\n  border-collapse: collapse;\n}\n\n.table td {\n  padding: 0.1875rem 0.5rem 0.1875rem 0;\n}\n\n.table tr {\n  transition: background-color .1s ease-out;\n}\n\n.table tr:hover  {\n  background-color: #253e52;\n}\n\n.report td {\n  padding: 0.5em 0 0.5em 0;\n  border-bottom: 1px solid var(--color-primary-200);\n}\n\n.report th,\n.table th {\n  padding: 0.375rem 0.5rem 0.375rem 0;\n  border-bottom: 1px solid var(--color-primary-200);\n  color: var(--color-muted);\n  font-weight: 600;\n  text-transform: uppercase;\n  font-size: var(--font-size-sm);\n}\n\n/* CARDS */\n\n@media screen and (min-width: 768px) {\n  .card-series {\n    max-width: 10rem;\n  }\n}\n\n.card-series__image {\n  aspect-ratio: 500 / 750;\n  transition: transform .2s ease-out, filter .3s ease-out, box-shadow .2s ease-out;\n  border: 2px solid var(--color-primary-200);\n  box-shadow: var(--color-primary-200) 0 0;\n  background-color: var(--color-accent-200);\n  background-position: top left;\n  background-image: linear-gradient(125deg, var(--color-accent-400) 25%, transparent 25%)\n}\n\na:hover .card-series__image {\n  transform: translate(-7px, -7px);\n  filter: brightness(1.25);\n  box-shadow: var(--color-primary-200) 7px 7px;\n}\n\n// .card-series__name {\n//   opacity: 0;\n// }\n\n// a:hover .card-series__name {\n//   opacity: 1;\n// }\n\n.search-query {\n  position: relative;\n  width: min-content;\n}\n\n.search-query input {\n  padding: .75rem .5rem;\n  background: var(--color-background);\n  border: 2px solid var(--color-primary-400);\n  color: var(--color-primary-light);\n  border-radius: .5rem;\n  font-size: var(--font-size-lg);\n  // box-shadow: 0 0 5px 2px var(--color-primary), inset 0 0 2px 1px var(--color-primary);\n}\n\n/* Hide arrow on Chrome https://stackoverflow.com/questions/20937475/remove-datalist-dropdown-arrow-in-chrome */\n.search-query input::-webkit-calendar-picker-indicator {\n  display: none !important;\n}\n\n\n@media screen and (min-width: 768px) {\n  .search-query input {\n    width: 30rem;\n  }\n}\n\n.search-query input:focus-visible {\n  outline: none;\n  // box-shadow: 0 0 5px 2px var(--color-accent), inset 0 0 2px 1px var(--color-accent);\n  border: 2px solid var(--anchor-color-hover);\n}\n\ninput::placeholder {\n  color: var(--color-primary-300);\n}\n\n.search-query button {\n  position: absolute;\n  top: 0;\n  right: 0;\n  z-index: 1;\n  padding: .75rem;\n  /* border: 2px solid var(--color-primary-400); */\n  border: 0;\n  /* border-left: 0; */\n  /* border-top-right-radius: .5rem;\n  border-bottom-right-radius: .5rem; */\n  /* background: var(--color-primary);\n  background-image: linear-gradient(180deg, rgba(255, 255, 255, 0.35) 0%, rgba(29, 41, 43, 1) 100%);\n  background-blend-mode: overlay; */\n  background: var(--color-background);\n  background: transparent;\n  /* color: var(--color-background); */\n  cursor: pointer;\n  /* transition: color .1s ease-in; */\n  font-size: var(--font-size-lg);\n  /* box-shadow: 0 0 5px 2px var(--color-primary);  */\n}\n\n.search-query button img {}\n\n\na:hover .card-episode__poster,\na:hover .card-episode__image,\n.btn-text:hover .card-episode__image {\n  border-color: var(--color-accent);\n  transition: border-color .1s ease-in;\n}\n\n\n.header .btn-icon:hover {\n  background-color: var(--color-primary-300);\n  transition: background-color .2s ease-out;\n}\n\n.header {\n  position: sticky;\n  top: 0;\n  height: 100vh;\n  display: flex;\n  gap: .5rem;\n  flex-direction: column;\n  background: var(--color-primary-200);\n}\n\n.header .btn-icon {\n  padding: .75rem;\n}\n\n/* Recolor icons site-wide, see generator at https://codepen.io/sosuke/pen/Pjoqqp */\n.icon,\n.header .btn-icon img {\n  filter: invert(88%) sepia(3%) saturate(2496%) hue-rotate(185deg) brightness(106%) contrast(94%);\n}\n\n.header .btn-icon:hover img {\n  filter: invert(78%) sepia(13%) saturate(3097%) hue-rotate(274deg) brightness(96%) contrast(85%);\n}\n\n@media screen and (min-width: 768px) {\n  .header {\n\n    /* justify-content: space-between; */\n    align-items: center;\n    /* padding: 1rem 0;\n    margin: 0 0 2rem 0; */\n  }\n\n  nav {\n    /* Push right */\n    /* margin-left: auto; */\n    background: none;\n  }\n\n  /* nav .btn-icon {\n    padding: 0;\n  } */\n}\n\nmain {\n  flex-grow: 1;\n  padding: 3rem;\n}\n\n.footer {\n  color: var(--color-muted);\n}\n\naside {\n  flex-basis: 14rem;\n  flex-shrink: 0;\n}\n\n.main-column {\n  flex-grow: 1;\n}\n\n// .today-series {\n//   display: grid;\n//   grid-template-columns: 1fr 2fr;  \n//   gap: 3rem;\n//   align-items: center;\n// }\n\n.card-episode {\n  position: relative;\n}\n\n.card-episode__image {\n  aspect-ratio: 300 / 170;  \n  transition: transform .2s ease-out, filter .3s ease-out, box-shadow .2s ease-out;\n  border: 2px solid var(--color-primary-300);\n  // box-shadow: var(--color-primary-200) 0 0;\n  background-position: top left;\n  background-color: var(--color-accent-200);\n  background-image: linear-gradient(125deg, var(--color-accent-400) 25%, transparent 25%);\n}\n\n.card-episode__poster {\n    max-width: 75px;\n    position: absolute;\n    bottom: -1rem;\n    right: 1rem;\n    z-index: 1;\n    border: 2px solid var(--color-primary-300);\n}\n\n// a:hover .card-episode__image {\n//   transform: translate(-7px, -7px);\n//   filter: brightness(1.25);\n//   box-shadow: var(--color-primary-200) 7px 7px;\n// }\n\n.series-poster__image {\n  aspect-ratio: 500 / 750;\n  border: 2px solid var(--color-primary-200);\n  background-position: top left;\n  background-color: var(--color-accent-200);\n  background-image: linear-gradient(125deg, var(--color-accent-400) 25%, transparent 25%);\n}\n\n@media screen and (min-width: 768px) {\n  .series-poster__image {\n    box-shadow: var(--color-primary-200) 7px 7px;\n  }\n}\n\n.episode-grid {\n    display: grid;\n    grid-template-columns: repeat(4, 1fr);\n    grid-template-rows: auto;\n    gap: 2rem;\n}\n\n.episode-grid__cell {\n  max-width: 300px;\n}\n\n/* .episode-grid__cell .view-all {\n  visibility: hidden;\n}\n\n.episode-grid__cell:hover .view-all {\n  visibility: visible;\n} */\n\n/* .series-vote {\n  position: absolute;\n  bottom: -3rem;\n  left: calc(50% - 2rem);\n  width: 4rem;\n  height: 4rem;\n  display: flex;\n  align-items: center;\n  justify-content: center;\n  border-radius: 50%;\n  color: var(--color-muted);\n  border: .25rem solid var(--color-primary-400);\n  background: var(--color-primary-100);\n}\n\n.series-vote span { \n  font-weight: 900;\n  color: var(--color-accent-light);\n  font-size: 1.5rem;\n} */\n\n\n.body-copy,\n.series-overview {\n  max-width: 75ch;\n}\n\n.fanart {\n  /* Bleed background into parent container */\n  margin-top: -3rem;\n  margin-right: -3rem;\n  margin-left: -3rem;\n  padding: 3rem 3rem 3rem 3rem;\n  background-position: top center;\n  background-attachment: fixed;\n  background-repeat: no-repeat;\n  background-size: cover;\n  background-blend-mode: multiply;\n  background-color: var(--color-accent-100);\n}\n\n@media screen and (min-width: 768px) {\n  .top-series-grid {\n    display: grid;\n    grid-template-columns: repeat(2, 1fr);\n    gap: 2rem;\n  }\n}\n\n.cards-grid {\n  display: grid;\n  grid-template-columns: repeat(3, 1fr);\n  gap: 1.5rem;\n  margin-bottom: 2rem;\n}\n\n@media screen and (min-width: 768px) {\n  .cards-grid {\n    grid-template-columns: repeat(6, 1fr);\n    gap: 2rem;\n  }\n}\n\ndialog {\n  background: transparent;\n  border: 0;\n  opacity: 0;\n  padding: 0;\n  margin: 0;\n  width: 100vw;\n  height: 100vh;\n  color: var(--color-body);\n  /* transition: transform .3s ease-out, opacity .3s ease-out;\n  transform: translate(0%, -5%); */\n  /* Reset browser defaults */\n  max-width: unset;\n  max-height: unset;\n}\n\n.dialog-body {\n  width: 30rem;\n  background: var(--color-primary-200);\n  padding: 2rem;\n  border-radius: 1rem;\n}\n\n.dialog-body--small {\n  width: 16rem;\n}\n\ndialog:modal {\n  display: flex;\n  align-items: center;\n  justify-content: center;\n  opacity: 1;\n  /* transform: translate(0%, 0%); */\n}\n\ndialog::backdrop {\n  background: rgba(21, 29, 39, .75);\n}\n\ndialog button[name=\"close\"] {\n  position: absolute;\n  top: 0;\n  right: 0;\n  z-index: 1;\n}\n\n/* Animations  */\n\n.anim-spin {\n  animation-name: spin;\n  animation-duration: 4s;\n  animation-iteration-count: infinite;\n  animation-timing-function: linear;\n}\n\n@keyframes spin {\n  from {\n    transform: rotate(0deg);\n  }\n\n  to {\n    transform: rotate(360deg);\n  }\n}\n\n/* A11y */\n\n.sr-only {\n  position: absolute;\n  white-space: nowrap;\n  width: 1px;\n  height: 1px;\n  overflow: hidden;\n  border: 0;\n  padding: 0;\n  clip: rect(0 0 0 0);\n  clip-path: inset(50%);\n  margin: -1px;\n}\n\n.skip-nav a {\n  position: absolute;\n  left: -9999px;\n  top: auto;\n  width: 1px;\n  height: 1px;\n  overflow: hidden;\n}\n\n.skip-nav a:focus {\n  position: static;\n  width: auto;\n  height: auto;\n}\n\n\n\n/*  \n  CSS mobile carousel, see: \n  https://css-tricks.com/can-get-pretty-far-making-slider-just-html-css/\n*/\n\n.mobile-carousel {\n  display: flex;\n  gap: 1.5rem;\n}\n\n@media screen and (max-width: 767.98px) {\n  .mobile-carousel {\n    display: flex;\n    scroll-behavior: smooth;\n    -webkit-overflow-scrolling: touch;\n    overflow-x: scroll;\n    scroll-snap-type: x mandatory;\n    margin: 0 -1rem 0 0;\n  }\n\n  .mobile-carousel>.mobile-carousel__item {\n    scroll-snap-align: start;\n    flex-shrink: 0;\n    /* 50% of the viewport width */\n    flex-basis: 50vw;\n  }\n\n  /* On mobile we want the swiping behavior but not the scroll bar */\n  .mobile-carousel::-webkit-scrollbar {\n    display: none;\n  }\n}\n\n@media screen and (min-width: 768px) {\n  .mobile-carousel {\n    gap: 2rem;\n    /* justify-content: space-between; */\n  }\n}\n\n/* Radio button group  */\n\n.radio-button-group {\n  display: flex;\n  border: 2px solid var(--color-primary-400);\n  color: var(--color-primary-light);\n  border-radius: .5rem;\n  // box-shadow: 0 0 5px 2px var(--color-primary), inset 0 0 2px 1px var(--color-primary);\n  font-size: var(--font-size-sm);\n  background-color: var(--color-primary-100);\n}\n\n.radio-button-group__label {\n  align-items: center;\n  display: inline-flex;\n  /* border-right: 1px solid var(--border-color); */\n  border-radius: .4rem;\n  padding: 0.5rem;\n  background-color: transparent;\n  color: var(--color-body);\n  cursor: pointer;\n}\n\n/* .radio-button-group__label:last-child {\n  border-right-color: transparent;\n} */\n\n.radio-button-group__label:has(input:checked) {\n  /* For selected radio */\n  background-color: var(--color-primary-300);\n  /* color: var(--color-primary-100); */\n}\n\n.radio-button-group__input {\n  position: absolute;\n  width: 1px;\n  height: 1px;\n  padding: 0;\n  overflow: hidden;\n  clip: rect(0, 0, 0, 0);\n  white-space: nowrap;\n  border: 0;  \n}\n\n/* Progress  */\n\nprogress {\n  accent-color: var(--color-accent-light);\n}",
-        "// Lifted from Bootstrap 4\n\n@function breakpoint-infix($name, $breakpoints: $grid-breakpoints) {\n  @return if(breakpoint-min($name, $breakpoints)==null, \"\", \"-#{$name}\");\n}\n\n@function breakpoint-next($name, $breakpoints: $grid-breakpoints, $breakpoint-names: map-keys($breakpoints)) {\n  $n: index($breakpoint-names, $name);\n  @return if($n !=null and $n < length($breakpoint-names), nth($breakpoint-names, $n + 1), null);\n}\n\n@function breakpoint-min($name, $breakpoints: $grid-breakpoints) {\n  $min: map-get($breakpoints, $name);\n  @return if($min !=0, $min, null);\n}\n\n@function breakpoint-max($name, $breakpoints: $grid-breakpoints) {\n  $next: breakpoint-next($name, $breakpoints);\n  @return if($next, breakpoint-min($next, $breakpoints) - .02, null);\n}\n\n@mixin media-breakpoint-up($name, $breakpoints: $grid-breakpoints) {\n  $min: breakpoint-min($name, $breakpoints);\n\n  @if $min {\n    @media (min-width: $min) {\n      @content;\n    }\n  }\n\n  @else {\n    @content;\n  }\n}\n\n@mixin media-breakpoint-down($name, $breakpoints: $grid-breakpoints) {\n  $max: breakpoint-max($name, $breakpoints);\n\n  @if $max {\n    @media (max-width: $max) {\n      @content;\n    }\n  }\n\n  @else {\n    @content;\n  }\n}\n\n// Display\n\n@each $breakpoint in map-keys($grid-breakpoints) {\n  @include media-breakpoint-up($breakpoint) {\n    $infix: breakpoint-infix($breakpoint, $grid-breakpoints);\n\n    @each $value in $displays {\n      .d#{$infix}-#{$value} {\n        display: $value !important;\n      }\n    }\n  }\n}\n\n// Margin and padding\n\n@each $breakpoint in map-keys($grid-breakpoints) {\n  @include media-breakpoint-up($breakpoint) {\n    $infix: breakpoint-infix($breakpoint, $grid-breakpoints);\n\n    @each $prop, $abbrev in (margin: m, padding: p) {\n      @each $size, $length in $spacers {\n        .#{$abbrev}#{$infix}-#{$size} {\n          #{$prop}: $length !important;\n        }\n\n        .#{$abbrev}t#{$infix}-#{$size},\n        .#{$abbrev}y#{$infix}-#{$size} {\n          #{$prop}-top: $length !important;\n        }\n\n        .#{$abbrev}r#{$infix}-#{$size},\n        .#{$abbrev}x#{$infix}-#{$size} {\n          #{$prop}-right: $length !important;\n        }\n\n        .#{$abbrev}b#{$infix}-#{$size},\n        .#{$abbrev}y#{$infix}-#{$size} {\n          #{$prop}-bottom: $length !important;\n        }\n\n        .#{$abbrev}l#{$infix}-#{$size},\n        .#{$abbrev}x#{$infix}-#{$size} {\n          #{$prop}-left: $length !important;\n        }\n      }\n    }\n\n    // Negative margins (e.g., where `.mb-n1` is negative version of `.mb-1`)\n    @each $size, $length in $spacers {\n      @if $size !=0 {\n        .m#{$infix}-n#{$size} {\n          margin: -$length !important;\n        }\n\n        .mt#{$infix}-n#{$size},\n        .my#{$infix}-n#{$size} {\n          margin-top: -$length !important;\n        }\n\n        .mr#{$infix}-n#{$size},\n        .mx#{$infix}-n#{$size} {\n          margin-right: -$length !important;\n        }\n\n        .mb#{$infix}-n#{$size},\n        .my#{$infix}-n#{$size} {\n          margin-bottom: -$length !important;\n        }\n\n        .ml#{$infix}-n#{$size},\n        .mx#{$infix}-n#{$size} {\n          margin-left: -$length !important;\n        }\n      }\n    }\n\n    // Some special margin utils\n    .m#{$infix}-auto {\n      margin: auto !important;\n    }\n\n    .mt#{$infix}-auto,\n    .my#{$infix}-auto {\n      margin-top: auto !important;\n    }\n\n    .mr#{$infix}-auto,\n    .mx#{$infix}-auto {\n      margin-right: auto !important;\n    }\n\n    .mb#{$infix}-auto,\n    .my#{$infix}-auto {\n      margin-bottom: auto !important;\n    }\n\n    .ml#{$infix}-auto,\n    .mx#{$infix}-auto {\n      margin-left: auto !important;\n    }\n  }\n}\n\n// Flex variations\n\n@each $breakpoint in map-keys($grid-breakpoints) {\n  @include media-breakpoint-up($breakpoint) {\n    $infix: breakpoint-infix($breakpoint, $grid-breakpoints);\n\n    .flex#{$infix}-row {\n      flex-direction: row !important;\n    }\n\n    .flex#{$infix}-column {\n      flex-direction: column !important;\n    }\n\n    .flex#{$infix}-row-reverse {\n      flex-direction: row-reverse !important;\n    }\n\n    .flex#{$infix}-column-reverse {\n      flex-direction: column-reverse !important;\n    }\n\n    .flex#{$infix}-wrap {\n      flex-wrap: wrap !important;\n    }\n\n    .flex#{$infix}-nowrap {\n      flex-wrap: nowrap !important;\n    }\n\n    .flex#{$infix}-wrap-reverse {\n      flex-wrap: wrap-reverse !important;\n    }\n\n    .flex#{$infix}-fill {\n      flex: 1 1 auto !important;\n    }\n\n    .flex#{$infix}-grow-0 {\n      flex-grow: 0 !important;\n    }\n\n    .flex#{$infix}-grow-1 {\n      flex-grow: 1 !important;\n    }\n\n    .flex#{$infix}-shrink-0 {\n      flex-shrink: 0 !important;\n    }\n\n    .flex#{$infix}-shrink-1 {\n      flex-shrink: 1 !important;\n    }\n\n    .justify-content#{$infix}-start {\n      justify-content: flex-start !important;\n    }\n\n    .justify-content#{$infix}-end {\n      justify-content: flex-end !important;\n    }\n\n    .justify-content#{$infix}-center {\n      justify-content: center !important;\n    }\n\n    .justify-content#{$infix}-between {\n      justify-content: space-between !important;\n    }\n\n    .justify-content#{$infix}-around {\n      justify-content: space-around !important;\n    }\n\n    .align-items#{$infix}-start {\n      align-items: flex-start !important;\n    }\n\n    .align-items#{$infix}-end {\n      align-items: flex-end !important;\n    }\n\n    .align-items#{$infix}-center {\n      align-items: center !important;\n    }\n\n    .align-items#{$infix}-baseline {\n      align-items: baseline !important;\n    }\n\n    .align-items#{$infix}-stretch {\n      align-items: stretch !important;\n    }\n\n    .align-content#{$infix}-start {\n      align-content: flex-start !important;\n    }\n\n    .align-content#{$infix}-end {\n      align-content: flex-end !important;\n    }\n\n    .align-content#{$infix}-center {\n      align-content: center !important;\n    }\n\n    .align-content#{$infix}-between {\n      align-content: space-between !important;\n    }\n\n    .align-content#{$infix}-around {\n      align-content: space-around !important;\n    }\n\n    .align-content#{$infix}-stretch {\n      align-content: stretch !important;\n    }\n\n    .align-self#{$infix}-auto {\n      align-self: auto !important;\n    }\n\n    .align-self#{$infix}-start {\n      align-self: flex-start !important;\n    }\n\n    .align-self#{$infix}-end {\n      align-self: flex-end !important;\n    }\n\n    .align-self#{$infix}-center {\n      align-self: center !important;\n    }\n\n    .align-self#{$infix}-baseline {\n      align-self: baseline !important;\n    }\n\n    .align-self#{$infix}-stretch {\n      align-self: stretch !important;\n    }\n  }\n}\n\n// Typography \n\nsmall,\n.text-sm {\n  font-size: var(--font-size-sm) !important;\n}\n\n.text-regular {\n  font-size: var(--font-size-regular) !important;\n}\n\n.text-lg {\n  font-size: var(--font-size-lg) !important;\n}\n\n.text-xlg {\n  font-size: var(--font-size-xlg) !important;\n}\n\n.text-right {\n  text-align: right;\n}\n\n.text-left {\n  text-align: left;\n}\n\n.text-center {\n  text-align: center;\n}\n\n.text-muted {\n  color: var(--color-muted) !important;\n}\n\n.text-uppercase {\n  text-transform: uppercase;\n}\n\n.font-weight-normal {\n  font-weight: normal;\n}\n\n.font-weight-bold {\n  font-weight: bold;\n}\n\n.font-weight-semibold {\n  font-weight: 600;\n}\n\n.font-weight-black {\n  font-weight: 900;\n}\n\n.font-style-italic {\n  font-style: italic;\n}\n\n.line-height-1 {\n  line-height: 1;\n}\n\n.text-decoration-none {\n  text-decoration: none;\n}\n\n.text-break-all {\n  word-break: break-all;\n}\n\n.text-nowrap {\n  white-space: nowrap\n}\n\n// Misc helpers\n\n.position-relative {\n  position: relative;\n}\n\n.img-fluid {\n  max-width: 100%;\n  height: auto;\n}\n\n.zero {\n  margin: 0;\n  padding: 0;\n}\n\n.invisible {\n  visibility: hidden;\n}\n\n.h-100 {\n  height: 100%;\n}\n\n.w-100 {\n  width: 100%;\n}\n\n.d-grid {\n  display: grid;\n  grid-auto-flow: column;\n  grid-auto-columns: 1fr;\n}\n\n.rounded {\n  border-radius: .5rem;\n}\n\n// Border \n\n.border {\n  border: 1px solid var(--border-color);\n}\n\n.border-top {\n  border-top: 1px solid var(--color-primary-300);\n}\n\n.border-bottom {\n  border-bottom: 1px solid var(--color-primary-300);\n}\n\n.border-right {\n  border-right: 1px solid var(--color-primary-300);\n}\n\n.border-left {\n  border-left: 1px solid var(--color-primary-300);\n}",
+        "@import \"normalize.css\";\n@import \"balloon.css\";\n\n/**\n=========\nVars\n=========\n*/\n\n:root {\n  --color-primary: #489fd9;\n  --color-primary-light: #abd9f7;\n  --color-primary-400: #3d7da9;\n  --color-primary-300: #315d7c;\n  --color-primary-200: #253e52;\n  --color-primary-100: #151d24;\n  --color-accent: #e37dd7;\n  --color-accent-light: #f794d5;\n  --color-accent-400: #b163a8;\n  --color-accent-300: #824b7b;\n  --color-accent-200: #563351;\n  --color-accent-100: #2d1d2a;\n\n  --color-body: #dfedf7;\n  --color-muted: #a3c1d4;\n  --color-background: var(--color-primary-100);\n  --anchor-color: #e3ddf0;\n  --anchor-color-hover: var(--color-accent-light);\n  --border-color: var(--color-primary-300);\n  --border-color-accent: var(--color-accent);\n  --balloon-color: var(--color-primary-400);\n\n  --color-success: #59c27c;\n  --color-warning: #f0ee78;\n  --color-danger: #cf4d4a;\n\n  --font-size-sm: .875rem;\n  --font-size-regular: 1rem;\n  --font-size-lg: 1.25rem;\n  --font-size-xlg: 2rem;\n  --font-size-xxlg: 3rem;\n}\n\n\n$displays: none, inline, inline-block, block, table, table-row, table-cell, flex, inline-flex !default;\n\n$spacer: 1rem !default;\n$spacers: () !default;\n$spacers: map-merge(\n  (\n    0: 0,\n    1: (\n      $spacer * 0.25\n    ),\n    2: (\n      $spacer * 0.5\n    ),\n    3: $spacer,\n    4: (\n      $spacer * 1.5\n    ),\n    5: (\n      $spacer * 2.5\n    ),\n  ),\n  $spacers\n);\n\n$grid-breakpoints: (\n  xs: 0,\n  // sm: 576px,\n  md: 768px,\n  // lg: 992px,\n  // xl: 1280px\n) !default;\n\n@import \"helpers.scss\";\n@import \"carousel.scss\";\n@import \"button.scss\";\n@import \"select.scss\";\n\n/**\n=========\nElemens\n=========\n*/\n\nh1,\nh2,\nh3,\nh4,\nh5,\nh6,\np {\n  margin: 0;\n}\n\nbody {\n  display: flex;\n  font: normal 1rem/1.5 system-ui, sans-serif;\n  color: var(--color-body);\n  background-color: var(--color-background);\n}\n\nh1,\nh2,\nh3,\nh4,\nh5,\nh6 {\n    line-height: 1.1;\n}\n\na {\n  color: inherit;\n  transition: color .1s ease-in;\n}\n\na:hover {\n  color: var(--anchor-color-hover);\n}\n\na:visited {\n  text-decoration: dotted;\n}\n\n:target {\n  color: var(--anchor-color-hover);\n}\n\ncode {\n  font-family: ui-monospace, Menlo, Monaco, Courier New, monospace;\n}\n\nhr {\n  border-top: 1px solid var(--border-color);\n  border-bottom: 0;\n}\n\ndl {\n\n}\n\ndt {\n  font-size: var(--font-size-sm);\n  text-transform: uppercase;\n  font-weight: 600;\n  color: var(--color-muted);\n}\n\ndd {\n  margin: 0 0 1rem 0;\n  font-size: var(--font-size-sm);\n}\n\n.badge {\n  padding: .1875rem .375rem;\n  border-radius: .5rem;\n  text-decoration: none;\n  color: var(--color-muted);\n  background-color: var(--color-primary-300);\n  /* transition: border-color .1s ease-in; */\n}\n\n.badge--outline {\n  padding: .1875rem .375rem;\n  border: 2px solid var(--color-primary-300);\n  border-radius: .5rem;\n  text-decoration: none;\n  color: var(--color-muted);\n  transition: border-color .1s ease-in;\n}\n\n.badge--outline:hover {\n  border-color: var(--anchor-color-hover);\n}\n\n\n.badge--pill {\n  border-radius: 1rem;\n}\n\n.badge-res {\n  background: var(--color-primary-200);\n  color: #fff;\n  padding: 0 3px;\n  border-radius: 4px;\n  font-size: 12px;\n  text-shadow: 1px 1px 0 #4d5078;\n}\n\n.badge-2160 {\n  background: #b82927;\n}\n\n.badge-1080 {\n  background: #e0560b;\n}\n\n.badge-720 {\n  background: var(--color-accent);\n}\n\n.badge-480 {\n  background: #269ddb;\n}\n\n.torrent-hi {}\n\n.torrent-medium {\n  color: var(--color-warning);\n}\n\n.torrent-low {\n  color: var(--color-danger);\n}\n\n/* FORMS */\n\nfieldset {\n  padding: 0;\n  margin: 0;\n  border: 0;  \n}\n\nlegend {\n  font-size: var(--font-size-sm);\n  text-transform: uppercase;\n  font-weight: 600;\n  color: var(--color-muted);\n}\n\n/* TABLES */\n\n.report,\n.table {\n  border-collapse: collapse;\n}\n\n.table td {\n  padding: 0.1875rem 0.5rem 0.1875rem 0;\n}\n\n.table tr {\n  transition: background-color .1s ease-out;\n}\n\n.table tr:hover  {\n  background-color: #253e52;\n}\n\n.report td {\n  padding: 0.25em 2rem 0.25rem 0;\n  // border-bottom: 1px solid var(--color-primary-200);\n}\n\n.report th,\n.table th {\n  padding: 0.375rem 0.5rem 0.375rem 0;\n  border-bottom: 1px solid var(--color-primary-200);\n  color: var(--color-muted);\n  font-weight: 600;\n  text-transform: uppercase;\n  font-size: var(--font-size-sm);\n}\n\n/* CARDS */\n\n@media screen and (min-width: 768px) {\n  .card-series {\n    max-width: 10rem;\n  }\n}\n\n.card-series__image {\n  aspect-ratio: 500 / 750;\n  transition: transform .2s ease-out, filter .3s ease-out, box-shadow .2s ease-out;\n  border: 2px solid var(--color-primary-200);\n  box-shadow: var(--color-primary-200) 0 0;\n  background-color: var(--color-accent-200);\n  background-position: top left;\n  background-image: linear-gradient(125deg, var(--color-accent-400) 25%, transparent 25%)\n}\n\na:hover .card-series__image {\n  transform: translate(-7px, -7px);\n  filter: brightness(1.25);\n  box-shadow: var(--color-primary-200) 7px 7px;\n}\n\n// .card-series__name {\n//   opacity: 0;\n// }\n\n// a:hover .card-series__name {\n//   opacity: 1;\n// }\n\n.search-query {\n  position: relative;\n  width: min-content;\n}\n\n.search-query input {\n  padding: .75rem .5rem;\n  background: var(--color-background);\n  border: 2px solid var(--color-primary-400);\n  color: var(--color-primary-light);\n  border-radius: .5rem;\n  font-size: var(--font-size-lg);\n  // box-shadow: 0 0 5px 2px var(--color-primary), inset 0 0 2px 1px var(--color-primary);\n}\n\n/* Hide arrow on Chrome https://stackoverflow.com/questions/20937475/remove-datalist-dropdown-arrow-in-chrome */\n.search-query input::-webkit-calendar-picker-indicator {\n  display: none !important;\n}\n\n\n@media screen and (min-width: 768px) {\n  .search-query input {\n    width: 30rem;\n  }\n}\n\n.search-query input:focus-visible {\n  outline: none;\n  // box-shadow: 0 0 5px 2px var(--color-accent), inset 0 0 2px 1px var(--color-accent);\n  border: 2px solid var(--anchor-color-hover);\n}\n\ninput::placeholder {\n  color: var(--color-primary-300);\n}\n\n.search-query button {\n  position: absolute;\n  top: 0;\n  right: 0;\n  z-index: 1;\n  padding: .75rem;\n  /* border: 2px solid var(--color-primary-400); */\n  border: 0;\n  /* border-left: 0; */\n  /* border-top-right-radius: .5rem;\n  border-bottom-right-radius: .5rem; */\n  /* background: var(--color-primary);\n  background-image: linear-gradient(180deg, rgba(255, 255, 255, 0.35) 0%, rgba(29, 41, 43, 1) 100%);\n  background-blend-mode: overlay; */\n  background: var(--color-background);\n  background: transparent;\n  /* color: var(--color-background); */\n  cursor: pointer;\n  /* transition: color .1s ease-in; */\n  font-size: var(--font-size-lg);\n  /* box-shadow: 0 0 5px 2px var(--color-primary);  */\n}\n\n.search-query button img {}\n\n\na:hover .card-episode__poster,\na:hover .card-episode__image,\n.btn-text:hover .card-episode__image {\n  border-color: var(--color-accent);\n  transition: border-color .1s ease-in;\n}\n\n\n.header .btn-icon:hover {\n  background-color: var(--color-primary-300);\n  transition: background-color .2s ease-out;\n}\n\n.header {\n  position: sticky;\n  top: 0;\n  height: 100vh;\n  display: flex;\n  gap: .5rem;\n  flex-direction: column;\n  background: var(--color-primary-200);\n}\n\n.header .btn-icon {\n  padding: .75rem;\n}\n\n/* Recolor icons site-wide, see generator at https://codepen.io/sosuke/pen/Pjoqqp */\n.icon,\n.header .btn-icon img {\n  filter: invert(88%) sepia(3%) saturate(2496%) hue-rotate(185deg) brightness(106%) contrast(94%);\n}\n\n.header .btn-icon:hover img {\n  filter: invert(78%) sepia(13%) saturate(3097%) hue-rotate(274deg) brightness(96%) contrast(85%);\n}\n\n@media screen and (min-width: 768px) {\n  .header {\n\n    /* justify-content: space-between; */\n    align-items: center;\n    /* padding: 1rem 0;\n    margin: 0 0 2rem 0; */\n  }\n\n  nav {\n    /* Push right */\n    /* margin-left: auto; */\n    background: none;\n  }\n\n  /* nav .btn-icon {\n    padding: 0;\n  } */\n}\n\nmain {\n  flex-grow: 1;\n  padding: 3rem;\n}\n\n.footer {\n  color: var(--color-muted);\n}\n\naside {\n  flex-basis: 14rem;\n  flex-shrink: 0;\n}\n\n.main-column {\n  flex-grow: 1;\n}\n\n// .today-series {\n//   display: grid;\n//   grid-template-columns: 1fr 2fr;  \n//   gap: 3rem;\n//   align-items: center;\n// }\n\n.card-episode {\n  position: relative;\n}\n\n.card-episode__image {\n  aspect-ratio: 300 / 170;  \n  transition: transform .2s ease-out, filter .3s ease-out, box-shadow .2s ease-out;\n  border: 2px solid var(--color-primary-300);\n  // box-shadow: var(--color-primary-200) 0 0;\n  background-position: top left;\n  background-color: var(--color-accent-200);\n  background-image: linear-gradient(125deg, var(--color-accent-400) 25%, transparent 25%);\n}\n\n.card-episode__poster {\n    max-width: 75px;\n    position: absolute;\n    bottom: -1rem;\n    right: 1rem;\n    z-index: 1;\n    border: 2px solid var(--color-primary-300);\n}\n\n// a:hover .card-episode__image {\n//   transform: translate(-7px, -7px);\n//   filter: brightness(1.25);\n//   box-shadow: var(--color-primary-200) 7px 7px;\n// }\n\n.series-poster__image {\n  aspect-ratio: 500 / 750;\n  border: 2px solid var(--color-primary-200);\n  background-position: top left;\n  background-color: var(--color-accent-200);\n  background-image: linear-gradient(125deg, var(--color-accent-400) 25%, transparent 25%);\n}\n\n@media screen and (min-width: 768px) {\n  .series-poster__image {\n    box-shadow: var(--color-primary-200) 7px 7px;\n  }\n}\n\n.episode-grid {\n    display: grid;\n    grid-template-columns: repeat(4, 1fr);\n    grid-template-rows: auto;\n    gap: 2rem;\n}\n\n.episode-grid__cell {\n  max-width: 300px;\n}\n\n/* .episode-grid__cell .view-all {\n  visibility: hidden;\n}\n\n.episode-grid__cell:hover .view-all {\n  visibility: visible;\n} */\n\n/* .series-vote {\n  position: absolute;\n  bottom: -3rem;\n  left: calc(50% - 2rem);\n  width: 4rem;\n  height: 4rem;\n  display: flex;\n  align-items: center;\n  justify-content: center;\n  border-radius: 50%;\n  color: var(--color-muted);\n  border: .25rem solid var(--color-primary-400);\n  background: var(--color-primary-100);\n}\n\n.series-vote span { \n  font-weight: 900;\n  color: var(--color-accent-light);\n  font-size: 1.5rem;\n} */\n\n\n.body-copy,\n.series-overview {\n  max-width: 75ch;\n}\n\n.fanart {\n  /* Bleed background into parent container */\n  margin-top: -3rem;\n  margin-right: -3rem;\n  margin-left: -3rem;\n  padding: 3rem 3rem 3rem 3rem;\n  background-position: top center;\n  background-attachment: fixed;\n  background-repeat: no-repeat;\n  background-size: cover;\n  background-blend-mode: multiply;\n  background-color: var(--color-accent-100);\n}\n\n@media screen and (min-width: 768px) {\n  .top-series-grid {\n    display: grid;\n    grid-template-columns: repeat(2, 1fr);\n    gap: 2rem;\n  }\n}\n\n.cards-grid {\n  display: grid;\n  grid-template-columns: repeat(3, 1fr);\n  gap: 1.5rem;\n  margin-bottom: 2rem;\n}\n\n@media screen and (min-width: 768px) {\n  .cards-grid {\n    grid-template-columns: repeat(6, 1fr);\n    gap: 2rem;\n  }\n}\n\ndialog {\n  background: transparent;\n  border: 0;\n  opacity: 0;\n  padding: 0;\n  margin: 0;\n  width: 100vw;\n  height: 100vh;\n  color: var(--color-body);\n  /* transition: transform .3s ease-out, opacity .3s ease-out;\n  transform: translate(0%, -5%); */\n  /* Reset browser defaults */\n  max-width: unset;\n  max-height: unset;\n  pointer-events: none;\n}\n\ndialog.in {\n  pointer-events: auto;\n  opacity: 1;\n  transition: opacity .3s ease-out;  \n}\n\ndialog.out {\n  opacity: 0;  \n  /* Wait 2s before disappear */\n  transition: opacity .3s ease-out 2s;\n}\n\n\n.dialog-body {\n  width: 30rem;\n  background: var(--color-primary-200);\n  padding: 2rem;\n  border-radius: 1rem;\n}\n\n.dialog-body--small {\n  width: 16rem;\n}\n\n// .dialog-body--toast {\n//   position: absolute;\n//   top: 1.5rem;\n//   right: 1.5rem;\n//   width: 16rem;\n//   z-index: 10;\n//   background: var(--color-primary-200);\n//   padding: 1rem;\n//   border-radius: .5rem;\n// }\n\ndialog:modal {\n  display: flex;\n  align-items: center;\n  justify-content: center;\n  opacity: 1;\n  pointer-events: auto;\n  /* transform: translate(0%, 0%); */\n}\n\ndialog::backdrop {\n  background: rgba(21, 29, 39, .75);\n}\n\n/* dialog button[name=\"close\"] {\n  position: absolute;\n  top: 0;\n  right: 0;\n  z-index: 1;\n} */\n\n/* Animations  */\n\n.anim-spin {\n  animation-name: spin;\n  animation-duration: 4s;\n  animation-iteration-count: infinite;\n  animation-timing-function: linear;\n}\n\n@keyframes spin {\n  from {\n    transform: rotate(0deg);\n  }\n\n  to {\n    transform: rotate(360deg);\n  }\n}\n\n/* A11y */\n\n.sr-only {\n  position: absolute;\n  white-space: nowrap;\n  width: 1px;\n  height: 1px;\n  overflow: hidden;\n  border: 0;\n  padding: 0;\n  clip: rect(0 0 0 0);\n  clip-path: inset(50%);\n  margin: -1px;\n}\n\n.skip-nav a {\n  position: absolute;\n  left: -9999px;\n  top: auto;\n  width: 1px;\n  height: 1px;\n  overflow: hidden;\n}\n\n.skip-nav a:focus {\n  position: static;\n  width: auto;\n  height: auto;\n}\n\n\n\n/*  \n  CSS mobile carousel, see: \n  https://css-tricks.com/can-get-pretty-far-making-slider-just-html-css/\n*/\n\n.mobile-carousel {\n  display: flex;\n  gap: 1.5rem;\n}\n\n@media screen and (max-width: 767.98px) {\n  .mobile-carousel {\n    display: flex;\n    scroll-behavior: smooth;\n    -webkit-overflow-scrolling: touch;\n    overflow-x: scroll;\n    scroll-snap-type: x mandatory;\n    margin: 0 -1rem 0 0;\n  }\n\n  .mobile-carousel>.mobile-carousel__item {\n    scroll-snap-align: start;\n    flex-shrink: 0;\n    /* 50% of the viewport width */\n    flex-basis: 50vw;\n  }\n\n  /* On mobile we want the swiping behavior but not the scroll bar */\n  .mobile-carousel::-webkit-scrollbar {\n    display: none;\n  }\n}\n\n@media screen and (min-width: 768px) {\n  .mobile-carousel {\n    gap: 2rem;\n    /* justify-content: space-between; */\n  }\n}\n\n/* Radio button group  */\n\n.radio-button-group {\n  display: flex;\n  border: 2px solid var(--color-primary-400);\n  color: var(--color-primary-light);\n  border-radius: .5rem;\n  // box-shadow: 0 0 5px 2px var(--color-primary), inset 0 0 2px 1px var(--color-primary);\n  font-size: var(--font-size-sm);\n  background-color: var(--color-primary-100);\n}\n\n.radio-button-group__label {\n  align-items: center;\n  display: inline-flex;\n  /* border-right: 1px solid var(--border-color); */\n  border-radius: .4rem;\n  padding: 0.5rem;\n  background-color: transparent;\n  color: var(--color-body);\n  cursor: pointer;\n}\n\n/* .radio-button-group__label:last-child {\n  border-right-color: transparent;\n} */\n\n.radio-button-group__label:has(input:checked) {\n  /* For selected radio */\n  background-color: var(--color-primary-300);\n  /* color: var(--color-primary-100); */\n}\n\n.radio-button-group__input {\n  position: absolute;\n  width: 1px;\n  height: 1px;\n  padding: 0;\n  overflow: hidden;\n  clip: rect(0, 0, 0, 0);\n  white-space: nowrap;\n  border: 0;  \n}\n\n/* Progress  */\n\nprogress {\n  accent-color: var(--color-accent-light);\n}\n\n/* Chart  */\n\n.chart {\n  max-width: 100%;\n}",
+        "// Lifted from Bootstrap 4\n\n@function breakpoint-infix($name, $breakpoints: $grid-breakpoints) {\n  @return if(breakpoint-min($name, $breakpoints)==null, \"\", \"-#{$name}\");\n}\n\n@function breakpoint-next($name, $breakpoints: $grid-breakpoints, $breakpoint-names: map-keys($breakpoints)) {\n  $n: index($breakpoint-names, $name);\n  @return if($n !=null and $n < length($breakpoint-names), nth($breakpoint-names, $n + 1), null);\n}\n\n@function breakpoint-min($name, $breakpoints: $grid-breakpoints) {\n  $min: map-get($breakpoints, $name);\n  @return if($min !=0, $min, null);\n}\n\n@function breakpoint-max($name, $breakpoints: $grid-breakpoints) {\n  $next: breakpoint-next($name, $breakpoints);\n  @return if($next, breakpoint-min($next, $breakpoints) - .02, null);\n}\n\n@mixin media-breakpoint-up($name, $breakpoints: $grid-breakpoints) {\n  $min: breakpoint-min($name, $breakpoints);\n\n  @if $min {\n    @media (min-width: $min) {\n      @content;\n    }\n  }\n\n  @else {\n    @content;\n  }\n}\n\n@mixin media-breakpoint-down($name, $breakpoints: $grid-breakpoints) {\n  $max: breakpoint-max($name, $breakpoints);\n\n  @if $max {\n    @media (max-width: $max) {\n      @content;\n    }\n  }\n\n  @else {\n    @content;\n  }\n}\n\n// Display\n\n@each $breakpoint in map-keys($grid-breakpoints) {\n  @include media-breakpoint-up($breakpoint) {\n    $infix: breakpoint-infix($breakpoint, $grid-breakpoints);\n\n    @each $value in $displays {\n      .d#{$infix}-#{$value} {\n        display: $value !important;\n      }\n    }\n  }\n}\n\n// Margin and padding\n\n@each $breakpoint in map-keys($grid-breakpoints) {\n  @include media-breakpoint-up($breakpoint) {\n    $infix: breakpoint-infix($breakpoint, $grid-breakpoints);\n\n    @each $prop, $abbrev in (margin: m, padding: p) {\n      @each $size, $length in $spacers {\n        .#{$abbrev}#{$infix}-#{$size} {\n          #{$prop}: $length !important;\n        }\n\n        .#{$abbrev}t#{$infix}-#{$size},\n        .#{$abbrev}y#{$infix}-#{$size} {\n          #{$prop}-top: $length !important;\n        }\n\n        .#{$abbrev}r#{$infix}-#{$size},\n        .#{$abbrev}x#{$infix}-#{$size} {\n          #{$prop}-right: $length !important;\n        }\n\n        .#{$abbrev}b#{$infix}-#{$size},\n        .#{$abbrev}y#{$infix}-#{$size} {\n          #{$prop}-bottom: $length !important;\n        }\n\n        .#{$abbrev}l#{$infix}-#{$size},\n        .#{$abbrev}x#{$infix}-#{$size} {\n          #{$prop}-left: $length !important;\n        }\n      }\n    }\n\n    // Negative margins (e.g., where `.mb-n1` is negative version of `.mb-1`)\n    @each $size, $length in $spacers {\n      @if $size !=0 {\n        .m#{$infix}-n#{$size} {\n          margin: -$length !important;\n        }\n\n        .mt#{$infix}-n#{$size},\n        .my#{$infix}-n#{$size} {\n          margin-top: -$length !important;\n        }\n\n        .mr#{$infix}-n#{$size},\n        .mx#{$infix}-n#{$size} {\n          margin-right: -$length !important;\n        }\n\n        .mb#{$infix}-n#{$size},\n        .my#{$infix}-n#{$size} {\n          margin-bottom: -$length !important;\n        }\n\n        .ml#{$infix}-n#{$size},\n        .mx#{$infix}-n#{$size} {\n          margin-left: -$length !important;\n        }\n      }\n    }\n\n    // Some special margin utils\n    .m#{$infix}-auto {\n      margin: auto !important;\n    }\n\n    .mt#{$infix}-auto,\n    .my#{$infix}-auto {\n      margin-top: auto !important;\n    }\n\n    .mr#{$infix}-auto,\n    .mx#{$infix}-auto {\n      margin-right: auto !important;\n    }\n\n    .mb#{$infix}-auto,\n    .my#{$infix}-auto {\n      margin-bottom: auto !important;\n    }\n\n    .ml#{$infix}-auto,\n    .mx#{$infix}-auto {\n      margin-left: auto !important;\n    }\n  }\n}\n\n// Flex variations\n\n@each $breakpoint in map-keys($grid-breakpoints) {\n  @include media-breakpoint-up($breakpoint) {\n    $infix: breakpoint-infix($breakpoint, $grid-breakpoints);\n\n    .flex#{$infix}-row {\n      flex-direction: row !important;\n    }\n\n    .flex#{$infix}-column {\n      flex-direction: column !important;\n    }\n\n    .flex#{$infix}-row-reverse {\n      flex-direction: row-reverse !important;\n    }\n\n    .flex#{$infix}-column-reverse {\n      flex-direction: column-reverse !important;\n    }\n\n    .flex#{$infix}-wrap {\n      flex-wrap: wrap !important;\n    }\n\n    .flex#{$infix}-nowrap {\n      flex-wrap: nowrap !important;\n    }\n\n    .flex#{$infix}-wrap-reverse {\n      flex-wrap: wrap-reverse !important;\n    }\n\n    .flex#{$infix}-fill {\n      flex: 1 1 auto !important;\n    }\n\n    .flex#{$infix}-grow-0 {\n      flex-grow: 0 !important;\n    }\n\n    .flex#{$infix}-grow-1 {\n      flex-grow: 1 !important;\n    }\n\n    .flex#{$infix}-shrink-0 {\n      flex-shrink: 0 !important;\n    }\n\n    .flex#{$infix}-shrink-1 {\n      flex-shrink: 1 !important;\n    }\n\n    .justify-content#{$infix}-start {\n      justify-content: flex-start !important;\n    }\n\n    .justify-content#{$infix}-end {\n      justify-content: flex-end !important;\n    }\n\n    .justify-content#{$infix}-center {\n      justify-content: center !important;\n    }\n\n    .justify-content#{$infix}-between {\n      justify-content: space-between !important;\n    }\n\n    .justify-content#{$infix}-around {\n      justify-content: space-around !important;\n    }\n\n    .align-items#{$infix}-start {\n      align-items: flex-start !important;\n    }\n\n    .align-items#{$infix}-end {\n      align-items: flex-end !important;\n    }\n\n    .align-items#{$infix}-center {\n      align-items: center !important;\n    }\n\n    .align-items#{$infix}-baseline {\n      align-items: baseline !important;\n    }\n\n    .align-items#{$infix}-stretch {\n      align-items: stretch !important;\n    }\n\n    .align-content#{$infix}-start {\n      align-content: flex-start !important;\n    }\n\n    .align-content#{$infix}-end {\n      align-content: flex-end !important;\n    }\n\n    .align-content#{$infix}-center {\n      align-content: center !important;\n    }\n\n    .align-content#{$infix}-between {\n      align-content: space-between !important;\n    }\n\n    .align-content#{$infix}-around {\n      align-content: space-around !important;\n    }\n\n    .align-content#{$infix}-stretch {\n      align-content: stretch !important;\n    }\n\n    .align-self#{$infix}-auto {\n      align-self: auto !important;\n    }\n\n    .align-self#{$infix}-start {\n      align-self: flex-start !important;\n    }\n\n    .align-self#{$infix}-end {\n      align-self: flex-end !important;\n    }\n\n    .align-self#{$infix}-center {\n      align-self: center !important;\n    }\n\n    .align-self#{$infix}-baseline {\n      align-self: baseline !important;\n    }\n\n    .align-self#{$infix}-stretch {\n      align-self: stretch !important;\n    }\n  }\n}\n\n// Typography \n\nsmall,\n.text-sm {\n  font-size: var(--font-size-sm) !important;\n}\n\n.text-regular {\n  font-size: var(--font-size-regular) !important;\n}\n\n.text-lg {\n  font-size: var(--font-size-lg) !important;\n}\n\n.text-xlg {\n  font-size: var(--font-size-xlg) !important;\n}\n\n.text-right {\n  text-align: right;\n}\n\n.text-left {\n  text-align: left;\n}\n\n.text-center {\n  text-align: center;\n}\n\n.text-muted {\n  color: var(--color-muted) !important;\n}\n\n.text-uppercase {\n  text-transform: uppercase;\n}\n\n.font-weight-normal {\n  font-weight: normal;\n}\n\n.font-weight-bold {\n  font-weight: bold;\n}\n\n.font-weight-semibold {\n  font-weight: 600;\n}\n\n.font-weight-black {\n  font-weight: 900;\n}\n\n.font-style-italic {\n  font-style: italic;\n}\n\n.font-small-caps {\n  font-variant: all-small-caps;\n}\n\n.line-height-1 {\n  line-height: 1;\n}\n\n.text-decoration-none {\n  text-decoration: none;\n}\n\n.text-break-all {\n  word-break: break-all;\n}\n\n.text-nowrap {\n  white-space: nowrap\n}\n\n// Misc helpers\n\n.position-relative {\n  position: relative;\n}\n\n.img-fluid {\n  max-width: 100%;\n  height: auto;\n}\n\n.zero {\n  margin: 0;\n  padding: 0;\n}\n\n.invisible {\n  visibility: hidden;\n}\n\n.h-100 {\n  height: 100%;\n}\n\n.w-100 {\n  width: 100%;\n}\n\n.d-grid {\n  display: grid;\n  grid-auto-flow: column;\n  grid-auto-columns: 1fr;\n}\n\n.rounded {\n  border-radius: .5rem;\n}\n\n// Border \n\n.border {\n  border: 1px solid var(--border-color);\n}\n\n.border-accent {\n  border: 1px solid var(--border-color-accent);\n}\n\n.border-top {\n  border-top: 1px solid var(--color-primary-300);\n}\n\n.border-bottom {\n  border-bottom: 1px solid var(--color-primary-300);\n}\n\n.border-right {\n  border-right: 1px solid var(--color-primary-300);\n}\n\n.border-left {\n  border-left: 1px solid var(--color-primary-300);\n}",
         "// An \"almost pure\" CSS carousel.\n//\n// See:\n//  * https://css-tricks.com/can-get-pretty-far-making-slider-just-html-css/\n//  * https://stackoverflow.com/a/58386348\n\n// Heights of the arrow icon element\n$image-carousel-nav-height: 24px !default;\n$image-carousel-item-width: 300px !default;\n// $outer-margin: 3rem;\n\n// Hide scrollbar but still allows to scroll horizontally\n// See https://stackoverflow.com/a/49278385\n@mixin hide-scrollbar-x() {\n  overflow-x: scroll;\n  /* Firefox */\n  scrollbar-width: none;\n  /* Internet Explorer 10+ */\n  -ms-overflow-style: none;\n\n  /* WebKit */\n  &::-webkit-scrollbar {\n    display: none;\n  }\n}\n\n.carousel {\n  position: relative;\n  margin: 0 -3rem 0 -3rem;\n}\n\n// -------------------\n// Slides\n// -------------------\n\n.carousel__items {\n  display: flex;\n  gap: 2rem;\n  width: 100%;\n\n  scroll-behavior: smooth;\n  -webkit-overflow-scrolling: touch;\n\n  // Horizontal scroll\n  overflow-x: scroll;\n  scroll-snap-type: x mandatory;\n  scroll-snap-align: start;\n\n  @include hide-scrollbar-x();\n}\n\n// Individual slide \n.carousel-item {\n  flex-shrink: 0;\n  max-width: $image-carousel-item-width;\n\n  &:first-child{\n    padding-left: 3rem;\n  }\n\n  &:last-child{\n    padding-right: 3rem;\n  }\n\n  // &.active {\n  //   background-color: lightblue;\n  // }  \n}\n\n// We want the swiping behavior but not the scroll bar\n.carousel__items::-webkit-scrollbar {\n  display: none;\n}\n\n// -------------------\n// Navigation\n// -------------------\n\n.carousel__next,\n.carousel__prev {\n  position: absolute;\n  top: calc(50% - #{$image-carousel-nav-height} / 2);\n  left: 0;\n  z-index: 1;\n}\n\n.carousel__next {\n  left: unset;\n  right: 0;\n}",
         "// --------------\n// Regular button\n// --------------\n\n.btn {\n    text-transform: uppercase;\n    font-size: var(--font-size-sm);\n    font-weight: bold;\n    letter-spacing: .05rem;\n    cursor: pointer;\n    padding: .75rem;\n    background: var(--color-background);\n    border: 2px solid var(--color-primary-400);\n    color: var(--color-primary-light);\n    border-radius: .5rem;\n    transition: border-color .1s ease-in;\n}\n\n.btn-small {\n    text-transform: uppercase;\n    font-size: var(--font-size-sm);\n    font-weight: bold;\n    cursor: pointer;\n    padding: .5rem;\n    background: var(--color-background);\n    border: 2px solid var(--color-primary-400);\n    color: var(--color-primary-light);\n    border-radius: .5rem;\n}\n\n.btn-small:hover,\n.btn:hover {\n    border-color: var(--anchor-color-hover);\n    color:  var(--anchor-color-hover);\n}\n\n.btn,\n.btn-small {\n    img {\n        filter: invert(77%) sepia(40%) saturate(250%) hue-rotate(164deg) brightness(100%) contrast(94%);\n    }\n    \n    &:hover img {\n        filter: invert(85%) sepia(46%) saturate(3508%) hue-rotate(287deg) brightness(112%) contrast(94%);\n    }\n}\n\n// --------------\n// Text button\n// --------------\n\n\n.btn-text {\n    padding: 0;\n    margin: 0;\n    background: transparent;\n    border: 0;\n    color: inherit;\n    font-size: inherit;\n    cursor: pointer;\n    transition: color .1s ease-in;\n    /* text-decoration: underline; */\n}\n\n.btn-text:hover {\n    color: var(--anchor-color-hover) !important;\n}\n\n// --------------\n// Icon button \n// --------------\n\n.btn-icon {\n    display: inline-flex;\n    align-items: center;\n    border: 0;\n    background: transparent;\n    cursor: pointer;\n    color: inherit;\n    transition: color .1s ease-in;\n    /* text-decoration: underline; */\n}",
         "select {\n    min-width: 20ch;\n    padding: .5rem 2rem .5rem .5rem;\n    border: 2px solid var(--color-primary-400);\n    color: var(--color-primary-light);\n    border-radius: .5rem;\n    // box-shadow: 0 0 5px 2px var(--color-primary), inset 0 0 2px 1px var(--color-primary);\n    /* transition: box-shadow .3s ease-in; */\n    font-size: var(--font-size-sm);\n    -webkit-appearance: none;\n    -moz-appearance: none;\n    appearance: none;\n    background: var(--color-background) url(\"data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='100' height='100' fill='%233d8fa9'><polygon points='0,0 100,0 50,50'/></svg>\") no-repeat;\n    background-size: 12px;\n    background-position: right .75em top 65%;\n    background-repeat: no-repeat;\n}\n\nselect:focus-visible {\n    outline: none;\n    // box-shadow: 0 0 5px 2px var(--color-accent), inset 0 0 2px 1px var(--color-accent);\n    border: 2px solid var(--anchor-color-hover);\n    color: var(--anchor-color-hover);\n}"
     ],
     "version": 3
 }
```

### Comparing `videobox-0.6.1/videobox/static/apple-touch-icon.png` & `videobox-0.7.0/videobox/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/videobox/static/default-poster.png` & `videobox-0.7.0/videobox/static/default-poster.png`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/videobox/static/default-still.png` & `videobox-0.7.0/videobox/static/default-still.png`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/videobox/static/favicon.png` & `videobox-0.7.0/videobox/static/favicon.png`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/videobox/static/favicon.svg` & `videobox-0.7.0/videobox/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/videobox/static/icon-grid-bold.svg` & `videobox-0.7.0/videobox/static/icon-grid-bold.svg`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/videobox/static/icon-grid.svg` & `videobox-0.7.0/videobox/static/icon-grid.svg`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/videobox/static/icon-heart-bold.svg` & `videobox-0.7.0/videobox/static/icon-heart-bold.svg`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/videobox/static/icon-heart-break-bold.svg` & `videobox-0.7.0/videobox/static/icon-heart-break-bold.svg`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/videobox/static/icon-heart-break.svg` & `videobox-0.7.0/videobox/static/icon-heart-break.svg`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/videobox/static/icon-heartbeat-bold.svg` & `videobox-0.7.0/videobox/static/icon-heartbeat-bold.svg`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/videobox/static/icon-heartbeat.svg` & `videobox-0.7.0/videobox/static/icon-heartbeat.svg`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/videobox/static/icon-magnet-bold.svg` & `videobox-0.7.0/videobox/static/icon-magnet-bold.svg`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/videobox/static/icon-magnet.svg` & `videobox-0.7.0/videobox/static/icon-magnet.svg`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/videobox/static/icon-update-bold.svg` & `videobox-0.7.0/videobox/static/icon-update-bold.svg`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/videobox/static/icon-update.svg` & `videobox-0.7.0/videobox/static/icon-update.svg`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/videobox/static/logo.svg` & `videobox-0.7.0/videobox/static/logo.svg`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/videobox/sync.py` & `videobox-0.7.0/videobox/sync.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,139 +1,161 @@
-from peewee import chunked, fn
 import time
+from urllib.parse import urlparse, parse_qs
 from datetime import datetime, timedelta, timezone
-from threading import Thread
+from threading import Thread, Event
+from peewee import chunked, fn
 from requests.exceptions import HTTPError, ReadTimeout
 from flask import current_app
 import videobox.api as api
 import videobox.models as models
-from videobox.models import Tag, SeriesTag, Series, SeriesIndex, Episode, Release, SyncLog
+import videobox.scraper as scraper
+from videobox.models import Tag, SeriesTag, Series, SeriesIndex, Episode, Release, Tracker, SyncLog
 
-# @@TODO check 
-# SQLite >3.32.0 has a limit of total 32766 max variables (SQLITE_MAX_VARIABLE_NUMBER)
-# https://stackoverflow.com/a/64419474 
-# https://stackoverflow.com/q/35616602
-INSERT_CHUNK_SIZE = 999 // 15   # Series class has the max numbes of fields 
 REQUEST_CHUNK_SIZE = 450        # Total URI must be < 4096
 TIMEOUT_BEFORE_RETRY = 5        # Seconds
+SYNC_INTERVAL = 60*60*2         # Seconds
+MIN_SYNC_INTERVAL = 60*15       # Seconds
+
+# The only sync worker tread
+sync_worker = None
 
 
 class SyncError(Exception):
     pass
 
+def default_progress_callback(message):
+    pass
+
+def default_done_callback(message, alert):
+    pass
 
 class SyncWorker(Thread):
 
-    def __init__(self, client_id, progress_callback=None, done_callback=None):
+    def __init__(self, client_id, progress_callback=default_progress_callback, done_callback=default_done_callback):
         super().__init__(name="Sync worker")
         self.app = current_app._get_current_object()
         self.client_id = client_id
         self.progress_callback = progress_callback
         self.done_callback = done_callback
+        # Start sync immediately at startup
+        self.interval = 0
+        self.abort_event = Event()        
+
+    def abort(self):
+        self.abort_event.set()
 
     def run(self):
-        last_log = models.get_last_log()
+        # Set up a recurring execution unless asked to abort
+        while not self.abort_event.is_set():
+            if self.interval:
+                self.app.logger.debug(f"Waiting for {self.interval}s before next sync...")
+            self.abort_event.wait(self.interval)
+            if self.abort_event.is_set():
+                self.app.logger.debug(f"Stopped {self.name} #{id(self)} thread")
+                return             
+            self._run_sync()            
+            # Schedule next sync
+            self.interval = SYNC_INTERVAL
+
+    def _run_sync(self):
+        last_log = models.get_last_successful_log()
         start_time = time.time()
 
         # Manually push the app context to make Flask
         #   logger to work on the separate thread
         with self.app.app_context():
-            current_log = SyncLog.create(description="Started import/sync")
+            if last_log:
+                sync_interval = datetime.now(timezone.utc) - last_log.timestamp.replace(tzinfo=timezone.utc) 
+                # timedelta.seconds upper bound is 3600*24
+                if sync_interval.days == 0 and sync_interval.seconds < MIN_SYNC_INTERVAL:
+                    self.app.logger.info(f"Sync request is below min. time interval of {MIN_SYNC_INTERVAL}s, ignored")
+                    return
+
+            current_log = SyncLog.create(description="Started sync")
 
             alert = ""
             try:
                 if last_log:
-                    alert, series_count, episode_count, release_count = self.update_library(
+                    alert, tags_count, series_count, episode_count, release_count = self.update_library(
                         last_log)
                 else:
-                    series_count, episode_count, release_count = self.import_library()
+                    tags_count, series_count, episode_count, release_count = self.import_library()
             except SyncError as ex:
                 self.update_log(current_log, status=models.SYNC_ERROR, description=str(ex))
-                if self.done_callback:
-                    self.done_callback(str(ex), alert)
+                self.done_callback(str(ex), alert)
                 return
 
             elapsed_time = time.time()-start_time
             if any([series_count, episode_count, release_count]):
-                description = f"Added/updated {series_count} series, {episode_count} episodes, and {release_count} torrents"
+                description = f"Added/updated {tags_count} tags, {series_count} series, {episode_count} episodes, and {release_count} torrents"
             else:
                 description = "No updates were found"
 
             # Mark import/sync successful
             self.update_log(current_log, status=models.SYNC_OK, description=description)
 
             self.app.logger.info(f"Finished in {elapsed_time:.1f}s: {description}")
 
-            if self.done_callback:
-                self.done_callback(description, alert)
+            self.done_callback(description, alert)
+
+            scraper.scrape_releases()
 
     def import_library(self):
-        series_count, episode_count, release_count = 0, 0, 0
-        instant = datetime.utcnow()
+        tags_count, series_count, episode_count, release_count = 0, 0, 0, 0
 
         self.app.logger.info("No local database found, starting full import")
-        
-        if self.progress_callback:
-            self.progress_callback("Importing all tags...", 0)
+
+        self.progress_callback("Importing all tags...")
 
         json = self.do_json_request(
             lambda: api.get_all_tags(self.client_id), retries=3)
         if json:
-            if self.progress_callback:
-                self.progress_callback("Saving tags to library...", 12.5)
-            self.save_tags(json)
+            self.progress_callback("Saving tags to library...")
+            tags_count = models.save_tags(self.app, json)
 
-        if self.progress_callback:
-            self.progress_callback("Importing all series...", 25)
+        self.progress_callback("Importing all series...")
 
         json = self.do_json_request(
             lambda: api.get_all_series(self.client_id))
         if json:
-            if self.progress_callback:
-                self.progress_callback("Saving series to library...", 37.5)
-            series_count = self.save_series(json, instant)
+            self.progress_callback("Saving series to library...")
+            series_count = models.save_series(self.app, json)
 
-        if self.progress_callback:
-            self.progress_callback("Importing all series tags...", 50)
+        self.progress_callback("Importing all series tags...")
 
         json = self.do_json_request(
             lambda: api.get_all_series_tags(self.client_id))
         if json:
-            self.save_series_tags(json)
+            models.save_series_tags(self.app, json)
 
-        if self.progress_callback:
-            self.progress_callback("Importing all episodes...", 62.5)
+        self.progress_callback("Importing all episodes...")
 
         json = self.do_json_request(
             lambda: api.get_all_episodes(self.client_id))
         if json:
-            if self.progress_callback:
-                self.progress_callback("Saving episodes to library...", 75)
-            episode_count = self.save_episodes(json, instant)
+            self.progress_callback("Saving episodes to library...")
+            episode_count = models.save_episodes(self.app, json)
 
-        if self.progress_callback:
-            self.progress_callback("Importing all torrents...", 87.5)
+        self.progress_callback("Importing all torrents...")
 
         json = self.do_json_request(
             lambda: api.get_all_releases(self.client_id))
         if json:
-            if self.progress_callback:
-                self.progress_callback("Saving torrents to library...", 87.5)            
-            release_count = self.save_releases(json, instant)
+            self.progress_callback("Saving torrents to library...")            
+            release_count = models.save_releases(self.app, json)
 
-        return series_count, episode_count, release_count
+        return tags_count, series_count, episode_count, release_count
 
     def update_library(self, last_log):
-        series_count, episode_count, release_count = 0, 0, 0
+        tags_count, series_count, episode_count, release_count = 0, 0, 0, 0
 
         self.app.logger.info("Last update done at {0} UTC, requesting updates since then".format(
             last_log.timestamp.isoformat()))
-        if self.progress_callback:
-            self.progress_callback("Getting updated series...")
-        # Ensure UTC tz
+        self.progress_callback("Getting updated series...")
+        # Ensure UTC timezone
         json = self.do_json_request(lambda: api.get_updated_series(
             self.client_id, last_log.timestamp.replace(tzinfo=timezone.utc)), retries=3)
 
         # Save alert from server, if any
         alert = json["alert"]
 
         tag_ids = json['tags']
@@ -159,227 +181,121 @@
         # Grab releases
         release_ids = json['releases']
         if release_ids:
             self.app.logger.debug(
                 "Got {0} releases, starting update".format(len(release_ids)))
             release_count = self.sync_releases(release_ids)
 
-        return alert, series_count, episode_count, release_count
-
-    def save_tags(self, response):
-        """
-        Insert new tags and attempt to update existing ones
-        """
-        count = 0
-        self.app.logger.debug("Saving tags to database...")
-        for batch in chunked(response, INSERT_CHUNK_SIZE):
-            count += (Tag.insert_many(batch)
-                      # Replace current tag with new data
-                      .on_conflict_replace()
-                      .as_rowcount()
-                      .execute())
-        return count
+        return alert, tags_count, series_count, episode_count, release_count
 
     def sync_tags(self, remote_ids):
         count = 0
 
         # Always request all remote ids so we have a chance to update existing series
         if remote_ids:
-            def callback(percent, remaining):
+            def callback(remaining):
                 self.progress_callback(
-                    f"Updating {remaining} tags...", 25 + percent)
+                    f"Updating {remaining} tags...")
 
             # Request all remote tags
             response = self.do_chunked_request(
                 api.get_tags_with_ids, remote_ids, callback)
             if response:
-                count = self.save_tags(response)
+                count = save_tags(self.app, response)
 
         return count
-    
+
     def sync_series(self, remote_ids):
-        instant = datetime.utcnow()
 
         # @@TODO
         # local_count = (Series.select(fn.Count(Series.id))
         #                .where((Series.id << remote_ids))
         #                .scalar())
         # missing_count = len(remote_ids) - local_count
         count, missing_count = 0, 0
 
         # Always request all remote ids so we have a chance to update existing series
         if remote_ids:
-            def callback(percent, remaining):
+            def callback(remaining):
                 self.progress_callback(
-                    f"Updating {remaining} series...", 25 + percent)
+                    f"Updating {remaining} series...")
 
-            self.app.logger.debug(
-                f"Found missing {missing_count} of {len(remote_ids)} series")
+            # self.app.logger.debug(
+            #     f"Found missing {missing_count} of {len(remote_ids)} series")
             # Request old and new series
             response = self.do_chunked_request(
                 api.get_series_with_ids, remote_ids, callback)
             if response:
-                count = self.save_series(response, instant)
+                count = models.save_series(self.app, response)
 
             #  Series tags
             response = self.do_chunked_request(
                 api.get_series_tags_for_ids, remote_ids, callback)
             if response:
-                self.save_series_tags(response)
+                models.save_series_tags(self.app, response)
 
         return count
 
-    def save_series(self, response, instant):
-        """
-        Insert new series and attempt to update existing ones
-        """
-        count = 0
-        self.app.logger.debug("Saving series to database...")
-        for batch in chunked(response, INSERT_CHUNK_SIZE):
-            count += (Series.insert_many(batch)
-                      .on_conflict(
-                conflict_target=[Series.id],
-                # Pass down values from insert clause
-                preserve=[Series.imdb_id, Series.name, Series.sort_name, Series.tagline, Series.overview, Series.network,
-                          Series.vote_average, Series.popularity, Series.poster_url, Series.fanart_url],
-                update={Series.last_updated_on: instant})
-                .as_rowcount()
-                .execute())
-            for series in batch:
-                content = ' '.join([series['network'], series['overview']]) 
-                # FTS5 insert_many cannot handle upserts
-                (SeriesIndex.insert({
-                    SeriesIndex.rowid: series['id'],                    
-                    SeriesIndex.name: series['name'],
-                    SeriesIndex.content: content,
-                })
-                    # Just replace name and content edits
-                    .on_conflict_replace()
-                    .execute())
-        SeriesIndex.optimize()
-        return count
 
-    def save_series_tags(self, response):
-        self.app.logger.debug("Saving series tags to database...")
-        for batch in chunked(response, INSERT_CHUNK_SIZE):
-            (SeriesTag.insert_many(batch)
-                # Ignore duplicate rows
-                .on_conflict_ignore()
-                .execute())
 
     def sync_episodes(self, remote_ids):
-        instant = datetime.utcnow()
 
         # local_ids = [e.id for e in Episode.select(Episode.id)]
         # new_ids = set(remote_ids) - set(local_ids)
         count, missing_count = 0, 0
 
         # Always request all remote ids so we have a chance to update existing episodes
         if remote_ids:
-            def callback(percent, remaining):
+            def callback(remaining):
                 self.progress_callback(
-                    f"Updating {remaining} episodes...", 50 + percent)
+                    f"Updating {remaining} episodes...")
 
-            self.app.logger.debug(
-                f"Found missing {missing_count} of {len(remote_ids)} episodes")
+            # self.app.logger.debug(
+            #     f"Found missing {missing_count} of {len(remote_ids)} episodes")
             # Request old and new episodes
             response = self.do_chunked_request(
                 api.get_episodes_with_ids, remote_ids, callback)
             if response:
-                count = self.save_episodes(response, instant)
-
-        return count
+                count = models.save_episodes(self.app, response)
 
-    def save_episodes(self, response, instant):
-        """
-        Insert new episodes and attempt to update existing ones
-        """
-        count = 0
-        self.app.logger.debug("Saving episodes to database...")
-        for batch in chunked(response, INSERT_CHUNK_SIZE):
-            # We need to cope with the unique constraint for (series, season, number)
-            #   index because we cannot rely on episodes id's,
-            #   they are often changed when TVDB users update them
-            count += (Episode
-                      .insert_many(batch)
-                      .on_conflict(
-                          conflict_target=[
-                              Episode.series, Episode.season, Episode.number],
-                          # Pass down values from insert clause
-                          preserve=[Episode.name, Episode.overview,
-                                    Episode.aired_on, Episode.thumbnail_url],
-                          update={Episode.last_updated_on: instant})
-                      .as_rowcount()
-                      .execute())
-            # EpisodeIndex.insert({
-            #     EpisodeIndex.rowid: episode_id,
-            #     EpisodeIndex.name: episode.name,
-            #     EpisodeIndex.overview: episode.overview}).execute()
-        #EpisodeIndex.optimize()            
         return count
 
     def sync_releases(self, remote_ids):
-        instant = datetime.utcnow()
 
         # local_ids = [r.id for r in Release.select(Release.id)]
         # new_ids = set(remote_ids) - set(local_ids)
         count, missing_count = 0, 0
 
         # Always request all remote ids so we have a chance to update existing releases
         if remote_ids:
-            def callback(percent, remaining):
+            def callback(remaining):
                 self.progress_callback(
-                    f"Updating {remaining} torrents...", 75 + percent)
+                    f"Updating {remaining} torrents...")
 
-            self.app.logger.debug(
-                f"Found missing {missing_count} of {len(remote_ids)} releases")
+            # self.app.logger.debug(
+            #     f"Found missing {missing_count} of {len(remote_ids)} releases")
             # Request old and new releases
             response = self.do_chunked_request(
                 api.get_releases_with_ids, remote_ids, callback)
             if response:
-                count = self.save_releases(response, instant)
+                count = models.save_releases(self.app, response)
 
         return count
 
-    def save_releases(self, response, instant):
-        """
-        Insert new releases and attempt to update existing ones
-        """
-        count = 0
-        self.app.logger.debug("Saving releases to database...")
-        for batch in chunked(response, INSERT_CHUNK_SIZE):
-            count += (Release
-                      .insert_many(batch)
-                      .on_conflict(
-                          conflict_target=[Release.id],
-                          # Pass down values from insert clause
-                          preserve=[Release.leechers, Release.seeders, Release.completed, Release.last_updated_on])
-                      .as_rowcount()
-                      .execute())
-        return count
-
-    def progress(self, value, min, max):
-        return self.scale_between(value, 0, 25, min, max)
-
-    def scale_between(self, value, min_allowed, max_allowed, min, max):
-        return (max_allowed - min_allowed) * (value - min) / (max - min) + min_allowed
-
     def update_log(self, log, status, description):
         log.status = status
         log.description = description
         log.save()
 
     def do_chunked_request(self, handler, ids, callback=None):
         result = []
         ids_count = len(ids)
         for index, chunked_ids in enumerate(chunked(ids, REQUEST_CHUNK_SIZE)):
             if callback:
-                percent = self.progress(index*REQUEST_CHUNK_SIZE, 0, ids_count)
-                callback(percent, ids_count -
-                         index*REQUEST_CHUNK_SIZE)
+                callback(ids_count - index*REQUEST_CHUNK_SIZE)
             self.app.logger.debug(
                 f"Requesting {index + 1} of {ids_count // REQUEST_CHUNK_SIZE + 1} chunks")
             json = self.do_json_request(
                 lambda: handler(self.client_id, chunked_ids))
             result.extend(json)
         return result
 
@@ -396,8 +312,8 @@
             except HTTPError as ex:
                 message = f'Server error {ex.response.status_code} occurred while handling the request, giving up'
                 self.app.logger.error(message)
                 raise SyncError(message)
             return response.json()
         # No more retries, giving up
         raise SyncError(
-            "Server timed out while handling the request. Please try again later.")
+            "Server timed out while handling the request")
```

### Comparing `videobox-0.6.1/videobox/templates/_episodes-grid.html` & `videobox-0.7.0/videobox/templates/_episodes-grid.html`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/videobox/templates/_episodes-list.html` & `videobox-0.7.0/videobox/templates/_episodes-list.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,13 @@
-{% macro air_date(value) %}
-  {% if value <= today %}
-    {{value | human_date}}
-  {% else %}
-    Will air {{value | human_date}}
-  {% endif %} 
-{% endmacro %}
+{% import "macros.html" as macros %}
 
 {% macro render_episode_row(episode) %}
   <tr id="e{{episode.id}}">
     <td class="text-center">{{episode.number}}.</td>
-    <td colspan="5" class="text-left"><span class="font-weight-bold">{{ episode.name }}</span>&ensp;<span class="text-muted text-sm">{{air_date(episode.aired_on)}}</span></td>
+    <td colspan="5" class="text-left"><span class="font-weight-bold">{{ episode.name }}</span>&ensp;<span class="text-muted text-sm">{{macros.air_date(episode.aired_on, today)}}</span></td>
   </tr>
   {{ render_release_row(episode.release) }}
 {% endmacro %}
 
 {% macro render_release_row(release) %}
   <tr>          
     <td class="text-center">&nbsp;</td>
@@ -54,22 +48,25 @@
             {% else %}
               {{ render_release_row(episode.release) }}
             {% endif %}
           {% endif %}
         {% else %}
           <!-- No releases -->
           <tr id="e{{episode.id}}">          
-            <td class="text-muted text-center">{{episode.number}}.</td>
-            <td class="text-muted font-style-italic"><span>{{ episode.name }}</span>&ensp;<span class="text-muted text-sm">{{air_date(episode.aired_on)}}</span></td>
+            <td class="text-muted text-center">{{episode.number}}.</td>            
+            <td class="text-muted"><span>{{ episode.name }}</span>&ensp;<span class="font-style-italic text-muted text-sm">{{macros.air_date(episode.aired_on, today)}}</span></td>
             <td class="text-muted text-center">—</td>
             <td class="text-muted text-center">—</td>
             <td class="text-muted text-right">—</td>
             <td class="text-muted text-right">—</td>
           </tr>
         {% endif %}            
       {% endfor %}
     </tbody>
   </table>  
  
 {% else %}  
-    <p class="border rounded p-3 font-style-italic" style="max-width: fit-content">⚠️ No releases found with <b>{{resolution}}p</b> resolution, try filtering for another value.</p>
+    <div class="d-flex align-items-center border rounded p-3 font-style-italic" style="max-width: fit-content">
+      <img src="{{ url_for('static', filename='icon-warning-bold.svg') }}" class="mr-2" width="16" height="16" alt="">
+      <span>No releases found with <b>{{resolution}}p</b> resolution, try filtering for another value.</span>
+    </div>
 {% endfor %}
```

#### html2text {}

```diff
@@ -1,22 +1,21 @@
-{% macro air_date(value) %} {% if value <= today %} {{value | human_date}} {%
-else %} Will air {{value | human_date}} {% endif %} {% endmacro %} {% macro
-render_episode_row(episode) %}
+{% import "macros.html" as macros %} {% macro render_episode_row(episode) %}
 {{episode.number}}.
-{{ episode.name }} {{air_date(episode.aired_on)}}
+{{ episode.name }} {{macros.air_date(episode.aired_on, today)}}
 {{ render_release_row(episode.release) }} {% endmacro %} {% macro
 render_release_row(release) %}
  
 {{release.name}}
 [/static/icon-magnet.svg]
 {{release.resolution if release.resolution else "?"}}
 {{release.size | filesizeformat}}
 {{release.seeders | torrent_health | safe if release.seeders else "â"}}
 {% endmacro %} {% for season, episodes in seasons_episodes %}
 ******** SSeeaassoonn {{{{sseeaassoonn}}}} {{{{ ""((CCuurrrreenntt))"" iiff lloooopp..iinnddeexx ==== 11 eellssee """" }}}} ********
-##                   EEppiissooddee                       DDoowwnn.. RReess.. SSiizzee SSeeeeddeerrss
-{{episode.number}}. {{ episode.name }} {{air_date â   â  â  â
-                    (episode.aired_on)}}
+##                   EEppiissooddee                            DDoowwnn.. RReess.. SSiizzee SSeeeeddeerrss
+                    {{ episode.name }} {
+{{episode.number}}. {macros.air_date(episode.aired_on, â   â  â  â
+                    today)}}
 {% else %}
-â ï¸ No releases found with {{{{rreessoolluuttiioonn}}}}pp resolution, try filtering for
-another value.
+No releases found with {{{{rreessoolluuttiioonn}}}}pp resolution, try filtering for another
+value.
 {% endfor %}
```

### Comparing `videobox-0.6.1/videobox/templates/_follow-button.html` & `videobox-0.7.0/videobox/templates/_follow-button.html`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/videobox/templates/_language-card-grid.html` & `videobox-0.7.0/videobox/templates/_language-card-grid.html`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/videobox/templates/_release_detail.html` & `videobox-0.7.0/videobox/templates/_release_detail.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 <div class="dialog-body">
     <form method="dialog">
         <h2 class="text-lg mb-3 text-break-all">{{release.name}}
         </h2>
-        <p class="py-3 d-flex align-items-center border-top border-bottom" style="gap: .25rem">
-            <img class="icon" width="20" height="20" src="/static/icon-magnet.svg"><a download href="{{release.magnet_uri}}">Download torrent with magnet link</a>
+        {% set languages = release.languages %}
+        {% if languages %}
+            <div class="d-flex p-2 mb-3 border-accent align-items-center rounded">
+                <img src="/static/icon-info.svg" class="icon mr-2" alt="Information" width="20" height="20">
+                <div class="text-sm">
+                    It looks like this episode contains subtitles or has been dubbed in: {{languages|join(", ")}}
+                </div>
+            </div>
+        {% endif %}
+        <p class="py-3 d-flex align-items-center border-top border-bottom">
+            <img class="icon mr-2" width="20" height="20" src="/static/icon-magnet.svg"><a download href="{{release.magnet_uri}}">Download torrent with magnet link</a>
         </p>
         <dl class="mb-4">
             <dt>
                 Added
             </dt>
             <dd>
                 {{release.added_on | human_date_time}} UTC
             </dd>
+            <dt>Size</dt>
+            <dd>
+                {{release.size | filesizeformat}} ({{release.size}} bytes)
+            </dd>
             <dt>
                 Info hash
             </dt>
             <dd class="">
                 <code>{{release.info_hash}}</code>
             </dd>
-            <dt>Size</dt>
-            <dd>
-                {{release.size | filesizeformat}} ({{release.size}} bytes)
-            </dd>
             <dt>
                 Swarm
             </dt>
             <dd>
                 {{"{:,}".format(release.seeders)}} seeders, {{"{:,}".format(release.leechers)}} leechers, and {{"{:,}".format(release.completed)}} downloads.<br> 
-                Last checked {{release.last_updated_on|datetime_since(utc_now)}}
+                Last checked {{release.last_updated_on|datetime_since(utc_now)}}.
             </dd>
         </dl>
         <button class="btn" type="submit">Close</button>        
     </form>
 </div>
```

### Comparing `videobox-0.6.1/videobox/templates/_tag-card-grid.html` & `videobox-0.7.0/videobox/templates/_tag-card-grid.html`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/videobox/templates/base.html` & `videobox-0.7.0/videobox/templates/base.html`

 * *Files 20% similar despite different names*

```diff
@@ -8,33 +8,27 @@
   {% endblock %}
   {% include "_meta.html" %}
 </head>
 
 {% block body %}
 <body>
   <header class="header">
-      <div class="header__branding"><a class="btn-icon" aria-label="Videobox Home"  data-balloon-pos="right" href="{{ url_for('main.home') }}"><img width="30" height="30" class="btn-logo img-fluid" aria-hidden="true" src="/static/logo.svg" alt=""></a></div>
+      <div class="header__branding"><a class="btn-icon" aria-label="Home"  data-balloon-pos="right" href="{{ url_for('main.home') }}"><img width="30" height="30" class="btn-logo img-fluid" aria-hidden="true" src="/static/logo.svg" alt=""></a></div>
       <button class="btn-icon" aria-label="Search" data-balloon-pos="right" type="button" onclick="Videobox.openSearchDialog(event)">
         <img width="30" height="30" aria-hidden="true" src="/static/icon-search.svg" alt="">
       </button>
       <a class="btn-icon text-decoration-none" aria-label="Tags" data-balloon-pos="right" href="{{ url_for('main.tag') }}"><img width="30" height="30" aria-hidden="true" src="/static/icon-tag.svg" alt=""></a>
-      <a class="btn-icon text-decoration-none" aria-label="Followed Series" data-balloon-pos="right" href="{{ url_for('main.following') }}"><img width="30" height="30" aria-hidden="true" src="/static/icon-heartbeat.svg" alt=""></a>
-      <button class="btn-icon" aria-label="Update Library" data-balloon-pos="right" type="button" onclick="Videobox.update()">
-        <img width="30" height="30" aria-hidden="true" src="/static/icon-update.svg" alt="">
-      </button>
+      <a class="btn-icon text-decoration-none" aria-label="Series Updates" data-balloon-pos="right" href="{{ url_for('main.following') }}"><img width="30" height="30" aria-hidden="true" src="/static/icon-heartbeat.svg" alt=""></a>
   </header>
   {% block content %}{% endblock %}
   <dialog id="search-dialog">
     <form class="search-query" action="/search" oninput="Videobox.suggest()" method="GET">
       <label class="sr-only" for="search-query">Search Series</label>
       <input list="search-suggestions" required autocomplete="off" spellcheck="false" id="search-query" type="text" size="20" maxlength="100" name="query" value="{{search_query}}" placeholder="Type a series name or keyword" />
       <button type="submit"><img class="icon" src="/static/icon-search.svg" alt=""></button>
     </form>
     <datalist id="search-suggestions"></datalist>
   </dialog>
-  <dialog id="update-dialog">
-    {% include "_update-dialog.html" %}
-  </dialog>  
   <dialog id="release-dialog"></dialog>  
 </body>
 {% endblock %}
 </html>
```

#### html2text {}

```diff
@@ -1,7 +1,6 @@
 {% block title %}
 {% endblock %} {% include "_meta.html" %}
 {% block body %}
 {% block content %}{% endblock %}
 Search Series[{{search_query}}    ]
-{% include "_update-dialog.html" %}
 {% endblock %}
```

### Comparing `videobox-0.6.1/videobox/templates/first-import.html` & `videobox-0.7.0/videobox/templates/first-import.html`

 * *Files 23% similar despite different names*

```diff
@@ -6,22 +6,21 @@
     <title>Videobox</title>
     {% endblock %}
     {% include "_meta.html" %}
 </head>
 
 {% block body %}
 
-<body class="d-flex flex-column align-items-center justify-content-center" style="height: 100vh;">    
-    <p class="text-lg mb-4">
-        No series found, please update your library.
-    </p>
-    <button class="btn d-flex align-items-center" type="button" onclick="Videobox.update()">
-        <img class="mr-2" width="30" height="30" aria-hidden="true" src="/static/icon-update.svg" alt="">Update Now
-    </button>
-    <dialog id="update-dialog">
-        {% include "_update-dialog.html" %}
-    </dialog>
+<body class="d-flex flex-column align-items-center justify-content-center" style="height: 100vh; gap: 2rem">    
+    <div class="d-flex flex-column align-items-center" style="gap: 1rem" id="update-dialog">
+        {% include "_update-progress.html" %}
+    </div>    
+    <script>
+        window.addEventListener("DOMContentLoaded", (event) => {
+            Videobox.sync()
+        })
+    </script>
 </body>
 
 {% endblock %}
 
 </html>
```

#### html2text {}

```diff
@@ -1,6 +1,5 @@
 {% block title %}
 {% endblock %} {% include "_meta.html" %}
 {% block body %}
-No series found, please update your library.
-Update Now {% include "_update-dialog.html" %}
+{% include "_update-progress.html" %}
 {% endblock %}
```

### Comparing `videobox-0.6.1/videobox/templates/following.html` & `videobox-0.7.0/videobox/templates/following.html`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/videobox/templates/home.html` & `videobox-0.7.0/videobox/templates/home.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 {% import "macros.html" as macros %}
 {% extends "base.html" %}
 
 {% block content %} 
     <main id="main">
         <!--  style="background-image: url({{ today_series.fanart_url if today_series and today_series.fanart_url else '' }});" -->
         <section>
-            <div class="mb-5">
-                <h1 class="text-xlg font-weight-black mb-2">Videobox</h1>
-                <p class="text-muted">
-                    Tracking <strong>{{ "{:,}".format(total_series) }}</strong> series and
-                    <strong>{{ "{:,}".format(total_releases) }}</strong> torrents • {% if last_sync %}Updated {{last_sync.timestamp|datetime_since(utc_now) }}&ensp;<a href="{{ url_for('main.update_history') }}">See history</a>{% endif %}
-                </p>
-            </div>
+            <h1 class="text-xlg font-weight-black mb-5">Videobox</h1>
 
             {% if server_alert %}
                 <p class="border rounded p-3 mb-5" style="max-width: fit-content">
                     ⚠️ {{server_alert}}
                 </p>
             {% endif %}
     
@@ -37,15 +31,15 @@
                                             <img class="card-episode__poster img-fluid rounded" loading="lazy" src="{{ s.poster }}" width="340" height="500" alt="Poster for {{ s.name }}" />                                            
                                         </a>
                                     </div>
                                     <div>
                                         <h2 class="text-sm text-muted text-uppercase mb-2">{{s.episode.season_episode_id}}</h2>
                                         <h3 class="text-regular">
                                             <a class="" href="{{ url_for('main.series_detail', series_id=s.id, view='list', _anchor=episode_hash) }}">
-                                                {{ s.episode.name }} 
+                                                {{ s.episode.name }}<!-- {{ s.total_completed }} -->
                                             </a>
                                         </h3>                                    
                                     </div>
                                 </div>
                             {% endfor %}
                         </div>
                     </div>
@@ -93,22 +87,33 @@
                 </div>
                     {{ macros.render_series_timeline(followed_series) }}
             </section>
             
             <hr class="my-5">
         {% endif %}
 
-        <!-- LEGAL -->
-
-        <p class="text-muted mb-2">
-            <small><strong>This is Videobox {{version}}</strong></small>
-        </p>
-
-        <p class="text-muted body-copy">
-            <small>Videobox doesn’t host any copyrighted content. TV series information and
-              images are provided by <a rel="noreferrer" href="https://www.themoviedb.org/">The Movie DB</a>, but we are not endorsed or
-              certified by The Movie DB or its affiliates.</small>
-        </p>
+        <footer>
+            <p class="text-muted mb-2">
+                <small><strong>This is Videobox {{version}}</strong></small>
+            </p>
+    
+            <p class="text-muted mb-2">
+                <small>Tracking {{ "{:,}".format(total_series) }} series and
+                {{ "{:,}".format(total_releases) }} torrents&emsp;
+                {% if last_sync and last_sync.status == "K" %}
+                    <img style="vertical-align: middle" class="mr-1" width="16" height="16" src="{{ url_for('static', filename='icon-check-bold.svg') }}"><a href="{{ url_for('main.system_status') }}">Library is up to date</a>
+                {% else %}
+                    <img style="vertical-align: middle" class="mr-1" width="16" height="16" src="{{ url_for('static', filename='icon-warning-bold.svg') }}"><a href="{{ url_for('main.system_status') }}">There were errors updating library</a>
+                {% endif %}
+                </small>
+            </p>
+            
+            <p class="text-muted body-copy">
+                <small>Videobox doesn’t host any copyrighted content. TV series information and
+                  images are provided by <a rel="noreferrer" href="https://www.themoviedb.org/">The Movie DB</a>, but we are not endorsed or
+                  certified by The Movie DB or its affiliates.</small>
+            </p>
+        </footer>
     </main>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,13 +1,10 @@
 {% import "macros.html" as macros %} {% extends "base.html" %} {% block content
 %}
 ************ VViiddeeoobbooxx ************
-Tracking {{{{ ""{{::,,}}""..ffoorrmmaatt((ttoottaall__sseerriieess)) }}}} series and {{{{ ""{{::,,}}""..ffoorrmmaatt
-((ttoottaall__rreelleeaasseess)) }}}} torrents â¢ {% if last_sync %}Updated {
-{last_sync.timestamp|datetime_since(utc_now) }} _S_e_e_ _h_i_s_t_o_r_y{% endif %}
 {% if server_alert %}
 â ï¸ {{server_alert}}
 {% endif %} {% if today_series %}
 ********** TTooddaayy?â??ss ttoopp eeppiissooddeess **********
 {% for s in today_series %}
 {% set episode_hash = 'e' ~ s.episode.id %}
 _[_S_t_i_l_l_ _f_o_r_ _e_p_i_s_o_d_e_ _{_{_s_._e_p_i_s_o_d_e_._s_e_a_s_o_n___e_p_i_s_o_d_e___i_d_}_}_]_[_P_o_s_t_e_r_ _f_o_r_ _{_{_ _s_._n_a_m_e_ _}_}_]
@@ -27,11 +24,16 @@
 {% if followed_series %}
 ********** FFoolllloowweedd sseerriieess **********
 _V_i_e_w_ _a_l_l
 {{ macros.render_series_timeline(followed_series) }}
 ===============================================================================
 {% endif %}
 TThhiiss iiss VViiddeeoobbooxx {{{{vveerrssiioonn}}}}
+Tracking {{ "{:,}".format(total_series) }} series and {{ "{:,}".format
+(total_releases) }} torrents  {% if last_sync and last_sync.status == "K" %} [{
+{ url_for('static', filename='icon-check-bold.svg') }}]_L_i_b_r_a_r_y_ _i_s_ _u_p_ _t_o_ _d_a_t_e {%
+else %} [{{ url_for('static', filename='icon-warning-bold.svg') }}]_T_h_e_r_e_ _w_e_r_e
+_e_r_r_o_r_s_ _u_p_d_a_t_i_n_g_ _l_i_b_r_a_r_y {% endif %}
 Videobox doesnât host any copyrighted content. TV series information and
 images are provided by _T_h_e_ _M_o_v_i_e_ _D_B, but we are not endorsed or certified by
 The Movie DB or its affiliates.
 {% endblock %}
```

### Comparing `videobox-0.6.1/videobox/templates/log.html` & `videobox-0.7.0/videobox/templates/tags.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,29 @@
+{% import "macros.html" as macros %}
 {% extends "base.html" %}
 
-{% macro row_status(value) %}
-  {% if value == 'K' %}
-    ✅
-  {% else %}
-    ❌
-  {% endif %} 
-{% endmacro %}
-
+{% block title %}
+  <title>Tags • Videobox</title>
+{% endblock %}
 
 {% block content %}
-<main id="main">
-    <div class="mb-5">
-        <h1 class="text-xlg font-weight-black mb-2">Update History</h1>
-        <p class="text-muted">Results for the last {{max_log_rows}} library updates.</p>        
-    </div>
-
-    {% if log_rows %}
-    <table class="report w-100">
-        <thead>
-            <tr>
-                <th>&nbsp;              
-                </th>
-                <th class="text-left">Date                    
-                </th>
-                <th class="text-left">Result
-                </th>
-            </tr>
-        </thead>
-        <tbody>
-            {% for row in log_rows %}
-            <tr>
-                <td class="text-center">{{row_status(row.status)}}</td>
-                <td>{{row.timestamp|human_date_time}}</td>
-                <td>{{row.description}}</td>
-            </tr>
-            {% endfor %}
-        </tbody>
-    </table>
-
-    {% endif %}
-</main>
-{% endblock %}
+  <main id="main">
+    <h1 class="text-xlg font-weight-black mb-5">Tags</h1>
+    {% for (tag_slug, tag_name), series in tags_series %}
+      <section class="mb-4 pb-4 border-bottom">
+          <div class="d-flex align-items-center mb-3">
+            <h2 class="text-lg font-weight-black">{{tag_name}}</h2>
+            <a class="ml-auto" href="{{ url_for('main.tag_detail', slug=tag_slug) }}"><small>View all</small></a>
+          </div>
+          <div class="mobile-carousel">
+              {% for s in (series|islice(8)) %}
+                  <div class="mobile-carousel__item">
+                    {{ macros.render_series_card(s) }}
+                  </div>
+              {% endfor %}
+          </div>
+      </section>
+    {% endfor %}  
+  </main>                            
+{% endblock %}
+     
+
```

#### html2text {}

```diff
@@ -1,9 +1,11 @@
-{% extends "base.html" %} {% macro row_status(value) %} {% if value == 'K' %}
-â {% else %} â {% endif %} {% endmacro %} {% block content %}
-************ UUppddaattee HHiissttoorryy ************
-Results for the last {{max_log_rows}} library updates.
-{% if log_rows %}
-?                           DDaattee                             RReessuulltt
-{{row_status(row.status)}} {                                {{row.description}}
-                           {row.timestamp|human_date_time}}
-{% endif %} {% endblock %}
+{% import "macros.html" as macros %} {% extends "base.html" %} {% block title
+%}
+{% endblock %} {% block content %}
+************ TTaaggss ************
+{% for (tag_slug, tag_name), series in tags_series %}
+********** {{{{ttaagg__nnaammee}}}} **********
+_V_i_e_w_ _a_l_l
+{% for s in (series|islice(8)) %}
+{{ macros.render_series_card(s) }}
+{% endfor %}
+{% endfor %} {% endblock %}
```

### Comparing `videobox-0.6.1/videobox/templates/macros.html` & `videobox-0.7.0/videobox/templates/macros.html`

 * *Files 24% similar despite different names*

```diff
@@ -41,13 +41,17 @@
                 loading="lazy" alt="Poster for {{series.name}}" />
             <h3 class="card-series__name my-1 font-weight-normal text-sm text-center">{{series.name}}</h3>
         </a>
     </div>
 {% endmacro %}
 
 {% macro air_date(value, today) %}
-  {% if value <= today %}
-    {{value | human_date}}
-  {% else %}
-    Will air {{value | human_date}}
-  {% endif %} 
+    {% if value %}
+        {% if value <= today %}
+            {{value | human_date}}
+        {% else %}
+            Will air {{value | human_date}}
+        {% endif %} 
+    {% else %}
+        &nbsp;
+    {% endif %}
 {% endmacro %}
```

#### html2text {}

```diff
@@ -9,10 +9,10 @@
 {{ "{:,}".format(s.release_count)}} new torrents
 {% endfor %}
 {% if not loop.last %}
 ===============================================================================
 {% endif %} {% endfor %} {% endmacro %} {% macro render_series_card(series) %}
 _[_P_o_s_t_e_r_ _f_o_r_ _{_{_s_e_r_i_e_s_._n_a_m_e_}_}_]
 _**_**_**_**_ _{{_{{_ss_ee_rr_ii_ee_ss_.._nn_aa_mm_ee_}}_}}_ _**_**_**_**
-{% endmacro %} {% macro air_date(value, today) %} {% if value <= today %} {
-{value | human_date}} {% else %} Will air {{value | human_date}} {% endif %} {%
-endmacro %}
+{% endmacro %} {% macro air_date(value, today) %} {% if value %} {% if value <=
+today %} {{value | human_date}} {% else %} Will air {{value | human_date}} {%
+endif %} {% else %}   {% endif %} {% endmacro %}
```

### Comparing `videobox-0.6.1/videobox/templates/search_results.html` & `videobox-0.7.0/videobox/templates/search_results.html`

 * *Files identical despite different names*

### Comparing `videobox-0.6.1/videobox/templates/series_detail.html` & `videobox-0.7.0/videobox/templates/series_detail.html`

 * *Files 11% similar despite different names*

```diff
@@ -2,26 +2,22 @@
 
 {% block title %}
 <title>{{series.name}} • Videobox</title>
 {% endblock %}
 
 {% block content %}
 <main id="main">
-  <section class="d-md-flex fanart border-bottom mb-5" style="gap: 3.5rem; background-image: url({{series.fanart_url}})">
+  <section class="d-md-flex align-items-center fanart border-bottom mb-5" style="gap: 3.5rem; background-image: url({{series.fanart_url}})">
     <aside class="d-none d-md-block">
       <!-- Desktop only  -->
-      <div class="series-poster mb-3">
+      <div class="series-poster">
         <img class="series-poster__image img-fluid rounded" loading="lazy"
           src="{{ series.poster }}" width="680" height="1000"
           alt="Poster for {{ series.name }}" />
       </div>
-      <!-- Toggle follow -->
-      <div class="d-flex justify-content-center">
-        {% include "_follow-button.html" %}
-      </div>
     </aside>
     <div class="main-column">
       <h2 class="text-sm text-muted text-uppercase mb-2">{{series.network|networks}}</h2>
       <h1 class="text-xlg font-weight-black mb-4">{{series.name}}
       </h1>
       <div class="d-flex align-items-top mb-4" style="gap: 1rem">
         {% if series.vote_average|int > 0 %}
@@ -53,26 +49,30 @@
       <!-- Mobile only -->
       <div class="series-poster d-md-none mr-3" style="float: left">
         <img class="series-poster__image img-fluid rounded" loading="lazy"
           src="{{ series.poster }}" width="120"
           height="250" alt="Poster for {{ series.name }}" />
       </div>
 
-      {% if series.overview %}
-      <p class="series-overview mb-4">{{series.overview}}
-      </p>
-      {% endif %}
-      <div class="text-muted">
+      <p class="series-overview mb-4">
+        {% if series.overview %}
+          {{series.overview}}<br>
+        {% endif%}   
         <a target="_blank" title="Find out more on The Movie DB" rel="noreferrer"
           href="{{series.tmdb_url}}">&#x2197;&nbsp;TMDB</a>
         {% if series.imdb_id %}
         &ensp;<a target="_blank" title="Find out more on IMDb" rel="noreferrer"
           href="{{series.imdb_url}}">&#x2197;&nbsp;IMDb</a>
-        {% endif%}
-      </div>
+        {% endif%}        
+      </p>
+
+      <!-- Toggle follow -->
+      <div class="">
+        {% include "_follow-button.html" %}
+      </div>      
     </div> <!-- /main-column -->
   </section>
 
   <form id="filter" class="d-flex align-items-end mb-5" onchange="this.submit()" action="{{ url_for('main.series_detail', series_id=series.id) }}" style="gap: 1rem" method="GET">
 
     <fieldset class="pr-3">
       <legend class="mb-2">Video Resolution</legend>
@@ -88,14 +88,28 @@
         {% for key, label in size_options.items() %}
         <option value="{{key}}" {{ "selected" if size==key else "" }}>{{label}}</option>
         {% endfor %}
       </select>
     </fieldset>
     <fieldset class="ml-auto">
       <div class="radio-button-group">
+        <label class="radio-button-group__label"><img aria-hidden="true" class="icon" src="/static/icon-sort-asc.svg"
+            width="20" height="20" alt="">
+          <input class="radio-button-group__input" type="radio" {{ 'checked' if episode_sorting=='asc' else '' }}
+            name="episode" value="asc">
+        </label>
+        <label class="radio-button-group__label"><img aria-hidden="true" class="icon" src="/static/icon-sort-desc.svg"
+          width="20" height="20" alt="">
+          <input class="radio-button-group__input" type="radio" {{ 'checked' if episode_sorting=='desc' else '' }}
+            name="episode" value="desc">
+        </label>
+      </div>
+    </fieldset>    
+    <fieldset class="">
+      <div class="radio-button-group">
         <label class="radio-button-group__label"><img aria-hidden="true" class="icon" src="/static/icon-grid.svg"
             width="20" height="20" alt="">
           <input class="radio-button-group__input" type="radio" {{ 'checked' if view_layout=='grid' else '' }}
             name="view" value="grid">
         </label>
         <label class="radio-button-group__label"><img aria-hidden="true" class="icon" src="/static/icon-list.svg"
           width="20" height="20" alt="">
```

#### html2text {}

```diff
@@ -1,31 +1,31 @@
 {% extends "base.html" %} {% block title %}
 {% endblock %} {% block content %}
 [Poster for {{ series.name }}]
-{% include "_follow-button.html" %}
 ********** {{{{sseerriieess..nneettwwoorrkk||nneettwwoorrkkss}}}} **********
 ************ {{{{sseerriieess..nnaammee}}}} ************
 {% if series.vote_average|int > 0 %}
 ******** SSccoorree ********
 {{(series.vote_average*10)|int}}%
 {% endif %}
 ******** LLaanngguuaaggee ********
 _{_{_ _s_e_r_i_e_s_._l_a_n_g_u_a_g_e_|_l_a_n_g_ _}_}
 {% if series_tags %}
 ******** GGeennrreess ********
 {% for tag in series_tags %} _{_{_t_a_g_._n_a_m_e_}_} {% endfor %}
 {% endif %}
 [Poster for {{ series.name }}]
-{% if series.overview %}
-{{series.overview}}
-{% endif %}
-_↗_ _T_M_D_B {% if series.imdb_id %}  _↗_ _I_M_D_b {% endif%}
+{% if series.overview %} {{series.overview}}
+{% endif%} _↗_ _T_M_D_B {% if series.imdb_id %}  _↗_ _I_M_D_b {% endif%}
+{% include "_follow-button.html" %}
 {% for key, label in resolution_options.items() %}
 { "selected" if resolution==key else "" }}>{{label}}
 {% endfor %}
 {% for key, label in size_options.items() %}
 { "selected" if size==key else "" }}>{{label}}
 {% endfor %}
+{ 'checked' if episode_sorting=='asc' else '' }} name="episode" value="asc">
+{ 'checked' if episode_sorting=='desc' else '' }} name="episode" value="desc">
 { 'checked' if view_layout=='grid' else '' }} name="view" value="grid">
 { 'checked' if view_layout=='list' else '' }} name="view" value="list">
 {% if view_layout == 'list' %} {% include "_episodes-list.html" %} {% else %}
 {% include "_episodes-grid.html" %} {% endif %} {% endblock %}
```

### Comparing `videobox-0.6.1/videobox/trackers.txt` & `videobox-0.7.0/videobox/trackers.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1 +1 @@
-http://1337.abcvg.info:80/announce,http://aboutbeautifulgallopinghorsesinthegreenpasture.online:80/announce,http://bt.okmp3.ru:2710/announce,http://bvarf.tracker.sh:2086/announce,http://ipv6.rer.lol:6969/announce,http://nyaa.tracker.wf:7777/announce,http://open.acgnxtracker.com:80/announce,http://share.camoe.cn:8080/announce,http://t.acg.rip:6699/announce,http://t.nyaatracker.com:80/announce,http://tinfoil.space:6969/announce,http://tk.greedland.net:80/announce,http://torrentsmd.com:8080/announce,http://tracker.electro-torrent.pl:80/announce,http://tracker.files.fm:6969/announce,http://tracker.gbitt.info:80/announce,http://tracker.ipv6tracker.ru:80/announce,http://tracker.renfei.net:8080/announce,http://tracker.tfile.co:80/announce,http://www.all4nothin.net:80/announce.php,http://www.wareztorrent.com:80/announce,https://t1.hloli.org:443/announce,https://tr.abir.ga:443/announce,https://tr.burnabyhighstar.com:443/announce,https://tracker.gbitt.info:443/announce,https://tracker.kuroy.me:443/announce,https://tracker.loligirl.cn:443/announce,https://tracker.tamersunion.org:443/announce,https://tracker.yemekyedim.com:443/announce,https://tracker1.520.jp:443/announce,https://trackers.mlsub.net:443/announce,https://www.peckservers.com:9443/announce,udp://aarsen.me:6969/announce,udp://amigacity.xyz:6969/announce,udp://bt1.archive.org:6969/announce,udp://d40969.acod.regrucolo.ru:6969/announce,udp://ec2-18-191-163-220.us-east-2.compute.amazonaws.com:6969/announce,udp://epider.me:6969/announce,udp://evan.im:6969/announce,udp://exodus.desync.com:6969/announce,udp://ipv6.fuuuuuck.com:6969/announce,udp://martin-gebhardt.eu:25/announce,udp://moonburrow.club:6969/announce,udp://movies.zsw.ca:6969/announce,udp://ns1.monolithindustries.com:6969/announce,udp://odd-hd.fr:6969/announce,udp://oh.fuuuuuck.com:6969/announce,udp://open.demonii.com:1337/announce,udp://open.demonoid.ch:6969/announce,udp://open.stealth.si:80/announce,udp://open.tracker.ink:6969/announce,udp://opentor.org:2710/announce,udp://opentracker.io:6969/announce,udp://p4p.arenabg.com:1337/announce,udp://retracker.lanta.me:2710/announce,udp://thetracker.org:80/announce,udp://tracker-udp.gbitt.info:80/announce,udp://tracker.0x7c0.com:6969/announce,udp://tracker.dler.com:6969/announce,udp://tracker.doko.moe:6969/announce,udp://tracker.fnix.net:6969/announce,udp://tracker.jamesthebard.net:6969/announce,udp://tracker.moeking.me:6969/announce,udp://tracker.opentrackr.org:1337/announce,udp://tracker.picotorrent.one:6969/announce,udp://tracker.qu.ax:6969/announce,udp://tracker.skyts.net:6969/announce,udp://tracker.srv00.com:6969/announce,udp://tracker.t-rb.org:6969/announce,udp://tracker.therarbg.com:6969/announce,udp://tracker.therarbg.to:6969/announce,udp://tracker.tiny-vps.com:6969/announce,udp://tracker.torrent.eu.org:451/announce,udp://tracker.tryhackx.org:6969/announce,udp://tracker1.bt.moack.co.kr:80/announce,udp://tracker1.myporn.club:9337/announce,udp://tracker2.dler.com:80/announce,udp://tracker2.dler.org:80/announce,udp://ttk2.nbaonlineservice.com:6969/announce,udp://wepzone.net:6969/announce,udp://www.torrent.eu.org:451/announce,wss://tracker.openwebtorrent.com:443/announce
+http://1337.abcvg.info:80/announce,http://bt.okmp3.ru:2710/announce,http://bvarf.tracker.sh:2086/announce,http://ipv6.rer.lol:6969/announce,http://nyaa.tracker.wf:7777/announce,http://open.acgnxtracker.com:80/announce,http://t.nyaatracker.com:80/announce,http://torrentsmd.com:8080/announce,http://tracker.bt4g.com:2095/announce,http://tracker.electro-torrent.pl:80/announce,http://tracker.files.fm:6969/announce,http://tracker.gbitt.info:80/announce,http://tracker.ipv6tracker.ru:80/announce,http://tracker.mywaifu.best:6969/announce,http://tracker.renfei.net:8080/announce,http://tracker.tfile.co:80/announce,http://www.all4nothin.net:80/announce.php,http://www.wareztorrent.com:80/announce,https://1337.abcvg.info:443/announce,https://t1.hloli.org:443/announce,https://tr.abir.ga:443/announce,https://tr.burnabyhighstar.com:443/announce,https://tracker.gbitt.info:443/announce,https://tracker.gcrreen.xyz:443/announce,https://tracker.kuroy.me:443/announce,https://tracker.loligirl.cn:443/announce,https://tracker.tamersunion.org:443/announce,https://tracker.yemekyedim.com:443/announce,https://tracker1.520.jp:443/announce,https://trackers.mlsub.net:443/announce,udp://amigacity.xyz:6969/announce,udp://api.boletera.org:3074/announce,udp://bt1.archive.org:6969/announce,udp://bt2.archive.org:6969/announce,udp://bubu.mapfactor.com:6969/announce,udp://d40969.acod.regrucolo.ru:6969/announce,udp://ec2-18-191-163-220.us-east-2.compute.amazonaws.com:6969/announce,udp://epider.me:6969/announce,udp://evan.im:6969/announce,udp://exodus.desync.com:6969/announce,udp://free.publictracker.xyz:6969/announce,udp://ipv6.fuuuuuck.com:6969/announce,udp://martin-gebhardt.eu:25/announce,udp://moonburrow.club:6969/announce,udp://odd-hd.fr:6969/announce,udp://oh.fuuuuuck.com:6969/announce,udp://open.demonii.com:1337/announce,udp://open.demonoid.ch:6969/announce,udp://open.stealth.si:80/announce,udp://open.tracker.ink:6969/announce,udp://open.xxtor.com:3074/announce,udp://opentor.org:2710/announce,udp://opentracker.io:6969/announce,udp://p2p.publictracker.xyz:6969/announce,udp://p4p.arenabg.com:1337/announce,udp://public.demonoid.ch:6969/announce,udp://retracker.hotplug.ru:2710/announce,udp://retracker.lanta.me:2710/announce,udp://run-2.publictracker.xyz:6969/announce,udp://run.publictracker.xyz:6969/announce,udp://tamas3.ynh.fr:6969/announce,udp://thetracker.org:80/announce,udp://tracker-udp.gbitt.info:80/announce,udp://tracker.0x7c0.com:6969/announce,udp://tracker.deadorbit.nl:6969/announce,udp://tracker.dler.com:6969/announce,udp://tracker.doko.moe:6969/announce,udp://tracker.fnix.net:6969/announce,udp://tracker.jamesthebard.net:6969/announce,udp://tracker.leena.network:6969/announce,udp://tracker.moeking.me:6969/announce,udp://tracker.opentrackr.org:1337/announce,udp://tracker.picotorrent.one:6969/announce,udp://tracker.publictracker.xyz:6969/announce,udp://tracker.silksa.co.za:6969/announce,udp://tracker.skyts.net:6969/announce,udp://tracker.srv00.com:6969/announce,udp://tracker.torrent.eu.org:451/announce,udp://tracker.tryhackx.org:6969/announce,udp://tracker1.bt.moack.co.kr:80/announce,udp://ttk2.nbaonlineservice.com:6969/announce,udp://www.torrent.eu.org:451/announce,wss://tracker.openwebtorrent.com:443/announce
```

### Comparing `videobox-0.6.1/videobox.egg-info/SOURCES.txt` & `videobox-0.7.0/videobox.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,61 @@
 .flake8
 .gitignore
+CONTRIBUTING.md
 LICENSE
 README.md
 Videobox.code-workspace
 app.py
 makefile
 package-lock.json
 package.json
 pyproject.toml
 requirements.txt
+screenshot.jpg
 setup-app.py
 .vscode/launch.json
 .vscode/settings.json
 assets/app.js
 assets/app.scss
 assets/balloon.css
 assets/button.scss
 assets/carousel.js
 assets/carousel.scss
 assets/helpers.scss
 assets/normalize.css
 assets/select.scss
 macos/icon.png
 macos/menubar-icon.svg
+tests/__init__.py
+tests/conftest.py
+tests/test_frontend.py
+tests/test_iso639.py
+tests/test_sync.py
+tests/sync/episodes.json
+tests/sync/releases.json
+tests/sync/series-tags.json
+tests/sync/series.json
+tests/sync/tags.json
+tests/sync/updated.json
 videobox/__init__.py
 videobox/api.py
 videobox/filters.py
-videobox/languages.py
+videobox/iso639.py
 videobox/models.py
+videobox/scraper.py
 videobox/sync.py
 videobox/trackers.txt
 videobox.egg-info/PKG-INFO
 videobox.egg-info/SOURCES.txt
 videobox.egg-info/dependency_links.txt
 videobox.egg-info/entry_points.txt
 videobox.egg-info/requires.txt
 videobox.egg-info/top_level.txt
 videobox/main/__init__.py
+videobox/main/announcer.py
 videobox/main/queries.py
 videobox/main/routes.py
 videobox/static/app.css
 videobox/static/app.css.map
 videobox/static/app.js
 videobox/static/app.js.map
 videobox/static/apple-touch-icon.png
@@ -56,41 +71,50 @@
 videobox/static/icon-grid.svg
 videobox/static/icon-heart-bold.svg
 videobox/static/icon-heart-break-bold.svg
 videobox/static/icon-heart-break.svg
 videobox/static/icon-heart.svg
 videobox/static/icon-heartbeat-bold.svg
 videobox/static/icon-heartbeat.svg
+videobox/static/icon-hourglass-bold.svg
+videobox/static/icon-hourglass.svg
+videobox/static/icon-info-bold.svg
+videobox/static/icon-info.svg
 videobox/static/icon-list-bold.svg
 videobox/static/icon-list.svg
 videobox/static/icon-magnet-bold.svg
 videobox/static/icon-magnet.svg
 videobox/static/icon-search-bold.svg
 videobox/static/icon-search.svg
+videobox/static/icon-sort-asc.svg
+videobox/static/icon-sort-desc.svg
 videobox/static/icon-tag-bold.svg
 videobox/static/icon-tag.svg
 videobox/static/icon-update-bold.svg
 videobox/static/icon-update.svg
+videobox/static/icon-warning-bold.svg
+videobox/static/icon-warning.svg
 videobox/static/logo.svg
 videobox/templates/404.html
+videobox/templates/_chart.html
 videobox/templates/_episodes-grid.html
 videobox/templates/_episodes-list.html
 videobox/templates/_follow-button.html
 videobox/templates/_following.html
 videobox/templates/_language-card-grid.html
 videobox/templates/_meta.html
 videobox/templates/_release_detail.html
 videobox/templates/_suggest.html
 videobox/templates/_tag-card-grid.html
-videobox/templates/_update-dialog-done.html
-videobox/templates/_update-dialog.html
+videobox/templates/_update-done.html
+videobox/templates/_update-progress.html
 videobox/templates/base.html
 videobox/templates/first-import.html
 videobox/templates/following.html
 videobox/templates/home.html
 videobox/templates/language_detail.html
-videobox/templates/log.html
 videobox/templates/macros.html
 videobox/templates/search_results.html
 videobox/templates/series_detail.html
+videobox/templates/status.html
 videobox/templates/tag_detail.html
 videobox/templates/tags.html
```

