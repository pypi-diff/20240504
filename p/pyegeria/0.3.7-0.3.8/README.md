# Comparing `tmp/pyegeria-0.3.7.tar.gz` & `tmp/pyegeria-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyegeria-0.3.7.tar", last modified: Fri May  3 12:19:27 2024, max compression
+gzip compressed data, was "pyegeria-0.3.8.tar", last modified: Sat May  4 15:51:17 2024, max compression
```

## Comparing `pyegeria-0.3.7.tar` & `pyegeria-0.3.8.tar`

### file list

```diff
@@ -1,112 +1,114 @@
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-03 12:19:27.748902 pyegeria-0.3.7/
--rw-r--r--   0 dwolfson   (501) staff       (20)    11357 2024-04-10 19:14:09.000000 pyegeria-0.3.7/LICENSE
--rw-r--r--   0 dwolfson   (501) staff       (20)       32 2024-04-12 00:32:44.000000 pyegeria-0.3.7/MANIFEST.in
--rw-r--r--   0 dwolfson   (501) staff       (20)     2389 2024-05-03 12:19:27.748675 pyegeria-0.3.7/PKG-INFO
--rw-r--r--   0 dwolfson   (501) staff       (20)     1458 2024-04-11 02:07:05.000000 pyegeria-0.3.7/README.md
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-03 12:19:27.736212 pyegeria-0.3.7/examples/
--rw-r--r--   0 dwolfson   (501) staff       (20)     6148 2024-04-24 00:37:23.000000 pyegeria-0.3.7/examples/.DS_Store
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-03 12:19:27.737808 pyegeria-0.3.7/examples/Coco_config/
--rw-r--r--   0 dwolfson   (501) staff       (20)      926 2024-04-10 19:14:09.000000 pyegeria-0.3.7/examples/Coco_config/README.md
--rw-r--r--   0 dwolfson   (501) staff       (20)       45 2024-04-12 00:25:29.000000 pyegeria-0.3.7/examples/Coco_config/__init__.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     4070 2024-04-10 19:14:09.000000 pyegeria-0.3.7/examples/Coco_config/config_cocoMDS1.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     3666 2024-04-10 19:14:09.000000 pyegeria-0.3.7/examples/Coco_config/config_cocoMDS2.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     3661 2024-04-10 19:14:09.000000 pyegeria-0.3.7/examples/Coco_config/config_cocoMDS3.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     2950 2024-04-10 19:14:09.000000 pyegeria-0.3.7/examples/Coco_config/config_cocoMDS4.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     3179 2024-04-10 19:14:09.000000 pyegeria-0.3.7/examples/Coco_config/config_cocoMDS5.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     3987 2024-04-10 19:14:09.000000 pyegeria-0.3.7/examples/Coco_config/config_cocoMDS6.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     4195 2024-04-10 19:14:09.000000 pyegeria-0.3.7/examples/Coco_config/config_cocoMDSx.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     5220 2024-04-10 19:14:09.000000 pyegeria-0.3.7/examples/Coco_config/config_cocoView1.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     3557 2024-04-10 19:14:09.000000 pyegeria-0.3.7/examples/Coco_config/config_exchangeDL01.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     2478 2024-04-10 19:14:09.000000 pyegeria-0.3.7/examples/Coco_config/config_governDL01.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     2063 2024-04-10 19:14:09.000000 pyegeria-0.3.7/examples/Coco_config/config_monitorDev01.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     8067 2024-04-10 19:14:09.000000 pyegeria-0.3.7/examples/Coco_config/config_monitorGov01.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     5899 2024-04-12 00:25:29.000000 pyegeria-0.3.7/examples/Coco_config/globals.py
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-03 12:19:27.738325 pyegeria-0.3.7/examples/Doc_Samples/
--rw-r--r--   0 dwolfson   (501) staff       (20)    11865 2024-04-18 16:25:08.000000 pyegeria-0.3.7/examples/Doc_Samples/Create_Collection_Sample.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     5049 2024-04-28 23:10:47.000000 pyegeria-0.3.7/examples/Doc_Samples/Create_Sustainability_Collection_Sample.py
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-03 12:19:27.738662 pyegeria-0.3.7/examples/Jupyter Notebooks/
--rw-r--r--   0 dwolfson   (501) staff       (20)   111673 2024-05-03 12:14:01.000000 pyegeria-0.3.7/examples/Jupyter Notebooks/P-egeria-server-config.ipynb
--rw-r--r--   0 dwolfson   (501) staff       (20)      170 2024-04-29 01:25:02.000000 pyegeria-0.3.7/examples/Jupyter Notebooks/README.md
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-03 12:19:27.740057 pyegeria-0.3.7/examples/Jupyter Notebooks/common/
--rw-r--r--   0 dwolfson   (501) staff       (20)     2914 2024-04-19 21:30:39.000000 pyegeria-0.3.7/examples/Jupyter Notebooks/common/P-environment-check.ipynb
--rw-r--r--   0 dwolfson   (501) staff       (20)      408 2024-03-20 02:16:23.000000 pyegeria-0.3.7/examples/Jupyter Notebooks/common/__init__.py
--rw-r--r--   0 dwolfson   (501) staff       (20)   276801 2024-03-18 16:53:11.000000 pyegeria-0.3.7/examples/Jupyter Notebooks/common/common-functions.ipynb
--rw-r--r--   0 dwolfson   (501) staff       (20)     1449 2024-03-18 16:53:11.000000 pyegeria-0.3.7/examples/Jupyter Notebooks/common/environment-check.ipynb
--rw-r--r--   0 dwolfson   (501) staff       (20)     7842 2024-03-18 16:53:11.000000 pyegeria-0.3.7/examples/Jupyter Notebooks/common/globals.ipynb
--rw-r--r--   0 dwolfson   (501) staff       (20)     5900 2024-04-19 21:30:39.000000 pyegeria-0.3.7/examples/Jupyter Notebooks/common/globals.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     5849 2024-03-18 16:53:11.000000 pyegeria-0.3.7/examples/Jupyter Notebooks/common/orig_globals.py
--rw-r--r--   0 dwolfson   (501) staff       (20)       18 2024-04-12 00:32:44.000000 pyegeria-0.3.7/examples/__init__.py
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-03 12:19:27.740164 pyegeria-0.3.7/examples/__pycache__/
--rw-r--r--   0 dwolfson   (501) staff       (20)      194 2024-04-11 16:37:25.000000 pyegeria-0.3.7/examples/__pycache__/__init__.cpython-312.pyc
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-03 12:19:27.742581 pyegeria-0.3.7/examples/widgets/
--rw-r--r--   0 dwolfson   (501) staff       (20)     6148 2024-04-24 00:47:25.000000 pyegeria-0.3.7/examples/widgets/.DS_Store
--rw-r--r--   0 dwolfson   (501) staff       (20)     1696 2024-04-29 00:22:17.000000 pyegeria-0.3.7/examples/widgets/README.md
--rw-r--r--   0 dwolfson   (501) staff       (20)       17 2024-04-12 00:25:29.000000 pyegeria-0.3.7/examples/widgets/__init__.py
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-03 12:19:27.742817 pyegeria-0.3.7/examples/widgets/__pycache__/
--rw-r--r--   0 dwolfson   (501) staff       (20)      201 2024-04-11 16:37:25.000000 pyegeria-0.3.7/examples/widgets/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0 dwolfson   (501) staff       (20)     5743 2024-04-11 16:45:53.000000 pyegeria-0.3.7/examples/widgets/__pycache__/server_status_widget.cpython-312-pytest-7.4.4.pyc
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     3157 2024-04-29 00:14:47.000000 pyegeria-0.3.7/examples/widgets/coco_status.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     3642 2024-04-18 19:49:26.000000 pyegeria-0.3.7/examples/widgets/collection_viewer.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     5234 2024-05-02 12:50:29.000000 pyegeria-0.3.7/examples/widgets/engine_action_status.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     5185 2024-04-12 00:32:44.000000 pyegeria-0.3.7/examples/widgets/find_todos.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     4947 2024-04-25 14:18:41.000000 pyegeria-0.3.7/examples/widgets/get_relationship_types.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     6857 2024-05-01 12:33:39.000000 pyegeria-0.3.7/examples/widgets/get_tech_details.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     3938 2024-04-30 15:13:17.000000 pyegeria-0.3.7/examples/widgets/get_tech_types.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     5299 2024-04-24 01:14:00.000000 pyegeria-0.3.7/examples/widgets/get_valid_metadata_values.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     4608 2024-04-12 00:32:44.000000 pyegeria-0.3.7/examples/widgets/glossary_view.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     4014 2024-04-12 00:32:44.000000 pyegeria-0.3.7/examples/widgets/gov_engine_status.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     4589 2024-04-12 00:32:44.000000 pyegeria-0.3.7/examples/widgets/integration_daemon_status.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     3499 2024-04-29 06:38:46.000000 pyegeria-0.3.7/examples/widgets/list_asset_types.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     3704 2024-04-18 13:42:39.000000 pyegeria-0.3.7/examples/widgets/multi-server_status.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     5674 2024-04-12 00:32:44.000000 pyegeria-0.3.7/examples/widgets/my_todos.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     4663 2024-04-12 00:32:44.000000 pyegeria-0.3.7/examples/widgets/open_todos.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     5448 2024-04-24 21:32:52.000000 pyegeria-0.3.7/examples/widgets/project_list_viewer.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     3360 2024-04-12 00:32:44.000000 pyegeria-0.3.7/examples/widgets/server_status.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     3102 2024-04-12 00:32:44.000000 pyegeria-0.3.7/examples/widgets/server_status_widget.py
--rwxr-xr-x   0 dwolfson   (501) staff       (20)     4619 2024-04-26 14:50:59.000000 pyegeria-0.3.7/examples/widgets/view_my_profile.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     1063 2024-05-03 12:18:36.000000 pyegeria-0.3.7/pyproject.toml
--rw-r--r--   0 dwolfson   (501) staff       (20)       38 2024-05-03 12:19:27.748947 pyegeria-0.3.7/setup.cfg
--rw-r--r--   0 dwolfson   (501) staff       (20)     2423 2024-05-03 12:19:24.000000 pyegeria-0.3.7/setup.py
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-03 12:19:27.735298 pyegeria-0.3.7/src/
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-03 12:19:27.745488 pyegeria-0.3.7/src/pyegeria/
--rw-r--r--   0 dwolfson   (501) staff       (20)     1769 2024-04-23 16:53:51.000000 pyegeria-0.3.7/src/pyegeria/__init__.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    23606 2024-04-11 02:07:05.000000 pyegeria-0.3.7/src/pyegeria/_client.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    18399 2024-04-11 02:07:05.000000 pyegeria-0.3.7/src/pyegeria/_exceptions.py
--rw-r--r--   0 dwolfson   (501) staff       (20)      558 2024-04-10 19:14:09.000000 pyegeria-0.3.7/src/pyegeria/_globals.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    12703 2024-04-11 02:07:05.000000 pyegeria-0.3.7/src/pyegeria/_validators.py
--rw-r--r--   0 dwolfson   (501) staff       (20)   102487 2024-05-02 16:23:06.000000 pyegeria-0.3.7/src/pyegeria/automated_curation_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)   114200 2024-04-29 01:32:02.000000 pyegeria-0.3.7/src/pyegeria/collection_manager_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    93244 2024-05-03 11:21:16.000000 pyegeria-0.3.7/src/pyegeria/core_omag_server_config.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    46146 2024-04-11 02:07:05.000000 pyegeria-0.3.7/src/pyegeria/full_omag_server_config.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    36500 2024-04-12 00:32:44.000000 pyegeria-0.3.7/src/pyegeria/glossary_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    19697 2024-04-12 00:32:44.000000 pyegeria-0.3.7/src/pyegeria/gov_engine.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     6340 2024-04-12 00:32:44.000000 pyegeria-0.3.7/src/pyegeria/governance_author.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    42441 2024-04-12 00:32:44.000000 pyegeria-0.3.7/src/pyegeria/my_profile_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    41955 2024-04-12 00:32:44.000000 pyegeria-0.3.7/src/pyegeria/platform_services.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    77305 2024-04-26 16:10:23.000000 pyegeria-0.3.7/src/pyegeria/project_manager_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     8775 2024-04-12 00:32:44.000000 pyegeria-0.3.7/src/pyegeria/registered_info.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    16323 2024-04-12 00:32:44.000000 pyegeria-0.3.7/src/pyegeria/server_operations.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     5240 2024-04-11 02:07:05.000000 pyegeria-0.3.7/src/pyegeria/utils.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    29710 2024-04-25 15:33:15.000000 pyegeria-0.3.7/src/pyegeria/valid_metadata_omvs.py
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-03 12:19:27.748314 pyegeria-0.3.7/src/pyegeria.egg-info/
--rw-r--r--   0 dwolfson   (501) staff       (20)     2389 2024-05-03 12:19:27.000000 pyegeria-0.3.7/src/pyegeria.egg-info/PKG-INFO
--rw-r--r--   0 dwolfson   (501) staff       (20)     3479 2024-05-03 12:19:27.000000 pyegeria-0.3.7/src/pyegeria.egg-info/SOURCES.txt
--rw-r--r--   0 dwolfson   (501) staff       (20)        1 2024-05-03 12:19:27.000000 pyegeria-0.3.7/src/pyegeria.egg-info/dependency_links.txt
--rw-r--r--   0 dwolfson   (501) staff       (20)      140 2024-05-03 12:19:27.000000 pyegeria-0.3.7/src/pyegeria.egg-info/requires.txt
--rw-r--r--   0 dwolfson   (501) staff       (20)        9 2024-05-03 12:19:27.000000 pyegeria-0.3.7/src/pyegeria.egg-info/top_level.txt
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-03 12:19:27.748130 pyegeria-0.3.7/tests/
--rw-r--r--   0 dwolfson   (501) staff       (20)    41409 2024-05-03 11:25:36.000000 pyegeria-0.3.7/tests/test_automated_curation_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     3006 2024-04-11 02:07:05.000000 pyegeria-0.3.7/tests/test_client.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    51872 2024-04-29 00:11:27.000000 pyegeria-0.3.7/tests/test_collection_manager_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    59269 2024-05-02 18:01:47.000000 pyegeria-0.3.7/tests/test_core_omag_server_config.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    11868 2024-04-10 19:14:09.000000 pyegeria-0.3.7/tests/test_full_omag_server_config.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    10582 2024-04-11 02:07:05.000000 pyegeria-0.3.7/tests/test_glossary_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     8350 2024-04-11 02:07:05.000000 pyegeria-0.3.7/tests/test_gov_engine.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     9625 2024-04-12 00:32:44.000000 pyegeria-0.3.7/tests/test_my_profile_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    40084 2024-04-23 14:27:57.000000 pyegeria-0.3.7/tests/test_platform_services.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    28529 2024-04-26 16:12:52.000000 pyegeria-0.3.7/tests/test_project_manager_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     4712 2024-04-29 06:35:51.000000 pyegeria-0.3.7/tests/test_registered_info.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     8108 2024-05-02 13:34:44.000000 pyegeria-0.3.7/tests/test_server_operations.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     5904 2024-04-11 02:07:05.000000 pyegeria-0.3.7/tests/test_util_exp.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    12782 2024-05-03 11:30:59.000000 pyegeria-0.3.7/tests/test_valid_metadata_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     6035 2024-04-11 02:07:05.000000 pyegeria-0.3.7/tests/test_validators.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-04 15:51:17.640114 pyegeria-0.3.8/
+-rw-r--r--   0 dwolfson   (501) staff       (20)    11357 2024-04-10 19:14:09.000000 pyegeria-0.3.8/LICENSE
+-rw-r--r--   0 dwolfson   (501) staff       (20)       32 2024-04-12 00:32:44.000000 pyegeria-0.3.8/MANIFEST.in
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2389 2024-05-04 15:51:17.639880 pyegeria-0.3.8/PKG-INFO
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1458 2024-04-11 02:07:05.000000 pyegeria-0.3.8/README.md
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-04 15:51:17.612598 pyegeria-0.3.8/examples/
+-rw-r--r--   0 dwolfson   (501) staff       (20)     6148 2024-04-24 00:37:23.000000 pyegeria-0.3.8/examples/.DS_Store
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-04 15:51:17.615754 pyegeria-0.3.8/examples/Coco_config/
+-rw-r--r--   0 dwolfson   (501) staff       (20)      926 2024-04-10 19:14:09.000000 pyegeria-0.3.8/examples/Coco_config/README.md
+-rw-r--r--   0 dwolfson   (501) staff       (20)       45 2024-04-12 00:25:29.000000 pyegeria-0.3.8/examples/Coco_config/__init__.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     4070 2024-04-10 19:14:09.000000 pyegeria-0.3.8/examples/Coco_config/config_cocoMDS1.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3666 2024-04-10 19:14:09.000000 pyegeria-0.3.8/examples/Coco_config/config_cocoMDS2.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3661 2024-04-10 19:14:09.000000 pyegeria-0.3.8/examples/Coco_config/config_cocoMDS3.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2950 2024-04-10 19:14:09.000000 pyegeria-0.3.8/examples/Coco_config/config_cocoMDS4.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3179 2024-04-10 19:14:09.000000 pyegeria-0.3.8/examples/Coco_config/config_cocoMDS5.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3987 2024-04-10 19:14:09.000000 pyegeria-0.3.8/examples/Coco_config/config_cocoMDS6.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     4195 2024-04-10 19:14:09.000000 pyegeria-0.3.8/examples/Coco_config/config_cocoMDSx.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5220 2024-04-10 19:14:09.000000 pyegeria-0.3.8/examples/Coco_config/config_cocoView1.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3557 2024-04-10 19:14:09.000000 pyegeria-0.3.8/examples/Coco_config/config_exchangeDL01.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2478 2024-04-10 19:14:09.000000 pyegeria-0.3.8/examples/Coco_config/config_governDL01.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2063 2024-04-10 19:14:09.000000 pyegeria-0.3.8/examples/Coco_config/config_monitorDev01.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     8067 2024-04-10 19:14:09.000000 pyegeria-0.3.8/examples/Coco_config/config_monitorGov01.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5899 2024-04-12 00:25:29.000000 pyegeria-0.3.8/examples/Coco_config/globals.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-04 15:51:17.616208 pyegeria-0.3.8/examples/Doc_Samples/
+-rw-r--r--   0 dwolfson   (501) staff       (20)    11865 2024-04-18 16:25:08.000000 pyegeria-0.3.8/examples/Doc_Samples/Create_Collection_Sample.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5049 2024-04-28 23:10:47.000000 pyegeria-0.3.8/examples/Doc_Samples/Create_Sustainability_Collection_Sample.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-04 15:51:17.617234 pyegeria-0.3.8/examples/Jupyter Notebooks/
+-rw-r--r--   0 dwolfson   (501) staff       (20)   111673 2024-05-04 10:56:38.000000 pyegeria-0.3.8/examples/Jupyter Notebooks/P-egeria-server-config.ipynb
+-rw-r--r--   0 dwolfson   (501) staff       (20)      170 2024-04-29 01:25:02.000000 pyegeria-0.3.8/examples/Jupyter Notebooks/README.md
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-04 15:51:17.619383 pyegeria-0.3.8/examples/Jupyter Notebooks/common/
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2942 2024-05-04 07:55:47.000000 pyegeria-0.3.8/examples/Jupyter Notebooks/common/P-environment-check.ipynb
+-rw-r--r--   0 dwolfson   (501) staff       (20)      408 2024-03-20 02:16:23.000000 pyegeria-0.3.8/examples/Jupyter Notebooks/common/__init__.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)   276801 2024-05-04 10:50:51.000000 pyegeria-0.3.8/examples/Jupyter Notebooks/common/common-functions.ipynb
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1449 2024-03-18 16:53:11.000000 pyegeria-0.3.8/examples/Jupyter Notebooks/common/environment-check.ipynb
+-rw-r--r--   0 dwolfson   (501) staff       (20)     7842 2024-03-18 16:53:11.000000 pyegeria-0.3.8/examples/Jupyter Notebooks/common/globals.ipynb
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5900 2024-04-19 21:30:39.000000 pyegeria-0.3.8/examples/Jupyter Notebooks/common/globals.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5849 2024-03-18 16:53:11.000000 pyegeria-0.3.8/examples/Jupyter Notebooks/common/orig_globals.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)       18 2024-04-12 00:32:44.000000 pyegeria-0.3.8/examples/__init__.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-04 15:51:17.619588 pyegeria-0.3.8/examples/__pycache__/
+-rw-r--r--   0 dwolfson   (501) staff       (20)      194 2024-04-11 16:37:25.000000 pyegeria-0.3.8/examples/__pycache__/__init__.cpython-312.pyc
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-04 15:51:17.624836 pyegeria-0.3.8/examples/widgets/
+-rw-r--r--   0 dwolfson   (501) staff       (20)     6148 2024-04-24 00:47:25.000000 pyegeria-0.3.8/examples/widgets/.DS_Store
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1696 2024-04-29 00:22:17.000000 pyegeria-0.3.8/examples/widgets/README.md
+-rw-r--r--   0 dwolfson   (501) staff       (20)       17 2024-04-12 00:25:29.000000 pyegeria-0.3.8/examples/widgets/__init__.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-04 15:51:17.625232 pyegeria-0.3.8/examples/widgets/__pycache__/
+-rw-r--r--   0 dwolfson   (501) staff       (20)      201 2024-04-11 16:37:25.000000 pyegeria-0.3.8/examples/widgets/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5743 2024-04-11 16:45:53.000000 pyegeria-0.3.8/examples/widgets/__pycache__/server_status_widget.cpython-312-pytest-7.4.4.pyc
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     3157 2024-04-29 00:14:47.000000 pyegeria-0.3.8/examples/widgets/coco_status.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     3642 2024-04-18 19:49:26.000000 pyegeria-0.3.8/examples/widgets/collection_viewer.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     5373 2024-05-03 13:19:09.000000 pyegeria-0.3.8/examples/widgets/engine_action_status.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     5183 2024-05-04 15:43:10.000000 pyegeria-0.3.8/examples/widgets/find_todos.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     4947 2024-04-25 14:18:41.000000 pyegeria-0.3.8/examples/widgets/get_relationship_types.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     6857 2024-05-01 12:33:39.000000 pyegeria-0.3.8/examples/widgets/get_tech_details.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     3938 2024-04-30 15:13:17.000000 pyegeria-0.3.8/examples/widgets/get_tech_types.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     5299 2024-04-24 01:14:00.000000 pyegeria-0.3.8/examples/widgets/get_valid_metadata_values.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     4608 2024-04-12 00:32:44.000000 pyegeria-0.3.8/examples/widgets/glossary_view.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     4014 2024-04-12 00:32:44.000000 pyegeria-0.3.8/examples/widgets/gov_engine_status.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     4589 2024-04-12 00:32:44.000000 pyegeria-0.3.8/examples/widgets/integration_daemon_status.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     3499 2024-04-29 06:38:46.000000 pyegeria-0.3.8/examples/widgets/list_asset_types.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     3704 2024-04-18 13:42:39.000000 pyegeria-0.3.8/examples/widgets/multi-server_status.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     5674 2024-04-12 00:32:44.000000 pyegeria-0.3.8/examples/widgets/my_todos.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     4663 2024-04-12 00:32:44.000000 pyegeria-0.3.8/examples/widgets/open_todos.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     5448 2024-04-24 21:32:52.000000 pyegeria-0.3.8/examples/widgets/project_list_viewer.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     3360 2024-04-12 00:32:44.000000 pyegeria-0.3.8/examples/widgets/server_status.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     3102 2024-04-12 00:32:44.000000 pyegeria-0.3.8/examples/widgets/server_status_widget.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     4619 2024-04-26 14:50:59.000000 pyegeria-0.3.8/examples/widgets/view_my_profile.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1063 2024-05-04 15:49:06.000000 pyegeria-0.3.8/pyproject.toml
+-rw-r--r--   0 dwolfson   (501) staff       (20)       38 2024-05-04 15:51:17.640155 pyegeria-0.3.8/setup.cfg
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2423 2024-05-03 12:19:24.000000 pyegeria-0.3.8/setup.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-04 15:51:17.611244 pyegeria-0.3.8/src/
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-04 15:51:17.632380 pyegeria-0.3.8/src/pyegeria/
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1821 2024-05-04 10:57:02.000000 pyegeria-0.3.8/src/pyegeria/__init__.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    23606 2024-04-11 02:07:05.000000 pyegeria-0.3.8/src/pyegeria/_client.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    18399 2024-04-11 02:07:05.000000 pyegeria-0.3.8/src/pyegeria/_exceptions.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)      558 2024-04-10 19:14:09.000000 pyegeria-0.3.8/src/pyegeria/_globals.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    12703 2024-04-11 02:07:05.000000 pyegeria-0.3.8/src/pyegeria/_validators.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)   102487 2024-05-02 16:23:06.000000 pyegeria-0.3.8/src/pyegeria/automated_curation_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)   114200 2024-04-29 01:32:02.000000 pyegeria-0.3.8/src/pyegeria/collection_manager_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    93244 2024-05-03 11:21:16.000000 pyegeria-0.3.8/src/pyegeria/core_omag_server_config.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    46146 2024-04-11 02:07:05.000000 pyegeria-0.3.8/src/pyegeria/full_omag_server_config.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    36500 2024-04-12 00:32:44.000000 pyegeria-0.3.8/src/pyegeria/glossary_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    19697 2024-04-12 00:32:44.000000 pyegeria-0.3.8/src/pyegeria/gov_engine.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     6340 2024-04-12 00:32:44.000000 pyegeria-0.3.8/src/pyegeria/governance_author.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     6226 2024-05-04 11:10:43.000000 pyegeria-0.3.8/src/pyegeria/loaded_resources_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    42489 2024-05-04 15:38:39.000000 pyegeria-0.3.8/src/pyegeria/my_profile_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    41955 2024-04-12 00:32:44.000000 pyegeria-0.3.8/src/pyegeria/platform_services.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    77305 2024-04-26 16:10:23.000000 pyegeria-0.3.8/src/pyegeria/project_manager_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     8793 2024-05-04 07:57:19.000000 pyegeria-0.3.8/src/pyegeria/registered_info.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    16323 2024-04-12 00:32:44.000000 pyegeria-0.3.8/src/pyegeria/server_operations.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5240 2024-04-11 02:07:05.000000 pyegeria-0.3.8/src/pyegeria/utils.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    29710 2024-04-25 15:33:15.000000 pyegeria-0.3.8/src/pyegeria/valid_metadata_omvs.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-04 15:51:17.639540 pyegeria-0.3.8/src/pyegeria.egg-info/
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2389 2024-05-04 15:51:17.000000 pyegeria-0.3.8/src/pyegeria.egg-info/PKG-INFO
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3548 2024-05-04 15:51:17.000000 pyegeria-0.3.8/src/pyegeria.egg-info/SOURCES.txt
+-rw-r--r--   0 dwolfson   (501) staff       (20)        1 2024-05-04 15:51:17.000000 pyegeria-0.3.8/src/pyegeria.egg-info/dependency_links.txt
+-rw-r--r--   0 dwolfson   (501) staff       (20)      140 2024-05-04 15:51:17.000000 pyegeria-0.3.8/src/pyegeria.egg-info/requires.txt
+-rw-r--r--   0 dwolfson   (501) staff       (20)        9 2024-05-04 15:51:17.000000 pyegeria-0.3.8/src/pyegeria.egg-info/top_level.txt
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-05-04 15:51:17.639236 pyegeria-0.3.8/tests/
+-rw-r--r--   0 dwolfson   (501) staff       (20)    41490 2024-05-03 16:29:09.000000 pyegeria-0.3.8/tests/test_automated_curation_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3006 2024-04-11 02:07:05.000000 pyegeria-0.3.8/tests/test_client.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    51872 2024-04-29 00:11:27.000000 pyegeria-0.3.8/tests/test_collection_manager_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    59269 2024-05-02 18:01:47.000000 pyegeria-0.3.8/tests/test_core_omag_server_config.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    11868 2024-04-10 19:14:09.000000 pyegeria-0.3.8/tests/test_full_omag_server_config.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    10582 2024-04-11 02:07:05.000000 pyegeria-0.3.8/tests/test_glossary_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     8350 2024-04-11 02:07:05.000000 pyegeria-0.3.8/tests/test_gov_engine.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    41146 2024-05-04 11:00:57.000000 pyegeria-0.3.8/tests/test_loaded_resources.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     9640 2024-05-04 15:38:39.000000 pyegeria-0.3.8/tests/test_my_profile_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    40084 2024-04-23 14:27:57.000000 pyegeria-0.3.8/tests/test_platform_services.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    28529 2024-04-26 16:12:52.000000 pyegeria-0.3.8/tests/test_project_manager_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     4712 2024-04-29 06:35:51.000000 pyegeria-0.3.8/tests/test_registered_info.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     8176 2024-05-03 16:46:09.000000 pyegeria-0.3.8/tests/test_server_operations.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5904 2024-04-11 02:07:05.000000 pyegeria-0.3.8/tests/test_util_exp.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    12782 2024-05-03 11:30:59.000000 pyegeria-0.3.8/tests/test_valid_metadata_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     6035 2024-04-11 02:07:05.000000 pyegeria-0.3.8/tests/test_validators.py
```

### Comparing `pyegeria-0.3.7/LICENSE` & `pyegeria-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/PKG-INFO` & `pyegeria-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyegeria
-Version: 0.3.7
+Version: 0.3.8
 Summary: A python client for Egeria
 Home-page: https://egeria-project.org/egeria-python
 Author: Dan Wolfson
 Author-email: Dan Wolfson <dan.wolfson@pdr-associates.com>
 Project-URL: Homepage, https://github.com/odpi/egeria-python
 Project-URL: Issues, https://github.com/odpi/egeria-python/issues
 Keywords: egeria,metadata,governance
