# Comparing `tmp/geoseeq-0.5.6a9.tar.gz` & `tmp/geoseeq-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoseeq-0.5.6a9.tar", last modified: Fri Apr  5 17:19:16 2024, max compression
+gzip compressed data, was "geoseeq-0.6.0.tar", last modified: Sat May  4 19:37:46 2024, max compression
```

## Comparing `geoseeq-0.5.6a9.tar` & `geoseeq-0.6.0.tar`

### file list

```diff
@@ -1,107 +1,111 @@
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 17:19:16.681753 geoseeq-0.5.6a9/
--rw-r--r--   0 dcdanko    (501) staff       (20)     1067 2023-02-09 21:51:44.000000 geoseeq-0.5.6a9/LICENSE
--rw-r--r--   0 dcdanko    (501) staff       (20)     4805 2024-04-05 17:19:16.681468 geoseeq-0.5.6a9/PKG-INFO
--rw-r--r--   0 dcdanko    (501) staff       (20)     4254 2023-10-24 18:48:30.000000 geoseeq-0.5.6a9/README.md
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 17:19:16.659236 geoseeq-0.5.6a9/geoseeq/
--rw-r--r--   0 dcdanko    (501) staff       (20)      946 2024-03-19 13:54:16.000000 geoseeq-0.5.6a9/geoseeq/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2387 2023-08-14 20:18:48.000000 geoseeq-0.5.6a9/geoseeq/app.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      188 2023-08-25 17:37:47.000000 geoseeq-0.5.6a9/geoseeq/blob_constructors.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2115 2023-07-05 19:40:08.000000 geoseeq-0.5.6a9/geoseeq/bulk_creators.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 17:19:16.663925 geoseeq-0.5.6a9/geoseeq/cli/
--rw-r--r--   0 dcdanko    (501) staff       (20)       24 2023-01-20 01:26:16.000000 geoseeq-0.5.6a9/geoseeq/cli/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      176 2023-01-20 01:26:16.000000 geoseeq-0.5.6a9/geoseeq/cli/constants.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2275 2024-02-05 19:19:37.000000 geoseeq-0.5.6a9/geoseeq/cli/copy.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4132 2024-02-05 19:19:37.000000 geoseeq-0.5.6a9/geoseeq/cli/detail.py
--rw-r--r--   0 dcdanko    (501) staff       (20)    17656 2024-03-19 02:18:54.000000 geoseeq-0.5.6a9/geoseeq/cli/download.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3083 2024-01-08 16:45:41.000000 geoseeq-0.5.6a9/geoseeq/cli/fastq_utils.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      997 2024-02-05 19:19:37.000000 geoseeq-0.5.6a9/geoseeq/cli/get_eula.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3259 2024-04-05 17:18:22.000000 geoseeq-0.5.6a9/geoseeq/cli/main.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     5929 2024-02-05 19:19:37.000000 geoseeq-0.5.6a9/geoseeq/cli/manage.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      738 2023-08-22 16:00:03.000000 geoseeq-0.5.6a9/geoseeq/cli/progress_bar.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3838 2024-02-05 19:19:37.000000 geoseeq-0.5.6a9/geoseeq/cli/run.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1015 2024-02-05 19:19:37.000000 geoseeq-0.5.6a9/geoseeq/cli/search.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 17:19:16.666206 geoseeq-0.5.6a9/geoseeq/cli/shared_params/
--rw-r--r--   0 dcdanko    (501) staff       (20)      325 2024-03-19 02:06:03.000000 geoseeq-0.5.6a9/geoseeq/cli/shared_params/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4095 2024-03-21 02:47:29.000000 geoseeq-0.5.6a9/geoseeq/cli/shared_params/common_state.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1072 2024-03-14 13:34:44.000000 geoseeq-0.5.6a9/geoseeq/cli/shared_params/config.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     9299 2024-03-19 02:05:53.000000 geoseeq-0.5.6a9/geoseeq/cli/shared_params/id_handlers.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2741 2023-08-22 14:05:04.000000 geoseeq-0.5.6a9/geoseeq/cli/shared_params/obj_getters.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2083 2024-04-05 17:01:58.000000 geoseeq-0.5.6a9/geoseeq/cli/shared_params/opts_and_args.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 17:19:16.667732 geoseeq-0.5.6a9/geoseeq/cli/upload/
--rw-r--r--   0 dcdanko    (501) staff       (20)      627 2024-03-18 18:33:30.000000 geoseeq-0.5.6a9/geoseeq/cli/upload/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     9203 2024-04-05 17:16:22.000000 geoseeq-0.5.6a9/geoseeq/cli/upload/upload.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3434 2023-11-09 22:36:49.000000 geoseeq-0.5.6a9/geoseeq/cli/upload/upload_advanced.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     7450 2024-04-05 17:17:32.000000 geoseeq-0.5.6a9/geoseeq/cli/upload/upload_reads.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      925 2023-02-10 03:32:14.000000 geoseeq-0.5.6a9/geoseeq/cli/user.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2873 2023-08-10 17:50:03.000000 geoseeq-0.5.6a9/geoseeq/cli/utils.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     6783 2024-02-05 19:19:37.000000 geoseeq-0.5.6a9/geoseeq/cli/view.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      431 2024-02-26 20:12:47.000000 geoseeq-0.5.6a9/geoseeq/constants.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 17:19:16.668064 geoseeq-0.5.6a9/geoseeq/contrib/
--rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-01-20 01:26:16.000000 geoseeq-0.5.6a9/geoseeq/contrib/__init__.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 17:19:16.669219 geoseeq-0.5.6a9/geoseeq/contrib/ncbi/
--rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-01-20 01:26:16.000000 geoseeq-0.5.6a9/geoseeq/contrib/ncbi/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1056 2023-02-09 21:51:44.000000 geoseeq-0.5.6a9/geoseeq/contrib/ncbi/api.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4341 2023-02-09 21:51:44.000000 geoseeq-0.5.6a9/geoseeq/contrib/ncbi/bioproject.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2400 2023-02-10 03:00:45.000000 geoseeq-0.5.6a9/geoseeq/contrib/ncbi/cli.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      175 2023-01-20 01:26:16.000000 geoseeq-0.5.6a9/geoseeq/contrib/ncbi/setup_logging.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4138 2024-04-05 15:21:33.000000 geoseeq-0.5.6a9/geoseeq/file_system_cache.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 17:19:16.671175 geoseeq-0.5.6a9/geoseeq/id_constructors/
--rw-r--r--   0 dcdanko    (501) staff       (20)      126 2023-08-25 17:28:11.000000 geoseeq-0.5.6a9/geoseeq/id_constructors/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     5702 2024-03-21 02:39:35.000000 geoseeq-0.5.6a9/geoseeq/id_constructors/from_blobs.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3151 2024-04-01 15:41:03.000000 geoseeq-0.5.6a9/geoseeq/id_constructors/from_ids.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4174 2024-02-26 20:07:19.000000 geoseeq-0.5.6a9/geoseeq/id_constructors/from_names.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3305 2024-02-26 20:08:43.000000 geoseeq-0.5.6a9/geoseeq/id_constructors/from_uuids.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2676 2024-02-26 20:08:58.000000 geoseeq-0.5.6a9/geoseeq/id_constructors/resolvers.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      723 2023-08-25 17:06:17.000000 geoseeq-0.5.6a9/geoseeq/id_constructors/utils.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     7898 2024-02-26 20:25:43.000000 geoseeq-0.5.6a9/geoseeq/knex.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2462 2023-07-05 19:40:08.000000 geoseeq-0.5.6a9/geoseeq/organization.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     9873 2023-11-19 15:30:12.000000 geoseeq-0.5.6a9/geoseeq/pipeline.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 17:19:16.672288 geoseeq-0.5.6a9/geoseeq/plotting/
--rw-r--r--   0 dcdanko    (501) staff       (20)      154 2023-08-25 16:47:04.000000 geoseeq-0.5.6a9/geoseeq/plotting/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      285 2023-08-23 12:02:35.000000 geoseeq-0.5.6a9/geoseeq/plotting/constants.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4096 2023-08-23 13:09:29.000000 geoseeq-0.5.6a9/geoseeq/plotting/highcharts.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 17:19:16.673343 geoseeq-0.5.6a9/geoseeq/plotting/map/
--rw-r--r--   0 dcdanko    (501) staff       (20)      295 2023-10-24 03:32:07.000000 geoseeq-0.5.6a9/geoseeq/plotting/map/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     4329 2023-10-24 03:21:34.000000 geoseeq-0.5.6a9/geoseeq/plotting/map/base_layer.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3907 2023-10-24 13:01:18.000000 geoseeq-0.5.6a9/geoseeq/plotting/map/map.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1795 2023-10-24 03:17:14.000000 geoseeq-0.5.6a9/geoseeq/plotting/map/overlay.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2554 2023-08-25 17:58:17.000000 geoseeq-0.5.6a9/geoseeq/plotting/selectable.py
--rw-r--r--   0 dcdanko    (501) staff       (20)    13741 2024-03-19 02:51:49.000000 geoseeq-0.5.6a9/geoseeq/project.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     7131 2024-04-02 19:52:31.000000 geoseeq-0.5.6a9/geoseeq/remote_object.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 17:19:16.675781 geoseeq-0.5.6a9/geoseeq/result/
--rw-r--r--   0 dcdanko    (501) staff       (20)      356 2023-08-10 17:50:03.000000 geoseeq-0.5.6a9/geoseeq/result/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     1782 2023-08-10 17:50:03.000000 geoseeq-0.5.6a9/geoseeq/result/bioinfo.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     5568 2024-04-02 20:04:55.000000 geoseeq-0.5.6a9/geoseeq/result/file_download.py
--rw-r--r--   0 dcdanko    (501) staff       (20)    11696 2024-04-05 17:15:32.000000 geoseeq-0.5.6a9/geoseeq/result/file_upload.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     8677 2024-04-05 17:13:21.000000 geoseeq-0.5.6a9/geoseeq/result/result_file.py
--rw-r--r--   0 dcdanko    (501) staff       (20)    11122 2024-03-18 21:38:47.000000 geoseeq-0.5.6a9/geoseeq/result/result_folder.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2772 2023-08-13 00:53:07.000000 geoseeq-0.5.6a9/geoseeq/result/utils.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     7981 2024-03-19 02:10:10.000000 geoseeq-0.5.6a9/geoseeq/sample.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3388 2023-10-05 16:43:42.000000 geoseeq-0.5.6a9/geoseeq/search.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     7423 2024-04-05 17:09:10.000000 geoseeq-0.5.6a9/geoseeq/upload_download_manager.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      690 2023-01-20 01:26:16.000000 geoseeq-0.5.6a9/geoseeq/user.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3577 2024-02-26 20:12:33.000000 geoseeq-0.5.6a9/geoseeq/utils.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 17:19:16.679529 geoseeq-0.5.6a9/geoseeq/vc/
--rw-r--r--   0 dcdanko    (501) staff       (20)        0 2023-02-10 03:25:58.000000 geoseeq-0.5.6a9/geoseeq/vc/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      710 2023-02-10 03:23:35.000000 geoseeq-0.5.6a9/geoseeq/vc/checksum.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2803 2023-08-25 17:39:54.000000 geoseeq-0.5.6a9/geoseeq/vc/cli.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     2486 2023-01-20 01:26:16.000000 geoseeq-0.5.6a9/geoseeq/vc/clone.py
--rw-r--r--   0 dcdanko    (501) staff       (20)       19 2023-01-20 01:26:16.000000 geoseeq-0.5.6a9/geoseeq/vc/constants.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      730 2023-01-20 01:26:16.000000 geoseeq-0.5.6a9/geoseeq/vc/vc_cache.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      457 2023-01-20 01:26:16.000000 geoseeq-0.5.6a9/geoseeq/vc/vc_dir.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3850 2023-08-25 17:41:01.000000 geoseeq-0.5.6a9/geoseeq/vc/vc_sample.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     3110 2023-08-25 17:40:12.000000 geoseeq-0.5.6a9/geoseeq/vc/vc_stub.py
--rw-r--r--   0 dcdanko    (501) staff       (20)     8071 2023-07-05 19:40:08.000000 geoseeq-0.5.6a9/geoseeq/work_orders.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 17:19:16.681161 geoseeq-0.5.6a9/geoseeq.egg-info/
--rw-r--r--   0 dcdanko    (501) staff       (20)     4805 2024-04-05 17:19:16.000000 geoseeq-0.5.6a9/geoseeq.egg-info/PKG-INFO
--rw-r--r--   0 dcdanko    (501) staff       (20)     2441 2024-04-05 17:19:16.000000 geoseeq-0.5.6a9/geoseeq.egg-info/SOURCES.txt
--rw-r--r--   0 dcdanko    (501) staff       (20)        1 2024-04-05 17:19:16.000000 geoseeq-0.5.6a9/geoseeq.egg-info/dependency_links.txt
--rw-r--r--   0 dcdanko    (501) staff       (20)       45 2024-04-05 17:19:16.000000 geoseeq-0.5.6a9/geoseeq.egg-info/entry_points.txt
--rw-r--r--   0 dcdanko    (501) staff       (20)       14 2024-04-05 17:19:16.000000 geoseeq-0.5.6a9/geoseeq.egg-info/top_level.txt
--rw-r--r--   0 dcdanko    (501) staff       (20)      643 2024-04-05 17:18:45.000000 geoseeq-0.5.6a9/pyproject.toml
--rw-r--r--   0 dcdanko    (501) staff       (20)       38 2024-04-05 17:19:16.681809 geoseeq-0.5.6a9/setup.cfg
--rw-r--r--   0 dcdanko    (501) staff       (20)      831 2024-04-05 17:19:10.000000 geoseeq-0.5.6a9/setup.py
-drwxr-xr-x   0 dcdanko    (501) staff       (20)        0 2024-04-05 17:19:16.680379 geoseeq-0.5.6a9/tests/
--rw-r--r--   0 dcdanko    (501) staff       (20)        0 2022-11-14 20:29:34.000000 geoseeq-0.5.6a9/tests/__init__.py
--rw-r--r--   0 dcdanko    (501) staff       (20)    12810 2023-10-24 13:59:25.000000 geoseeq-0.5.6a9/tests/test_api_client.py
--rw-r--r--   0 dcdanko    (501) staff       (20)      784 2023-10-24 13:03:13.000000 geoseeq-0.5.6a9/tests/test_plotting.py
+drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-04 19:37:46.030428 geoseeq-0.6.0/
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     1067 2023-03-22 01:07:34.000000 geoseeq-0.6.0/LICENSE
+-rw-r--r--   0 dcdanko   (1000) dcdanko   (1000)     4803 2024-05-04 19:37:46.030428 geoseeq-0.6.0/PKG-INFO
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     4254 2024-04-15 16:42:26.000000 geoseeq-0.6.0/README.md
+drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-04 19:37:46.030428 geoseeq-0.6.0/geoseeq/
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      946 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/__init__.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2387 2023-08-13 06:22:51.000000 geoseeq-0.6.0/geoseeq/app.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      188 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/blob_constructors.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2115 2023-06-14 19:17:52.000000 geoseeq-0.6.0/geoseeq/bulk_creators.py
+drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-04 19:37:46.030428 geoseeq-0.6.0/geoseeq/cli/
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)       24 2023-03-22 01:07:34.000000 geoseeq-0.6.0/geoseeq/cli/__init__.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      176 2023-03-22 01:07:34.000000 geoseeq-0.6.0/geoseeq/cli/constants.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2275 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/cli/copy.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     4132 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/cli/detail.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)    17766 2024-04-24 00:22:47.000000 geoseeq-0.6.0/geoseeq/cli/download.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3083 2023-03-22 01:07:34.000000 geoseeq-0.6.0/geoseeq/cli/fastq_utils.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      997 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/cli/get_eula.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3791 2024-05-04 19:36:40.000000 geoseeq-0.6.0/geoseeq/cli/main.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     5929 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/cli/manage.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      738 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/cli/progress_bar.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3030 2024-04-24 14:28:45.000000 geoseeq-0.6.0/geoseeq/cli/project.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     1884 2023-08-15 00:17:43.000000 geoseeq-0.6.0/geoseeq/cli/raw.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3838 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/cli/run.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     1015 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/cli/search.py
+drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-04 19:37:46.030428 geoseeq-0.6.0/geoseeq/cli/shared_params/
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      325 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/cli/shared_params/__init__.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     4095 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/cli/shared_params/common_state.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     1072 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/cli/shared_params/config.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     9299 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/cli/shared_params/id_handlers.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2741 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/cli/shared_params/obj_getters.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2083 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/cli/shared_params/opts_and_args.py
+drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-04 19:37:46.030428 geoseeq-0.6.0/geoseeq/cli/upload/
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      627 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/cli/upload/__init__.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)    10081 2024-05-04 19:25:40.000000 geoseeq-0.6.0/geoseeq/cli/upload/upload.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3434 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/cli/upload/upload_advanced.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)    10706 2024-05-04 18:41:04.000000 geoseeq-0.6.0/geoseeq/cli/upload/upload_reads.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      925 2023-03-22 01:07:34.000000 geoseeq-0.6.0/geoseeq/cli/user.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2873 2023-08-12 19:50:20.000000 geoseeq-0.6.0/geoseeq/cli/utils.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     6783 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/cli/view.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      431 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/constants.py
+drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-04 19:37:46.030428 geoseeq-0.6.0/geoseeq/contrib/
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)        0 2023-03-22 01:07:34.000000 geoseeq-0.6.0/geoseeq/contrib/__init__.py
+drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-04 19:37:46.030428 geoseeq-0.6.0/geoseeq/contrib/ncbi/
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)        0 2023-03-22 01:07:34.000000 geoseeq-0.6.0/geoseeq/contrib/ncbi/__init__.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     1056 2023-03-22 01:07:34.000000 geoseeq-0.6.0/geoseeq/contrib/ncbi/api.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     4341 2023-03-22 01:07:34.000000 geoseeq-0.6.0/geoseeq/contrib/ncbi/bioproject.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2400 2023-03-22 01:07:34.000000 geoseeq-0.6.0/geoseeq/contrib/ncbi/cli.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      175 2023-03-22 01:07:34.000000 geoseeq-0.6.0/geoseeq/contrib/ncbi/setup_logging.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     4138 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/file_system_cache.py
+drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-04 19:37:46.030428 geoseeq-0.6.0/geoseeq/id_constructors/
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      126 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/id_constructors/__init__.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     5702 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/id_constructors/from_blobs.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3151 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/id_constructors/from_ids.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     4174 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/id_constructors/from_names.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3305 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/id_constructors/from_uuids.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2676 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/id_constructors/resolvers.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      723 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/id_constructors/utils.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     7965 2024-04-15 16:42:46.000000 geoseeq-0.6.0/geoseeq/knex.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2462 2023-06-14 19:17:52.000000 geoseeq-0.6.0/geoseeq/organization.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     9873 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/pipeline.py
+drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-04 19:37:46.030428 geoseeq-0.6.0/geoseeq/plotting/
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      154 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/plotting/__init__.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      285 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/plotting/constants.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     4096 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/plotting/highcharts.py
+drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-04 19:37:46.030428 geoseeq-0.6.0/geoseeq/plotting/map/
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      295 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/plotting/map/__init__.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     4329 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/plotting/map/base_layer.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3907 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/plotting/map/map.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     1795 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/plotting/map/overlay.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2554 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/plotting/selectable.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)    13741 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/project.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     7131 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/remote_object.py
+drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-04 19:37:46.030428 geoseeq-0.6.0/geoseeq/result/
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      356 2023-08-12 19:50:20.000000 geoseeq-0.6.0/geoseeq/result/__init__.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     1782 2023-08-12 19:50:20.000000 geoseeq-0.6.0/geoseeq/result/bioinfo.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     1758 2024-05-03 02:52:42.000000 geoseeq-0.6.0/geoseeq/result/file_chunker.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     5790 2024-05-03 02:15:50.000000 geoseeq-0.6.0/geoseeq/result/file_download.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)    10648 2024-05-04 19:34:06.000000 geoseeq-0.6.0/geoseeq/result/file_upload.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     8677 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/result/result_file.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)    11122 2024-05-04 19:22:58.000000 geoseeq-0.6.0/geoseeq/result/result_folder.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3811 2024-05-04 19:09:33.000000 geoseeq-0.6.0/geoseeq/result/resumable_upload_tracker.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2772 2023-08-13 00:32:52.000000 geoseeq-0.6.0/geoseeq/result/utils.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     7981 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/sample.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3388 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/search.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     8751 2024-05-04 19:26:42.000000 geoseeq-0.6.0/geoseeq/upload_download_manager.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      690 2023-03-22 01:07:34.000000 geoseeq-0.6.0/geoseeq/user.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3577 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/utils.py
+drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-04 19:37:46.030428 geoseeq-0.6.0/geoseeq/vc/
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)        0 2023-03-22 01:07:34.000000 geoseeq-0.6.0/geoseeq/vc/__init__.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      710 2023-03-22 01:07:34.000000 geoseeq-0.6.0/geoseeq/vc/checksum.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2803 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/vc/cli.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2486 2023-03-22 01:07:34.000000 geoseeq-0.6.0/geoseeq/vc/clone.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)       19 2023-03-22 01:07:34.000000 geoseeq-0.6.0/geoseeq/vc/constants.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      730 2023-03-22 01:07:34.000000 geoseeq-0.6.0/geoseeq/vc/vc_cache.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      457 2023-03-22 01:07:34.000000 geoseeq-0.6.0/geoseeq/vc/vc_dir.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3850 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/vc/vc_sample.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     3110 2024-04-15 16:42:26.000000 geoseeq-0.6.0/geoseeq/vc/vc_stub.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     8071 2023-06-14 19:17:52.000000 geoseeq-0.6.0/geoseeq/work_orders.py
+drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-04 19:37:46.030428 geoseeq-0.6.0/geoseeq.egg-info/
+-rw-r--r--   0 dcdanko   (1000) dcdanko   (1000)     4803 2024-05-04 19:37:46.000000 geoseeq-0.6.0/geoseeq.egg-info/PKG-INFO
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)     2557 2024-05-04 19:37:46.000000 geoseeq-0.6.0/geoseeq.egg-info/SOURCES.txt
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)        1 2024-05-04 19:37:46.000000 geoseeq-0.6.0/geoseeq.egg-info/dependency_links.txt
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)       45 2024-05-04 19:37:46.000000 geoseeq-0.6.0/geoseeq.egg-info/entry_points.txt
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)       14 2024-05-04 19:37:46.000000 geoseeq-0.6.0/geoseeq.egg-info/top_level.txt
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      641 2024-05-04 19:36:50.000000 geoseeq-0.6.0/pyproject.toml
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)       38 2024-05-04 19:37:46.030428 geoseeq-0.6.0/setup.cfg
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      831 2024-04-15 16:42:26.000000 geoseeq-0.6.0/setup.py
+drwxrwxr-x   0 dcdanko   (1000) dcdanko   (1000)        0 2024-05-04 19:37:46.030428 geoseeq-0.6.0/tests/
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)        0 2022-11-29 19:57:49.000000 geoseeq-0.6.0/tests/__init__.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)    12810 2024-04-15 16:42:26.000000 geoseeq-0.6.0/tests/test_api_client.py
+-rw-rw-r--   0 dcdanko   (1000) dcdanko   (1000)      784 2024-04-15 16:42:26.000000 geoseeq-0.6.0/tests/test_plotting.py
```

### Comparing `geoseeq-0.5.6a9/LICENSE` & `geoseeq-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/PKG-INFO` & `geoseeq-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoseeq
-Version: 0.5.6a9
+Version: 0.6.0
 Summary: GeoSeeq command line tools and python API
 Author: David C. Danko
 Author-email: "David C. Danko" <dcdanko@biotia.io>
 Project-URL: Homepage, https://github.com/biotia/geoseeq_api_client
 Project-URL: Issues, https://github.com/biotia/geoseeq_api_client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geoseeq-0.5.6a9/README.md` & `geoseeq-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/__init__.py` & `geoseeq-0.6.0/geoseeq/__init__.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/app.py` & `geoseeq-0.6.0/geoseeq/app.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/bulk_creators.py` & `geoseeq-0.6.0/geoseeq/bulk_creators.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/cli/copy.py` & `geoseeq-0.6.0/geoseeq/cli/copy.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/cli/detail.py` & `geoseeq-0.6.0/geoseeq/cli/detail.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/cli/download.py` & `geoseeq-0.6.0/geoseeq/cli/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,21 +93,22 @@
         metadata[sample.name] = sample.metadata
     metadata = pd.DataFrame.from_dict(metadata, orient="index")
     metadata.to_csv(state.outfile)
     click.echo("Metadata successfully downloaded for samples.", err=True)
 
 
 cores_option = click.option('--cores', default=1, help='Number of downloads to run in parallel')
