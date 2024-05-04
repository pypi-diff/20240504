# Comparing `tmp/gravitino-0.5.0.dev2.tar.gz` & `tmp/gravitino-0.5.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitino-0.5.0.dev2.tar", last modified: Sat May  4 01:20:16 2024, max compression
+gzip compressed data, was "gravitino-0.5.0.dev3.tar", last modified: Sat May  4 02:17:36 2024, max compression
```

## Comparing `gravitino-0.5.0.dev2.tar` & `gravitino-0.5.0.dev3.tar`

### file list

```diff
@@ -1,22 +1,96 @@
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 01:20:16.578039 gravitino-0.5.0.dev2/
--rw-r--r--   0 xun        (501) staff       (20)     3714 2024-05-04 01:20:16.577917 gravitino-0.5.0.dev2/PKG-INFO
--rw-r--r--   0 xun        (501) staff       (20)     3424 2024-05-03 12:21:44.000000 gravitino-0.5.0.dev2/README.md
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 01:20:16.576876 gravitino-0.5.0.dev2/gravitino/
--rw-r--r--   0 xun        (501) staff       (20)      244 2024-04-08 10:35:22.000000 gravitino-0.5.0.dev2/gravitino/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)      119 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev2/gravitino/constants.py
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev2/gravitino/exceptions.py
--rw-r--r--   0 xun        (501) staff       (20)     4404 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev2/gravitino/gravitino_client.py
--rw-r--r--   0 xun        (501) staff       (20)     9035 2024-05-01 10:39:47.000000 gravitino-0.5.0.dev2/gravitino/name_identifier.py
--rw-r--r--   0 xun        (501) staff       (20)     7608 2024-05-01 10:39:47.000000 gravitino-0.5.0.dev2/gravitino/namespace.py
--rw-r--r--   0 xun        (501) staff       (20)     2430 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev2/gravitino/service.py
--rw-r--r--   0 xun        (501) staff       (20)      318 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev2/gravitino/typing.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 01:20:16.577484 gravitino-0.5.0.dev2/gravitino.egg-info/
--rw-r--r--   0 xun        (501) staff       (20)     3714 2024-05-04 01:20:16.000000 gravitino-0.5.0.dev2/gravitino.egg-info/PKG-INFO
--rw-r--r--   0 xun        (501) staff       (20)      405 2024-05-04 01:20:16.000000 gravitino-0.5.0.dev2/gravitino.egg-info/SOURCES.txt
--rw-r--r--   0 xun        (501) staff       (20)        1 2024-05-04 01:20:16.000000 gravitino-0.5.0.dev2/gravitino.egg-info/dependency_links.txt
--rw-r--r--   0 xun        (501) staff       (20)       62 2024-05-04 01:20:16.000000 gravitino-0.5.0.dev2/gravitino.egg-info/requires.txt
--rw-r--r--   0 xun        (501) staff       (20)       10 2024-05-04 01:20:16.000000 gravitino-0.5.0.dev2/gravitino.egg-info/top_level.txt
--rw-r--r--   0 xun        (501) staff       (20)       38 2024-05-04 01:20:16.578091 gravitino-0.5.0.dev2/setup.cfg
--rw-r--r--   0 xun        (501) staff       (20)      722 2024-05-04 01:20:02.000000 gravitino-0.5.0.dev2/setup.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 01:20:16.577623 gravitino-0.5.0.dev2/tests/
--rw-r--r--   0 xun        (501) staff       (20)     2175 2024-04-13 14:55:38.000000 gravitino-0.5.0.dev2/tests/test_gravitino_client.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:17:36.932213 gravitino-0.5.0.dev3/
+-rw-r--r--   0 xun        (501) staff       (20)     3710 2024-05-04 02:17:36.932071 gravitino-0.5.0.dev3/PKG-INFO
+-rw-r--r--   0 xun        (501) staff       (20)     3420 2024-05-04 02:12:18.000000 gravitino-0.5.0.dev3/README.md
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:17:36.909958 gravitino-0.5.0.dev3/gravitino/
+-rw-r--r--   0 xun        (501) staff       (20)      244 2024-04-08 10:35:22.000000 gravitino-0.5.0.dev3/gravitino/__init__.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:17:36.915127 gravitino-0.5.0.dev3/gravitino/api/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev3/gravitino/api/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)      942 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev3/gravitino/api/audit.py
+-rw-r--r--   0 xun        (501) staff       (20)      440 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev3/gravitino/api/auditable.py
+-rw-r--r--   0 xun        (501) staff       (20)     4113 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev3/gravitino/api/catalog.py
+-rw-r--r--   0 xun        (501) staff       (20)     8759 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/api/catalog_change.py
+-rw-r--r--   0 xun        (501) staff       (20)     3556 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/api/fileset.py
+-rw-r--r--   0 xun        (501) staff       (20)     9226 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/api/fileset_change.py
+-rw-r--r--   0 xun        (501) staff       (20)     1155 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/api/metalake.py
+-rw-r--r--   0 xun        (501) staff       (20)     3403 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/api/metalake_change.py
+-rw-r--r--   0 xun        (501) staff       (20)     1044 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/api/schema.py
+-rw-r--r--   0 xun        (501) staff       (20)     4847 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/api/schema_change.py
+-rw-r--r--   0 xun        (501) staff       (20)     3870 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/api/supports_schemas.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:17:36.916385 gravitino-0.5.0.dev3/gravitino/client/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev3/gravitino/client/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     4651 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/client/gravitino_admin_client.py
+-rw-r--r--   0 xun        (501) staff       (20)     2739 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/client/gravitino_client.py
+-rw-r--r--   0 xun        (501) staff       (20)     2483 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/client/gravitino_client_base.py
+-rw-r--r--   0 xun        (501) staff       (20)     7664 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/client/gravitino_metalake.py
+-rw-r--r--   0 xun        (501) staff       (20)      408 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev3/gravitino/client/gravitino_version.py
+-rw-r--r--   0 xun        (501) staff       (20)      119 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev3/gravitino/constants.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:17:36.918388 gravitino-0.5.0.dev3/gravitino/dto/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev3/gravitino/dto/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     1753 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev3/gravitino/dto/audit_dto.py
+-rw-r--r--   0 xun        (501) staff       (20)     1590 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev3/gravitino/dto/catalog_dto.py
+-rw-r--r--   0 xun        (501) staff       (20)     3019 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/dto_converters.py
+-rw-r--r--   0 xun        (501) staff       (20)     1313 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/fileset_dto.py
+-rw-r--r--   0 xun        (501) staff       (20)     1883 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/metalake_dto.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:17:36.921150 gravitino-0.5.0.dev3/gravitino/dto/requests/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev3/gravitino/dto/requests/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     1560 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/requests/catalog_create_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     2534 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/requests/catalog_update_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     1065 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/requests/catalog_updates_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     1438 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/requests/fileset_create_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     4267 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/requests/fileset_update_request.py
+-rw-r--r--   0 xun        (501) staff       (20)      750 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/requests/fileset_updates_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     1070 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/requests/metalake_create_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     4145 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/requests/metalake_update_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     1029 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/requests/metalake_updates_request.py
+-rw-r--r--   0 xun        (501) staff       (20)      908 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/requests/schema_create_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     2519 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/requests/schema_update_request.py
+-rw-r--r--   0 xun        (501) staff       (20)      990 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/requests/schema_updates_request.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:17:36.925235 gravitino-0.5.0.dev3/gravitino/dto/responses/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev3/gravitino/dto/responses/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)      683 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/responses/base_response.py
+-rw-r--r--   0 xun        (501) staff       (20)      573 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/responses/catalog_list_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1051 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev3/gravitino/dto/responses/catalog_response.py
+-rw-r--r--   0 xun        (501) staff       (20)      476 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev3/gravitino/dto/responses/drop_response.py
+-rw-r--r--   0 xun        (501) staff       (20)      871 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/responses/entity_list_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1061 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/responses/fileset_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1162 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/responses/metalake_list_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1063 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/responses/metalake_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1058 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/responses/schema_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1382 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/schema_dto.py
+-rw-r--r--   0 xun        (501) staff       (20)      431 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev3/gravitino/dto/version_dto.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:17:36.927237 gravitino-0.5.0.dev3/gravitino/exceptions/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev3/gravitino/exceptions/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)      302 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/exceptions/gravitino_runtime_exception.py
+-rw-r--r--   0 xun        (501) staff       (20)      363 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/exceptions/illegal_name_identifier_exception.py
+-rw-r--r--   0 xun        (501) staff       (20)      352 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/exceptions/illegal_namespace_exception.py
+-rw-r--r--   0 xun        (501) staff       (20)      288 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/exceptions/no_such_metalake_exception.py
+-rw-r--r--   0 xun        (501) staff       (20)      323 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/exceptions/not_found_exception.py
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev3/gravitino/exceptions.py
+-rw-r--r--   0 xun        (501) staff       (20)     4404 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev3/gravitino/gravitino_client.py
+-rw-r--r--   0 xun        (501) staff       (20)     9268 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/name_identifier.py
+-rw-r--r--   0 xun        (501) staff       (20)     7603 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/namespace.py
+-rw-r--r--   0 xun        (501) staff       (20)     2430 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev3/gravitino/service.py
+-rw-r--r--   0 xun        (501) staff       (20)      318 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev3/gravitino/typing.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:17:36.928666 gravitino-0.5.0.dev3/gravitino/utils/
+-rw-r--r--   0 xun        (501) staff       (20)      175 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev3/gravitino/utils/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     2692 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/utils/exceptions.py
+-rw-r--r--   0 xun        (501) staff       (20)     5479 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/utils/http_client.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:17:36.911862 gravitino-0.5.0.dev3/gravitino.egg-info/
+-rw-r--r--   0 xun        (501) staff       (20)     3710 2024-05-04 02:17:36.000000 gravitino-0.5.0.dev3/gravitino.egg-info/PKG-INFO
+-rw-r--r--   0 xun        (501) staff       (20)     2881 2024-05-04 02:17:36.000000 gravitino-0.5.0.dev3/gravitino.egg-info/SOURCES.txt
+-rw-r--r--   0 xun        (501) staff       (20)        1 2024-05-04 02:17:36.000000 gravitino-0.5.0.dev3/gravitino.egg-info/dependency_links.txt
+-rw-r--r--   0 xun        (501) staff       (20)       69 2024-05-04 02:17:36.000000 gravitino-0.5.0.dev3/gravitino.egg-info/requires.txt
+-rw-r--r--   0 xun        (501) staff       (20)       16 2024-05-04 02:17:36.000000 gravitino-0.5.0.dev3/gravitino.egg-info/top_level.txt
+-rw-r--r--   0 xun        (501) staff       (20)       38 2024-05-04 02:17:36.932279 gravitino-0.5.0.dev3/setup.cfg
+-rw-r--r--   0 xun        (501) staff       (20)      627 2024-05-04 02:16:59.000000 gravitino-0.5.0.dev3/setup.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:17:36.929889 gravitino-0.5.0.dev3/tests/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev3/tests/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     3607 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev3/tests/fixtures.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:17:36.931703 gravitino-0.5.0.dev3/tests/integration/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev3/tests/integration/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     3768 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/tests/integration/integration_test_env.py
+-rw-r--r--   0 xun        (501) staff       (20)     7086 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/tests/integration/test_fileset_catalog.py
+-rw-r--r--   0 xun        (501) staff       (20)     6653 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/tests/integration/test_metalake.py
+-rw-r--r--   0 xun        (501) staff       (20)     6058 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/tests/integration/test_schema.py
+-rw-r--r--   0 xun        (501) staff       (20)     2175 2024-04-13 14:55:38.000000 gravitino-0.5.0.dev3/tests/test_gravitino_client.py
+-rw-r--r--   0 xun        (501) staff       (20)     1323 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev3/tests/utils.py
```

### Comparing `gravitino-0.5.0.dev2/PKG-INFO` & `gravitino-0.5.0.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gravitino
-Version: 0.5.0.dev2
+Version: 0.5.0.dev3
 Summary: Python lib/client for Gravitino
 Home-page: https://github.com/datastrato/gravitino
 Author: datastrato
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -47,15 +47,14 @@
 # Create a HDFS connector client
 client = InsecureClient('http://hive:50070', user='root')
 
 # List HDFS file and directories
 print(client.list('/'))
 ```
 
-
 ```python
 import gravitino
 
 gravitino_admin_client = GravitinoAdminClient(uri="http://localhost:8090")
 metalake = gravitino_admin_client.create_metalake(
     ident=NameIdentifier.of("default"),
     comment="metalake comment", properties={})
