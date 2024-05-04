# Comparing `tmp/lytils-0.1.7.tar.gz` & `tmp/lytils-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lytils-0.1.7.tar", max compression
+gzip compressed data, was "lytils-0.1.8.tar", max compression
```

## Comparing `lytils-0.1.7.tar` & `lytils-0.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11558 2024-04-10 19:18:21.187313 lytils-0.1.7/LICENSE
--rw-r--r--   0        0        0      111 2024-02-21 21:27:17.496125 lytils-0.1.7/lytils/__init__.py
--rw-r--r--   0        0        0     2766 2024-03-11 19:56:01.645968 lytils-0.1.7/lytils/app.py
--rw-r--r--   0        0        0       56 2023-08-27 21:31:43.244103 lytils-0.1.7/lytils/classes/__init__.py
--rw-r--r--   0        0        0      926 2023-08-27 22:42:07.795890 lytils-0.1.7/lytils/classes/Regex.py
--rw-r--r--   0        0        0     1220 2024-04-29 06:18:46.279205 lytils-0.1.7/lytils/common.py
--rw-r--r--   0        0        0       36 2023-10-16 01:49:34.901392 lytils-0.1.7/lytils/discord/__init__.py
--rw-r--r--   0        0        0     4534 2024-04-10 19:21:06.136630 lytils-0.1.7/lytils/discord/DiscordBot.py
--rw-r--r--   0        0        0       37 2024-04-04 00:00:24.647508 lytils-0.1.7/lytils/email/__init__.py
--rw-r--r--   0        0        0     2384 2024-04-12 07:06:16.170788 lytils-0.1.7/lytils/email/Email.py
--rw-r--r--   0        0        0     1829 2024-04-30 07:52:51.978200 lytils-0.1.7/lytils/file.py
--rw-r--r--   0        0        0      127 2024-05-01 06:20:57.735715 lytils-0.1.7/lytils/google_sheets/__init__.py
--rw-r--r--   0        0        0      550 2024-01-30 18:05:03.141133 lytils-0.1.7/lytils/google_sheets/Column.py
--rw-r--r--   0        0        0     3672 2024-02-22 21:29:15.946213 lytils-0.1.7/lytils/google_sheets/format.py
--rw-r--r--   0        0        0      610 2024-05-01 07:07:48.459412 lytils-0.1.7/lytils/google_sheets/GoogleSheets.py
--rw-r--r--   0        0        0      308 2024-04-10 19:21:06.136630 lytils-0.1.7/lytils/google_sheets/helpers.py
--rw-r--r--   0        0        0      265 2024-05-01 06:59:31.597206 lytils-0.1.7/lytils/google_sheets/Sheet.py
--rw-r--r--   0        0        0     7541 2024-04-18 01:07:42.696739 lytils-0.1.7/lytils/google_sheets/Tab.py
--rw-r--r--   0        0        0      653 2024-01-23 06:16:04.647379 lytils-0.1.7/lytils/input.py
--rw-r--r--   0        0        0      616 2024-03-12 00:24:52.524374 lytils-0.1.7/lytils/logging.py
--rw-r--r--   0        0        0     1048 2023-12-31 07:36:14.446133 lytils-0.1.7/lytils/print.py
--rw-r--r--   0        0        0      419 2024-02-25 07:04:04.187197 lytils-0.1.7/lytils/regex.py
--rw-r--r--   0        0        0     1253 2024-04-12 07:03:04.806336 lytils-0.1.7/lytils/surfshark.py
--rw-r--r--   0        0        0      318 2024-05-01 07:08:17.479302 lytils-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       47 2024-04-10 19:18:21.187313 lytils-0.1.7/README.md
--rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 lytils-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11558 2024-04-10 19:18:21.187313 lytils-0.1.8/LICENSE
+-rw-r--r--   0        0        0       87 2024-05-04 01:51:31.649310 lytils-0.1.8/lytils/__init__.py
+-rw-r--r--   0        0        0     2766 2024-03-11 19:56:01.645968 lytils-0.1.8/lytils/app.py
+-rw-r--r--   0        0        0       56 2023-08-27 21:31:43.244103 lytils-0.1.8/lytils/classes/__init__.py
+-rw-r--r--   0        0        0      926 2023-08-27 22:42:07.795890 lytils-0.1.8/lytils/classes/Regex.py
+-rw-r--r--   0        0        0     1220 2024-04-29 06:18:46.279205 lytils-0.1.8/lytils/common.py
+-rw-r--r--   0        0        0       36 2023-10-16 01:49:34.901392 lytils-0.1.8/lytils/discord/__init__.py
+-rw-r--r--   0        0        0     4534 2024-04-10 19:21:06.136630 lytils-0.1.8/lytils/discord/DiscordBot.py
+-rw-r--r--   0        0        0       37 2024-04-04 00:00:24.647508 lytils-0.1.8/lytils/email/__init__.py
+-rw-r--r--   0        0        0     2384 2024-04-12 07:06:16.170788 lytils-0.1.8/lytils/email/Email.py
+-rw-r--r--   0        0        0     1902 2024-05-04 01:19:41.529249 lytils-0.1.8/lytils/file.py
+-rw-r--r--   0        0        0      127 2024-05-01 06:20:57.735715 lytils-0.1.8/lytils/google_sheets/__init__.py
+-rw-r--r--   0        0        0      550 2024-01-30 18:05:03.141133 lytils-0.1.8/lytils/google_sheets/Column.py
+-rw-r--r--   0        0        0     3672 2024-02-22 21:29:15.946213 lytils-0.1.8/lytils/google_sheets/format.py
+-rw-r--r--   0        0        0      610 2024-05-01 07:07:48.459412 lytils-0.1.8/lytils/google_sheets/GoogleSheets.py
+-rw-r--r--   0        0        0      308 2024-04-10 19:21:06.136630 lytils-0.1.8/lytils/google_sheets/helpers.py
+-rw-r--r--   0        0        0      265 2024-05-01 06:59:31.597206 lytils-0.1.8/lytils/google_sheets/Sheet.py
+-rw-r--r--   0        0        0     7541 2024-04-18 01:07:42.696739 lytils-0.1.8/lytils/google_sheets/Tab.py
+-rw-r--r--   0        0        0      653 2024-01-23 06:16:04.647379 lytils-0.1.8/lytils/input.py
+-rw-r--r--   0        0        0     4387 2024-05-04 01:50:40.726122 lytils-0.1.8/lytils/logger.py
+-rw-r--r--   0        0        0     1048 2023-12-31 07:36:14.446133 lytils-0.1.8/lytils/print.py
+-rw-r--r--   0        0        0      419 2024-02-25 07:04:04.187197 lytils-0.1.8/lytils/regex.py
+-rw-r--r--   0        0        0     1253 2024-04-12 07:03:04.806336 lytils-0.1.8/lytils/surfshark.py
+-rw-r--r--   0        0        0      318 2024-05-04 01:52:16.922152 lytils-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       47 2024-04-10 19:18:21.187313 lytils-0.1.8/README.md
+-rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 lytils-0.1.8/PKG-INFO
```

### Comparing `lytils-0.1.7/LICENSE` & `lytils-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lytils-0.1.7/lytils/app.py` & `lytils-0.1.8/lytils/app.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.7/lytils/classes/Regex.py` & `lytils-0.1.8/lytils/classes/Regex.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.7/lytils/common.py` & `lytils-0.1.8/lytils/common.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.7/lytils/discord/DiscordBot.py` & `lytils-0.1.8/lytils/discord/DiscordBot.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.7/lytils/email/Email.py` & `lytils-0.1.8/lytils/email/Email.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.7/lytils/file.py` & `lytils-0.1.8/lytils/file.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,36 +35,39 @@
     """
     with open(path, "w") as file:
         json.dump(data, file, indent=indent)
 
 
 class LyFile:
     def __init__(self, path: str = "LyFile/file.txt"):
-        self.path = path
+        self._path = path
+
+    def exists(self):
+        return os.path.exists(self._path)
 
     def create(self):
         """
         Creates a blank file at path.
         """
         # Split path into directory and filename
-        directory, _ = os.path.split(self.path)
+        directory, _ = os.path.split(self._path)
 
         # If directory was included, create it if it doesn't exist
         if directory and not os.path.exists(directory):
             os.makedirs(directory)
 
-        open(self.path, "w").close()  # Create file
+        open(self._path, "w").close()  # Create file
 
     def append(self, text):
         """
         Appends text to file at path.
         """
-        with open(self.path, "a") as file:
+        with open(self._path, "a") as file:
             file.write(f"{text}\n")
 
     def append_json(self, data, indent: int = 4):
         """
         Appends json data to file at path.
         """
-        with open(self.path, "a") as file:
+        with open(self._path, "a") as file:
             json.dump(data, file, indent=indent)
             file.write("\n")
```

### Comparing `lytils-0.1.7/lytils/google_sheets/Column.py` & `lytils-0.1.8/lytils/google_sheets/Column.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.7/lytils/google_sheets/format.py` & `lytils-0.1.8/lytils/google_sheets/format.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.7/lytils/google_sheets/GoogleSheets.py` & `lytils-0.1.8/lytils/google_sheets/GoogleSheets.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.7/lytils/google_sheets/Tab.py` & `lytils-0.1.8/lytils/google_sheets/Tab.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.7/lytils/input.py` & `lytils-0.1.8/lytils/input.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.7/lytils/print.py` & `lytils-0.1.8/lytils/print.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.7/lytils/surfshark.py` & `lytils-0.1.8/lytils/surfshark.py`

 * *Files identical despite different names*

