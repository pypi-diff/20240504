# Comparing `tmp/helios-client-0.4.20240424.post1.tar.gz` & `tmp/helios-client-0.4.20240503.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helios-client-0.4.20240424.post1.tar", last modified: Thu Apr 25 05:37:15 2024, max compression
+gzip compressed data, was "helios-client-0.4.20240503.post1.tar", last modified: Sat May  4 05:29:59 2024, max compression
```

## Comparing `helios-client-0.4.20240424.post1.tar` & `helios-client-0.4.20240503.post1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2024-04-25 05:37:15.123819 helios-client-0.4.20240424.post1/
--rw-rw-r--   0 kip       (1000) kip       (1000)     7652 2017-09-30 07:16:26.000000 helios-client-0.4.20240424.post1/Copying
--rw-rw-r--   0 kip       (1000) kip       (1000)       30 2019-05-23 01:39:54.000000 helios-client-0.4.20240424.post1/MANIFEST.in
--rw-rw-r--   0 kip       (1000) kip       (1000)     5833 2024-04-25 05:37:15.127819 helios-client-0.4.20240424.post1/PKG-INFO
--rw-rw-r--   0 kip       (1000) kip       (1000)     4342 2024-03-15 02:16:20.000000 helios-client-0.4.20240424.post1/README.md
-drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2024-04-25 05:37:15.119819 helios-client-0.4.20240424.post1/Source/
-drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2024-04-25 05:37:15.123819 helios-client-0.4.20240424.post1/Source/helios/
--rw-rw-r--   0 kip       (1000) kip       (1000)      228 2024-03-15 02:17:25.000000 helios-client-0.4.20240424.post1/Source/helios/__init__.py
--rw-rw-r--   0 kip       (1000) kip       (1000)      221 2024-04-25 03:28:50.000000 helios-client-0.4.20240424.post1/Source/helios/__version__.py
--rwxrwxr-x   0 kip       (1000) kip       (1000)     1457 2024-03-15 02:17:14.000000 helios-client-0.4.20240424.post1/Source/helios/chunked_upload.py
--rwxrwxr-x   0 kip       (1000) kip       (1000)    48195 2024-04-24 01:44:58.000000 helios-client-0.4.20240424.post1/Source/helios/client.py
--rwxrwxr-x   0 kip       (1000) kip       (1000)     3437 2024-03-15 02:17:21.000000 helios-client-0.4.20240424.post1/Source/helios/exceptions.py
--rwxrwxr-x   0 kip       (1000) kip       (1000)     4937 2024-04-23 01:51:01.000000 helios-client-0.4.20240424.post1/Source/helios/requests.py
--rwxrwxr-x   0 kip       (1000) kip       (1000)    12931 2024-04-17 01:46:47.000000 helios-client-0.4.20240424.post1/Source/helios/responses.py
-drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2024-04-25 05:37:15.123819 helios-client-0.4.20240424.post1/Source/helios_client.egg-info/
--rw-rw-r--   0 kip       (1000) kip       (1000)     5833 2024-04-25 05:37:14.000000 helios-client-0.4.20240424.post1/Source/helios_client.egg-info/PKG-INFO
--rw-rw-r--   0 kip       (1000) kip       (1000)      752 2024-04-25 05:37:15.000000 helios-client-0.4.20240424.post1/Source/helios_client.egg-info/SOURCES.txt
--rw-rw-r--   0 kip       (1000) kip       (1000)        1 2024-04-25 05:37:14.000000 helios-client-0.4.20240424.post1/Source/helios_client.egg-info/dependency_links.txt
--rw-rw-r--   0 kip       (1000) kip       (1000)       92 2024-04-25 05:37:14.000000 helios-client-0.4.20240424.post1/Source/helios_client.egg-info/requires.txt
--rw-rw-r--   0 kip       (1000) kip       (1000)        7 2024-04-25 05:37:14.000000 helios-client-0.4.20240424.post1/Source/helios_client.egg-info/top_level.txt
--rw-rw-r--   0 kip       (1000) kip       (1000)        1 2024-04-25 05:37:14.000000 helios-client-0.4.20240424.post1/Source/helios_client.egg-info/zip-safe
-drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2024-04-25 05:37:15.123819 helios-client-0.4.20240424.post1/debian/
--rw-rw-r--   0 kip       (1000) kip       (1000)      189 2024-04-25 04:43:34.000000 helios-client-0.4.20240424.post1/debian/changelog
--rw-rw-r--   0 kip       (1000) kip       (1000)     1174 2024-04-25 05:28:12.000000 helios-client-0.4.20240424.post1/debian/control
--rw-rw-r--   0 kip       (1000) kip       (1000)      377 2024-04-25 04:44:12.000000 helios-client-0.4.20240424.post1/debian/copyright
--rw-rw-r--   0 kip       (1000) kip       (1000)       11 2019-05-15 03:31:30.000000 helios-client-0.4.20240424.post1/debian/docs
--rw-rw-r--   0 kip       (1000) kip       (1000)      130 2024-04-25 05:27:55.000000 helios-client-0.4.20240424.post1/debian/lintian-overrides
--rwxr-xr-x   0 kip       (1000) kip       (1000)     3238 2024-03-15 02:16:39.000000 helios-client-0.4.20240424.post1/debian/rules
-drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2024-04-25 05:37:15.123819 helios-client-0.4.20240424.post1/debian/source/
--rw-rw-r--   0 kip       (1000) kip       (1000)       12 2015-01-02 04:54:06.000000 helios-client-0.4.20240424.post1/debian/source/format
--rw-rw-r--   0 kip       (1000) kip       (1000)       63 2019-09-16 23:53:59.000000 helios-client-0.4.20240424.post1/debian/source/options
-drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2024-04-25 05:37:15.127819 helios-client-0.4.20240424.post1/debian/tests/
--rw-------   0 kip       (1000) kip       (1000)      834 2024-03-15 01:22:53.000000 helios-client-0.4.20240424.post1/debian/tests/control
--rwx--x--x   0 kip       (1000) kip       (1000)      417 2024-03-15 01:09:49.000000 helios-client-0.4.20240424.post1/debian/tests/test-import-module.py
--rwx--x--x   0 kip       (1000) kip       (1000)     3768 2024-04-23 02:00:12.000000 helios-client-0.4.20240424.post1/debian/tests/test-module-usage.py
--rw-rw-r--   0 kip       (1000) kip       (1000)      214 2024-04-25 04:41:51.000000 helios-client-0.4.20240424.post1/debian/watch
--rw-rw-r--   0 kip       (1000) kip       (1000)       38 2024-04-25 05:37:15.127819 helios-client-0.4.20240424.post1/setup.cfg
--rwxrwxr-x   0 kip       (1000) kip       (1000)     3358 2024-04-07 02:31:28.000000 helios-client-0.4.20240424.post1/setup.py
+drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2024-05-04 05:29:59.155845 helios-client-0.4.20240503.post1/
+-rw-rw-r--   0 kip       (1000) kip       (1000)     7652 2017-09-30 07:16:26.000000 helios-client-0.4.20240503.post1/Copying
+-rw-rw-r--   0 kip       (1000) kip       (1000)       30 2019-05-23 01:39:54.000000 helios-client-0.4.20240503.post1/MANIFEST.in
+-rw-rw-r--   0 kip       (1000) kip       (1000)     5833 2024-05-04 05:29:59.239845 helios-client-0.4.20240503.post1/PKG-INFO
+-rw-rw-r--   0 kip       (1000) kip       (1000)     4342 2024-03-15 02:16:20.000000 helios-client-0.4.20240503.post1/README.md
+drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2024-05-04 05:29:59.155845 helios-client-0.4.20240503.post1/Source/
+drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2024-05-04 05:29:59.159844 helios-client-0.4.20240503.post1/Source/helios/
+-rw-rw-r--   0 kip       (1000) kip       (1000)      228 2024-03-15 02:17:25.000000 helios-client-0.4.20240503.post1/Source/helios/__init__.py
+-rw-rw-r--   0 kip       (1000) kip       (1000)      221 2024-05-04 00:49:13.000000 helios-client-0.4.20240503.post1/Source/helios/__version__.py
+-rwxrwxr-x   0 kip       (1000) kip       (1000)     1457 2024-03-15 02:17:14.000000 helios-client-0.4.20240503.post1/Source/helios/chunked_upload.py
+-rwxrwxr-x   0 kip       (1000) kip       (1000)    48573 2024-05-04 01:13:40.000000 helios-client-0.4.20240503.post1/Source/helios/client.py
+-rwxrwxr-x   0 kip       (1000) kip       (1000)     3437 2024-03-15 02:17:21.000000 helios-client-0.4.20240503.post1/Source/helios/exceptions.py
+-rwxrwxr-x   0 kip       (1000) kip       (1000)     4937 2024-04-23 01:51:01.000000 helios-client-0.4.20240503.post1/Source/helios/requests.py
+-rwxrwxr-x   0 kip       (1000) kip       (1000)    12931 2024-04-17 01:46:47.000000 helios-client-0.4.20240503.post1/Source/helios/responses.py
+drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2024-05-04 05:29:59.235845 helios-client-0.4.20240503.post1/Source/helios_client.egg-info/
+-rw-rw-r--   0 kip       (1000) kip       (1000)     5833 2024-05-04 05:29:58.000000 helios-client-0.4.20240503.post1/Source/helios_client.egg-info/PKG-INFO
+-rw-rw-r--   0 kip       (1000) kip       (1000)      752 2024-05-04 05:29:59.000000 helios-client-0.4.20240503.post1/Source/helios_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 kip       (1000) kip       (1000)        1 2024-05-04 05:29:58.000000 helios-client-0.4.20240503.post1/Source/helios_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 kip       (1000) kip       (1000)       92 2024-05-04 05:29:58.000000 helios-client-0.4.20240503.post1/Source/helios_client.egg-info/requires.txt
+-rw-rw-r--   0 kip       (1000) kip       (1000)        7 2024-05-04 05:29:58.000000 helios-client-0.4.20240503.post1/Source/helios_client.egg-info/top_level.txt
+-rw-rw-r--   0 kip       (1000) kip       (1000)        1 2024-05-04 05:29:58.000000 helios-client-0.4.20240503.post1/Source/helios_client.egg-info/zip-safe
+drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2024-05-04 05:29:59.239845 helios-client-0.4.20240503.post1/debian/
+-rw-rw-r--   0 kip       (1000) kip       (1000)      189 2024-05-04 00:49:40.000000 helios-client-0.4.20240503.post1/debian/changelog
+-rw-rw-r--   0 kip       (1000) kip       (1000)     1174 2024-04-25 05:28:12.000000 helios-client-0.4.20240503.post1/debian/control
+-rw-rw-r--   0 kip       (1000) kip       (1000)      377 2024-04-25 04:44:12.000000 helios-client-0.4.20240503.post1/debian/copyright
+-rw-rw-r--   0 kip       (1000) kip       (1000)       11 2019-05-15 03:31:30.000000 helios-client-0.4.20240503.post1/debian/docs
+-rw-rw-r--   0 kip       (1000) kip       (1000)      130 2024-04-25 05:27:55.000000 helios-client-0.4.20240503.post1/debian/lintian-overrides
+-rwxr-xr-x   0 kip       (1000) kip       (1000)     3238 2024-03-15 02:16:39.000000 helios-client-0.4.20240503.post1/debian/rules
+drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2024-05-04 05:29:59.239845 helios-client-0.4.20240503.post1/debian/source/
+-rw-rw-r--   0 kip       (1000) kip       (1000)       12 2015-01-02 04:54:06.000000 helios-client-0.4.20240503.post1/debian/source/format
+-rw-rw-r--   0 kip       (1000) kip       (1000)       63 2019-09-16 23:53:59.000000 helios-client-0.4.20240503.post1/debian/source/options
+drwxrwxr-x   0 kip       (1000) kip       (1000)        0 2024-05-04 05:29:59.239845 helios-client-0.4.20240503.post1/debian/tests/
+-rw-------   0 kip       (1000) kip       (1000)      834 2024-03-15 01:22:53.000000 helios-client-0.4.20240503.post1/debian/tests/control
+-rwx--x--x   0 kip       (1000) kip       (1000)      417 2024-03-15 01:09:49.000000 helios-client-0.4.20240503.post1/debian/tests/test-import-module.py
+-rwx--x--x   0 kip       (1000) kip       (1000)     5291 2024-05-04 01:33:15.000000 helios-client-0.4.20240503.post1/debian/tests/test-module-usage.py
+-rw-rw-r--   0 kip       (1000) kip       (1000)      214 2024-04-25 04:41:51.000000 helios-client-0.4.20240503.post1/debian/watch
+-rw-rw-r--   0 kip       (1000) kip       (1000)       38 2024-05-04 05:29:59.239845 helios-client-0.4.20240503.post1/setup.cfg
+-rwxrwxr-x   0 kip       (1000) kip       (1000)     3358 2024-04-07 02:31:28.000000 helios-client-0.4.20240503.post1/setup.py
```

### Comparing `helios-client-0.4.20240424.post1/Copying` & `helios-client-0.4.20240503.post1/Copying`

 * *Files identical despite different names*

### Comparing `helios-client-0.4.20240424.post1/PKG-INFO` & `helios-client-0.4.20240503.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helios-client
-Version: 0.4.20240424.post1
+Version: 0.4.20240503.post1
 Summary: Pure python 3 module to communicate with a Helios server.
 Home-page: https://www.heliosmusic.io
 Author: Cartesian Theatre
 Author-email: kip@heliosmusic.io
 License: LGPL
 Project-URL: Bug Tracker, https://github.com/cartesiantheatre/python-helios-client/issues
 Project-URL: Documentation, https://heliosmusic.io/api.html