-
+head_option = click.option('--head', default=None, type=int, help='Download the first N bytes of each file')
 
 @cli_download.command("files")
 @use_common_state
 @cores_option
 @click.option("--target-dir", default=".")
 @yes_option
+@head_option
 @click.option("--download/--urls-only", default=True, help="Download files or just print urls")
 @click.option("--folder-type", type=click.Choice(['all', 'sample', 'project'], case_sensitive=False), default="all", help='Download files from sample folders, project folders, or both')
 @click.option("--folder-name", multiple=True, help='Filter folders for names that include this string. Case insensitive.')
 @click.option("--sample-name-includes", multiple=True, help='Filter samples for names that include this string. Case insensitive.')
 @click.option("--file-name", multiple=True, help="Filter files for names that include this string. Case insensitive.")
 @click.option("--extension", multiple=True, help="Only download files with this extension. e.g. 'fastq.gz', 'bam', 'csv'")
 @click.option("--with-versions/--without-versions", default=False, help="Download all versions of a file, not just the latest")
@@ -116,14 +117,15 @@
 @sample_ids_arg
 def cli_download_files(
     state,
     cores,
     sample_name_includes,
     target_dir,
     yes,
+    head,
     folder_type,
     folder_name,
     file_name,
     extension,
     with_versions,
     download,
     ignore_errors,
@@ -209,14 +211,15 @@
             click.confirm(f'Do you want to download {len(response["links"])} files?', abort=True)
 
         download_manager = GeoSeeqDownloadManager(
             n_parallel_downloads=cores,
             ignore_errors=ignore_errors,
             log_level=state.log_level,
             progress_tracker_factory=PBarManager().get_new_bar,
+            head=head,
         )
         for fname, url in response["links"].items():
             download_manager.add_download(url, join(target_dir, fname))
         
         click.echo(download_manager.get_preview_string(), err=True)
         if not yes:
             click.confirm('Continue?', abort=True)
@@ -226,19 +229,20 @@
 
 
 @cli_download.command("folders")
 @use_common_state
 @cores_option
 @click.option("-t", "--target-dir", default=".")
 @yes_option
+@head_option
 @click.option("--download/--urls-only", default=True, help="Download files or just print urls")
 @ignore_errors_option
 @click.option('--hidden/--no-hidden', default=True, help='Download hidden files in folder')
 @folder_ids_arg
-def cli_download_folders(state, cores, target_dir, yes, download, ignore_errors, hidden, folder_ids):
+def cli_download_folders(state, cores, target_dir, yes, head, download, ignore_errors, hidden, folder_ids):
     """Download entire folders from GeoSeeq.
     
     This command downloads folders directly based on their ID. This is used for "manual"
     downloads of GeoSeeq folders.
 
     ---
 
@@ -263,14 +267,15 @@
         handle_folder_id(knex, folder_id, create=False) for folder_id in folder_ids
     ]
     download_manager = GeoSeeqDownloadManager(
         n_parallel_downloads=cores,
         ignore_errors=ignore_errors,
         log_level=state.log_level,
         progress_tracker_factory=PBarManager().get_new_bar,
+        head=head,
     )
     for result_folder in result_folders:
         download_manager.add_result_folder_download(
             result_folder, join(target_dir, result_folder.name), hidden_files=hidden
         )
     click.echo(download_manager.get_preview_string(), err=True)
     if not yes:
@@ -282,15 +287,15 @@
 @cli_download.command("ids")
 @use_common_state
 @cores_option
 @click.option("--target-dir", default=".")
 @click.option("-n", "--file-name", multiple=True, help="File name to use for downloaded files. If set you must specify once per ID.")
 @yes_option
 @click.option("--download/--urls-only", default=True, help="Download files or just print urls")
-@click.option('--head', default=None, type=int, help='Download the first N bytes of each file')
+@head_option
 @ignore_errors_option
 @click.argument("ids", nargs=-1)
 def cli_download_ids(state, cores, target_dir, file_name, yes, download, head, ignore_errors, ids):
     """Download a files from GeoSeeq based on their UUID or GeoSeeq Resource Number (GRN).
 
     This command downloads files directly based on their ID. This is used for "manual"
     downloads of relatively small amounts of data. For bulk downloads, use the
@@ -459,7 +464,8 @@
         print(download_manager.get_url_string(), file=state.outfile)
     else:
         click.echo(download_manager.get_preview_string(), err=True)
         if not yes:
             click.confirm('Continue?', abort=True)
         logger.info(f'Downloading {len(download_manager)} files to {target_dir}')
         download_manager.download_files()
+
```

### Comparing `geoseeq-0.5.6a9/geoseeq/cli/fastq_utils.py` & `geoseeq-0.6.0/geoseeq/cli/fastq_utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/cli/get_eula.py` & `geoseeq-0.6.0/geoseeq/cli/get_eula.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/cli/main.py` & `geoseeq-0.6.0/geoseeq/cli/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from geoseeq.vc.cli import cli_vc
 from geoseeq.knex import DEFAULT_ENDPOINT
 from geoseeq.utils import set_profile
 from .shared_params.opts_and_args import overwrite_option, yes_option
 from .detail import cli_detail
 from .run import cli_app
 from .get_eula import cli_eula
+from .project import cli_project
 
 logger = logging.getLogger('geoseeq_api')
 handler = logging.StreamHandler()
 handler.setFormatter(logging.Formatter('[%(levelname)s] %(name)s :: %(message)s'))
 logger.addHandler(handler)
 
 
@@ -49,26 +50,27 @@
     """Print the version of the Geoseeq API being used.
 
     ---
     
     Use of this tool implies acceptance of the GeoSeeq End User License Agreement.
     Run `geoseeq eula show` to view the EULA.
     """
-    click.echo('0.5.6a9')  # remember to update setup
+    click.echo('0.6.0')  # remember to update setup
 
 
 @main.group('advanced')
 def cli_advanced():
     """Advanced commands."""
     pass
 
 cli_advanced.add_command(cli_copy)
 cli_advanced.add_command(cli_user)
 cli_advanced.add_command(cli_detail)
 cli_advanced.add_command(cli_upload_advanced)
+cli_advanced.add_command(cli_project)
 
 @cli_advanced.group('experimental')
 def cli_experimental():
     """Experimental commands."""
     pass
 
 cli_experimental.add_command(cli_vc)
@@ -97,8 +99,24 @@
         api_token = click.prompt(f'Enter your GeoSeeq API token', hide_input=True).strip(' \"\'')
     if not yes:
         eula_accepted = click.confirm(f'Have you read and accepted the GeoSeeq End User License Agreement? Use `geoseeq eula show` to view the EULA.')
         if not eula_accepted:
             click.echo('You must accept the EULA to use the GeoSeeq API.')
             return
     set_profile(api_token, endpoint=endpoint, profile=profile, overwrite=overwrite)
-    click.echo(f'Profile configured.')
+    click.echo(f'Profile configured.')
+
+
+@main.command('clear-cache')
+@yes_option
+def cli_clear_cache(yes):
+    """Clear the local cache.
+
+    ---
+    
+    Use of this tool implies acceptance of the GeoSeeq End User License Agreement.
+    Run `geoseeq eula show` to view the EULA.
+    """
+    from geoseeq.file_system_cache import GEOSEEQ_CACHE_DIR
+    import shutil
+    if yes or click.confirm('Are you sure you want to clear the cache?'):
+        shutil.rmtree(GEOSEEQ_CACHE_DIR, ignore_errors=True)
```

### Comparing `geoseeq-0.5.6a9/geoseeq/cli/manage.py` & `geoseeq-0.6.0/geoseeq/cli/manage.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/cli/progress_bar.py` & `geoseeq-0.6.0/geoseeq/cli/progress_bar.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/cli/run.py` & `geoseeq-0.6.0/geoseeq/cli/run.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/cli/search.py` & `geoseeq-0.6.0/geoseeq/cli/search.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/cli/shared_params/common_state.py` & `geoseeq-0.6.0/geoseeq/cli/shared_params/common_state.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/cli/shared_params/config.py` & `geoseeq-0.6.0/geoseeq/cli/shared_params/config.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/cli/shared_params/id_handlers.py` & `geoseeq-0.6.0/geoseeq/cli/shared_params/id_handlers.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/cli/shared_params/obj_getters.py` & `geoseeq-0.6.0/geoseeq/cli/shared_params/obj_getters.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/cli/shared_params/opts_and_args.py` & `geoseeq-0.6.0/geoseeq/cli/shared_params/opts_and_args.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/cli/upload/__init__.py` & `geoseeq-0.6.0/geoseeq/cli/upload/__init__.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/cli/upload/upload.py` & `geoseeq-0.6.0/geoseeq/cli/upload/upload.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,37 +21,43 @@
     handle_folder_id,
     overwrite_option,
     project_id_arg,
     handle_project_id,
     project_or_sample_id_arg,
     handle_project_or_sample_id,
     no_new_versions_option,
+    ignore_errors_option,
 )
 from geoseeq.upload_download_manager import GeoSeeqUploadManager
 
 logger = logging.getLogger('geoseeq_api')
 
 recursive_option = click.option('--recursive/--no-recursive', default=True, help='Upload files in subfolders')
 hidden_option = click.option('--hidden/--no-hidden', default=False, help='Upload hidden files in subfolders')
 
 
 @click.command('files')
 @use_common_state
