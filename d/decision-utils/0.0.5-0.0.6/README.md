# Comparing `tmp/decision-utils-0.0.5.tar.gz` & `tmp/decision_utils-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decision-utils-0.0.5.tar", last modified: Thu Mar  7 07:22:55 2024, max compression
+gzip compressed data, was "decision_utils-0.0.6.tar", last modified: Sat May  4 01:30:17 2024, max compression
```

## Comparing `decision-utils-0.0.5.tar` & `decision_utils-0.0.6.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-03-07 07:22:55.951413 decision-utils-0.0.5/
--rw-r--r--   0 mv         (501) staff       (20)      882 2024-03-07 07:22:55.951084 decision-utils-0.0.5/PKG-INFO
--rw-r--r--   0 mv         (501) staff       (20)     6716 2024-02-17 09:43:52.000000 decision-utils-0.0.5/README.md
--rw-r--r--   0 mv         (501) staff       (20)     1133 2024-02-18 10:40:08.000000 decision-utils-0.0.5/pyproject.toml
--rw-r--r--   0 mv         (501) staff       (20)       38 2024-03-07 07:22:55.951481 decision-utils-0.0.5/setup.cfg
-drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-03-07 07:22:55.918629 decision-utils-0.0.5/src/
-drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-03-07 07:22:55.923473 decision-utils-0.0.5/src/decision_fetcher/
--rw-r--r--   0 mv         (501) staff       (20)      104 2024-02-17 00:51:48.000000 decision-utils-0.0.5/src/decision_fetcher/__init__.py
--rw-r--r--   0 mv         (501) staff       (20)     1674 2024-02-17 00:41:57.000000 decision-utils-0.0.5/src/decision_fetcher/__main__.py
--rw-r--r--   0 mv         (501) staff       (20)     2538 2024-02-17 00:18:59.000000 decision-utils-0.0.5/src/decision_fetcher/config.py
--rw-r--r--   0 mv         (501) staff       (20)     7075 2024-02-17 00:20:35.000000 decision-utils-0.0.5/src/decision_fetcher/dissect.py
--rw-r--r--   0 mv         (501) staff       (20)    14954 2024-02-17 10:24:17.000000 decision-utils-0.0.5/src/decision_fetcher/draft.py
--rw-r--r--   0 mv         (501) staff       (20)     4600 2024-02-17 00:19:02.000000 decision-utils-0.0.5/src/decision_fetcher/items.py
--rw-r--r--   0 mv         (501) staff       (20)     1364 2024-02-17 00:51:29.000000 decision-utils-0.0.5/src/decision_fetcher/logger.py
--rw-r--r--   0 mv         (501) staff       (20)     1220 2024-02-17 00:28:30.000000 decision-utils-0.0.5/src/decision_fetcher/sanitize.py
-drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-03-07 07:22:55.928799 decision-utils-0.0.5/src/decision_fetcher_fields/
--rw-r--r--   0 mv         (501) staff       (20)      597 2024-02-17 00:20:21.000000 decision-utils-0.0.5/src/decision_fetcher_fields/__init__.py
--rw-r--r--   0 mv         (501) staff       (20)      963 2024-02-17 00:21:38.000000 decision-utils-0.0.5/src/decision_fetcher_fields/citation.py
--rw-r--r--   0 mv         (501) staff       (20)     3057 2024-02-16 16:53:30.000000 decision-utils-0.0.5/src/decision_fetcher_fields/cullables.py
-drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-03-07 07:22:55.930059 decision-utils-0.0.5/src/decision_fetcher_fields/dispositive/
--rw-r--r--   0 mv         (501) staff       (20)      138 2024-02-16 16:53:30.000000 decision-utils-0.0.5/src/decision_fetcher_fields/dispositive/__init__.py
--rw-r--r--   0 mv         (501) staff       (20)      469 2024-02-16 16:53:30.000000 decision-utils-0.0.5/src/decision_fetcher_fields/dispositive/ordered.py
--rw-r--r--   0 mv         (501) staff       (20)     2492 2024-02-17 00:18:41.000000 decision-utils-0.0.5/src/decision_fetcher_fields/dispositive/phrases.py
--rw-r--r--   0 mv         (501) staff       (20)     1658 2024-02-16 16:53:30.000000 decision-utils-0.0.5/src/decision_fetcher_fields/dispositive/wherefore.py
--rw-r--r--   0 mv         (501) staff       (20)      893 2024-02-16 16:53:30.000000 decision-utils-0.0.5/src/decision_fetcher_fields/footnotes.py
--rw-r--r--   0 mv         (501) staff       (20)     1626 2024-02-17 00:21:43.000000 decision-utils-0.0.5/src/decision_fetcher_fields/header.py
--rw-r--r--   0 mv         (501) staff       (20)     1092 2024-02-16 16:53:30.000000 decision-utils-0.0.5/src/decision_fetcher_fields/ruling.py
--rw-r--r--   0 mv         (501) staff       (20)      891 2024-02-16 16:53:30.000000 decision-utils-0.0.5/src/decision_fetcher_fields/ruling_cues.py
-drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-03-07 07:22:55.934620 decision-utils-0.0.5/src/decision_fetcher_fields/ruling_patterns/
--rw-r--r--   0 mv         (501) staff       (20)      415 2024-02-16 16:53:30.000000 decision-utils-0.0.5/src/decision_fetcher_fields/ruling_patterns/__init__.py
--rw-r--r--   0 mv         (501) staff       (20)      229 2024-02-16 16:53:30.000000 decision-utils-0.0.5/src/decision_fetcher_fields/ruling_patterns/after_review.py
--rw-r--r--   0 mv         (501) staff       (20)      688 2024-02-16 16:53:30.000000 decision-utils-0.0.5/src/decision_fetcher_fields/ruling_patterns/court_acts.py
--rw-r--r--   0 mv         (501) staff       (20)     1554 2024-02-16 16:53:30.000000 decision-utils-0.0.5/src/decision_fetcher_fields/ruling_patterns/court_admin.py
--rw-r--r--   0 mv         (501) staff       (20)     1098 2024-02-16 16:53:30.000000 decision-utils-0.0.5/src/decision_fetcher_fields/ruling_patterns/granted_denied.py
--rw-r--r--   0 mv         (501) staff       (20)      664 2024-02-16 16:53:30.000000 decision-utils-0.0.5/src/decision_fetcher_fields/ruling_patterns/hence_this.py
--rw-r--r--   0 mv         (501) staff       (20)     1647 2024-02-16 16:53:30.000000 decision-utils-0.0.5/src/decision_fetcher_fields/ruling_patterns/issue_errors.py
--rw-r--r--   0 mv         (501) staff       (20)      187 2024-02-16 16:53:30.000000 decision-utils-0.0.5/src/decision_fetcher_fields/ruling_patterns/issue_resolution.py
--rw-r--r--   0 mv         (501) staff       (20)      874 2024-02-16 16:53:30.000000 decision-utils-0.0.5/src/decision_fetcher_fields/ruling_patterns/main_issue.py
--rw-r--r--   0 mv         (501) staff       (20)      411 2024-02-16 16:53:30.000000 decision-utils-0.0.5/src/decision_fetcher_fields/ruling_patterns/merit.py
--rw-r--r--   0 mv         (501) staff       (20)      459 2024-02-16 16:53:30.000000 decision-utils-0.0.5/src/decision_fetcher_fields/ruling_patterns/resolve_issue.py
--rw-r--r--   0 mv         (501) staff       (20)      270 2024-02-16 16:53:30.000000 decision-utils-0.0.5/src/decision_fetcher_fields/ruling_patterns/single_issue.py
-drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-03-07 07:22:55.935562 decision-utils-0.0.5/src/decision_fetcher_fields/tags/
--rw-r--r--   0 mv         (501) staff       (20)      185 2024-02-16 16:53:30.000000 decision-utils-0.0.5/src/decision_fetcher_fields/tags/__init__.py
--rw-r--r--   0 mv         (501) staff       (20)     1450 2024-02-16 16:53:30.000000 decision-utils-0.0.5/src/decision_fetcher_fields/tags/base.py
--rw-r--r--   0 mv         (501) staff       (20)     1452 2024-02-16 16:53:30.000000 decision-utils-0.0.5/src/decision_fetcher_fields/tags/specific.py
--rw-r--r--   0 mv         (501) staff       (20)      987 2024-02-16 16:53:30.000000 decision-utils-0.0.5/src/decision_fetcher_fields/tags/utils.py
--rw-r--r--   0 mv         (501) staff       (20)     3823 2024-02-16 16:53:30.000000 decision-utils-0.0.5/src/decision_fetcher_fields/title_tags.py
--rw-r--r--   0 mv         (501) staff       (20)      183 2024-02-17 00:21:29.000000 decision-utils-0.0.5/src/decision_fetcher_fields/utils.py
--rw-r--r--   0 mv         (501) staff       (20)      825 2024-02-16 16:53:30.000000 decision-utils-0.0.5/src/decision_fetcher_fields/voteline.py
--rw-r--r--   0 mv         (501) staff       (20)     1022 2024-02-17 00:21:54.000000 decision-utils-0.0.5/src/decision_fetcher_fields/writer.py
-drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-03-07 07:22:55.937120 decision-utils-0.0.5/src/decision_updater/
--rw-r--r--   0 mv         (501) staff       (20)      283 2024-02-17 08:36:48.000000 decision-utils-0.0.5/src/decision_updater/__init__.py
--rw-r--r--   0 mv         (501) staff       (20)     1139 2024-02-16 17:00:02.000000 decision-utils-0.0.5/src/decision_updater/__main__.py
--rw-r--r--   0 mv         (501) staff       (20)     3247 2024-02-17 15:22:54.000000 decision-utils-0.0.5/src/decision_updater/clean.py
--rw-r--r--   0 mv         (501) staff       (20)      437 2024-02-08 03:12:00.000000 decision-utils-0.0.5/src/decision_updater/dumper.py
--rw-r--r--   0 mv         (501) staff       (20)     1364 2024-02-08 03:12:00.000000 decision-utils-0.0.5/src/decision_updater/logger.py
--rw-r--r--   0 mv         (501) staff       (20)     1164 2024-02-08 08:16:42.000000 decision-utils-0.0.5/src/decision_updater/md.py
--rw-r--r--   0 mv         (501) staff       (20)     4125 2024-02-20 01:23:36.000000 decision-utils-0.0.5/src/decision_updater/writer.py
-drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-03-07 07:22:55.939465 decision-utils-0.0.5/src/decision_utils/
--rw-r--r--   0 mv         (501) staff       (20)      201 2024-02-17 00:38:58.000000 decision-utils-0.0.5/src/decision_utils/__init__.py
--rw-r--r--   0 mv         (501) staff       (20)       13 2024-02-08 03:41:37.000000 decision-utils-0.0.5/src/decision_utils/__main__.py
--rw-r--r--   0 mv         (501) staff       (20)     2915 2023-10-13 13:27:11.000000 decision-utils-0.0.5/src/decision_utils/author.py
--rw-r--r--   0 mv         (501) staff       (20)     7698 2024-01-29 02:03:38.000000 decision-utils-0.0.5/src/decision_utils/block.py
--rw-r--r--   0 mv         (501) staff       (20)    10486 2024-02-17 08:16:33.000000 decision-utils-0.0.5/src/decision_utils/decision.py
--rw-r--r--   0 mv         (501) staff       (20)    10524 2024-02-19 13:49:19.000000 decision-utils-0.0.5/src/decision_utils/opinion.py
-drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-03-07 07:22:55.949026 decision-utils-0.0.5/src/decision_utils/utils/
--rw-r--r--   0 mv         (501) staff       (20)      259 2023-10-29 05:19:46.000000 decision-utils-0.0.5/src/decision_utils/utils/__init__.py
--rw-r--r--   0 mv         (501) staff       (20)     4624 2023-10-25 02:47:41.000000 decision-utils-0.0.5/src/decision_utils/utils/annex.py
--rw-r--r--   0 mv         (501) staff       (20)      410 2023-10-19 05:38:51.000000 decision-utils-0.0.5/src/decision_utils/utils/casename.py
--rw-r--r--   0 mv         (501) staff       (20)     5184 2023-10-16 09:49:26.000000 decision-utils-0.0.5/src/decision_utils/utils/courts.py
--rw-r--r--   0 mv         (501) staff       (20)      437 2023-10-14 10:37:51.000000 decision-utils-0.0.5/src/decision_utils/utils/dumper.py
--rw-r--r--   0 mv         (501) staff       (20)     2876 2023-10-18 03:38:31.000000 decision-utils-0.0.5/src/decision_utils/utils/fallo.py
--rw-r--r--   0 mv         (501) staff       (20)     3254 2024-02-17 08:40:03.000000 decision-utils-0.0.5/src/decision_utils/utils/formatter.py
--rw-r--r--   0 mv         (501) staff       (20)     1059 2024-02-06 22:04:26.000000 decision-utils-0.0.5/src/decision_utils/utils/md.py
--rw-r--r--   0 mv         (501) staff       (20)     5639 2023-10-24 14:52:02.000000 decision-utils-0.0.5/src/decision_utils/utils/phrase.py
--rw-r--r--   0 mv         (501) staff       (20)      846 2023-10-14 10:38:30.000000 decision-utils-0.0.5/src/decision_utils/utils/regex.py
-drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-03-07 07:22:55.950007 decision-utils-0.0.5/src/decision_utils.egg-info/
--rw-r--r--   0 mv         (501) staff       (20)      882 2024-03-07 07:22:55.000000 decision-utils-0.0.5/src/decision_utils.egg-info/PKG-INFO
--rw-r--r--   0 mv         (501) staff       (20)     2870 2024-03-07 07:22:55.000000 decision-utils-0.0.5/src/decision_utils.egg-info/SOURCES.txt
--rw-r--r--   0 mv         (501) staff       (20)        1 2024-03-07 07:22:55.000000 decision-utils-0.0.5/src/decision_utils.egg-info/dependency_links.txt
--rw-r--r--   0 mv         (501) staff       (20)      128 2024-03-07 07:22:55.000000 decision-utils-0.0.5/src/decision_utils.egg-info/entry_points.txt
--rw-r--r--   0 mv         (501) staff       (20)      328 2024-03-07 07:22:55.000000 decision-utils-0.0.5/src/decision_utils.egg-info/requires.txt
--rw-r--r--   0 mv         (501) staff       (20)       90 2024-03-07 07:22:55.000000 decision-utils-0.0.5/src/decision_utils.egg-info/top_level.txt
-drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-03-07 07:22:55.949577 decision-utils-0.0.5/src/decision_watcher/
--rw-r--r--   0 mv         (501) staff       (20)       24 2024-02-08 03:40:51.000000 decision-utils-0.0.5/src/decision_watcher/__init__.py
--rw-r--r--   0 mv         (501) staff       (20)     2322 2024-02-17 00:39:11.000000 decision-utils-0.0.5/src/decision_watcher/__main__.py
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-04 01:30:17.839624 decision_utils-0.0.6/
+-rw-r--r--   0 mv         (501) staff       (20)      832 2024-05-04 01:30:17.839250 decision_utils-0.0.6/PKG-INFO
+-rw-r--r--   0 mv         (501) staff       (20)     7388 2024-05-04 01:29:37.000000 decision_utils-0.0.6/README.md
+-rw-r--r--   0 mv         (501) staff       (20)     1284 2024-05-04 01:29:37.000000 decision_utils-0.0.6/pyproject.toml
+-rw-r--r--   0 mv         (501) staff       (20)       38 2024-05-04 01:30:17.839701 decision_utils-0.0.6/setup.cfg
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-04 01:30:17.808068 decision_utils-0.0.6/src/
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-04 01:30:17.812624 decision_utils-0.0.6/src/decision_fetcher/
+-rw-r--r--   0 mv         (501) staff       (20)      104 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher/__init__.py
+-rw-r--r--   0 mv         (501) staff       (20)     1670 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher/__main__.py
+-rw-r--r--   0 mv         (501) staff       (20)     2538 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher/config.py
+-rw-r--r--   0 mv         (501) staff       (20)     7075 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher/dissect.py
+-rw-r--r--   0 mv         (501) staff       (20)    14966 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher/draft.py
+-rw-r--r--   0 mv         (501) staff       (20)     4640 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher/items.py
+-rw-r--r--   0 mv         (501) staff       (20)     1364 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher/logger.py
+-rw-r--r--   0 mv         (501) staff       (20)     1220 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher/sanitize.py
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-04 01:30:17.818481 decision_utils-0.0.6/src/decision_fetcher_fields/
+-rw-r--r--   0 mv         (501) staff       (20)      597 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/__init__.py
+-rw-r--r--   0 mv         (501) staff       (20)      963 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/citation.py
+-rw-r--r--   0 mv         (501) staff       (20)     3057 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/cullables.py
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-04 01:30:17.819459 decision_utils-0.0.6/src/decision_fetcher_fields/dispositive/
+-rw-r--r--   0 mv         (501) staff       (20)      138 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/dispositive/__init__.py
+-rw-r--r--   0 mv         (501) staff       (20)      469 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/dispositive/ordered.py
+-rw-r--r--   0 mv         (501) staff       (20)     2492 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/dispositive/phrases.py
+-rw-r--r--   0 mv         (501) staff       (20)     1658 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/dispositive/wherefore.py
+-rw-r--r--   0 mv         (501) staff       (20)      893 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/footnotes.py
+-rw-r--r--   0 mv         (501) staff       (20)     1626 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/header.py
+-rw-r--r--   0 mv         (501) staff       (20)     1092 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/ruling.py
+-rw-r--r--   0 mv         (501) staff       (20)      891 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/ruling_cues.py
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-04 01:30:17.824996 decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/
+-rw-r--r--   0 mv         (501) staff       (20)      415 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/__init__.py
+-rw-r--r--   0 mv         (501) staff       (20)      229 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/after_review.py
+-rw-r--r--   0 mv         (501) staff       (20)      688 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/court_acts.py
+-rw-r--r--   0 mv         (501) staff       (20)     1554 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/court_admin.py
+-rw-r--r--   0 mv         (501) staff       (20)     1098 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/granted_denied.py
+-rw-r--r--   0 mv         (501) staff       (20)      664 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/hence_this.py
+-rw-r--r--   0 mv         (501) staff       (20)     1647 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/issue_errors.py
+-rw-r--r--   0 mv         (501) staff       (20)      187 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/issue_resolution.py
+-rw-r--r--   0 mv         (501) staff       (20)      874 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/main_issue.py
+-rw-r--r--   0 mv         (501) staff       (20)      411 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/merit.py
+-rw-r--r--   0 mv         (501) staff       (20)      459 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/resolve_issue.py
+-rw-r--r--   0 mv         (501) staff       (20)      270 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/single_issue.py
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-04 01:30:17.827545 decision_utils-0.0.6/src/decision_fetcher_fields/tags/
+-rw-r--r--   0 mv         (501) staff       (20)      185 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/tags/__init__.py
+-rw-r--r--   0 mv         (501) staff       (20)     1450 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/tags/base.py
+-rw-r--r--   0 mv         (501) staff       (20)     1452 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/tags/specific.py
+-rw-r--r--   0 mv         (501) staff       (20)      987 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/tags/utils.py
+-rw-r--r--   0 mv         (501) staff       (20)     3823 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/title_tags.py
+-rw-r--r--   0 mv         (501) staff       (20)      183 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/utils.py
+-rw-r--r--   0 mv         (501) staff       (20)      825 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/voteline.py
+-rw-r--r--   0 mv         (501) staff       (20)     1022 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_fetcher_fields/writer.py
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-04 01:30:17.829731 decision_utils-0.0.6/src/decision_updater/
+-rw-r--r--   0 mv         (501) staff       (20)      283 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_updater/__init__.py
+-rw-r--r--   0 mv         (501) staff       (20)     1139 2024-02-16 17:00:02.000000 decision_utils-0.0.6/src/decision_updater/__main__.py
+-rw-r--r--   0 mv         (501) staff       (20)     3247 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_updater/clean.py
+-rw-r--r--   0 mv         (501) staff       (20)      437 2024-02-08 03:12:00.000000 decision_utils-0.0.6/src/decision_updater/dumper.py
+-rw-r--r--   0 mv         (501) staff       (20)     1364 2024-02-08 03:12:00.000000 decision_utils-0.0.6/src/decision_updater/logger.py
+-rw-r--r--   0 mv         (501) staff       (20)     1164 2024-02-08 08:16:42.000000 decision_utils-0.0.6/src/decision_updater/md.py
+-rw-r--r--   0 mv         (501) staff       (20)     4129 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_updater/writer.py
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-04 01:30:17.831728 decision_utils-0.0.6/src/decision_utils/
+-rw-r--r--   0 mv         (501) staff       (20)      201 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_utils/__init__.py
+-rw-r--r--   0 mv         (501) staff       (20)       13 2024-02-08 03:41:37.000000 decision_utils-0.0.6/src/decision_utils/__main__.py
+-rw-r--r--   0 mv         (501) staff       (20)     2915 2023-10-13 13:27:11.000000 decision_utils-0.0.6/src/decision_utils/author.py
+-rw-r--r--   0 mv         (501) staff       (20)     7698 2024-01-29 02:03:38.000000 decision_utils-0.0.6/src/decision_utils/block.py
+-rw-r--r--   0 mv         (501) staff       (20)    10486 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_utils/decision.py
+-rw-r--r--   0 mv         (501) staff       (20)    10760 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_utils/opinion.py
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-04 01:30:17.836876 decision_utils-0.0.6/src/decision_utils/utils/
+-rw-r--r--   0 mv         (501) staff       (20)      259 2023-10-29 05:19:46.000000 decision_utils-0.0.6/src/decision_utils/utils/__init__.py
+-rw-r--r--   0 mv         (501) staff       (20)     4624 2023-10-25 02:47:41.000000 decision_utils-0.0.6/src/decision_utils/utils/annex.py
+-rw-r--r--   0 mv         (501) staff       (20)      410 2023-10-19 05:38:51.000000 decision_utils-0.0.6/src/decision_utils/utils/casename.py
+-rw-r--r--   0 mv         (501) staff       (20)     5184 2023-10-16 09:49:26.000000 decision_utils-0.0.6/src/decision_utils/utils/courts.py
+-rw-r--r--   0 mv         (501) staff       (20)      437 2023-10-14 10:37:51.000000 decision_utils-0.0.6/src/decision_utils/utils/dumper.py
+-rw-r--r--   0 mv         (501) staff       (20)     2876 2023-10-18 03:38:31.000000 decision_utils-0.0.6/src/decision_utils/utils/fallo.py
+-rw-r--r--   0 mv         (501) staff       (20)     3254 2024-02-17 08:40:03.000000 decision_utils-0.0.6/src/decision_utils/utils/formatter.py
+-rw-r--r--   0 mv         (501) staff       (20)     1059 2024-02-06 22:04:26.000000 decision_utils-0.0.6/src/decision_utils/utils/md.py
+-rw-r--r--   0 mv         (501) staff       (20)     5639 2023-10-24 14:52:02.000000 decision_utils-0.0.6/src/decision_utils/utils/phrase.py
+-rw-r--r--   0 mv         (501) staff       (20)      846 2023-10-14 10:38:30.000000 decision_utils-0.0.6/src/decision_utils/utils/regex.py
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-04 01:30:17.838132 decision_utils-0.0.6/src/decision_utils.egg-info/
+-rw-r--r--   0 mv         (501) staff       (20)      832 2024-05-04 01:30:17.000000 decision_utils-0.0.6/src/decision_utils.egg-info/PKG-INFO
+-rw-r--r--   0 mv         (501) staff       (20)     2870 2024-05-04 01:30:17.000000 decision_utils-0.0.6/src/decision_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 mv         (501) staff       (20)        1 2024-05-04 01:30:17.000000 decision_utils-0.0.6/src/decision_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 mv         (501) staff       (20)      128 2024-05-04 01:30:17.000000 decision_utils-0.0.6/src/decision_utils.egg-info/entry_points.txt
+-rw-r--r--   0 mv         (501) staff       (20)      309 2024-05-04 01:30:17.000000 decision_utils-0.0.6/src/decision_utils.egg-info/requires.txt
+-rw-r--r--   0 mv         (501) staff       (20)       90 2024-05-04 01:30:17.000000 decision_utils-0.0.6/src/decision_utils.egg-info/top_level.txt
+drwxr-xr-x   0 mv         (501) staff       (20)        0 2024-05-04 01:30:17.837657 decision_utils-0.0.6/src/decision_watcher/
+-rw-r--r--   0 mv         (501) staff       (20)       24 2024-02-08 03:40:51.000000 decision_utils-0.0.6/src/decision_watcher/__init__.py
+-rw-r--r--   0 mv         (501) staff       (20)     2322 2024-05-04 01:29:37.000000 decision_utils-0.0.6/src/decision_watcher/__main__.py
```

### Comparing `decision-utils-0.0.5/PKG-INFO` & `decision_utils-0.0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: decision-utils
-Version: 0.0.5
+Version: 0.0.6
 Summary: Preprocess frontmatter-ish markdown with Philippine artifacts, statutes, citations.
 Requires-Python: >=3.11