```

### Comparing `pyegeria-0.3.7/README.md` & `pyegeria-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/.DS_Store` & `pyegeria-0.3.8/examples/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/Coco_config/README.md` & `pyegeria-0.3.8/examples/Coco_config/README.md`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/Coco_config/config_cocoMDS1.py` & `pyegeria-0.3.8/examples/Coco_config/config_cocoMDS1.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/Coco_config/config_cocoMDS2.py` & `pyegeria-0.3.8/examples/Coco_config/config_cocoMDS2.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/Coco_config/config_cocoMDS3.py` & `pyegeria-0.3.8/examples/Coco_config/config_cocoMDS3.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/Coco_config/config_cocoMDS4.py` & `pyegeria-0.3.8/examples/Coco_config/config_cocoMDS4.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/Coco_config/config_cocoMDS5.py` & `pyegeria-0.3.8/examples/Coco_config/config_cocoMDS5.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/Coco_config/config_cocoMDS6.py` & `pyegeria-0.3.8/examples/Coco_config/config_cocoMDS6.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/Coco_config/config_cocoMDSx.py` & `pyegeria-0.3.8/examples/Coco_config/config_cocoMDSx.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/Coco_config/config_cocoView1.py` & `pyegeria-0.3.8/examples/Coco_config/config_cocoView1.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/Coco_config/config_exchangeDL01.py` & `pyegeria-0.3.8/examples/Coco_config/config_exchangeDL01.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/Coco_config/config_governDL01.py` & `pyegeria-0.3.8/examples/Coco_config/config_governDL01.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/Coco_config/config_monitorDev01.py` & `pyegeria-0.3.8/examples/Coco_config/config_monitorDev01.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/Coco_config/config_monitorGov01.py` & `pyegeria-0.3.8/examples/Coco_config/config_monitorGov01.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/Coco_config/globals.py` & `pyegeria-0.3.8/examples/Coco_config/globals.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/Doc_Samples/Create_Collection_Sample.py` & `pyegeria-0.3.8/examples/Doc_Samples/Create_Collection_Sample.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/Doc_Samples/Create_Sustainability_Collection_Sample.py` & `pyegeria-0.3.8/examples/Doc_Samples/Create_Sustainability_Collection_Sample.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/Jupyter Notebooks/P-egeria-server-config.ipynb` & `pyegeria-0.3.8/examples/Jupyter Notebooks/P-egeria-server-config.ipynb`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/Jupyter Notebooks/common/P-environment-check.ipynb` & `pyegeria-0.3.8/examples/Jupyter Notebooks/common/P-environment-check.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9958333333333333%*

 * *Differences: {"'cells'": "{5: {'execution_count': None}}"}*

