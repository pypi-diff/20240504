# Comparing `tmp/gravitino-0.5.0.dev3.tar.gz` & `tmp/gravitino-0.5.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitino-0.5.0.dev3.tar", last modified: Sat May  4 02:17:36 2024, max compression
+gzip compressed data, was "gravitino-0.5.0.dev4.tar", last modified: Sat May  4 02:28:39 2024, max compression
```

## Comparing `gravitino-0.5.0.dev3.tar` & `gravitino-0.5.0.dev4.tar`

### file list

```diff
@@ -1,96 +1,103 @@
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:17:36.932213 gravitino-0.5.0.dev3/
--rw-r--r--   0 xun        (501) staff       (20)     3710 2024-05-04 02:17:36.932071 gravitino-0.5.0.dev3/PKG-INFO
--rw-r--r--   0 xun        (501) staff       (20)     3420 2024-05-04 02:12:18.000000 gravitino-0.5.0.dev3/README.md
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:17:36.909958 gravitino-0.5.0.dev3/gravitino/
--rw-r--r--   0 xun        (501) staff       (20)      244 2024-04-08 10:35:22.000000 gravitino-0.5.0.dev3/gravitino/__init__.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:17:36.915127 gravitino-0.5.0.dev3/gravitino/api/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev3/gravitino/api/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)      942 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev3/gravitino/api/audit.py
--rw-r--r--   0 xun        (501) staff       (20)      440 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev3/gravitino/api/auditable.py
--rw-r--r--   0 xun        (501) staff       (20)     4113 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev3/gravitino/api/catalog.py
--rw-r--r--   0 xun        (501) staff       (20)     8759 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/api/catalog_change.py
--rw-r--r--   0 xun        (501) staff       (20)     3556 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/api/fileset.py
--rw-r--r--   0 xun        (501) staff       (20)     9226 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/api/fileset_change.py
--rw-r--r--   0 xun        (501) staff       (20)     1155 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/api/metalake.py
--rw-r--r--   0 xun        (501) staff       (20)     3403 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/api/metalake_change.py
--rw-r--r--   0 xun        (501) staff       (20)     1044 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/api/schema.py
--rw-r--r--   0 xun        (501) staff       (20)     4847 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/api/schema_change.py
--rw-r--r--   0 xun        (501) staff       (20)     3870 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/api/supports_schemas.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:17:36.916385 gravitino-0.5.0.dev3/gravitino/client/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev3/gravitino/client/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     4651 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/client/gravitino_admin_client.py
--rw-r--r--   0 xun        (501) staff       (20)     2739 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/client/gravitino_client.py
--rw-r--r--   0 xun        (501) staff       (20)     2483 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/client/gravitino_client_base.py
--rw-r--r--   0 xun        (501) staff       (20)     7664 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/client/gravitino_metalake.py
--rw-r--r--   0 xun        (501) staff       (20)      408 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev3/gravitino/client/gravitino_version.py
--rw-r--r--   0 xun        (501) staff       (20)      119 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev3/gravitino/constants.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:17:36.918388 gravitino-0.5.0.dev3/gravitino/dto/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev3/gravitino/dto/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     1753 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev3/gravitino/dto/audit_dto.py
--rw-r--r--   0 xun        (501) staff       (20)     1590 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev3/gravitino/dto/catalog_dto.py
--rw-r--r--   0 xun        (501) staff       (20)     3019 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/dto_converters.py
--rw-r--r--   0 xun        (501) staff       (20)     1313 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/fileset_dto.py
--rw-r--r--   0 xun        (501) staff       (20)     1883 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/metalake_dto.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:17:36.921150 gravitino-0.5.0.dev3/gravitino/dto/requests/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev3/gravitino/dto/requests/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     1560 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/requests/catalog_create_request.py
--rw-r--r--   0 xun        (501) staff       (20)     2534 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/requests/catalog_update_request.py
--rw-r--r--   0 xun        (501) staff       (20)     1065 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/requests/catalog_updates_request.py
--rw-r--r--   0 xun        (501) staff       (20)     1438 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/requests/fileset_create_request.py
--rw-r--r--   0 xun        (501) staff       (20)     4267 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/requests/fileset_update_request.py
--rw-r--r--   0 xun        (501) staff       (20)      750 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/requests/fileset_updates_request.py
--rw-r--r--   0 xun        (501) staff       (20)     1070 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/requests/metalake_create_request.py
--rw-r--r--   0 xun        (501) staff       (20)     4145 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/requests/metalake_update_request.py
--rw-r--r--   0 xun        (501) staff       (20)     1029 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/requests/metalake_updates_request.py
--rw-r--r--   0 xun        (501) staff       (20)      908 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/requests/schema_create_request.py
--rw-r--r--   0 xun        (501) staff       (20)     2519 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/requests/schema_update_request.py
--rw-r--r--   0 xun        (501) staff       (20)      990 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/requests/schema_updates_request.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:17:36.925235 gravitino-0.5.0.dev3/gravitino/dto/responses/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev3/gravitino/dto/responses/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)      683 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/responses/base_response.py
--rw-r--r--   0 xun        (501) staff       (20)      573 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/responses/catalog_list_response.py
--rw-r--r--   0 xun        (501) staff       (20)     1051 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev3/gravitino/dto/responses/catalog_response.py
--rw-r--r--   0 xun        (501) staff       (20)      476 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev3/gravitino/dto/responses/drop_response.py
--rw-r--r--   0 xun        (501) staff       (20)      871 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/responses/entity_list_response.py
--rw-r--r--   0 xun        (501) staff       (20)     1061 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/responses/fileset_response.py
--rw-r--r--   0 xun        (501) staff       (20)     1162 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/responses/metalake_list_response.py
--rw-r--r--   0 xun        (501) staff       (20)     1063 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/responses/metalake_response.py
--rw-r--r--   0 xun        (501) staff       (20)     1058 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/responses/schema_response.py
--rw-r--r--   0 xun        (501) staff       (20)     1382 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/dto/schema_dto.py
--rw-r--r--   0 xun        (501) staff       (20)      431 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev3/gravitino/dto/version_dto.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:17:36.927237 gravitino-0.5.0.dev3/gravitino/exceptions/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev3/gravitino/exceptions/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)      302 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/exceptions/gravitino_runtime_exception.py
--rw-r--r--   0 xun        (501) staff       (20)      363 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/exceptions/illegal_name_identifier_exception.py
--rw-r--r--   0 xun        (501) staff       (20)      352 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/exceptions/illegal_namespace_exception.py
--rw-r--r--   0 xun        (501) staff       (20)      288 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/exceptions/no_such_metalake_exception.py
--rw-r--r--   0 xun        (501) staff       (20)      323 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/exceptions/not_found_exception.py
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev3/gravitino/exceptions.py
--rw-r--r--   0 xun        (501) staff       (20)     4404 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev3/gravitino/gravitino_client.py
--rw-r--r--   0 xun        (501) staff       (20)     9268 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/name_identifier.py
--rw-r--r--   0 xun        (501) staff       (20)     7603 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/namespace.py
--rw-r--r--   0 xun        (501) staff       (20)     2430 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev3/gravitino/service.py
--rw-r--r--   0 xun        (501) staff       (20)      318 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev3/gravitino/typing.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:17:36.928666 gravitino-0.5.0.dev3/gravitino/utils/
--rw-r--r--   0 xun        (501) staff       (20)      175 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev3/gravitino/utils/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     2692 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/utils/exceptions.py
--rw-r--r--   0 xun        (501) staff       (20)     5479 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/gravitino/utils/http_client.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:17:36.911862 gravitino-0.5.0.dev3/gravitino.egg-info/
--rw-r--r--   0 xun        (501) staff       (20)     3710 2024-05-04 02:17:36.000000 gravitino-0.5.0.dev3/gravitino.egg-info/PKG-INFO
--rw-r--r--   0 xun        (501) staff       (20)     2881 2024-05-04 02:17:36.000000 gravitino-0.5.0.dev3/gravitino.egg-info/SOURCES.txt
--rw-r--r--   0 xun        (501) staff       (20)        1 2024-05-04 02:17:36.000000 gravitino-0.5.0.dev3/gravitino.egg-info/dependency_links.txt
--rw-r--r--   0 xun        (501) staff       (20)       69 2024-05-04 02:17:36.000000 gravitino-0.5.0.dev3/gravitino.egg-info/requires.txt
--rw-r--r--   0 xun        (501) staff       (20)       16 2024-05-04 02:17:36.000000 gravitino-0.5.0.dev3/gravitino.egg-info/top_level.txt
--rw-r--r--   0 xun        (501) staff       (20)       38 2024-05-04 02:17:36.932279 gravitino-0.5.0.dev3/setup.cfg
--rw-r--r--   0 xun        (501) staff       (20)      627 2024-05-04 02:16:59.000000 gravitino-0.5.0.dev3/setup.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:17:36.929889 gravitino-0.5.0.dev3/tests/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev3/tests/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     3607 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev3/tests/fixtures.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:17:36.931703 gravitino-0.5.0.dev3/tests/integration/
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev3/tests/integration/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)     3768 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/tests/integration/integration_test_env.py
--rw-r--r--   0 xun        (501) staff       (20)     7086 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/tests/integration/test_fileset_catalog.py
--rw-r--r--   0 xun        (501) staff       (20)     6653 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/tests/integration/test_metalake.py
--rw-r--r--   0 xun        (501) staff       (20)     6058 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev3/tests/integration/test_schema.py
--rw-r--r--   0 xun        (501) staff       (20)     2175 2024-04-13 14:55:38.000000 gravitino-0.5.0.dev3/tests/test_gravitino_client.py
--rw-r--r--   0 xun        (501) staff       (20)     1323 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev3/tests/utils.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:28:39.659835 gravitino-0.5.0.dev4/
+-rw-r--r--   0 xun        (501) staff       (20)     3774 2024-05-04 02:28:39.659682 gravitino-0.5.0.dev4/PKG-INFO
+-rw-r--r--   0 xun        (501) staff       (20)     3484 2024-05-04 02:27:17.000000 gravitino-0.5.0.dev4/README.md
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:28:39.640125 gravitino-0.5.0.dev4/gravitino/
+-rw-r--r--   0 xun        (501) staff       (20)      244 2024-04-08 10:35:22.000000 gravitino-0.5.0.dev4/gravitino/__init__.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:28:39.645737 gravitino-0.5.0.dev4/gravitino/api/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev4/gravitino/api/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)      942 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev4/gravitino/api/audit.py
+-rw-r--r--   0 xun        (501) staff       (20)      440 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev4/gravitino/api/auditable.py
+-rw-r--r--   0 xun        (501) staff       (20)     4113 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev4/gravitino/api/catalog.py
+-rw-r--r--   0 xun        (501) staff       (20)     8759 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/api/catalog_change.py
+-rw-r--r--   0 xun        (501) staff       (20)     3556 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/api/fileset.py
+-rw-r--r--   0 xun        (501) staff       (20)     9226 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/api/fileset_change.py
+-rw-r--r--   0 xun        (501) staff       (20)     1155 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/api/metalake.py
+-rw-r--r--   0 xun        (501) staff       (20)     3403 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/api/metalake_change.py
+-rw-r--r--   0 xun        (501) staff       (20)     1044 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/api/schema.py
+-rw-r--r--   0 xun        (501) staff       (20)     4847 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/api/schema_change.py
+-rw-r--r--   0 xun        (501) staff       (20)     3870 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/api/supports_schemas.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:28:39.646523 gravitino-0.5.0.dev4/gravitino/catalog/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev4/gravitino/catalog/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     7079 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/catalog/base_schema_catalog.py
+-rw-r--r--   0 xun        (501) staff       (20)     7344 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/catalog/fileset_catalog.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:28:39.648453 gravitino-0.5.0.dev4/gravitino/client/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev4/gravitino/client/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     4651 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/client/gravitino_admin_client.py
+-rw-r--r--   0 xun        (501) staff       (20)     2739 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/client/gravitino_client.py
+-rw-r--r--   0 xun        (501) staff       (20)     2483 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/client/gravitino_client_base.py
+-rw-r--r--   0 xun        (501) staff       (20)     7664 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/client/gravitino_metalake.py
+-rw-r--r--   0 xun        (501) staff       (20)      408 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev4/gravitino/client/gravitino_version.py
+-rw-r--r--   0 xun        (501) staff       (20)      119 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev4/gravitino/constants.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:28:39.650891 gravitino-0.5.0.dev4/gravitino/dto/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev4/gravitino/dto/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     1753 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev4/gravitino/dto/audit_dto.py
+-rw-r--r--   0 xun        (501) staff       (20)     1590 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev4/gravitino/dto/catalog_dto.py
+-rw-r--r--   0 xun        (501) staff       (20)     3019 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/dto/dto_converters.py
+-rw-r--r--   0 xun        (501) staff       (20)     1313 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/dto/fileset_dto.py
+-rw-r--r--   0 xun        (501) staff       (20)     1883 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/dto/metalake_dto.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:28:39.653202 gravitino-0.5.0.dev4/gravitino/dto/requests/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev4/gravitino/dto/requests/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     1560 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/dto/requests/catalog_create_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     2534 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/dto/requests/catalog_update_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     1065 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/dto/requests/catalog_updates_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     1438 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/dto/requests/fileset_create_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     4267 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/dto/requests/fileset_update_request.py
+-rw-r--r--   0 xun        (501) staff       (20)      750 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/dto/requests/fileset_updates_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     1070 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/dto/requests/metalake_create_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     4145 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/dto/requests/metalake_update_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     1029 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/dto/requests/metalake_updates_request.py
+-rw-r--r--   0 xun        (501) staff       (20)      908 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/dto/requests/schema_create_request.py
+-rw-r--r--   0 xun        (501) staff       (20)     2519 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/dto/requests/schema_update_request.py
+-rw-r--r--   0 xun        (501) staff       (20)      990 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/dto/requests/schema_updates_request.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:28:39.655037 gravitino-0.5.0.dev4/gravitino/dto/responses/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev4/gravitino/dto/responses/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)      683 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/dto/responses/base_response.py
+-rw-r--r--   0 xun        (501) staff       (20)      573 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/dto/responses/catalog_list_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1051 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev4/gravitino/dto/responses/catalog_response.py
+-rw-r--r--   0 xun        (501) staff       (20)      476 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev4/gravitino/dto/responses/drop_response.py
+-rw-r--r--   0 xun        (501) staff       (20)      871 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/dto/responses/entity_list_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1061 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/dto/responses/fileset_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1162 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/dto/responses/metalake_list_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1063 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/dto/responses/metalake_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1058 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/dto/responses/schema_response.py
+-rw-r--r--   0 xun        (501) staff       (20)     1382 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/dto/schema_dto.py
+-rw-r--r--   0 xun        (501) staff       (20)      431 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev4/gravitino/dto/version_dto.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:28:39.656022 gravitino-0.5.0.dev4/gravitino/exceptions/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-11 14:36:22.000000 gravitino-0.5.0.dev4/gravitino/exceptions/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)      302 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/exceptions/gravitino_runtime_exception.py
+-rw-r--r--   0 xun        (501) staff       (20)      363 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/exceptions/illegal_name_identifier_exception.py
+-rw-r--r--   0 xun        (501) staff       (20)      352 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/exceptions/illegal_namespace_exception.py
+-rw-r--r--   0 xun        (501) staff       (20)      288 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/exceptions/no_such_metalake_exception.py
+-rw-r--r--   0 xun        (501) staff       (20)      323 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/exceptions/not_found_exception.py
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev4/gravitino/exceptions.py
+-rw-r--r--   0 xun        (501) staff       (20)     4404 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev4/gravitino/gravitino_client.py
+-rw-r--r--   0 xun        (501) staff       (20)     9268 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/name_identifier.py
+-rw-r--r--   0 xun        (501) staff       (20)     7603 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/namespace.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:28:39.656429 gravitino-0.5.0.dev4/gravitino/rest/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev4/gravitino/rest/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     1198 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev4/gravitino/rest/rest_message.py
+-rw-r--r--   0 xun        (501) staff       (20)     2430 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev4/gravitino/service.py
+-rw-r--r--   0 xun        (501) staff       (20)      318 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev4/gravitino/typing.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:28:39.657085 gravitino-0.5.0.dev4/gravitino/utils/
+-rw-r--r--   0 xun        (501) staff       (20)      175 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev4/gravitino/utils/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     2692 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/utils/exceptions.py
+-rw-r--r--   0 xun        (501) staff       (20)     5479 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/gravitino/utils/http_client.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:28:39.642202 gravitino-0.5.0.dev4/gravitino.egg-info/
+-rw-r--r--   0 xun        (501) staff       (20)     3774 2024-05-04 02:28:39.000000 gravitino-0.5.0.dev4/gravitino.egg-info/PKG-INFO
+-rw-r--r--   0 xun        (501) staff       (20)     3047 2024-05-04 02:28:39.000000 gravitino-0.5.0.dev4/gravitino.egg-info/SOURCES.txt
+-rw-r--r--   0 xun        (501) staff       (20)        1 2024-05-04 02:28:39.000000 gravitino-0.5.0.dev4/gravitino.egg-info/dependency_links.txt
+-rw-r--r--   0 xun        (501) staff       (20)       72 2024-05-04 02:28:39.000000 gravitino-0.5.0.dev4/gravitino.egg-info/requires.txt
+-rw-r--r--   0 xun        (501) staff       (20)       16 2024-05-04 02:28:39.000000 gravitino-0.5.0.dev4/gravitino.egg-info/top_level.txt
+-rw-r--r--   0 xun        (501) staff       (20)       38 2024-05-04 02:28:39.659893 gravitino-0.5.0.dev4/setup.cfg
+-rw-r--r--   0 xun        (501) staff       (20)      627 2024-05-04 02:28:17.000000 gravitino-0.5.0.dev4/setup.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:28:39.658206 gravitino-0.5.0.dev4/tests/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev4/tests/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     3607 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev4/tests/fixtures.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 02:28:39.659398 gravitino-0.5.0.dev4/tests/integration/
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-13 14:46:55.000000 gravitino-0.5.0.dev4/tests/integration/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)     3768 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/tests/integration/integration_test_env.py
+-rw-r--r--   0 xun        (501) staff       (20)     7086 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/tests/integration/test_fileset_catalog.py
+-rw-r--r--   0 xun        (501) staff       (20)     6653 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/tests/integration/test_metalake.py
+-rw-r--r--   0 xun        (501) staff       (20)     6058 2024-05-04 02:09:56.000000 gravitino-0.5.0.dev4/tests/integration/test_schema.py
+-rw-r--r--   0 xun        (501) staff       (20)     2175 2024-04-13 14:55:38.000000 gravitino-0.5.0.dev4/tests/test_gravitino_client.py
+-rw-r--r--   0 xun        (501) staff       (20)     1323 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev4/tests/utils.py
```

### Comparing `gravitino-0.5.0.dev3/PKG-INFO` & `gravitino-0.5.0.dev4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gravitino
-Version: 0.5.0.dev3
+Version: 0.5.0.dev4
 Summary: Python lib/client for Gravitino
 Home-page: https://github.com/datastrato/gravitino
 Author: datastrato
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -48,14 +48,19 @@
 client = InsecureClient('http://hive:50070', user='root')
 
 # List HDFS file and directories
 print(client.list('/'))
 ```
 
 ```python