-Requires-Dist: statute-utils>=0.6.10
+Requires-Dist: statute-utils>=0.6.11
 Requires-Dist: citation-utils>=0.4.10
 Requires-Dist: citation-title>=0.0.1
 Requires-Dist: corpus-judge>=0.1.4
-Requires-Dist: python-frontmatter>=1.1.0
 Requires-Dist: environs>=10.3
-Requires-Dist: watchdog>=3.0
-Requires-Dist: beautifulsoup4>=4.12.3
 Requires-Dist: markdownify>=0.11.6
-Requires-Dist: httpx>=0.26.0
+Requires-Dist: httpx>=0.27.0
 Requires-Dist: html-sanitizer>=2.3.0
+Requires-Dist: beautifulsoup4>=4.12.3
+Requires-Dist: watchdog>=3.0
+Requires-Dist: python-frontmatter>=1.1.0
 Requires-Dist: rich>=13.7
 Provides-Extra: dev
 Requires-Dist: ipykernel>=6.29; extra == "dev"
-Requires-Dist: pytest>=8.0; extra == "dev"
+Requires-Dist: pytest>=8.2; extra == "dev"
 Requires-Dist: pytest-cov>=4.1; extra == "dev"
-Requires-Dist: sqlite-utils>=3.36; extra == "dev"
 Requires-Dist: build>=1.0.3; extra == "dev"
 Requires-Dist: twine>=4.0.2; extra == "dev"