```diff
@@ -79,14 +79,15 @@
                 "\n",
                 "print (\"Done.\")\n",
                 "   "
             ]
         },
         {
             "cell_type": "code",
+            "execution_count": null,
             "metadata": {
                 "collapsed": false
             },
             "outputs": [],
             "source": []
         }
     ],
```

### Comparing `pyegeria-0.3.7/examples/Jupyter Notebooks/common/common-functions.ipynb` & `pyegeria-0.3.8/examples/Jupyter Notebooks/common/common-functions.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -2,15 +2,14 @@
     "cells": [
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "is_executing": true
             },
-            "outputs": [],
             "source": [
                 "#\n",
                 "# This file contains the common functions and definitions used in the Egeria Hands on\n",
                 "# Lab Notebooks.\n",
                 "#\n",
                 "\n",
                 "# These functions define the location and names of Coco Pharmaceutical's\n",
@@ -50,21 +49,21 @@
                 "\n",
                 "#\n",
                 "# Flag to enable debug, this cases extra information to be printed including rest calls request and response details\n",
                 "# Switching this flag to True produces a very large amount of output and is not recommended.\n",
                 "# A targeted use of this flag is recommended, set this before and reset this after the code you would like to produce debug\n",
                 "#\n",
                 "isDebug = False"
-            ]
+            ],
+            "outputs": []
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [],
             "source": [
                 "#\n",
                 "# Definitions of the Coco Pharmaceuticals Environment\n",
                 "#\n",
                 "\n",
                 "# These are the three main platforms used to run Egeria's OMAG Servers\n",
                 "corePlatformURL      = os.environ.get('corePlatformURL', 'https://localhost:9443')\n",
@@ -174,21 +173,21 @@
                 "monitorGov01MDS          = \"cocoMDS1\"\n",
                 "\n",
                 "monitorDev01PlatformURL  = devPlatformURL\n",
                 "monitorDev01PlatformName = devPlatformName\n",
                 "monitorDev01Name         = \"monitorDev01\"\n",
                 "monitorDev01ServerType   = \"Integration Daemon\"\n",
                 "monitorDev01MDS          = \"cocoMDSx\"\n"
-            ]
+            ],
+            "outputs": []
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [],
             "source": [
                 "#\n",
                 "# Common processing of REST API errors.\n",
                 "#\n",
                 "\n",
                 "import requests\n",
                 "import pprint\n",
@@ -306,42 +305,42 @@
                 "             printUnexpectedResponse(serverName, serverPlatformName, serverPlatformURL, response)\n",
                 "    return []\n",
                 "\n",
                 "def postAndPrintResult(url, json=None, headers=None):\n",
                 "    print (\"   ...... (POST\", url, \")\")\n",
                 "    response = requests.post(url, json=json, headers=headers, verify=False)\n",
                 "    print (\"   ...... Response: \", response.json())\n"
-            ]
+            ],
+            "outputs": []
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [],
             "source": [
                 "# Server configuration can be deployed from one OMAG Server Platform to another.\n",
                 "# This enables a server configuration to be tested and then deployed in production.\n",
                 "\n",
                 "def deployServerToPlatform(adminPlatformURL, adminUserId, serverName, platformURL):\n",
                 "    print(\"   ... deploying\", serverName, \"to the\", platformURL, \"platform...\")\n",
                 "    adminCommandURLRoot = adminPlatformURL + '/open-metadata/admin-services/users/' + adminUserId + '/servers/'\n",
                 "    url = adminCommandURLRoot + serverName + '/configuration/deploy'\n",
                 "    platformTarget = {\n",
                 "        \"class\": \"URLRequestBody\",\n",
                 "        \"urlRoot\": platformURL\n",
                 "    }\n",
                 "    jsonContentHeader = {'content-type':'application/json'}\n",
                 "    postAndPrintResult(url, json=platformTarget, headers=jsonContentHeader)\n"
-            ]
+            ],
+            "outputs": []
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [],
             "source": [
                 "# The OMAG Server Platform is a single executable (application) that can be started\n",
                 "# from the command line or a script or as part of a pre-built container environment\n",
                 "# such as Kubernetes.  The function below checks that a specific\n",
                 "# server platform is running.\n",
                 "\n",
                 "def checkServerPlatform(serverPlatformName, serverPlatformURL):\n",
@@ -487,19 +486,19 @@
                 "        if servers is not None:\n",
                 "            print(\"  \", servers)\n",
                 "    else:\n",
                 "        prettyResponse = json.dumps(response.json(), indent=4)\n",
                 "        print (\"Response: \")\n",
                 "        print (prettyResponse)\n",
                 "        print (\" \")\n"
-            ]
+            ],
+            "outputs": []
         },
         {
             "cell_type": "code",
-            "outputs": [],
             "source": [
                 "\n",
                 "#\n",
                 "# Administration services\n",
                 "#\n",
                 "\n",
                 "#\n",
@@ -713,21 +712,21 @@
                 "        \"omagserverName\" : mdrServerName,\n",
                 "        \"engines\" : governanceEngines\n",
                 "    }\n",
                 "    url = adminCommandURLRoot + engineServerName + '/engine-services/' + engineServiceURLMarker\n",
                 "    issuePost(url, requestBody)"
             ],
             "metadata": {},
-            "execution_count": 0
+            "execution_count": 0,
+            "outputs": []
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [],
             "source": [
                 "\n",
                 "# Each server is configured to define which services should be active.  This configuration results in\n",
                 "# the creation of a configuration document.  This document is read when the server is started and\n",
                 "# drives the initialization of the services.\n",
                 "\n",
                 "def checkServerConfigured(serverName, serverPlatformName, serverPlatformURL):\n",
@@ -827,21 +826,21 @@
                 "\n",
                 "def reActivatePlatform(serverPlatformName, serverPlatformURL, hostedServerNames):\n",
                 "    available = checkServerPlatform(serverPlatformName, serverPlatformURL)\n",
                 "    if available == True:\n",
                 "        for x in range(len(hostedServerNames)):\n",
                 "            activateServerOnPlatform(hostedServerNames[x], serverPlatformName, serverPlatformURL)\n",
                 "\n"
-            ]
+            ],
+            "outputs": []
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [],
             "source": [
                 "#\n",
                 "# Repository Services\n",
                 "#\n",
                 "\n",
                 "# Understanding Cohorts\n",
                 "#\n",
@@ -1002,28 +1001,28 @@
                 "        printRemoteRegistrations(serverName, cohorts[x], serverPlatformName, serverPlatformURL)\n",
                 "        print(\" \")\n",
                 "\n",
                 "def unregisterFromCohort(serverName, cohortName, serverPlatformName, serverPlatformURL):\n",
                 "    metadataHighwayServicesURLcore = '/servers/' + serverName + '/open-metadata/repository-services/users/' + adminUserId + '/metadata-highway'\n",
                 "    url = serverPlatformURL + metadataHighwayServicesURLcore + '/cohorts/' + cohortName + '/unregister'\n",
                 "    response = issueGet(url)\n"
-            ]
+            ],
+            "outputs": []
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [],
-            "source": []
+            "source": [],
+            "outputs": []
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [],
             "source": [
                 "#\n",
                 "# OMAS\n",
                 "# Working with asset elements - this set of functions displays assets returned from the open metadata repositories.\n",
                 "# \n",
                 "\n",
                 "def printAssetSummary(asset):\n",
@@ -1108,21 +1107,21 @@
                 "def getLastGUID(guids):\n",
                 "    if guids == None:\n",
                 "        return \"<unknown>\"\n",
                 "    else:\n",
                 "        for guid in guids:\n",
                 "            returnGUID = guid\n",
                 "        return returnGUID"
-            ]
+            ],
+            "outputs": []
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [],
             "source": [
                 "#\n",
                 "# OCF Common services\n",
                 "# Working with assets - this set of functions displays assets returned from the open metadata repositories.\n",
                 "# \n",
                 "\n",
                 "\n",
@@ -1599,21 +1598,21 @@
                 "            if commentText:\n",
                 "                print(\"  comment text: \" + commentText)\n",
                 "            if commentUser:\n",
                 "                print(\"  created by:   \" + commentUser)\n",
                 "            if isPublic:\n",
                 "                print(\"  public:       \" + str(isPublic))\n",
                 "\n"
-            ]
+            ],
+            "outputs": []
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [],
             "source": [
                 "   \n",
                 "#\n",
                 "# Working with assets - this set of functions are for authoring assets.\n",
                 "# Using the Asset Owner OMAS interface to create and query assets.  Notice that the interface returns all of the asset contents.\n",
                 "# \n",
                 "\n",
@@ -1810,21 +1809,21 @@
                 "    semanticAssignmentURL =  assetOwnerURL + '/assets/' + assetGUID + '/attachments/' + schemaGUID + '/meanings/' + glossaryTermGUID\n",
                 "    response=issuePost(semanticAssignmentURL, {})\n",
                 "    if response.status_code == 200:\n",
                 "        print(\"Semantic assignment relationship created\") \n",
                 "    else:\n",
                 "        print (\"No semantic assignment Relationship created\")\n",
                 "        processErrorResponse(serverName, serverPlatformName, serverPlatformURL, response)\n"
-            ]
+            ],
+            "outputs": []
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [],
             "source": [
                 "#\n",
                 "# Asset Consumer OMAS\n",
                 "#\n",
                 "\n",
                 "# Retrieve the OutTopic connection\n",
                 "\n",
@@ -2262,21 +2261,21 @@
                 "    printAssetCommentReplies(serverName, serverPlatformName, serverPlatformURL, \"asset-consumer\", userId, requestType, commentGUID)\n",
                 "\n",
                 "def assetConsumerPrintRelatedAssets(serverName, serverPlatformName, serverPlatformURL, userId, requestType):\n",
                 "    printRelatedAssets(serverName, serverPlatformName, serverPlatformURL, \"asset-consumer\", userId, requestType)\n",
                 "\n",
                 "def assetConsumerPrintAssetComments(serverName, serverPlatformName, serverPlatformURL, userId, requestType):\n",
                 "    printAssetComments(serverName, serverPlatformName, serverPlatformURL, \"asset-consumer\", userId, requestType)\n"
-            ]
+            ],
+            "outputs": []
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [],
             "source": [
                 "#\n",
                 "# Asset Manager OMAS\n",
                 "# This function assumes the assets exist, and it creates the lineage between the source asset schema type, to the port to the process to the port to \n",
                 "# the target asset schematype\n",
                 "#\n",
                 "def createDirectedProcessBetweenAssets(serverName, serverPlatformName, serverPlatformURL, userId, sourceSchemaTypeGuid, targetSchemaTypeGuid, processName, processDescription, processFormula):\n",
@@ -2378,28 +2377,28 @@
                 "        else:\n",
                 "            print (\"Process \" + processName + \" created.\") \n",
                 "        return processGuid\n",
                 "    else:\n",
                 "        print (\"No process created\")\n",
                 "        processErrorResponse(serverName, serverPlatformName, serverPlatformURL, response)\n",
                 "    "
-            ]
+            ],
+            "outputs": []
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [],
-            "source": []
+            "source": [],
+            "outputs": []
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [],
             "source": [
                 "#\n",
                 "# Subject Area OMAS\n",
                 "# Working with glossaries - this set of functions displays glossary content returned from the open metadata repositories.\n",
                 "#         \n",
                 "\n",
                 "def printGlossarySummary(glossary):\n",
@@ -2650,21 +2649,21 @@
                 "    except EnvironmentError: # parent of IOError, OSError *and* WindowsError where available\n",
                 "        print(\"Error opening File \" + fileName)         \n",
                 "    if (term_count > 0):        \n",
                 "        print(\"Created \" + str(term_count))    \n",
                 "    else:\n",
                 "        print(\"No terms created\")\n",
                 "        \n"
-            ]
+            ],
+            "outputs": []
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [],
             "source": [
                 "# Open Governance and Discovery\n",
                 "# Working with the engine host server and the Governance Engine OMAS of the metadata server.\n",
                 "\n",
                 "## Governance Action Open Metadata Engine Services (OMES) validation of a governance service connector\n",
                 "\n",
                 "def validateGovernanceActionEngineConnector(serverName, serverPlatformName, serverPlatformURL, userId, connectorProvider):\n",
@@ -3303,21 +3302,21 @@
                 "            else:\n",
                 "                printUnexpectedResponse(serverName, serverPlatformName, serverPlatformURL, response)\n",
                 "        else:\n",
                 "            printUnexpectedResponse(serverName, serverPlatformName, serverPlatformURL, response)\n",
                 "    except Exception as error:\n",
                 "        print(\"Exception: %s\" % error)\n",
                 "        print(\"Platform \" + serverPlatformURL + \" is returning an error\")\n"
-            ]
+            ],
+            "outputs": []
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [],
             "source": [
                 "#\n",
                 "# Working with Governance Actions, Governance Action Processes and Governance Action Types through the Governance Engine OMAS\n",
                 "#\n",
                 "\n",
                 "def createIntegrationGroup(serverName, serverPlatformName, serverPlatformURL, userId, integrationGroupName, description):\n",
                 "    commandURLRoot = serverPlatformURL + \"/servers/\" + serverName + \"/open-metadata/access-services/governance-engine/users/\" + userId        \n",
@@ -3663,33 +3662,33 @@
                 "            if relatedHTTPCode != 200:\n",
                 "                printUnexpectedResponse(serverName, serverPlatformName, serverPlatformURL, response)\n",
                 "        else:\n",
                 "            printUnexpectedResponse(serverName, serverPlatformName, serverPlatformURL, response)\n",
                 "    except Exception as error:\n",
                 "        print(\"Exception: %s\" % error )\n",
                 "        print(\"Platform \" + serverPlatformURL + \" is returning an error\")\n"
-            ]
+            ],
+            "outputs": []
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [],
             "source": [
                 "#\n",
                 "# Using the OpenMetadataStore services to report on running governance action processes.\n",
                 "#\n",
                 "\n"
-            ]
+            ],
+            "outputs": []
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [],
             "source": [
                 "# \n",
                 "# Interaction with the Integration Daemon OMAG Server\n",
                 "#\n",
                 "def printIntegrationConnectorStatus(integrationConnectorSummary):\n",
                 "    connectorName = integrationConnectorSummary.get('connectorName')\n",
                 "    if connectorName:\n",
@@ -3841,21 +3840,21 @@
                 "                printResponse(response)\n",
                 "        else:\n",
                 "            printResponse(response)\n",
                 "    except Exception as error:\n",
                 "        print(\"Exception: %s\" % error)\n",
                 "        print(\"Platform \" + serverPlatformURL + \" is returning an error\")\n",
                 "        "
-            ]
+            ],
+            "outputs": []
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [],
             "source": [
                 "## Open Metadata Integration Services\n",
                 "\n",
                 "def validateIntegrationConnector(serverName, serverPlatformName, serverPlatformURL, serviceURLMarker, userId, connectorProvider):\n",
                 "    try:\n",
                 "        integrationServiceURL = serverPlatformURL + '/servers/' + serverName + '/open-metadata/integration-services/' + serviceURLMarker + '/users/' + userId \n",
                 "        getStatusURL = integrationServiceURL + '/validate-connector/' + connectorProvider\n",
@@ -3916,21 +3915,21 @@
                 "                printResponse(response)\n",
                 "        else:\n",
                 "            printResponse(response)\n",
                 "    except Exception as error:\n",
                 "        print(\"Exception: %s\" % error)\n",
                 "        print(\"Platform \" + serverPlatformURL + \" is returning an error\")\n",
                 "        \n"
-            ]
+            ],
+            "outputs": []
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [],
             "source": [
                 "#\n",
                 "# Load an archive\n",
                 "#\n",
                 "def loadArchive(serverName, serverPlatformName, serverPlatformURL, archiveFileName):\n",
                 "    loadArchiveURL = serverPlatformURL +  '/open-metadata/admin-services/users/' +  adminUserId + '/servers/' + serverName + '/instance/open-metadata-archives/file'\n",
                 "    print(\" \")\n",
@@ -3939,21 +3938,21 @@
                 "        print(\"Archive loaded: \" + archiveFileName)\n",
                 "    else:\n",
                 "        print (\"Returns:\")\n",
                 "        prettyResponse = json.dumps(response.json(), indent=4)\n",
                 "        print (prettyResponse)\n",
                 "    print(\" \")\n",
                 "\n"
-            ]
+            ],
+            "outputs": []
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
-            "outputs": [],
             "source": [
                 "#\n",
                 "# Issue requests to the Asset Manager OMAS\n",
                 "#\n",
                 "\n",
                 "def displayTermSummary(displayName, description):\n",
                 "    nameWidth=40\n",
@@ -4663,15 +4662,16 @@
                 "            printResponse(response)\n",
                 "    except Exception as error:\n",
                 "        print(\"Exception: %s\" % error)\n",
                 "        print(\"Platform \" + serverPlatformName + \" (\" + serverPlatformURL + \") is returning an error\")\n",
                 "\n",
                 "\n",
                 "\n"
-            ]
+            ],
+            "outputs": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
```

### Comparing `pyegeria-0.3.7/examples/Jupyter Notebooks/common/environment-check.ipynb` & `pyegeria-0.3.8/examples/Jupyter Notebooks/common/environment-check.ipynb`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/Jupyter Notebooks/common/globals.ipynb` & `pyegeria-0.3.8/examples/Jupyter Notebooks/common/globals.ipynb`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/Jupyter Notebooks/common/globals.py` & `pyegeria-0.3.8/examples/Jupyter Notebooks/common/globals.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/Jupyter Notebooks/common/orig_globals.py` & `pyegeria-0.3.8/examples/Jupyter Notebooks/common/orig_globals.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/widgets/.DS_Store` & `pyegeria-0.3.8/examples/widgets/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/widgets/README.md` & `pyegeria-0.3.8/examples/widgets/README.md`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/widgets/__pycache__/server_status_widget.cpython-312-pytest-7.4.4.pyc` & `pyegeria-0.3.8/examples/widgets/__pycache__/server_status_widget.cpython-312-pytest-7.4.4.pyc`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/widgets/coco_status.py` & `pyegeria-0.3.8/examples/widgets/coco_status.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/widgets/collection_viewer.py` & `pyegeria-0.3.8/examples/widgets/collection_viewer.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/widgets/engine_action_status.py` & `pyegeria-0.3.8/examples/widgets/engine_action_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 A simple status display for Engine Actions
 """
 
 import argparse
 import json
 import time
+import sys
 
 from rich import box
 from rich.live import Live
 from rich.table import Table
 from rich.console import Console
 
 from pyegeria import (
@@ -72,27 +73,27 @@
         table.add_column("Target Element")
         table.add_column("Completion Time")
         table.add_column("Process Name")
         table.add_column("Completion Message")
 
         token = g_client.create_egeria_bearer_token()
         action_status = g_client.get_engine_actions()
-        if "No Elements" in action_status:
+        if type(action_status) is str:
             requested_time = " "
             start_time = " "
             completion_time = " "
             engine_name = " "
             request_type = " "
             action_status = " "
             target_element = " "
             process_name = " "
             completion_message = " "
-        else:
+        elif type(action_status) is list:
             for action in action_status:
-                requested_time = action["requestedTime"]
+                requested_time = action.get("requestedTime", " ")
                 start_time = action.get("startTime", " ")
                 completion_time = action.get("completionTime", " ")
 
                 engine_name = action["governanceEngineName"]
                 request_type = action["requestType"]
                 action_guid = action["elementHeader"]["guid"]
                 if action["actionStatus"] in ("REQUESTED", "APPROVED", "WAITING", "ACTIVATING"):
@@ -111,15 +112,17 @@
                 process_name = action.get("processName", " ")
                 completion_message = action.get("completionMessage", " ")
 
                 table.add_row(
                     requested_time, start_time, action_guid,engine_name, request_type,
                     action_status, target_element, completion_time, process_name, completion_message
                 )
-
+        else:
+            print("Egeria integration daemon not running")
+            sys.exit()
         # g_client.close_session()
         return table
 
     try:
         console = Console()
         with console.pager():
             console.print(generate_table())
```

### Comparing `pyegeria-0.3.7/examples/widgets/find_todos.py` & `pyegeria-0.3.8/examples/widgets/find_todos.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,17 +77,17 @@
         table.add_column("Created")
         table.add_column("Priority")
         table.add_column("Due")
         table.add_column("Completion")
         table.add_column("Status")
         table.add_column("Sponsor")
 
-        todo_items = m_client.find_to_do("*", starts_with=True)
+        todo_items = m_client.find_to_do(search_string)
 
-        if todo_items is None:
+        if type(todo_items) is str:
             name = " "
             type_name = " "
             created = " "
             priority = " "
             due = " "
             completed = " "
             status = " "
@@ -103,15 +103,15 @@
                 completed = props.get("completionTime", " ")
                 status = props.get("status")
                 # assigned_actors = item["assignedActors"]
                 # sponsor = assigned_actors[0].get("uniqueName", " ")
                 sponsor = "erinoverview"
                 if status in ("WAITING", "OPEN"):
                     status = f"[yellow]{status}"
-                elif status in ("INPROGRESS", "COMPLETE"):
+                elif status in ("IN_PROGRESS", "COMPLETE"):
                     status = f"[green]{status}"
                 else:
                     status = f"[red]{status}"
 
                 table.add_row(
                     name, type_name, created, priority, due, completed, status, sponsor
                 )
```

### Comparing `pyegeria-0.3.7/examples/widgets/get_relationship_types.py` & `pyegeria-0.3.8/examples/widgets/get_relationship_types.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/widgets/get_tech_details.py` & `pyegeria-0.3.8/examples/widgets/get_tech_details.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/widgets/get_tech_types.py` & `pyegeria-0.3.8/examples/widgets/get_tech_types.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/widgets/get_valid_metadata_values.py` & `pyegeria-0.3.8/examples/widgets/get_valid_metadata_values.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/widgets/glossary_view.py` & `pyegeria-0.3.8/examples/widgets/glossary_view.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/widgets/gov_engine_status.py` & `pyegeria-0.3.8/examples/widgets/gov_engine_status.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/widgets/integration_daemon_status.py` & `pyegeria-0.3.8/examples/widgets/integration_daemon_status.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/widgets/list_asset_types.py` & `pyegeria-0.3.8/examples/widgets/list_asset_types.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/widgets/multi-server_status.py` & `pyegeria-0.3.8/examples/widgets/multi-server_status.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/widgets/my_todos.py` & `pyegeria-0.3.8/examples/widgets/my_todos.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/widgets/open_todos.py` & `pyegeria-0.3.8/examples/widgets/open_todos.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/widgets/project_list_viewer.py` & `pyegeria-0.3.8/examples/widgets/project_list_viewer.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/widgets/server_status.py` & `pyegeria-0.3.8/examples/widgets/server_status.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/widgets/server_status_widget.py` & `pyegeria-0.3.8/examples/widgets/server_status_widget.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/examples/widgets/view_my_profile.py` & `pyegeria-0.3.8/examples/widgets/view_my_profile.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/pyproject.toml` & `pyegeria-0.3.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #requires = ["hatchling"]
 requires = ["setuptools", "wheel"]
 #build-backend = "hatchling.build"
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyegeria"
-version = "0.3.7"
+version = "0.3.8"
 #license = 'Apache 2.0'
 authors = [
     {name ="Dan Wolfson", email= "dan.wolfson@pdr-associates.com"},
 ]
 dependencies = [
     "requests~=2.31.0",
     "validators~=0.22.0",
```

### Comparing `pyegeria-0.3.7/setup.py` & `pyegeria-0.3.8/setup.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/src/pyegeria/__init__.py` & `pyegeria-0.3.8/src/pyegeria/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,8 +39,9 @@
 from .gov_engine import GovEng
 from .my_profile_omvs import MyProfile
 from .full_omag_server_config import FullServerConfig
 from .server_operations import ServerOps
 from .collection_manager_omvs import CollectionManager
 from .project_manager_omvs import ProjectManager
 from .valid_metadata_omvs import ValidMetadataManager
-__version__ = "0.3"
+from .loaded_resources_omvs import LoadedResources
+__version__ = "0.38"
```

### Comparing `pyegeria-0.3.7/src/pyegeria/_client.py` & `pyegeria-0.3.8/src/pyegeria/_client.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/src/pyegeria/_exceptions.py` & `pyegeria-0.3.8/src/pyegeria/_exceptions.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/src/pyegeria/_globals.py` & `pyegeria-0.3.8/src/pyegeria/_globals.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/src/pyegeria/_validators.py` & `pyegeria-0.3.8/src/pyegeria/_validators.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/src/pyegeria/automated_curation_omvs.py` & `pyegeria-0.3.8/src/pyegeria/automated_curation_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/src/pyegeria/collection_manager_omvs.py` & `pyegeria-0.3.8/src/pyegeria/collection_manager_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/src/pyegeria/core_omag_server_config.py` & `pyegeria-0.3.8/src/pyegeria/core_omag_server_config.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/src/pyegeria/full_omag_server_config.py` & `pyegeria-0.3.8/src/pyegeria/full_omag_server_config.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/src/pyegeria/glossary_omvs.py` & `pyegeria-0.3.8/src/pyegeria/glossary_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/src/pyegeria/gov_engine.py` & `pyegeria-0.3.8/src/pyegeria/gov_engine.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/src/pyegeria/governance_author.py` & `pyegeria-0.3.8/src/pyegeria/governance_author.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/src/pyegeria/my_profile_omvs.py` & `pyegeria-0.3.8/src/pyegeria/my_profile_omvs.py`

 * *Files 1% similar despite different names*

```diff
@@ -717,15 +717,15 @@
            NotAuthorizedException
            The principle specified by the user_id does not have authorization for the requested action
            """
         loop = asyncio.get_event_loop()
         loop.run_until_complete(self._async_reassign_to_do(todo_guid, actor_guid, status, server_name))
         return
 
