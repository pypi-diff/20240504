# Comparing `tmp/pydolarvenezuela-1.5.2.tar.gz` & `tmp/pydolarvenezuela-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydolarvenezuela-1.5.2.tar", last modified: Mon Apr 29 16:13:07 2024, max compression
+gzip compressed data, was "pydolarvenezuela-1.5.3.tar", last modified: Fri May  3 19:00:15 2024, max compression
```

## Comparing `pydolarvenezuela-1.5.2.tar` & `pydolarvenezuela-1.5.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 16:13:07.896654 pydolarvenezuela-1.5.2/
--rw-rw-rw-   0        0        0     1094 2023-10-12 04:26:29.000000 pydolarvenezuela-1.5.2/LICENSE
--rw-rw-rw-   0        0        0     7221 2024-04-29 16:13:07.893655 pydolarvenezuela-1.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     4830 2024-04-28 21:36:23.000000 pydolarvenezuela-1.5.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 16:13:07.782611 pydolarvenezuela-1.5.2/pyDolarVenezuela/
--rw-rw-rw-   0        0        0     2712 2024-04-29 16:12:38.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:13:07.811276 pydolarvenezuela-1.5.2/pyDolarVenezuela/assets/
--rw-rw-rw-   0        0        0       20 2023-11-22 01:27:36.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:13:07.815278 pydolarvenezuela-1.5.2/pyDolarVenezuela/assets/icons/
--rw-rw-rw-   0        0        0      927 2023-11-22 01:28:58.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/assets/icons/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:13:07.831659 pydolarvenezuela-1.5.2/pyDolarVenezuela/data/
--rw-rw-rw-   0        0        0        0 2024-04-25 17:18:32.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/data/__init__.py
--rw-rw-rw-   0        0        0      684 2024-04-26 15:20:21.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/data/redis.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:13:07.847609 pydolarvenezuela-1.5.2/pyDolarVenezuela/models/
--rw-rw-rw-   0        0        0        0 2024-04-25 22:38:51.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/models/__init__.py
--rw-rw-rw-   0        0        0      364 2024-04-26 04:56:19.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/models/database.py
--rw-rw-rw-   0        0        0      312 2024-04-28 07:05:31.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/models/pages.py
--rw-rw-rw-   0        0        0      453 2024-04-27 21:40:31.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/network.py
--rw-rw-rw-   0        0        0      740 2024-04-28 16:11:30.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/pages.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:13:07.872898 pydolarvenezuela-1.5.2/pyDolarVenezuela/provider/
--rw-rw-rw-   0        0        0     5145 2024-04-29 16:08:34.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/provider/__init__.py
--rw-rw-rw-   0        0        0     2141 2024-04-28 15:44:15.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/provider/bcv.py
--rw-rw-rw-   0        0        0     1762 2024-04-29 16:09:28.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/provider/criptodolar.py
--rw-rw-rw-   0        0        0     2315 2024-04-28 12:10:54.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/provider/exchangemonitor.py
--rw-rw-rw-   0        0        0     1282 2024-04-28 21:32:57.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/provider/italcambio.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:13:07.884889 pydolarvenezuela-1.5.2/pyDolarVenezuela/tools/
--rw-rw-rw-   0        0        0      104 2024-04-02 19:26:40.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/tools/__init__.py
--rw-rw-rw-   0        0        0      670 2024-03-07 02:06:16.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/tools/calculator.py
--rw-rw-rw-   0        0        0     2187 2024-04-02 19:26:31.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/tools/time.py
--rw-rw-rw-   0        0        0     2236 2024-04-28 11:49:26.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:13:07.890658 pydolarvenezuela-1.5.2/pyDolarVenezuela.egg-info/
--rw-rw-rw-   0        0        0     7221 2024-04-29 16:13:07.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      897 2024-04-29 16:13:07.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 16:13:07.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-29 16:13:07.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-29 16:13:07.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-04-29 16:12:24.000000 pydolarvenezuela-1.5.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-29 16:13:07.897657 pydolarvenezuela-1.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1488 2024-04-29 16:12:30.000000 pydolarvenezuela-1.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 19:00:15.510208 pydolarvenezuela-1.5.3/
+-rw-rw-rw-   0        0        0     1094 2023-10-12 04:26:29.000000 pydolarvenezuela-1.5.3/LICENSE
+-rw-rw-rw-   0        0        0     7221 2024-05-03 19:00:15.495756 pydolarvenezuela-1.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4830 2024-04-28 21:36:23.000000 pydolarvenezuela-1.5.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 19:00:15.293785 pydolarvenezuela-1.5.3/pyDolarVenezuela/
+-rw-rw-rw-   0        0        0     2712 2024-05-03 18:56:58.000000 pydolarvenezuela-1.5.3/pyDolarVenezuela/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 19:00:15.360635 pydolarvenezuela-1.5.3/pyDolarVenezuela/assets/
+-rw-rw-rw-   0        0        0       20 2023-11-22 01:27:36.000000 pydolarvenezuela-1.5.3/pyDolarVenezuela/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 19:00:15.360635 pydolarvenezuela-1.5.3/pyDolarVenezuela/assets/icons/
+-rw-rw-rw-   0        0        0      927 2023-11-22 01:28:58.000000 pydolarvenezuela-1.5.3/pyDolarVenezuela/assets/icons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 19:00:15.393557 pydolarvenezuela-1.5.3/pyDolarVenezuela/data/
+-rw-rw-rw-   0        0        0        0 2024-04-25 17:18:32.000000 pydolarvenezuela-1.5.3/pyDolarVenezuela/data/__init__.py
+-rw-rw-rw-   0        0        0      684 2024-04-26 15:20:21.000000 pydolarvenezuela-1.5.3/pyDolarVenezuela/data/redis.py
+drwxrwxrwx   0        0        0        0 2024-05-03 19:00:15.409794 pydolarvenezuela-1.5.3/pyDolarVenezuela/models/
+-rw-rw-rw-   0        0        0        0 2024-04-25 22:38:51.000000 pydolarvenezuela-1.5.3/pyDolarVenezuela/models/__init__.py
+-rw-rw-rw-   0        0        0      364 2024-04-26 04:56:19.000000 pydolarvenezuela-1.5.3/pyDolarVenezuela/models/database.py
+-rw-rw-rw-   0        0        0      312 2024-04-28 07:05:31.000000 pydolarvenezuela-1.5.3/pyDolarVenezuela/models/pages.py
+-rw-rw-rw-   0        0        0      453 2024-04-27 21:40:31.000000 pydolarvenezuela-1.5.3/pyDolarVenezuela/network.py
+-rw-rw-rw-   0        0        0      740 2024-04-28 16:11:30.000000 pydolarvenezuela-1.5.3/pyDolarVenezuela/pages.py
+drwxrwxrwx   0        0        0        0 2024-05-03 19:00:15.461361 pydolarvenezuela-1.5.3/pyDolarVenezuela/provider/
+-rw-rw-rw-   0        0        0     5190 2024-05-03 18:53:55.000000 pydolarvenezuela-1.5.3/pyDolarVenezuela/provider/__init__.py
+-rw-rw-rw-   0        0        0     2141 2024-04-28 15:44:15.000000 pydolarvenezuela-1.5.3/pyDolarVenezuela/provider/bcv.py
+-rw-rw-rw-   0        0        0     1762 2024-04-29 16:09:28.000000 pydolarvenezuela-1.5.3/pyDolarVenezuela/provider/criptodolar.py
+-rw-rw-rw-   0        0        0     2315 2024-04-28 12:10:54.000000 pydolarvenezuela-1.5.3/pyDolarVenezuela/provider/exchangemonitor.py
+-rw-rw-rw-   0        0        0     1282 2024-04-28 21:32:57.000000 pydolarvenezuela-1.5.3/pyDolarVenezuela/provider/italcambio.py
+drwxrwxrwx   0        0        0        0 2024-05-03 19:00:15.491973 pydolarvenezuela-1.5.3/pyDolarVenezuela/tools/
+-rw-rw-rw-   0        0        0      104 2024-04-02 19:26:40.000000 pydolarvenezuela-1.5.3/pyDolarVenezuela/tools/__init__.py
+-rw-rw-rw-   0        0        0      670 2024-03-07 02:06:16.000000 pydolarvenezuela-1.5.3/pyDolarVenezuela/tools/calculator.py
+-rw-rw-rw-   0        0        0     2187 2024-04-02 19:26:31.000000 pydolarvenezuela-1.5.3/pyDolarVenezuela/tools/time.py
+-rw-rw-rw-   0        0        0     2236 2024-04-28 11:49:26.000000 pydolarvenezuela-1.5.3/pyDolarVenezuela/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-03 19:00:15.495756 pydolarvenezuela-1.5.3/pyDolarVenezuela.egg-info/
+-rw-rw-rw-   0        0        0     7221 2024-05-03 19:00:14.000000 pydolarvenezuela-1.5.3/pyDolarVenezuela.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      897 2024-05-03 19:00:15.000000 pydolarvenezuela-1.5.3/pyDolarVenezuela.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 19:00:14.000000 pydolarvenezuela-1.5.3/pyDolarVenezuela.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-03 19:00:14.000000 pydolarvenezuela-1.5.3/pyDolarVenezuela.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-03 19:00:14.000000 pydolarvenezuela-1.5.3/pyDolarVenezuela.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-05-03 18:56:51.000000 pydolarvenezuela-1.5.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-03 19:00:15.510208 pydolarvenezuela-1.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     1488 2024-05-03 18:56:54.000000 pydolarvenezuela-1.5.3/setup.py
```

### Comparing `pydolarvenezuela-1.5.2/LICENSE` & `pydolarvenezuela-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.2/PKG-INFO` & `pydolarvenezuela-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.5.2
+Version: 1.5.3
 Summary: Esta librería en Python consulta los precios del dólar y/o euro en diversos monitores en Venezuela, además de la tasa de cambio oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Francisco Griman