-@click.option('--cores', default=1, help='Number of uploads to run in parallel')
+@click.option('--cores', default=1, help='Number of uploads to run in parallel', show_default=True)
+@click.option('--threads-per-upload', default=4, help='Number of threads used to upload each file', show_default=True)
+@click.option('--num-retries', default=3, help='Number of times to retry a failed upload', show_default=True)
+@click.option('--chunk-size-mb', default=-1, help='Size of chunks to upload in MB', show_default=True)
+@ignore_errors_option
 @yes_option
 @private_option
 @link_option
 @recursive_option
 @hidden_option
 @no_new_versions_option
 @click.option('-n', '--geoseeq-file-name', default=None, multiple=True,
-              help='Specify a different name for the file on GeoSeeq than the local file name.')
+              help='Specify a different name for the file on GeoSeeq than the local file name.',
+              show_default=True)
 @folder_id_arg
 @click.argument('file_paths', type=click.Path(exists=True), nargs=-1)
-def cli_upload_file(state, cores, yes, private, link_type, recursive, hidden, no_new_versions, geoseeq_file_name, folder_id, file_paths):
+def cli_upload_file(state, cores, threads_per_upload, num_retries, chunk_size_mb, ignore_errors, yes, private, link_type, recursive, hidden, no_new_versions, geoseeq_file_name, folder_id, file_paths):
     """Upload files to GeoSeeq.
 
     This command uploads files to either a sample or project on GeoSeeq. It can be used to upload
     multiple files to the same folder at once.
     
     ---
 
@@ -88,33 +94,41 @@
     names for an org, project, sample, folder separated by a slash. Can exclude
     the sample name if the folder is for a project.
 
     [FILE_PATHS]... One or more paths to files on your local machine.
 
     ---
     """