```

### Comparing `decision-utils-0.0.5/README.md` & `decision_utils-0.0.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -48,51 +48,70 @@
 
 First create an interim `decision_files.db`:
 
 ```sh
 fetcher init-db
 ```
 
-Then collect the links, storing the same to the database:
+Populate this database with links via:
 
 ```sh
-fetcher list-urls --start 1996 --2024
+fetcher list-urls --start 1996 --end 2024
 ```
 
-Then draft local files in `/corpus-decisions`
+This searches the elibrary for decisions within the years indicated. Note that `--end` means it is excluded from the years list.
+
+The collection of entries in the database serves as a directory.
+
+This allows us to add files to a local directory (skipping pre-existing files), e.g.: `/corpus-decisions`.
+
+Create markdown files based on the database links via:
 
 ```sh
 fetcher draft-files --start 2019
 ```
 
-After files are considered drafts since these ought to be edited first, e.g. search for markdown files prefixed with `**/a*.md` with regex string: `^label:`
+The files are considered **drafts** since these ought to be edited first.
+
+### Edit opinion files
+
+1. Go to the local directory where the files have been "drafted": e.g.: `/corpus-decisions`.
+2. Using VSCode, search for markdown files prefixed with `**/a*.md` with regex string: `^label:`.
+3. Alhtough some really do not have any others (being a per curiam opinion), most files need to be adjusted since the opinion authors have to be identified with their digits
+4. Where it is warranted, create a separate `/opinion` folder on each decision
 
 ## `decision-watcher`
 
