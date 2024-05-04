# Comparing `tmp/ao3statscraper-0.1.4.tar.gz` & `tmp/ao3statscraper-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ao3statscraper-0.1.4.tar", last modified: Thu May  2 13:09:12 2024, max compression
+gzip compressed data, was "ao3statscraper-0.1.7.tar", last modified: Sat May  4 13:52:31 2024, max compression
```

## Comparing `ao3statscraper-0.1.4.tar` & `ao3statscraper-0.1.7.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-05-02 13:09:12.195262 ao3statscraper-0.1.4/
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)    35137 2024-04-10 17:46:52.000000 ao3statscraper-0.1.4/LICENSE
--rw-r--r--   0 mivkov    (1000) mivkov    (1000)    48957 2024-05-02 13:09:12.195262 ao3statscraper-0.1.4/PKG-INFO
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     7554 2024-05-02 13:08:38.000000 ao3statscraper-0.1.4/README.md
-drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-05-02 13:09:12.195262 ao3statscraper-0.1.4/ao3statscraper/
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      523 2024-04-24 14:13:41.000000 ao3statscraper-0.1.4/ao3statscraper/__init__.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       22 2024-05-02 13:08:38.000000 ao3statscraper-0.1.4/ao3statscraper/__version__.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     2425 2024-05-02 13:08:38.000000 ao3statscraper-0.1.4/ao3statscraper/ao3requester.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     8351 2024-05-02 13:08:38.000000 ao3statscraper-0.1.4/ao3statscraper/configuration.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     6530 2024-04-24 14:13:41.000000 ao3statscraper-0.1.4/ao3statscraper/plotting.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     3862 2024-04-24 14:13:41.000000 ao3statscraper-0.1.4/ao3statscraper/pw.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     8015 2024-04-24 22:00:25.000000 ao3statscraper-0.1.4/ao3statscraper/scrape.py
-drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-05-02 13:09:12.195262 ao3statscraper-0.1.4/ao3statscraper/scripts/
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      177 2024-04-24 14:13:41.000000 ao3statscraper-0.1.4/ao3statscraper/scripts/__init__.py
--rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)      905 2024-04-24 14:13:41.000000 ao3statscraper-0.1.4/ao3statscraper/scripts/ao3_hits_to_kudos.py
--rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)     3234 2024-04-24 21:11:36.000000 ao3statscraper-0.1.4/ao3statscraper/scripts/ao3_purge_stats_data.py
--rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)     3660 2024-04-24 21:10:58.000000 ao3statscraper-0.1.4/ao3statscraper/scripts/ao3plot.py
--rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)     3961 2024-05-02 13:08:38.000000 ao3statscraper-0.1.4/ao3statscraper/scripts/ao3scrape.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)    11255 2024-04-24 14:13:41.000000 ao3statscraper-0.1.4/ao3statscraper/statsdata.py
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     1396 2024-04-24 14:13:41.000000 ao3statscraper-0.1.4/ao3statscraper/utils.py
-drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-05-02 13:09:12.195262 ao3statscraper-0.1.4/ao3statscraper.egg-info/
--rw-r--r--   0 mivkov    (1000) mivkov    (1000)    48957 2024-05-02 13:09:12.000000 ao3statscraper-0.1.4/ao3statscraper.egg-info/PKG-INFO
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      754 2024-05-02 13:09:12.000000 ao3statscraper-0.1.4/ao3statscraper.egg-info/SOURCES.txt
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)        1 2024-05-02 13:09:12.000000 ao3statscraper-0.1.4/ao3statscraper.egg-info/dependency_links.txt
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      263 2024-05-02 13:09:12.000000 ao3statscraper-0.1.4/ao3statscraper.egg-info/entry_points.txt
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      119 2024-05-02 13:09:12.000000 ao3statscraper-0.1.4/ao3statscraper.egg-info/requires.txt
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       15 2024-05-02 13:09:12.000000 ao3statscraper-0.1.4/ao3statscraper.egg-info/top_level.txt
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     1630 2024-05-02 13:08:38.000000 ao3statscraper-0.1.4/pyproject.toml
--rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       38 2024-05-02 13:09:12.195262 ao3statscraper-0.1.4/setup.cfg
-drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-05-02 13:09:12.195262 ao3statscraper-0.1.4/tests/
--rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)      933 2024-04-24 14:13:41.000000 ao3statscraper-0.1.4/tests/test_passwords.py
--rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)      642 2024-04-24 14:13:41.000000 ao3statscraper-0.1.4/tests/test_writing_data.py
+drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-05-04 13:52:31.768155 ao3statscraper-0.1.7/
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)    35137 2024-04-10 17:46:52.000000 ao3statscraper-0.1.7/LICENSE
+-rw-r--r--   0 mivkov    (1000) mivkov    (1000)    49444 2024-05-04 13:52:31.768155 ao3statscraper-0.1.7/PKG-INFO
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     8041 2024-05-04 13:52:09.000000 ao3statscraper-0.1.7/README.md
+drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-05-04 13:52:31.764155 ao3statscraper-0.1.7/ao3statscraper/
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      554 2024-05-04 13:52:09.000000 ao3statscraper-0.1.7/ao3statscraper/__init__.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       22 2024-05-04 13:52:25.000000 ao3statscraper-0.1.7/ao3statscraper/__version__.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     2425 2024-05-02 13:08:38.000000 ao3statscraper-0.1.7/ao3statscraper/ao3requester.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     8351 2024-05-04 13:52:09.000000 ao3statscraper-0.1.7/ao3statscraper/configuration.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     6530 2024-04-24 14:13:41.000000 ao3statscraper-0.1.7/ao3statscraper/plotting.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     3862 2024-04-24 14:13:41.000000 ao3statscraper-0.1.7/ao3statscraper/pw.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     8015 2024-04-24 22:00:25.000000 ao3statscraper-0.1.7/ao3statscraper/scrape.py
+drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-05-04 13:52:31.764155 ao3statscraper-0.1.7/ao3statscraper/scripts/
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      200 2024-05-04 13:52:09.000000 ao3statscraper-0.1.7/ao3statscraper/scripts/__init__.py
+-rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)      932 2024-05-04 13:52:09.000000 ao3statscraper-0.1.7/ao3statscraper/scripts/ao3_hits_to_kudos.py
+-rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)     3328 2024-05-04 13:52:09.000000 ao3statscraper-0.1.7/ao3statscraper/scripts/ao3_purge_stats_data.py
+-rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)     4505 2024-05-04 13:52:09.000000 ao3statscraper-0.1.7/ao3statscraper/scripts/ao3diff.py
+-rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)     4264 2024-05-04 13:52:09.000000 ao3statscraper-0.1.7/ao3statscraper/scripts/ao3get.py
+-rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)     3682 2024-05-04 13:52:09.000000 ao3statscraper-0.1.7/ao3statscraper/scripts/ao3plot.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     9019 2024-05-04 13:52:09.000000 ao3statscraper-0.1.7/ao3statscraper/statsdata.py
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     1396 2024-04-24 14:13:41.000000 ao3statscraper-0.1.7/ao3statscraper/utils.py
+drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-05-04 13:52:31.768155 ao3statscraper-0.1.7/ao3statscraper.egg-info/
+-rw-r--r--   0 mivkov    (1000) mivkov    (1000)    49444 2024-05-04 13:52:31.000000 ao3statscraper-0.1.7/ao3statscraper.egg-info/PKG-INFO
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      785 2024-05-04 13:52:31.000000 ao3statscraper-0.1.7/ao3statscraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)        1 2024-05-04 13:52:31.000000 ao3statscraper-0.1.7/ao3statscraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      298 2024-05-04 13:52:31.000000 ao3statscraper-0.1.7/ao3statscraper.egg-info/entry_points.txt
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)      119 2024-05-04 13:52:31.000000 ao3statscraper-0.1.7/ao3statscraper.egg-info/requires.txt
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       15 2024-05-04 13:52:31.000000 ao3statscraper-0.1.7/ao3statscraper.egg-info/top_level.txt
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)     1666 2024-05-04 13:52:25.000000 ao3statscraper-0.1.7/pyproject.toml
+-rw-rw-r--   0 mivkov    (1000) mivkov    (1000)       38 2024-05-04 13:52:31.768155 ao3statscraper-0.1.7/setup.cfg
+drwxrwxr-x   0 mivkov    (1000) mivkov    (1000)        0 2024-05-04 13:52:31.768155 ao3statscraper-0.1.7/tests/
+-rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)      933 2024-04-24 14:13:41.000000 ao3statscraper-0.1.7/tests/test_passwords.py
+-rwxrwxr-x   0 mivkov    (1000) mivkov    (1000)      642 2024-04-24 14:13:41.000000 ao3statscraper-0.1.7/tests/test_writing_data.py
```

### Comparing `ao3statscraper-0.1.4/LICENSE` & `ao3statscraper-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.1.4/PKG-INFO` & `ao3statscraper-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ao3statscraper
-Version: 0.1.4
+Version: 0.1.7
 Summary: Scrape stats from your AO3 stats page.
 Author-email: Lars Ikarion <lars.ikarion@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -757,19 +757,20 @@
 stored in a separate file from your work statistics.
 
 
 
 ### Getting Started
 
 The main use case for `AO3StatScraper` is to fetch and display your current AO3
