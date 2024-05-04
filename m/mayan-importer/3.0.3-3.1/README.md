# Comparing `tmp/mayan-importer-3.0.3.tar.gz` & `tmp/mayan-importer-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mayan-importer-3.0.3.tar", last modified: Wed Apr  3 13:18:53 2024, max compression
+gzip compressed data, was "mayan-importer-3.1.tar", last modified: Fri May  3 08:55:35 2024, max compression
```

## Comparing `mayan-importer-3.0.3.tar` & `mayan-importer-3.1.tar`

### file list

```diff
@@ -1,74 +1,92 @@
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-03 13:18:53.983857 mayan-importer-3.0.3/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6341 2024-04-01 10:00:26.000000 mayan-importer-3.0.3/HISTORY.rst
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      555 2020-10-02 10:42:37.000000 mayan-importer-3.0.3/LICENSE
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       39 2020-10-02 10:42:37.000000 mayan-importer-3.0.3/MANIFEST.in
--rw-r--r--   0 rosarior  (1000) rosarior  (1000)     9233 2024-04-03 13:18:53.983857 mayan-importer-3.0.3/PKG-INFO
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1628 2020-10-02 10:42:37.000000 mayan-importer-3.0.3/README.rst
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-03 13:18:53.969857 mayan-importer-3.0.3/importer/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       49 2020-10-02 10:42:37.000000 mayan-importer-3.0.3/importer/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      405 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/admin.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4643 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/api_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7455 2024-04-03 06:48:45.000000 mayan-importer-3.0.3/importer/apps.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7145 2024-04-01 11:57:21.000000 mayan-importer-3.0.3/importer/classes.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      145 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/dependencies.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1729 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/events.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       93 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/exceptions.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      997 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/forms.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1366 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/icons.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8712 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/importers.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     5779 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/links.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      904 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/literals.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-03 13:18:53.976857 mayan-importer-3.0.3/importer/migrations/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4126 2020-10-02 10:42:37.000000 mayan-importer-3.0.3/importer/migrations/0001_initial.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1475 2020-10-02 10:42:37.000000 mayan-importer-3.0.3/importer/migrations/0002_auto_20200908_0458.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      669 2020-10-02 10:42:37.000000 mayan-importer-3.0.3/importer/migrations/0003_importsetup_metadata_map.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      795 2023-04-12 05:57:59.000000 mayan-importer-3.0.3/importer/migrations/0004_auto_20200908_0853.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      607 2023-04-12 05:57:59.000000 mayan-importer-3.0.3/importer/migrations/0005_importsetup_state.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      333 2023-04-12 05:57:59.000000 mayan-importer-3.0.3/importer/migrations/0006_auto_20200924_0802.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      428 2023-04-12 05:57:59.000000 mayan-importer-3.0.3/importer/migrations/0007_auto_20200924_0802.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      603 2023-04-12 05:57:59.000000 mayan-importer-3.0.3/importer/migrations/0008_auto_20200924_0903.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2451 2023-04-12 05:57:59.000000 mayan-importer-3.0.3/importer/migrations/0009_importsetupaction.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      289 2023-04-12 05:57:59.000000 mayan-importer-3.0.3/importer/migrations/0010_remove_importsetup_metadata_map.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      568 2023-04-12 05:57:59.000000 mayan-importer-3.0.3/importer/migrations/0011_auto_20201004_0042.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      522 2023-04-12 05:57:59.000000 mayan-importer-3.0.3/importer/migrations/0012_importsetupitem_documents.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1796 2023-04-12 05:57:59.000000 mayan-importer-3.0.3/importer/migrations/0013_auto_20201225_0155.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      396 2023-04-12 05:57:59.000000 mayan-importer-3.0.3/importer/migrations/0014_auto_20201227_0610.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      848 2023-04-12 05:57:59.000000 mayan-importer-3.0.3/importer/migrations/0015_auto_20220901_0932.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      526 2023-04-12 05:57:59.000000 mayan-importer-3.0.3/importer/migrations/0016_importsetup_item_time_buffer.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      239 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/migrations/0017_delete_importsetuplog.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1064 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/migrations/0018_auto_20240401_0808.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1326 2024-04-02 11:02:22.000000 mayan-importer-3.0.3/importer/migrations/0019_auto_20240402_1101.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2020-10-02 10:42:37.000000 mayan-importer-3.0.3/importer/migrations/__init__.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-03 13:18:53.977857 mayan-importer-3.0.3/importer/models/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      134 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/models/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4220 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/models/import_setup_item_model_mixins.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2882 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/models/import_setup_item_models.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     5737 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/models/import_setup_model_mixins.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2470 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/models/import_setup_models.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1386 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/permissions.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1197 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/queues.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3473 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/serializers.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2794 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/tasks.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-03 13:18:53.980857 mayan-importer-3.0.3/importer/tests/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/tests/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1559 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/tests/importers.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      408 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/tests/literals.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8729 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/tests/mixins.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8233 2023-04-12 05:57:59.000000 mayan-importer-3.0.3/importer/tests/test_import_setup_api.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7881 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/tests/test_import_setup_item_api.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    12253 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/tests/test_import_setup_item_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6425 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/tests/test_import_setup_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     5600 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/urls.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-03 13:18:53.981857 mayan-importer-3.0.3/importer/views/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2023-04-12 05:57:59.000000 mayan-importer-3.0.3/importer/views/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    16658 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/views/import_setup_item_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4343 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/views/import_setup_views.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-03 13:18:53.982857 mayan-importer-3.0.3/mayan_importer.egg-info/
--rw-r--r--   0 rosarior  (1000) rosarior  (1000)     9233 2024-04-03 13:18:53.000000 mayan-importer-3.0.3/mayan_importer.egg-info/PKG-INFO
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2195 2024-04-03 13:18:53.000000 mayan-importer-3.0.3/mayan_importer.egg-info/SOURCES.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2024-04-03 13:18:53.000000 mayan-importer-3.0.3/mayan_importer.egg-info/dependency_links.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2024-04-03 13:18:53.000000 mayan-importer-3.0.3/mayan_importer.egg-info/not-zip-safe
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       16 2024-04-03 13:18:53.000000 mayan-importer-3.0.3/mayan_importer.egg-info/requires.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        9 2024-04-03 13:18:53.000000 mayan-importer-3.0.3/mayan_importer.egg-info/top_level.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      129 2024-04-03 13:18:53.983857 mayan-importer-3.0.3/setup.cfg
--rwxrwxr-x   0 rosarior  (1000) rosarior  (1000)     3038 2024-04-03 13:18:25.000000 mayan-importer-3.0.3/setup.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-03 08:55:35.871172 mayan-importer-3.1/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6509 2024-05-03 08:54:55.000000 mayan-importer-3.1/HISTORY.rst
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      555 2020-10-02 10:42:37.000000 mayan-importer-3.1/LICENSE
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       39 2020-10-02 10:42:37.000000 mayan-importer-3.1/MANIFEST.in
+-rw-r--r--   0 rosarior  (1000) rosarior  (1000)     9399 2024-05-03 08:55:35.871172 mayan-importer-3.1/PKG-INFO
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1628 2020-10-02 10:42:37.000000 mayan-importer-3.1/README.rst
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-03 08:55:35.863172 mayan-importer-3.1/importer/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       49 2020-10-02 10:42:37.000000 mayan-importer-3.1/importer/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      405 2024-04-01 10:00:47.000000 mayan-importer-3.1/importer/admin.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4643 2024-04-01 10:00:47.000000 mayan-importer-3.1/importer/api_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7817 2024-05-03 08:03:48.000000 mayan-importer-3.1/importer/apps.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7182 2024-05-03 08:30:22.000000 mayan-importer-3.1/importer/classes.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      145 2024-04-01 10:00:47.000000 mayan-importer-3.1/importer/dependencies.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1729 2024-04-01 10:00:47.000000 mayan-importer-3.1/importer/events.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       93 2024-04-01 10:00:47.000000 mayan-importer-3.1/importer/exceptions.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-03 08:55:35.863172 mayan-importer-3.1/importer/forms/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-05-03 06:18:39.000000 mayan-importer-3.1/importer/forms/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      326 2024-05-03 06:38:56.000000 mayan-importer-3.1/importer/forms/filer_forms.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      431 2024-05-03 08:05:46.000000 mayan-importer-3.1/importer/forms/form_mixins.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      949 2024-05-03 06:38:56.000000 mayan-importer-3.1/importer/forms/import_setup_forms.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      591 2024-05-03 06:40:26.000000 mayan-importer-3.1/importer/forms/import_setup_item_forms.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-03 08:55:35.864172 mayan-importer-3.1/importer/icons/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-05-02 06:30:26.000000 mayan-importer-3.1/importer/icons/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      222 2024-05-03 06:38:56.000000 mayan-importer-3.1/importer/icons/import_setup_filer_icons.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      914 2024-05-03 06:38:56.000000 mayan-importer-3.1/importer/icons/import_setup_icons.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      710 2024-05-03 06:38:56.000000 mayan-importer-3.1/importer/icons/import_setup_item_icons.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8715 2024-05-03 08:31:33.000000 mayan-importer-3.1/importer/importers.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-03 08:55:35.864172 mayan-importer-3.1/importer/links/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-05-02 06:05:24.000000 mayan-importer-3.1/importer/links/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      974 2024-05-03 06:38:56.000000 mayan-importer-3.1/importer/links/import_setup_filer_links.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2534 2024-05-03 06:38:56.000000 mayan-importer-3.1/importer/links/import_setup_item_links.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3461 2024-05-03 06:37:19.000000 mayan-importer-3.1/importer/links/import_setup_links.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1205 2024-05-02 22:28:59.000000 mayan-importer-3.1/importer/literals.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-03 08:55:35.867172 mayan-importer-3.1/importer/migrations/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4126 2020-10-02 10:42:37.000000 mayan-importer-3.1/importer/migrations/0001_initial.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1475 2020-10-02 10:42:37.000000 mayan-importer-3.1/importer/migrations/0002_auto_20200908_0458.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      669 2020-10-02 10:42:37.000000 mayan-importer-3.1/importer/migrations/0003_importsetup_metadata_map.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      795 2023-04-12 05:57:59.000000 mayan-importer-3.1/importer/migrations/0004_auto_20200908_0853.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      607 2023-04-12 05:57:59.000000 mayan-importer-3.1/importer/migrations/0005_importsetup_state.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      333 2023-04-12 05:57:59.000000 mayan-importer-3.1/importer/migrations/0006_auto_20200924_0802.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      428 2023-04-12 05:57:59.000000 mayan-importer-3.1/importer/migrations/0007_auto_20200924_0802.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      603 2023-04-12 05:57:59.000000 mayan-importer-3.1/importer/migrations/0008_auto_20200924_0903.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2451 2023-04-12 05:57:59.000000 mayan-importer-3.1/importer/migrations/0009_importsetupaction.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      287 2024-05-02 22:00:10.000000 mayan-importer-3.1/importer/migrations/0010_remove_importsetup_metadata_map.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      568 2023-04-12 05:57:59.000000 mayan-importer-3.1/importer/migrations/0011_auto_20201004_0042.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      522 2023-04-12 05:57:59.000000 mayan-importer-3.1/importer/migrations/0012_importsetupitem_documents.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1796 2023-04-12 05:57:59.000000 mayan-importer-3.1/importer/migrations/0013_auto_20201225_0155.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      396 2023-04-12 05:57:59.000000 mayan-importer-3.1/importer/migrations/0014_auto_20201227_0610.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      848 2023-04-12 05:57:59.000000 mayan-importer-3.1/importer/migrations/0015_auto_20220901_0932.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      526 2023-04-12 05:57:59.000000 mayan-importer-3.1/importer/migrations/0016_importsetup_item_time_buffer.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      239 2024-04-01 10:00:47.000000 mayan-importer-3.1/importer/migrations/0017_delete_importsetuplog.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1064 2024-04-01 10:00:47.000000 mayan-importer-3.1/importer/migrations/0018_auto_20240401_0808.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1326 2024-04-02 11:02:22.000000 mayan-importer-3.1/importer/migrations/0019_auto_20240402_1101.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1449 2024-05-02 19:09:03.000000 mayan-importer-3.1/importer/migrations/0020_auto_20240502_1907.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1596 2024-05-03 06:35:16.000000 mayan-importer-3.1/importer/migrations/0021_migrate_state_codes.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1063 2024-05-03 08:53:58.000000 mayan-importer-3.1/importer/migrations/0022_auto_20240503_0853.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2020-10-02 10:42:37.000000 mayan-importer-3.1/importer/migrations/__init__.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-03 08:55:35.868172 mayan-importer-3.1/importer/models/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      134 2024-04-01 10:00:47.000000 mayan-importer-3.1/importer/models/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4172 2024-05-03 08:45:32.000000 mayan-importer-3.1/importer/models/import_setup_item_model_mixins.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2945 2024-05-03 07:37:19.000000 mayan-importer-3.1/importer/models/import_setup_item_models.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6122 2024-05-03 08:39:32.000000 mayan-importer-3.1/importer/models/import_setup_model_mixins.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2421 2024-05-03 08:48:29.000000 mayan-importer-3.1/importer/models/import_setup_models.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3132 2024-05-03 08:49:55.000000 mayan-importer-3.1/importer/models/model_mixins.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1386 2024-04-01 10:00:47.000000 mayan-importer-3.1/importer/permissions.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1197 2024-04-01 10:00:47.000000 mayan-importer-3.1/importer/queues.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3473 2024-04-01 10:00:47.000000 mayan-importer-3.1/importer/serializers.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2314 2024-05-03 08:30:22.000000 mayan-importer-3.1/importer/tasks.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-03 08:55:35.869171 mayan-importer-3.1/importer/tests/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 10:00:47.000000 mayan-importer-3.1/importer/tests/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1650 2024-05-03 08:30:22.000000 mayan-importer-3.1/importer/tests/importers.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      408 2024-04-01 10:00:47.000000 mayan-importer-3.1/importer/tests/literals.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8743 2024-05-03 08:05:05.000000 mayan-importer-3.1/importer/tests/mixins.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8233 2024-05-03 08:09:51.000000 mayan-importer-3.1/importer/tests/test_import_setup_api.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7881 2024-04-01 10:00:47.000000 mayan-importer-3.1/importer/tests/test_import_setup_item_api.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    11635 2024-05-03 08:50:46.000000 mayan-importer-3.1/importer/tests/test_import_setup_item_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6425 2024-04-01 10:00:47.000000 mayan-importer-3.1/importer/tests/test_import_setup_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     5779 2024-05-02 06:54:59.000000 mayan-importer-3.1/importer/urls.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-03 08:55:35.870171 mayan-importer-3.1/importer/views/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2023-04-12 05:57:59.000000 mayan-importer-3.1/importer/views/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3693 2024-05-03 06:34:50.000000 mayan-importer-3.1/importer/views/import_setup_filer_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8134 2024-05-03 08:02:03.000000 mayan-importer-3.1/importer/views/import_setup_item_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     9643 2024-05-03 08:07:00.000000 mayan-importer-3.1/importer/views/import_setup_views.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-03 08:55:35.871172 mayan-importer-3.1/mayan_importer.egg-info/
+-rw-r--r--   0 rosarior  (1000) rosarior  (1000)     9399 2024-05-03 08:55:35.000000 mayan-importer-3.1/mayan_importer.egg-info/PKG-INFO
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2822 2024-05-03 08:55:35.000000 mayan-importer-3.1/mayan_importer.egg-info/SOURCES.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2024-05-03 08:55:35.000000 mayan-importer-3.1/mayan_importer.egg-info/dependency_links.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2024-05-03 08:55:35.000000 mayan-importer-3.1/mayan_importer.egg-info/not-zip-safe
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       16 2024-05-03 08:55:35.000000 mayan-importer-3.1/mayan_importer.egg-info/requires.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        9 2024-05-03 08:55:35.000000 mayan-importer-3.1/mayan_importer.egg-info/top_level.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      129 2024-05-03 08:55:35.871172 mayan-importer-3.1/setup.cfg
+-rwxrwxr-x   0 rosarior  (1000) rosarior  (1000)     3036 2024-05-03 08:54:32.000000 mayan-importer-3.1/setup.py
```

### Comparing `mayan-importer-3.0.3/HISTORY.rst` & `mayan-importer-3.1/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+3.1 (2024-05-03)
+================
+- Improve navigation.
+- Improve processing condition logic.
+- Split modules.
+- Move common state code into a mixin.
+- Add fieldsets.
+
 3.0 (2024-04-01)
 ================
 - Refactor app.
 - Remove import setup action.
 - Use source metadata to store import metadata.
 - Don't deserialize import item source column.
 - Use upstream backend, dynamic forms, credentials mixins, model mixins,
