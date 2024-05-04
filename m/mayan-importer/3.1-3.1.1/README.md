# Comparing `tmp/mayan-importer-3.1.tar.gz` & `tmp/mayan-importer-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mayan-importer-3.1.tar", last modified: Fri May  3 08:55:35 2024, max compression
+gzip compressed data, was "mayan-importer-3.1.1.tar", last modified: Sat May  4 07:50:15 2024, max compression
```

## Comparing `mayan-importer-3.1.tar` & `mayan-importer-3.1.1.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-03 08:55:35.871172 mayan-importer-3.1/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6509 2024-05-03 08:54:55.000000 mayan-importer-3.1/HISTORY.rst
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      555 2020-10-02 10:42:37.000000 mayan-importer-3.1/LICENSE
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       39 2020-10-02 10:42:37.000000 mayan-importer-3.1/MANIFEST.in
--rw-r--r--   0 rosarior  (1000) rosarior  (1000)     9399 2024-05-03 08:55:35.871172 mayan-importer-3.1/PKG-INFO
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1628 2020-10-02 10:42:37.000000 mayan-importer-3.1/README.rst
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-03 08:55:35.863172 mayan-importer-3.1/importer/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       49 2020-10-02 10:42:37.000000 mayan-importer-3.1/importer/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      405 2024-04-01 10:00:47.000000 mayan-importer-3.1/importer/admin.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4643 2024-04-01 10:00:47.000000 mayan-importer-3.1/importer/api_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7817 2024-05-03 08:03:48.000000 mayan-importer-3.1/importer/apps.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7182 2024-05-03 08:30:22.000000 mayan-importer-3.1/importer/classes.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      145 2024-04-01 10:00:47.000000 mayan-importer-3.1/importer/dependencies.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1729 2024-04-01 10:00:47.000000 mayan-importer-3.1/importer/events.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       93 2024-04-01 10:00:47.000000 mayan-importer-3.1/importer/exceptions.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-03 08:55:35.863172 mayan-importer-3.1/importer/forms/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-05-03 06:18:39.000000 mayan-importer-3.1/importer/forms/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      326 2024-05-03 06:38:56.000000 mayan-importer-3.1/importer/forms/filer_forms.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      431 2024-05-03 08:05:46.000000 mayan-importer-3.1/importer/forms/form_mixins.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      949 2024-05-03 06:38:56.000000 mayan-importer-3.1/importer/forms/import_setup_forms.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      591 2024-05-03 06:40:26.000000 mayan-importer-3.1/importer/forms/import_setup_item_forms.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-03 08:55:35.864172 mayan-importer-3.1/importer/icons/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-05-02 06:30:26.000000 mayan-importer-3.1/importer/icons/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      222 2024-05-03 06:38:56.000000 mayan-importer-3.1/importer/icons/import_setup_filer_icons.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      914 2024-05-03 06:38:56.000000 mayan-importer-3.1/importer/icons/import_setup_icons.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      710 2024-05-03 06:38:56.000000 mayan-importer-3.1/importer/icons/import_setup_item_icons.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8715 2024-05-03 08:31:33.000000 mayan-importer-3.1/importer/importers.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-03 08:55:35.864172 mayan-importer-3.1/importer/links/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-05-02 06:05:24.000000 mayan-importer-3.1/importer/links/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      974 2024-05-03 06:38:56.000000 mayan-importer-3.1/importer/links/import_setup_filer_links.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2534 2024-05-03 06:38:56.000000 mayan-importer-3.1/importer/links/import_setup_item_links.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3461 2024-05-03 06:37:19.000000 mayan-importer-3.1/importer/links/import_setup_links.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1205 2024-05-02 22:28:59.000000 mayan-importer-3.1/importer/literals.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-03 08:55:35.867172 mayan-importer-3.1/importer/migrations/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4126 2020-10-02 10:42:37.000000 mayan-importer-3.1/importer/migrations/0001_initial.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1475 2020-10-02 10:42:37.000000 mayan-importer-3.1/importer/migrations/0002_auto_20200908_0458.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      669 2020-10-02 10:42:37.000000 mayan-importer-3.1/importer/migrations/0003_importsetup_metadata_map.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      795 2023-04-12 05:57:59.000000 mayan-importer-3.1/importer/migrations/0004_auto_20200908_0853.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      607 2023-04-12 05:57:59.000000 mayan-importer-3.1/importer/migrations/0005_importsetup_state.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      333 2023-04-12 05:57:59.000000 mayan-importer-3.1/importer/migrations/0006_auto_20200924_0802.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      428 2023-04-12 05:57:59.000000 mayan-importer-3.1/importer/migrations/0007_auto_20200924_0802.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      603 2023-04-12 05:57:59.000000 mayan-importer-3.1/importer/migrations/0008_auto_20200924_0903.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2451 2023-04-12 05:57:59.000000 mayan-importer-3.1/importer/migrations/0009_importsetupaction.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      287 2024-05-02 22:00:10.000000 mayan-importer-3.1/importer/migrations/0010_remove_importsetup_metadata_map.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      568 2023-04-12 05:57:59.000000 mayan-importer-3.1/importer/migrations/0011_auto_20201004_0042.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      522 2023-04-12 05:57:59.000000 mayan-importer-3.1/importer/migrations/0012_importsetupitem_documents.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1796 2023-04-12 05:57:59.000000 mayan-importer-3.1/importer/migrations/0013_auto_20201225_0155.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      396 2023-04-12 05:57:59.000000 mayan-importer-3.1/importer/migrations/0014_auto_20201227_0610.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      848 2023-04-12 05:57:59.000000 mayan-importer-3.1/importer/migrations/0015_auto_20220901_0932.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      526 2023-04-12 05:57:59.000000 mayan-importer-3.1/importer/migrations/0016_importsetup_item_time_buffer.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      239 2024-04-01 10:00:47.000000 mayan-importer-3.1/importer/migrations/0017_delete_importsetuplog.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1064 2024-04-01 10:00:47.000000 mayan-importer-3.1/importer/migrations/0018_auto_20240401_0808.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1326 2024-04-02 11:02:22.000000 mayan-importer-3.1/importer/migrations/0019_auto_20240402_1101.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1449 2024-05-02 19:09:03.000000 mayan-importer-3.1/importer/migrations/0020_auto_20240502_1907.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1596 2024-05-03 06:35:16.000000 mayan-importer-3.1/importer/migrations/0021_migrate_state_codes.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1063 2024-05-03 08:53:58.000000 mayan-importer-3.1/importer/migrations/0022_auto_20240503_0853.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2020-10-02 10:42:37.000000 mayan-importer-3.1/importer/migrations/__init__.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-03 08:55:35.868172 mayan-importer-3.1/importer/models/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      134 2024-04-01 10:00:47.000000 mayan-importer-3.1/importer/models/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4172 2024-05-03 08:45:32.000000 mayan-importer-3.1/importer/models/import_setup_item_model_mixins.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2945 2024-05-03 07:37:19.000000 mayan-importer-3.1/importer/models/import_setup_item_models.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6122 2024-05-03 08:39:32.000000 mayan-importer-3.1/importer/models/import_setup_model_mixins.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2421 2024-05-03 08:48:29.000000 mayan-importer-3.1/importer/models/import_setup_models.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3132 2024-05-03 08:49:55.000000 mayan-importer-3.1/importer/models/model_mixins.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1386 2024-04-01 10:00:47.000000 mayan-importer-3.1/importer/permissions.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1197 2024-04-01 10:00:47.000000 mayan-importer-3.1/importer/queues.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3473 2024-04-01 10:00:47.000000 mayan-importer-3.1/importer/serializers.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2314 2024-05-03 08:30:22.000000 mayan-importer-3.1/importer/tasks.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-03 08:55:35.869171 mayan-importer-3.1/importer/tests/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 10:00:47.000000 mayan-importer-3.1/importer/tests/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1650 2024-05-03 08:30:22.000000 mayan-importer-3.1/importer/tests/importers.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      408 2024-04-01 10:00:47.000000 mayan-importer-3.1/importer/tests/literals.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8743 2024-05-03 08:05:05.000000 mayan-importer-3.1/importer/tests/mixins.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8233 2024-05-03 08:09:51.000000 mayan-importer-3.1/importer/tests/test_import_setup_api.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7881 2024-04-01 10:00:47.000000 mayan-importer-3.1/importer/tests/test_import_setup_item_api.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    11635 2024-05-03 08:50:46.000000 mayan-importer-3.1/importer/tests/test_import_setup_item_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6425 2024-04-01 10:00:47.000000 mayan-importer-3.1/importer/tests/test_import_setup_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     5779 2024-05-02 06:54:59.000000 mayan-importer-3.1/importer/urls.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-03 08:55:35.870171 mayan-importer-3.1/importer/views/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2023-04-12 05:57:59.000000 mayan-importer-3.1/importer/views/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3693 2024-05-03 06:34:50.000000 mayan-importer-3.1/importer/views/import_setup_filer_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8134 2024-05-03 08:02:03.000000 mayan-importer-3.1/importer/views/import_setup_item_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     9643 2024-05-03 08:07:00.000000 mayan-importer-3.1/importer/views/import_setup_views.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-03 08:55:35.871172 mayan-importer-3.1/mayan_importer.egg-info/
--rw-r--r--   0 rosarior  (1000) rosarior  (1000)     9399 2024-05-03 08:55:35.000000 mayan-importer-3.1/mayan_importer.egg-info/PKG-INFO
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2822 2024-05-03 08:55:35.000000 mayan-importer-3.1/mayan_importer.egg-info/SOURCES.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2024-05-03 08:55:35.000000 mayan-importer-3.1/mayan_importer.egg-info/dependency_links.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2024-05-03 08:55:35.000000 mayan-importer-3.1/mayan_importer.egg-info/not-zip-safe
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       16 2024-05-03 08:55:35.000000 mayan-importer-3.1/mayan_importer.egg-info/requires.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        9 2024-05-03 08:55:35.000000 mayan-importer-3.1/mayan_importer.egg-info/top_level.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      129 2024-05-03 08:55:35.871172 mayan-importer-3.1/setup.cfg
--rwxrwxr-x   0 rosarior  (1000) rosarior  (1000)     3036 2024-05-03 08:54:32.000000 mayan-importer-3.1/setup.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-04 07:50:15.169953 mayan-importer-3.1.1/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6566 2024-05-04 07:49:13.000000 mayan-importer-3.1.1/HISTORY.rst
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      555 2020-10-02 10:42:37.000000 mayan-importer-3.1.1/LICENSE
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       39 2020-10-02 10:42:37.000000 mayan-importer-3.1.1/MANIFEST.in
+-rw-r--r--   0 rosarior  (1000) rosarior  (1000)     9458 2024-05-04 07:50:15.169953 mayan-importer-3.1.1/PKG-INFO
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1628 2020-10-02 10:42:37.000000 mayan-importer-3.1.1/README.rst
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-04 07:50:15.158953 mayan-importer-3.1.1/importer/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       49 2020-10-02 10:42:37.000000 mayan-importer-3.1.1/importer/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      405 2024-04-01 10:00:47.000000 mayan-importer-3.1.1/importer/admin.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4643 2024-04-01 10:00:47.000000 mayan-importer-3.1.1/importer/api_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7817 2024-05-04 06:47:22.000000 mayan-importer-3.1.1/importer/apps.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7165 2024-05-03 23:02:13.000000 mayan-importer-3.1.1/importer/classes.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      145 2024-04-01 10:00:47.000000 mayan-importer-3.1.1/importer/dependencies.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1729 2024-04-01 10:00:47.000000 mayan-importer-3.1.1/importer/events.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       93 2024-04-01 10:00:47.000000 mayan-importer-3.1.1/importer/exceptions.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-04 07:50:15.159953 mayan-importer-3.1.1/importer/forms/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-05-03 06:18:39.000000 mayan-importer-3.1.1/importer/forms/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      327 2024-05-04 06:39:44.000000 mayan-importer-3.1.1/importer/forms/filer_forms.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      431 2024-05-03 08:05:46.000000 mayan-importer-3.1.1/importer/forms/form_mixins.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      949 2024-05-03 06:38:56.000000 mayan-importer-3.1.1/importer/forms/import_setup_forms.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      591 2024-05-03 06:40:26.000000 mayan-importer-3.1.1/importer/forms/import_setup_item_forms.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-04 07:50:15.160953 mayan-importer-3.1.1/importer/icons/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-05-02 06:30:26.000000 mayan-importer-3.1.1/importer/icons/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      222 2024-05-03 06:38:56.000000 mayan-importer-3.1.1/importer/icons/import_setup_filer_icons.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      914 2024-05-03 06:38:56.000000 mayan-importer-3.1.1/importer/icons/import_setup_icons.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      710 2024-05-03 06:38:56.000000 mayan-importer-3.1.1/importer/icons/import_setup_item_icons.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8715 2024-05-03 08:31:33.000000 mayan-importer-3.1.1/importer/importers.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-04 07:50:15.161953 mayan-importer-3.1.1/importer/links/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-05-02 06:05:24.000000 mayan-importer-3.1.1/importer/links/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      974 2024-05-03 06:38:56.000000 mayan-importer-3.1.1/importer/links/import_setup_filer_links.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2534 2024-05-03 06:38:56.000000 mayan-importer-3.1.1/importer/links/import_setup_item_links.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3461 2024-05-03 06:37:19.000000 mayan-importer-3.1.1/importer/links/import_setup_links.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1205 2024-05-02 22:28:59.000000 mayan-importer-3.1.1/importer/literals.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-04 07:50:15.164953 mayan-importer-3.1.1/importer/migrations/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4126 2020-10-02 10:42:37.000000 mayan-importer-3.1.1/importer/migrations/0001_initial.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1475 2020-10-02 10:42:37.000000 mayan-importer-3.1.1/importer/migrations/0002_auto_20200908_0458.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      669 2020-10-02 10:42:37.000000 mayan-importer-3.1.1/importer/migrations/0003_importsetup_metadata_map.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      795 2023-04-12 05:57:59.000000 mayan-importer-3.1.1/importer/migrations/0004_auto_20200908_0853.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      607 2023-04-12 05:57:59.000000 mayan-importer-3.1.1/importer/migrations/0005_importsetup_state.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      333 2023-04-12 05:57:59.000000 mayan-importer-3.1.1/importer/migrations/0006_auto_20200924_0802.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      428 2023-04-12 05:57:59.000000 mayan-importer-3.1.1/importer/migrations/0007_auto_20200924_0802.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      603 2023-04-12 05:57:59.000000 mayan-importer-3.1.1/importer/migrations/0008_auto_20200924_0903.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2451 2023-04-12 05:57:59.000000 mayan-importer-3.1.1/importer/migrations/0009_importsetupaction.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      287 2024-05-02 22:00:10.000000 mayan-importer-3.1.1/importer/migrations/0010_remove_importsetup_metadata_map.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      568 2023-04-12 05:57:59.000000 mayan-importer-3.1.1/importer/migrations/0011_auto_20201004_0042.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      522 2023-04-12 05:57:59.000000 mayan-importer-3.1.1/importer/migrations/0012_importsetupitem_documents.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1796 2023-04-12 05:57:59.000000 mayan-importer-3.1.1/importer/migrations/0013_auto_20201225_0155.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      396 2023-04-12 05:57:59.000000 mayan-importer-3.1.1/importer/migrations/0014_auto_20201227_0610.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      848 2023-04-12 05:57:59.000000 mayan-importer-3.1.1/importer/migrations/0015_auto_20220901_0932.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      526 2023-04-12 05:57:59.000000 mayan-importer-3.1.1/importer/migrations/0016_importsetup_item_time_buffer.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      239 2024-04-01 10:00:47.000000 mayan-importer-3.1.1/importer/migrations/0017_delete_importsetuplog.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1064 2024-04-01 10:00:47.000000 mayan-importer-3.1.1/importer/migrations/0018_auto_20240401_0808.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1326 2024-04-02 11:02:22.000000 mayan-importer-3.1.1/importer/migrations/0019_auto_20240402_1101.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1449 2024-05-02 19:09:03.000000 mayan-importer-3.1.1/importer/migrations/0020_auto_20240502_1907.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1596 2024-05-03 06:35:16.000000 mayan-importer-3.1.1/importer/migrations/0021_migrate_state_codes.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1063 2024-05-03 08:53:58.000000 mayan-importer-3.1.1/importer/migrations/0022_auto_20240503_0853.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2020-10-02 10:42:37.000000 mayan-importer-3.1.1/importer/migrations/__init__.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-04 07:50:15.165953 mayan-importer-3.1.1/importer/models/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       91 2024-05-04 07:48:41.000000 mayan-importer-3.1.1/importer/models/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4172 2024-05-03 08:45:32.000000 mayan-importer-3.1.1/importer/models/import_setup_item_model_mixins.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2945 2024-05-03 07:37:19.000000 mayan-importer-3.1.1/importer/models/import_setup_item_models.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6055 2024-05-04 06:55:03.000000 mayan-importer-3.1.1/importer/models/import_setup_model_mixins.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2421 2024-05-04 06:55:15.000000 mayan-importer-3.1.1/importer/models/import_setup_models.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3132 2024-05-04 06:54:17.000000 mayan-importer-3.1.1/importer/models/model_mixins.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1386 2024-04-01 10:00:47.000000 mayan-importer-3.1.1/importer/permissions.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1197 2024-04-01 10:00:47.000000 mayan-importer-3.1.1/importer/queues.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3473 2024-04-01 10:00:47.000000 mayan-importer-3.1.1/importer/serializers.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2314 2024-05-03 08:30:22.000000 mayan-importer-3.1.1/importer/tasks.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-04 07:50:15.167953 mayan-importer-3.1.1/importer/tests/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 10:00:47.000000 mayan-importer-3.1.1/importer/tests/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1650 2024-05-03 08:30:22.000000 mayan-importer-3.1.1/importer/tests/importers.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      695 2024-05-04 07:00:01.000000 mayan-importer-3.1.1/importer/tests/literals.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1294 2024-05-04 07:47:44.000000 mayan-importer-3.1.1/importer/tests/test_filer_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8230 2024-05-04 06:59:12.000000 mayan-importer-3.1.1/importer/tests/test_import_setup_api.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7720 2024-05-04 07:46:59.000000 mayan-importer-3.1.1/importer/tests/test_import_setup_item_api.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    11484 2024-05-04 07:46:59.000000 mayan-importer-3.1.1/importer/tests/test_import_setup_item_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6309 2024-05-04 07:46:59.000000 mayan-importer-3.1.1/importer/tests/test_import_setup_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     5787 2024-05-04 06:26:52.000000 mayan-importer-3.1.1/importer/urls.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-04 07:50:15.167953 mayan-importer-3.1.1/importer/views/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2023-04-12 05:57:59.000000 mayan-importer-3.1.1/importer/views/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3693 2024-05-03 06:34:50.000000 mayan-importer-3.1.1/importer/views/import_setup_filer_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8134 2024-05-03 08:02:03.000000 mayan-importer-3.1.1/importer/views/import_setup_item_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     9643 2024-05-03 08:07:00.000000 mayan-importer-3.1.1/importer/views/import_setup_views.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-05-04 07:50:15.168953 mayan-importer-3.1.1/mayan_importer.egg-info/
+-rw-r--r--   0 rosarior  (1000) rosarior  (1000)     9458 2024-05-04 07:50:15.000000 mayan-importer-3.1.1/mayan_importer.egg-info/PKG-INFO
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2832 2024-05-04 07:50:15.000000 mayan-importer-3.1.1/mayan_importer.egg-info/SOURCES.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2024-05-04 07:50:15.000000 mayan-importer-3.1.1/mayan_importer.egg-info/dependency_links.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2024-05-04 07:50:15.000000 mayan-importer-3.1.1/mayan_importer.egg-info/not-zip-safe
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       16 2024-05-04 07:50:15.000000 mayan-importer-3.1.1/mayan_importer.egg-info/requires.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        9 2024-05-04 07:50:15.000000 mayan-importer-3.1.1/mayan_importer.egg-info/top_level.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      129 2024-05-04 07:50:15.169953 mayan-importer-3.1.1/setup.cfg
+-rwxrwxr-x   0 rosarior  (1000) rosarior  (1000)     3038 2024-05-04 07:49:25.000000 mayan-importer-3.1.1/setup.py
```

### Comparing `mayan-importer-3.1/HISTORY.rst` & `mayan-importer-3.1.1/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+3.1.1 (2024-05-04)
+==================
+- Fix filer load.
+
 3.1 (2024-05-03)
 ================
 - Improve navigation.
 - Improve processing condition logic.
 - Split modules.
 - Move common state code into a mixin.
 - Add fieldsets.