-    async def _async_find_to_do(self, search_string: str = "*", server_name: str = "None", status: str = None,
+    async def _async_find_to_do(self, search_string: str = "*", server_name: str = "None", status: str = "OPEN",
                                 starts_with: bool = False, ends_with: bool = False, ignore_case: bool = True,
                                 start_from: int = 0, page_size: int = 100) -> list | str:
         """ find To-Do items. Async version.
               Parameters
               ----------
                 search_string: str
                    String to search against. If '*' then all to-do items will match.
@@ -761,30 +761,31 @@
         ends_with_s = str(ends_with).lower()
         ignore_case_s = str(ignore_case).lower()
 
         if search_string is '*':
             search_string = " "
 
         body = {
-            "status": status,
+            "class": "ToDoStatusSearchString",
+            "toDoStatus": status,
             "searchString": search_string
         }
 
         validate_search_string(search_string)
 
         url = (f"{self.my_profile_command_root}/{server_name}/api/open-metadata/my-profile/to-dos/"
                f"find-by-search-string?startFrom={start_from}&pageSize={page_size}&"
                f"startsWith={starts_with_s}&endsWith={ends_with_s}&ignoreCase={ignore_case_s}")
 
         response = await self._async_make_request("POST", url, body)
         # return response.text
-        return response.json().get("toDoElements", "No guid returned")
+        return response.json().get("toDoElements", "No ToDos found")
 
     def find_to_do(self, search_string: str, server_name: str = None, status: str = "OPEN",
-                   starts_with: bool = True, ends_with: bool = False, ignore_case: bool = False,
+                   starts_with: bool = False, ends_with: bool = False, ignore_case: bool = True,
                    start_from: int = 0, page_size: int = 100) -> list | str:
         """ find To-Do items.
             Parameters
             ----------
            search_string: str
               String to search against. If '*' then all to-do items will match.
            server_name : str, optional
@@ -861,15 +862,15 @@
 
         }
 
         url = (f"{self.my_profile_command_root}/{server_name}/api/open-metadata/my-profile/to-dos/types/"
                f"{todo_type}?startFrom={start_from}&pageSize={page_size}")
 
         response = await self._async_make_request("POST", url, body)