-statistics using scripts provided by `AO3StatScraper`. Currently, there are 4
+statistics using scripts provided by `AO3StatScraper`. Currently, there are 5
 scripts:
 
 - `ao3get` : The main script to fetch and display your AO3 stats.
 - `ao3plot`: Plots the stats stored with `ao3get`.
+- `ao3diff`: Show the difference in stats compared to an earlier date.
 - `ao3_hits_to_kudos`: List all your works in ascending order of their
   hits/kudos ratio
 - `ao3_purge`: Deletes saved stats such that there is a minumum time between the
   remaining ones
 
 The scripts are discussed in more detail further below.
 
@@ -834,14 +835,25 @@
 It is possible that the stats graphs aren't displayed nicely on all screens. If
 that is the case for you, you may want to try the `--no-prettify` flag to obtain
 a bare-bones plot without any prettifications. It may not look as nice, but at
 least you should be able to see the data.
 
 
 
+### `ao3diff`
+
+Fetch (but do not store) your AO3 stats and compare them to stats from the past.
+It never stores snapshots itself, you will need to do that using `ao3get`.
+By default, it will compare to your stats from a week ago, but you can also
+select a day, a week, a month, or a year back using the `-d`, `-w`, `-m`, or `-y`
+flag, respectively. Alternately, you can specify a date in the `YYYY-MM-DD`
+format.
+
+
+
 ### `ao3_hits_to_kudos`
 
 This script just reads in the last stored snapshot and prints out all your works
 in ascending order of their hits/kudos ratio.