```

### Comparing `mayan-importer-3.1/LICENSE` & `mayan-importer-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/PKG-INFO` & `mayan-importer-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mayan-importer
-Version: 3.1
+Version: 3.1.1
 Summary: Mayan EDMS importer
 Home-page: https://gitlab.com/mayan-edms/importer
 Author: Roberto Rosario
 Author-email: roberto.rosario@mayan-edms.com
 License: Apache 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -93,14 +93,18 @@
 - Generate an Access Token with no expiration.
 - Create a credential instance in the Mayan EDMS Importer app and enter the Access Token.
 - Create an Import Setup that will filter the files to fetch from Dropbox.
 - Click the "Populate" button and check that the item count is correct.
 - Click the "Process" button to start the import process.
 
 
+3.1.1 (2024-05-04)
+==================
+- Fix filer load.
+
 3.1 (2024-05-03)
 ================
 - Improve navigation.
 - Improve processing condition logic.
 - Split modules.
 - Move common state code into a mixin.
 - Add fieldsets.
```

### Comparing `mayan-importer-3.1/README.rst` & `mayan-importer-3.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/api_views.py` & `mayan-importer-3.1.1/importer/api_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/apps.py` & `mayan-importer-3.1.1/importer/apps.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/classes.py` & `mayan-importer-3.1.1/importer/classes.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,44 +110,43 @@
     def get_model_full_name(self):
         return ModelFiler.get_full_model_name(model=self.model)
 
     def items_load(self, shared_upload_file, field_defaults=None, user=None):
         if not field_defaults:
             field_defaults = {}
 