+    if num_retries < 1:
+        raise click.UsageError('--num-retries must be at least 1')
     knex = state.get_knex()
     result_folder = handle_folder_id(knex, folder_id, yes=yes, private=private, create=True)
     if geoseeq_file_name:
         uploading_folders = sum([isdir(fp) for fp in file_paths])
         if uploading_folders:
             raise click.UsageError('Cannot use --geoseeq-file-name with recursive folder uploads')
         if len(geoseeq_file_name) != len(file_paths):
             raise click.UsageError('Number of --geoseeq-file-name arguments must match number of file_paths')
         name_pairs = zip(geoseeq_file_name, file_paths)
     else:
         name_pairs = zip([basename(fp) for fp in file_paths], file_paths)
     
     upload_manager = GeoSeeqUploadManager(
         n_parallel_uploads=cores,
+        threads_per_upload=threads_per_upload,
         link_type=link_type,
         progress_tracker_factory=PBarManager().get_new_bar,
         log_level=state.log_level,
         no_new_versions=no_new_versions,
         use_cache=state.use_cache,
+        num_retries=num_retries,
+        ignore_errors=ignore_errors,
+        use_atomic_upload=True,
+        session=None, #knex.new_session(),
+        chunk_size_mb=chunk_size_mb if chunk_size_mb > 0 else None,
     )
     for geoseeq_file_name, file_path in name_pairs:
         if isfile(file_path):
             upload_manager.add_local_file_to_result_folder(result_folder, file_path)
         elif isdir(file_path) and recursive:
             upload_manager.add_local_folder_to_result_folder(result_folder, file_path, recursive=recursive, hidden_files=hidden, prefix=file_path)
         elif isdir(file_path) and not recursive:
@@ -143,14 +157,15 @@
         n_parallel_uploads=cores,
         link_type='upload',
         progress_tracker_factory=PBarManager().get_new_bar,
         log_level=logging.INFO,
         overwrite=True,
         use_cache=state.use_cache,
         no_new_versions=no_new_versions,
+        use_atomic_upload=True,
     )
     for folder_name in folder_names:
         result_folder = root_obj.result_folder(folder_name).idem()
         upload_manager.add_local_folder_to_result_folder(result_folder, folder_name, recursive=recursive, hidden_files=hidden)
     click.echo(upload_manager.get_preview_string(), err=True)
     if not yes:
         click.confirm('Continue?', abort=True)
```

### Comparing `geoseeq-0.5.6a9/geoseeq/cli/upload/upload_advanced.py` & `geoseeq-0.6.0/geoseeq/cli/upload/upload_advanced.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/cli/upload/upload_reads.py` & `geoseeq-0.6.0/geoseeq/cli/upload/upload_reads.py`

 * *Files 18% similar despite different names*

```diff
@@ -94,14 +94,15 @@
             session=session,
             link_type=link_type,
             log_level=state.log_level,
             overwrite=overwrite,
             progress_tracker_factory=PBarManager().get_new_bar,
             use_cache=state.use_cache,
             no_new_versions=no_new_versions,
+            use_atomic_upload=True,
         )
         for group in groups:
             sample = lib.sample(group['sample_name']).idem()
             read_folder = sample.result_folder(module_name).idem()
             for field_name, path in group['fields'].items():
                 result_file = read_folder.read_file(field_name)
                 upload_manager.add_result_file(result_file, filepaths[path])
@@ -128,14 +129,36 @@
                 for line in f:
                     line = line.strip()
                     if line and not line.startswith('#'):
                         flattened.append(line)
     return flattened
 
 
+def _is_bam(path):
+    for ext in ['.bam', '.bai']:
+        if path.endswith(ext):
+            return True
+    return False
+
+
+def flatten_list_of_bams(filepaths):
+    """Turn a list of bam filepaths and txt files containing bam filepaths into a single list of bam filepaths."""
+    flattened = []
+    for path in filepaths:
+        if _is_bam(path):
+            flattened.append(path)
+        else:
+            with open(path) as f:
+                for line in f:
+                    line = line.strip()
+                    if line and not line.startswith('#'):
+                        flattened.append(line)
+    return flattened
+
+
 
 @click.command('reads')
 @use_common_state
 @click.option('--cores', default=1, help='Number of uploads to run in parallel')
 @overwrite_option
 @yes_option
 @click.option('--regex', default=None, help='An optional regex to use to extract sample names from the file names')
@@ -196,7 +219,71 @@
     knex = state.get_knex()
     proj = handle_project_id(knex, project_id, yes, private)
     filepaths = {basename(line): line for line in flatten_list_of_fastqs(fastq_files)}
     click.echo(f'Found {len(filepaths)} files to upload.', err=True)
     regex = _get_regex(knex, filepaths, module_name, proj, regex)
     groups = _group_files(knex, filepaths, module_name, regex, yes)
     _do_upload(groups, module_name, link_type, proj, filepaths, overwrite, no_new_versions, cores, state)
+
+
+# @click.command('bam')
+# @use_common_state
+# @click.option('--genome', default=None, help='The genome aligned to the BAM files. Should be in 2bit format.')
+# @click.option('--cores', default=1, help='Number of uploads to run in parallel')
+# @overwrite_option
+# @yes_option
+# @click.option('--regex', default=None, help='An optional regex to use to extract sample names from the file names')
+# @private_option
+# @link_option
+# @no_new_versions_option
+# @project_id_arg
+# @click.argument('files', type=click.Path(exists=True), nargs=-1)
+# def cli_upload_bams(state, genome, cores, overwrite, yes, regex, private, link_type, no_new_versions, project_id, files):
+    """Upload BAM files to GeoSeeq.
+
+    This command automatically groups bams with their index files.
+
+    ---
+
+    Example Usage:
+
+    \b
+    # Upload a list of BAM files to a project, useful if you have hundreds of files
+    $ ls -1 path/to/bam/files/*.bam > file_list.txt
+    $ geoseeq upload bams "GeoSeeq/Example CLI Project" file_list.txt
+
+    \b
+    # Upload all the BAM files in a directory to a project with BAM indexes
+    $ geoseeq upload bams ed59b913-91ec-489b-a1b9-4ea137a6e5cf path/to/bam/files/*.bam path/to/bam/files/*.bam.bai
+
+    \b
+    # Upload all the BAM files in a directory to a project, performing 4 uploads in parallel
+    $ geoseeq upload bams --cores 4 ed59b913-91ec-489b-a1b9-4ea137a6e5cf path/to/bam/files/*.bam
+
+    \b
+    # Upload a list of BAM files to a project, automatically creating a new project and overwriting existing files
+    $ ls -1 path/to/bam/files/*.bam > file_list.txt
+    $ geoseeq upload bams --yes --overwrite "GeoSeeq/Example CLI Project" file_list.txt
+
+    ---
+
+    Command Arguments:
+    
+    [PROJECT_ID] Can be a project UUID, GeoSeeq Resource Number (GRN), or an
+    organization name and project name separated by a slash.
+
+    \b
+    Examples: 
+     - Name pair: "GeoSeeq/Example CLI Project"
+     - UUID: "ed59b913-91ec-489b-a1b9-4ea137a6e5cf"
+     - GRN: "grn:gs1:project:ed59b913-91ec-489b-a1b9-4ea137a6e5cf"
+
+    \b
+    [FILES...] can be paths to BAM files or a file containing a list of paths, or a mix of both.
+    Example: "path/to/bam/files
+    """
+    knex = state.get_knex()
+    proj = handle_project_id(knex, project_id, yes, private)
+    filepaths = {basename(line): line for line in flatten_list_of_bams(files)}
+    click.echo(f'Found {len(filepaths)} files to upload.', err=True)
+    groups = _group_files(knex, filepaths, 'bam::bam', regex, yes)
+    _do_upload(groups, 'bam::bam', link_type, proj, filepaths, overwrite, no_new_versions, cores, state)
```

### Comparing `geoseeq-0.5.6a9/geoseeq/cli/user.py` & `geoseeq-0.6.0/geoseeq/cli/user.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/cli/utils.py` & `geoseeq-0.6.0/geoseeq/cli/utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/cli/view.py` & `geoseeq-0.6.0/geoseeq/cli/view.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/contrib/ncbi/api.py` & `geoseeq-0.6.0/geoseeq/contrib/ncbi/api.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/contrib/ncbi/bioproject.py` & `geoseeq-0.6.0/geoseeq/contrib/ncbi/bioproject.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/contrib/ncbi/cli.py` & `geoseeq-0.6.0/geoseeq/contrib/ncbi/cli.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/file_system_cache.py` & `geoseeq-0.6.0/geoseeq/file_system_cache.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/id_constructors/from_blobs.py` & `geoseeq-0.6.0/geoseeq/id_constructors/from_blobs.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/id_constructors/from_ids.py` & `geoseeq-0.6.0/geoseeq/id_constructors/from_ids.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/id_constructors/from_names.py` & `geoseeq-0.6.0/geoseeq/id_constructors/from_names.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/id_constructors/from_uuids.py` & `geoseeq-0.6.0/geoseeq/id_constructors/from_uuids.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/id_constructors/resolvers.py` & `geoseeq-0.6.0/geoseeq/id_constructors/resolvers.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/id_constructors/utils.py` & `geoseeq-0.6.0/geoseeq/id_constructors/utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/knex.py` & `geoseeq-0.6.0/geoseeq/knex.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,17 @@
         if hasattr(self, 'sess') and self.sess:
             self.sess.close()
         sess = requests.Session()
         sess.headers = self.headers
         sess.auth = self.auth
         sess.verify = self._verify
         return sess