```

### Comparing `helios-client-0.4.20240424.post1/README.md` & `helios-client-0.4.20240503.post1/README.md`

 * *Files identical despite different names*

### Comparing `helios-client-0.4.20240424.post1/Source/helios/chunked_upload.py` & `helios-client-0.4.20240503.post1/Source/helios/chunked_upload.py`

 * *Files identical despite different names*

### Comparing `helios-client-0.4.20240424.post1/Source/helios/client.py` & `helios-client-0.4.20240503.post1/Source/helios/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,29 +104,36 @@
 #            requests_log = logging.getLogger("urllib3")
 #            requests_log.setLevel(logging.DEBUG)
 #            requests_log.propagate = True
 
     # Add the given learning example triplet...
     def add_learning_example(self, anchor_song_reference, positive_song_reference, negative_song_reference):
 
+        # Construct a list of the caller's single triplet...
+        single_triplet_list = [(anchor_song_reference, positive_song_reference, negative_song_reference)]
+
+        # Upload to server...
+        self.add_learning_examples(single_triplet_list)
+
+    # Add the given list of learning example triplets...
+    def add_learning_examples(self, learning_example_triplets):
+
         # Initialize headers...
         headers                     = self._common_headers
         headers['Accept']           = Client._json_mime_type
         headers['Content-Type']     = Client._json_mime_type
 