-        field_names = ModelFiler.get_field_names(model=self.model)
-
         manager = self.model._meta.default_manager
 
         if self.bulk_size:
             manager.filter(**field_defaults).delete()
         else:
             for instance in manager.filter(**field_defaults):
                 instance.delete()
 
         with shared_upload_file.open() as file_object_binary:
             with io.TextIOWrapper(file_object_binary) as file_object:
-                file_object.readline()  # Header
-                reader = csv.DictReader(file_object, fieldnames=field_names)
+                reader = csv.reader(file_object, delimiter=',')
+                header = next(reader)
+
+                reader = csv.DictReader(file_object, fieldnames=header)
 
                 if self.bulk_size:
-                    bulk_list = []
                     bulk_count = 0
+                    bulk_list = []
 
                     for row in reader:
                         row.update(**field_defaults)
-                        bulk_list.append(
-                            self.model(**row)
-                        )
+                        model_instance = self.model(**row)
+                        bulk_list.append(model_instance)
                         bulk_count += 1
 
                         if bulk_count > self.bulk_size:
                             manager.bulk_create(bulk_list)
-                            bulk_list = []
                             bulk_count = 0
+                            bulk_list = []
 
                     manager.bulk_create(bulk_list)
                 else:
                     for row in reader:
                         row.update(**field_defaults)
                         manager.create(**row)