+pip install requests dataclasses-json gravitino
+```
+
+
+```python
 import gravitino
 
 gravitino_admin_client = GravitinoAdminClient(uri="http://localhost:8090")
 metalake = gravitino_admin_client.create_metalake(
     ident=NameIdentifier.of("default"),
     comment="metalake comment", properties={})
```

### Comparing `gravitino-0.5.0.dev3/README.md` & `gravitino-0.5.0.dev4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,19 @@
 client = InsecureClient('http://hive:50070', user='root')
 
 # List HDFS file and directories
 print(client.list('/'))
 ```
 
 ```python
+pip install requests dataclasses-json gravitino
+```
+
+
+```python
 import gravitino
 
 gravitino_admin_client = GravitinoAdminClient(uri="http://localhost:8090")
 metalake = gravitino_admin_client.create_metalake(
     ident=NameIdentifier.of("default"),
     comment="metalake comment", properties={})
```

### Comparing `gravitino-0.5.0.dev3/gravitino/api/audit.py` & `gravitino-0.5.0.dev4/gravitino/api/audit.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/api/catalog.py` & `gravitino-0.5.0.dev4/gravitino/api/catalog.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/api/catalog_change.py` & `gravitino-0.5.0.dev4/gravitino/api/catalog_change.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/api/fileset.py` & `gravitino-0.5.0.dev4/gravitino/api/fileset.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/api/fileset_change.py` & `gravitino-0.5.0.dev4/gravitino/api/fileset_change.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/api/metalake.py` & `gravitino-0.5.0.dev4/gravitino/api/metalake.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/api/metalake_change.py` & `gravitino-0.5.0.dev4/gravitino/api/metalake_change.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/api/schema.py` & `gravitino-0.5.0.dev4/gravitino/api/schema.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/api/schema_change.py` & `gravitino-0.5.0.dev4/gravitino/api/schema_change.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/api/supports_schemas.py` & `gravitino-0.5.0.dev4/gravitino/api/supports_schemas.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/client/gravitino_admin_client.py` & `gravitino-0.5.0.dev4/gravitino/client/gravitino_admin_client.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/client/gravitino_client.py` & `gravitino-0.5.0.dev4/gravitino/client/gravitino_client.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/client/gravitino_client_base.py` & `gravitino-0.5.0.dev4/gravitino/client/gravitino_client_base.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/client/gravitino_metalake.py` & `gravitino-0.5.0.dev4/gravitino/client/gravitino_metalake.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/dto/audit_dto.py` & `gravitino-0.5.0.dev4/gravitino/dto/audit_dto.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/dto/catalog_dto.py` & `gravitino-0.5.0.dev4/gravitino/dto/catalog_dto.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/dto/dto_converters.py` & `gravitino-0.5.0.dev4/gravitino/dto/dto_converters.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/dto/fileset_dto.py` & `gravitino-0.5.0.dev4/gravitino/dto/fileset_dto.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/dto/metalake_dto.py` & `gravitino-0.5.0.dev4/gravitino/dto/metalake_dto.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/dto/requests/catalog_create_request.py` & `gravitino-0.5.0.dev4/gravitino/dto/requests/catalog_create_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/dto/requests/catalog_update_request.py` & `gravitino-0.5.0.dev4/gravitino/dto/requests/catalog_update_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/dto/requests/catalog_updates_request.py` & `gravitino-0.5.0.dev4/gravitino/dto/requests/catalog_updates_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/dto/requests/fileset_create_request.py` & `gravitino-0.5.0.dev4/gravitino/dto/requests/fileset_create_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/dto/requests/fileset_update_request.py` & `gravitino-0.5.0.dev4/gravitino/dto/requests/fileset_update_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/dto/requests/fileset_updates_request.py` & `gravitino-0.5.0.dev4/gravitino/dto/requests/fileset_updates_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/dto/requests/metalake_create_request.py` & `gravitino-0.5.0.dev4/gravitino/dto/requests/metalake_create_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/dto/requests/metalake_update_request.py` & `gravitino-0.5.0.dev4/gravitino/dto/requests/metalake_update_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/dto/requests/metalake_updates_request.py` & `gravitino-0.5.0.dev4/gravitino/dto/requests/metalake_updates_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/dto/requests/schema_create_request.py` & `gravitino-0.5.0.dev4/gravitino/dto/requests/schema_create_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/dto/requests/schema_update_request.py` & `gravitino-0.5.0.dev4/gravitino/dto/requests/schema_update_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/dto/requests/schema_updates_request.py` & `gravitino-0.5.0.dev4/gravitino/dto/requests/schema_updates_request.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/dto/responses/base_response.py` & `gravitino-0.5.0.dev4/gravitino/dto/responses/base_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/dto/responses/catalog_list_response.py` & `gravitino-0.5.0.dev4/gravitino/dto/responses/catalog_list_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/dto/responses/catalog_response.py` & `gravitino-0.5.0.dev4/gravitino/dto/responses/catalog_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/dto/responses/entity_list_response.py` & `gravitino-0.5.0.dev4/gravitino/dto/responses/entity_list_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/dto/responses/fileset_response.py` & `gravitino-0.5.0.dev4/gravitino/dto/responses/fileset_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/dto/responses/metalake_list_response.py` & `gravitino-0.5.0.dev4/gravitino/dto/responses/metalake_list_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/dto/responses/metalake_response.py` & `gravitino-0.5.0.dev4/gravitino/dto/responses/metalake_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/dto/responses/schema_response.py` & `gravitino-0.5.0.dev4/gravitino/dto/responses/schema_response.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/dto/schema_dto.py` & `gravitino-0.5.0.dev4/gravitino/dto/schema_dto.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/gravitino_client.py` & `gravitino-0.5.0.dev4/gravitino/gravitino_client.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/name_identifier.py` & `gravitino-0.5.0.dev4/gravitino/name_identifier.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/namespace.py` & `gravitino-0.5.0.dev4/gravitino/namespace.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/service.py` & `gravitino-0.5.0.dev4/gravitino/service.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/utils/exceptions.py` & `gravitino-0.5.0.dev4/gravitino/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino/utils/http_client.py` & `gravitino-0.5.0.dev4/gravitino/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/gravitino.egg-info/PKG-INFO` & `gravitino-0.5.0.dev4/gravitino.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gravitino
-Version: 0.5.0.dev3
+Version: 0.5.0.dev4
 Summary: Python lib/client for Gravitino
 Home-page: https://github.com/datastrato/gravitino
 Author: datastrato
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -48,14 +48,19 @@
 client = InsecureClient('http://hive:50070', user='root')
 
 # List HDFS file and directories
 print(client.list('/'))
 ```
 
 ```python