-When modifying files in the /corpus-decisions directory (outside of this package), the markdown file is modified automatically with `decision_utils.update_content()`. In order for automation to work, the folder needs to be watched for manual changes.
+When modifying files in the /corpus-decisions directory (outside of this package), the markdown file cane be modified automatically with `decision_utils.update_content()`.
+
+But in order for automation to work, the folder needs to be watched for manual changes.
 
 ```sh
 watcher # uses default ../corpus-decisions
 ```
 
 This component only needs to be run before a user edits the local markdown files directly.
 
 ## `decision-updater`
 
+> [!IMPORTANT]
+> Used when bulk modifying `/corpus-decisions` metadata.
+
 This component of the package only needs to be run occasionally, specifically when any/all of the following libraries are updated:
 
 1. `citation-utils`
 2. `statute-utils`
 3. `citation-title`
 4. `lexcorpora` _en_artifacts model_
 
-When these libraries are updated, the outputted metadata will vary. Hence the need to re-run for consistency. In addition, cleaning functions can be applied.
+When these libraries are updated, the outputted metadata will vary.
 
-> [!IMPORTANT]
-> `decision-updater` necessary when bulk modifying `/corpus-decisions` metadata.
+Hence the need to re-run for consistency.
+
+In addition, cleaning functions can be applied.
 
 Delete `statute_files.db` (if it already exists) since this may have been previously updated via their original yaml files. The lack of a statutes database is remedied when program is run for the first time c/o _statute-utils_. The latter package is used to detect statute objects found within each opinion and add it to each opinion's metadata.
 
 To run the updating step, open up a jupyter notebook:
 
 ```sh
 # expects a range of years
```