```

### Comparing `mayan-importer-3.1/importer/events.py` & `mayan-importer-3.1.1/importer/events.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/forms/import_setup_forms.py` & `mayan-importer-3.1.1/importer/forms/import_setup_forms.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/forms/import_setup_item_forms.py` & `mayan-importer-3.1.1/importer/forms/import_setup_item_forms.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/icons/import_setup_icons.py` & `mayan-importer-3.1.1/importer/icons/import_setup_icons.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/icons/import_setup_item_icons.py` & `mayan-importer-3.1.1/importer/icons/import_setup_item_icons.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/importers.py` & `mayan-importer-3.1.1/importer/importers.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/links/import_setup_filer_links.py` & `mayan-importer-3.1.1/importer/links/import_setup_filer_links.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/links/import_setup_item_links.py` & `mayan-importer-3.1.1/importer/links/import_setup_item_links.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/links/import_setup_links.py` & `mayan-importer-3.1.1/importer/links/import_setup_links.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/literals.py` & `mayan-importer-3.1.1/importer/literals.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/migrations/0001_initial.py` & `mayan-importer-3.1.1/importer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/migrations/0002_auto_20200908_0458.py` & `mayan-importer-3.1.1/importer/migrations/0002_auto_20200908_0458.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/migrations/0003_importsetup_metadata_map.py` & `mayan-importer-3.1.1/importer/migrations/0003_importsetup_metadata_map.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/migrations/0004_auto_20200908_0853.py` & `mayan-importer-3.1.1/importer/migrations/0004_auto_20200908_0853.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/migrations/0005_importsetup_state.py` & `mayan-importer-3.1.1/importer/migrations/0005_importsetup_state.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/migrations/0008_auto_20200924_0903.py` & `mayan-importer-3.1.1/importer/migrations/0008_auto_20200924_0903.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/migrations/0009_importsetupaction.py` & `mayan-importer-3.1.1/importer/migrations/0009_importsetupaction.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/migrations/0011_auto_20201004_0042.py` & `mayan-importer-3.1.1/importer/migrations/0011_auto_20201004_0042.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/migrations/0012_importsetupitem_documents.py` & `mayan-importer-3.1.1/importer/migrations/0012_importsetupitem_documents.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/migrations/0013_auto_20201225_0155.py` & `mayan-importer-3.1.1/importer/migrations/0013_auto_20201225_0155.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/migrations/0015_auto_20220901_0932.py` & `mayan-importer-3.1.1/importer/migrations/0015_auto_20220901_0932.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/migrations/0016_importsetup_item_time_buffer.py` & `mayan-importer-3.1.1/importer/migrations/0016_importsetup_item_time_buffer.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/migrations/0018_auto_20240401_0808.py` & `mayan-importer-3.1.1/importer/migrations/0018_auto_20240401_0808.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/migrations/0019_auto_20240402_1101.py` & `mayan-importer-3.1.1/importer/migrations/0019_auto_20240402_1101.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/migrations/0020_auto_20240502_1907.py` & `mayan-importer-3.1.1/importer/migrations/0020_auto_20240502_1907.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/migrations/0021_migrate_state_codes.py` & `mayan-importer-3.1.1/importer/migrations/0021_migrate_state_codes.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/migrations/0022_auto_20240503_0853.py` & `mayan-importer-3.1.1/importer/migrations/0022_auto_20240503_0853.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/models/import_setup_item_model_mixins.py` & `mayan-importer-3.1.1/importer/models/import_setup_item_model_mixins.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/models/import_setup_item_models.py` & `mayan-importer-3.1.1/importer/models/import_setup_item_models.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/models/import_setup_model_mixins.py` & `mayan-importer-3.1.1/importer/models/import_setup_model_mixins.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 )
 from ..literals import (
     IMPORT_SETUP_ITEM_STATE_PROCESSED, IMPORT_SETUP_STATE_ERROR,
     IMPORT_SETUP_STATE_NONE, IMPORT_SETUP_STATE_POPULATING,
     IMPORT_SETUP_STATE_POPULATED, IMPORT_SETUP_STATE_PROCESSING,
     IMPORT_SETUP_STATE_PROCESSED
 )
-# ~ from ..tasks import task_import_setup_item_process_apply_async
 
 
 class ImportSetupBusinessLogicMixin:
     @classmethod
     def get_process_allowed_state_list(self):
         return (
             IMPORT_SETUP_STATE_ERROR, IMPORT_SETUP_STATE_NONE,
```

### Comparing `mayan-importer-3.1/importer/models/import_setup_models.py` & `mayan-importer-3.1.1/importer/models/import_setup_models.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/models/model_mixins.py` & `mayan-importer-3.1.1/importer/models/model_mixins.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/permissions.py` & `mayan-importer-3.1.1/importer/permissions.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/queues.py` & `mayan-importer-3.1.1/importer/queues.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/serializers.py` & `mayan-importer-3.1.1/importer/serializers.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/tasks.py` & `mayan-importer-3.1.1/importer/tasks.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/tests/importers.py` & `mayan-importer-3.1.1/importer/tests/importers.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/tests/test_import_setup_api.py` & `mayan-importer-3.1.1/importer/tests/test_import_setup_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,20 +5,19 @@
 
 from ..events import event_import_setup_created, event_import_setup_edited
 from ..models import ImportSetup
 from ..permissions import (
     permission_import_setup_create, permission_import_setup_delete,
     permission_import_setup_edit, permission_import_setup_view
 )
-from .mixins import ImportSetupAPIViewTestMixin, ImportSetupTestMixin
+from .mixins.import_setup_mixins import ImportSetupAPIViewTestMixin
 
 
 class ImportSetupAPIViewTestCase(
-    DocumentTestMixin, ImportSetupAPIViewTestMixin, ImportSetupTestMixin,
-    BaseAPITestCase
+    DocumentTestMixin, ImportSetupAPIViewTestMixin, BaseAPITestCase
 ):
     auto_upload_test_document = False
 
     def test_import_setup_create_api_view_no_permission(self):
         import_setup_count = ImportSetup.objects.count()
 
         self._clear_events()
@@ -45,16 +44,16 @@
             ImportSetup.objects.count(), import_setup_count + 1
         )
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 1)
 
         self.assertEqual(events[0].action_object, None)
-        self.assertEqual(events[0].actor, self.test_import_setup)
-        self.assertEqual(events[0].target, self.test_import_setup)
+        self.assertEqual(events[0].actor, self._test_import_setup)
+        self.assertEqual(events[0].target, self._test_import_setup)
         self.assertEqual(events[0].verb, event_import_setup_created.id)
 
     def test_import_setup_delete_api_view_no_permission(self):
         self._create_test_import_setup()
 
         import_setup_count = ImportSetup.objects.count()
 
@@ -72,15 +71,15 @@
 
     def test_import_setup_delete_api_view_with_access(self):
         self._create_test_import_setup()
 
         import_setup_count = ImportSetup.objects.count()
 
         self.grant_access(
-            obj=self.test_import_setup,
+            obj=self._test_import_setup,
             permission=permission_import_setup_delete
         )
 
         self._clear_events()
 
         response = self._request_test_import_setup_delete_api_view()
         self.assertEqual(response.status_code, status.HTTP_204_NO_CONTENT)
@@ -104,119 +103,119 @@
         events = self._get_test_events()
         self.assertEqual(events.count(), 0)
 
     def test_import_setup_detail_api_view_with_access(self):
         self._create_test_import_setup()
 
         self.grant_access(
-            obj=self.test_import_setup,
+            obj=self._test_import_setup,
             permission=permission_import_setup_view
         )
 
         self._clear_events()
 
         response = self._request_test_import_setup_detail_api_view()
         self.assertEqual(response.status_code, status.HTTP_200_OK)
         self.assertEqual(
-            response.data['id'], self.test_import_setup.pk
+            response.data['id'], self._test_import_setup.pk
         )
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 0)
 
     def test_import_setup_edit_via_patch_api_view_no_permssion(self):
         self._create_test_import_setup()
 
-        import_setup_label = self.test_import_setup.label
+        import_setup_label = self._test_import_setup.label
 
         self._clear_events()
 
         response = self._request_test_import_setup_edit_via_patch_api_view()
         self.assertEqual(response.status_code, status.HTTP_404_NOT_FOUND)
 
