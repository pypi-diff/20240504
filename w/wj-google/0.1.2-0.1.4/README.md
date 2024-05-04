# Comparing `tmp/wj_google-0.1.2.tar.gz` & `tmp/wj_google-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wj_google-0.1.2.tar", max compression
+gzip compressed data, was "wj_google-0.1.4.tar", max compression
```

## Comparing `wj_google-0.1.2.tar` & `wj_google-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     5429 2024-04-23 01:58:59.402346 wj_google-0.1.2/README.md
--rw-r--r--   0        0        0      584 2024-04-23 01:58:59.402346 wj_google-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-23 01:58:59.426345 wj_google-0.1.2/wj_google/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 01:58:59.426345 wj_google-0.1.2/wj_google/examples/__init__.py
--rw-r--r--   0        0        0     1961 2024-04-23 01:58:59.403346 wj_google-0.1.2/wj_google/examples/bigquery.py
--rw-r--r--   0        0        0     2736 2024-04-23 01:58:59.403346 wj_google-0.1.2/wj_google/examples/sorage_and_drive.py
--rw-r--r--   0        0        0     1522 2024-04-23 01:58:59.403346 wj_google-0.1.2/wj_google/google_api/Google.py
--rw-r--r--   0        0        0        0 2024-04-23 01:58:59.426345 wj_google-0.1.2/wj_google/google_api/__init__.py
--rw-r--r--   0        0        0     1985 2024-04-23 01:58:59.403346 wj_google-0.1.2/wj_google/google_api/google_api.py
--rw-r--r--   0        0        0        0 2024-04-23 01:58:59.426345 wj_google-0.1.2/wj_google/google_cloud/__init__.py
--rw-r--r--   0        0        0     5249 2024-04-23 01:58:59.403346 wj_google-0.1.2/wj_google/google_cloud/cloud_connector.py
--rw-r--r--   0        0        0     3227 2024-04-23 01:58:59.403346 wj_google-0.1.2/wj_google/main.py
--rw-r--r--   0        0        0        0 2024-04-23 01:58:59.426345 wj_google-0.1.2/wj_google/tools/__init__.py
--rw-r--r--   0        0        0      384 2024-04-23 01:58:59.404346 wj_google-0.1.2/wj_google/tools/files_manage.py
--rw-r--r--   0        0        0     6269 1970-01-01 00:00:00.000000 wj_google-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     5053 2024-05-04 02:13:59.538706 wj_google-0.1.4/README.md
+-rw-r--r--   0        0        0      585 2024-05-04 02:13:59.539706 wj_google-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-04 02:13:59.564706 wj_google-0.1.4/wj_google/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-04 02:13:59.564706 wj_google-0.1.4/wj_google/examples/__init__.py
+-rw-r--r--   0        0        0     1961 2024-05-04 02:13:59.539706 wj_google-0.1.4/wj_google/examples/bigquery.py
+-rw-r--r--   0        0        0     2736 2024-05-04 02:13:59.539706 wj_google-0.1.4/wj_google/examples/sorage_and_drive.py
+-rw-r--r--   0        0        0     1522 2024-05-04 02:13:59.539706 wj_google-0.1.4/wj_google/google_api/Google.py
+-rw-r--r--   0        0        0        0 2024-05-04 02:13:59.564706 wj_google-0.1.4/wj_google/google_api/__init__.py
+-rw-r--r--   0        0        0     1985 2024-05-04 02:13:59.539706 wj_google-0.1.4/wj_google/google_api/google_api.py
+-rw-r--r--   0        0        0        0 2024-05-04 02:13:59.564706 wj_google-0.1.4/wj_google/google_cloud/__init__.py
+-rw-r--r--   0        0        0     5251 2024-05-04 02:13:59.539706 wj_google-0.1.4/wj_google/google_cloud/cloud_connector.py
+-rw-r--r--   0        0        0     3227 2024-05-04 02:13:59.539706 wj_google-0.1.4/wj_google/main.py
+-rw-r--r--   0        0        0        0 2024-05-04 02:13:59.564706 wj_google-0.1.4/wj_google/tools/__init__.py
+-rw-r--r--   0        0        0      384 2024-05-04 02:13:59.539706 wj_google-0.1.4/wj_google/tools/files_manage.py
+-rw-r--r--   0        0        0     5836 1970-01-01 00:00:00.000000 wj_google-0.1.4/PKG-INFO
```

### Comparing `wj_google-0.1.2/README.md` & `wj_google-0.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,19 @@
 # wj_google
