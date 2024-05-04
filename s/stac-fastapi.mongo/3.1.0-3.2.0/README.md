# Comparing `tmp/stac_fastapi_mongo-3.1.0.tar.gz` & `tmp/stac_fastapi_mongo-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_fastapi_mongo-3.1.0.tar", last modified: Fri Apr 26 04:56:31 2024, max compression
+gzip compressed data, was "stac_fastapi_mongo-3.2.0.tar", last modified: Sat May  4 15:46:21 2024, max compression
```

## Comparing `stac_fastapi_mongo-3.1.0.tar` & `stac_fastapi_mongo-3.2.0.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-26 04:56:30.960650 stac_fastapi_mongo-3.1.0/
--rw-r--r--   0 primeradiant   (501) staff       (20)     1071 2024-03-03 16:18:26.000000 stac_fastapi_mongo-3.1.0/LICENSE
--rw-r--r--   0 primeradiant   (501) staff       (20)       42 2024-03-10 17:01:51.000000 stac_fastapi_mongo-3.1.0/MANIFEST.in
--rw-r--r--   0 primeradiant   (501) staff       (20)     6330 2024-04-26 04:56:30.949797 stac_fastapi_mongo-3.1.0/PKG-INFO
--rw-r--r--   0 primeradiant   (501) staff       (20)     4938 2024-04-26 04:44:59.000000 stac_fastapi_mongo-3.1.0/README.md
--rw-r--r--   0 primeradiant   (501) staff       (20)       38 2024-04-26 04:56:30.961627 stac_fastapi_mongo-3.1.0/setup.cfg
--rw-r--r--   0 primeradiant   (501) staff       (20)     1527 2024-04-26 04:45:17.000000 stac_fastapi_mongo-3.1.0/setup.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-26 04:56:30.813793 stac_fastapi_mongo-3.1.0/stac_fastapi/
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-26 04:56:30.931146 stac_fastapi_mongo-3.1.0/stac_fastapi/mongo/
--rw-r--r--   0 primeradiant   (501) staff       (20)       25 2024-04-13 13:01:33.000000 stac_fastapi_mongo-3.1.0/stac_fastapi/mongo/__init__.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     3077 2024-04-26 04:44:59.000000 stac_fastapi_mongo-3.1.0/stac_fastapi/mongo/app.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     3741 2024-04-26 04:44:59.000000 stac_fastapi_mongo-3.1.0/stac_fastapi/mongo/basic_auth.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     2477 2024-04-13 13:01:33.000000 stac_fastapi_mongo-3.1.0/stac_fastapi/mongo/config.py
--rw-r--r--   0 primeradiant   (501) staff       (20)    40317 2024-04-26 04:44:59.000000 stac_fastapi_mongo-3.1.0/stac_fastapi/mongo/database_logic.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     2911 2024-04-26 04:44:59.000000 stac_fastapi_mongo-3.1.0/stac_fastapi/mongo/utilities.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-04-26 04:56:30.933967 stac_fastapi_mongo-3.1.0/stac_fastapi.mongo.egg-info/
--rw-r--r--   0 primeradiant   (501) staff       (20)     6330 2024-04-26 04:56:30.000000 stac_fastapi_mongo-3.1.0/stac_fastapi.mongo.egg-info/PKG-INFO
--rw-r--r--   0 primeradiant   (501) staff       (20)      521 2024-04-26 04:56:30.000000 stac_fastapi_mongo-3.1.0/stac_fastapi.mongo.egg-info/SOURCES.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-04-26 04:56:30.000000 stac_fastapi_mongo-3.1.0/stac_fastapi.mongo.egg-info/dependency_links.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)       66 2024-04-26 04:56:30.000000 stac_fastapi_mongo-3.1.0/stac_fastapi.mongo.egg-info/entry_points.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-04-15 06:55:54.000000 stac_fastapi_mongo-3.1.0/stac_fastapi.mongo.egg-info/not-zip-safe
--rw-r--r--   0 primeradiant   (501) staff       (20)      244 2024-04-26 04:56:30.000000 stac_fastapi_mongo-3.1.0/stac_fastapi.mongo.egg-info/requires.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)       59 2024-04-26 04:56:30.000000 stac_fastapi_mongo-3.1.0/stac_fastapi.mongo.egg-info/top_level.txt
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-04 15:46:20.993304 stac_fastapi_mongo-3.2.0/
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1071 2024-03-03 16:18:26.000000 stac_fastapi_mongo-3.2.0/LICENSE
+-rw-r--r--   0 primeradiant   (501) staff       (20)       42 2024-03-10 17:01:51.000000 stac_fastapi_mongo-3.2.0/MANIFEST.in
+-rw-r--r--   0 primeradiant   (501) staff       (20)     6330 2024-05-04 15:46:20.992140 stac_fastapi_mongo-3.2.0/PKG-INFO
+-rw-r--r--   0 primeradiant   (501) staff       (20)     4938 2024-04-26 04:44:59.000000 stac_fastapi_mongo-3.2.0/README.md
+-rw-r--r--   0 primeradiant   (501) staff       (20)       38 2024-05-04 15:46:20.993462 stac_fastapi_mongo-3.2.0/setup.cfg
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1527 2024-05-04 15:45:48.000000 stac_fastapi_mongo-3.2.0/setup.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-04 15:46:20.936392 stac_fastapi_mongo-3.2.0/stac_fastapi/
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-04 15:46:20.983424 stac_fastapi_mongo-3.2.0/stac_fastapi/mongo/
+-rw-r--r--   0 primeradiant   (501) staff       (20)       25 2024-04-13 13:01:33.000000 stac_fastapi_mongo-3.2.0/stac_fastapi/mongo/__init__.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     3076 2024-05-04 15:45:48.000000 stac_fastapi_mongo-3.2.0/stac_fastapi/mongo/app.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     2477 2024-04-13 13:01:33.000000 stac_fastapi_mongo-3.2.0/stac_fastapi/mongo/config.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)    40317 2024-04-26 04:44:59.000000 stac_fastapi_mongo-3.2.0/stac_fastapi/mongo/database_logic.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     2911 2024-04-26 04:44:59.000000 stac_fastapi_mongo-3.2.0/stac_fastapi/mongo/utilities.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-04 15:46:20.985799 stac_fastapi_mongo-3.2.0/stac_fastapi.mongo.egg-info/
+-rw-r--r--   0 primeradiant   (501) staff       (20)     6330 2024-05-04 15:46:20.000000 stac_fastapi_mongo-3.2.0/stac_fastapi.mongo.egg-info/PKG-INFO
+-rw-r--r--   0 primeradiant   (501) staff       (20)      488 2024-05-04 15:46:20.000000 stac_fastapi_mongo-3.2.0/stac_fastapi.mongo.egg-info/SOURCES.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-05-04 15:46:20.000000 stac_fastapi_mongo-3.2.0/stac_fastapi.mongo.egg-info/dependency_links.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)       66 2024-05-04 15:46:20.000000 stac_fastapi_mongo-3.2.0/stac_fastapi.mongo.egg-info/entry_points.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-04-15 06:55:54.000000 stac_fastapi_mongo-3.2.0/stac_fastapi.mongo.egg-info/not-zip-safe
+-rw-r--r--   0 primeradiant   (501) staff       (20)      244 2024-05-04 15:46:20.000000 stac_fastapi_mongo-3.2.0/stac_fastapi.mongo.egg-info/requires.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)       59 2024-05-04 15:46:20.000000 stac_fastapi_mongo-3.2.0/stac_fastapi.mongo.egg-info/top_level.txt
```

### Comparing `stac_fastapi_mongo-3.1.0/LICENSE` & `stac_fastapi_mongo-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stac_fastapi_mongo-3.1.0/PKG-INFO` & `stac_fastapi_mongo-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.mongo
-Version: 3.1.0
+Version: 3.2.0
 Summary: Mongodb stac-fastapi backend.
 Home-page: https://github.com/Healy-Hyperspatial/stac-fastapi-mongo
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: stac-fastapi.core==2.3.0
+Requires-Dist: stac-fastapi.core==2.4.0
 Requires-Dist: motor==3.3.2
 Requires-Dist: pymongo==4.6.2
 Requires-Dist: uvicorn
 Requires-Dist: starlette
 Requires-Dist: typing_extensions==4.4.0
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `stac_fastapi_mongo-3.1.0/README.md` & `stac_fastapi_mongo-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `stac_fastapi_mongo-3.1.0/setup.py` & `stac_fastapi_mongo-3.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import find_namespace_packages, setup
 
 with open("README.md") as f:
     desc = f.read()
 
 install_requires = [
-    "stac-fastapi.core==2.3.0",
+    "stac-fastapi.core==2.4.0",
     "motor==3.3.2",
     "pymongo==4.6.2",
     "uvicorn",
     "starlette",
     "typing_extensions==4.4.0",
 ]
 
