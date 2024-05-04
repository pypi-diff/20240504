# Comparing `tmp/stac_fastapi_core-2.3.0.tar.gz` & `tmp/stac_fastapi_core-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_fastapi_core-2.3.0.tar", last modified: Wed Apr 24 05:12:07 2024, max compression
+gzip compressed data, was "stac_fastapi_core-2.3.1.tar", last modified: Sat May  4 10:06:04 2024, max compression
```

## Comparing `stac_fastapi_core-2.3.0.tar` & `stac_fastapi_core-2.3.1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-24 05:12:07.682021 stac_fastapi_core-2.3.0/
--rw-r--r--   0 primeradiant   (501) staff       (20)     1159 2024-04-24 05:12:07.681148 stac_fastapi_core-2.3.0/PKG-INFO
--rw-r--r--   0 primeradiant   (501) staff       (20)       69 2024-02-08 06:37:21.000000 stac_fastapi_core-2.3.0/README.md
--rw-r--r--   0 primeradiant   (501) staff       (20)      104 2024-04-24 05:12:07.683853 stac_fastapi_core-2.3.0/setup.cfg
--rw-r--r--   0 primeradiant   (501) staff       (20)     1335 2024-04-23 10:59:36.000000 stac_fastapi_core-2.3.0/setup.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-24 05:12:07.592529 stac_fastapi_core-2.3.0/stac_fastapi/
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-24 05:12:07.656256 stac_fastapi_core-2.3.0/stac_fastapi/core/
--rw-r--r--   0 primeradiant   (501) staff       (20)       20 2024-02-08 06:37:21.000000 stac_fastapi_core-2.3.0/stac_fastapi/core/__init__.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     1608 2024-02-08 06:37:21.000000 stac_fastapi_core-2.3.0/stac_fastapi/core/base_database_logic.py
--rw-r--r--   0 primeradiant   (501) staff       (20)      239 2024-02-08 06:37:21.000000 stac_fastapi_core-2.3.0/stac_fastapi/core/base_settings.py
--rw-r--r--   0 primeradiant   (501) staff       (20)    35941 2024-04-23 11:34:10.000000 stac_fastapi_core-2.3.0/stac_fastapi/core/core.py
--rw-r--r--   0 primeradiant   (501) staff       (20)      384 2024-02-08 06:37:21.000000 stac_fastapi_core-2.3.0/stac_fastapi/core/datetime_utils.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-24 05:12:07.663568 stac_fastapi_core-2.3.0/stac_fastapi/core/extensions/
--rw-r--r--   0 primeradiant   (501) staff       (20)      167 2024-02-08 06:37:21.000000 stac_fastapi_core-2.3.0/stac_fastapi/core/extensions/__init__.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     7464 2024-02-08 06:37:21.000000 stac_fastapi_core-2.3.0/stac_fastapi/core/extensions/filter.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     1892 2024-02-08 06:37:21.000000 stac_fastapi_core-2.3.0/stac_fastapi/core/extensions/query.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-24 05:12:07.671653 stac_fastapi_core-2.3.0/stac_fastapi/core/models/
--rw-r--r--   0 primeradiant   (501) staff       (20)       48 2024-02-08 06:37:21.000000 stac_fastapi_core-2.3.0/stac_fastapi/core/models/__init__.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     4470 2024-03-19 04:19:17.000000 stac_fastapi_core-2.3.0/stac_fastapi/core/models/links.py
--rw-r--r--   0 primeradiant   (501) staff       (20)       27 2024-02-08 06:37:21.000000 stac_fastapi_core-2.3.0/stac_fastapi/core/models/search.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     5892 2024-03-19 04:19:17.000000 stac_fastapi_core-2.3.0/stac_fastapi/core/serializers.py
--rw-r--r--   0 primeradiant   (501) staff       (20)      473 2024-02-08 06:37:21.000000 stac_fastapi_core-2.3.0/stac_fastapi/core/session.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-24 05:12:07.673254 stac_fastapi_core-2.3.0/stac_fastapi/core/types/
--rw-r--r--   0 primeradiant   (501) staff       (20)     9155 2024-04-23 10:58:50.000000 stac_fastapi_core-2.3.0/stac_fastapi/core/types/core.py
--rw-r--r--   0 primeradiant   (501) staff       (20)      933 2024-02-08 06:37:21.000000 stac_fastapi_core-2.3.0/stac_fastapi/core/utilities.py
--rw-r--r--   0 primeradiant   (501) staff       (20)       45 2024-04-24 05:07:59.000000 stac_fastapi_core-2.3.0/stac_fastapi/core/version.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-24 05:12:07.676343 stac_fastapi_core-2.3.0/stac_fastapi.core.egg-info/
--rw-r--r--   0 primeradiant   (501) staff       (20)     1159 2024-04-24 05:12:07.000000 stac_fastapi_core-2.3.0/stac_fastapi.core.egg-info/PKG-INFO
--rw-r--r--   0 primeradiant   (501) staff       (20)      818 2024-04-24 05:12:07.000000 stac_fastapi_core-2.3.0/stac_fastapi.core.egg-info/SOURCES.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-04-24 05:12:07.000000 stac_fastapi_core-2.3.0/stac_fastapi.core.egg-info/dependency_links.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-01-31 08:38:37.000000 stac_fastapi_core-2.3.0/stac_fastapi.core.egg-info/not-zip-safe
--rw-r--r--   0 primeradiant   (501) staff       (20)      207 2024-04-24 05:12:07.000000 stac_fastapi_core-2.3.0/stac_fastapi.core.egg-info/requires.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)       18 2024-04-24 05:12:07.000000 stac_fastapi_core-2.3.0/stac_fastapi.core.egg-info/top_level.txt
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-04 10:06:04.737167 stac_fastapi_core-2.3.1/
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1217 2024-05-04 10:06:04.736840 stac_fastapi_core-2.3.1/PKG-INFO
+-rw-r--r--   0 primeradiant   (501) staff       (20)       69 2024-02-08 06:37:21.000000 stac_fastapi_core-2.3.1/README.md
+-rw-r--r--   0 primeradiant   (501) staff       (20)      104 2024-05-04 10:06:04.745323 stac_fastapi_core-2.3.1/setup.cfg
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1385 2024-05-04 09:54:48.000000 stac_fastapi_core-2.3.1/setup.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-04 10:06:04.657884 stac_fastapi_core-2.3.1/stac_fastapi/
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-04 10:06:04.702210 stac_fastapi_core-2.3.1/stac_fastapi/core/
+-rw-r--r--   0 primeradiant   (501) staff       (20)       20 2024-02-08 06:37:21.000000 stac_fastapi_core-2.3.1/stac_fastapi/core/__init__.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1608 2024-02-08 06:37:21.000000 stac_fastapi_core-2.3.1/stac_fastapi/core/base_database_logic.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)      239 2024-02-08 06:37:21.000000 stac_fastapi_core-2.3.1/stac_fastapi/core/base_settings.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     3826 2024-05-02 09:57:35.000000 stac_fastapi_core-2.3.1/stac_fastapi/core/basic_auth.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)    35978 2024-05-02 09:57:35.000000 stac_fastapi_core-2.3.1/stac_fastapi/core/core.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)      384 2024-02-08 06:37:21.000000 stac_fastapi_core-2.3.1/stac_fastapi/core/datetime_utils.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-04 10:06:04.708142 stac_fastapi_core-2.3.1/stac_fastapi/core/extensions/
+-rw-r--r--   0 primeradiant   (501) staff       (20)      167 2024-02-08 06:37:21.000000 stac_fastapi_core-2.3.1/stac_fastapi/core/extensions/__init__.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     7464 2024-02-08 06:37:21.000000 stac_fastapi_core-2.3.1/stac_fastapi/core/extensions/filter.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1892 2024-02-08 06:37:21.000000 stac_fastapi_core-2.3.1/stac_fastapi/core/extensions/query.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-04 10:06:04.729008 stac_fastapi_core-2.3.1/stac_fastapi/core/models/
+-rw-r--r--   0 primeradiant   (501) staff       (20)       48 2024-02-08 06:37:21.000000 stac_fastapi_core-2.3.1/stac_fastapi/core/models/__init__.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     4470 2024-03-19 04:19:17.000000 stac_fastapi_core-2.3.1/stac_fastapi/core/models/links.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)       27 2024-02-08 06:37:21.000000 stac_fastapi_core-2.3.1/stac_fastapi/core/models/search.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     5892 2024-03-19 04:19:17.000000 stac_fastapi_core-2.3.1/stac_fastapi/core/serializers.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)      473 2024-02-08 06:37:21.000000 stac_fastapi_core-2.3.1/stac_fastapi/core/session.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-04 10:06:04.731994 stac_fastapi_core-2.3.1/stac_fastapi/core/types/
+-rw-r--r--   0 primeradiant   (501) staff       (20)     9155 2024-04-24 05:29:38.000000 stac_fastapi_core-2.3.1/stac_fastapi/core/types/core.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)      933 2024-02-08 06:37:21.000000 stac_fastapi_core-2.3.1/stac_fastapi/core/utilities.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)       45 2024-05-04 10:01:58.000000 stac_fastapi_core-2.3.1/stac_fastapi/core/version.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-04 10:06:04.735630 stac_fastapi_core-2.3.1/stac_fastapi.core.egg-info/
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1217 2024-05-04 10:06:04.000000 stac_fastapi_core-2.3.1/stac_fastapi.core.egg-info/PKG-INFO
+-rw-r--r--   0 primeradiant   (501) staff       (20)      850 2024-05-04 10:06:04.000000 stac_fastapi_core-2.3.1/stac_fastapi.core.egg-info/SOURCES.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-05-04 10:06:04.000000 stac_fastapi_core-2.3.1/stac_fastapi.core.egg-info/dependency_links.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-01-31 08:38:37.000000 stac_fastapi_core-2.3.1/stac_fastapi.core.egg-info/not-zip-safe
+-rw-r--r--   0 primeradiant   (501) staff       (20)      250 2024-05-04 10:06:04.000000 stac_fastapi_core-2.3.1/stac_fastapi.core.egg-info/requires.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)       18 2024-05-04 10:06:04.000000 stac_fastapi_core-2.3.1/stac_fastapi.core.egg-info/top_level.txt
```

### Comparing `stac_fastapi_core-2.3.0/PKG-INFO` & `stac_fastapi_core-2.3.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.core
-Version: 2.3.0
+Version: 2.3.1
 Summary: Core library for the Elasticsearch and Opensearch stac-fastapi backends.
 Home-page: https://github.com/stac-utils/stac-fastapi-elasticsearch-opensearch
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
@@ -14,17 +14,18 @@
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: fastapi
 Requires-Dist: attrs
 Requires-Dist: pydantic[dotenv]<2
 Requires-Dist: stac_pydantic==2.0.*