```

### Comparing `mayan-importer-3.0.3/LICENSE` & `mayan-importer-3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.3/PKG-INFO` & `mayan-importer-3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mayan-importer
-Version: 3.0.3
+Version: 3.1
 Summary: Mayan EDMS importer
 Home-page: https://gitlab.com/mayan-edms/importer
 Author: Roberto Rosario
 Author-email: roberto.rosario@mayan-edms.com
 License: Apache 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -93,14 +93,22 @@
 - Generate an Access Token with no expiration.
 - Create a credential instance in the Mayan EDMS Importer app and enter the Access Token.
 - Create an Import Setup that will filter the files to fetch from Dropbox.
 - Click the "Populate" button and check that the item count is correct.
 - Click the "Process" button to start the import process.
 
 
+3.1 (2024-05-03)
+================
+- Improve navigation.
+- Improve processing condition logic.
+- Split modules.
+- Move common state code into a mixin.
+- Add fieldsets.
+
 3.0 (2024-04-01)
 ================
 - Refactor app.
 - Remove import setup action.
 - Use source metadata to store import metadata.
 - Don't deserialize import item source column.
 - Use upstream backend, dynamic forms, credentials mixins, model mixins,
```

### Comparing `mayan-importer-3.0.3/README.rst` & `mayan-importer-3.1/README.rst`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.3/importer/api_views.py` & `mayan-importer-3.1/importer/api_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.3/importer/apps.py` & `mayan-importer-3.1/importer/apps.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,34 +8,40 @@
     menu_list_facet, menu_multi_item, menu_object, menu_related, menu_return,
     menu_secondary, menu_setup
 )
 from mayan.apps.credentials.links import link_credential_list
 from mayan.apps.events.classes import EventModelRegistry, ModelEventType
 from mayan.apps.logging.classes import ErrorLog
 from mayan.apps.navigation.classes import SourceColumn
+from mayan.apps.views.column_widgets import TwoStateWidget
 
 from .classes import ImportSetupBackend, ModelFiler
 from .events import (
     event_import_setup_edited, event_import_setup_item_finished,
     event_import_setup_item_deleted, event_import_setup_item_edited,
     event_import_setup_process_finished, event_import_setup_process_started,
     event_import_setup_populate_finished, event_import_setup_populate_started
 )
-from .links import (
-    link_import_setup_backend_selection, link_import_setup_delete,
-    link_import_setup_clear, link_import_setup_edit,
-    link_import_setup_item_delete, link_import_setup_item_edit,
-    link_import_setup_item_multiple_delete,
-    link_import_setup_item_document_list,
-    link_import_setup_item_multiple_process, link_import_setup_item_list,
-    link_import_setup_item_process, link_import_setup_multiple_clear,
-    link_import_setup_multiple_populate, link_import_setup_multiple_process,
-    link_import_setup_populate, link_import_setup_process,
-    link_import_setup_list, link_import_setup_setup, link_model_filer_load,
-    link_model_filer_save
+from .links.import_setup_filer_links import (
+    link_model_filer_load, link_model_filer_save
+)
+from .links.import_setup_item_links import (
+    link_import_setup_item_delete_multiple,
+    link_import_setup_item_delete_single,
+    link_import_setup_item_document_list, link_import_setup_item_edit,
+    link_import_setup_item_list, link_import_setup_item_process_multiple,
+    link_import_setup_item_process_single
+)
+from .links.import_setup_links import (
+    link_import_setup_backend_selection, link_import_setup_clear_multiple,
+    link_import_setup_clear_single, link_import_setup_delete,
+    link_import_setup_edit, link_import_setup_list,
+    link_import_setup_populate_multiple, link_import_setup_populate_single,
+    link_import_setup_process_multiple, link_import_setup_process_single,
+    link_import_setups
 )
 from .permissions import (
     permission_import_setup_delete, permission_import_setup_edit,
     permission_import_setup_process, permission_import_setup_view,
     permission_model_filer_load, permission_model_filer_save
 )
 
@@ -82,17 +88,16 @@
         )
 
         ModelFiler(model=ImportSetupItem)
 
         ModelPermission.register(
             model=ImportSetup, permissions=(
                 permission_import_setup_delete, permission_import_setup_edit,
-                permission_import_setup_process,
-                permission_import_setup_view, permission_model_filer_load,
-                permission_model_filer_save
+                permission_import_setup_process, permission_import_setup_view,
+                permission_model_filer_load, permission_model_filer_save
             )
         )
 
         ModelPermission.register_inheritance(
             model=ImportSetupItem, related='import_setup',
         )
 
@@ -103,21 +108,25 @@
             source=ImportSetup
         )
         SourceColumn(
             attribute='get_backend_class_label', include_label=True,
             source=ImportSetup
         )
         SourceColumn(
-            attribute='item_count_percent', empty_value=_(message='0%'),
+            attribute='get_item_processed_percent', empty_value=_(message='0%'),
             include_label=True, source=ImportSetup
         )
         SourceColumn(
             attribute='get_state_label', include_label=True,
             is_sortable=True, sort_field='state', source=ImportSetup
         )
+        SourceColumn(
+            attribute='get_process_allowed', include_label=True,
+            source=ImportSetup, widget=TwoStateWidget
+        )
 
         # Import setup item
 
         SourceColumn(
             attribute='identifier', is_identifier=True, is_sortable=True,
             source=ImportSetupItem
         )
@@ -134,83 +143,82 @@
 
         menu_list_facet.bind_links(
             links=(link_import_setup_item_list,), sources=(ImportSetup,)
         )
 
         menu_multi_item.bind_links(
             links=(
-                link_import_setup_multiple_clear,
-                link_import_setup_multiple_populate,
-                link_import_setup_multiple_process
+                link_import_setup_clear_multiple,
+                link_import_setup_populate_multiple,
+                link_import_setup_process_multiple
             ), sources=(ImportSetup,)
         )
 
         menu_object.bind_links(
             links=(
                 link_import_setup_delete, link_import_setup_edit,
-                link_import_setup_process
+                link_import_setup_process_single
             ), sources=(ImportSetup,)
         )
 
         menu_related.bind_links(
             links=(link_credential_list,),
             sources=(
                 ImportSetup, ImportSetupItem,
                 'importer:import_setup_backend_selection',
-                'importer:import_setup_create',
-                'importer:import_setup_list'
+                'importer:import_setup_create', 'importer:import_setup_list'
             )
         )
 
         menu_return.bind_links(
             links=(link_import_setup_list,), sources=(
                 ImportSetup, ImportSetupItem,
                 'importer:import_setup_backend_selection',
-                'importer:import_setup_create',
-                'importer:import_setup_list'
+                'importer:import_setup_create', 'importer:import_setup_list'
             )
         )
 
         menu_secondary.bind_links(
             links=(link_import_setup_backend_selection,),
             sources=(
                 ImportSetup, 'importer:import_setup_items_list',
                 'importer:import_setup_create', 'importer:import_setup_list'
             )
         )
 
         menu_secondary.bind_links(
             links=(
-                link_import_setup_clear, link_import_setup_populate,
-                link_model_filer_load, link_model_filer_save
+                link_import_setup_clear_single,
+                link_import_setup_populate_single, link_model_filer_load,
+                link_model_filer_save
             ),
             sources=(
                 'importer:import_setup_load',
                 'importer:import_setup_items_list',
-                'importer:import_setup_populate',
-                'importer:import_setup_save'
+                'importer:import_setup_populate', 'importer:import_setup_save'
             )
         )
 
         menu_setup.bind_links(
-            links=(link_import_setup_setup,)
+            links=(link_import_setups,)
         )
 
         # Import setup item
 
         menu_list_facet.bind_links(
             links=(
                 link_import_setup_item_document_list,
             ), sources=(ImportSetupItem,)
         )
         menu_multi_item.bind_links(
             links=(
-                link_import_setup_item_multiple_delete,
-                link_import_setup_item_multiple_process
+                link_import_setup_item_delete_multiple,
+                link_import_setup_item_process_multiple
             ), sources=(ImportSetupItem,)
         )
         menu_object.bind_links(
             links=(
-                link_import_setup_item_delete, link_import_setup_item_edit,
-                link_import_setup_item_process
+                link_import_setup_item_delete_single,
+                link_import_setup_item_edit,
+                link_import_setup_item_process_single
             ), sources=(ImportSetupItem,)
         )
```