@@ -26,15 +26,15 @@
     ],
     "docs": ["mkdocs", "mkdocs-material", "pdocs"],
     "server": ["uvicorn[standard]==0.19.0"],
 }
 
 setup(
     name="stac-fastapi.mongo",
-    version="3.1.0",
+    version="3.2.0",
     description="Mongodb stac-fastapi backend.",
     long_description=desc,
     long_description_content_type="text/markdown",
     python_requires=">=3.8",
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
```

### Comparing `stac_fastapi_mongo-3.1.0/stac_fastapi/mongo/app.py` & `stac_fastapi_mongo-3.2.0/stac_fastapi/mongo/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """FastAPI application."""
 
 from stac_fastapi.api.app import StacApi
 from stac_fastapi.api.models import create_get_request_model, create_post_request_model
+from stac_fastapi.core.basic_auth import apply_basic_auth
 from stac_fastapi.core.core import (  # BulkTransactionsClient,
     CoreClient,
     EsAsyncBaseFiltersClient,
     TransactionsClient,
 )
 from stac_fastapi.core.extensions import QueryExtension
 from stac_fastapi.core.session import Session
@@ -13,15 +14,14 @@
     ContextExtension,
     FieldsExtension,
     FilterExtension,
     SortExtension,
     TokenPaginationExtension,
     TransactionExtension,
 )