+    
+    def new_session(self):
+        return self._new_session()
 
     def _set_verify(self):
         try:
             val = environ['GEOSEEQ_NO_SSL_VERIFICATION']
             if val.lower() == 'true':
                 return False
             if val.lower() == 'false':
```

### Comparing `geoseeq-0.5.6a9/geoseeq/organization.py` & `geoseeq-0.6.0/geoseeq/organization.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/pipeline.py` & `geoseeq-0.6.0/geoseeq/pipeline.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/plotting/highcharts.py` & `geoseeq-0.6.0/geoseeq/plotting/highcharts.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/plotting/map/base_layer.py` & `geoseeq-0.6.0/geoseeq/plotting/map/base_layer.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/plotting/map/map.py` & `geoseeq-0.6.0/geoseeq/plotting/map/map.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/plotting/map/overlay.py` & `geoseeq-0.6.0/geoseeq/plotting/map/overlay.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/plotting/selectable.py` & `geoseeq-0.6.0/geoseeq/plotting/selectable.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/project.py` & `geoseeq-0.6.0/geoseeq/project.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/remote_object.py` & `geoseeq-0.6.0/geoseeq/remote_object.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/result/bioinfo.py` & `geoseeq-0.6.0/geoseeq/result/bioinfo.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/result/file_download.py` & `geoseeq-0.6.0/geoseeq/result/file_download.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 
 from geoseeq.utils import download_ftp
 from geoseeq.constants import FIVE_MB
 
 logger = logging.getLogger("geoseeq_api")  # Same name as calling module
 
 
-def _download_head(url, filename, head=None, progress_tracker=None):
+def _download_head(url, filename, head=None, start=0, progress_tracker=None):
     headers = None
     if head and head > 0:
-        headers = {"Range": f"bytes=0-{head}"}
+        headers = {"Range": f"bytes={start}-{head}"}
     response = requests.get(url, stream=True, headers=headers)
     response.raise_for_status()
     total_size_in_bytes = int(response.headers.get('content-length', 0))
     if progress_tracker: progress_tracker.set_num_chunks(total_size_in_bytes)
     block_size = FIVE_MB
     with open(filename, 'wb') as file:
         for data in response.iter_content(block_size):
@@ -42,14 +42,19 @@
         return 'ftp'
     else:
         return 'generic'
 
 
 def download_url(url, kind='guess', filename=None, head=None, progress_tracker=None):
     """Return a local filepath to the downloaded file. Download the file."""
+    if filename and isfile(filename):
+        file_size = getsize(filename)
+        if file_size > 0:
+            logger.info(f"File already exists: {filename}. Not overwriting.")
+            return filename
     if kind == 'guess':
         kind = guess_download_kind(url)
         logger.info(f"Guessed download kind: {kind} for {url}")
     logger.info(f"Downloading {kind} file to {filename}")
     if kind == 'generic':
         return _download_generic(url, filename, head=head)
     elif kind == 's3':
@@ -58,15 +63,14 @@
         return _download_head(url, filename, head=head)
     elif kind == 'ftp':
         return download_ftp(url, filename, head=head)
     else:
         raise ValueError(f"Unknown download kind: {kind}")
 
 
-
 class ResultFileDownload:
     """Abstract class that handles download methods for result files."""
 
     def get_download_url(self):
         """Return a URL that can be used to download the file for this result."""
         blob_type = self.stored_data.get("__type__", "").lower()
         if blob_type not in ["s3", "sra", "ftp", "azure"]:
```

### Comparing `geoseeq-0.5.6a9/geoseeq/result/file_upload.py` & `geoseeq-0.6.0/geoseeq/result/file_upload.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,195 +1,123 @@
 
 import time
 import json
 import os
-from os.path import basename, getsize, join, dirname, isfile
+from os.path import basename, getsize, join, dirname, isfile, getctime
 from pathlib import Path
-
+from random import random
 import requests
 
 from geoseeq.knex import GeoseeqGeneralError
 from geoseeq.constants import FIVE_MB
 from geoseeq.utils import md5_checksum
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from .utils import *
 from geoseeq.file_system_cache import GEOSEEQ_CACHE_DIR
-
-class FileChunker:
-
-    def __init__(self, filepath, chunk_size):
-        self.filepath = filepath
-        self.chunk_size = chunk_size
-        self.file_size = getsize(filepath)
-        self.n_parts = int(self.file_size / self.chunk_size) + 1
-        self.loaded_parts = []
-
-    def load_all_chunks(self):
-        if len(self.loaded_parts) != self.n_parts:
-            with open(self.filepath, "rb") as f:
-                f.seek(0)
-                for i in range(self.n_parts):
-                    chunk = f.read(self.chunk_size)
-                    self.loaded_parts.append(chunk)
-        return self  # convenience for chaining
-
-    def get_chunk(self, num):
-        self.load_all_chunks()
-        return self.loaded_parts[num]
-    
-    def get_chunk_size(self, num):
-        self.load_all_chunks()
-        return len(self.loaded_parts[num])
-    
-
-class ResumableUploadTracker:
-
-    def __init__(self, filepath, chunk_size, tracker_file_prefix="gs_resumable_upload_tracker"):
-        self.open, self.upload_started = True, False
-        self.upload_id, self.urls = None, None
-        self.filepath = filepath
-        self.tracker_file = join(
-            GEOSEEQ_CACHE_DIR, 'upload',
-            tracker_file_prefix + f".{chunk_size}." + basename(filepath)
-        )
-        try:
-            os.makedirs(dirname(self.tracker_file), exist_ok=True)
-        except Exception as e:
-            logger.warning(f'Could not create resumable upload tracker directory. {e}')
-            self.open = False
-        self._loaded_parts = {}
-        self._load_parts_from_file()
-
-    def start_upload(self, upload_id, urls):
-        if not self.open:
-            return
-        if self.upload_started:
-            raise GeoseeqGeneralError("Upload has already started.")
-        blob = dict(upload_id=upload_id, urls=urls)
-        serialized = json.dumps(blob)
-        with open(self.tracker_file, "w") as f:
-            f.write(serialized + "\n")
-        self.upload_id, self.urls = upload_id, urls
-        self.upload_started = True
-    
-    def add_part(self, part_upload_info):
-        if not self.open:
-            return
-        part_id = part_upload_info["PartNumber"]
-        serialized = json.dumps(part_upload_info)
-        with open(self.tracker_file, "a") as f:
-            f.write(serialized + "\n")
-        self._loaded_parts[part_id] = part_upload_info
-        if len(self._loaded_parts) == len(self.urls):
-            self.cleanup()
-            self.open = False
-    
-    def _load_parts_from_file(self):
-        if not isfile(self.tracker_file):
-            return
-        with open(self.tracker_file, "r") as f:
-            header_blob = json.loads(f.readline())
-            self.upload_id, self.urls = header_blob["upload_id"], header_blob["urls"]
-            self.upload_started = True
-            for line in f:
-                blob = json.loads(line)
-                part_id = blob["PartNumber"]
-                self._loaded_parts[part_id] = blob
-    
-    def part_has_been_uploaded(self, part_number):
-        if not self.open:
-            return False
-        return part_number in self._loaded_parts
-    
-    def get_part_info(self, part_number):
-        return self._loaded_parts[part_number]
-    
-    def cleanup(self):
-        if not self.open:
-            return
-        try:
-            os.remove(self.tracker_file)
-        except FileNotFoundError:
-            pass
+from .file_chunker import FileChunker
+from .resumable_upload_tracker import ResumableUploadTracker
 
 
 class ResultFileUpload:
     """Abstract class that handles upload methods for result files."""
 