```

### Comparing `ao3statscraper-0.1.4/README.md` & `ao3statscraper-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,19 +56,20 @@
 stored in a separate file from your work statistics.
 
 
 
 ### Getting Started
 
 The main use case for `AO3StatScraper` is to fetch and display your current AO3
-statistics using scripts provided by `AO3StatScraper`. Currently, there are 4
+statistics using scripts provided by `AO3StatScraper`. Currently, there are 5
 scripts:
 
 - `ao3get` : The main script to fetch and display your AO3 stats.
 - `ao3plot`: Plots the stats stored with `ao3get`.
+- `ao3diff`: Show the difference in stats compared to an earlier date.
 - `ao3_hits_to_kudos`: List all your works in ascending order of their
   hits/kudos ratio
 - `ao3_purge`: Deletes saved stats such that there is a minumum time between the
   remaining ones
 
 The scripts are discussed in more detail further below.
 
@@ -133,14 +134,25 @@
 It is possible that the stats graphs aren't displayed nicely on all screens. If
 that is the case for you, you may want to try the `--no-prettify` flag to obtain
 a bare-bones plot without any prettifications. It may not look as nice, but at
 least you should be able to see the data.
 
 
 
+### `ao3diff`
+
+Fetch (but do not store) your AO3 stats and compare them to stats from the past.
+It never stores snapshots itself, you will need to do that using `ao3get`.
+By default, it will compare to your stats from a week ago, but you can also
+select a day, a week, a month, or a year back using the `-d`, `-w`, `-m`, or `-y`
+flag, respectively. Alternately, you can specify a date in the `YYYY-MM-DD`
+format.
+
+
+
 ### `ao3_hits_to_kudos`
 
 This script just reads in the last stored snapshot and prints out all your works
 in ascending order of their hits/kudos ratio.
```

### Comparing `ao3statscraper-0.1.4/ao3statscraper/__init__.py` & `ao3statscraper-0.1.7/ao3statscraper/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,10 +6,11 @@
 from .scrape import UserSession
 from .statsdata import StatsData, WorkStatsData, TotStatsData
 from .utils import clear_terminal
 from .plotting import plot_total_stats, plot_work_stats
 from .pw import store_secrets, read_secrets
 
 from .scripts.ao3plot import ao3plot
-from .scripts.ao3scrape import ao3scrape
+from .scripts.ao3get import ao3get
+from .scripts.ao3diff import ao3diff
 from .scripts.ao3_purge_stats_data import ao3_purge_stats_data
 from .scripts.ao3_hits_to_kudos import ao3_hits_to_kudos
```

### Comparing `ao3statscraper-0.1.4/ao3statscraper/ao3requester.py` & `ao3statscraper-0.1.7/ao3statscraper/ao3requester.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.1.4/ao3statscraper/configuration.py` & `ao3statscraper-0.1.7/ao3statscraper/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
         refresh_config = False
         # Catch versions too old to even keep track of config version
         try:
             self.store_login = confdata["Globals"]["version"]
         except KeyError:
             refresh_config = True
 
