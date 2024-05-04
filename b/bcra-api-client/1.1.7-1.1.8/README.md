# Comparing `tmp/bcra-api-client-1.1.7.tar.gz` & `tmp/bcra_api_client-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcra-api-client-1.1.7.tar", last modified: Sat May  4 17:56:56 2024, max compression
+gzip compressed data, was "bcra_api_client-1.1.8.tar", last modified: Sat May  4 18:38:05 2024, max compression
```

## Comparing `bcra-api-client-1.1.7.tar` & `bcra_api_client-1.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 17:56:56.688432 bcra-api-client-1.1.7/
--rw-rw-rw-   0        0        0     1082 2024-05-03 18:04:37.000000 bcra-api-client-1.1.7/LICENSE
--rw-rw-rw-   0        0        0      708 2024-05-04 17:56:56.685442 bcra-api-client-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0       94 2024-05-03 18:04:37.000000 bcra-api-client-1.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 17:56:56.668488 bcra-api-client-1.1.7/bcra/
--rw-rw-rw-   0        0        0      141 2024-05-04 17:50:59.000000 bcra-api-client-1.1.7/bcra/__init__.py
--rw-rw-rw-   0        0        0     1105 2024-05-03 23:02:06.000000 bcra-api-client-1.1.7/bcra/base.py
--rw-rw-rw-   0        0        0      264 2024-05-03 22:41:40.000000 bcra-api-client-1.1.7/bcra/client.py
--rw-rw-rw-   0        0        0      341 2024-05-03 22:41:40.000000 bcra-api-client-1.1.7/bcra/config.py
--rw-rw-rw-   0        0        0      300 2024-05-04 17:37:24.000000 bcra-api-client-1.1.7/bcra/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-04 17:56:56.673473 bcra-api-client-1.1.7/bcra/statistics/
--rw-rw-rw-   0        0        0      239 2024-05-03 21:48:25.000000 bcra-api-client-1.1.7/bcra/statistics/__init__.py
--rw-rw-rw-   0        0        0     1248 2024-05-04 17:53:43.000000 bcra-api-client-1.1.7/bcra/statistics/variables.py
-drwxrwxrwx   0        0        0        0 2024-05-04 17:56:56.683446 bcra-api-client-1.1.7/bcra_api_client.egg-info/
--rw-rw-rw-   0        0        0      708 2024-05-04 17:56:56.000000 bcra-api-client-1.1.7/bcra_api_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2024-05-04 17:56:56.000000 bcra-api-client-1.1.7/bcra_api_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 17:56:56.000000 bcra-api-client-1.1.7/bcra_api_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-04 17:56:56.000000 bcra-api-client-1.1.7/bcra_api_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      632 2024-05-04 17:56:35.000000 bcra-api-client-1.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-04 17:56:56.688432 bcra-api-client-1.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:38:05.409231 bcra_api_client-1.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-04 18:38:00.000000 bcra_api_client-1.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-04 18:38:05.409231 bcra_api_client-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-04 18:38:00.000000 bcra_api_client-1.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:38:05.409231 bcra_api_client-1.1.8/bcra/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-04 18:38:00.000000 bcra_api_client-1.1.8/bcra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-04 18:38:00.000000 bcra_api_client-1.1.8/bcra/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-04 18:38:00.000000 bcra_api_client-1.1.8/bcra/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-04 18:38:00.000000 bcra_api_client-1.1.8/bcra/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-04 18:38:00.000000 bcra_api_client-1.1.8/bcra/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:38:05.409231 bcra_api_client-1.1.8/bcra/statistics/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-04 18:38:00.000000 bcra_api_client-1.1.8/bcra/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-04 18:38:00.000000 bcra_api_client-1.1.8/bcra/statistics/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:38:05.409231 bcra_api_client-1.1.8/bcra_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-04 18:38:05.000000 bcra_api_client-1.1.8/bcra_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-04 18:38:05.000000 bcra_api_client-1.1.8/bcra_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 18:38:05.000000 bcra_api_client-1.1.8/bcra_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-04 18:38:05.000000 bcra_api_client-1.1.8/bcra_api_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-04 18:38:00.000000 bcra_api_client-1.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 18:38:05.409231 bcra_api_client-1.1.8/setup.cfg
```

### Comparing `bcra-api-client-1.1.7/bcra/base.py` & `bcra_api_client-1.1.8/bcra/base.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from .config import ConfigClient
-import pkg_resources
-import urllib3
-import json
-
-version = "unknown"
-
-try:
-    version = pkg_resources.require("bcra-api-client")[0].version
-except:
-    pass
-
-
-class BaseClient:
-
-    def __init__(self, config: ConfigClient) -> None:
-
-        self.base_url = config.base_url
-
-        self.headers = {
-            "Accept-Encoding": "gzip",
-            "User-Agent": f"paivae/BCRA BCRA_Python_Client/{version}",
-        }
-
-        self.client = urllib3.PoolManager(
-            headers=self.headers
-        )
-
-    def _decoded(self, response):
-        return json.loads(response.data.decode("utf-8"))
-
-    def _get(self,
-             path: str
-             ):
-
-        response = self.client.request(
-            "GET",
-            self.base_url + path,
-            headers=self.headers
-        )
-
-        if response.status != 200:
-            raise "Error in Query"
-
-        try:
-            obj = self._decoded(response)
-            return obj
-        except Exception as e:
-            print(f"Error json response: {e}")
+from .config import ConfigClient
+import pkg_resources
+import urllib3
+import json
+
+version = "unknown"
+
+try:
+    version = pkg_resources.require("bcra-api-client")[0].version
+except:
+    pass
+
+
+class BaseClient:
+
+    def __init__(self, config: ConfigClient) -> None:
+
+        self.base_url = config.base_url
+
+        self.headers = {
+            "Accept-Encoding": "gzip",
+            "User-Agent": f"paivae/BCRA BCRA_Python_Client/{version}",
+        }
+
+        self.client = urllib3.PoolManager(
+            headers=self.headers
+        )
+
+    def _decoded(self, response):
+        return json.loads(response.data.decode("utf-8"))
+
+    def _get(self,
+             path: str
+             ):
+
+        response = self.client.request(
+            "GET",
+            self.base_url + path,
+            headers=self.headers
+        )
+
+        if response.status != 200:
+            raise "Error in Query"
+
+        try:
+            obj = self._decoded(response)
+            return obj
+        except Exception as e:
+            print(f"Error json response: {e}")
```

