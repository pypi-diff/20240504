# Comparing `tmp/dreams_core-0.0.4.tar.gz` & `tmp/dreams_core-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreams_core-0.0.4.tar", last modified: Sat Apr 27 00:23:00 2024, max compression
+gzip compressed data, was "dreams_core-0.0.5.tar", last modified: Sat May  4 03:19:56 2024, max compression
```

## Comparing `dreams_core-0.0.4.tar` & `dreams_core-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-04-27 00:23:00.217876 dreams_core-0.0.4/
--rw-r--r--   0 jeremy     (502) staff       (20)     1126 2024-04-24 21:32:45.000000 dreams_core-0.0.4/LICENSE
--rw-r--r--   0 jeremy     (502) staff       (20)      178 2024-04-25 04:05:52.000000 dreams_core-0.0.4/MANIFEST.in
--rw-r--r--   0 jeremy     (502) staff       (20)     1187 2024-04-27 00:23:00.217655 dreams_core-0.0.4/PKG-INFO
--rw-r--r--   0 jeremy     (502) staff       (20)      317 2024-04-24 22:09:04.000000 dreams_core-0.0.4/README.md
--rw-r--r--   0 jeremy     (502) staff       (20)      884 2024-04-27 00:22:36.000000 dreams_core-0.0.4/pyproject.toml
--rw-r--r--   0 jeremy     (502) staff       (20)       38 2024-04-27 00:23:00.217932 dreams_core-0.0.4/setup.cfg
-drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-04-27 00:23:00.215402 dreams_core-0.0.4/src/
-drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-04-27 00:23:00.216578 dreams_core-0.0.4/src/dreams_core/
--rw-r--r--   0 jeremy     (502) staff       (20)       21 2024-04-27 00:22:32.000000 dreams_core-0.0.4/src/dreams_core/__init__.py
--rw-r--r--   0 jeremy     (502) staff       (20)     5233 2024-04-27 00:20:21.000000 dreams_core-0.0.4/src/dreams_core/core.py
--rw-r--r--   0 jeremy     (502) staff       (20)     3897 2024-04-25 04:03:45.000000 dreams_core-0.0.4/src/dreams_core/dune.py
--rw-r--r--   0 jeremy     (502) staff       (20)     4457 2024-04-27 00:12:49.000000 dreams_core-0.0.4/src/dreams_core/googlecloud.py
-drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-04-27 00:23:00.217414 dreams_core-0.0.4/src/dreams_core.egg-info/
--rw-r--r--   0 jeremy     (502) staff       (20)     1187 2024-04-27 00:23:00.000000 dreams_core-0.0.4/src/dreams_core.egg-info/PKG-INFO
--rw-r--r--   0 jeremy     (502) staff       (20)      369 2024-04-27 00:23:00.000000 dreams_core-0.0.4/src/dreams_core.egg-info/SOURCES.txt
--rw-r--r--   0 jeremy     (502) staff       (20)        1 2024-04-27 00:23:00.000000 dreams_core-0.0.4/src/dreams_core.egg-info/dependency_links.txt
--rw-r--r--   0 jeremy     (502) staff       (20)      159 2024-04-27 00:23:00.000000 dreams_core-0.0.4/src/dreams_core.egg-info/requires.txt
--rw-r--r--   0 jeremy     (502) staff       (20)       12 2024-04-27 00:23:00.000000 dreams_core-0.0.4/src/dreams_core.egg-info/top_level.txt
+drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-05-04 03:19:56.765268 dreams_core-0.0.5/
+-rw-r--r--   0 jeremy     (502) staff       (20)     1126 2024-04-24 21:32:45.000000 dreams_core-0.0.5/LICENSE
+-rw-r--r--   0 jeremy     (502) staff       (20)      178 2024-04-25 04:05:52.000000 dreams_core-0.0.5/MANIFEST.in
+-rw-r--r--   0 jeremy     (502) staff       (20)     1187 2024-05-04 03:19:56.765037 dreams_core-0.0.5/PKG-INFO
+-rw-r--r--   0 jeremy     (502) staff       (20)      317 2024-04-24 22:09:04.000000 dreams_core-0.0.5/README.md
+-rw-r--r--   0 jeremy     (502) staff       (20)      884 2024-05-04 03:19:13.000000 dreams_core-0.0.5/pyproject.toml
+-rw-r--r--   0 jeremy     (502) staff       (20)       38 2024-05-04 03:19:56.765309 dreams_core-0.0.5/setup.cfg
+drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-05-04 03:19:56.762156 dreams_core-0.0.5/src/
+drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-05-04 03:19:56.764056 dreams_core-0.0.5/src/dreams_core/
+-rw-r--r--   0 jeremy     (502) staff       (20)       21 2024-04-27 00:22:32.000000 dreams_core-0.0.5/src/dreams_core/__init__.py
+-rw-r--r--   0 jeremy     (502) staff       (20)     5233 2024-04-27 00:20:21.000000 dreams_core-0.0.5/src/dreams_core/core.py
+-rw-r--r--   0 jeremy     (502) staff       (20)     3897 2024-04-25 04:03:45.000000 dreams_core-0.0.5/src/dreams_core/dune.py
+-rw-r--r--   0 jeremy     (502) staff       (20)     4560 2024-05-04 03:18:52.000000 dreams_core-0.0.5/src/dreams_core/googlecloud.py
+drwxr-xr-x   0 jeremy     (502) staff       (20)        0 2024-05-04 03:19:56.764784 dreams_core-0.0.5/src/dreams_core.egg-info/
+-rw-r--r--   0 jeremy     (502) staff       (20)     1187 2024-05-04 03:19:56.000000 dreams_core-0.0.5/src/dreams_core.egg-info/PKG-INFO
+-rw-r--r--   0 jeremy     (502) staff       (20)      369 2024-05-04 03:19:56.000000 dreams_core-0.0.5/src/dreams_core.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremy     (502) staff       (20)        1 2024-05-04 03:19:56.000000 dreams_core-0.0.5/src/dreams_core.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremy     (502) staff       (20)      159 2024-05-04 03:19:56.000000 dreams_core-0.0.5/src/dreams_core.egg-info/requires.txt
+-rw-r--r--   0 jeremy     (502) staff       (20)       12 2024-05-04 03:19:56.000000 dreams_core-0.0.5/src/dreams_core.egg-info/top_level.txt
```

### Comparing `dreams_core-0.0.4/LICENSE` & `dreams_core-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dreams_core-0.0.4/PKG-INFO` & `dreams_core-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreams_core
-Version: 0.0.4
+Version: 0.0.5
 Summary: brought to you by the dreamslabs discord community
 Author-email: tentabs <tentabs00@gmail.com>
 Project-URL: Community, https://discord.gg/dreamcrypto
 Project-URL: Github, https://github.com/dreams-labs/core-functions
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `dreams_core-0.0.4/pyproject.toml` & `dreams_core-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dreams_core"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="tentabs", email="tentabs00@gmail.com" },
 ]
 description = "brought to you by the dreamslabs discord community"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
```