-        if Version(ao3SSversion) > min_compatible_version:
+        if Version(ao3SSversion) < min_compatible_version:
             refresh_config = True
 
         if refresh_config:
             print(
                 "ERROR: Your config file is set up for an older version of AO3StatScraper."
             )
             print("Please re-configure it using `ao3get -c`")
```

### Comparing `ao3statscraper-0.1.4/ao3statscraper/plotting.py` & `ao3statscraper-0.1.7/ao3statscraper/plotting.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.1.4/ao3statscraper/pw.py` & `ao3statscraper-0.1.7/ao3statscraper/pw.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.1.4/ao3statscraper/scrape.py` & `ao3statscraper-0.1.7/ao3statscraper/scrape.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.1.4/ao3statscraper/scripts/ao3_hits_to_kudos.py` & `ao3statscraper-0.1.7/ao3statscraper/scripts/ao3_hits_to_kudos.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 """
 Prints the hits/kudos ratio of all your works, in ascending order.
 """
 
 
 def ao3_hits_to_kudos():
     from ..configuration import Config
-    from ..statsdata import WorkStatsData, TotStatsData
+    from ..statsdata import WorkStatsData, TotStatsData, get_latest_dump_filename
 
     # Setup
     conf = Config()
 
-    wsfile = WorkStatsData.get_latest_dump_filename(conf)
+    wsfile = get_latest_dump_filename(conf, WorkStatsData)
     ws_old = WorkStatsData(conf, source=wsfile)
 
     work_data = ws_old.data
     work_data.drop_duplicates(["ID"], ignore_index=True, inplace=True)
 
     work_data["Hits/Kudos"] = 0.0
     hpk = work_data.loc[:, "Hits"] / work_data.loc[:, "Kudos"]
```

### Comparing `ao3statscraper-0.1.4/ao3statscraper/scripts/ao3_purge_stats_data.py` & `ao3statscraper-0.1.7/ao3statscraper/scripts/ao3_purge_stats_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,33 +30,38 @@
 
 
 def ao3_purge_stats_data():
     import datetime
     import os
 
     from ..configuration import Config
-    from ..statsdata import WorkStatsData, TotStatsData
+    from ..statsdata import (
+        WorkStatsData,
+        TotStatsData,
+        get_dump_file_list,
+        get_timestamp_from_filename,
+    )
 
     # Setup
     args = _parse_purge_args()
     conf = Config()
 
     # Get and check list of dump files.
-    tsfiles = TotStatsData.get_dump_file_list(conf)
-    wsfiles = WorkStatsData.get_dump_file_list(conf)
+    tsfiles = get_dump_file_list(conf, TotStatsData)
+    wsfiles = get_dump_file_list(conf, WorkStatsData)
 
     tsDummy = TotStatsData(conf, source=tsfiles[0])
     wsDummy = WorkStatsData(conf, source=wsfiles[0])
 
     times = []
 
     for i in range(len(tsfiles)):
         try:
-            tt = tsDummy.get_timestamp_from_filename(tsfiles[i])
-            tw = wsDummy.get_timestamp_from_filename(wsfiles[i])
+            tt = get_timestamp_from_filename(tsDummy, tsfiles[i])
+            tw = get_timestamp_from_filename(wsDummy, wsfiles[i])
         except IndexError:
             print("Unequal number of total stats data files and work data files")
             print("This needs special handling.")
             quit()
 
         if tt != tw:
             raise ValueError("Total and work times are not equal", tt, tw)