+pip install requests dataclasses-json gravitino
+```
+
+
+```python
 import gravitino
 
 gravitino_admin_client = GravitinoAdminClient(uri="http://localhost:8090")
 metalake = gravitino_admin_client.create_metalake(
     ident=NameIdentifier.of("default"),
     comment="metalake comment", properties={})
```

### Comparing `gravitino-0.5.0.dev3/gravitino.egg-info/SOURCES.txt` & `gravitino-0.5.0.dev4/gravitino.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 gravitino/api/fileset.py
 gravitino/api/fileset_change.py
 gravitino/api/metalake.py
 gravitino/api/metalake_change.py
 gravitino/api/schema.py
 gravitino/api/schema_change.py
 gravitino/api/supports_schemas.py
+gravitino/catalog/__init__.py
+gravitino/catalog/base_schema_catalog.py
+gravitino/catalog/fileset_catalog.py
 gravitino/client/__init__.py
 gravitino/client/gravitino_admin_client.py
 gravitino/client/gravitino_client.py
 gravitino/client/gravitino_client_base.py
 gravitino/client/gravitino_metalake.py
 gravitino/client/gravitino_version.py
 gravitino/dto/__init__.py
@@ -64,14 +67,16 @@
 gravitino/dto/responses/schema_response.py
 gravitino/exceptions/__init__.py
 gravitino/exceptions/gravitino_runtime_exception.py
 gravitino/exceptions/illegal_name_identifier_exception.py
 gravitino/exceptions/illegal_namespace_exception.py
 gravitino/exceptions/no_such_metalake_exception.py
 gravitino/exceptions/not_found_exception.py