-        return response.text if response is not None else "No Results"
+        return response.json().get("toDoElements","No ToDos found")
 
     def get_to_dos_by_type(self, todo_type: str,  server_name: str = None, status: str = "OPEN",
                            start_from: int = 0, page_size: int = 100) -> list | str:
         """ Get To-Do items by type.
             Parameters
             ----------
             todo_type: str
```

### Comparing `pyegeria-0.3.7/src/pyegeria/platform_services.py` & `pyegeria-0.3.8/src/pyegeria/platform_services.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/src/pyegeria/project_manager_omvs.py` & `pyegeria-0.3.8/src/pyegeria/project_manager_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/src/pyegeria/registered_info.py` & `pyegeria-0.3.8/src/pyegeria/registered_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 SPDX-License-Identifier: Apache-2.0
 Copyright Contributors to the ODPi Egeria project.
 
 
 
 This module allows users to query the available (registered) capabilities of Egeria. Detailed information is returned
 to provide both insight and understanding in how to use these capabilities. For example, when configuring an Egeria
-integration service, it is important to know what companion service it depends on so that you can make sure the
+integration service, it is importregistered_info.pyant to know what companion service it depends on so that you can make sure the
 companion service is also configured and running.
 
 """
 import json
 from rich.console import Console
 from rich import print, print_json