-        # Construct learning example object...
-        learning_example = helios.requests.LearningExample(
-            anchor_song_reference,
-            positive_song_reference,
-            negative_song_reference)
-
-        learning_examples = [learning_example]
+        # Construct list of learning example objects from triplet list...
+        learning_examples = [
+            helios.requests.LearningExample(anchor, positive, negative) for
+            (anchor, positive, negative) in learning_example_triplets
+        ]
 
-        # Construct learning example schema to transform learning example into
-        #  JSON...
+        # Construct learning example schema to transform learning example list
+        #  into JSON...
         learning_example_schema = helios.requests.LearningExampleSchema(many=True)
 
         # Submit request...
         response = self._submit_request(
             endpoint='/learning/examples',
             method='POST',
             headers=headers,
```

### Comparing `helios-client-0.4.20240424.post1/Source/helios/exceptions.py` & `helios-client-0.4.20240503.post1/Source/helios/exceptions.py`

 * *Files identical despite different names*

### Comparing `helios-client-0.4.20240424.post1/Source/helios/requests.py` & `helios-client-0.4.20240503.post1/Source/helios/requests.py`

 * *Files identical despite different names*

### Comparing `helios-client-0.4.20240424.post1/Source/helios/responses.py` & `helios-client-0.4.20240503.post1/Source/helios/responses.py`

 * *Files identical despite different names*

### Comparing `helios-client-0.4.20240424.post1/Source/helios_client.egg-info/PKG-INFO` & `helios-client-0.4.20240503.post1/Source/helios_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helios-client
-Version: 0.4.20240424.post1
+Version: 0.4.20240503.post1
 Summary: Pure python 3 module to communicate with a Helios server.
 Home-page: https://www.heliosmusic.io
 Author: Cartesian Theatre
 Author-email: kip@heliosmusic.io
 License: LGPL
 Project-URL: Bug Tracker, https://github.com/cartesiantheatre/python-helios-client/issues
 Project-URL: Documentation, https://heliosmusic.io/api.html
```

### Comparing `helios-client-0.4.20240424.post1/Source/helios_client.egg-info/SOURCES.txt` & `helios-client-0.4.20240503.post1/Source/helios_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helios-client-0.4.20240424.post1/debian/control` & `helios-client-0.4.20240503.post1/debian/control`

 * *Files identical despite different names*

### Comparing `helios-client-0.4.20240424.post1/debian/rules` & `helios-client-0.4.20240503.post1/debian/rules`

 * *Files identical despite different names*

### Comparing `helios-client-0.4.20240424.post1/debian/tests/control` & `helios-client-0.4.20240503.post1/debian/tests/control`

 * *Files identical despite different names*

### Comparing `helios-client-0.4.20240424.post1/setup.py` & `helios-client-0.4.20240503.post1/setup.py`

 * *Files identical despite different names*