+gravitino/rest/__init__.py
+gravitino/rest/rest_message.py
 gravitino/utils/__init__.py
 gravitino/utils/exceptions.py
 gravitino/utils/http_client.py
 tests/__init__.py
 tests/fixtures.py
 tests/test_gravitino_client.py
 tests/utils.py
```

### Comparing `gravitino-0.5.0.dev3/setup.py` & `gravitino-0.5.0.dev4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from setuptools import find_packages, setup
 
 
 setup(
     name="gravitino",
     description="Python lib/client for Gravitino",
-    version="0.5.0.dev3",
+    version="0.5.0.dev4",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/datastrato/gravitino",
     author="datastrato",
     python_requires=">=3.8",
     packages=find_packages(),
     install_requires=open("requirements.txt").read(),
```

### Comparing `gravitino-0.5.0.dev3/tests/fixtures.py` & `gravitino-0.5.0.dev4/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/tests/integration/integration_test_env.py` & `gravitino-0.5.0.dev4/tests/integration/integration_test_env.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/tests/integration/test_fileset_catalog.py` & `gravitino-0.5.0.dev4/tests/integration/test_fileset_catalog.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/tests/integration/test_metalake.py` & `gravitino-0.5.0.dev4/tests/integration/test_metalake.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/tests/integration/test_schema.py` & `gravitino-0.5.0.dev4/tests/integration/test_schema.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/tests/test_gravitino_client.py` & `gravitino-0.5.0.dev4/tests/test_gravitino_client.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev3/tests/utils.py` & `gravitino-0.5.0.dev4/tests/utils.py`

 * *Files identical despite different names*