-        self.test_import_setup.refresh_from_db()
+        self._test_import_setup.refresh_from_db()
         self.assertEqual(
-            self.test_import_setup.label, import_setup_label
+            self._test_import_setup.label, import_setup_label
         )
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 0)
 
     def test_import_setup_edit_via_patch_api_view_with_access(self):
         self._create_test_import_setup()
 
-        import_setup_label = self.test_import_setup.label
+        import_setup_label = self._test_import_setup.label
 
         self.grant_access(
-            obj=self.test_import_setup,
+            obj=self._test_import_setup,
             permission=permission_import_setup_edit
         )
 
         self._clear_events()
 
         response = self._request_test_import_setup_edit_via_patch_api_view()
         self.assertEqual(response.status_code, status.HTTP_200_OK)
 
-        self.test_import_setup.refresh_from_db()
+        self._test_import_setup.refresh_from_db()
         self.assertNotEqual(
-            self.test_import_setup.label, import_setup_label
+            self._test_import_setup.label, import_setup_label
         )
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 1)
 
         self.assertEqual(events[0].action_object, None)
-        self.assertEqual(events[0].actor, self.test_import_setup)
-        self.assertEqual(events[0].target, self.test_import_setup)
+        self.assertEqual(events[0].actor, self._test_import_setup)
+        self.assertEqual(events[0].target, self._test_import_setup)
         self.assertEqual(events[0].verb, event_import_setup_edited.id)
 
     def test_import_setup_edit_via_put_api_view_no_permission(self):
         self._create_test_import_setup()
 
-        import_setup_label = self.test_import_setup.label
+        import_setup_label = self._test_import_setup.label
 
         self._clear_events()
 
         response = self._request_test_import_setup_edit_via_put_api_view()
         self.assertEqual(response.status_code, status.HTTP_404_NOT_FOUND)
 
-        self.test_import_setup.refresh_from_db()
+        self._test_import_setup.refresh_from_db()
         self.assertEqual(
-            self.test_import_setup.label, import_setup_label
+            self._test_import_setup.label, import_setup_label
         )
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 0)
 
     def test_import_setup_edit_via_put_api_view_with_access(self):
         self._create_test_import_setup()
 
-        import_setup_label = self.test_import_setup.label
+        import_setup_label = self._test_import_setup.label
 
         self.grant_access(
-            obj=self.test_import_setup,
+            obj=self._test_import_setup,
             permission=permission_import_setup_edit
         )
 
         self._clear_events()
 
         response = self._request_test_import_setup_edit_via_put_api_view()
         self.assertEqual(response.status_code, status.HTTP_200_OK)
 
-        self.test_import_setup.refresh_from_db()
+        self._test_import_setup.refresh_from_db()
         self.assertNotEqual(
-            self.test_import_setup.label, import_setup_label
+            self._test_import_setup.label, import_setup_label
         )
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 1)
 
         self.assertEqual(events[0].action_object, None)
-        self.assertEqual(events[0].actor, self.test_import_setup)
-        self.assertEqual(events[0].target, self.test_import_setup)
+        self.assertEqual(events[0].actor, self._test_import_setup)
+        self.assertEqual(events[0].target, self._test_import_setup)
         self.assertEqual(events[0].verb, event_import_setup_edited.id)
 
     def test_import_setup_list_api_view_no_permission(self):
         self._create_test_import_setup()
 
         self._clear_events()
 
@@ -227,21 +226,21 @@
         events = self._get_test_events()
         self.assertEqual(events.count(), 0)
 
     def test_import_setup_list_api_view_with_access(self):
         self._create_test_import_setup()
 
         self.grant_access(
-            obj=self.test_import_setup,
+            obj=self._test_import_setup,
             permission=permission_import_setup_view
         )
 
         self._clear_events()
 
         response = self._request_test_import_setup_list_api_view()
         self.assertEqual(response.status_code, status.HTTP_200_OK)
         self.assertEqual(
-            response.data['results'][0]['id'], self.test_import_setup.pk
+            response.data['results'][0]['id'], self._test_import_setup.pk
         )
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 0)
```

### Comparing `mayan-importer-3.1/importer/tests/test_import_setup_item_api.py` & `mayan-importer-3.1.1/importer/tests/test_import_setup_item_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,79 +1,73 @@
 from rest_framework import status
 
-from mayan.apps.credentials.tests.mixins import StoredCredentialTestMixin
 from mayan.apps.documents.tests.mixins.document_mixins import DocumentTestMixin
 from mayan.apps.rest_api.tests.base import BaseAPITestCase
 
 from ..events import (
     event_import_setup_item_edited, event_import_setup_item_deleted
 )
 from ..permissions import (
     permission_import_setup_edit, permission_import_setup_view
 )
-from .mixins import (
-    ImportSetupItemAPIViewTestMixin, ImportSetupItemTestMixin,
-    ImportSetupTestMixin
-)
+from .mixins.import_setup_item_mixins import ImportSetupItemAPIViewTestMixin
 
 
 class ImportSetupItemAPIViewTestCase(
-    DocumentTestMixin, ImportSetupItemTestMixin,
-    ImportSetupItemAPIViewTestMixin,
-    ImportSetupTestMixin, StoredCredentialTestMixin, BaseAPITestCase
+    DocumentTestMixin, ImportSetupItemAPIViewTestMixin, BaseAPITestCase
 ):
     auto_upload_test_document = False
 
     def setUp(self):
         super().setUp()
         self._create_test_stored_credential()
         self._create_test_import_setup()
 
     def test_import_setup_item_delete_api_view_no_permission(self):
         self._create_test_import_setup_item()
 
-        import_setup_item_count = self.test_import_setup.items.count()
+        import_setup_item_count = self._test_import_setup.items.count()
 
         self._clear_events()
 
         response = self._request_test_import_setup_item_delete_api_view()
         self.assertEqual(response.status_code, status.HTTP_404_NOT_FOUND)
 
         self.assertEqual(
-            self.test_import_setup.items.count(), import_setup_item_count
+            self._test_import_setup.items.count(), import_setup_item_count
         )
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 0)
 
     def test_import_setup_item_delete_api_view_with_access(self):
         self._create_test_import_setup_item()
 
-        import_setup_item_count = self.test_import_setup.items.count()
+        import_setup_item_count = self._test_import_setup.items.count()
 
         self.grant_access(
-            obj=self.test_import_setup,
+            obj=self._test_import_setup,
             permission=permission_import_setup_edit
         )
 
         self._clear_events()
 
         response = self._request_test_import_setup_item_delete_api_view()
         self.assertEqual(response.status_code, status.HTTP_204_NO_CONTENT)
 
         self.assertEqual(
-            self.test_import_setup.items.count(), import_setup_item_count - 1
+            self._test_import_setup.items.count(), import_setup_item_count - 1
         )
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 1)
 
         self.assertEqual(events[0].action_object, None)
-        self.assertEqual(events[0].actor, self.test_import_setup)
-        self.assertEqual(events[0].target, self.test_import_setup)
+        self.assertEqual(events[0].actor, self._test_import_setup)
+        self.assertEqual(events[0].target, self._test_import_setup)
         self.assertEqual(events[0].verb, event_import_setup_item_deleted.id)
 
     def test_import_setup_item_detail_api_view_no_permission(self):
         self._create_test_import_setup_item()
 
         self._clear_events()
 
@@ -84,119 +78,119 @@
         events = self._get_test_events()
         self.assertEqual(events.count(), 0)
 
     def test_import_setup_item_detail_api_view_with_access(self):
         self._create_test_import_setup_item()
 
         self.grant_access(
-            obj=self.test_import_setup,
+            obj=self._test_import_setup,
             permission=permission_import_setup_view
         )
 
         self._clear_events()
 
         response = self._request_test_import_setup_item_detail_api_view()
         self.assertEqual(response.status_code, status.HTTP_200_OK)
         self.assertEqual(
-            response.data['id'], self.test_import_setup_item.pk
+            response.data['id'], self._test_import_setup_item.pk
         )
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 0)
 
     def test_import_setup_item_edit_via_patch_api_view_no_permssion(self):
         self._create_test_import_setup_item()
 