### Comparing `decision-utils-0.0.5/pyproject.toml` & `decision_utils-0.0.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 [project]
 name = "decision-utils"
 description = "Preprocess frontmatter-ish markdown with Philippine artifacts, statutes, citations."
-version = "0.0.5"
+version = "0.0.6"
 requires-python = ">=3.11"
 dependencies = [
-  "statute-utils >= 0.6.10",
+  "statute-utils >= 0.6.11",
   "citation-utils >= 0.4.10",
   "citation-title >= 0.0.1",
   "corpus-judge >= 0.1.4",
-  "python-frontmatter >= 1.1.0",
-  "environs >= 10.3",
-  "watchdog >= 3.0",
-  "beautifulsoup4 >= 4.12.3",
-  "markdownify >= 0.11.6",
-  "httpx >= 0.26.0",
-  "html-sanitizer >= 2.3.0",
-  "rich >= 13.7",
+  "environs >= 10.3",             # config
+  "markdownify >= 0.11.6",        # fetcher
+  "httpx >= 0.27.0",              # fetcher
+  "html-sanitizer >= 2.3.0",      # fetcher
+  "beautifulsoup4 >= 4.12.3",     # fetcher-fields
+  "watchdog >= 3.0",              # updater
+  "python-frontmatter >= 1.1.0",  # updater / fetcher
+  "rich >= 13.7",                 # updater / watcher
 ]
 
 [project.optional-dependencies]
 dev = [
   "ipykernel >= 6.29",
-  "pytest >= 8.0",
+  "pytest >= 8.2",
   "pytest-cov >= 4.1",
-  "sqlite-utils >= 3.36",
   "build >= 1.0.3",
   "twine >= 4.0.2",
 ]
 
 [project.scripts]
 fetcher = "decision_fetcher:cli"
 updater = "decision_updater:update_files"
 watcher = "decision_watcher:watch_files"
 
 [tool.pytest.ini_options]
