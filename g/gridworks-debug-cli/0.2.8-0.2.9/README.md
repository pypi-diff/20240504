# Comparing `tmp/gridworks_debug_cli-0.2.8.tar.gz` & `tmp/gridworks_debug_cli-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_debug_cli-0.2.8.tar", max compression
+gzip compressed data, was "gridworks_debug_cli-0.2.9.tar", max compression
```

## Comparing `gridworks_debug_cli-0.2.8.tar` & `gridworks_debug_cli-0.2.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1073 2023-05-09 19:31:30.050498 gridworks_debug_cli-0.2.8/LICENSE
--rw-r--r--   0        0        0     4476 2023-05-09 19:31:30.050498 gridworks_debug_cli-0.2.8/README.md
--rw-r--r--   0        0        0     2375 2023-05-09 19:31:48.446355 gridworks_debug_cli-0.2.8/pyproject.toml
--rw-r--r--   0        0        0       27 2023-05-09 19:31:30.054498 gridworks_debug_cli-0.2.8/src/gwdcli/__init__.py
--rw-r--r--   0        0        0      467 2023-05-09 19:31:30.054498 gridworks_debug_cli-0.2.8/src/gwdcli/__main__.py
--rw-r--r--   0        0        0       63 2023-05-09 19:31:30.054498 gridworks_debug_cli-0.2.8/src/gwdcli/csv/__init__.py
--rw-r--r--   0        0        0     2880 2023-05-09 19:31:30.054498 gridworks_debug_cli-0.2.8/src/gwdcli/csv/__main__.py
--rw-r--r--   0        0        0    11313 2023-05-09 19:31:30.054498 gridworks_debug_cli-0.2.8/src/gwdcli/csv/egauge_download.py
--rw-r--r--   0        0        0     3939 2023-05-09 19:31:30.054498 gridworks_debug_cli-0.2.8/src/gwdcli/csv/settings.py
--rw-r--r--   0        0        0       66 2023-05-09 19:31:30.054498 gridworks_debug_cli-0.2.8/src/gwdcli/events/__init__.py
--rw-r--r--   0        0        0     6808 2023-05-09 19:31:48.446355 gridworks_debug_cli-0.2.8/src/gwdcli/events/__main__.py
--rw-r--r--   0        0        0     9281 2023-05-09 19:31:30.054498 gridworks_debug_cli-0.2.8/src/gwdcli/events/models.py
--rw-r--r--   0        0        0     4578 2023-05-09 19:31:30.054498 gridworks_debug_cli-0.2.8/src/gwdcli/events/mqtt.py
--rw-r--r--   0        0        0     1429 2023-05-09 19:31:30.054498 gridworks_debug_cli-0.2.8/src/gwdcli/events/queue_loop.py
--rw-r--r--   0        0        0     3763 2023-05-09 19:31:48.450355 gridworks_debug_cli-0.2.8/src/gwdcli/events/settings.py
--rw-r--r--   0        0        0     1936 2023-05-09 19:31:30.054498 gridworks_debug_cli-0.2.8/src/gwdcli/events/show_dir.py
--rw-r--r--   0        0        0     5768 2023-05-09 19:31:30.054498 gridworks_debug_cli-0.2.8/src/gwdcli/events/sync.py
--rw-r--r--   0        0        0    20408 2023-05-09 19:31:48.450355 gridworks_debug_cli-0.2.8/src/gwdcli/events/tui.py
--rw-r--r--   0        0        0        0 2023-05-09 19:31:30.054498 gridworks_debug_cli-0.2.8/src/gwdcli/py.typed
--rw-r--r--   0        0        0        0 2023-05-09 19:31:30.054498 gridworks_debug_cli-0.2.8/src/gwdcli/utils/__init__.py
--rw-r--r--   0        0        0      509 2023-05-09 19:31:30.054498 gridworks_debug_cli-0.2.8/src/gwdcli/utils/settings.py
--rw-r--r--   0        0        0     5835 1970-01-01 00:00:00.000000 gridworks_debug_cli-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-10-16 14:44:19.324080 gridworks_debug_cli-0.2.9/LICENSE
+-rw-r--r--   0        0        0     4476 2023-10-16 14:44:19.324080 gridworks_debug_cli-0.2.9/README.md
+-rw-r--r--   0        0        0     2375 2023-10-16 14:44:36.632392 gridworks_debug_cli-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-10-16 14:44:19.324080 gridworks_debug_cli-0.2.9/src/gwdcli/__init__.py
+-rw-r--r--   0        0        0      467 2023-10-16 14:44:19.324080 gridworks_debug_cli-0.2.9/src/gwdcli/__main__.py
+-rw-r--r--   0        0        0       63 2023-10-16 14:44:19.324080 gridworks_debug_cli-0.2.9/src/gwdcli/csv/__init__.py
+-rw-r--r--   0        0        0     2880 2023-10-16 14:44:19.328081 gridworks_debug_cli-0.2.9/src/gwdcli/csv/__main__.py
+-rw-r--r--   0        0        0    11313 2023-10-16 14:44:19.328081 gridworks_debug_cli-0.2.9/src/gwdcli/csv/egauge_download.py
+-rw-r--r--   0        0        0     3939 2023-10-16 14:44:19.328081 gridworks_debug_cli-0.2.9/src/gwdcli/csv/settings.py
+-rw-r--r--   0        0        0       66 2023-10-16 14:44:19.328081 gridworks_debug_cli-0.2.9/src/gwdcli/events/__init__.py
+-rw-r--r--   0        0        0     6808 2023-10-16 14:44:19.328081 gridworks_debug_cli-0.2.9/src/gwdcli/events/__main__.py
+-rw-r--r--   0        0        0     9281 2023-10-16 14:44:19.328081 gridworks_debug_cli-0.2.9/src/gwdcli/events/models.py
+-rw-r--r--   0        0        0     4578 2023-10-16 14:44:19.328081 gridworks_debug_cli-0.2.9/src/gwdcli/events/mqtt.py
+-rw-r--r--   0        0        0     1429 2023-10-16 14:44:19.328081 gridworks_debug_cli-0.2.9/src/gwdcli/events/queue_loop.py
+-rw-r--r--   0        0        0     3763 2023-10-16 14:44:19.328081 gridworks_debug_cli-0.2.9/src/gwdcli/events/settings.py
+-rw-r--r--   0        0        0     1936 2023-10-16 14:44:19.328081 gridworks_debug_cli-0.2.9/src/gwdcli/events/show_dir.py
+-rw-r--r--   0        0        0     5768 2023-10-16 14:44:19.328081 gridworks_debug_cli-0.2.9/src/gwdcli/events/sync.py
+-rw-r--r--   0        0        0    20465 2023-10-16 14:44:36.632392 gridworks_debug_cli-0.2.9/src/gwdcli/events/tui.py
+-rw-r--r--   0        0        0        0 2023-10-16 14:44:19.328081 gridworks_debug_cli-0.2.9/src/gwdcli/py.typed
+-rw-r--r--   0        0        0        0 2023-10-16 14:44:19.328081 gridworks_debug_cli-0.2.9/src/gwdcli/utils/__init__.py
+-rw-r--r--   0        0        0      509 2023-10-16 14:44:19.328081 gridworks_debug_cli-0.2.9/src/gwdcli/utils/settings.py
+-rw-r--r--   0        0        0     5835 1970-01-01 00:00:00.000000 gridworks_debug_cli-0.2.9/PKG-INFO
```

### Comparing `gridworks_debug_cli-0.2.8/LICENSE` & `gridworks_debug_cli-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.8/README.md` & `gridworks_debug_cli-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.8/pyproject.toml` & `gridworks_debug_cli-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks-debug-cli"
-version = "0.2.8"
+version = "0.2.9"
 description = "Gridworks Debug Cli"
 authors = ["Andrew Schweitzer <schweitz72@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/anschweitzer/gridworks-debug-cli"
 repository = "https://github.com/anschweitzer/gridworks-debug-cli"
 documentation = "https://gridworks-debug-cli.readthedocs.io"
```

### Comparing `gridworks_debug_cli-0.2.8/src/gwdcli/csv/__main__.py` & `gridworks_debug_cli-0.2.9/src/gwdcli/csv/__main__.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.8/src/gwdcli/csv/egauge_download.py` & `gridworks_debug_cli-0.2.9/src/gwdcli/csv/egauge_download.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.8/src/gwdcli/csv/settings.py` & `gridworks_debug_cli-0.2.9/src/gwdcli/csv/settings.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.8/src/gwdcli/events/__main__.py` & `gridworks_debug_cli-0.2.9/src/gwdcli/events/__main__.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.8/src/gwdcli/events/models.py` & `gridworks_debug_cli-0.2.9/src/gwdcli/events/models.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.8/src/gwdcli/events/mqtt.py` & `gridworks_debug_cli-0.2.9/src/gwdcli/events/mqtt.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.8/src/gwdcli/events/queue_loop.py` & `gridworks_debug_cli-0.2.9/src/gwdcli/events/queue_loop.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.8/src/gwdcli/events/settings.py` & `gridworks_debug_cli-0.2.9/src/gwdcli/events/settings.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.8/src/gwdcli/events/show_dir.py` & `gridworks_debug_cli-0.2.9/src/gwdcli/events/show_dir.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.8/src/gwdcli/events/sync.py` & `gridworks_debug_cli-0.2.9/src/gwdcli/events/sync.py`

 * *Files identical despite different names*

### Comparing `gridworks_debug_cli-0.2.8/src/gwdcli/events/tui.py` & `gridworks_debug_cli-0.2.9/src/gwdcli/events/tui.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,14 +125,15 @@
                 date_parser=functools.partial(pd.to_datetime, utc=True),
             )
         else:
             self.df = pd.DataFrame(
                 index=pd.DatetimeIndex([], name="TimeNS"),
                 columns=["MessageId", "Src", "TypeName", "other_fields"],
             )
+            self.df.to_csv(self.settings.paths.csv_path)
         self.df.drop_duplicates("MessageId", inplace=True)
         self.live_history_df = self.df.head(0)
         self.display_df = self.extract_display_df()
         self.queue = queue.Queue()
         self.gwd_text = Text()
         self.sync_spinners = SyncSpinners()
         # noinspection PyTypeChecker
```

### Comparing `gridworks_debug_cli-0.2.8/PKG-INFO` & `gridworks_debug_cli-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridworks-debug-cli
-Version: 0.2.8
+Version: 0.2.9
 Summary: Gridworks Debug Cli
 Home-page: https://github.com/anschweitzer/gridworks-debug-cli
 License: MIT
 Author: Andrew Schweitzer
 Author-email: schweitz72@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