```

### Comparing `ao3statscraper-0.1.4/ao3statscraper/scripts/ao3plot.py` & `ao3statscraper-0.1.7/ao3statscraper/scripts/ao3plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,25 +65,25 @@
     AO3StatScraper. By default, this program will run a dialogue and ask you
     what to plot. Alternately, you can skip this dialogue by using the -t or
     the -i flags.
     """
 
     from ..plotting import plot_total_stats, plot_work_stats
     from ..configuration import Config
-    from ..statsdata import WorkStatsData, TotStatsData
+    from ..statsdata import WorkStatsData, TotStatsData, get_dump_file_list
     from ..utils import clear_terminal
 
     # Setup
     args = _parse_plotter_args()
     conf = Config()
     conf.plotting.prettify = not args.no_pretty
 
     # Get and check list of dump files.
-    tsfiles = TotStatsData.get_dump_file_list(conf)
-    wsfiles = WorkStatsData.get_dump_file_list(conf)
+    tsfiles = get_dump_file_list(conf, TotStatsData)
+    wsfiles = get_dump_file_list(conf, WorkStatsData)
 
     if len(tsfiles) == 0:
         print("Error: Found no total stats files.")
         quit()
     if len(tsfiles) == 1:
         print("Error: Found only 1 total stats file.")
         quit()
```

### Comparing `ao3statscraper-0.1.4/ao3statscraper/scripts/ao3scrape.py` & `ao3statscraper-0.1.7/ao3statscraper/scripts/ao3get.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 def _parse_scrape_args():
     """
     Setup argument parser and read cmdline args.
     """
 
     parser = argparse.ArgumentParser(
-        prog="getAO3stats.py",
+        prog="ao3get.py",
         description="Scrape your AO3 statistics.",
         epilog="The program will require you to log in to your AO3 account.",
     )
 
     parser.add_argument(
         "-a",
         "--all",
@@ -74,29 +74,34 @@
     )
 
     args = parser.parse_args()
 
     return args
 
 
-def ao3scrape():
+def ao3get():
     from ..configuration import Config
-    from ..statsdata import WorkStatsData, TotStatsData
+    from ..statsdata import (
+        WorkStatsData,
+        TotStatsData,
+        get_latest_dump_filename,
+        get_2_latest_dump_filenames,
+    )
     from ..scrape import UserSession
 
     args = _parse_scrape_args()
     conf = Config(reset_conffile=args.run_config)
 
     if args.showdir:
         print(f"Data directory is '{conf.datadir}'")
         quit()
 
     if args.remove_last:
-        tsfile = TotStatsData.get_latest_dump_filename(conf)
-        wsfile = WorkStatsData.get_latest_dump_filename(conf)
+        tsfile = get_latest_dump_filename(conf, TotStatsData)
+        wsfile = get_latest_dump_filename(conf, WorkStatsData)
 
         print(f"This will remove files {tsfile} and {wsfile}.")
         answer = input("Continue? [y/N] ")
         if answer.startswith(("y", "Y")):
             os.remove(tsfile)
             print(f"Deleted {tsfile}")
             os.remove(wsfile)
@@ -109,20 +114,22 @@
 
     if args.print_all:
         session = UserSession(conf)
         ts_new, ws_new = session.get_stats(conf)
         ts_new.print()
         ws_new.print()
         if not args.no_write:
+            # synchronize time stamp first, just in case.
+            ts_new.timestamp = ws_new.timestamp
             ts_new.dump()
             ws_new.dump()
 
     elif args.repeat:
-        tsfile1, tsfile2 = TotStatsData.get_2_latest_dump_filenames(conf)
-        wsfile1, wsfile2 = WorkStatsData.get_2_latest_dump_filenames(conf)
+        tsfile1, tsfile2 = get_2_latest_dump_filenames(conf, TotStatsData)
+        wsfile1, wsfile2 = get_2_latest_dump_filenames(conf, WorkStatsData)
 
         ts_old = TotStatsData(conf, source=tsfile1)
         ws_old = WorkStatsData(conf, source=wsfile1)
         ts_new = TotStatsData(conf, source=tsfile2)
         ws_new = WorkStatsData(conf, source=wsfile2)
 
         ts_new.diff(ts_old)
@@ -130,22 +137,24 @@
 
     elif args.diff:
         # Diff is skipped if repeat is on
 
         session = UserSession(conf)
         ts_new, ws_new = session.get_stats(conf)
 
-        tsfile = TotStatsData.get_latest_dump_filename(conf)
-        wsfile = WorkStatsData.get_latest_dump_filename(conf)
+        tsfile = get_latest_dump_filename(conf, TotStatsData)
+        wsfile = get_latest_dump_filename(conf, WorkStatsData)
         ts_old = TotStatsData(conf, source=tsfile)
         ws_old = WorkStatsData(conf, source=wsfile)
 
         ts_new.diff(ts_old)
         changes = ws_new.diff(ws_old)
 
         if changes and not args.no_write:
+            # synchronize time stamp first, just in case.
+            ts_new.timestamp = ws_new.timestamp
             ts_new.dump()
             ws_new.dump()
 
 
 if __name__ == "__main__":
-    ao3scrape()
+    ao3get()
```

### Comparing `ao3statscraper-0.1.4/ao3statscraper/statsdata.py` & `ao3statscraper-0.1.7/ao3statscraper/statsdata.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 
 import datetime
 import pandas
 import os
-from typing import Union
+from typing import Union, Type
 import tabulate
 
 from .configuration import Config
 from .utils import (
     get_datetime_from_time_string,
     get_title_output,
     colour_numeric_string,
@@ -23,82 +23,23 @@
     def __init__(self, conf: Config, data: Union[None, pandas.DataFrame] = None):
         self.timestamp = datetime.datetime.now()
         self.datadir = conf.datadir
         self.username = conf.username
         self.data = data
         return
 
-    @staticmethod
-    def generate_dump_base_name():
-        """
-        Generate the base name of the dump file for this class.
-        """
-        return (
-            WorkStatsData.dump_base_name
-            + WorkStatsData.dump_delimiter
-            + WorkStatsData.datatype
-            + WorkStatsData.dump_delimiter
-        )
-
-    @staticmethod
-    def get_dump_file_list(conf: Config):
-        """
-        Get a list of all dump files for this class of data.
-        """
-
-        datadir = conf.datadir
-        base = WorkStatsData.generate_dump_base_name()
-        ls = os.listdir(datadir)
-        candidates = []
-        for f in ls:
-            if f.startswith(base):
-                candidates.append(f)
-
-        filelist = sorted(candidates)
-
-        return [os.path.join(datadir, f) for f in filelist]
-
-    @staticmethod
-    def get_latest_dump_filename(conf: Config):
-        """
-        Find the file name of the latest snapshot.
-        Returns the path to the file as a string.
-        """
-
-        fl = StatsData.get_dump_file_list(conf)
-        if len(fl) == 0:
-            print("Error: I couldn't find any previously saved statistics files in")
-            print(f"       {conf.datadir}. If this is your first time running")
-            print("       this script, run it with the --all flag.")
-            quit(1)
-        return fl[-1]
-
-    def get_timestamp_from_filename(self, filepath: str, suffix: str = "csv"):
-        """
-        Extract the time stamp from the stats file name.
-
-        Returns: Datetime object of the time
-        """
-
-        filename = filepath.rstrip(suffix)
-        ao3stats, datatype, timestamp = filename.split(self.dump_delimiter)
-
-        t = get_datetime_from_time_string(timestamp)
-
-        return t
-
     def _generate_dump_filename(self):
         """
         Generate the file name of the dump.
         Returns the file name as a string.
         """
         t = self.timestamp
         timestamp = f"{t.year:04d}{t.month:02d}{t.day:02d}{t.hour:02d}{t.minute:02d}{t.second:02d}"
 
-        return self.generate_dump_base_name() + timestamp
+        return generate_dump_base_name(self) + timestamp
 
     def dump(self):
         """
         Dump the data this object contains into a dump file.
         """
 
         filename = self._generate_dump_filename()
@@ -108,15 +49,15 @@
         self.data.to_csv(filepath, index=False)
         return
 
     def _read(self, filepath):
         suffix = ".csv"
         self.data = pandas.read_csv(filepath)
 
-        self.timestamp = self.get_timestamp_from_filename(filepath, suffix=suffix)
+        self.timestamp = get_timestamp_from_filename(self, filepath, suffix=suffix)
 
         #  print(
         #      f"Read in stats from {t.year}-{t.month:02d}-{t.day:02d} {t.hour:02d}:{t.minute:02d}:{t.second:02d}"
         #  )
 
         return
 
@@ -147,58 +88,14 @@
             self.data = pandas.DataFrame(data)
 
         else:
             self._read(source)
 
         return
 
-    @staticmethod
-    def generate_dump_base_name():
-        """
-        Generate the base name of the dump file for this class.
-        """
-        return (
-            WorkStatsData.dump_base_name
-            + WorkStatsData.dump_delimiter
-            + WorkStatsData.datatype
-            + WorkStatsData.dump_delimiter
-        )
-
-    @staticmethod
-    def get_dump_file_list(conf: Config):
-        """
-        Get a list of all dump files for this class of data.
-        """
-
-        datadir = conf.datadir
-        base = WorkStatsData.generate_dump_base_name()
-        ls = os.listdir(datadir)
-        candidates = []
-        for f in ls:
-            if f.startswith(base):
-                candidates.append(f)
-
-        filelist = sorted(candidates)
-
-        return [os.path.join(datadir, f) for f in filelist]
-
-    @staticmethod
-    def get_latest_dump_filename(conf: Config):
-        fl = WorkStatsData.get_dump_file_list(conf)
-        return fl[-1]
-
-    @staticmethod
-    def get_2_latest_dump_filenames(conf: Config):
-        """
-        Returns older, newest
-        """
-
-        fl = WorkStatsData.get_dump_file_list(conf)
-        return fl[-2], fl[-1]
-
     def _print_database(self, data: pandas.DataFrame, columns=None):
         """
         Print out a nice table.
         Provide list of columns to print as list of strings (column keys)
         via the `columns` parameter.
         """
 
@@ -307,67 +204,14 @@
             self.data = pandas.DataFrame(data)
 
         else:
             self._read(source)
 
         return
 
-    @staticmethod
-    def generate_dump_base_name():
-        """
-        Generates the base name of dump files.
-        """
-        return (
-            TotStatsData.dump_base_name
-            + TotStatsData.dump_delimiter
-            + TotStatsData.datatype
-            + TotStatsData.dump_delimiter
-        )
-
-    @staticmethod
-    def get_dump_file_list(conf: Config):
-        """
-        Get a list of all dump files for this class of data.
-        """
-
-        datadir = conf.datadir
-        base = TotStatsData.generate_dump_base_name()
-        ls = os.listdir(datadir)
-        candidates = []
-        for f in ls:
-            if f.startswith(base):
-                candidates.append(f)
-
-        filelist = sorted(candidates)
-
-        return [os.path.join(datadir, f) for f in filelist]
-
-    @staticmethod
-    def get_latest_dump_filename(conf: Config):
-        """
-        Find the file name of the latest snapshot.
-        """
-
-        fl = TotStatsData.get_dump_file_list(conf)
-        if len(fl) == 0:
-            print("Error: I couldn't find any previously saved statistics files in")
-            print(f"       {conf.datadir}. If this is your first time running")
-            print("       this script, run it with the --all flag.")
-            quit(1)
-        return fl[-1]
-
-    @staticmethod
-    def get_2_latest_dump_filenames(conf: Config):
-        """
-        Returns older, newest
-        """
-
-        fl = TotStatsData.get_dump_file_list(conf)
-        return fl[-2], fl[-1]
-
     def _print_database(self, data: pandas.DataFrame):
         titlestr = f"Total Statistics For User {self.username}"
         title_output = get_title_output(titlestr)
 
         output = tabulate.tabulate(
             data,
             tablefmt="simple_grid",
@@ -406,7 +250,89 @@
         #  diff_str[diff < 0] = " (" + diff_str[diff < 0] + ")"
 
         new_str += diff_str_colored
 
         self._print_database(new_str)
 
         return
+
+
+def get_timestamp_from_filename(
+    st: Type[StatsData], filepath: str, suffix: str = "csv"
+):
+    """
+    Extract the time stamp from the stats file name of stats with the type StatsData.
+    st: A class of StatsData
+    filepath: the path of the file to extract timestamp from
+
+    Returns: Datetime object of the time
+    """
+
+    filename = filepath.rstrip(suffix)
+
+    ao3stats, datatype, timestamp = filename.split(st.dump_delimiter)
+
+    t = get_datetime_from_time_string(timestamp)
+
+    return t
+
+
+def generate_dump_base_name(st: Type[StatsData]):
+    """
+    Generate the base name of the dump file for a StatsData object
+    st: A class of StatsData
+
+    returns: dump base name as string
+    """
+    return st.dump_base_name + st.dump_delimiter + st.datatype + st.dump_delimiter
+
+
+def get_dump_file_list(conf: Config, st: Type[StatsData]):
+    """
+    Get a list of all written dump data files of StatsData object.
+    conf: a Config object
+    st: A class of StatsData
+
+    Returns: list of strings of paths of files
+    """
+
+    datadir = conf.datadir
+    base = generate_dump_base_name(st)
+    ls = os.listdir(datadir)
+    candidates = []
+    for f in ls:
+        if f.startswith(base):
+            candidates.append(f)
+
+    filelist = sorted(candidates)
+
+    return [os.path.join(datadir, f) for f in filelist]
+
+
+def get_latest_dump_filename(conf: Config, st: Type[StatsData]):
+    """
+    Find the file name of the latest snapshot of StatsData object.
+    conf: a Config object
+    st: A class of StatsData
+
+    Returns: the path to the file as a string.
+
+    """
+
+    fl = get_dump_file_list(conf, st)
+    if len(fl) == 0:
+        print("Error: I couldn't find any previously saved statistics files in")
+        print(f"       {conf.datadir}. If this is your first time running")
+        print("       this script, run it with the --all flag.")
+        quit(1)
+    return fl[-1]
+
+
+def get_2_latest_dump_filenames(conf: Config, st: Type[StatsData]):
+    """
+    conf: a Config object
+    st: A class of StatsData
+    Returns: 2 strings of dump file names in the order older, newest
+    """
+
+    fl = get_dump_file_list(conf, st)
+    return fl[-2], fl[-1]
```

### Comparing `ao3statscraper-0.1.4/ao3statscraper/utils.py` & `ao3statscraper-0.1.7/ao3statscraper/utils.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.1.4/ao3statscraper.egg-info/PKG-INFO` & `ao3statscraper-0.1.7/ao3statscraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ao3statscraper
-Version: 0.1.4
+Version: 0.1.7
 Summary: Scrape stats from your AO3 stats page.
 Author-email: Lars Ikarion <lars.ikarion@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -757,19 +757,20 @@
 stored in a separate file from your work statistics.
 
 
 
 ### Getting Started
 
 The main use case for `AO3StatScraper` is to fetch and display your current AO3
-statistics using scripts provided by `AO3StatScraper`. Currently, there are 4
+statistics using scripts provided by `AO3StatScraper`. Currently, there are 5
 scripts:
 
 - `ao3get` : The main script to fetch and display your AO3 stats.
 - `ao3plot`: Plots the stats stored with `ao3get`.
+- `ao3diff`: Show the difference in stats compared to an earlier date.
 - `ao3_hits_to_kudos`: List all your works in ascending order of their
   hits/kudos ratio
 - `ao3_purge`: Deletes saved stats such that there is a minumum time between the
   remaining ones
 
 The scripts are discussed in more detail further below.
 
@@ -834,14 +835,25 @@
 It is possible that the stats graphs aren't displayed nicely on all screens. If
 that is the case for you, you may want to try the `--no-prettify` flag to obtain
 a bare-bones plot without any prettifications. It may not look as nice, but at
 least you should be able to see the data.
 
 
 
+### `ao3diff`
+
+Fetch (but do not store) your AO3 stats and compare them to stats from the past.
+It never stores snapshots itself, you will need to do that using `ao3get`.
+By default, it will compare to your stats from a week ago, but you can also
+select a day, a week, a month, or a year back using the `-d`, `-w`, `-m`, or `-y`
+flag, respectively. Alternately, you can specify a date in the `YYYY-MM-DD`
+format.
+
+
+
 ### `ao3_hits_to_kudos`
 
 This script just reads in the last stored snapshot and prints out all your works
 in ascending order of their hits/kudos ratio.
```

### Comparing `ao3statscraper-0.1.4/ao3statscraper.egg-info/SOURCES.txt` & `ao3statscraper-0.1.7/ao3statscraper.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -15,11 +15,12 @@
 ao3statscraper.egg-info/dependency_links.txt
 ao3statscraper.egg-info/entry_points.txt
 ao3statscraper.egg-info/requires.txt
 ao3statscraper.egg-info/top_level.txt
 ao3statscraper/scripts/__init__.py
 ao3statscraper/scripts/ao3_hits_to_kudos.py
 ao3statscraper/scripts/ao3_purge_stats_data.py
+ao3statscraper/scripts/ao3diff.py
+ao3statscraper/scripts/ao3get.py
 ao3statscraper/scripts/ao3plot.py
-ao3statscraper/scripts/ao3scrape.py
 tests/test_passwords.py
 tests/test_writing_data.py
```

### Comparing `ao3statscraper-0.1.4/pyproject.toml` & `ao3statscraper-0.1.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 packages = ["ao3statscraper", "ao3statscraper.scripts"]
 
 
 [project]
 name = "ao3statscraper"
 description="Scrape stats from your AO3 stats page."
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.7"
 authors= [
     { name = "Lars Ikarion", email="lars.ikarion@gmail.com"},
     ]
 license = { file = "LICENSE" }
 classifiers=[
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -37,23 +37,24 @@
     "termcolor",
     ]
 
 [project.scripts]
 ao3_hits_to_kudos= "ao3statscraper.scripts:ao3_hits_to_kudos"
 ao3_purge= "ao3statscraper.scripts:ao3_purge_stats_data"
 ao3plot= "ao3statscraper.scripts:ao3plot"
-ao3scrape= "ao3statscraper.scripts:ao3scrape"
-ao3get= "ao3statscraper.scripts:ao3scrape"
+ao3scrape= "ao3statscraper.scripts:ao3get"
+ao3get= "ao3statscraper.scripts:ao3get"
+ao3diff= "ao3statscraper.scripts:ao3diff"
 
 
 [project.urls]
 "Homepage" = "https://gitlab.com/athenaslilowl1/AO3StatScraper"
 
 [tool.bumpver]
-current_version = "0.1.4"
+current_version = "0.1.7"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `ao3statscraper-0.1.4/tests/test_passwords.py` & `ao3statscraper-0.1.7/tests/test_passwords.py`

 * *Files identical despite different names*

### Comparing `ao3statscraper-0.1.4/tests/test_writing_data.py` & `ao3statscraper-0.1.7/tests/test_writing_data.py`

 * *Files identical despite different names*

