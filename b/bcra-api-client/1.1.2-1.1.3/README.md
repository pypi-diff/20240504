# Comparing `tmp/bcra-api-client-1.1.2.tar.gz` & `tmp/bcra-api-client-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcra-api-client-1.1.2.tar", last modified: Fri May  3 21:52:53 2024, max compression
+gzip compressed data, was "bcra-api-client-1.1.3.tar", last modified: Fri May  3 21:57:58 2024, max compression
```

## Comparing `bcra-api-client-1.1.2.tar` & `bcra-api-client-1.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 21:52:53.812816 bcra-api-client-1.1.2/
--rw-rw-rw-   0        0        0     1082 2024-05-03 18:04:37.000000 bcra-api-client-1.1.2/LICENSE
--rw-rw-rw-   0        0        0      708 2024-05-03 21:52:53.810822 bcra-api-client-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       94 2024-05-03 18:04:37.000000 bcra-api-client-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 21:52:53.795863 bcra-api-client-1.1.2/bcra/
--rw-rw-rw-   0        0        0       78 2024-05-03 19:21:19.000000 bcra-api-client-1.1.2/bcra/__init__.py
--rw-rw-rw-   0        0        0     1203 2024-05-03 21:22:17.000000 bcra-api-client-1.1.2/bcra/base.py
--rw-rw-rw-   0        0        0      301 2024-05-03 21:27:11.000000 bcra-api-client-1.1.2/bcra/client.py
--rw-rw-rw-   0        0        0      394 2024-05-03 21:22:17.000000 bcra-api-client-1.1.2/bcra/config.py
-drwxrwxrwx   0        0        0        0 2024-05-03 21:52:53.800848 bcra-api-client-1.1.2/bcra/statistics/
--rw-rw-rw-   0        0        0      239 2024-05-03 21:48:25.000000 bcra-api-client-1.1.2/bcra/statistics/__init__.py
--rw-rw-rw-   0        0        0      614 2024-05-03 21:48:25.000000 bcra-api-client-1.1.2/bcra/statistics/variables.py
-drwxrwxrwx   0        0        0        0 2024-05-03 21:52:53.808827 bcra-api-client-1.1.2/bcra_api_client.egg-info/
--rw-rw-rw-   0        0        0      708 2024-05-03 21:52:53.000000 bcra-api-client-1.1.2/bcra_api_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-05-03 21:52:53.000000 bcra-api-client-1.1.2/bcra_api_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 21:52:53.000000 bcra-api-client-1.1.2/bcra_api_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-03 21:52:53.000000 bcra-api-client-1.1.2/bcra_api_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      632 2024-05-03 21:50:47.000000 bcra-api-client-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-03 21:52:53.813813 bcra-api-client-1.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-03 21:57:58.013746 bcra-api-client-1.1.3/
+-rw-rw-rw-   0        0        0     1082 2024-05-03 18:04:37.000000 bcra-api-client-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0      708 2024-05-03 21:57:58.010756 bcra-api-client-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       94 2024-05-03 18:04:37.000000 bcra-api-client-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 21:57:57.995794 bcra-api-client-1.1.3/bcra/
+-rw-rw-rw-   0        0        0       78 2024-05-03 19:21:19.000000 bcra-api-client-1.1.3/bcra/__init__.py
+-rw-rw-rw-   0        0        0     1085 2024-05-03 21:57:00.000000 bcra-api-client-1.1.3/bcra/base.py
+-rw-rw-rw-   0        0        0      301 2024-05-03 21:27:11.000000 bcra-api-client-1.1.3/bcra/client.py
+-rw-rw-rw-   0        0        0      394 2024-05-03 21:22:17.000000 bcra-api-client-1.1.3/bcra/config.py
+drwxrwxrwx   0        0        0        0 2024-05-03 21:57:57.998785 bcra-api-client-1.1.3/bcra/statistics/
+-rw-rw-rw-   0        0        0      239 2024-05-03 21:48:25.000000 bcra-api-client-1.1.3/bcra/statistics/__init__.py
+-rw-rw-rw-   0        0        0      609 2024-05-03 21:57:00.000000 bcra-api-client-1.1.3/bcra/statistics/variables.py
+drwxrwxrwx   0        0        0        0 2024-05-03 21:57:58.009755 bcra-api-client-1.1.3/bcra_api_client.egg-info/
+-rw-rw-rw-   0        0        0      708 2024-05-03 21:57:57.000000 bcra-api-client-1.1.3/bcra_api_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-05-03 21:57:57.000000 bcra-api-client-1.1.3/bcra_api_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 21:57:57.000000 bcra-api-client-1.1.3/bcra_api_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-03 21:57:57.000000 bcra-api-client-1.1.3/bcra_api_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      632 2024-05-03 21:57:44.000000 bcra-api-client-1.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-03 21:57:58.013746 bcra-api-client-1.1.3/setup.cfg
```

### Comparing `bcra-api-client-1.1.2/LICENSE` & `bcra-api-client-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bcra-api-client-1.1.2/PKG-INFO` & `bcra-api-client-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcra-api-client
-Version: 1.1.2
+Version: 1.1.3
 Summary: Consumo de datos de la API del banco central de la Republica Argentina
 Author-email: Emmanuel Paiva <none@email.com>
 Project-URL: Homepage, https://github.com/paivae/BCRA-client-python
 Project-URL: Issues, https://github.com/paivae/BCRA-client-python/issues
 Keywords: Argentina,data,api,BCRA,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bcra-api-client-1.1.2/bcra/base.py` & `bcra-api-client-1.1.3/bcra/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,52 +2,49 @@
 import pkg_resources
 import urllib3
 import json
 
 version = "unknown"
 
 try:
-   version = pkg_resources.require("bcra-api-client")[0].version
+    version = pkg_resources.require("bcra-api-client")[0].version
 except:
     pass
 
+
 class BaseClient:
 
     def __init__(self, config: ConfigClient) -> None:
-        
+
         self.base_url = config.base_url
-        
+
         self.headers = {
             "Accept-Encoding": "gzip",
             "User-Agent": f"paivae/BCRA BCRA_Python_Client/{version}",
         }
 
         self.client = urllib3.PoolManager(
-            headers = self.headers
+            headers=self.headers
         )
 
+    def _decoded(self, response):
+        return json.loads(response.data.decode("utf-8"))
 
     def _get(self,
-             path: str,
-             params : str
+             path: str
              ):
-        
+
         response = self.client.request(
             "GET",
-            self.BASE + path,
-            fields = params,
-            headers = self.headers
+            self.base_url + path,
+            headers=self.headers
         )
-        
 
-        if response.status != 200 :
+        if response.status != 200:
             raise "Error in Query"
-        
+
         try:
             obj = self._decoded(response)
         except Exception as e:
-            print(f"Error json response: {e.message}")
-        
+            print(f"Error json response: {e}")
+
 
-    def _decoded(self, response):
-        return json.loads(response.data.decode("utf-8"))
-
```

### Comparing `bcra-api-client-1.1.2/bcra/statistics/variables.py` & `bcra-api-client-1.1.3/bcra/statistics/variables.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,11 +10,11 @@
 
     def get(self,
             id_variable: int = None,
             from_: str = None,
             to: str = None):
         path_params = ""
 
-        if (id_variable != None and from_ != None and to != None):
-            path_params = f"{self.path}/{id_variable}/{from_}/{to}"
+        if id_variable is not None and from_ is not None and to != None:
+            self.path = f"{self.path}{self.path}/{id_variable}/{from_}/{to}"
 
-        return self._get(path=self.path, params=path_params)
+        return self._get(path=self.path)
```

### Comparing `bcra-api-client-1.1.2/bcra_api_client.egg-info/PKG-INFO` & `bcra-api-client-1.1.3/bcra_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcra-api-client
-Version: 1.1.2
+Version: 1.1.3
 Summary: Consumo de datos de la API del banco central de la Republica Argentina
 Author-email: Emmanuel Paiva <none@email.com>
 Project-URL: Homepage, https://github.com/paivae/BCRA-client-python
 Project-URL: Issues, https://github.com/paivae/BCRA-client-python/issues
 Keywords: Argentina,data,api,BCRA,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bcra-api-client-1.1.2/pyproject.toml` & `bcra-api-client-1.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bcra-api-client"
-version = "1.1.2"
+version = "1.1.3"
 authors = [
   { name="Emmanuel Paiva", email="none@email.com"},
 ]
 description = "Consumo de datos de la API del banco central de la Republica Argentina"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