```

### Comparing `pyegeria-0.3.7/src/pyegeria/server_operations.py` & `pyegeria-0.3.8/src/pyegeria/server_operations.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/src/pyegeria/utils.py` & `pyegeria-0.3.8/src/pyegeria/utils.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/src/pyegeria/valid_metadata_omvs.py` & `pyegeria-0.3.8/src/pyegeria/valid_metadata_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/src/pyegeria.egg-info/PKG-INFO` & `pyegeria-0.3.8/src/pyegeria.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyegeria
-Version: 0.3.7
+Version: 0.3.8
 Summary: A python client for Egeria
 Home-page: https://egeria-project.org/egeria-python
 Author: Dan Wolfson
 Author-email: Dan Wolfson <dan.wolfson@pdr-associates.com>
 Project-URL: Homepage, https://github.com/odpi/egeria-python
 Project-URL: Issues, https://github.com/odpi/egeria-python/issues
 Keywords: egeria,metadata,governance
```

### Comparing `pyegeria-0.3.7/src/pyegeria.egg-info/SOURCES.txt` & `pyegeria-0.3.8/src/pyegeria.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 src/pyegeria/automated_curation_omvs.py
 src/pyegeria/collection_manager_omvs.py
 src/pyegeria/core_omag_server_config.py
 src/pyegeria/full_omag_server_config.py
 src/pyegeria/glossary_omvs.py
 src/pyegeria/gov_engine.py
 src/pyegeria/governance_author.py