-        import_setup_item_label = self.test_import_setup_item.identifier
+        import_setup_item_label = self._test_import_setup_item.identifier
 
         self._clear_events()
 
         response = self._request_test_import_setup_item_edit_via_patch_api_view()
         self.assertEqual(response.status_code, status.HTTP_404_NOT_FOUND)
 
-        self.test_import_setup_item.refresh_from_db()
+        self._test_import_setup_item.refresh_from_db()
         self.assertEqual(
-            self.test_import_setup_item.identifier, import_setup_item_label
+            self._test_import_setup_item.identifier, import_setup_item_label
         )
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 0)
 
     def test_import_setup_item_edit_via_patch_api_view_with_access(self):
         self._create_test_import_setup_item()
 
-        import_setup_item_label = self.test_import_setup_item.identifier
+        import_setup_item_label = self._test_import_setup_item.identifier
 
         self.grant_access(
-            obj=self.test_import_setup,
+            obj=self._test_import_setup,
             permission=permission_import_setup_edit
         )
 
         self._clear_events()
 
         response = self._request_test_import_setup_item_edit_via_patch_api_view()
         self.assertEqual(response.status_code, status.HTTP_200_OK)
 
-        self.test_import_setup_item.refresh_from_db()
+        self._test_import_setup_item.refresh_from_db()
         self.assertNotEqual(
-            self.test_import_setup_item.identifier, import_setup_item_label
+            self._test_import_setup_item.identifier, import_setup_item_label
         )
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 1)
 
-        self.assertEqual(events[0].action_object, self.test_import_setup)
-        self.assertEqual(events[0].actor, self.test_import_setup_item)
-        self.assertEqual(events[0].target, self.test_import_setup_item)
+        self.assertEqual(events[0].action_object, self._test_import_setup)
+        self.assertEqual(events[0].actor, self._test_import_setup_item)
+        self.assertEqual(events[0].target, self._test_import_setup_item)
         self.assertEqual(events[0].verb, event_import_setup_item_edited.id)
 
     def test_import_setup_item_edit_via_put_api_view_no_permission(self):
         self._create_test_import_setup_item()
 
-        import_setup_item_label = self.test_import_setup_item.identifier
+        import_setup_item_label = self._test_import_setup_item.identifier
 
         self._clear_events()
 
         response = self._request_test_import_setup_item_edit_via_put_api_view()
         self.assertEqual(response.status_code, status.HTTP_404_NOT_FOUND)
 
-        self.test_import_setup_item.refresh_from_db()
+        self._test_import_setup_item.refresh_from_db()
         self.assertEqual(
-            self.test_import_setup_item.identifier, import_setup_item_label
+            self._test_import_setup_item.identifier, import_setup_item_label
         )
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 0)
 
     def test_import_setup_item_edit_via_put_api_view_with_access(self):
         self._create_test_import_setup_item()
 
-        import_setup_item_label = self.test_import_setup_item.identifier
+        import_setup_item_label = self._test_import_setup_item.identifier
 
         self.grant_access(
-            obj=self.test_import_setup,
+            obj=self._test_import_setup,
             permission=permission_import_setup_edit
         )
 
         self._clear_events()
 
         response = self._request_test_import_setup_item_edit_via_put_api_view()
         self.assertEqual(response.status_code, status.HTTP_200_OK)
 
-        self.test_import_setup_item.refresh_from_db()
+        self._test_import_setup_item.refresh_from_db()
         self.assertNotEqual(
-            self.test_import_setup_item.identifier, import_setup_item_label
+            self._test_import_setup_item.identifier, import_setup_item_label
         )
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 1)
 
-        self.assertEqual(events[0].action_object, self.test_import_setup)
-        self.assertEqual(events[0].actor, self.test_import_setup_item)
-        self.assertEqual(events[0].target, self.test_import_setup_item)
+        self.assertEqual(events[0].action_object, self._test_import_setup)
+        self.assertEqual(events[0].actor, self._test_import_setup_item)
+        self.assertEqual(events[0].target, self._test_import_setup_item)
         self.assertEqual(events[0].verb, event_import_setup_item_edited.id)
 
     def test_import_setup_item_list_api_view_no_permission(self):
         self._create_test_import_setup_item()
 
         self._clear_events()
 
@@ -207,21 +201,21 @@
         events = self._get_test_events()
         self.assertEqual(events.count(), 0)
 
     def test_import_setup_item_list_api_view_with_access(self):
         self._create_test_import_setup_item()
 
         self.grant_access(
-            obj=self.test_import_setup,
+            obj=self._test_import_setup,
             permission=permission_import_setup_view
         )
 
         self._clear_events()
 
         response = self._request_test_import_setup_item_list_api_view()
         self.assertEqual(response.status_code, status.HTTP_200_OK)
         self.assertEqual(
-            response.data['results'][0]['id'], self.test_import_setup_item.pk
+            response.data['results'][0]['id'], self._test_import_setup_item.pk
         )
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 0)
```

### Comparing `mayan-importer-3.1/importer/tests/test_import_setup_item_views.py` & `mayan-importer-3.1.1/importer/tests/test_import_setup_item_views.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from mayan.apps.credentials.tests.mixins import StoredCredentialTestMixin
 from mayan.apps.documents.events import (
     event_document_created, event_document_file_created,
     event_document_file_edited, event_document_version_created,
     event_document_version_page_created
 )
 from mayan.apps.documents.models.document_models import Document
 from mayan.apps.documents.tests.base import GenericDocumentViewTestCase
@@ -13,226 +12,221 @@
     event_import_setup_populate_finished, event_import_setup_populate_started,
     event_import_setup_process_finished, event_import_setup_process_started
 )
 from ..permissions import (
     permission_import_setup_edit, permission_import_setup_process
 )
 
-from .mixins import (
-    ImportSetupTestMixin, ImportSetupItemTestMixin,
-    ImportSetupItemViewTestMixin
-)
+from .mixins.import_setup_item_mixins import ImportSetupItemViewTestMixin
 
 
 class ImportSetupItemViewTestCase(
-    StoredCredentialTestMixin, ImportSetupTestMixin,
-    ImportSetupItemTestMixin, ImportSetupItemViewTestMixin,
-    GenericDocumentViewTestCase
+    ImportSetupItemViewTestMixin, GenericDocumentViewTestCase
 ):
     auto_upload_test_document = False
 
     def setUp(self):
         super().setUp()
         self._create_test_stored_credential()
         self._create_test_import_setup()
 
     def test_import_setup_clear_view_no_permission(self):
         self._create_test_import_setup_item()
 
-        import_setup_item_count = self.test_import_setup.items.count()
+        import_setup_item_count = self._test_import_setup.items.count()
 
         self._clear_events()
 
         response = self._request_test_import_setup_clear_view()
         self.assertEqual(response.status_code, 404)
 
         self.assertEqual(
-            self.test_import_setup.items.count(), import_setup_item_count
+            self._test_import_setup.items.count(), import_setup_item_count
         )
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 0)
 
     def test_import_setup_clear_view_with_access(self):
         self._create_test_import_setup_item()
 
         self.grant_access(
-            obj=self.test_import_setup,
+            obj=self._test_import_setup,
             permission=permission_import_setup_process
         )
 
-        import_setup_item_count = self.test_import_setup.items.count()
+        import_setup_item_count = self._test_import_setup.items.count()
 
         self._clear_events()
 
         response = self._request_test_import_setup_clear_view()
         self.assertEqual(response.status_code, 302)
 
         self.assertEqual(
-            self.test_import_setup.items.count(), import_setup_item_count - 1
+            self._test_import_setup.items.count(), import_setup_item_count - 1
         )
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 0)
 
     def test_import_setup_item_delete_view_no_permission(self):
         self._create_test_import_setup_item()
 