-Requires-Dist: stac-fastapi.types==2.5.3
-Requires-Dist: stac-fastapi.api==2.5.3
-Requires-Dist: stac-fastapi.extensions==2.5.3
+Requires-Dist: stac-fastapi.types==2.5.5.post1
+Requires-Dist: stac-fastapi.api==2.5.5.post1
+Requires-Dist: stac-fastapi.extensions==2.5.5.post1
 Requires-Dist: pystac[validation]
 Requires-Dist: orjson
 Requires-Dist: overrides
 Requires-Dist: geojson-pydantic
 Requires-Dist: pygeofilter==0.2.1
+Requires-Dist: typing_extensions==4.4.0
 
 # stac-fastapi core library for Elasticsearch and Opensearch backends
```

### Comparing `stac_fastapi_core-2.3.0/setup.py` & `stac_fastapi_core-2.3.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,22 +6,23 @@
     desc = f.read()
 
 install_requires = [
     "fastapi",
     "attrs",
     "pydantic[dotenv]<2",
     "stac_pydantic==2.0.*",
-    "stac-fastapi.types==2.5.3",
-    "stac-fastapi.api==2.5.3",
-    "stac-fastapi.extensions==2.5.3",
+    "stac-fastapi.types==2.5.5.post1",
+    "stac-fastapi.api==2.5.5.post1",
+    "stac-fastapi.extensions==2.5.5.post1",
     "pystac[validation]",
     "orjson",
     "overrides",
     "geojson-pydantic",
     "pygeofilter==0.2.1",
+    "typing_extensions==4.4.0",
 ]
 
 setup(
     name="stac-fastapi.core",
     description="Core library for the Elasticsearch and Opensearch stac-fastapi backends.",
     long_description=desc,
     long_description_content_type="text/markdown",
```

### Comparing `stac_fastapi_core-2.3.0/stac_fastapi/core/base_database_logic.py` & `stac_fastapi_core-2.3.1/stac_fastapi/core/base_database_logic.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_core-2.3.0/stac_fastapi/core/core.py` & `stac_fastapi_core-2.3.1/stac_fastapi/core/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -673,15 +673,15 @@
                 collection_id, processed_items, refresh=kwargs.get("refresh", False)
             )
 
             return None
         else:
             item = await self.database.prep_create_item(item=item, base_url=base_url)
             await self.database.create_item(item, refresh=kwargs.get("refresh", False))