-    def _create_multipart_upload(self, filepath, file_size, optional_fields):
+    def _result_type(self, atomic=False):
+        if self.is_sample_result:
+            return "sample"
+        if atomic:
+            return "project"
+        return "group"
+
+    def _create_multipart_upload(self, filepath, file_size, optional_fields, atomic=False):
         optional_fields = optional_fields if optional_fields else {}
         optional_fields.update(
             {
                 "md5_checksum": md5_checksum(filepath),
                 "file_size_bytes": file_size,
             }
         )
         data = {
             "filename": basename(filepath),
             "optional_fields": optional_fields,
-            "result_type": "sample" if self.is_sample_result else "group",
+            "result_type": self._result_type(atomic),
         }
-        response = self.knex.post(f"/ar_fields/{self.uuid}/create_upload", json=data)
+        url = f"/ar_fields/{self.uuid}/create_upload"
+        if atomic:
+            data["fieldname"] = self.name
+            url = f"/ars/{self.parent.uuid}/create_atomic_upload"
+        response = self.knex.post(url, json=data)
         return response
     
-    def _prep_multipart_upload(self, filepath, file_size, chunk_size, optional_fields):
+    def _prep_multipart_upload(self, filepath, file_size, chunk_size, optional_fields, atomic=False):
         n_parts = int(file_size / chunk_size) + 1
-        response = self._create_multipart_upload(filepath, file_size, optional_fields)
+        response = self._create_multipart_upload(filepath, file_size, optional_fields, atomic=atomic)
         upload_id = response["upload_id"]
-        parts = list(range(1, n_parts + 1))
         data = {
-            "parts": parts,
+            "parts": list(range(1, n_parts + 1)),
             "stance": "upload-multipart",
             "upload_id": upload_id,
-            "result_type": "sample" if self.is_sample_result else "group",
+            "result_type": self._result_type(atomic),
         }
-        response = self.knex.post(f"/ar_fields/{self.uuid}/create_upload_urls", json=data)
+        url = f"/ar_fields/{self.uuid}/create_upload_urls"
+        if atomic:
+            data["uuid"] = response["uuid"]
+            data["fieldname"] = self.name
+            url = f"ars/{self.parent.uuid}/create_atomic_upload_urls"
+        response = self.knex.post(url, json=data)
         urls = response
         return upload_id, urls
     
     def _upload_one_part(self, file_chunker, url, num, max_retries, session=None, resumable_upload_tracker=None):
         if resumable_upload_tracker and resumable_upload_tracker.part_has_been_uploaded(num + 1):
             logger.info(f"Part {num + 1} has already been uploaded. Skipping.")
             return resumable_upload_tracker.get_part_info(num + 1)
         file_chunk = file_chunker.get_chunk(num)
         attempts = 0
         while attempts < max_retries:
             try:
+                # url = url.replace("s3.wasabisys.com", "s3.us-east-1.wasabisys.com")
+                logger.debug(f"Uploading part {num + 1} to {url}. Size: {len(file_chunk)} bytes.")
                 if session:
                     http_response = session.put(url, data=file_chunk)
                 else:
                     http_response = requests.put(url, data=file_chunk)
                 http_response.raise_for_status()
                 logger.debug(f"Upload for part {num + 1} succeeded.")
                 break
-            except requests.exceptions.HTTPError:
-                logger.warn(
-                    f"Upload for part {num + 1} failed. Attempt {attempts + 1} of {max_retries}."
-                )
+            except (requests.exceptions.HTTPError, requests.exceptions.SSLError, requests.exceptions.ConnectionError) as e:
                 attempts += 1
-                if attempts == max_retries:
-                    raise
-                time.sleep(10**attempts)  # exponential backoff, (10 ** 2)s default max
+                logger.debug(
+                    f"Upload for part {num + 1} failed. Attempt {attempts} of {max_retries}. Error: {e}"
+                )
+                if attempts >= max_retries:
+                    raise e
+
+                retry_time = min(8 ** attempts, 120)  # exponential backoff, max 120s
+                retry_time *= 0.6 + (random() * 0.8)  # randomize to avoid thundering herd
+                logger.debug(f"Retrying upload for part {num + 1} in {retry_time} seconds.")
+                time.sleep(retry_time)
+            
         etag = http_response.headers["ETag"].replace('"', "")
         blob = {"ETag": etag, "PartNumber": num + 1}
         if resumable_upload_tracker:
             # TODO technically not thread safe, but should be fine for now
             resumable_upload_tracker.add_part(blob)
         return blob
     
-    def _finish_multipart_upload(self, upload_id, complete_parts):
-        response = self.knex.post(
-            f"/ar_fields/{self.uuid}/complete_upload",
-            json={
-                "parts": complete_parts,
-                "upload_id": upload_id,
-                "result_type": "sample" if self.is_sample_result else "group",
-            },
-            json_response=False,
-        )
+    def _finish_multipart_upload(self, upload_id, complete_parts, atomic=False):
+        data = {
+            "parts": complete_parts,
+            "upload_id": upload_id,
+            "result_type": self._result_type(atomic),
+        }
+        url = f"/ar_fields/{self.uuid}/complete_upload"
+        if atomic:
+            data["fieldname"] = self.name
+            url = f"/ars/{self.parent.uuid}/complete_atomic_upload"
+        response = self.knex.post(url, json=data, json_response=False)
         response.raise_for_status()
 
     def _upload_parts(self, file_chunker, urls, max_retries, session, progress_tracker, threads, resumable_upload_tracker=None):
         if threads == 1:
             logger.info(f"Uploading parts in series for {file_chunker.filepath}")
             complete_parts = []
             for num, url in enumerate(list(urls.values())):
@@ -219,55 +147,78 @@
         return complete_parts
 
     def multipart_upload_file(
         self,
         filepath,
         file_size,
         optional_fields=None,
-        chunk_size=FIVE_MB,
+        chunk_size=None,
         max_retries=3,
         session=None,
         progress_tracker=None,
         threads=1,
         use_cache=True,
+        use_atomic_upload=False,
     ):
         """Upload a file to S3 using the multipart upload process."""
         logger.info(f"Uploading {filepath} to S3 using multipart upload.")
+        if not chunk_size:
+            chunk_size = FIVE_MB
+            if file_size >= 10 * FIVE_MB:
+                chunk_size = 5 * FIVE_MB
+        logger.debug(f"Using chunk size of {chunk_size} bytes.")
         resumable_upload_tracker = None
         if use_cache and file_size > 10 * FIVE_MB:  # only use resumable upload tracker for larger files
-            resumable_upload_tracker = ResumableUploadTracker(filepath, chunk_size)
+            upload_target_uuid = self.parent.uuid if use_atomic_upload else self.uuid
+            resumable_upload_tracker = ResumableUploadTracker(filepath, chunk_size, upload_target_uuid)
+
         if resumable_upload_tracker and resumable_upload_tracker.upload_started:
+            # a resumable upload for this file has already started
+            resumable_upload_exists_and_is_valid = True
             upload_id, urls = resumable_upload_tracker.upload_id, resumable_upload_tracker.urls
+            use_atomic_upload = resumable_upload_tracker.is_atomic_upload
             logger.info(f'Resuming upload for "{filepath}", upload_id: "{upload_id}"')
         else:
-            upload_id, urls = self._prep_multipart_upload(filepath, file_size, chunk_size, optional_fields)
+            upload_id, urls = self._prep_multipart_upload(filepath, file_size, chunk_size, optional_fields, atomic=use_atomic_upload)
             if resumable_upload_tracker:
                 logger.info(f'Creating new resumable upload for "{filepath}", upload_id: "{upload_id}"')
-                resumable_upload_tracker.start_upload(upload_id, urls)
+                resumable_upload_tracker.start_upload(upload_id, urls, is_atomic_upload=use_atomic_upload)
+
         logger.info(f'Starting upload for "{filepath}"')
         complete_parts = []
-        file_chunker = FileChunker(filepath, chunk_size).load_all_chunks()
+        file_chunker = FileChunker(filepath, chunk_size)
+        if file_chunker.file_size < 10 * FIVE_MB:
+            file_chunker.load_all_chunks()
+            logger.debug(f"Preloaded all chunks for {filepath}")
+        else:
+            logger.debug(f"Did not preload chunks for {filepath}")
         if progress_tracker: progress_tracker.set_num_chunks(file_chunker.file_size)
         complete_parts = self._upload_parts(
             file_chunker,
             urls,
             max_retries,
             session,
             progress_tracker,
             threads,
             resumable_upload_tracker=resumable_upload_tracker
         )
-        self._finish_multipart_upload(upload_id, complete_parts)
+        self._finish_multipart_upload(upload_id, complete_parts, atomic=use_atomic_upload)
         logger.info(f'Finished Upload for "{filepath}"')
+        if use_atomic_upload:
+            # if this was an atomic upload then this result may not have existed on the server before
+            self.get()
         return self
 
     def upload_file(self, filepath, multipart_thresh=FIVE_MB, overwrite=True, no_new_versions=False, **kwargs):
         if self.exists() and not overwrite:  
             raise GeoseeqGeneralError(f"Overwrite is set to False and file {self.uuid} already exists.")