-minversion = "8.0"
+minversion = "8.2"
 addopts = "-ra -q -vv --cov --doctest-modules"
 testpaths = ["src","tests"]
 filterwarnings = ["ignore::DeprecationWarning"]
 
 [tool.ruff]
 line-length = 88
```

### Comparing `decision-utils-0.0.5/src/decision_fetcher/__main__.py` & `decision_utils-0.0.6/src/decision_fetcher/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 
 @cli.command()
 @click.option(
     "--start",
     required=True,
     type=int,
-    help="Start year to include from the the database",
+    help="Start year to include from the database",
 )
 def draft_files(start: int):
     db = Database(filename_or_conn=db_file, use_counts_table=True)
     for row in db["elib"].rows_where("date >= ?", (f"{start}-01-01",)):
         try:
             draft = KeyDraft(key=row["id"])
             draft.add_files(db=db)
```

### Comparing `decision-utils-0.0.5/src/decision_fetcher/config.py` & `decision_utils-0.0.6/src/decision_fetcher/config.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_fetcher/dissect.py` & `decision_utils-0.0.6/src/decision_fetcher/dissect.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_fetcher/draft.py` & `decision_utils-0.0.6/src/decision_fetcher/draft.py`

 * *Files 0% similar despite different names*

```diff
@@ -407,11 +407,11 @@
                 logging.info(f"Creating {target_file=}.")
                 row.write_to_target_file(db)
 
                 # clean the file
                 update_content(target_file)
 
                 # add statutes / citations / short title (if appropriate)