### Comparing `dreams_core-0.0.4/src/dreams_core/core.py` & `dreams_core-0.0.5/src/dreams_core/core.py`

 * *Files identical despite different names*

### Comparing `dreams_core-0.0.4/src/dreams_core/dune.py` & `dreams_core-0.0.5/src/dreams_core/dune.py`

 * *Files identical despite different names*

### Comparing `dreams_core-0.0.4/src/dreams_core/googlecloud.py` & `dreams_core-0.0.5/src/dreams_core/googlecloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,21 @@
             service_account_json_path=None,
             verbose=False
         ):
         # load credentials using service account and scope
         if service_account_json_path is None:
             service_account_json_path = os.getenv('GOOGLE_APPLICATION_CREDENTIALS')
         scopes = ["https://www.googleapis.com/auth/cloud-platform"]
-        self.credentials = service_account.Credentials.from_service_account_file(
-            service_account_json_path
-            ,scopes=scopes
-        )
+        try:
+            self.credentials = service_account.Credentials.from_service_account_file(
+                service_account_json_path
+                ,scopes=scopes
+            )
+        except: 
+            self.credentials, _ = google.auth.default()
 
         # other variables
         self.verbose = verbose
         self.location = 'US'
         self.project_id = 'western-verve-411004'
         self.project_name = 'dreams-labs-data'
         self.bucket_name = 'dreams-labs-storage'
@@ -120,7 +123,8 @@
                 print('returned fresh csv and refreshed cache')
         else:
             query_df = pd.read_csv(f'gs://{self.bucket_name}/{filepath}')
             if self.verbose:
                 print('returned cached csv')
 
         return query_df
+g
```

### Comparing `dreams_core-0.0.4/src/dreams_core.egg-info/PKG-INFO` & `dreams_core-0.0.5/src/dreams_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreams_core
-Version: 0.0.4
+Version: 0.0.5
 Summary: brought to you by the dreamslabs discord community
 Author-email: tentabs <tentabs00@gmail.com>
 Project-URL: Community, https://discord.gg/dreamcrypto
 Project-URL: Github, https://github.com/dreams-labs/core-functions
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