-        import_setup_item_count = self.test_import_setup.items.count()
+        import_setup_item_count = self._test_import_setup.items.count()
 
         self._clear_events()
 
         response = self._request_test_import_setup_item_delete_view()
         self.assertEqual(response.status_code, 404)
 
         self.assertEqual(
-            self.test_import_setup.items.count(), import_setup_item_count
+            self._test_import_setup.items.count(), import_setup_item_count
         )
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 0)
 
     def test_import_setup_item_delete_view_with_access(self):
         self._create_test_import_setup_item()
 
         self.grant_access(
-            obj=self.test_import_setup,
+            obj=self._test_import_setup,
             permission=permission_import_setup_edit
         )
 
-        import_setup_item_count = self.test_import_setup.items.count()
+        import_setup_item_count = self._test_import_setup.items.count()
 
         self._clear_events()
 
         response = self._request_test_import_setup_item_delete_view()
         self.assertEqual(response.status_code, 302)
 
         self.assertEqual(
-            self.test_import_setup.items.count(), import_setup_item_count - 1
+            self._test_import_setup.items.count(), import_setup_item_count - 1
         )
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 1)
 
         self.assertEqual(events[0].action_object, None)
-        self.assertEqual(events[0].actor, self.test_import_setup)
-        self.assertEqual(events[0].target, self.test_import_setup)
+        self.assertEqual(events[0].actor, self._test_import_setup)
+        self.assertEqual(events[0].target, self._test_import_setup)
         self.assertEqual(
             events[0].verb, event_import_setup_item_deleted.id
         )
 
     def test_import_setup_item_edit_view_no_permission(self):
         self._create_test_import_setup_item()
 
-        import_setup_item_label = self.test_import_setup_item.identifier
+        import_setup_item_label = self._test_import_setup_item.identifier
 
         self._clear_events()
 
         response = self._request_test_import_setup_item_edit_view()
         self.assertEqual(response.status_code, 404)
 
-        self.test_import_setup_item.refresh_from_db()
+        self._test_import_setup_item.refresh_from_db()
         self.assertEqual(
-            self.test_import_setup_item.identifier, import_setup_item_label
+            self._test_import_setup_item.identifier, import_setup_item_label
         )
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 0)
 
     def test_import_setup_item_edit_view_with_access(self):
         self._create_test_import_setup_item()
 
         self.grant_access(
-            obj=self.test_import_setup,
+            obj=self._test_import_setup,
             permission=permission_import_setup_edit
         )
 
-        import_setup_item_label = self.test_import_setup_item.identifier
+        import_setup_item_label = self._test_import_setup_item.identifier
 
         self._clear_events()
 
         response = self._request_test_import_setup_item_edit_view()
         self.assertEqual(response.status_code, 302)
 
-        self.test_import_setup_item.refresh_from_db()
+        self._test_import_setup_item.refresh_from_db()
         self.assertNotEqual(
-            self.test_import_setup_item.identifier, import_setup_item_label
+            self._test_import_setup_item.identifier, import_setup_item_label
         )
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 1)
 
-        self.assertEqual(events[0].action_object, self.test_import_setup)
+        self.assertEqual(events[0].action_object, self._test_import_setup)
         self.assertEqual(events[0].actor, self._test_case_user)
-        self.assertEqual(events[0].target, self.test_import_setup_item)
+        self.assertEqual(events[0].target, self._test_import_setup_item)
         self.assertEqual(
             events[0].verb, event_import_setup_item_edited.id
         )
 
     def test_import_setup_populate_view_no_permission(self):
-        import_setup_item_count = self.test_import_setup.items.count()
+        import_setup_item_count = self._test_import_setup.items.count()
 
         self._clear_events()
 
         response = self._request_test_import_setup_populate_view()
         self.assertEqual(response.status_code, 404)
 
         self.assertEqual(
-            self.test_import_setup.items.count(), import_setup_item_count
+            self._test_import_setup.items.count(), import_setup_item_count
         )
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 0)
 
     def test_import_setup_populate_view_with_access(self):
         self.grant_access(
-            obj=self.test_import_setup,
+            obj=self._test_import_setup,
             permission=permission_import_setup_process
         )
 
-        import_setup_item_count = self.test_import_setup.items.count()
+        import_setup_item_count = self._test_import_setup.items.count()
 
         self._clear_events()
 
         response = self._request_test_import_setup_populate_view()
         self.assertEqual(response.status_code, 302)
 
         self.assertEqual(
-            self.test_import_setup.items.count(), import_setup_item_count + 1
+            self._test_import_setup.items.count(), import_setup_item_count + 1
         )
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 4)
 
-        test_import_setup_item = self.test_import_setup.items.first()
+        test_import_setup_item = self._test_import_setup.items.first()
 
         self.assertEqual(events[0].action_object, None)
-        self.assertEqual(events[0].actor, self.test_import_setup)
-        self.assertEqual(events[0].target, self.test_import_setup)
+        self.assertEqual(events[0].actor, self._test_import_setup)
+        self.assertEqual(events[0].target, self._test_import_setup)
         self.assertEqual(
             events[0].verb, event_import_setup_populate_started.id
         )
 
-        self.assertEqual(events[1].action_object, self.test_import_setup)
+        self.assertEqual(events[1].action_object, self._test_import_setup)
         self.assertEqual(events[1].actor, test_import_setup_item)
         self.assertEqual(events[1].target, test_import_setup_item)
         self.assertEqual(
             events[1].verb, event_import_setup_item_created.id
         )
 
-        self.assertEqual(events[2].action_object, self.test_import_setup)
+        self.assertEqual(events[2].action_object, self._test_import_setup)
         self.assertEqual(events[2].actor, test_import_setup_item)
         self.assertEqual(events[2].target, test_import_setup_item)
         self.assertEqual(
             events[2].verb, event_import_setup_item_edited.id
         )
 
         self.assertEqual(events[3].action_object, None)
-        self.assertEqual(events[3].actor, self.test_import_setup)
-        self.assertEqual(events[3].target, self.test_import_setup)
+        self.assertEqual(events[3].actor, self._test_import_setup)
+        self.assertEqual(events[3].target, self._test_import_setup)
         self.assertEqual(
             events[3].verb, event_import_setup_populate_finished.id
         )
 
     def test_import_setup_process_view_no_permission(self):
         self._create_test_import_setup_item()
 
@@ -250,15 +244,15 @@
         events = self._get_test_events()
         self.assertEqual(events.count(), 0)
 
     def test_import_setup_process_view_with_access(self):
         self._create_test_import_setup_item()
 
         self.grant_access(
-            obj=self.test_import_setup,
+            obj=self._test_import_setup,
             permission=permission_import_setup_process
         )
         document_count = self._test_document_type.documents.count()
 
         self._clear_events()
 
         response = self._request_test_import_setup_process_view()
@@ -273,16 +267,16 @@
 
         test_document = Document.objects.last()
         test_document_file = test_document.file_latest
         test_document_version = test_document.versions.last()
         test_document_version_page = test_document_version.pages.first()
 
         self.assertEqual(events[0].action_object, None)
-        self.assertEqual(events[0].actor, self.test_import_setup)
-        self.assertEqual(events[0].target, self.test_import_setup)
+        self.assertEqual(events[0].actor, self._test_import_setup)
+        self.assertEqual(events[0].target, self._test_import_setup)
         self.assertEqual(
             events[0].verb, event_import_setup_process_started.id
         )
 
         self.assertEqual(events[1].action_object, self._test_document_type)
         self.assertEqual(events[1].actor, test_document)
         self.assertEqual(events[1].target, test_document)
@@ -306,20 +300,20 @@
         self.assertEqual(events[5].action_object, test_document_version)
         self.assertEqual(events[5].actor, test_document_version_page)
         self.assertEqual(events[5].target, test_document_version_page)
         self.assertEqual(
             events[5].verb, event_document_version_page_created.id
         )
 
-        self.assertEqual(events[6].action_object, self.test_import_setup)
-        self.assertEqual(events[6].actor, self.test_import_setup_item)
-        self.assertEqual(events[6].target, self.test_import_setup_item)
+        self.assertEqual(events[6].action_object, self._test_import_setup)
+        self.assertEqual(events[6].actor, self._test_import_setup_item)
+        self.assertEqual(events[6].target, self._test_import_setup_item)
         self.assertEqual(
             events[6].verb, event_import_setup_item_finished.id
         )
 
         self.assertEqual(events[7].action_object, None)