@@ -94,25 +93,25 @@
 
 # Development Environment
 
 1. Install dependency
     ```bash
     pip install -e '.[dev]'
     ```
-   
+
 2. Run integration tests
     ```bash
     cd gravitino
     ./gradlew compileDistribution -x test
     ./gradlew :clients:client-python:test
     ```
 
 ## Resources
 + Official website https://datastrato.ai/
-+ Project home on Github: https://github.com/datastrato/gravitino/ 
++ Project home on GitHub: https://github.com/datastrato/gravitino/ 
 + Playground with Docker: https://github.com/datastrato/gravitino-playground
 + User documentation: https://datastrato.ai/docs/
 + Videos on Youtube: https://www.youtube.com/@Datastrato
 + Twitter: https://twitter.com/datastrato
 + Linkedin: https://www.linkedin.com/company/datastrato
 + Slack Community: [https://join.slack.com/t/datastrato-community](https://join.slack.com/t/datastrato-community/shared_invite/zt-2a8vsjoch-cU_uUwHA_QU6Ab50thoq8w)
 + Discourse Community: https://gravitino.discourse.group/
```

### Comparing `gravitino-0.5.0.dev2/README.md` & `gravitino-0.5.0.dev3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 # Create a HDFS connector client
 client = InsecureClient('http://hive:50070', user='root')
 
 # List HDFS file and directories
 print(client.list('/'))
 ```
 
-
 ```python
 import gravitino
 
 gravitino_admin_client = GravitinoAdminClient(uri="http://localhost:8090")
 metalake = gravitino_admin_client.create_metalake(
     ident=NameIdentifier.of("default"),
     comment="metalake comment", properties={})
@@ -82,25 +81,25 @@
 
 # Development Environment
 
 1. Install dependency
     ```bash
     pip install -e '.[dev]'
     ```
-   
+
 2. Run integration tests
     ```bash
     cd gravitino
     ./gradlew compileDistribution -x test
     ./gradlew :clients:client-python:test
     ```
 
 ## Resources
 + Official website https://datastrato.ai/
-+ Project home on Github: https://github.com/datastrato/gravitino/ 
++ Project home on GitHub: https://github.com/datastrato/gravitino/ 
 + Playground with Docker: https://github.com/datastrato/gravitino-playground
 + User documentation: https://datastrato.ai/docs/
 + Videos on Youtube: https://www.youtube.com/@Datastrato
 + Twitter: https://twitter.com/datastrato
 + Linkedin: https://www.linkedin.com/company/datastrato
 + Slack Community: [https://join.slack.com/t/datastrato-community](https://join.slack.com/t/datastrato-community/shared_invite/zt-2a8vsjoch-cU_uUwHA_QU6Ab50thoq8w)
 + Discourse Community: https://gravitino.discourse.group/
```

### Comparing `gravitino-0.5.0.dev2/gravitino/gravitino_client.py` & `gravitino-0.5.0.dev3/gravitino/gravitino_client.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev2/gravitino/name_identifier.py` & `gravitino-0.5.0.dev3/gravitino/name_identifier.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 """
 Copyright 2024 Datastrato Pvt Ltd.
 This software is licensed under the Apache License version 2.
 """
+from dataclasses import dataclass, field
+
+from dataclasses_json import DataClassJsonMixin, config
+
 from gravitino.exceptions.illegal_name_identifier_exception import IllegalNameIdentifierException
 from gravitino.namespace import Namespace
 
 
-class NameIdentifier:
+@dataclass
+class NameIdentifier(DataClassJsonMixin):
     """A name identifier is a sequence of names separated by dots. It's used to identify a metalake, a
     catalog, a schema or a table. For example, "metalake1" can represent a metalake,
     "metalake1.catalog1" can represent a catalog, "metalake1.catalog1.schema1" can represent a
     schema.
     """
 
-    DOT: str = '.'
+    _name: str = field(metadata=config(field_name='name'))
+    _namespace: Namespace = field(metadata=config(field_name='namespace'))
 
-    _namespace: Namespace = None
-    _name: str = None
+    DOT: str = '.'
 
-    def __init__(self, namespace: Namespace, name: str):
-        self._namespace = namespace
-        self._name = name
+    @classmethod
+    def builder(cls, namespace: Namespace, name: str):
+        return NameIdentifier(_namespace=namespace, _name=name)
 
     def namespace(self):
         return self._namespace
 
     def name(self):
         return self._name
 
@@ -38,28 +43,28 @@
         Returns:
             The created NameIdentifier
         """
 
         NameIdentifier.check(names is not None, "Cannot create a NameIdentifier with null names")
         NameIdentifier.check(len(names) > 0, "Cannot create a NameIdentifier with no names")
 
-        return NameIdentifier(Namespace.of(*names[:-1]), names[-1])
+        return NameIdentifier.builder(Namespace.of(*names[:-1]), names[-1])
 
     @staticmethod
     def of_namespace(namespace: Namespace, name: str) -> 'NameIdentifier':
         """Create the NameIdentifier with the given Namespace and name.
 
         Args:
             namespace: The namespace of the identifier
             name: The name of the identifier
 
         Returns:
             The created NameIdentifier
         """
-        return NameIdentifier(namespace, name)
+        return NameIdentifier.builder(namespace, name)
 
     @staticmethod
     def of_metalake(metalake: str) -> 'NameIdentifier':
         """Create the metalake NameIdentifier with the given name.
 
         Args:
             metalake: The metalake name
@@ -233,37 +238,36 @@
 
     def get_namespace(self):
         """Get the namespace of the NameIdentifier.
 
         Returns:
             The namespace of the NameIdentifier.
         """
-        return self.namespace
+        return self._namespace
 
     def get_name(self):
         """Get the name of the NameIdentifier.
 
         Returns:
             The name of the NameIdentifier.
         """
-        return self.name
+        return self._name
 
     def __eq__(self, other):
         if not isinstance(other, NameIdentifier):
             return False
-        return self.namespace == other.namespace and self.name == other.name
+        return self._namespace == other._namespace and self._name == other._name
 
     def __hash__(self):
-        return hash((self.namespace, self.name))
+        return hash(self._namespace, self._name)
 
     def __str__(self):
         if self.has_namespace():
-            return str(self.namespace) + "." + self.name
-        else:
-            return self.name
+            return str(self._namespace) + "." + self._name
+        return self._name
 
     @staticmethod
     def check(condition, message, *args):
         """Check the given condition is true. Throw an {@link IllegalNameIdentifierException} if it's not.
 
         Args:
             condition: The condition to check.
```

### Comparing `gravitino-0.5.0.dev2/gravitino/namespace.py` & `gravitino-0.5.0.dev3/gravitino/namespace.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,15 @@
             return False
         return self._levels == other._levels
 
     def __hash__(self) -> int:
         return hash(tuple(self._levels))
 
     def __str__(self) -> str:
-        return Namespace._DOT.join(self._levels)
+        return self._DOT.join(self._levels)
 
     @staticmethod
     def check(expression: bool, message: str, *args) -> None:
         """Check the given condition is true. Throw an IllegalNamespaceException if it's not.
 
         Args:
             expression: The expression to check.
```

### Comparing `gravitino-0.5.0.dev2/gravitino/service.py` & `gravitino-0.5.0.dev3/gravitino/service.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev2/gravitino.egg-info/PKG-INFO` & `gravitino-0.5.0.dev3/gravitino.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gravitino
-Version: 0.5.0.dev2
+Version: 0.5.0.dev3
 Summary: Python lib/client for Gravitino
 Home-page: https://github.com/datastrato/gravitino
 Author: datastrato
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -47,15 +47,14 @@
 # Create a HDFS connector client
 client = InsecureClient('http://hive:50070', user='root')
 
 # List HDFS file and directories
 print(client.list('/'))
 ```
 
-
 ```python
 import gravitino
 
 gravitino_admin_client = GravitinoAdminClient(uri="http://localhost:8090")
 metalake = gravitino_admin_client.create_metalake(
     ident=NameIdentifier.of("default"),
     comment="metalake comment", properties={})
@@ -94,25 +93,25 @@
 
 # Development Environment
 
 1. Install dependency
     ```bash
     pip install -e '.[dev]'
     ```
-   
+
 2. Run integration tests
     ```bash
     cd gravitino
     ./gradlew compileDistribution -x test
     ./gradlew :clients:client-python:test
     ```
 
 ## Resources
 + Official website https://datastrato.ai/
-+ Project home on Github: https://github.com/datastrato/gravitino/ 
++ Project home on GitHub: https://github.com/datastrato/gravitino/ 
 + Playground with Docker: https://github.com/datastrato/gravitino-playground
 + User documentation: https://datastrato.ai/docs/
 + Videos on Youtube: https://www.youtube.com/@Datastrato
 + Twitter: https://twitter.com/datastrato
 + Linkedin: https://www.linkedin.com/company/datastrato
 + Slack Community: [https://join.slack.com/t/datastrato-community](https://join.slack.com/t/datastrato-community/shared_invite/zt-2a8vsjoch-cU_uUwHA_QU6Ab50thoq8w)
 + Discourse Community: https://gravitino.discourse.group/
```

### Comparing `gravitino-0.5.0.dev2/setup.py` & `gravitino-0.5.0.dev3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,21 +5,19 @@
 
 from setuptools import find_packages, setup
 
 
 setup(
     name="gravitino",
     description="Python lib/client for Gravitino",
-    version="0.5.0.dev2",
+    version="0.5.0.dev3",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/datastrato/gravitino",
     author="datastrato",
     python_requires=">=3.8",
-    packages=find_packages(include=["gravitino", ".*"]),
-    include_package_data=True,
-    package_data={"": ["assets/*"]},
+    packages=find_packages(),
     install_requires=open("requirements.txt").read(),
     extras_require={
         "dev": open("requirements-dev.txt").read(),
     },
 )
```

### Comparing `gravitino-0.5.0.dev2/tests/test_gravitino_client.py` & `gravitino-0.5.0.dev3/tests/test_gravitino_client.py`

 * *Files identical despite different names*

