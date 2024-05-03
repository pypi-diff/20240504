# Comparing `tmp/bcra-api-client-1.1.3.tar.gz` & `tmp/bcra-api-client-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcra-api-client-1.1.3.tar", last modified: Fri May  3 21:57:58 2024, max compression
+gzip compressed data, was "bcra-api-client-1.1.4.tar", last modified: Fri May  3 22:42:02 2024, max compression
```

## Comparing `bcra-api-client-1.1.3.tar` & `bcra-api-client-1.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 21:57:58.013746 bcra-api-client-1.1.3/
--rw-rw-rw-   0        0        0     1082 2024-05-03 18:04:37.000000 bcra-api-client-1.1.3/LICENSE
--rw-rw-rw-   0        0        0      708 2024-05-03 21:57:58.010756 bcra-api-client-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       94 2024-05-03 18:04:37.000000 bcra-api-client-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 21:57:57.995794 bcra-api-client-1.1.3/bcra/
--rw-rw-rw-   0        0        0       78 2024-05-03 19:21:19.000000 bcra-api-client-1.1.3/bcra/__init__.py
--rw-rw-rw-   0        0        0     1085 2024-05-03 21:57:00.000000 bcra-api-client-1.1.3/bcra/base.py
--rw-rw-rw-   0        0        0      301 2024-05-03 21:27:11.000000 bcra-api-client-1.1.3/bcra/client.py
--rw-rw-rw-   0        0        0      394 2024-05-03 21:22:17.000000 bcra-api-client-1.1.3/bcra/config.py
-drwxrwxrwx   0        0        0        0 2024-05-03 21:57:57.998785 bcra-api-client-1.1.3/bcra/statistics/
--rw-rw-rw-   0        0        0      239 2024-05-03 21:48:25.000000 bcra-api-client-1.1.3/bcra/statistics/__init__.py
--rw-rw-rw-   0        0        0      609 2024-05-03 21:57:00.000000 bcra-api-client-1.1.3/bcra/statistics/variables.py
-drwxrwxrwx   0        0        0        0 2024-05-03 21:57:58.009755 bcra-api-client-1.1.3/bcra_api_client.egg-info/
--rw-rw-rw-   0        0        0      708 2024-05-03 21:57:57.000000 bcra-api-client-1.1.3/bcra_api_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-05-03 21:57:57.000000 bcra-api-client-1.1.3/bcra_api_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 21:57:57.000000 bcra-api-client-1.1.3/bcra_api_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-03 21:57:57.000000 bcra-api-client-1.1.3/bcra_api_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      632 2024-05-03 21:57:44.000000 bcra-api-client-1.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-03 21:57:58.013746 bcra-api-client-1.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-03 22:42:02.732959 bcra-api-client-1.1.4/
+-rw-rw-rw-   0        0        0     1082 2024-05-03 18:04:37.000000 bcra-api-client-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0      708 2024-05-03 22:42:02.730965 bcra-api-client-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       94 2024-05-03 18:04:37.000000 bcra-api-client-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 22:42:02.714011 bcra-api-client-1.1.4/bcra/
+-rw-rw-rw-   0        0        0       78 2024-05-03 19:21:19.000000 bcra-api-client-1.1.4/bcra/__init__.py
+-rw-rw-rw-   0        0        0     1085 2024-05-03 21:57:00.000000 bcra-api-client-1.1.4/bcra/base.py
+-rw-rw-rw-   0        0        0      264 2024-05-03 22:41:40.000000 bcra-api-client-1.1.4/bcra/client.py
+-rw-rw-rw-   0        0        0      341 2024-05-03 22:41:40.000000 bcra-api-client-1.1.4/bcra/config.py
+drwxrwxrwx   0        0        0        0 2024-05-03 22:42:02.718997 bcra-api-client-1.1.4/bcra/statistics/
+-rw-rw-rw-   0        0        0      239 2024-05-03 21:48:25.000000 bcra-api-client-1.1.4/bcra/statistics/__init__.py
+-rw-rw-rw-   0        0        0      618 2024-05-03 22:37:27.000000 bcra-api-client-1.1.4/bcra/statistics/variables.py
+drwxrwxrwx   0        0        0        0 2024-05-03 22:42:02.728973 bcra-api-client-1.1.4/bcra_api_client.egg-info/
+-rw-rw-rw-   0        0        0      708 2024-05-03 22:42:02.000000 bcra-api-client-1.1.4/bcra_api_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-05-03 22:42:02.000000 bcra-api-client-1.1.4/bcra_api_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 22:42:02.000000 bcra-api-client-1.1.4/bcra_api_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-03 22:42:02.000000 bcra-api-client-1.1.4/bcra_api_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      632 2024-05-03 22:41:40.000000 bcra-api-client-1.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-03 22:42:02.733958 bcra-api-client-1.1.4/setup.cfg
```

### Comparing `bcra-api-client-1.1.3/LICENSE` & `bcra-api-client-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bcra-api-client-1.1.3/PKG-INFO` & `bcra-api-client-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcra-api-client
-Version: 1.1.3
+Version: 1.1.4
 Summary: Consumo de datos de la API del banco central de la Republica Argentina
 Author-email: Emmanuel Paiva <none@email.com>
 Project-URL: Homepage, https://github.com/paivae/BCRA-client-python
 Project-URL: Issues, https://github.com/paivae/BCRA-client-python/issues
 Keywords: Argentina,data,api,BCRA,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bcra-api-client-1.1.3/bcra/base.py` & `bcra-api-client-1.1.4/bcra/base.py`

 * *Files identical despite different names*

### Comparing `bcra-api-client-1.1.3/bcra/statistics/variables.py` & `bcra-api-client-1.1.4/bcra/statistics/variables.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from bcra.base import BaseClient
 from bcra.config import ConfigClient
 
 
 class Variables(BaseClient):
 
-    def __init__(self, config: ConfigClient, path_root) -> None:
+    def __init__(self, config: ConfigClient, path_root: str) -> None:
         self.path = path_root + "principalesvariables"
         super().__init__(config)
 
     def get(self,
             id_variable: int = None,
             from_: str = None,
             to: str = None):
         path_params = ""
 
-        if id_variable is not None and from_ is not None and to != None:
+        if id_variable is not None and from_ is not None and to is not None:
             self.path = f"{self.path}{self.path}/{id_variable}/{from_}/{to}"
 
         return self._get(path=self.path)
```

### Comparing `bcra-api-client-1.1.3/bcra_api_client.egg-info/PKG-INFO` & `bcra-api-client-1.1.4/bcra_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcra-api-client
-Version: 1.1.3
+Version: 1.1.4
 Summary: Consumo de datos de la API del banco central de la Republica Argentina
 Author-email: Emmanuel Paiva <none@email.com>
 Project-URL: Homepage, https://github.com/paivae/BCRA-client-python
 Project-URL: Issues, https://github.com/paivae/BCRA-client-python/issues
 Keywords: Argentina,data,api,BCRA,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bcra-api-client-1.1.3/pyproject.toml` & `bcra-api-client-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bcra-api-client"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
   { name="Emmanuel Paiva", email="none@email.com"},
 ]
 description = "Consumo de datos de la API del banco central de la Republica Argentina"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