-        self.assertEqual(events[7].actor, self.test_import_setup)
-        self.assertEqual(events[7].target, self.test_import_setup)
+        self.assertEqual(events[7].actor, self._test_import_setup)
+        self.assertEqual(events[7].target, self._test_import_setup)
         self.assertEqual(
             events[7].verb, event_import_setup_process_finished.id
         )
```

### Comparing `mayan-importer-3.1/importer/tests/test_import_setup_views.py` & `mayan-importer-3.1.1/importer/tests/test_import_setup_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-from mayan.apps.credentials.tests.mixins import StoredCredentialTestMixin
 from mayan.apps.documents.tests.base import GenericDocumentViewTestCase
 
 from ..events import event_import_setup_created, event_import_setup_edited
 from ..models import ImportSetup
 from ..permissions import (
     permission_import_setup_create, permission_import_setup_delete,
     permission_import_setup_edit, permission_import_setup_view
 )
 
-from .mixins import ImportSetupTestMixin, ImportSetupViewTestMixin
+from .mixins.import_setup_mixins import ImportSetupViewTestMixin
 
 
 class ImportSetupViewTestCase(
-    StoredCredentialTestMixin, ImportSetupTestMixin,
     ImportSetupViewTestMixin, GenericDocumentViewTestCase
 ):
     auto_upload_test_document = False
 
     def setUp(self):
         super().setUp()
         self._create_test_stored_credential()
@@ -77,15 +75,15 @@
         )
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 1)
 
         self.assertEqual(events[0].action_object, None)
         self.assertEqual(events[0].actor, self._test_case_user)
-        self.assertEqual(events[0].target, self.test_import_setup)
+        self.assertEqual(events[0].target, self._test_import_setup)
         self.assertEqual(events[0].verb, event_import_setup_created.id)
 
     def test_import_setup_delete_view_no_permissions(self):
         self._create_test_import_setup()
 
         import_setup_count = ImportSetup.objects.count()
 
@@ -99,15 +97,15 @@
         events = self._get_test_events()
         self.assertEqual(events.count(), 0)
 
     def test_import_setup_delete_view_with_access(self):
         self._create_test_import_setup()
 
         self.grant_access(
-            obj=self.test_import_setup,
+            obj=self._test_import_setup,
             permission=permission_import_setup_delete
         )
 
         import_setup_count = ImportSetup.objects.count()
 
         self._clear_events()
 
@@ -120,78 +118,78 @@
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 0)
 
     def test_import_setup_edit_view_no_permissions(self):
         self._create_test_import_setup()
 
-        import_setup_label = self.test_import_setup.label
+        import_setup_label = self._test_import_setup.label
 
         self._clear_events()
 
         response = self._request_test_import_setup_edit_view()
         self.assertEqual(response.status_code, 404)
 
-        self.test_import_setup.refresh_from_db()
-        self.assertEqual(self.test_import_setup.label, import_setup_label)
+        self._test_import_setup.refresh_from_db()
+        self.assertEqual(self._test_import_setup.label, import_setup_label)
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 0)
 
     def test_import_setup_edit_view_with_access(self):
         self._create_test_import_setup()
 
         self.grant_access(
-            obj=self.test_import_setup,
+            obj=self._test_import_setup,
             permission=permission_import_setup_edit
         )
 
-        import_setup_label = self.test_import_setup.label
+        import_setup_label = self._test_import_setup.label
 
         self._clear_events()
 
         response = self._request_test_import_setup_edit_view()
         self.assertEqual(response.status_code, 302)
 
-        self.test_import_setup.refresh_from_db()
-        self.assertNotEqual(self.test_import_setup.label, import_setup_label)
+        self._test_import_setup.refresh_from_db()
+        self.assertNotEqual(self._test_import_setup.label, import_setup_label)
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 1)
 
         self.assertEqual(events[0].action_object, None)
         self.assertEqual(events[0].actor, self._test_case_user)
-        self.assertEqual(events[0].target, self.test_import_setup)
+        self.assertEqual(events[0].target, self._test_import_setup)
         self.assertEqual(events[0].verb, event_import_setup_edited.id)
 
     def test_import_setup_list_view_with_no_permission(self):
         self._create_test_import_setup()
 
         self._clear_events()
 
         response = self._request_test_import_setup_list_view()
         self.assertNotContains(
-            response=response, text=self.test_import_setup.label,
+            response=response, text=self._test_import_setup.label,
             status_code=200
         )
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 0)
 
     def test_import_setup_list_view_with_access(self):
         self._create_test_import_setup()
 
         self.grant_access(
-            obj=self.test_import_setup,
+            obj=self._test_import_setup,
             permission=permission_import_setup_view
         )
 
         self._clear_events()
 
         response = self._request_test_import_setup_list_view()
         self.assertContains(
-            response=response, text=self.test_import_setup.label,
+            response=response, text=self._test_import_setup.label,
             status_code=200
         )
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 0)
```

### Comparing `mayan-importer-3.1/importer/urls.py` & `mayan-importer-3.1.1/importer/urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,16 @@
 urlpatterns_import_setup_filer = [
     url(
         regex=r'^import_setups/(?P<import_setup_id>\d+)/load/$',
         name='import_setup_load', view=ImportSetupFilerLoadView.as_view()
     ),
     url(
         regex=r'^import_setups/(?P<import_setup_id>\d+)/save/$',
-        name='import_setup_save', view=ImportSetupFilerSaveConfirmView.as_view()
+        name='import_setup_save',
+        view=ImportSetupFilerSaveConfirmView.as_view()
     )
 ]
 
 
 urlpatterns_import_setup_items = [
     url(
         regex=r'^import_setups/(?P<import_setup_id>\d+)/clear/$',
```

### Comparing `mayan-importer-3.1/importer/views/import_setup_filer_views.py` & `mayan-importer-3.1.1/importer/views/import_setup_filer_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/views/import_setup_item_views.py` & `mayan-importer-3.1.1/importer/views/import_setup_item_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/importer/views/import_setup_views.py` & `mayan-importer-3.1.1/importer/views/import_setup_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.1/mayan_importer.egg-info/PKG-INFO` & `mayan-importer-3.1.1/mayan_importer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mayan-importer
-Version: 3.1
+Version: 3.1.1
 Summary: Mayan EDMS importer
 Home-page: https://gitlab.com/mayan-edms/importer
 Author: Roberto Rosario
 Author-email: roberto.rosario@mayan-edms.com
 License: Apache 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -93,14 +93,18 @@
 - Generate an Access Token with no expiration.
 - Create a credential instance in the Mayan EDMS Importer app and enter the Access Token.
 - Create an Import Setup that will filter the files to fetch from Dropbox.
 - Click the "Populate" button and check that the item count is correct.
 - Click the "Process" button to start the import process.
 
 
+3.1.1 (2024-05-04)
+==================
+- Fix filer load.
+
 3.1 (2024-05-03)
 ================
 - Improve navigation.
 - Improve processing condition logic.
 - Split modules.
 - Move common state code into a mixin.
 - Add fieldsets.
```

### Comparing `mayan-importer-3.1/mayan_importer.egg-info/SOURCES.txt` & `mayan-importer-3.1.1/mayan_importer.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 importer/models/import_setup_item_models.py
 importer/models/import_setup_model_mixins.py
 importer/models/import_setup_models.py
 importer/models/model_mixins.py
 importer/tests/__init__.py
 importer/tests/importers.py
 importer/tests/literals.py
-importer/tests/mixins.py
+importer/tests/test_filer_views.py
 importer/tests/test_import_setup_api.py
 importer/tests/test_import_setup_item_api.py
 importer/tests/test_import_setup_item_views.py
 importer/tests/test_import_setup_views.py
 importer/views/__init__.py
 importer/views/import_setup_filer_views.py
 importer/views/import_setup_item_views.py
```

### Comparing `mayan-importer-3.1/setup.py` & `mayan-importer-3.1.1/setup.py`

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
-    version='3.1',
+    version='3.1.1',
     zip_safe=False,
 )
```