### Comparing `mayan-importer-3.0.3/importer/classes.py` & `mayan-importer-3.1/importer/classes.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 from django.utils.translation import ugettext_lazy as _
 
 from mayan.apps.backends.class_mixins import DynamicFormBackendMixin
 from mayan.apps.backends.classes import ModelBaseBackend
 from mayan.apps.locales.utils import to_language
 from mayan.apps.storage.utils import NamedTemporaryFile
 
-from .permissions import permission_import_setup_view
-
 logger = logging.getLogger(name=__name__)
 
 __all__ = ('ImportSetupBackend',)
 MESSAGE_MODEL_FILER_SAVE_BODY = _(
     'The model data from object type %(save_file_title)s has been '
     'exported and is available for download using the '
     'link: %(download_url)s or from '
@@ -59,21 +57,24 @@
         fieldsets = (
             (
                 _('General'), {
                     'fields': ('label', 'document_type')
                 }
             ), (
                 _(message='Processing'), {
-                    'fields': ('item_time_buffer', 'process_size')
+                    'fields': ('item_time_buffer', 'process_size', 'state')
                 }
             ),
         )
 
         return fieldsets
 
+    def do_check_valid(self, identifier, data):
+        raise NotImplementedError
+
 
 class NullBackend(ImportSetupBackend):
     label = _(message='Null backend')
 
 
 class ModelFiler:
     _registry = {}
```

### Comparing `mayan-importer-3.0.3/importer/events.py` & `mayan-importer-3.1/importer/events.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.3/importer/forms.py` & `mayan-importer-3.1/importer/forms/import_setup_forms.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,31 @@
-from django import forms
+from django import forms as django_forms
 from django.utils.translation import ugettext_lazy as _
 
 from mayan.apps.backends.forms import FormDynamicModelBackend
+from mayan.apps.views import forms
 
-from .classes import ImportSetupBackend
-from .models import ImportSetup
+from ..classes import ImportSetupBackend
+from ..models import ImportSetup
+
+from .form_mixins import FormMixinState
 
 
 class ImportSetupBackendSelectionForm(forms.Form):
-    backend = forms.ChoiceField(
+    backend = django_forms.ChoiceField(
         choices=(), label=_(message='Backend'), help_text=_(
             message='The backend to use for the import setup.'
         )
     )
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.fields['backend'].choices = ImportSetupBackend.get_choices()
 
 
-class ImportSetupBackendDynamicForm(FormDynamicModelBackend):
+class ImportSetupBackendDynamicForm(FormMixinState, FormDynamicModelBackend):
     class Meta:
         fields = (
-            'label', 'document_type', 'process_size', 'item_time_buffer'
+            'label', 'document_type', 'process_size', 'item_time_buffer',
+            'state'
         )
         model = ImportSetup
-
-
-class ModelFilerUpload(forms.Form):
-    uploaded_file = forms.FileField(
-        help_text=_(message='CSV file that contain rows of model data'),
-        label=_(message='File')
-    )
```

### Comparing `mayan-importer-3.0.3/importer/icons.py` & `mayan-importer-3.1/importer/icons/import_setup_item_icons.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,22 @@
 from mayan.apps.appearance.classes import Icon
 from mayan.apps.documents.icons import icon_document
 
-icon_import_setup_backend_selection = icon_tag_create = Icon(
-    driver_name='fontawesome-dual', primary_symbol='cloud-upload-alt',
-    secondary_symbol='plus'
-)
-icon_import_setup_clear = Icon(
-    driver_name='fontawesome', symbol='eraser'
-)
-icon_import_setup_delete = Icon(driver_name='fontawesome', symbol='times')
-
-icon_import_setup_edit = Icon(driver_name='fontawesome', symbol='pencil-alt')
-icon_import_setup_process = Icon(
-    driver_name='fontawesome', symbol='play'
+icon_import_setup_item_delete_multiple = Icon(
+    driver_name='fontawesome', symbol='times'
 )
-
-# Import setup items
-
-icon_import_setup_item_delete = Icon(
+icon_import_setup_item_delete_single = Icon(
     driver_name='fontawesome', symbol='times'
 )
+icon_import_setup_item_document_list = icon_document
 icon_import_setup_item_edit = Icon(
     driver_name='fontawesome', symbol='pencil-alt'
 )
-icon_import_setup_item_document_list = icon_document
-icon_import_setup_item_process = Icon(
-    driver_name='fontawesome', symbol='play'
-)
 icon_import_setup_items_list = Icon(
     driver_name='fontawesome', symbol='file-upload'
 )
-icon_import_setup_list = Icon(
-    driver_name='fontawesome', symbol='cloud-upload-alt'
-)
-icon_import_setup_populate = Icon(
-    driver_name='fontawesome', symbol='file-signature'
-)
-
-# Model filer
-
-icon_model_filer_load = Icon(
-    driver_name='fontawesome', symbol='upload'
+icon_import_setup_item_process_multiple = Icon(
+    driver_name='fontawesome', symbol='play'
 )
-icon_model_filer_save = Icon(
-    driver_name='fontawesome', symbol='download'
+icon_import_setup_item_process_single = Icon(
+    driver_name='fontawesome', symbol='play'
 )
```

### Comparing `mayan-importer-3.0.3/importer/importers.py` & `mayan-importer-3.1/importer/importers.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             return self.team_admin_id
         else:
             client_kwargs = self.get_client_base_kwargs()
             client_team = dropbox.DropboxTeam(**client_kwargs)
             token_get_authenticated_admin_result = client_team.team_token_get_authenticated_admin()
             return token_get_authenticated_admin_result.admin_profile.team_member_id
 
-    def check_valid(self, identifier, data):
+    def do_check_valid(self, identifier, data):
         entry = self.get_entry(identifier=identifier, data=data)
 
         return self.match_filename_factory(entry=entry) and self.match_folder_factory(entry=entry)
 
     def get_client(self):
         """
         Return an instance of the Dropbox API client.
```

### Comparing `mayan-importer-3.0.3/importer/migrations/0001_initial.py` & `mayan-importer-3.1/importer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.3/importer/migrations/0002_auto_20200908_0458.py` & `mayan-importer-3.1/importer/migrations/0002_auto_20200908_0458.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.3/importer/migrations/0003_importsetup_metadata_map.py` & `mayan-importer-3.1/importer/migrations/0003_importsetup_metadata_map.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.3/importer/migrations/0004_auto_20200908_0853.py` & `mayan-importer-3.1/importer/migrations/0004_auto_20200908_0853.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.3/importer/migrations/0005_importsetup_state.py` & `mayan-importer-3.1/importer/migrations/0005_importsetup_state.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.3/importer/migrations/0008_auto_20200924_0903.py` & `mayan-importer-3.1/importer/migrations/0008_auto_20200924_0903.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.3/importer/migrations/0009_importsetupaction.py` & `mayan-importer-3.1/importer/migrations/0009_importsetupaction.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.3/importer/migrations/0011_auto_20201004_0042.py` & `mayan-importer-3.1/importer/migrations/0011_auto_20201004_0042.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.3/importer/migrations/0012_importsetupitem_documents.py` & `mayan-importer-3.1/importer/migrations/0012_importsetupitem_documents.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.3/importer/migrations/0013_auto_20201225_0155.py` & `mayan-importer-3.1/importer/migrations/0013_auto_20201225_0155.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.3/importer/migrations/0015_auto_20220901_0932.py` & `mayan-importer-3.1/importer/migrations/0015_auto_20220901_0932.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.3/importer/migrations/0016_importsetup_item_time_buffer.py` & `mayan-importer-3.1/importer/migrations/0016_importsetup_item_time_buffer.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.3/importer/migrations/0018_auto_20240401_0808.py` & `mayan-importer-3.1/importer/migrations/0018_auto_20240401_0808.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.3/importer/migrations/0019_auto_20240402_1101.py` & `mayan-importer-3.1/importer/migrations/0019_auto_20240402_1101.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.3/importer/models/import_setup_item_model_mixins.py` & `mayan-importer-3.1/importer/models/import_setup_item_model_mixins.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,84 +5,69 @@
 
 from mayan.apps.documents.tasks.document_tasks import task_document_upload
 from mayan.apps.events.decorators import method_event
 from mayan.apps.events.event_managers import EventManagerMethodAfter
 
 from ..events import event_import_setup_item_finished
 from ..literals import (
-    SETUP_ITEM_STATE_COMPLETE, SETUP_ITEM_STATE_ERROR, SETUP_ITEM_STATE_NONE,
-    SETUP_ITEM_STATE_PROCESSING
+    IMPORT_SETUP_ITEM_STATE_ERROR, IMPORT_SETUP_ITEM_STATE_NONE,
+    IMPORT_SETUP_ITEM_STATE_PROCESSED, IMPORT_SETUP_ITEM_STATE_PROCESSING,
+    IMPORT_SETUP_ITEM_STATE_QUEUED
 )
 
 
 class ImportSetupItemBusinessLogicMixin:
     @classmethod
     def get_process_allowed_state_list(self):
         return (
-            SETUP_ITEM_STATE_COMPLETE, SETUP_ITEM_STATE_ERROR,
-            SETUP_ITEM_STATE_NONE
-        )
-
-    def check_valid(self):
-        backend_instance = self.import_setup.get_backend_instance()
-        return backend_instance.check_valid(
-            identifier=self.identifier, data=self.data
+            IMPORT_SETUP_ITEM_STATE_PROCESSED, IMPORT_SETUP_ITEM_STATE_ERROR,
+            IMPORT_SETUP_ITEM_STATE_NONE
         )
 
     @property
     def data(self):
         return self.load_data()
 
-    def load_data(self):
-        return json.loads(s=self.serialized_data or '{}')
+    def do_check_valid(self):
+        backend_instance = self.import_setup.get_backend_instance()
+        return backend_instance.do_check_valid(
+            identifier=self.identifier, data=self.data
+        )
+
+    def do_data_dump(self, obj):
+        self.serialized_data = json.dumps(obj=obj)
 
     def get_data_display(self):
         return ', '.join(
             [
                 '"{}": "{}"'.format(key, value) for key, value in self.data.items()
             ]
         )
     get_data_display.short_description = _(message='Data')
 
-    def dump_data(self, obj):
-        self.serialized_data = json.dumps(obj=obj)
-
-    def get_process_allowed(self):
-        return self.state in self.get_process_allowed_state_list()
-
-    def get_state_label(self):
-        return self.get_state_display()
-    get_state_label.help_text = _(
-        message='The last recorded state of the item. The field will be '
-        'sorted by the numeric value of the state and not the actual text.'
-    )
-    get_state_label.short_description = _(message='State')
-
     @method_event(
         event_manager_class=EventManagerMethodAfter,
         event=event_import_setup_item_finished,
         action_object='import_setup',
         target='self'
     )
-    def process(self, force=False):
+    def do_process(self, force=False):
         shared_uploaded_file = None
 
         if force or self.get_process_allowed():
-            self.state = SETUP_ITEM_STATE_PROCESSING
-            self.save()
+            self.do_state_set(state=IMPORT_SETUP_ITEM_STATE_PROCESSING)
 
             backend_instance = self.import_setup.get_backend_instance()
 
             try:
                 shared_uploaded_file = backend_instance.item_process(
                     identifier=self.identifier, data=self.data
                 )
             except Exception as exception:
-                self.state = SETUP_ITEM_STATE_ERROR
-                self.save()
+                self.do_state_set(state=IMPORT_SETUP_ITEM_STATE_ERROR)
 
                 self.error_log.create(
                     text=str(exception)
                 )
 
                 if settings.DEBUG:
                     raise
@@ -115,12 +100,22 @@
                         'document_type_id': self.import_setup.document_type.pk,
                         'shared_uploaded_file_id': shared_uploaded_file.pk,
                         'callback_dict': callback_dict,
                         'label': label
                     }
                 )
 
-                self.state = SETUP_ITEM_STATE_COMPLETE
-                self.save()
+                self.do_state_set(state=IMPORT_SETUP_ITEM_STATE_PROCESSED)
 
                 queryset = self.error_log.all()
                 queryset.delete()
+
+    def get_process_allowed(self):
+        return self.state in self.get_process_allowed_state_list()
+
+    get_process_allowed.short_description = _(message='Can be processed?')
+
+    def load_data(self):
+        return json.loads(s=self.serialized_data or '{}')
+
+    def queue_task_import_setup_item_process_pre(self):
+        self.do_state_set(state=IMPORT_SETUP_ITEM_STATE_QUEUED)
```

### Comparing `mayan-importer-3.0.3/importer/models/import_setup_item_models.py` & `mayan-importer-3.1/importer/models/import_setup_models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,87 +1,70 @@
 from django.db import models
 from django.urls import reverse
 from django.utils.translation import ugettext_lazy as _
 
-from mayan.apps.documents.models.document_models import Document
+from mayan.apps.backends.model_mixins import BackendModelMixin
+from mayan.apps.documents.models.document_type_models import DocumentType
 from mayan.apps.events.decorators import method_event
-from mayan.apps.events.event_managers import (
-    EventManagerMethodAfter, EventManagerSave
-)
+from mayan.apps.events.event_managers import EventManagerSave
 
-from ..events import (
-    event_import_setup_item_created, event_import_setup_item_deleted,
-    event_import_setup_item_edited
+from ..events import event_import_setup_created, event_import_setup_edited
+from ..literals import (
+    DEFAULT_ITEM_TIME_BUFFER, DEFAULT_PROCESS_SIZE,
+    IMPORT_SETUP_STATE_CHOICES, IMPORT_SETUP_STATE_NONE
 )
-from ..literals import SETUP_ITEM_STATE_CHOICES, SETUP_ITEM_STATE_NONE
 
-from .import_setup_item_model_mixins import ImportSetupItemBusinessLogicMixin
-from .import_setup_models import ImportSetup
+from .import_setup_model_mixins import ImportSetupBusinessLogicMixin
+from .model_mixins import ModelMixinState
 
 
-class ImportSetupItem(ImportSetupItemBusinessLogicMixin, models.Model):
-    import_setup = models.ForeignKey(
-        on_delete=models.CASCADE, related_name='items',
-        to=ImportSetup, verbose_name=_(message='Import setup')
-    )
-    identifier = models.CharField(
-        db_index=True, help_text=_(
-            message='Source data element that uniquely identifies a file to '
-            'import.'
-        ), max_length=64, verbose_name=_(message='Identifier')
-    )
-    serialized_data = models.TextField(
-        blank=True, default='{}', help_text=_(
-            message='Source data corresponding to a file to import.'
-        ), verbose_name=_(message='Serialized data')
-    )
-    state = models.IntegerField(
-        db_index=True, choices=SETUP_ITEM_STATE_CHOICES,
-        default=SETUP_ITEM_STATE_NONE, verbose_name=_(message='State')
-    )
-    documents = models.ManyToManyField(
-        blank=True, related_name='import_items', to=Document,
-        verbose_name=_(message='Document')
+class ImportSetup(
+    BackendModelMixin, ImportSetupBusinessLogicMixin, ModelMixinState,
+    models.Model
+):
+    _ordering_fields = ('label', 'process_size', 'state')
+
+    label = models.CharField(
+        help_text=_(message='Short description of this import setup.'),
+        max_length=128, unique=True, verbose_name=_('Label')
+    )
+    document_type = models.ForeignKey(
+        on_delete=models.CASCADE, related_name='import_setups',
+        to=DocumentType, verbose_name=_(message='Document type')
+    )
+    process_size = models.PositiveIntegerField(
+        default=DEFAULT_PROCESS_SIZE, help_text=_(
+            'Number of items to process per execution.'
+        ), verbose_name=_(message='Process size')
+    )
+    item_time_buffer = models.PositiveIntegerField(
+        default=DEFAULT_ITEM_TIME_BUFFER, help_text=_(
+            'Delay in milliseconds between item import tasks execution.'
+        ), verbose_name=_(message='Item time buffer')
     )
 
     class Meta:
-        ordering = ('import_setup', 'identifier')
-        verbose_name = _(message='Import setup item')
-        verbose_name_plural = _(message='Import setup items')
+        ordering = ('label',)
+        state_choices = IMPORT_SETUP_STATE_CHOICES
+        state_default = IMPORT_SETUP_STATE_NONE
+        verbose_name = _(message='Import setup')
+        verbose_name_plural = _(message='Import setups')
 
     def __str__(self):
-        return self.identifier
+        return self.label
 
     def get_absolute_url(self):
-        return reverse(
-            viewname='importer:import_setup_items_list', kwargs={
-                'import_setup_id': self.import_setup.pk
-            }
-        )
-
-    @method_event(
-        event_manager_class=EventManagerMethodAfter,
-        event=event_import_setup_item_deleted,
-        action_object='self',
-        target='import_setup'
-    )
-    def delete(self):
-        return super().delete()
+        return reverse(viewname='importer:import_setup_list')
 
     @method_event(
         event_manager_class=EventManagerSave,
         created={
-            'action_object': 'import_setup',
-            'event': event_import_setup_item_created,
+            'event': event_import_setup_created,
             'target': 'self'
         },
         edited={
-            'action_object': 'import_setup',
-            'event': event_import_setup_item_edited,
+            'event': event_import_setup_edited,
             'target': 'self'
         }
     )
     def save(self, *args, **kwargs):
-        if not self.state:
-            self.state = SETUP_ITEM_STATE_NONE
-
-        super().save(*args, **kwargs)
+        return super().save(*args, **kwargs)
```

### Comparing `mayan-importer-3.0.3/importer/models/import_setup_model_mixins.py` & `mayan-importer-3.1/importer/models/import_setup_model_mixins.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,174 +6,169 @@
 from django.utils.translation import gettext_lazy as _
 
 from ..events import (
     event_import_setup_populate_finished, event_import_setup_populate_started,
     event_import_setup_process_finished, event_import_setup_process_started
 )
 from ..literals import (
-    ENABLE_STATE_CHANGE, SETUP_ITEM_STATE_COMPLETE, SETUP_STATE_ERROR,
-    SETUP_STATE_EXECUTING, SETUP_STATE_NONE, SETUP_STATE_POPULATING
+    IMPORT_SETUP_ITEM_STATE_PROCESSED, IMPORT_SETUP_STATE_ERROR,
+    IMPORT_SETUP_STATE_NONE, IMPORT_SETUP_STATE_POPULATING,
+    IMPORT_SETUP_STATE_POPULATED, IMPORT_SETUP_STATE_PROCESSING,
+    IMPORT_SETUP_STATE_PROCESSED
 )
-from ..tasks import task_import_setup_item_process_apply_async
+# ~ from ..tasks import task_import_setup_item_process_apply_async
 
 
 class ImportSetupBusinessLogicMixin:
-    def clear(self):
+    @classmethod
+    def get_process_allowed_state_list(self):
+        return (
+            IMPORT_SETUP_STATE_ERROR, IMPORT_SETUP_STATE_NONE,
+            IMPORT_SETUP_STATE_POPULATED, IMPORT_SETUP_STATE_PROCESSED
+        )
+
+    def do_clear(self):
         self.items.all().delete()
 
-    def get_state_label(self):
-        return self.get_state_display()
-    get_state_label.short_description = _(message='State')
-    get_state_label.help_text = _(
-        message='The last recorded state of the setup item. The field will '
-        'be sorted by the numeric value of the state and not the actual '
-        'text.'
-    )
-
-    def item_count_all(self):
-        return self.items.count()
-
-    item_count_all.short_description = _(message='Items')
-
-    def item_count_complete(self):
-        return self.items.filter(state=SETUP_ITEM_STATE_COMPLETE).count()
-
-    item_count_complete.short_description = _(message='Items complete')
-
-    def item_count_percent(self):
-        items_complete = self.item_count_complete()
-        items_all = self.item_count_all()
+    def do_populate(self, force=False, user=None):
+        if force or self.get_process_allowed():
+            event_import_setup_populate_started.commit(
+                actor=user, target=self
+            )
 
-        if items_all == 0:
-            percent = 0
-        else:
-            percent = items_complete / items_all * 100.0
+            self.do_state_set(state=IMPORT_SETUP_STATE_POPULATING)
 
-        return '{} of {} ({:.0f}%)'.format(
-            intcomma(value=items_complete), intcomma(value=items_all),
-            percent
-        )
+            try:
+                backend_instance = self.get_backend_instance()
 
-    item_count_percent.short_description = _(message='Progress')
+                for item in backend_instance.get_item_list():
 
-    def populate(self, user=None):
-        event_import_setup_populate_started.commit(
-            actor=user, target=self
-        )
+                    identifer_field = backend_instance.item_identifier
+                    try:
+                        # Try as an attribute.
+                        identifier = getattr(item, identifer_field)
+                    except (AttributeError, TypeError):
+                        # Try as dictionary.
+                        identifier = item[identifer_field]
 
-        if ENABLE_STATE_CHANGE:
-            self.state = SETUP_STATE_POPULATING
-            self.save()
-
-        try:
-            backend_instance = self.get_backend_instance()
-
-            for item in backend_instance.get_item_list():
-
-                identifer_field = backend_instance.item_identifier
-                try:
-                    # Try as an attribute.
-                    identifier = getattr(item, identifer_field)
-                except (AttributeError, TypeError):
-                    # Try as dictionary.
-                    identifier = item[identifer_field]
-
-                setup_item, created = self.items.get_or_create(
-                    identifier=identifier
-                )
-                if created:
-                    setup_item.dump_data(
-                        obj=item
+                    setup_item, created = self.items.get_or_create(
+                        identifier=identifier
+                    )
+                    if created:
+                        setup_item.do_data_dump(obj=item)
+                        setup_item.save()
+            except Exception as exception:
+                self.do_state_set(state=IMPORT_SETUP_STATE_ERROR)
+
+                self.error_log.create(
+                    text='{}; {}'.format(
+                        exception.__class__.__name__, exception
                     )
-                    setup_item.save()
-        except Exception as exception:
-            if ENABLE_STATE_CHANGE:
-                self.state = SETUP_STATE_ERROR
-                self.save()
-
-            self.error_log.create(
-                text='{}; {}'.format(
-                    exception.__class__.__name__, exception
                 )
-            )
-
-            if settings.DEBUG:
-                raise
-        else:
-            if ENABLE_STATE_CHANGE:
-                self.state = SETUP_STATE_NONE
-                self.save()
+                if settings.DEBUG:
+                    raise
+            else:
+                self.do_state_set(state=IMPORT_SETUP_STATE_POPULATED)
 
-            event_import_setup_populate_finished.commit(
-                actor=user, target=self
-            )
+                event_import_setup_populate_finished.commit(
+                    actor=user, target=self
+                )
 
-            queryset_logs = self.error_log.all()
-            queryset_logs.delete()
+                queryset_logs = self.error_log.all()
+                queryset_logs.delete()
 
-    def process(self, user=None):
+    def do_process(self, force=False, user=None):
         """
         Iterate of the `ImportSetupItem` instances downloading and creating
         documents from them.
         """
-        if ENABLE_STATE_CHANGE:
-            self.state = SETUP_STATE_EXECUTING
-            self.save()
+        if force or self.get_process_allowed():
+            self.do_state_set(state=IMPORT_SETUP_STATE_PROCESSING)
 
-        event_import_setup_process_started.commit(
-            actor=user, target=self
-        )
-
-        try:
-            count = 0
-            eta = datetime.utcnow()
-            # Only schedule items that have not succeeded in being imported.
-            ImportSetupItem = apps.get_model(
-                app_label='importer', model_name='ImportSetupItem'
-            )
-            queryset = self.items.exclude(
-                state__in=ImportSetupItem.get_process_allowed_state_list()
+            event_import_setup_process_started.commit(
+                actor=user, target=self
             )
-            iterator = queryset.iterator()
 
-            while True:
-                item = next(iterator)
-                if item.check_valid():
-                    count = count + 1
-                    eta += timedelta(milliseconds=self.item_time_buffer)
-                    task_import_setup_item_process_apply_async(
-                        eta=eta, kwargs={
-                            'import_setup_item_id': item.pk
-                        }
-                    )
-                    if count >= self.process_size:
-                        break
-        except StopIteration:
-            """
-            Expected exception when iterator is exhausted before the process
-            size is reached.
-            """
-        except Exception as exception:
-            if ENABLE_STATE_CHANGE:
-                self.state = SETUP_STATE_ERROR
-                self.save()
+            try:
+                count = 0
+                eta = datetime.utcnow()
+                # Only schedule items that have not succeeded in being
+                # imported.
+                ImportSetupItem = apps.get_model(
+                    app_label='importer', model_name='ImportSetupItem'
+                )
+                queryset = self.items.filter(
+                    state__in=ImportSetupItem.get_process_allowed_state_list()
+                )
+                iterator = queryset.iterator()
 
-            self.error_log.create(
-                text=str(exception)
-            )
+                while True:
+                    item = next(iterator)
+                    if item.do_check_valid():
+                        count = count + 1
+                        eta += timedelta(milliseconds=self.item_time_buffer)
+                        item.queue_task_import_setup_item_process(
+                            eta=eta, kwargs={'import_setup_item_id': item.pk}
+                        )
+
+                        if count >= self.process_size:
+                            break
+
+            except StopIteration:
+                """
+                Expected exception when iterator is exhausted before the
+                process size is reached.
+                """
+            except Exception as exception:
+                self.do_state_set(state=IMPORT_SETUP_STATE_ERROR)
+
+                self.error_log.create(
+                    text=str(exception)
+                )
+
+                if settings.DEBUG:
+                    raise
+
+                # Exit the method to avoid committing the ended event.
+                return
+
+            # This line is reached on `StopIteration` or from the break in the
+            # loop.
+            self.do_state_set(state=IMPORT_SETUP_STATE_PROCESSED)
+
+            queryset = self.error_log.all()
+            queryset.delete()
+
+            event_import_setup_process_finished.commit(actor=user, target=self)
+
+    def get_item_all_count(self):
+        queryset = self.items.all()
+        return queryset.count()
 
-            if settings.DEBUG:
-                raise
+    get_item_all_count.short_description = _(message='Items')
 
-            # Exit the method to avoid committing the ended event.
-            return
+    def get_item_processed_count(self):
+        queryset = self.items.filter(state=IMPORT_SETUP_ITEM_STATE_PROCESSED)
+        return queryset.count()
+
+    get_item_processed_count.short_description = _(message='Items complete')
+
+    def get_item_processed_percent(self):
+        items_complete = self.get_item_processed_count()
+        items_all = self.get_item_all_count()
+
+        if items_all == 0:
+            percent = 0
+        else:
+            percent = items_complete / items_all * 100.0
+
+        return '{} of {} ({:.0f}%)'.format(
+            intcomma(value=items_complete), intcomma(value=items_all),
+            percent
+        )
 
-        # This line is reached on `StopIteration` or from the break in the
-        # loop.
-        if ENABLE_STATE_CHANGE:
-            self.state = SETUP_STATE_NONE
-            self.save()
+    get_item_processed_percent.short_description = _(message='Progress')
 
-        queryset = self.error_log.all()
-        queryset.delete()
+    def get_process_allowed(self):
+        return self.state in self.get_process_allowed_state_list()
 
-        event_import_setup_process_finished.commit(actor=user, target=self)
+    get_process_allowed.short_description = _(message='Can be processed?')
```

### Comparing `mayan-importer-3.0.3/importer/permissions.py` & `mayan-importer-3.1/importer/permissions.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.3/importer/queues.py` & `mayan-importer-3.1/importer/queues.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.3/importer/serializers.py` & `mayan-importer-3.1/importer/serializers.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.3/importer/tasks.py` & `mayan-importer-3.1/importer/tasks.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,62 +2,46 @@
 
 from django.apps import apps
 from django.contrib.auth import get_user_model
 
 from mayan.celery import app
 
 from .classes import ModelFiler
-from .literals import SETUP_ITEM_STATE_QUEUED
 
 logger = logging.getLogger(name=__name__)
 
 
 @app.task(ignore_result=True)
 def task_import_setup_process(import_setup_id):
     ImportSetup = apps.get_model(
         app_label='importer', model_name='ImportSetup'
     )
 
     import_setup = ImportSetup.objects.get(pk=import_setup_id)
-    import_setup.process()
+    import_setup.do_process()
 
 
 @app.task(ignore_result=True)
 def task_import_setup_item_process(import_setup_item_id):
     ImportSetupItem = apps.get_model(
         app_label='importer', model_name='ImportSetupItem'
     )
 
     import_setup_item = ImportSetupItem.objects.get(pk=import_setup_item_id)
-    import_setup_item.process(force=True)
-
-
-def task_import_setup_item_process_apply_async(**kwargs):
-    task_code_kwargs = kwargs['kwargs']
-    import_setup_item_id = task_code_kwargs['import_setup_item_id']
-
-    ImportSetupItem = apps.get_model(
-        app_label='importer', model_name='ImportSetupItem'
-    )
-
-    ImportSetupItem.objects.filter(pk=import_setup_item_id).update(
-        state=SETUP_ITEM_STATE_QUEUED
-    )
-
-    task_import_setup_item_process.apply_async(**kwargs)
+    import_setup_item.do_process(force=True)
 
 
 @app.task(ignore_result=True)
 def task_import_setup_populate(import_setup_id):
     ImportSetup = apps.get_model(
         app_label='importer', model_name='ImportSetup'
     )
 
     import_setup = ImportSetup.objects.get(pk=import_setup_id)
-    import_setup.populate()
+    import_setup.do_populate()
 
 
 @app.task(ignore_result=True)
 def task_model_filer_load(
     full_model_name, shared_upload_file_id, field_defaults=None,
     organization_installation_url=None, user_id=None
 ):
```

### Comparing `mayan-importer-3.0.3/importer/tests/importers.py` & `mayan-importer-3.1/importer/tests/importers.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,20 @@
         return TestImporterItem(
             id=TEST_IMPORT_SETUP_ITEM_IDENTIFIER,
             name=TEST_IMPORT_SETUP_ITEM_NAME
         )
 
     @staticmethod
     def get_item_list():
-        return [TestImporter.get_test_item()]
+        return [
+            TestImporter.get_test_item()
+        ]
+
+    def do_check_valid(self, identifier, data):
+        return True
 
     def item_process(self, identifier, data):
         # Copy the Dropbox file to a temporary location using streaming
         # download.
         # The create a shared upload instance from the temporary file.
         with open(TEST_FILE_SMALL_PATH, mode='rb') as document_file_object:
             with NamedTemporaryFile() as file_object:
```

### Comparing `mayan-importer-3.0.3/importer/tests/mixins.py` & `mayan-importer-3.1/importer/tests/mixins.py`

 * *Files 4% similar despite different names*

```diff
@@ -235,18 +235,18 @@
                 'identifier': TEST_IMPORT_SETUP_ITEM_IDENTIFIER_EDITED,
                 'state': self.test_import_setup_item.state
             }
         )
 
     def _request_test_import_setup_process_view(self):
         return self.post(
-            viewname='importer:import_setup_process', kwargs={
+            viewname='importer:import_setup_process_single', kwargs={
                 'import_setup_id': self.test_import_setup.pk
             }
         )
 
     def _request_test_import_setup_populate_view(self):
         return self.post(
-            viewname='importer:import_setup_populate', kwargs={
+            viewname='importer:import_setup_populate_single', kwargs={
                 'import_setup_id': self.test_import_setup.pk
             }
         )
```

### Comparing `mayan-importer-3.0.3/importer/tests/test_import_setup_api.py` & `mayan-importer-3.1/importer/tests/test_import_setup_api.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.3/importer/tests/test_import_setup_item_api.py` & `mayan-importer-3.1/importer/tests/test_import_setup_item_api.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.3/importer/tests/test_import_setup_item_views.py` & `mayan-importer-3.1/importer/tests/test_import_setup_item_views.py`

 * *Files 4% similar despite different names*

```diff
@@ -265,71 +265,61 @@
         self.assertEqual(response.status_code, 302)
 
         self.assertEqual(
             self._test_document_type.documents.count(), document_count + 1
         )
 
         events = self._get_test_events()
-        self.assertEqual(events.count(), 10)
+        self.assertEqual(events.count(), 8)
 
         test_document = Document.objects.last()
         test_document_file = test_document.file_latest
         test_document_version = test_document.versions.last()
         test_document_version_page = test_document_version.pages.first()
 
-        test_import_setup_item = self.test_import_setup.items.first()
-
         self.assertEqual(events[0].action_object, None)
         self.assertEqual(events[0].actor, self.test_import_setup)
         self.assertEqual(events[0].target, self.test_import_setup)
         self.assertEqual(
             events[0].verb, event_import_setup_process_started.id
         )
 
-        self.assertEqual(events[1].action_object, self.test_import_setup)
-        self.assertEqual(events[1].actor, test_import_setup_item)
-        self.assertEqual(events[1].target, test_import_setup_item)
-        self.assertEqual(events[1].verb, event_import_setup_item_edited.id)
-
-        self.assertEqual(events[2].action_object, self._test_document_type)
-        self.assertEqual(events[2].actor, test_document)
-        self.assertEqual(events[2].target, test_document)
-        self.assertEqual(events[2].verb, event_document_created.id)
-
-        self.assertEqual(events[3].action_object, self.test_import_setup)
-        self.assertEqual(events[3].actor, test_import_setup_item)
-        self.assertEqual(events[3].target, test_import_setup_item)
-        self.assertEqual(events[3].verb, event_import_setup_item_edited.id)
+        self.assertEqual(events[1].action_object, self._test_document_type)
+        self.assertEqual(events[1].actor, test_document)
+        self.assertEqual(events[1].target, test_document)
+        self.assertEqual(events[1].verb, event_document_created.id)
+
+        self.assertEqual(events[2].action_object, test_document)
+        self.assertEqual(events[2].actor, test_document_file)
+        self.assertEqual(events[2].target, test_document_file)
+        self.assertEqual(events[2].verb, event_document_file_created.id)
+
+        self.assertEqual(events[3].action_object, test_document)
+        self.assertEqual(events[3].actor, test_document_file)
+        self.assertEqual(events[3].target, test_document_file)
+        self.assertEqual(events[3].verb, event_document_file_edited.id)
 
         self.assertEqual(events[4].action_object, test_document)
-        self.assertEqual(events[4].actor, test_document_file)
-        self.assertEqual(events[4].target, test_document_file)
-        self.assertEqual(events[4].verb, event_document_file_created.id)
-
-        self.assertEqual(events[5].action_object, test_document)
-        self.assertEqual(events[5].actor, test_document_file)
-        self.assertEqual(events[5].target, test_document_file)
-        self.assertEqual(events[5].verb, event_document_file_edited.id)
-
-        self.assertEqual(events[6].action_object, test_document)
-        self.assertEqual(events[6].actor, test_document_version)
-        self.assertEqual(events[6].target, test_document_version)
-        self.assertEqual(events[6].verb, event_document_version_created.id)
-
-        self.assertEqual(events[7].action_object, test_document_version)
-        self.assertEqual(events[7].actor, test_document_version_page)
-        self.assertEqual(events[7].target, test_document_version_page)
+        self.assertEqual(events[4].actor, test_document_version)
+        self.assertEqual(events[4].target, test_document_version)
+        self.assertEqual(events[4].verb, event_document_version_created.id)
+
+        self.assertEqual(events[5].action_object, test_document_version)
+        self.assertEqual(events[5].actor, test_document_version_page)
+        self.assertEqual(events[5].target, test_document_version_page)
         self.assertEqual(
-            events[7].verb, event_document_version_page_created.id
+            events[5].verb, event_document_version_page_created.id
         )
 
-        self.assertEqual(events[8].action_object, self.test_import_setup)
-        self.assertEqual(events[8].actor, self.test_import_setup_item)
-        self.assertEqual(events[8].target, self.test_import_setup_item)
+        self.assertEqual(events[6].action_object, self.test_import_setup)
+        self.assertEqual(events[6].actor, self.test_import_setup_item)
+        self.assertEqual(events[6].target, self.test_import_setup_item)
         self.assertEqual(
-            events[8].verb, event_import_setup_item_finished.id
+            events[6].verb, event_import_setup_item_finished.id
         )
 
-        self.assertEqual(events[9].action_object, None)
-        self.assertEqual(events[9].actor, self.test_import_setup)
-        self.assertEqual(events[9].target, self.test_import_setup)
-        self.assertEqual(events[9].verb, event_import_setup_process_finished.id)
+        self.assertEqual(events[7].action_object, None)
+        self.assertEqual(events[7].actor, self.test_import_setup)
+        self.assertEqual(events[7].target, self.test_import_setup)
+        self.assertEqual(
+            events[7].verb, event_import_setup_process_finished.id
+        )
```

### Comparing `mayan-importer-3.0.3/importer/tests/test_import_setup_views.py` & `mayan-importer-3.1/importer/tests/test_import_setup_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.3/importer/urls.py` & `mayan-importer-3.1/importer/urls.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 
 from .api_views import (
     APIImportSetupClearView, APIImportSetupDetailView,
     APIImportSetupListView, APIImportSetupPopulateView,
     APIImportSetupProcessView, APIImportSetupItemDetailView,
     APIImportSetupItemListView
 )
+from .views.import_setup_filer_views import (
+    ImportSetupFilerLoadView, ImportSetupFilerSaveConfirmView
+)
 from .views.import_setup_item_views import (
-    ImportSetupClearView, ImportSetupItemDeleteView,
-    ImportSetupItemDocumentListView, ImportSetupItemEditView,
-    ImportSetupItemListView, ImportSetupItemLoadView,
-    ImportSetupItemProcessView, ImportSetupItemSaveConfirmView,
-    ImportSetupPopulateView, ImportSetupProcessView
+    ImportSetupItemDeleteView, ImportSetupItemDocumentListView,
+    ImportSetupItemEditView, ImportSetupItemListView,
+    ImportSetupItemProcessView
 )
 from .views.import_setup_views import (
-    ImportSetupBackendSelectionView,
+    ImportSetupBackendSelectionView, ImportSetupClearView,
     ImportSetupCreateView, ImportSetupDeleteView, ImportSetupEditView,
-    ImportSetupListView
+    ImportSetupListView, ImportSetupPopulateView, ImportSetupProcessView
 )
 
 
 urlpatterns_import_setup = [
     url(
         regex=r'^import_setups/$', name='import_setup_list',
         view=ImportSetupListView.as_view()
@@ -41,64 +42,70 @@
     ),
     url(
         regex=r'^import_setups/(?P<import_setup_id>\d+)/edit/$',
         name='import_setup_edit', view=ImportSetupEditView.as_view()
     )
 ]
 
+urlpatterns_import_setup_filer = [
+    url(
+        regex=r'^import_setups/(?P<import_setup_id>\d+)/load/$',
+        name='import_setup_load', view=ImportSetupFilerLoadView.as_view()
+    ),
+    url(
+        regex=r'^import_setups/(?P<import_setup_id>\d+)/save/$',
+        name='import_setup_save', view=ImportSetupFilerSaveConfirmView.as_view()
+    )
+]
+
+
 urlpatterns_import_setup_items = [
     url(
         regex=r'^import_setups/(?P<import_setup_id>\d+)/clear/$',
         name='import_setup_clear',
         view=ImportSetupClearView.as_view()
     ),
     url(
         regex=r'^import_setups/multiple/clear/$',
         name='import_setup_multiple_clear',
         view=ImportSetupClearView.as_view()
     ),
     url(
-        regex=r'^import_setups/(?P<import_setup_id>\d+)/load/$',
-        name='import_setup_load', view=ImportSetupItemLoadView.as_view()
-    ),
-    url(
         regex=r'^import_setups/(?P<import_setup_id>\d+)/populate/$',
-        name='import_setup_populate', view=ImportSetupPopulateView.as_view()
+        name='import_setup_populate_single',
+        view=ImportSetupPopulateView.as_view()
     ),
     url(
         regex=r'^import_setups/multiple/populate/$',
-        name='import_setup_multiple_populate',
+        name='import_setup_populate_multiple',
         view=ImportSetupPopulateView.as_view()
     ),
     url(
         regex=r'^import_setups/(?P<import_setup_id>\d+)/process/$',
-        name='import_setup_process', view=ImportSetupProcessView.as_view()
+        name='import_setup_process_single',
+        view=ImportSetupProcessView.as_view()
     ),
     url(
         regex=r'^import_setups/multiple/process/$',
-        name='import_setup_multiple_process',
+        name='import_setup_process_multiple',
         view=ImportSetupProcessView.as_view()
     ),
     url(
-        regex=r'^import_setups/(?P<import_setup_id>\d+)/save/$',
-        name='import_setup_save', view=ImportSetupItemSaveConfirmView.as_view()
-    ),
-    url(
         regex=r'^import_setups/(?P<import_setup_id>\d+)/items/$',
         name='import_setup_items_list',
         view=ImportSetupItemListView.as_view()
     ),
     url(
         regex=r'^import_setups/items/(?P<import_setup_item_id>\d+)/delete/$',
-        name='import_setup_item_delete',
+        name='import_setup_item_delete_single',
         view=ImportSetupItemDeleteView.as_view()
     ),
     url(
         regex=r'^import_setups/items/multiple/delete/$',
-        name='import_setup_item_multiple_delete',
+        name='import_setup_item_delete_multiple',
         view=ImportSetupItemDeleteView.as_view()
     ),
     url(
         regex=r'^import_setups/items/(?P<import_setup_item_id>\d+)/documents/$',
         name='import_setup_item_document_list',
         view=ImportSetupItemDocumentListView.as_view()
     ),
@@ -110,26 +117,27 @@
     url(
         regex=r'^import_setups/items/(?P<import_setup_item_id>\d+)/edit/$',
         name='import_setup_item_edit',
         view=ImportSetupItemEditView.as_view()
     ),
     url(
         regex=r'^import_setups/items/multiple/process/$',
-        name='import_setup_item_multiple_process',
+        name='import_setup_item_process_multiple',
         view=ImportSetupItemProcessView.as_view()
     ),
     url(
         regex=r'^import_setups/items/(?P<import_setup_item_id>\d+)/process/$',
-        name='import_setup_item_process',
+        name='import_setup_item_process_single',
         view=ImportSetupItemProcessView.as_view()
     ),
 ]
 
 urlpatterns = []
 urlpatterns.extend(urlpatterns_import_setup)
+urlpatterns.extend(urlpatterns_import_setup_filer)
 urlpatterns.extend(urlpatterns_import_setup_items)
 
 api_urls = [
     url(
         regex=r'^import_setups/$', name='importsetup-list',
         view=APIImportSetupListView.as_view()
     ),
@@ -153,9 +161,9 @@
         regex=r'^import_setups/(?P<import_setup_id>[0-9]+)/items/$',
         name='importsetupitem-list', view=APIImportSetupItemListView.as_view()
     ),
     url(
         regex=r'^import_setups/(?P<import_setup_id>[0-9]+)/items/(?P<import_setup_item_id>[0-9]+)/$',
         name='importsetupitem-detail',
         view=APIImportSetupItemDetailView.as_view()
-    ),
+    )
 ]
```

### Comparing `mayan-importer-3.0.3/mayan_importer.egg-info/PKG-INFO` & `mayan-importer-3.1/mayan_importer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mayan-importer
-Version: 3.0.3
+Version: 3.1
 Summary: Mayan EDMS importer
 Home-page: https://gitlab.com/mayan-edms/importer
 Author: Roberto Rosario
 Author-email: roberto.rosario@mayan-edms.com
 License: Apache 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -93,14 +93,22 @@
 - Generate an Access Token with no expiration.
 - Create a credential instance in the Mayan EDMS Importer app and enter the Access Token.
 - Create an Import Setup that will filter the files to fetch from Dropbox.
 - Click the "Populate" button and check that the item count is correct.
 - Click the "Process" button to start the import process.
 
 
+3.1 (2024-05-03)
+================
+- Improve navigation.
+- Improve processing condition logic.
+- Split modules.
+- Move common state code into a mixin.
+- Add fieldsets.
+
 3.0 (2024-04-01)
 ================
 - Refactor app.
 - Remove import setup action.
 - Use source metadata to store import metadata.
 - Don't deserialize import item source column.
 - Use upstream backend, dynamic forms, credentials mixins, model mixins,
```

### Comparing `mayan-importer-3.0.3/mayan_importer.egg-info/SOURCES.txt` & `mayan-importer-3.1/mayan_importer.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,24 +8,34 @@
 importer/admin.py
 importer/api_views.py
 importer/apps.py
 importer/classes.py
 importer/dependencies.py
 importer/events.py
 importer/exceptions.py
-importer/forms.py
-importer/icons.py
 importer/importers.py
-importer/links.py
 importer/literals.py
 importer/permissions.py
 importer/queues.py
 importer/serializers.py
 importer/tasks.py
 importer/urls.py
+importer/forms/__init__.py
+importer/forms/filer_forms.py
+importer/forms/form_mixins.py
+importer/forms/import_setup_forms.py
+importer/forms/import_setup_item_forms.py
+importer/icons/__init__.py
+importer/icons/import_setup_filer_icons.py
+importer/icons/import_setup_icons.py
+importer/icons/import_setup_item_icons.py
+importer/links/__init__.py
+importer/links/import_setup_filer_links.py
+importer/links/import_setup_item_links.py
+importer/links/import_setup_links.py
 importer/migrations/0001_initial.py
 importer/migrations/0002_auto_20200908_0458.py
 importer/migrations/0003_importsetup_metadata_map.py
 importer/migrations/0004_auto_20200908_0853.py
 importer/migrations/0005_importsetup_state.py
 importer/migrations/0006_auto_20200924_0802.py
 importer/migrations/0007_auto_20200924_0802.py
@@ -37,29 +47,34 @@
 importer/migrations/0013_auto_20201225_0155.py
 importer/migrations/0014_auto_20201227_0610.py
 importer/migrations/0015_auto_20220901_0932.py
 importer/migrations/0016_importsetup_item_time_buffer.py
 importer/migrations/0017_delete_importsetuplog.py
 importer/migrations/0018_auto_20240401_0808.py
 importer/migrations/0019_auto_20240402_1101.py
+importer/migrations/0020_auto_20240502_1907.py
+importer/migrations/0021_migrate_state_codes.py
+importer/migrations/0022_auto_20240503_0853.py
 importer/migrations/__init__.py
 importer/models/__init__.py
 importer/models/import_setup_item_model_mixins.py
 importer/models/import_setup_item_models.py
 importer/models/import_setup_model_mixins.py
 importer/models/import_setup_models.py
+importer/models/model_mixins.py
 importer/tests/__init__.py
 importer/tests/importers.py
 importer/tests/literals.py
 importer/tests/mixins.py
 importer/tests/test_import_setup_api.py
 importer/tests/test_import_setup_item_api.py
 importer/tests/test_import_setup_item_views.py
 importer/tests/test_import_setup_views.py
 importer/views/__init__.py
+importer/views/import_setup_filer_views.py
 importer/views/import_setup_item_views.py
 importer/views/import_setup_views.py
 mayan_importer.egg-info/PKG-INFO
 mayan_importer.egg-info/SOURCES.txt
 mayan_importer.egg-info/dependency_links.txt
 mayan_importer.egg-info/not-zip-safe
 mayan_importer.egg-info/requires.txt
```

### Comparing `mayan-importer-3.0.3/setup.py` & `mayan-importer-3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,10 +94,10 @@
     license='Apache 2.0',
     long_description=readme + '\n\n' + history,
     name=PACKAGE_NAME,
     packages=find_packages(PACKAGE_DIR),
     platforms=['any'],
     python_requires='!=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*',
     url='https://gitlab.com/mayan-edms/importer',
-    version='3.0.3',
+    version='3.1',
     zip_safe=False,
 )
```

