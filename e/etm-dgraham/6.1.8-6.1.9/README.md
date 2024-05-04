# Comparing `tmp/etm-dgraham-6.1.8.tar.gz` & `tmp/etm-dgraham-6.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etm-dgraham-6.1.8.tar", last modified: Wed Feb  7 11:41:54 2024, max compression
+gzip compressed data, was "etm-dgraham-6.1.9.tar", last modified: Mon Feb 12 22:21:34 2024, max compression
```

## Comparing `etm-dgraham-6.1.8.tar` & `etm-dgraham-6.1.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-02-07 11:41:54.178340 etm-dgraham-6.1.8/
--rw-r--r--   0 dag        (501) staff       (20)     7567 2024-02-07 11:41:51.000000 etm-dgraham-6.1.8/CHANGES.txt
--rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-6.1.8/MANIFEST.in
--rw-r--r--   0 dag        (501) staff       (20)   140381 2024-02-07 11:41:54.178119 etm-dgraham-6.1.8/PKG-INFO
--rw-r--r--   0 dag        (501) staff       (20)   138812 2024-01-29 15:51:27.000000 etm-dgraham-6.1.8/README.md
--rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-6.1.8/_config.yml
--rwxr-xr-x   0 dag        (501) staff       (20)     4096 2024-01-10 16:26:22.000000 etm-dgraham-6.1.8/bump.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-02-07 11:41:54.171823 etm-dgraham-6.1.8/docs/
--rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-6.1.8/docs/index_konnections.md
--rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-6.1.8/docs/index_usedtime.md
--rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-6.1.8/docs/multiple_timers.md
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-02-07 11:41:54.174426 etm-dgraham-6.1.8/etm/
--rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-6.1.8/etm/__init__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    17070 2024-01-22 11:20:38.000000 etm-dgraham-6.1.8/etm/__main__.py
--rwxr-xr-x   0 dag        (501) staff       (20)       17 2024-02-07 11:41:51.000000 etm-dgraham-6.1.8/etm/__version__.py
--rw-r--r--   0 dag        (501) staff       (20)     9349 2024-02-05 12:23:30.000000 etm-dgraham-6.1.8/etm/common.py
--rwxr-xr-x   0 dag        (501) staff       (20)    12489 2024-02-05 12:23:30.000000 etm-dgraham-6.1.8/etm/data.py
--rwxr-xr-x   0 dag        (501) staff       (20)     8766 2024-02-07 11:41:51.000000 etm-dgraham-6.1.8/etm/make_examples.py
--rwxr-xr-x   0 dag        (501) staff       (20)   324270 2024-02-07 11:41:51.000000 etm-dgraham-6.1.8/etm/model.py
--rwxr-xr-x   0 dag        (501) staff       (20)    36361 2024-01-31 11:55:08.000000 etm-dgraham-6.1.8/etm/options.py
--rwxr-xr-x   0 dag        (501) staff       (20)    27874 2024-01-31 11:55:08.000000 etm-dgraham-6.1.8/etm/report.py
--rwxr-xr-x   0 dag        (501) staff       (20)   122662 2024-02-07 11:41:51.000000 etm-dgraham-6.1.8/etm/view.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-02-07 11:41:54.176553 etm-dgraham-6.1.8/etm_dgraham.egg-info/
--rw-r--r--   0 dag        (501) staff       (20)   140381 2024-02-07 11:41:54.000000 etm-dgraham-6.1.8/etm_dgraham.egg-info/PKG-INFO
--rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-6.1.8/etm_dgraham.egg-info/PKG-INFO [conflicted]
--rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-6.1.8/etm_dgraham.egg-info/SOURCES [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      882 2024-02-07 11:41:54.000000 etm-dgraham-6.1.8/etm_dgraham.egg-info/SOURCES.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        1 2024-02-07 11:41:54.000000 etm-dgraham-6.1.8/etm_dgraham.egg-info/dependency_links.txt
--rwxrwxrwx   0 dag        (501) staff       (20)       71 2024-02-07 11:41:54.000000 etm-dgraham-6.1.8/etm_dgraham.egg-info/entry_points.txt
--rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-6.1.8/etm_dgraham.egg-info/requires [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      300 2024-02-07 11:41:54.000000 etm-dgraham-6.1.8/etm_dgraham.egg-info/requires.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-6.1.8/etm_dgraham.egg-info/top_level [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2024-02-07 11:41:54.000000 etm-dgraham-6.1.8/etm_dgraham.egg-info/top_level.txt
--rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-6.1.8/etmlogo.png
--rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-6.1.8/etmlogo_small.png
--rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-6.1.8/etmview_agenda.png
--rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-6.1.8/namedcolors.py
--rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-6.1.8/new.png
--rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-6.1.8/requirements.txt
--rw-r--r--   0 dag        (501) staff       (20)       38 2024-02-07 11:41:54.178387 etm-dgraham-6.1.8/setup.cfg
--rwxr-xr-x   0 dag        (501) staff       (20)     4952 2024-01-10 16:01:12.000000 etm-dgraham-6.1.8/setup.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-02-07 11:41:54.176674 etm-dgraham-6.1.8/test/
--rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-6.1.8/test/test_parser.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-02-07 11:41:54.177611 etm-dgraham-6.1.8/utilities/
--rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-6.1.8/utilities/colons_to_slashes.py
--rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-6.1.8/utilities/etm_in
--rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-6.1.8/utilities/inbasket
--rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-6.1.8/utilities/open_in_mutt
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-02-12 22:21:34.142033 etm-dgraham-6.1.9/
+-rw-r--r--   0 dag        (501) staff       (20)     8135 2024-02-12 22:21:30.000000 etm-dgraham-6.1.9/CHANGES.txt
+-rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-6.1.9/MANIFEST.in
+-rw-r--r--   0 dag        (501) staff       (20)   140381 2024-02-12 22:21:34.141804 etm-dgraham-6.1.9/PKG-INFO
+-rw-r--r--   0 dag        (501) staff       (20)   138812 2024-01-29 15:51:27.000000 etm-dgraham-6.1.9/README.md
+-rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-6.1.9/_config.yml
+-rwxr-xr-x   0 dag        (501) staff       (20)     4096 2024-01-10 16:26:22.000000 etm-dgraham-6.1.9/bump.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-02-12 22:21:34.135781 etm-dgraham-6.1.9/docs/
+-rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-6.1.9/docs/index_konnections.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-6.1.9/docs/index_usedtime.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-6.1.9/docs/multiple_timers.md
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-02-12 22:21:34.137919 etm-dgraham-6.1.9/etm/
+-rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-6.1.9/etm/__init__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    17070 2024-01-22 11:20:38.000000 etm-dgraham-6.1.9/etm/__main__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)       17 2024-02-12 22:21:30.000000 etm-dgraham-6.1.9/etm/__version__.py
+-rw-r--r--   0 dag        (501) staff       (20)     9349 2024-02-05 12:23:30.000000 etm-dgraham-6.1.9/etm/common.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    12489 2024-02-05 12:23:30.000000 etm-dgraham-6.1.9/etm/data.py
+-rwxr-xr-x   0 dag        (501) staff       (20)     9226 2024-02-12 22:21:30.000000 etm-dgraham-6.1.9/etm/make_examples.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   324721 2024-02-12 22:21:30.000000 etm-dgraham-6.1.9/etm/model.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    36709 2024-02-12 22:21:30.000000 etm-dgraham-6.1.9/etm/options.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    27874 2024-01-31 11:55:08.000000 etm-dgraham-6.1.9/etm/report.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   122890 2024-02-12 22:21:30.000000 etm-dgraham-6.1.9/etm/view.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-02-12 22:21:34.140161 etm-dgraham-6.1.9/etm_dgraham.egg-info/
+-rw-r--r--   0 dag        (501) staff       (20)   140381 2024-02-12 22:21:34.000000 etm-dgraham-6.1.9/etm_dgraham.egg-info/PKG-INFO
+-rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-6.1.9/etm_dgraham.egg-info/PKG-INFO [conflicted]
+-rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-6.1.9/etm_dgraham.egg-info/SOURCES [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      882 2024-02-12 22:21:34.000000 etm-dgraham-6.1.9/etm_dgraham.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        1 2024-02-12 22:21:34.000000 etm-dgraham-6.1.9/etm_dgraham.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)       71 2024-02-12 22:21:34.000000 etm-dgraham-6.1.9/etm_dgraham.egg-info/entry_points.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-6.1.9/etm_dgraham.egg-info/requires [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      300 2024-02-12 22:21:34.000000 etm-dgraham-6.1.9/etm_dgraham.egg-info/requires.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-6.1.9/etm_dgraham.egg-info/top_level [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2024-02-12 22:21:34.000000 etm-dgraham-6.1.9/etm_dgraham.egg-info/top_level.txt
+-rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-6.1.9/etmlogo.png
+-rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-6.1.9/etmlogo_small.png
+-rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-6.1.9/etmview_agenda.png
+-rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-6.1.9/namedcolors.py
+-rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-6.1.9/new.png
+-rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-6.1.9/requirements.txt
+-rw-r--r--   0 dag        (501) staff       (20)       38 2024-02-12 22:21:34.142068 etm-dgraham-6.1.9/setup.cfg
+-rwxr-xr-x   0 dag        (501) staff       (20)     4952 2024-01-10 16:01:12.000000 etm-dgraham-6.1.9/setup.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-02-12 22:21:34.140272 etm-dgraham-6.1.9/test/
+-rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-6.1.9/test/test_parser.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-02-12 22:21:34.141355 etm-dgraham-6.1.9/utilities/
+-rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-6.1.9/utilities/colons_to_slashes.py
+-rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-6.1.9/utilities/etm_in
+-rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-6.1.9/utilities/inbasket
+-rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-6.1.9/utilities/open_in_mutt
```

### Comparing `etm-dgraham-6.1.8/CHANGES.txt` & `etm-dgraham-6.1.9/CHANGES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,33 @@
-2024-02-07 b8481c1 Daniel Graham
+2024-02-12 34ef252 Daniel Graham
+    Tagged version 6.1.9.
+
+2024-02-12 6059ead Daniel Graham
+    corrected erroneous change to __version__.py
+
+2024-02-12 ba39b1c Daniel Graham
+    In row2id, skip 'wrapper' rows. When creating @K inbox entries
+    insure that 'created' is added. In populating konnections_from and
+    konnections_to, make sure that doc_ids correspond to existing data
+    entries. Added focus_on_click and search_field to details_area.
+    Require is_not_editing for 'k' binding in showing_konnections.
+    Changed menu name for 'J' to 'jot it down'.
+
+2024-02-09 0caec39 Daniel Graham
+    Simplified format for journal daily. No @s entry, take the
+    datetime from the summary. Format @d with weekday, long format
+    datetime and then modified norg headings for hour:minute entry
+    timestamps. Remove extra linebread in jinsa template for @d.
+
+2024-02-08 dcf36bd Daniel Graham
+    <enter> toggles showing details leaving text_area in focus. When
+    details is showing, up|down moves selection to previous|next item
+    and shows details for the current selection.
+
+2024-02-07 5e819fc Daniel Graham
     Tagged version 6.1.8.
 
 2024-02-07 415aec7 Daniel Graham
     Fixed bug in processing keyvals in text_changed.
 
 2024-02-05 d44dba2 Daniel Graham
     Tagged version 6.1.7.
@@ -207,24 +232,7 @@
     Tagged version 6.0.6. Fixes for bump.py.
 
 2024-01-10 ecd332f Daniel Graham
     More bump tweaks.
 
 2024-01-10 7ded0b3 Daniel Graham
     restored bump.py changes
-
-2024-01-10 e61af52 Daniel Graham
-    Tagged version 6.0.5. Testing update procedure and tagging.
-
-2024-01-10 e460628 Daniel Graham
-    Tagged version 6.0.4. Back to master and working in github - etm 6
-    is now the official and only release
-
-2024-01-10 a3c1111 Daniel Graham
-    Fixed CHANGES.txt
-
-2024-01-10 b1312df Daniel Graham
-    bump fix
-
-2024-01-10 e239fa6 Daniel Graham
-    Tagged version 6.0.4. Github modifications: master6 -> master;
-    working6 -> working. etm 6 is now the official (and only) release.
```

### Comparing `etm-dgraham-6.1.8/PKG-INFO` & `etm-dgraham-6.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 6.1.8
+Version: 6.1.9
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `etm-dgraham-6.1.8/README.md` & `etm-dgraham-6.1.9/README.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.1.8/bump.py` & `etm-dgraham-6.1.9/bump.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.1.8/docs/index_konnections.md` & `etm-dgraham-6.1.9/docs/index_konnections.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.1.8/docs/index_usedtime.md` & `etm-dgraham-6.1.9/docs/index_usedtime.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.1.8/docs/multiple_timers.md` & `etm-dgraham-6.1.9/docs/multiple_timers.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.1.8/etm/__main__.py` & `etm-dgraham-6.1.9/etm/__main__.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.1.8/etm/common.py` & `etm-dgraham-6.1.9/etm/common.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.1.8/etm/data.py` & `etm-dgraham-6.1.9/etm/data.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.1.8/etm/make_examples.py` & `etm-dgraham-6.1.9/etm/make_examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,20 @@
     return ' '.join(words).rstrip()
 
 
 def word():
     return lorem.sentence()[:-1].split(' ')[0]
 
 
+def note_time():
+    hour = random.choice(range(6, 18))
+    minute = random.choice(range(0, 60))
+    return f'{hour:02}:{minute:02}'
+
+
 def days_or_weeks():
     return random.choice(['d', 'w'])
 
 
 freq = [
     '@r w',
     '@r w &w MO, WE, FR',
@@ -152,15 +158,18 @@
         f"""\
 ! README @t lorem @d .
 1) This inbox item and each of the other {num_items+len(examples)} internally generated reminders is tagged 'lorem'. All of them can be removed in one step by opening query view (press 'q'), entering the query 'any t lorem | remove' and pressing 'return'.
 2). The examples are generated to fit within a period including the week they were generated together with 5 subsequent and 6 previous weeks. You can remove and regenerate them whenever you like to keep them current.\
 """
     )
 
-    for _ in range(num_items):
+    daily = []
+
+    while len(examples) < num_items:
+        # for _ in range(num_items):
         t = random.choice(types)
         summary = phrase()
         start = random.choice(datetimes)
         end = random.choice(datetimes)
         date = random.choice(dates)
         s = (
             start.strftime('%Y-%m-%d')
@@ -186,15 +195,21 @@
                 e = start.strftime('%Y-%m-%d')
             else:
                 e = (start + timedelta(minutes=u)).strftime('%Y-%m-%d %I:%M%p')
             if start < now:
                 used += f'@u {u}m: {e} '
 
         if t == '%' and start <= now:
-            examples.append(f'{t} {summary} @s {s} @i #daily @d {d} @t lorem')
+            summary = start.strftime('%Y-%m-%d')
+            if summary not in daily:
+                daily.append(summary)
+                description = start.strftime('%A, %B %-d %Y')
+                examples.append(
+                    f'{t} {summary} @i #daily @t lorem @d {description}\n\n* {note_time()}\n  - {phrase()}'
+                )
 
         elif t == '*':
             if date:      # an event
                 examples.append(
                     f'{t} {summary} @s {s} @t {random.choice(tags)} @t lorem'
                 )
             else:
```

### Comparing `etm-dgraham-6.1.8/etm/model.py` & `etm-dgraham-6.1.9/etm/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,14 +82,15 @@
 def sortprd(prd):
     # assumes prd is a Period
     return prd.start.strftime('%Y%m%d%H%M')
 
 
 PHONE_REGEX = re.compile(r'[0-9]{10}@.*')
 KONNECT_REGEX = re.compile(r'^.+:\s+(\d+)\s*$')
+YMD_REGEX = re.compile(r'[0-9]{4}-[0-9]{2}-[0-9]{2}')  # 4-digit year - 2-digit month - 2-digit month day
 
 # The style sheet for terminal output
 style = Style.from_dict(
     {
         'plain': '#fffafa',
         'selection': '#fffafa',
         'inbox': '#ff00ff',
@@ -862,14 +863,16 @@
             self.db.insert(Document(self.item_hsh, doc_id=self.doc_id))
         except Exception as e:
             logger.debug(f"exception: {e}")
         return True
 
     def do_insert(self):
         # timer_insert = TimeIt('***INSERT***')
+        if 'created' not in self.item_hsh:
+            self.item_hsh['created'] = datetime.now().astimezone()
         doc_id = self.db.insert(self.item_hsh)
         # timer_insert.stop()
         return doc_id
 
     def edit_item(self, doc_id=None, entry=''):
         if not (doc_id and entry):
             return None
@@ -2696,15 +2699,16 @@
                     )
                     if self.compact:
                         tmp = f'{indent}{leaf[0]} {rhc}{summary}{flags}'
                     else:
                         tmp = f'{indent}{leaf[0]} {rhc}{summary}{flags}'
 
                     self.output.append(tmp)
-                    self.row2id[self.row] = leaf[4]
+                    if leaf[0] not in [wrapbefore, wrapafter]:
+                        self.row2id[self.row] = leaf[4]
                     self.row += 1
                     if len(leaf) > 5:
                         lines = self.leaf_detail(leaf[5], depth)
                         for line in lines:
                             self.output.append(line)
                             self.row += 1
             depth -= 1
@@ -3003,21 +3007,22 @@
         """
         to_hsh: ID -> ids of items with @k ID
         from_hsh ID -> ids in @k
         """
         self.konnections_to = {}
         self.konnections_from = {}
         self.konnected = []
-
+        all_ids = [item.doc_id for item in self.db]
         for item in self.db:
             doc_id = item.doc_id
             if 'k' in item and item['k']:
                 for id in item['k']:
-                    self.konnections_from.setdefault(doc_id, []). append(id)
-                    self.konnections_to.setdefault(id, []).append(doc_id)
+                    if id in all_ids:
+                        self.konnections_from.setdefault(doc_id, []). append(id)
+                        self.konnections_to.setdefault(id, []).append(doc_id)
         konnected = [x for x in self.konnections_to] + [
             x for x in self.konnections_from
         ]
         self.konnected = list(set(konnected))
         self.konnected.sort()
         row = 0
         for id in self.konnected:
@@ -4899,15 +4904,16 @@
 @o {{ h['o'] }}{% endif %} \
 {% endif %}\
 {% for k in ['+', '-'] %}\
 {% if k in h and h[k] %}
 @{{ k }} {{ nowrap(dtlst2str(h[k])) }} \
 {%- endif %}\
 {%- endfor %}\
-{% if 'd' in h %}
+{% if 'd' in h %}\
+
 @d {{ nowrap(h['d'], 0) }} \
 {% endif -%}
 {%- if 'j' in h %}\
 {%- for x in h['j'] %}\
 {%- set job -%}\
 {{ x['j'] }}\
 {%- for k in ['s', 'e'] -%}
@@ -5005,21 +5011,22 @@
 @r {{ wrap(rrule) }} \
 {% endif -%}\
 {%- endfor %}\
 {% if 'o' in h %}\
 @o {{ h['o'] }}{% endif %} \
 {% endif %}\
 {% for k in ['+', '-'] %}\
-{% if k in h and h[k] %}
-@{{ k }} {{ wrap(dtlst2str(h[k])) }} \
+{% if k in h and h[k] %}\
+@{{ k }} {{ wrap(dtlst2str(h[k])) }}\
 {%- endif %}\
 {%- endfor %}\
-{% if 'd' in h %}
+{% if 'd' in h %}\
+
 @d {{ wrap(h['d'], 0) }} \
-{% endif -%}
+{% endif -%}\
 {%- if 'j' in h %}\
 {%- for x in h['j'] %}\
 {%- set job -%}\
 {{ x['j'] }}\
 {%- for k in ['s', 'e'] -%}
 {%- if k in x and x[k] %} {{ "&{} {}".format(k, in2str(x[k])) }}{% endif %}\
 {%- endfor %}
@@ -7419,17 +7426,18 @@
         rows.append(
             {
                 'sort': dt,
                 'path': year,
                 'values': [itemtype, summary, flags, rhc, doc_id],
             }
         )
-    if len(rows) == 1:
-        ok, res = rows[0]
-        return item_details(res), {}
+    # if len(rows) == 1:
+    #     logger.debug(f"rows[0]: {rows[0]}")
+    #     res = rows[0]
+    #     return item_details(res), {}
 
     rdict = NDict()
     path = f'query: {text[:summary_width]}{item_count}'
     for row in rows:
         values = row['values']
         rdict.add(path, values)
     tree, row2id = rdict.as_tree(rdict, level=0)
@@ -7825,43 +7833,50 @@
     konnected=[],
     timers={},
 ):
     """
     journal grouped by index entry
     """
     rows = []
+    journal_name = settings.get('journal_name')
     for item in db:
-        doc_id = item.doc_id
-        if item['itemtype'] != '%':
+        itemtype = item.get('itemtype')
+        if itemtype != '%':
             continue
-        s = item.get('s', None)
+        doc_id = item.doc_id
+        summary = item.get('summary')
+        index = item.get('i', '~')
+
+        if YMD_REGEX.match(summary) and index == journal_name:
+            DAILY = True
+            s = parse_datetime(summary)[1]
+        else:
+            DAILY = False
+            s = item.get('s', None)
         if s:
             ss = date_to_datetime(s).timestamp()
             year = s.strftime("%Y")
             month = s.strftime("%B")
         else:
             ss = 0.0
             year = month = ''
-        index = item.get('i', '~')
+
         if s:
-            if index == settings['journal_name']:
+            if DAILY:
                 # this is a 'daily' entry
                 # sort = (index, -int(s.strftime('%Y')), -int(s.strftime('%m')), -int(s.strftime('%d')))
-                sort = (index, -ss, item['summary'])
+                sort = (index, -ss, summary)
                 path = f'{index}/{year}/{month}'
-                # summary = s.strftime(settings['journal_summary'])
-                ok, summary = format_date(s,separator='-',omit_zeros=False)
             else:
-                sort = (index, ss, item['summary'])
+                sort = (index, ss, summary)
                 path = index
-                summary = f"{item['summary']}"
         else:
             sort = (index, ss, item['summary'])
             path = index
-            summary = f"{item['summary']}"
+
 
         itemtype = item['itemtype']
         flags = get_flags(
             doc_id, repeat_list, link_list, konnected, pinned_list, timers
         )
         rows.append(
             {
```

### Comparing `etm-dgraham-6.1.8/etm/options.py` & `etm-dgraham-6.1.9/etm/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,15 +207,15 @@
         'pw': '',
     }
     locations = ''
     queries = {'lorem': 'any t lorem | remove'}
     style = 'dark'
     type_colors = ''
     window_colors = ''
-    journal_name = '# daily'
+    journal_name = '#daily'
 
     # use these to format the template
     settings_hsh = {
         'ampm': ampm,
         'show_minutes': show_minutes,
         'dayfirst': dayfirst,
         'yearfirst': yearfirst,
@@ -241,15 +241,14 @@
         'smtp': dict2yaml(smtp),
         'locations': dict2yaml(locations),
         'queries': dict2yaml(queries),
         'style': style,
         'type_colors': dict2yaml(type_colors),  # user modifications only
         'window_colors': dict2yaml(window_colors),  # user modifications only
         'journal_name': journal_name,
-        'journal_summary': '%a %-d',
         'etmversion': etmversion,
     }
 
     template = """\
 #### begin cfg.yaml ####
 etmversion: {etmversion}
 # The current version of etm and this file. DO NOT EDIT. This is
@@ -390,36 +389,37 @@
 # 0, 1, 6, 12, 30 or 60. This setting only affects how used times are
 # reported - with 0, no rounding up is done, with 1 times are rounded up
 # to the nearest minute, with 6 times are rounded up to the nearest 0.1 of
 # an hour, with 12 to the nearest 0.2 of an hour and so forth.  E.g., with
 # usedtime_minutes = 12, a used time entry of 15 minutes would be rounded
 # up to the nearest multiple of 12 or to 24 minutes = 0.4 hours for
 # reporting in the used time views. This setting does not affect how the
-# times are recorded but only how they are reported in used time views.
+# times are recorded but only how they are reported in usedtime views.
 
 usedtime_hours: {usedtime_hours}
 # 0, 1, 2, ..., 24. The daily goal for used time. This is used in
 # effort view to control the display of the daily used time bars. The
 # goal is to to maximize the granularity of the bar when displaying
 # this number of hours in the space allowed by the terminal width so
 # that, e.g., with a goal of 6 the used time bar for the day would
 # take all of the available space when the actual used time spent is 6
 # or more hours.
 
 journal_name: '{journal_name}'
-# Journal items with this index entry and with an @s entry will have
-# the year and month appended to the index. E.g., with the setting
-#   journal_name: '# daily'
+# Journal items with this index entry and with a summary in 'yyyy-mm-dd'
+# format will have the year and month appended to the index. E.g., with
+# the setting
+#   journal_name: '#daily'
 # this journal entry
-#   % visited Yellowstone @s 22/10/24 @i # daily
+#   % 2022/10/24 @i #daily
 # would be displayed in journal view as if the index entry were
 #   @i # daily/2022/10
 # thus organizing such entries by the year and month and, within each
-# month, also by the month day. The '#' places '# daily' near the top
-# in journal with daily entries sorted in reverse order so that the
+# month, by the month day. The '#' places '#daily' near the top in
+# journal with daily entries sorted in reverse order so that the
 # most recent entries are always at the top.
 #
 # Pressing 'J' in any view will open a daily journal entry for the
 # current date with a summary corresponding to the current date and
 # an index entry equal to {journal_name}. This journal entry will be
 # created if necessary.
 
@@ -515,18 +515,25 @@
 # values. Each "query" must be one that could be entered as the
 # command in query view. Keys can be any short string other than
 # 'a', 'u', 'c' or 'l' which are already in use.
 # queries:
 #    td: m l -q equals itemtype - and ~exists f
 #    mi: exists u and ~exists i
 #    arch: a exists itemtype
-#    find: includes summary d {{}}
-# The latter would allow you to enter, e.g., `find waldo` and have
+#    lorem: any t lorem | remove
+#    daily: in i {journal_name} and in d {{}}
+#    find: in summary d {{}}
+# 'find' would allow you to enter, e.g., `find waldo` and have
 # it expand to `includes summary d waldo` and thus locate all
 # reminders with `waldo` either in the summary or d (the description).
+# 'lorem' would identify every item that has 'lorem' as a tag and
+# remove them - thus deleting all the lorem examples. 'daily' would
+# allow you to enter, e.g., 'daily whatever' and have it expand to
+# `in i {journal_name} and in d whatever` thus identifying every
+# daily note that contains 'whatever' in the description.
 
 style: {style}
 # dark or light. Set the defaults for dark or light terminal
 # backgounds. Some output may not be visible unless this is set
 # correctly for your display.
 
 type_colors: {type_colors}
```

### Comparing `etm-dgraham-6.1.8/etm/report.py` & `etm-dgraham-6.1.9/etm/report.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.1.8/etm/view.py` & `etm-dgraham-6.1.9/etm/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -1995,15 +1995,16 @@
 
 
 details_area = TextArea(
     text='',
     style='class:details',
     read_only=True,
     scrollbar=True,
-    search_field=None,
+    focus_on_click=True,
+    search_field=search_field,
 )
 
 
 busy_area = TextArea(
     text='',
     style='class:details',
     read_only=True,
@@ -2511,81 +2512,76 @@
     md, wd = d.split(', ')
     return f"{model.ordinal(int(md))}, {wd}"
 
 @bindings.add('J', filter=is_viewing & is_items_table)
 def edit_or_add_journal(*event):
     global item
     global starting_buffer_text
+    now = datetime.now()
     app = get_app()
     app.editing_mode = (
         EditingMode.VI if settings['vi_mode'] else EditingMode.EMACS
     )
 
     if dataview.is_showing_details:
         application.layout.focus(text_area)
         dataview.hide_details()
 
     # to restore the current cursor row after completed
     dataview.current_row = text_area.document.cursor_position_row
     dataview.is_editing = True
     dataview.control_z_active = False
-    summary_fmt = settings['journal_summary']
+    # summary_fmt = settings['journal_summary']
 
     journal_name = settings.get('journal_name')
     doc_id, entry = dataview.get_details(
         text_area.document.cursor_position_row, True
     )
-    summary = model.format_date(datetime.today(), separator='-', omit_zeros=False)[1]
+    # summary = model.format_date(datetime.today(), separator='-', omit_zeros=False)[1]
+    summary = now.strftime("%Y-%m-%d")
     relevant = None
     for it in ETMDB:
-        itemtype = it.get('itemtype')
-        index = it.get('i')
-        start = it.get('s')
-        if isinstance(start, datetime):
-            start = start.date()
-        logger.debug(f"itemtype: {itemtype}; index: {index}; journal_name: {journal_name}; start: {start}; today: {today.date()}")
-        if itemtype == '%' and index == journal_name and start and start == date.today():
+        if it.get('itemtype') != '%':
+            continue
+        if it.get('i') != journal_name:
+            continue
+        if it.get('summary') == summary:
             relevant = it
             break
     logger.debug(f"relevant: {relevant}")
-    doc_id, entry = dataview.get_details(
-        text_area.document.cursor_position_row, True
-    )
     if relevant:
         doc_id = relevant.doc_id
-        relevant['summary'] = summary
         entry = item_details(relevant, True)
         item.edit_item(doc_id, entry)
         edit_buffer.text = item.entry
         starting_buffer_text = item.entry
         default_buffer_changed(event)
         default_cursor_position_changed(event)
         application.layout.focus(edit_buffer)
     else:
-        start = datetime.today().strftime("%Y-%m-%d")
         starting_buffer_text = ""
         template = f"""\
 % {summary}
-@s {start} @i {settings['journal_name']}
-@d --
-* {today.strftime('%A, %B %-d, %Y')}\
+@i {journal_name}
+@d {now.strftime('%A, %B %-d, %Y')}\
 """
         item.new_item()
         default_buffer_changed(event)
         default_cursor_position_changed(event)
         application.layout.focus(edit_buffer)
         edit_buffer.text = template
-    edit_buffer.text = f"{edit_buffer.text}\n\n** {datetime.now().strftime('%H:%M')}\n   "
+    # cursor_right below will move over just to the end of '\n   - '
+    edit_buffer.text = f"{edit_buffer.text}\n\n* {now.strftime('%H:%M')}\n  - "
     starting_buffer_text = edit_buffer.text
     lines_in_buffer = len(edit_buffer.text.split('\n'))
     position = edit_buffer.document.get_end_of_document_position()
     logger.debug(f"end_of_document: {position}; lines: {lines_in_buffer}")
     for i in range(lines_in_buffer):
         edit_buffer.cursor_down()
-    for i in range(3):
+    for i in range(4):
         edit_buffer.cursor_right()
 
     # edit_buffer.cursor_position = position
 
 
 
 @bindings.add('E', filter=is_viewing_or_details & is_item_view)
@@ -3395,30 +3391,30 @@
 
 @bindings.add('r', filter=is_viewing)
 def review_view(*event):
     set_view('r')
 
 
 
-@bindings.add('k', filter=is_viewing & is_not_showing_konnected)
+@bindings.add('k', filter=is_viewing & is_not_showing_konnected & is_not_editing)
 def konnected_view(*event):
     doc_id, entry = dataview.get_details(
         text_area.document.cursor_position_row, True
     )
     # id2row = {id: row for row, id in dataview.konnections_row2id.items()}
     konnected_row = dataview.konnected_id2row.get(doc_id, None)
     # logger.debug(f"doc_id: {doc_id}; konnected_row: {konnected_row}; dataview.konnected_id2row: {dataview.konnected_id2row}")
     set_view('k')
     if konnected_row:
         text_area.buffer.cursor_position = (
             text_area.buffer.document.translate_row_col_to_index(
                 konnected_row, 0)
             )
 
-@bindings.add('k', filter=is_showing_konnected & is_not_showing_konnections)
+@bindings.add('k', filter=is_showing_konnected & is_not_showing_konnections & is_not_editing)
 def get_konnections(*event):
     if not dataview.active_view == 'konnected':
         return
 
     selected_id = dataview.get_details(text_area.document.cursor_position_row)[
         0
     ]
@@ -3589,14 +3585,20 @@
             else row2id[next_row]
         )
     else:
         next_id = '?'
     text_area.buffer.cursor_position = (
         text_area.buffer.document.translate_row_col_to_index(next_row, 0)
     )
+    if is_showing_details():
+        tmp = dataview.get_details(text_area.document.cursor_position_row)[1]
+        if tmp:
+            dataview.show_details()
+            details_area.text = tmp.rstrip()
+            application.layout.focus(text_area)
 
 
 @bindings.add('up', filter=is_not_busy_view & is_not_yearly_view & is_viewing)
 def previous_id(*event):
     row2id = dataview.row2id
     if not row2id:
         return
@@ -3615,14 +3617,20 @@
             else row2id[next_row]
         )
     else:
         next_id = '?'
     text_area.buffer.cursor_position = (
         text_area.buffer.document.translate_row_col_to_index(next_row, 0)
     )
+    if is_showing_details():
+        tmp = dataview.get_details(text_area.document.cursor_position_row)[1]
+        if tmp:
+            dataview.show_details()
+            details_area.text = tmp.rstrip()
+            application.layout.focus(text_area)
 
 
 @bindings.add('c-p', filter=is_viewing)
 def next_pinned(*event):
     """
     Move the cursor to the next row corresponding to a pinned id if there is such a row and to row 0 otherwise.
     """
@@ -3747,15 +3755,15 @@
         application.layout.focus(text_area)
         dataview.hide_details()
     else:
         tmp = dataview.get_details(text_area.document.cursor_position_row)[1]
         if tmp:
             dataview.show_details()
             details_area.text = tmp.rstrip()
-            application.layout.focus(details_area)
+            application.layout.focus(text_area)
 
 
 @bindings.add(
     'enter',
     filter=is_showing_konnections & is_not_querying)
 def show_details(*event):
     if dataview.is_showing_details:
@@ -3977,15 +3985,15 @@
                 MenuItem('^p) go to next pinned item', handler=next_pinned),
             ],
         ),
         MenuItem(
             'edit',
             children=[
                 MenuItem('+) add new item', handler=edit_new),
-                MenuItem('J) edit today\'s journal entry', handler=edit_or_add_journal),
+                MenuItem('J) jot it down', handler=edit_or_add_journal),
                 MenuItem('-', disabled=True),
                 MenuItem('^g) test goto link', handler=do_goto),
                 MenuItem('^r) show repetitions', handler=is_editing_reps),
                 MenuItem('^s) save changes & close', handler=save_changes),
                 MenuItem('^z) discard changes & close', handler=close_edit),
             ],
         ),
```

### Comparing `etm-dgraham-6.1.8/etm_dgraham.egg-info/PKG-INFO` & `etm-dgraham-6.1.9/etm_dgraham.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 6.1.8
+Version: 6.1.9
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `etm-dgraham-6.1.8/etm_dgraham.egg-info/PKG-INFO [conflicted]` & `etm-dgraham-6.1.9/etm_dgraham.egg-info/PKG-INFO [conflicted]`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.1.8/etm_dgraham.egg-info/SOURCES.txt` & `etm-dgraham-6.1.9/etm_dgraham.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.1.8/etmlogo.png` & `etm-dgraham-6.1.9/etmlogo.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.1.8/etmlogo_small.png` & `etm-dgraham-6.1.9/etmlogo_small.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.1.8/etmview_agenda.png` & `etm-dgraham-6.1.9/etmview_agenda.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.1.8/namedcolors.py` & `etm-dgraham-6.1.9/namedcolors.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.1.8/new.png` & `etm-dgraham-6.1.9/new.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.1.8/setup.py` & `etm-dgraham-6.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.1.8/test/test_parser.py` & `etm-dgraham-6.1.9/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.1.8/utilities/colons_to_slashes.py` & `etm-dgraham-6.1.9/utilities/colons_to_slashes.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.1.8/utilities/etm_in` & `etm-dgraham-6.1.9/utilities/etm_in`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.1.8/utilities/inbasket` & `etm-dgraham-6.1.9/utilities/inbasket`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.1.8/utilities/open_in_mutt` & `etm-dgraham-6.1.9/utilities/open_in_mutt`

 * *Files identical despite different names*