-from stac_fastapi.mongo.basic_auth import apply_basic_auth
 
 # from stac_fastapi.extensions.third_party import BulkTransactionExtension
 from stac_fastapi.mongo.config import AsyncMongoDBSettings
 from stac_fastapi.mongo.database_logic import (
     DatabaseLogic,
     create_collection_index,
     create_item_index,
```

### Comparing `stac_fastapi_mongo-3.1.0/stac_fastapi/mongo/config.py` & `stac_fastapi_mongo-3.2.0/stac_fastapi/mongo/config.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_mongo-3.1.0/stac_fastapi/mongo/database_logic.py` & `stac_fastapi_mongo-3.2.0/stac_fastapi/mongo/database_logic.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_mongo-3.1.0/stac_fastapi/mongo/utilities.py` & `stac_fastapi_mongo-3.2.0/stac_fastapi/mongo/utilities.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_mongo-3.1.0/stac_fastapi.mongo.egg-info/PKG-INFO` & `stac_fastapi_mongo-3.2.0/stac_fastapi.mongo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.mongo
-Version: 3.1.0
+Version: 3.2.0
 Summary: Mongodb stac-fastapi backend.
 Home-page: https://github.com/Healy-Hyperspatial/stac-fastapi-mongo
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: stac-fastapi.core==2.3.0
+Requires-Dist: stac-fastapi.core==2.4.0
 Requires-Dist: motor==3.3.2
 Requires-Dist: pymongo==4.6.2
 Requires-Dist: uvicorn
 Requires-Dist: starlette
 Requires-Dist: typing_extensions==4.4.0
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
```

