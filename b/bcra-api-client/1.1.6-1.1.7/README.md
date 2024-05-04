# Comparing `tmp/bcra-api-client-1.1.6.tar.gz` & `tmp/bcra-api-client-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcra-api-client-1.1.6.tar", last modified: Fri May  3 23:04:50 2024, max compression
+gzip compressed data, was "bcra-api-client-1.1.7.tar", last modified: Sat May  4 17:56:56 2024, max compression
```

## Comparing `bcra-api-client-1.1.6.tar` & `bcra-api-client-1.1.7.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 23:04:50.303379 bcra-api-client-1.1.6/
--rw-rw-rw-   0        0        0     1082 2024-05-03 18:04:37.000000 bcra-api-client-1.1.6/LICENSE
--rw-rw-rw-   0        0        0      708 2024-05-03 23:04:50.301384 bcra-api-client-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       94 2024-05-03 18:04:37.000000 bcra-api-client-1.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 23:04:50.278445 bcra-api-client-1.1.6/bcra/
--rw-rw-rw-   0        0        0       78 2024-05-03 19:21:19.000000 bcra-api-client-1.1.6/bcra/__init__.py
--rw-rw-rw-   0        0        0     1105 2024-05-03 23:02:06.000000 bcra-api-client-1.1.6/bcra/base.py
--rw-rw-rw-   0        0        0      264 2024-05-03 22:41:40.000000 bcra-api-client-1.1.6/bcra/client.py
--rw-rw-rw-   0        0        0      341 2024-05-03 22:41:40.000000 bcra-api-client-1.1.6/bcra/config.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:04:50.286424 bcra-api-client-1.1.6/bcra/statistics/
--rw-rw-rw-   0        0        0      239 2024-05-03 21:48:25.000000 bcra-api-client-1.1.6/bcra/statistics/__init__.py
--rw-rw-rw-   0        0        0      658 2024-05-03 23:04:17.000000 bcra-api-client-1.1.6/bcra/statistics/variables.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:04:50.299391 bcra-api-client-1.1.6/bcra_api_client.egg-info/
--rw-rw-rw-   0        0        0      708 2024-05-03 23:04:50.000000 bcra-api-client-1.1.6/bcra_api_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-05-03 23:04:50.000000 bcra-api-client-1.1.6/bcra_api_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 23:04:50.000000 bcra-api-client-1.1.6/bcra_api_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-03 23:04:50.000000 bcra-api-client-1.1.6/bcra_api_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      632 2024-05-03 23:04:28.000000 bcra-api-client-1.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-03 23:04:50.303379 bcra-api-client-1.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-04 17:56:56.688432 bcra-api-client-1.1.7/
+-rw-rw-rw-   0        0        0     1082 2024-05-03 18:04:37.000000 bcra-api-client-1.1.7/LICENSE
+-rw-rw-rw-   0        0        0      708 2024-05-04 17:56:56.685442 bcra-api-client-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       94 2024-05-03 18:04:37.000000 bcra-api-client-1.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 17:56:56.668488 bcra-api-client-1.1.7/bcra/
+-rw-rw-rw-   0        0        0      141 2024-05-04 17:50:59.000000 bcra-api-client-1.1.7/bcra/__init__.py
+-rw-rw-rw-   0        0        0     1105 2024-05-03 23:02:06.000000 bcra-api-client-1.1.7/bcra/base.py
+-rw-rw-rw-   0        0        0      264 2024-05-03 22:41:40.000000 bcra-api-client-1.1.7/bcra/client.py
+-rw-rw-rw-   0        0        0      341 2024-05-03 22:41:40.000000 bcra-api-client-1.1.7/bcra/config.py
+-rw-rw-rw-   0        0        0      300 2024-05-04 17:37:24.000000 bcra-api-client-1.1.7/bcra/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-04 17:56:56.673473 bcra-api-client-1.1.7/bcra/statistics/
+-rw-rw-rw-   0        0        0      239 2024-05-03 21:48:25.000000 bcra-api-client-1.1.7/bcra/statistics/__init__.py
+-rw-rw-rw-   0        0        0     1248 2024-05-04 17:53:43.000000 bcra-api-client-1.1.7/bcra/statistics/variables.py
+drwxrwxrwx   0        0        0        0 2024-05-04 17:56:56.683446 bcra-api-client-1.1.7/bcra_api_client.egg-info/
+-rw-rw-rw-   0        0        0      708 2024-05-04 17:56:56.000000 bcra-api-client-1.1.7/bcra_api_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2024-05-04 17:56:56.000000 bcra-api-client-1.1.7/bcra_api_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 17:56:56.000000 bcra-api-client-1.1.7/bcra_api_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-04 17:56:56.000000 bcra-api-client-1.1.7/bcra_api_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      632 2024-05-04 17:56:35.000000 bcra-api-client-1.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-04 17:56:56.688432 bcra-api-client-1.1.7/setup.cfg
```

### Comparing `bcra-api-client-1.1.6/LICENSE` & `bcra-api-client-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bcra-api-client-1.1.6/PKG-INFO` & `bcra-api-client-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcra-api-client
-Version: 1.1.6
+Version: 1.1.7
 Summary: Consumo de datos de la API del banco central de la Republica Argentina
 Author-email: Emmanuel Paiva <none@email.com>
 Project-URL: Homepage, https://github.com/paivae/BCRA-client-python
 Project-URL: Issues, https://github.com/paivae/BCRA-client-python/issues
 Keywords: Argentina,data,api,BCRA,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bcra-api-client-1.1.6/bcra/base.py` & `bcra-api-client-1.1.7/bcra/base.py`

 * *Files identical despite different names*

### Comparing `bcra-api-client-1.1.6/bcra_api_client.egg-info/PKG-INFO` & `bcra-api-client-1.1.7/bcra_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcra-api-client
-Version: 1.1.6
+Version: 1.1.7
 Summary: Consumo de datos de la API del banco central de la Republica Argentina
 Author-email: Emmanuel Paiva <none@email.com>
 Project-URL: Homepage, https://github.com/paivae/BCRA-client-python
 Project-URL: Issues, https://github.com/paivae/BCRA-client-python/issues
 Keywords: Argentina,data,api,BCRA,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bcra-api-client-1.1.6/pyproject.toml` & `bcra-api-client-1.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bcra-api-client"
-version = "1.1.6"
+version = "1.1.7"
 authors = [
   { name="Emmanuel Paiva", email="none@email.com"},
 ]
 description = "Consumo de datos de la API del banco central de la Republica Argentina"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