-                update_markdown_opinion_file(target_file)
+                update_markdown_opinion_file(target_file, timeout=25)
                 if row.counter == 1:  # ponencia
                     record = convert_path_to_record(target_file)
                     db["decisions"].insert(record=record)  # type: ignore
```

### Comparing `decision-utils-0.0.5/src/decision_fetcher/items.py` & `decision_utils-0.0.6/src/decision_fetcher/items.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,15 @@
 
     @classmethod
     def from_year(cls, year: int, db: Database):
         for member in cls:
             # e-library partial URL to get a list of decisions for a given month
             if soup := url_to_soup(url=f"{ELIB}/docmonth/{member.name}/{year}/1"):
                 for tag in soup(id="container_title")[0]("li"):
+                    # logging.info(tag)
                     try:
                         item = Item(
                             url=tag("a")[0]["href"].replace(
                                 "showdocs",
                                 "showdocsfriendly",
                             ),  # get the better formatted url
                             docket=tag("strong")[0].text,
```

### Comparing `decision-utils-0.0.5/src/decision_fetcher/logger.py` & `decision_utils-0.0.6/src/decision_fetcher/logger.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_fetcher/sanitize.py` & `decision_utils-0.0.6/src/decision_fetcher/sanitize.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_fetcher_fields/__init__.py` & `decision_utils-0.0.6/src/decision_fetcher_fields/__init__.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_fetcher_fields/citation.py` & `decision_utils-0.0.6/src/decision_fetcher_fields/citation.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_fetcher_fields/cullables.py` & `decision_utils-0.0.6/src/decision_fetcher_fields/cullables.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_fetcher_fields/dispositive/phrases.py` & `decision_utils-0.0.6/src/decision_fetcher_fields/dispositive/phrases.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_fetcher_fields/dispositive/wherefore.py` & `decision_utils-0.0.6/src/decision_fetcher_fields/dispositive/wherefore.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_fetcher_fields/footnotes.py` & `decision_utils-0.0.6/src/decision_fetcher_fields/footnotes.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_fetcher_fields/header.py` & `decision_utils-0.0.6/src/decision_fetcher_fields/header.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_fetcher_fields/ruling.py` & `decision_utils-0.0.6/src/decision_fetcher_fields/ruling.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_fetcher_fields/ruling_cues.py` & `decision_utils-0.0.6/src/decision_fetcher_fields/ruling_cues.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_fetcher_fields/ruling_patterns/court_acts.py` & `decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/court_acts.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_fetcher_fields/ruling_patterns/court_admin.py` & `decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/court_admin.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_fetcher_fields/ruling_patterns/granted_denied.py` & `decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/granted_denied.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_fetcher_fields/ruling_patterns/hence_this.py` & `decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/hence_this.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_fetcher_fields/ruling_patterns/issue_errors.py` & `decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/issue_errors.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_fetcher_fields/ruling_patterns/main_issue.py` & `decision_utils-0.0.6/src/decision_fetcher_fields/ruling_patterns/main_issue.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_fetcher_fields/tags/base.py` & `decision_utils-0.0.6/src/decision_fetcher_fields/tags/base.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_fetcher_fields/tags/specific.py` & `decision_utils-0.0.6/src/decision_fetcher_fields/tags/specific.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_fetcher_fields/tags/utils.py` & `decision_utils-0.0.6/src/decision_fetcher_fields/tags/utils.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_fetcher_fields/title_tags.py` & `decision_utils-0.0.6/src/decision_fetcher_fields/title_tags.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_fetcher_fields/voteline.py` & `decision_utils-0.0.6/src/decision_fetcher_fields/voteline.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_fetcher_fields/writer.py` & `decision_utils-0.0.6/src/decision_fetcher_fields/writer.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_updater/__main__.py` & `decision_utils-0.0.6/src/decision_updater/__main__.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_updater/clean.py` & `decision_utils-0.0.6/src/decision_updater/clean.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_updater/logger.py` & `decision_utils-0.0.6/src/decision_updater/logger.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_updater/md.py` & `decision_utils-0.0.6/src/decision_updater/md.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_updater/writer.py` & `decision_utils-0.0.6/src/decision_updater/writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,22 +105,22 @@
 
     # frontmatter.dump does not include a trailing new line which is
     # a standard for markdown files, a hack is simply to add a new line manually
     # see https://github.com/eyeseast/python-frontmatter/issues/87
     # file.write_text(data=file.read_text() + "\n")
 
 
-def update_markdown_opinion_file(file: Path, timeout: float = 5):
+def update_markdown_opinion_file(file: Path, timeout: float = 10):
     """Time-based wrapper around `update_file()` to ensure that it doesn't exceed
-    5 seconds in processing the file. If the process is still running at the 5-second
+    10 seconds in processing the file. If the process is still running at the 10-second
     mark, will terminate.
 
     Args:
         file (Path): File to update
-        timeout (float, optional): Number of seconds before timeout. Defaults to 5.
+        timeout (float, optional): Number of seconds before timeout. Defaults to 10.
     """
     process = multiprocessing.Process(target=update_opinion, args=(file,))
     process.start()
     process.join(timeout=timeout)
     if process.is_alive():
         logging.error(f"Took too long: {file=}")
         process.terminate()
```

### Comparing `decision-utils-0.0.5/src/decision_utils/author.py` & `decision_utils-0.0.6/src/decision_utils/author.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_utils/block.py` & `decision_utils-0.0.6/src/decision_utils/block.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_utils/decision.py` & `decision_utils-0.0.6/src/decision_utils/decision.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_utils/opinion.py` & `decision_utils-0.0.6/src/decision_utils/opinion.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .block import Block, fn_pattern
 from .utils import Annex, Footnote
 
 INVALID_ARTIFACTS = [
     "Act",
     "Manual",
     "same Constitution",
+    "this Constitution",
     "Children Act",
     "(Constitution",
     "Precinct No. 4",
     "CHILD",
     "Philippine Code",
     "Per Special Order No. 775 dated November 3, 2009",
     "ICAB",
@@ -76,14 +77,15 @@
     rule = auto()
     statute = auto()
 
 
 @dataclass
 class Artifact:
     text: str
+    cased_text: str
     category: ArtifactCategory
     count: int
 
     @property
     def as_row(self):
         data = asdict(self)
         data.pop("category")
@@ -91,29 +93,31 @@
         return data
 
     @classmethod
     def from_phrases(cls, phrases: list[str]):
         artifacts = []
         if phrases:
             for phrase in phrases:  # type: ignore
-                if objs := phrase.split("__"):
-                    if len(objs) == 3:
-                        text = objs[0].strip(": ")
+                if partial_phrases := phrase.split("__"):
+                    if len(partial_phrases) == 3:
+                        text = partial_phrases[0].strip(": ")
                         if not text or len(text) <= 2:
                             logging.error(f"Bad phrase: {phrase}")
                             continue
                         if text in INVALID_ARTIFACTS:
                             logging.error(f"Skip invalid phrase: {phrase}")
                             continue
-                        key = objs[1].strip("_ ")  # handle cases like _docket
+                        key = partial_phrases[1].strip("_ ")  # e.g. _docket
                         artifacts.append(
                             Artifact(
-                                text=objs[0],
+                                # ensure uniform case for db entry
+                                text=partial_phrases[0].lower(),
+                                cased_text=partial_phrases[0],
                                 category=ArtifactCategory[key],
-                                count=int(objs[2]),
+                                count=int(partial_phrases[2]),
                             )
                         )
         return artifacts
 
 
 @dataclass
 class Segment:
```

### Comparing `decision-utils-0.0.5/src/decision_utils/utils/annex.py` & `decision_utils-0.0.6/src/decision_utils/utils/annex.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_utils/utils/courts.py` & `decision_utils-0.0.6/src/decision_utils/utils/courts.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_utils/utils/fallo.py` & `decision_utils-0.0.6/src/decision_utils/utils/fallo.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_utils/utils/formatter.py` & `decision_utils-0.0.6/src/decision_utils/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_utils/utils/md.py` & `decision_utils-0.0.6/src/decision_utils/utils/md.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_utils/utils/phrase.py` & `decision_utils-0.0.6/src/decision_utils/utils/phrase.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_utils/utils/regex.py` & `decision_utils-0.0.6/src/decision_utils/utils/regex.py`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_utils.egg-info/PKG-INFO` & `decision_utils-0.0.6/src/decision_utils.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: decision-utils
-Version: 0.0.5
+Version: 0.0.6
 Summary: Preprocess frontmatter-ish markdown with Philippine artifacts, statutes, citations.
 Requires-Python: >=3.11
-Requires-Dist: statute-utils>=0.6.10
+Requires-Dist: statute-utils>=0.6.11
 Requires-Dist: citation-utils>=0.4.10
 Requires-Dist: citation-title>=0.0.1
 Requires-Dist: corpus-judge>=0.1.4
-Requires-Dist: python-frontmatter>=1.1.0
 Requires-Dist: environs>=10.3
-Requires-Dist: watchdog>=3.0
-Requires-Dist: beautifulsoup4>=4.12.3
 Requires-Dist: markdownify>=0.11.6
-Requires-Dist: httpx>=0.26.0
+Requires-Dist: httpx>=0.27.0
 Requires-Dist: html-sanitizer>=2.3.0
+Requires-Dist: beautifulsoup4>=4.12.3
+Requires-Dist: watchdog>=3.0
+Requires-Dist: python-frontmatter>=1.1.0
 Requires-Dist: rich>=13.7
 Provides-Extra: dev
 Requires-Dist: ipykernel>=6.29; extra == "dev"
-Requires-Dist: pytest>=8.0; extra == "dev"
+Requires-Dist: pytest>=8.2; extra == "dev"
 Requires-Dist: pytest-cov>=4.1; extra == "dev"
-Requires-Dist: sqlite-utils>=3.36; extra == "dev"
 Requires-Dist: build>=1.0.3; extra == "dev"
 Requires-Dist: twine>=4.0.2; extra == "dev"
```

### Comparing `decision-utils-0.0.5/src/decision_utils.egg-info/SOURCES.txt` & `decision_utils-0.0.6/src/decision_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `decision-utils-0.0.5/src/decision_watcher/__main__.py` & `decision_utils-0.0.6/src/decision_watcher/__main__.py`

 * *Files identical despite different names*