+## Connection to GCP
+In order to use the client, you need a json [credentials](https://cloud.google.com/docs/authentication/application-default-credentials?hl=es-419) from the google project. The first time to connect to a service, It is necessary to authorize the app through the browser.
 
-
-
-## Getting started
-### Poetry
-To make more easy the instalation, is recomended use [Poetry](https://python-poetry.org/docs/), follow the instructions, and then use the command:
-```
-poetry install
-```
-To activate the vierual enviroment use:
-```
-poetry shell
-```
-### Virtual Enviroment
-Or you can use your own virtual enviroment, and install the requirements:
-```
-python -m venv <env_name>
-<env_name>/scripts/activate
-pip install -r requirements.txt
-```
-### Connection to GCP
-Is important consult the documentation of GCP, is required obtain the json credentials with the permission to use the resource that is going to use. ***
 ## Supported services
 
 The currently supported services are:
 - Google Drive
 - Buckets
-- BigQuery (just sql consults)***
+- BigQuery
 
-### Google Drive
+## Google Drive
 The GCP account must have Google Drive API enabled, and make sure that you have a OAuth 2.0 application created, in Google Cloud console, you can see the [documentation](https://developers.google.com/drive/api/guides/about-sdk?hl=es-419).
 
 The following methods are currently supported:
 - Upload files
 - Download files
 - Create directory
 You must The package must be instantiated as follows:
@@ -44,15 +25,15 @@
     api_name=API_NAME, -> drive in this case
     api_version=API_VERSION, -> Current version, 3 in this case
     scopes=GOOGLE_DRIVE_SCOPES, -> Scope of drive see doc
 )
 ```
 There are diferent scopes, as you can see in the [documentation](https://developers.google.com/drive/api/guides/api-specific-auth?hl=es-419).
 
-### Google Drive
+## Google Drive
 The GCP account must have Google Drive API enabled, and make sure that you have a OAuth 2.0 application created, in Google Cloud console, you can see the [documentation](https://developers.google.com/drive/api/guides/about-sdk?hl=es-419).
 
 The following methods are currently supported:
 - Upload files
 - Download files
 - Create directory
 
@@ -65,37 +46,37 @@
     api_name=API_NAME, -> drive in this case
     api_version=API_VERSION, -> Current version, 3 in this case
     scopes=GOOGLE_DRIVE_SCOPES, -> Scope of drive see doc
 )
 ```
 There are diferent scopes, as you can see in the [documentation](https://developers.google.com/drive/api/guides/api-specific-auth?hl=es-419).
 
-#### Uploading a file:
+### Uploading a file:
 ```
 googleApi.upload_files_to_drive(
     folder_id, -> Id from the drive of the directory 
     file_paths, -> Path of yur file
     mime_types -> Type of file
 )
 ```
-#### Downloading a file:
+### Downloading a file:
 ```
 googleApi.download_files_drive(
     file_ids -> Google Drive id file, you can find it in the uri
     file_names -> Name given in your local
 )
 ```
-#### Creating a directory:
+### Creating a directory:
 ```
 googleApi.create_directory_drive(
     directory_name
 )
 ```
 
-### Google storage buckets
+## Google storage buckets
 
 This resource can be used with the credentials of a service user, you see de [documentation](https://cloud.google.com/iam/docs/manage-access-service-accounts?hl=es).
 
 The following methods are currently supported:
 - Upload files
 - Download files
 - Create directory
@@ -104,81 +85,81 @@
 ```
 from wj_google.google_cloud.cloud_connector import GoogleStorage
 googleStorageClient = GoogleStorage(
     service -> STORAGE in this case and for now***
     credentials
 )
 ```
-#### Uploading a file:
+### Uploading a file:
 ```
 googleStorageClient.upload_file(
     bucket_name -> Destination bucket 
     source_file_name -> Path of the file to upload
     destination_file_name Name of the file in bucket
 )
 ```
-#### Downloading a file:
+### Downloading a file:
 ```
 googleStorageClient.download_file(
     bucket_name -> bucket file
     file_name -> name and path in the bucket
     destination_file -> name and path in your local of the file
 )
 ```
-#### Creating a bucket:
+### Creating a bucket:
 ```
 googleStorageClient.create_bucket(
     bucket_name,
     storage_class, -> Optional, to define the type of bucket to use
     location, -> Optional, to define in which region the bucket is hosted 
 )
 ```
-#### Listing bucket's files:
+### Listing bucket's files:
 ```
 googleStorageClient.list_files(bucket_name)
 ```
 
-### Google BigQuery
+## Google BigQuery
 This resource can be used with the credentials of a service user, you see de [documentation](https://cloud.google.com/python/docs/reference/bigquery/latest).
 
 
 With the credentials are required. After which the resource is instantiated, in this case just execute the query.
 ```
 from google_cloud.cloud_connector import GoogleBigQuery
 
 bigquery = GoogleBigQuery(
     service=BIGQUERY,
     credentials=GOOGLE_BIGQUEY_CREDENTIALS,
     scopes=scopes -> To use services like Google Drive
 )
 
 ```
-#### Do a consult:
+### Do a consult:
 
 ```
 query = 'YOUR_SQL_QUERY'
 sql_job = bigquery.sql_query(query=query)
 ```
 
 You can iterate over the sql_job:
 ```
 for item in sql_job:
     print(item.name)
 ```
 
-#### Add label to bigquery table:
+### Add label to bigquery table:
 
 ```
 labels = {
     "type": "social_media",
     "category": "cloud",
 }
 bigquery = GoogleBigQuery(service=BIGQUERY, credentials=GOOGLE_BIGQUEY_CREDENTIALS)
 bigquery.add_table_labels(
     labels=labels, dataset_name=dataset_name, table_name=table_name
 )
 
 ```
-#### Delete label to bigquery table:
+### Delete label to bigquery table:
 ```
 delete_labels_in_table(dataset_name, table_name)
 ```
```

### Comparing `wj_google-0.1.2/pyproject.toml` & `wj_google-0.1.4/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "wj-google"
-version = "0.1.2"
+version = "0.1.4"
 description = ""
 authors = ["Johan <mantimanti89@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "wj_google" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.9"
 google = "^3.0.0"
 google-api-python-client = "^2.121.0"
 google-auth-oauthlib = "^1.2.0"
 python-dotenv = "^1.0.1"
 google-cloud-storage = "^2.15.0"
-flake8 = "^7.0.0"
-black = "^24.2.0"
 google-cloud-bigquery = "^3.18.0"
-pandas = "^2.2.1"
 db-dtypes = "^1.2.0"
-pytest = "^8.1.1"
 
 
+[tool.poetry.group.dev.dependencies]
+pytest = "^8.2.0"
+black = "^24.4.2"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `wj_google-0.1.2/wj_google/examples/bigquery.py` & `wj_google-0.1.4/wj_google/examples/bigquery.py`

 * *Files identical despite different names*

### Comparing `wj_google-0.1.2/wj_google/examples/sorage_and_drive.py` & `wj_google-0.1.4/wj_google/examples/sorage_and_drive.py`

 * *Files identical despite different names*

### Comparing `wj_google-0.1.2/wj_google/google_api/Google.py` & `wj_google-0.1.4/wj_google/google_api/Google.py`

 * *Files identical despite different names*

### Comparing `wj_google-0.1.2/wj_google/google_api/google_api.py` & `wj_google-0.1.4/wj_google/google_api/google_api.py`

 * *Files identical despite different names*

### Comparing `wj_google-0.1.2/wj_google/google_cloud/cloud_connector.py` & `wj_google-0.1.4/wj_google/google_cloud/cloud_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 import time
 from typing import List, Any, Tuple, Dict, Optional
 from google.cloud import storage
 from google.cloud.storage import Bucket
 from google.cloud import bigquery
 import os
-#from ..tools.files_manage import insert_data_in_df
+
+# from ..tools.files_manage import insert_data_in_df
 
 
 class GoogleCloud:
 
     def __init__(
         self, service: str, credentials: str, scopes: Optional[List[str]] = None
     ) -> None:
@@ -137,21 +138,21 @@
             job_config=query_job_config,
         )
 
         while query_job.state != "DONE":
             time.sleep(1)
             query_job.reload()
 
-    '''def export_queries_to_excel(self, queries: List[str]):
+    """def export_queries_to_excel(self, queries: List[str]):
         xl_app = win32.Dispatch("Excel.Application")
         xl_app.Visible = True
         wb = xl_app.Workbooks.Add()
 
         for query in queries:
             query_job = self.bigquery_client.query(query)
             while query_job.state != "DONE":
                 time.sleep(1)
                 query_job.reload()
             response = query_job.result(max_results=None)
             dataframe = response.to_dataframe()
             worksheet = wb.Worksheets.Add()
-            insert_data_in_df(worksheet=worksheet, dataframe=dataframe)'''
+            insert_data_in_df(worksheet=worksheet, dataframe=dataframe)"""
```

### Comparing `wj_google-0.1.2/wj_google/main.py` & `wj_google-0.1.4/wj_google/main.py`

 * *Files identical despite different names*

### Comparing `wj_google-0.1.2/PKG-INFO` & `wj_google-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,40 @@
 Metadata-Version: 2.1
 Name: wj-google
-Version: 0.1.2
+Version: 0.1.4
 Summary: 
 Author: Johan
 Author-email: mantimanti89@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: black (>=24.2.0,<25.0.0)
 Requires-Dist: db-dtypes (>=1.2.0,<2.0.0)
-Requires-Dist: flake8 (>=7.0.0,<8.0.0)
 Requires-Dist: google (>=3.0.0,<4.0.0)
 Requires-Dist: google-api-python-client (>=2.121.0,<3.0.0)
 Requires-Dist: google-auth-oauthlib (>=1.2.0,<2.0.0)
 Requires-Dist: google-cloud-bigquery (>=3.18.0,<4.0.0)
 Requires-Dist: google-cloud-storage (>=2.15.0,<3.0.0)
-Requires-Dist: pandas (>=2.2.1,<3.0.0)
-Requires-Dist: pytest (>=8.1.1,<9.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # wj_google
+## Connection to GCP
+In order to use the client, you need a json [credentials](https://cloud.google.com/docs/authentication/application-default-credentials?hl=es-419) from the google project. The first time to connect to a service, It is necessary to authorize the app through the browser.
 
-
-
-## Getting started
-### Poetry
-To make more easy the instalation, is recomended use [Poetry](https://python-poetry.org/docs/), follow the instructions, and then use the command:
-```
-poetry install
-```
-To activate the vierual enviroment use:
-```
-poetry shell
-```
-### Virtual Enviroment
-Or you can use your own virtual enviroment, and install the requirements:
-```
-python -m venv <env_name>
-<env_name>/scripts/activate
-pip install -r requirements.txt
-```
-### Connection to GCP
-Is important consult the documentation of GCP, is required obtain the json credentials with the permission to use the resource that is going to use. ***
 ## Supported services
 
 The currently supported services are:
 - Google Drive
 - Buckets
-- BigQuery (just sql consults)***
+- BigQuery
 
-### Google Drive
+## Google Drive
 The GCP account must have Google Drive API enabled, and make sure that you have a OAuth 2.0 application created, in Google Cloud console, you can see the [documentation](https://developers.google.com/drive/api/guides/about-sdk?hl=es-419).
 
 The following methods are currently supported:
 - Upload files
 - Download files
 - Create directory
 You must The package must be instantiated as follows:
@@ -67,15 +46,15 @@
     api_name=API_NAME, -> drive in this case
     api_version=API_VERSION, -> Current version, 3 in this case
     scopes=GOOGLE_DRIVE_SCOPES, -> Scope of drive see doc
 )
 ```
 There are diferent scopes, as you can see in the [documentation](https://developers.google.com/drive/api/guides/api-specific-auth?hl=es-419).
 
-### Google Drive
+## Google Drive
 The GCP account must have Google Drive API enabled, and make sure that you have a OAuth 2.0 application created, in Google Cloud console, you can see the [documentation](https://developers.google.com/drive/api/guides/about-sdk?hl=es-419).
 
 The following methods are currently supported:
 - Upload files
 - Download files
 - Create directory
 
@@ -88,37 +67,37 @@
     api_name=API_NAME, -> drive in this case
     api_version=API_VERSION, -> Current version, 3 in this case
     scopes=GOOGLE_DRIVE_SCOPES, -> Scope of drive see doc
 )
 ```
 There are diferent scopes, as you can see in the [documentation](https://developers.google.com/drive/api/guides/api-specific-auth?hl=es-419).
 
-#### Uploading a file:
+### Uploading a file:
 ```
 googleApi.upload_files_to_drive(
     folder_id, -> Id from the drive of the directory 
     file_paths, -> Path of yur file
     mime_types -> Type of file
 )
 ```
-#### Downloading a file:
+### Downloading a file:
 ```
 googleApi.download_files_drive(
     file_ids -> Google Drive id file, you can find it in the uri
     file_names -> Name given in your local
 )
 ```
-#### Creating a directory:
+### Creating a directory:
 ```
 googleApi.create_directory_drive(
     directory_name
 )
 ```
 
-### Google storage buckets
+## Google storage buckets
 
 This resource can be used with the credentials of a service user, you see de [documentation](https://cloud.google.com/iam/docs/manage-access-service-accounts?hl=es).
 
 The following methods are currently supported:
 - Upload files
 - Download files
 - Create directory
@@ -127,82 +106,82 @@
 ```
 from wj_google.google_cloud.cloud_connector import GoogleStorage
 googleStorageClient = GoogleStorage(
     service -> STORAGE in this case and for now***
     credentials
 )
 ```
-#### Uploading a file:
+### Uploading a file:
 ```
 googleStorageClient.upload_file(
     bucket_name -> Destination bucket 
     source_file_name -> Path of the file to upload
     destination_file_name Name of the file in bucket
 )
 ```
-#### Downloading a file:
+### Downloading a file:
 ```
 googleStorageClient.download_file(
     bucket_name -> bucket file
     file_name -> name and path in the bucket
     destination_file -> name and path in your local of the file
 )
 ```
-#### Creating a bucket:
+### Creating a bucket:
 ```
 googleStorageClient.create_bucket(
     bucket_name,
     storage_class, -> Optional, to define the type of bucket to use
     location, -> Optional, to define in which region the bucket is hosted 
 )
 ```
-#### Listing bucket's files:
+### Listing bucket's files:
 ```
 googleStorageClient.list_files(bucket_name)
 ```
 
-### Google BigQuery
+## Google BigQuery
 This resource can be used with the credentials of a service user, you see de [documentation](https://cloud.google.com/python/docs/reference/bigquery/latest).
 
 
 With the credentials are required. After which the resource is instantiated, in this case just execute the query.
 ```
 from google_cloud.cloud_connector import GoogleBigQuery
 
 bigquery = GoogleBigQuery(
     service=BIGQUERY,
     credentials=GOOGLE_BIGQUEY_CREDENTIALS,
     scopes=scopes -> To use services like Google Drive
 )
 
 ```
-#### Do a consult:
+### Do a consult:
 
 ```
 query = 'YOUR_SQL_QUERY'
 sql_job = bigquery.sql_query(query=query)
 ```
 
 You can iterate over the sql_job:
 ```
 for item in sql_job:
     print(item.name)
 ```
 
-#### Add label to bigquery table:
+### Add label to bigquery table:
 
 ```
 labels = {
     "type": "social_media",
     "category": "cloud",
 }
 bigquery = GoogleBigQuery(service=BIGQUERY, credentials=GOOGLE_BIGQUEY_CREDENTIALS)
 bigquery.add_table_labels(
     labels=labels, dataset_name=dataset_name, table_name=table_name
 )
 
 ```
-#### Delete label to bigquery table:
+### Delete label to bigquery table:
 ```
 delete_labels_in_table(dataset_name, table_name)
 ```
```