+src/pyegeria/loaded_resources_omvs.py
 src/pyegeria/my_profile_omvs.py
 src/pyegeria/platform_services.py
 src/pyegeria/project_manager_omvs.py
 src/pyegeria/registered_info.py
 src/pyegeria/server_operations.py
 src/pyegeria/utils.py
 src/pyegeria/valid_metadata_omvs.py
@@ -83,14 +84,15 @@
 tests/test_automated_curation_omvs.py
 tests/test_client.py
 tests/test_collection_manager_omvs.py
 tests/test_core_omag_server_config.py
 tests/test_full_omag_server_config.py
 tests/test_glossary_omvs.py
 tests/test_gov_engine.py
+tests/test_loaded_resources.py
 tests/test_my_profile_omvs.py
 tests/test_platform_services.py
 tests/test_project_manager_omvs.py
 tests/test_registered_info.py
 tests/test_server_operations.py
 tests/test_util_exp.py
 tests/test_valid_metadata_omvs.py
```

### Comparing `pyegeria-0.3.7/tests/test_automated_curation_omvs.py` & `pyegeria-0.3.8/tests/test_automated_curation_omvs.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,20 +66,20 @@
 
     def test_create_element_from_template(self):
         try:
             a_client = AutomatedCuration(self.good_view_server_1, self.good_platform1_url,
                                          user_id=self.good_user_2, user_pwd="secret")
             token = a_client.create_egeria_bearer_token()
             body = {
-                "templateGUID": "5e1ff810-5418-43f7-b7c4-e6e062f9aff7",
+                "templateGUID": "379e6c05-9cfa-4d31-a837-0ed4eee6482a",
                 "isOwnAnchor": "true",
                 "placeholderPropertyValues": {
-                    "serverName": "localKafka6",
-                    "hostIdentifier": "localhost",
-                    "portNumber": "9092"
+                    "pathName": "/Users/dwolfson/localGit/thebrain-api-quickstart-python",
+                    "deployedImplementationType": "File Folder",
+                    "folderName": "brain-api-quickstart"
                 }
             }
             start_time = time.perf_counter()
             response = a_client.create_element_from_template(body)
             duration = time.perf_counter() - start_time
             print(f"\n\tDuration was {duration} seconds")
             print("Guid of created element is:" + response)
@@ -131,18 +131,18 @@
     def test_create_postgres_server_element_from_template(self):
         try:
             a_client = AutomatedCuration(self.good_view_server_1, self.good_platform1_url,
                                          user_id=self.good_user_2, user_pwd="secret")
             token = a_client.create_egeria_bearer_token()
 
             start_time = time.perf_counter()