```

### Comparing `pydolarvenezuela-1.5.2/README.md` & `pydolarvenezuela-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.2/pyDolarVenezuela/__init__.py` & `pydolarvenezuela-1.5.3/pyDolarVenezuela/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from . import network
 from .models.pages import Page
 from .data.redis import Redis
 from .tools import get_time_zone as getdate, currency_converter
 from .provider import select_monitor
 
-version = '1.5.2'
+version = '1.5.3'
 """
 Versión actual de la biblioteca    
 """
 
 class CheckVersion:
     """
     Verificar actualización de la biblioteca
```

### Comparing `pydolarvenezuela-1.5.2/pyDolarVenezuela/assets/icons/__init__.py` & `pydolarvenezuela-1.5.3/pyDolarVenezuela/assets/icons/__init__.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.2/pyDolarVenezuela/data/redis.py` & `pydolarvenezuela-1.5.3/pyDolarVenezuela/data/redis.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.2/pyDolarVenezuela/pages.py` & `pydolarvenezuela-1.5.3/pyDolarVenezuela/pages.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.2/pyDolarVenezuela/provider/__init__.py` & `pydolarvenezuela-1.5.3/pyDolarVenezuela/provider/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,37 +64,38 @@
         except KeyError:
             raise KeyError("Does not match any of the properties that were provided in the dictionary. Most information: https://github.com/fcoagz/pyDolarVenezuela")
 
     def _update_item(existing_data_dict: dict, i: Any, last_data: dict):
         if existing_data_dict[i]['price'] != last_data[i]['price']:
             price = existing_data_dict[i]['price']
             new_price = last_data[i]['price']
+            price_old = last_data[i].get('price_old', None)
             change  = round(float(new_price - price), 2)
             percent = float(f'{round(float((change / new_price) * 100 if price != 0 else 0), 2)}'.replace('-', ' '))
             symbol  = "" if change == 0 else "▲" if change >= 0 else "▼"
             color   = "red" if symbol == '▼' else "green" if symbol == '▲' else "neutral"
             last_update = last_data[i].get('last_update', None)
             change = float(str(change).replace('-', ' '))
 
-            if last_update:
-                existing_data_dict[i].update({
+            existing_data_dict[i].update({
                     'price': new_price,
                     'change': change,
                     'percent': percent,
                     'color': color,
                     'symbol': symbol,
+            })
+
+            if last_update and price_old is not None:
+                existing_data_dict[i].update({
+                    'price_old': price_old,
                     'last_update': last_update
                 })
             else:
                 existing_data_dict[i].update({
-                    'price': new_price,
-                    'change': change,
-                    'percent': percent,
-                    'color': color,
-                    'symbol': symbol,
+                    'last_update': last_update
                 })
 
     try:
         monitor_class = None
 
         for monitor in monitor_classes:
             if monitor.get(provider.name) and currency in monitor.get(provider.name)['currency']:
```

### Comparing `pydolarvenezuela-1.5.2/pyDolarVenezuela/provider/bcv.py` & `pydolarvenezuela-1.5.3/pyDolarVenezuela/provider/bcv.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.2/pyDolarVenezuela/provider/criptodolar.py` & `pydolarvenezuela-1.5.3/pyDolarVenezuela/provider/criptodolar.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.2/pyDolarVenezuela/provider/exchangemonitor.py` & `pydolarvenezuela-1.5.3/pyDolarVenezuela/provider/exchangemonitor.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.2/pyDolarVenezuela/provider/italcambio.py` & `pydolarvenezuela-1.5.3/pyDolarVenezuela/provider/italcambio.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.2/pyDolarVenezuela/tools/calculator.py` & `pydolarvenezuela-1.5.3/pyDolarVenezuela/tools/calculator.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.2/pyDolarVenezuela/tools/time.py` & `pydolarvenezuela-1.5.3/pyDolarVenezuela/tools/time.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.2/pyDolarVenezuela/utils.py` & `pydolarvenezuela-1.5.3/pyDolarVenezuela/utils.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.2/pyDolarVenezuela.egg-info/PKG-INFO` & `pydolarvenezuela-1.5.3/pyDolarVenezuela.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.5.2
+Version: 1.5.3
 Summary: Esta librería en Python consulta los precios del dólar y/o euro en diversos monitores en Venezuela, además de la tasa de cambio oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Francisco Griman
```

### Comparing `pydolarvenezuela-1.5.2/pyDolarVenezuela.egg-info/SOURCES.txt` & `pydolarvenezuela-1.5.3/pyDolarVenezuela.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.2/pyproject.toml` & `pydolarvenezuela-1.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyDolarVenezuela"
-version = "1.5.2"
+version = "1.5.3"
 dependencies = [
   "requests",
   "curl_cffi",
   "beautifulsoup4",
   "babel",
   "pytz",
   "colorama",
```

### Comparing `pydolarvenezuela-1.5.2/setup.py` & `pydolarvenezuela-1.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.5.2'
+VERSION = '1.5.3'
 PACKAGE_NAME = 'pyDolarVenezuela' 
 AUTHOR = 'Francisco Griman'
 AUTHOR_EMAIL = 'grihardware@gmail.com'
 URL = 'https://github.com/fcoagz/pydolarvenezuela'
 
 LICENSE = 'MIT'
 DESCRIPTION = 'esta es una librería en python que te permite consultar los precios del dólar en diferentes monitores en Venezuela y el dolar oficial BCV.'
```