-        self.idem()
+        if not kwargs.get("use_atomic_upload", False):
+            self.idem()
+        else:
+            self.parent.idem()
         if no_new_versions and self.has_downloadable_file():
             raise GeoseeqGeneralError(f"File {self} already has a downloadable file. Not uploading a new version.")
         resolved_path = Path(filepath).resolve()
         file_size = getsize(resolved_path)
         return self.multipart_upload_file(filepath, file_size, **kwargs)
     
     def upload_json(self, data, **kwargs):
```

### Comparing `geoseeq-0.5.6a9/geoseeq/result/result_file.py` & `geoseeq-0.6.0/geoseeq/result/result_file.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/result/result_folder.py` & `geoseeq-0.6.0/geoseeq/result/result_folder.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/result/utils.py` & `geoseeq-0.6.0/geoseeq/result/utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/sample.py` & `geoseeq-0.6.0/geoseeq/sample.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/search.py` & `geoseeq-0.6.0/geoseeq/search.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/upload_download_manager.py` & `geoseeq-0.6.0/geoseeq/upload_download_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,55 +17,80 @@
     logger.addHandler(handler)
     return logger
 
 
 def _upload_one_file(args):
     (result_file, filepath, session, progress_tracker,
      link_type, overwrite, log_level, parallel_uploads,
-     use_cache, no_new_versions) = args
+     use_cache, no_new_versions, threads_per_upload,
+     num_retries, ignore_errors, chunk_size_mb, use_atomic_upload) = args
+    chunk_size = chunk_size_mb * 1024 * 1024 if chunk_size_mb else None
     if parallel_uploads:
         _make_in_process_logger(log_level)
-    if link_type == 'upload':
-        # TODO: check checksums to see if the file is the same
-        result_file.upload_file(
-            filepath,
-            session=session, overwrite=overwrite, progress_tracker=progress_tracker,
-            threads=4, use_cache=use_cache, no_new_versions=no_new_versions
-        )
-    else:
-        result_file.link_file(link_type, filepath)
+    try:
+        if link_type == 'upload':
+            # TODO: check checksums to see if the file is the same
+            result_file.upload_file(
+                filepath,
+                session=session, overwrite=overwrite, progress_tracker=progress_tracker,
+                threads=threads_per_upload, use_cache=use_cache, chunk_size=chunk_size,
+                no_new_versions=no_new_versions, max_retries=num_retries,
+                use_atomic_upload=use_atomic_upload
+            )
+        else:
+            result_file.link_file(link_type, filepath)
+    except Exception as e:
+        if ignore_errors:
+            logger.error(f"Error uploading {filepath}: {e}")
+        else:
+            raise e
     return result_file
 
 
 class GeoSeeqUploadManager:
 
     def __init__(self,
                  n_parallel_uploads=1,
+                 threads_per_upload=4,
                  session=None,
                  link_type='upload',
                  progress_tracker_factory=None,
                  log_level=logging.WARNING,
                  overwrite=True,
                  no_new_versions=False,
+                 num_retries=3,
+                 ignore_errors=False,
+                 chunk_size_mb=5,
+                 use_atomic_upload=True,
                  use_cache=True):
         self.session = session
         self.n_parallel_uploads = n_parallel_uploads
         self.progress_tracker_factory = progress_tracker_factory if progress_tracker_factory else lambda x: None
         self.log_level = log_level
         self.link_type = link_type
         self.overwrite = overwrite
         self._result_files = []
         self.no_new_versions = no_new_versions
         self.use_cache = use_cache
+        self.threads_per_upload = threads_per_upload
+        self.num_retries = num_retries
+        self.ignore_errors = ignore_errors
+        self.chunk_size_mb = chunk_size_mb
+        self.use_atomic_upload = use_atomic_upload
 
     def add_result_file(self, result_file, local_path):
         self._result_files.append((result_file, local_path))
 
     def add_local_file_to_result_folder(self, result_folder, local_path, geoseeq_file_name=None):
-        geoseeq_file_name = geoseeq_file_name if geoseeq_file_name else local_path
+        if not geoseeq_file_name:
+            if local_path.startswith("/"):  # if local path is an absolute path use the basename
+                geoseeq_file_name = basename(local_path)
+            else:
+                # remove "./" and "../" from local path to get a geoseeq file name
+                geoseeq_file_name = local_path.replace("./", "").replace("../", "")
         result_file = result_folder.result_file(geoseeq_file_name)
         self.add_result_file(result_file, local_path)
 
     def add_local_folder_to_result_folder(self, result_folder, local_path, recursive=False, hidden_files=False, prefix=""):
         for result_file, local_path in result_folder._prepare_folder_upload(local_path, recursive, hidden_files, prefix):
             self.add_result_file(result_file, local_path)
 
@@ -76,15 +101,17 @@
         return "\n".join(out)
 
     def upload_files(self):
         upload_args = [(
                 result_file, local_path,
                 self.session, self.progress_tracker_factory(local_path),
                 self.link_type, self.overwrite, self.log_level,
-                self.n_parallel_uploads > 1, self.use_cache, self.no_new_versions
+                self.n_parallel_uploads > 1, self.use_cache, self.no_new_versions,
+                self.threads_per_upload, self.num_retries, self.ignore_errors,
+                self.chunk_size_mb, self.use_atomic_upload
             ) for result_file, local_path in self._result_files
         ]
         out = []
         if self.n_parallel_uploads == 1:
             logger.info(f"Uploading files in series.")
             for upload_arg in upload_args:
                 out.append(_upload_one_file(upload_arg))
```

### Comparing `geoseeq-0.5.6a9/geoseeq/user.py` & `geoseeq-0.6.0/geoseeq/user.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/utils.py` & `geoseeq-0.6.0/geoseeq/utils.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/vc/checksum.py` & `geoseeq-0.6.0/geoseeq/vc/checksum.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/vc/cli.py` & `geoseeq-0.6.0/geoseeq/vc/cli.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/vc/clone.py` & `geoseeq-0.6.0/geoseeq/vc/clone.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/vc/vc_cache.py` & `geoseeq-0.6.0/geoseeq/vc/vc_cache.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/vc/vc_sample.py` & `geoseeq-0.6.0/geoseeq/vc/vc_sample.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/vc/vc_stub.py` & `geoseeq-0.6.0/geoseeq/vc/vc_stub.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq/work_orders.py` & `geoseeq-0.6.0/geoseeq/work_orders.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/geoseeq.egg-info/PKG-INFO` & `geoseeq-0.6.0/geoseeq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoseeq
-Version: 0.5.6a9
+Version: 0.6.0
 Summary: GeoSeeq command line tools and python API
 Author: David C. Danko
 Author-email: "David C. Danko" <dcdanko@biotia.io>
 Project-URL: Homepage, https://github.com/biotia/geoseeq_api_client
 Project-URL: Issues, https://github.com/biotia/geoseeq_api_client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geoseeq-0.5.6a9/geoseeq.egg-info/SOURCES.txt` & `geoseeq-0.6.0/geoseeq.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 geoseeq/cli/detail.py
 geoseeq/cli/download.py
 geoseeq/cli/fastq_utils.py
 geoseeq/cli/get_eula.py
 geoseeq/cli/main.py
 geoseeq/cli/manage.py
 geoseeq/cli/progress_bar.py
+geoseeq/cli/project.py
+geoseeq/cli/raw.py
 geoseeq/cli/run.py
 geoseeq/cli/search.py
 geoseeq/cli/user.py
 geoseeq/cli/utils.py
 geoseeq/cli/view.py
 geoseeq/cli/shared_params/__init__.py
 geoseeq/cli/shared_params/common_state.py
@@ -68,18 +70,20 @@
 geoseeq/plotting/selectable.py
 geoseeq/plotting/map/__init__.py
 geoseeq/plotting/map/base_layer.py
 geoseeq/plotting/map/map.py
 geoseeq/plotting/map/overlay.py
 geoseeq/result/__init__.py
 geoseeq/result/bioinfo.py
+geoseeq/result/file_chunker.py
 geoseeq/result/file_download.py
 geoseeq/result/file_upload.py
 geoseeq/result/result_file.py
 geoseeq/result/result_folder.py
+geoseeq/result/resumable_upload_tracker.py
 geoseeq/result/utils.py
 geoseeq/vc/__init__.py
 geoseeq/vc/checksum.py
 geoseeq/vc/cli.py
 geoseeq/vc/clone.py
 geoseeq/vc/constants.py
 geoseeq/vc/vc_cache.py
```

### Comparing `geoseeq-0.5.6a9/pyproject.toml` & `geoseeq-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "geoseeq"
-version = "0.5.6a9"
+version = "0.6.0"
 authors = [
   { name="David C. Danko", email="dcdanko@biotia.io" },
 ]
 description = "GeoSeeq command line tools and python API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `geoseeq-0.5.6a9/setup.py` & `geoseeq-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/tests/test_api_client.py` & `geoseeq-0.6.0/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `geoseeq-0.5.6a9/tests/test_plotting.py` & `geoseeq-0.6.0/tests/test_plotting.py`

 * *Files identical despite different names*