-            response = a_client.create_postgres_server_element_from_template("egeria-pdr",
-                                                                             "egeria.com",
-                                                                             "5432", db_user="surveyor",
-                                                                             db_pwd="secret")
+            response = a_client.create_postgres_server_element_from_template("egeria-laz-postgres",
+                                                                             "localhost",
+                                                                             "5432", db_user="postgres",
+                                                                             db_pwd="notingres")
             duration = time.perf_counter() - start_time
             print(f"\n\tDuration was {duration} seconds")
             if type(response) is list :
                 out = ("\n\n" + json.dumps(response, indent=4))
                 count = len(response)
                 pprint(f"Found {count} elements")
                 print_json(out)
@@ -851,16 +851,16 @@
     def test_catalog_folder_files(self):
         try:
             a_client = AutomatedCuration(self.good_view_server_1, self.good_platform1_url,
                                          user_id=self.good_user_2, user_pwd="secret")
             token = a_client.create_egeria_bearer_token()
             # jdbc_database_connector_guid = "70dcd0b7-9f06-48ad-ad44-ae4d7a7762aa"
             # postgres_connector_guid = "36f69fd0-54ba-4f59-8a44-11ccf2687a34"
-            folder_guid = "289172e5-d5f5-4673-854c-847192f2eaef"
-            catalog_target_name = "Dan's Downloads Folder"
+            folder_guid = "aaffdb1b-269f-4a1e-9325-7a324ee0ddf4"
+            catalog_target_name = "Brain-API-Quickstart"
             file_connector_guid = "d13ba229-d406-43f7-b395-9462b7d98900"
             # element_guid = "64296369-323f-4d74-aab3-c2ebae923d25"
             # catalog_target_name = "coco_ods_catalog_target"
             start_time = time.perf_counter()
             a_client.add_catalog_target(file_connector_guid,
                                                    folder_guid, catalog_target_name)
             duration = time.perf_counter() - start_time
@@ -909,15 +909,15 @@
             a_client.close_session()
 
     def test_initiate_postgres_server_survey(self):
         try:
             a_client = AutomatedCuration(self.good_view_server_1, self.good_platform1_url,
                                          user_id=self.good_user_2, user_pwd="secret")
             token = a_client.create_egeria_bearer_token()
-            a_postgres_server_guid = "64296369-323f-4d74-aab3-c2ebae923d25"
+            a_postgres_server_guid = "045d25f5-d998-44fa-b196-eaec7be7c376"
             start_time = time.perf_counter()
 
             response = a_client.initiate_postgres_server_survey(a_postgres_server_guid)
             duration = time.perf_counter() - start_time
             print(f"\n\tDuration was {duration} seconds")
             if type(response) is dict:
                 out = ("\n\n" + json.dumps(response, indent=4))
@@ -974,15 +974,15 @@
     def test_initiate_file_folder_survey(self):
         try:
             a_client = AutomatedCuration(self.good_view_server_1, self.good_platform1_url,
                                          user_id=self.good_user_2, user_pwd="secret")
             token = a_client.create_egeria_bearer_token()
 
             start_time = time.perf_counter()
-            file_folder_guid = "289172e5-d5f5-4673-854c-847192f2eaef"
+            file_folder_guid = "aaffdb1b-269f-4a1e-9325-7a324ee0ddf4"
             response = a_client.initiate_file_folder_survey(file_folder_guid)
             duration = time.perf_counter() - start_time
             print(f"\n\tDuration was {duration} seconds")
             if type(response) is dict:
                 out = ("\n\n" + json.dumps(response, indent=4))
                 count = len(response)
                 console.log(f"Found {count} elements")
```

### Comparing `pyegeria-0.3.7/tests/test_client.py` & `pyegeria-0.3.8/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/tests/test_collection_manager_omvs.py` & `pyegeria-0.3.8/tests/test_collection_manager_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/tests/test_core_omag_server_config.py` & `pyegeria-0.3.8/tests/test_core_omag_server_config.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/tests/test_full_omag_server_config.py` & `pyegeria-0.3.8/tests/test_full_omag_server_config.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/tests/test_glossary_omvs.py` & `pyegeria-0.3.8/tests/test_glossary_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/tests/test_gov_engine.py` & `pyegeria-0.3.8/tests/test_gov_engine.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/tests/test_my_profile_omvs.py` & `pyegeria-0.3.8/tests/test_my_profile_omvs.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,15 @@
     def test_create_to_do(self, server_name:str = good_view_server_1):
         try:
             m_client = MyProfile(server_name, self.good_platform1_url,
                                  user_id=self.good_user_2)
 
             token = m_client.create_egeria_bearer_token(self.good_user_2, "secret")
             erins_guid = "a588fb08-ae09-4415-bd5d-991882ceacba"
-            to_do = "Make Latte"
+            to_do = "Peter will delegate the Latte to Mandy"
             to_do_desc = "Latte to go"
             to_do_type = "drink"
             body = {
                         "properties": {
                             "class" : "ToDoProperties",
                             "qualifiedName": f"Test-To-Do-{time.asctime()}",
                             "name": to_do,
@@ -226,15 +226,15 @@
         console = Console()
         try:
             m_client = MyProfile(server_name, self.good_platform1_url,
                                  user_id=self.good_user_2)
 
             token = m_client.create_egeria_bearer_token(self.good_user_2, "secret")
 
-            response = m_client.find_to_do("*", starts_with=True)
+            response = m_client.find_to_do("latte")
 
             if type(response) is list:
                 print(f"Found {len(response)} todos that matched the criteria")
 
                 print_json(data=response)
             elif type(response) is str:
                 console.print("\n\n\t Response is " + response)
@@ -256,20 +256,20 @@
         console = Console()
         try:
             m_client = MyProfile(server_name, self.good_platform1_url,
                                  user_id=self.good_user_2)
 
             token = m_client.create_egeria_bearer_token(self.good_user_2, "secret")
 
-            response = m_client.get_to_dos_by_type("Drink", server_name, status="OPEN")
+            response = m_client.get_to_dos_by_type("Drink", server_name, status=None)
 
             if type(response) is list | dict:
                 print_json(data=response)
             elif type(response) is str:
-                console.print("\n\n\t Response is" + response)
+                console.print("\n\n\t Response is \n" + response)
             assert True
 
         except (
                 InvalidParameterException,
                 PropertyServerException,
                 UserNotAuthorizedException
         ) as e:
```

### Comparing `pyegeria-0.3.7/tests/test_platform_services.py` & `pyegeria-0.3.8/tests/test_platform_services.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/tests/test_project_manager_omvs.py` & `pyegeria-0.3.8/tests/test_project_manager_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/tests/test_registered_info.py` & `pyegeria-0.3.8/tests/test_registered_info.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/tests/test_server_operations.py` & `pyegeria-0.3.8/tests/test_server_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from pyegeria.server_operations import ServerOps
 
 disable_ssl_warnings = True
 
 
 class TestServerOperations:
     good_platform1_url = "https://127.0.0.1:9443"
-    good_platform2_url = "https://oak.local:9443"
+    good_platform2_url = "https://localhost:9446"
     bad_platform1_url = "https://localhost:9443"
 
     # good_platform1_url = "https://127.0.0.1:30080"
     # good_platform2_url = "https://127.0.0.1:30081"
     # bad_platform1_url = "https://localhost:9443"
 
     good_user_1 = "garygeeke"
@@ -160,33 +160,35 @@
         except (InvalidParameterException, PropertyServerException) as e:
             print_exception_response(e)
             assert e.related_http_code != "200", "Invalid parameters"
 
 # todo - review with Mandy?
     def test_restart_integration_connector(self, server:str = good_server_2):
         try:
-            server_name = server
+            server_name = "ecosystem-monitor"
             # connector = "FilesMonitor"
-            connector = "DataFilesMonitorIntegrationConnector"
-            s_client = ServerOps(server_name, self.good_platform1_url, self.good_user_1)
+            # connector = "DataFilesMonitorIntegrationConnector"
+
+            connector = None
+            s_client = ServerOps(server_name, self.good_platform2_url, self.good_user_1)
             # response = s_client.restart_integration_connector(connector,server)
-            s_client.restart_integration_connector(connector, server)
+            s_client.restart_integration_connector(connector, server_name)
 
             assert True, "Invalid URL or server"
 
         except (InvalidParameterException, PropertyServerException) as e:
             print_exception_response(e)
             assert e.related_http_code != "200", "Invalid parameters"
 
     def test_refresh_integration_connectors(self, server:str = good_server_2):
         try:
-            server_name = server
+            server_name = "ecosystem-monitor"
             connector = "FilesMonitor"
-            s_client = ServerOps(server_name, self.good_platform1_url, self.good_user_1)
+            s_client = ServerOps(server_name, self.good_platform2_url, self.good_user_1)
 
-            s_client.refresh_integration_connectors(None, server)
+            s_client.refresh_integration_connectors(None, server_name)
 
             assert True, "Invalid URL or server"
 
         except (InvalidParameterException, PropertyServerException) as e:
             print_exception_response(e)
             assert e.related_http_code != "200", "Invalid parameters"
```

### Comparing `pyegeria-0.3.7/tests/test_util_exp.py` & `pyegeria-0.3.8/tests/test_util_exp.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/tests/test_valid_metadata_omvs.py` & `pyegeria-0.3.8/tests/test_valid_metadata_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.7/tests/test_validators.py` & `pyegeria-0.3.8/tests/test_validators.py`

 * *Files identical despite different names*