-            return item
+            return ItemSerializer.db_to_stac(item, base_url)
 
     @overrides
     async def update_item(
         self, collection_id: str, item_id: str, item: stac_types.Item, **kwargs
     ) -> stac_types.Item:
         """Update an item in the collection.
```

### Comparing `stac_fastapi_core-2.3.0/stac_fastapi/core/extensions/filter.py` & `stac_fastapi_core-2.3.1/stac_fastapi/core/extensions/filter.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_core-2.3.0/stac_fastapi/core/extensions/query.py` & `stac_fastapi_core-2.3.1/stac_fastapi/core/extensions/query.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_core-2.3.0/stac_fastapi/core/models/links.py` & `stac_fastapi_core-2.3.1/stac_fastapi/core/models/links.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_core-2.3.0/stac_fastapi/core/serializers.py` & `stac_fastapi_core-2.3.1/stac_fastapi/core/serializers.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_core-2.3.0/stac_fastapi/core/types/core.py` & `stac_fastapi_core-2.3.1/stac_fastapi/core/types/core.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_core-2.3.0/stac_fastapi/core/utilities.py` & `stac_fastapi_core-2.3.1/stac_fastapi/core/utilities.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_core-2.3.0/stac_fastapi.core.egg-info/PKG-INFO` & `stac_fastapi_core-2.3.1/stac_fastapi.core.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.core
-Version: 2.3.0
+Version: 2.3.1
 Summary: Core library for the Elasticsearch and Opensearch stac-fastapi backends.
 Home-page: https://github.com/stac-utils/stac-fastapi-elasticsearch-opensearch
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
@@ -14,17 +14,18 @@
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: fastapi
 Requires-Dist: attrs
 Requires-Dist: pydantic[dotenv]<2
 Requires-Dist: stac_pydantic==2.0.*
-Requires-Dist: stac-fastapi.types==2.5.3
-Requires-Dist: stac-fastapi.api==2.5.3
-Requires-Dist: stac-fastapi.extensions==2.5.3
+Requires-Dist: stac-fastapi.types==2.5.5.post1
+Requires-Dist: stac-fastapi.api==2.5.5.post1
+Requires-Dist: stac-fastapi.extensions==2.5.5.post1
 Requires-Dist: pystac[validation]
 Requires-Dist: orjson
 Requires-Dist: overrides
 Requires-Dist: geojson-pydantic
 Requires-Dist: pygeofilter==0.2.1
+Requires-Dist: typing_extensions==4.4.0
 
 # stac-fastapi core library for Elasticsearch and Opensearch backends
```

### Comparing `stac_fastapi_core-2.3.0/stac_fastapi.core.egg-info/SOURCES.txt` & `stac_fastapi_core-2.3.1/stac_fastapi.core.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 stac_fastapi.core.egg-info/dependency_links.txt
 stac_fastapi.core.egg-info/not-zip-safe
 stac_fastapi.core.egg-info/requires.txt
 stac_fastapi.core.egg-info/top_level.txt
 stac_fastapi/core/__init__.py
 stac_fastapi/core/base_database_logic.py
 stac_fastapi/core/base_settings.py
+stac_fastapi/core/basic_auth.py
 stac_fastapi/core/core.py
 stac_fastapi/core/datetime_utils.py
 stac_fastapi/core/serializers.py
 stac_fastapi/core/session.py
 stac_fastapi/core/utilities.py
 stac_fastapi/core/version.py
 stac_fastapi/core/extensions/__init__.py
```

