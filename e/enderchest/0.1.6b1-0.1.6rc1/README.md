# Comparing `tmp/enderchest-0.1.6b1.tar.gz` & `tmp/enderchest-0.1.6rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enderchest-0.1.6b1.tar", last modified: Fri Feb 23 22:04:33 2024, max compression
+gzip compressed data, was "enderchest-0.1.6rc1.tar", last modified: Sat Apr 27 17:28:50 2024, max compression
```

## Comparing `enderchest-0.1.6b1.tar` & `enderchest-0.1.6rc1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 22:04:33.681292 enderchest-0.1.6b1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-02-23 22:04:33.681292 enderchest-0.1.6b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 22:04:33.681292 enderchest-0.1.6b1/enderchest/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-02-23 22:04:33.681292 enderchest-0.1.6b1/enderchest/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    25458 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    33526 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/craft.py
--rw-r--r--   0 runner    (1001) docker     (127)    18698 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/enderchest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)    23042 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/gather.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    13405 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/loggers.py
--rw-r--r--   0 runner    (1001) docker     (127)    26205 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/place.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9140 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)    14628 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/shulker_box.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 22:04:33.677292 enderchest-0.1.6b1/enderchest/sync/
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13573 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/sync/file.py
--rw-r--r--   0 runner    (1001) docker     (127)    17958 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/sync/rsync.py
--rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/sync/sftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9176 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/sync/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 22:04:33.677292 enderchest-0.1.6b1/enderchest/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8090 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/test/mock_paramiko.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/test/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/test/test_break.py
--rw-r--r--   0 runner    (1001) docker     (127)    22824 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7848 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    27052 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/test/test_craft.py
--rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/test/test_gather.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/test/test_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/test/test_inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)    50204 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/test/test_place.py
--rw-r--r--   0 runner    (1001) docker     (127)    39936 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/test/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/test/test_sync_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 22:04:33.677292 enderchest-0.1.6b1/enderchest/test/testing_files/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/test/testing_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/test/testing_files/enderchest.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/test/testing_files/instgroups.json
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/test/testing_files/launcher_profiles.json
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/test/testing_files/lstat_cache.json
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/test/testing_files/options.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/test/testing_files/version_manifest_v2.json
--rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/test/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/enderchest/uninstall.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 22:04:33.677292 enderchest-0.1.6b1/enderchest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-02-23 22:04:33.000000 enderchest-0.1.6b1/enderchest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-02-23 22:04:33.000000 enderchest-0.1.6b1/enderchest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 22:04:33.000000 enderchest-0.1.6b1/enderchest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-23 22:04:33.000000 enderchest-0.1.6b1/enderchest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-23 22:04:33.000000 enderchest-0.1.6b1/enderchest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-23 22:04:33.000000 enderchest-0.1.6b1/enderchest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-02-23 22:04:33.681292 enderchest-0.1.6b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    83196 2024-02-23 22:04:24.000000 enderchest-0.1.6b1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:28:50.767629 enderchest-0.1.6rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-04-27 17:28:50.767629 enderchest-0.1.6rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:28:50.767629 enderchest-0.1.6rc1/enderchest/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-27 17:28:50.767629 enderchest-0.1.6rc1/enderchest/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26070 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33526 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/craft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18698 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/enderchest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23042 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/gather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13405 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26205 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/place.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9140 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14628 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/shulker_box.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:28:50.763629 enderchest-0.1.6rc1/enderchest/sync/
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13574 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/sync/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17959 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/sync/rsync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18517 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/sync/sftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/sync/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:28:50.767629 enderchest-0.1.6rc1/enderchest/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8091 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/test/mock_paramiko.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/test/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/test/test_break.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25023 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7848 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27052 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/test/test_craft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16980 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/test/test_gather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/test/test_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/test/test_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50204 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/test/test_place.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39936 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/test/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/test/test_sync_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:28:50.767629 enderchest-0.1.6rc1/enderchest/test/testing_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/test/testing_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/test/testing_files/enderchest.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/test/testing_files/instgroups.json
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/test/testing_files/launcher_profiles.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/test/testing_files/lstat_cache.json
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/test/testing_files/options.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/test/testing_files/version_manifest_v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13343 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/test/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/enderchest/uninstall.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:28:50.767629 enderchest-0.1.6rc1/enderchest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-04-27 17:28:50.000000 enderchest-0.1.6rc1/enderchest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-27 17:28:50.000000 enderchest-0.1.6rc1/enderchest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:28:50.000000 enderchest-0.1.6rc1/enderchest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-27 17:28:50.000000 enderchest-0.1.6rc1/enderchest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-27 17:28:50.000000 enderchest-0.1.6rc1/enderchest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-27 17:28:50.000000 enderchest-0.1.6rc1/enderchest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-27 17:28:50.767629 enderchest-0.1.6rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83196 2024-04-27 17:28:44.000000 enderchest-0.1.6rc1/versioneer.py
```

### Comparing `enderchest-0.1.6b1/LICENSE` & `enderchest-0.1.6rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.6b1/PKG-INFO` & `enderchest-0.1.6rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enderchest
-Version: 0.1.6b1
+Version: 0.1.6rc1
 Summary: syncing and linking for all your Minecraft instances
 Home-page: https://github.com/OpenBagTwo/EnderChest
 Author: Gili "OpenBagTwo" Barlev
 License: GPL v3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `enderchest-0.1.6b1/README.md` & `enderchest-0.1.6rc1/README.md`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.6b1/enderchest/cli.py` & `enderchest-0.1.6rc1/enderchest/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,15 @@
 )
 _list_aliases = ("inventory", "list")
 
 
 class Action(Protocol):  # pragma: no cover
     """Common protocol for CLI actions"""
 
-    def __call__(self, minecraft_root: Path, /) -> Any:
-        ...
+    def __call__(self, minecraft_root: Path, /) -> Any: ...
 
 
 def _place(
     minecraft_root: Path,
     errors: str = "prompt",
     keep_broken_links: bool = False,
     keep_stale_links: bool = False,
@@ -166,14 +165,22 @@
     if exit_code := pytest.main(
         ["--pyargs", "enderchest.test", *pytest_args],
         plugins=(plugin,),
     ):
         raise SystemExit(f"Tests Failed with exit code: {exit_code}")
 
 
+def _break(minecraft_root: Path, instances: Iterable[str] | None = None):
+    """Router for the break verb"""
+    if not instances:
+        uninstall.break_ender_chest(minecraft_root)
+    else:
+        uninstall.break_instances(minecraft_root, instances)
+
+
 ACTIONS: tuple[tuple[tuple[str, ...], str, Action], ...] = (
     # action names (first one is canonical), action description, action method
     (
         sum(((verb, verb + " enderchest") for verb in _create_aliases), ()),
         "create and configure a new EnderChest installation",
         craft.craft_ender_chest,
     ),
@@ -267,17 +274,17 @@
     (
         ("close",),
         "push changes to other EnderChests",
         _close,
     ),
     (
         ("break",),
-        "uninstall EnderChest by copying all linked resources"
-        " into its registered instances",
-        uninstall.break_ender_chest,
+        "uninstall EnderChest by copying linked resources"
+        " into some or all of the registered instances",
+        _break,
     ),
     (
         ("test",),
         "run the EnderChest test suite",
         _test,
     ),
 )
@@ -335,23 +342,24 @@
     for verb, description in descriptions.items():
         parser = ArgumentParser(
             prog=f"enderchest {verb}",
             description=description,
         )
         if verb != "test":
             root = parser.add_mutually_exclusive_group()
-            root.add_argument(
-                "root",
-                nargs="?",
-                help=(
-                    "optionally specify your root minecraft directory."
-                    "  If no path is given, the current working directory will be used."
-                ),
-                type=Path,
-            )
+            if verb != "break":
+                root.add_argument(
+                    "root",
+                    nargs="?",
+                    help=(
+                        "optionally specify your root minecraft directory."
+                        "  If no path is given, the current working directory will be used."
+                    ),
+                    type=Path,
+                )
             root.add_argument(
                 "--root",
                 dest="root_flag",
                 help="specify your root minecraft directory",
                 type=Path,
             )
 
@@ -686,14 +694,22 @@
             "-c",
             dest="sync_confirm_wait",
             action="store_true",
             help="after performing the dry run, explicitly ask for confirmation"
             " before performing the real sync",
         )
 
+    break_parser = action_parsers["break"]
+    break_parser.add_argument(
+        "instances",
+        nargs="*",
+        help="instead of breaking your entire EnderChest, just deregister and"
+        " copy linked resources into the specified instances (by name)",
+    )
+
     # test pass-through
     test_parser = action_parsers["test"]
     test_parser.add_argument(
         "--use-local-ssh",
         action="store_true",
         dest="use_local_ssh",
         help=(
@@ -762,15 +778,15 @@
                 action_parsers[aliases[command]].parse_args(
                     argv[1 + len(command.split()) :]
                 )
             )
 
             action = actions[aliases[command]]
 
-            root_arg = action_kwargs.pop("root")
+            root_arg = None if command == "break" else action_kwargs.pop("root")
             root_flag = action_kwargs.pop("root_flag")
 
             verbosity = action_kwargs.pop("verbose") - action_kwargs.pop("quiet")
 
             argspec = inspect.getfullargspec(action)
             if "verbosity" in argspec.args + argspec.kwonlyargs:
                 action_kwargs["verbosity"] = verbosity
```

### Comparing `enderchest-0.1.6b1/enderchest/config.py` & `enderchest-0.1.6rc1/enderchest/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Helpers for parsing and writing INI-format config files"""
+
 import ast
 import datetime as dt
 from configparser import ConfigParser, ParsingError
 from io import StringIO
 from pathlib import Path
 from typing import Any, Iterable, Mapping, Sequence
```

### Comparing `enderchest-0.1.6b1/enderchest/craft.py` & `enderchest-0.1.6rc1/enderchest/craft.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.6b1/enderchest/enderchest.py` & `enderchest-0.1.6rc1/enderchest/enderchest.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.6b1/enderchest/filesystem.py` & `enderchest-0.1.6rc1/enderchest/filesystem.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.6b1/enderchest/gather.py` & `enderchest-0.1.6rc1/enderchest/gather.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.6b1/enderchest/instance.py` & `enderchest-0.1.6rc1/enderchest/instance.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.6b1/enderchest/inventory.py` & `enderchest-0.1.6rc1/enderchest/inventory.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.6b1/enderchest/loggers.py` & `enderchest-0.1.6rc1/enderchest/loggers.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.6b1/enderchest/place.py` & `enderchest-0.1.6rc1/enderchest/place.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.6b1/enderchest/prompt.py` & `enderchest-0.1.6rc1/enderchest/prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities for helping build interactive prompts"""
+
 import getpass
 
 CURSOR = "\x1b[35;1m==>\x1b[0m"
 
 # https://stackoverflow.com/a/18472142
 YES = ("y", "yes", "t", "true", "on", "1")
 
@@ -56,15 +57,15 @@
 
     Returns
     -------
     bool
         Whether the user has opted to continue
     """
 
-    response = prompt("Do you wish to continue?", "Y/n" if default else "y/N")
+    response = prompt("Do you wish to continue?", "Y/n" if default else "y/N").lower()
 
     if response == "":
         return default
 
     if response in YES:
         return True
```

### Comparing `enderchest-0.1.6b1/enderchest/remote.py` & `enderchest-0.1.6rc1/enderchest/remote.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.6b1/enderchest/shulker_box.py` & `enderchest-0.1.6rc1/enderchest/shulker_box.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.6b1/enderchest/sync/__init__.py` & `enderchest-0.1.6rc1/enderchest/sync/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Low-level functionality for synchronizing across different machines"""
+
 import importlib
 from contextlib import contextmanager
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Collection, Generator
 from urllib.parse import ParseResult
```

### Comparing `enderchest-0.1.6b1/enderchest/sync/file.py` & `enderchest-0.1.6rc1/enderchest/sync/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """shutil-based sync implementation"""
+
 import fnmatch
 import logging
 import os
 import shutil
 import stat
 from pathlib import Path
 from typing import Callable, Collection
```

### Comparing `enderchest-0.1.6b1/enderchest/sync/rsync.py` & `enderchest-0.1.6rc1/enderchest/sync/rsync.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """rsync sync implementation. Relies on the user having rsync installed on their system"""
+
 import os.path
 import re
 import shutil
 import subprocess
 from collections import defaultdict
 from pathlib import Path
 from typing import Iterable
```

### Comparing `enderchest-0.1.6b1/enderchest/sync/sftp.py` & `enderchest-0.1.6rc1/enderchest/sync/sftp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """paramiko-based sftp sync implementation"""
+
 import os
 import posixpath
 import stat
 from contextlib import contextmanager
 from pathlib import Path
 from typing import Any, Collection, Generator
 from urllib.parse import ParseResult, unquote
```

### Comparing `enderchest-0.1.6b1/enderchest/sync/utils.py` & `enderchest-0.1.6rc1/enderchest/sync/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,24 +87,21 @@
     if uri.hostname != alias:
         uri_string += f" ({alias})"
     return uri_string
 
 
 class _StatLike(Protocol):  # pragma: no cover
     @property
-    def st_mode(self) -> int | None:
-        ...
+    def st_mode(self) -> int | None: ...
 
     @property
-    def st_size(self) -> float | None:
-        ...
+    def st_size(self) -> float | None: ...
 
     @property
-    def st_mtime(self) -> float | None:
-        ...
+    def st_mtime(self) -> float | None: ...
 
 
 def is_identical(object_one: _StatLike, object_two: _StatLike) -> bool:
     """Determine if two objects are identical (meaning: skip when syncing)
 
     Parameters
     ----------
```

### Comparing `enderchest-0.1.6b1/enderchest/test/conftest.py` & `enderchest-0.1.6rc1/enderchest/test/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Useful setup / teardown fixtures"""
+
 from importlib.resources import as_file
 from pathlib import Path
 from typing import Generator
 
 import pytest
 
 from .testing_files import CLIENT_OPTIONS
```

### Comparing `enderchest-0.1.6b1/enderchest/test/mock_paramiko.py` & `enderchest-0.1.6rc1/enderchest/test/mock_paramiko.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """A mock Paramiko SFTP client to be used for testing on systems without local SSH"""
+
 import json
 import os
 import shutil
 from contextlib import contextmanager
 from importlib.resources import as_file
 from pathlib import Path
 from typing import Callable, Generator, NamedTuple
```

### Comparing `enderchest-0.1.6b1/enderchest/test/plugin.py` & `enderchest-0.1.6rc1/enderchest/test/plugin.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.6b1/enderchest/test/test_cli.py` & `enderchest-0.1.6rc1/enderchest/test/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 from pathlib import Path
 from typing import Generator
 
 import pytest
 
 import enderchest
-from enderchest import cli, inventory, place, remote
+from enderchest import cli, inventory, place, remote, uninstall
 
 
 class TestHelp:
     @pytest.mark.parametrize("help_flag", ("-h", "--help"))
     def test_help_displays_version(self, capsys, help_flag):
         with pytest.raises(SystemExit):
             cli.parse_args(["enderchest", help_flag])
@@ -42,14 +42,15 @@
             cli.parse_args(["enderchest", version_flag, "foo"])
 
         assert "foo" not in capsys.readouterr().out
         assert "foo" not in capsys.readouterr().err
 
 
 class ActionTestSuite:
+    action: str
     required_args: tuple[str, ...] = ()
 
     @pytest.mark.parametrize("help_flag", ("-h", "--help"))
     def test_help_gives_action_specific_help(
         self,
         capsys,
         help_flag,
@@ -677,7 +678,68 @@
 class TestClose(TestOpen):
     action = "close"
     op = "push"
 
 
 class TestBreak(ActionTestSuite):
     action = "break"
+
+    @pytest.fixture(autouse=True)
+    def prevent_actual_breakage(self, monkeypatch):
+        def mock_break(*args, **kwargs):
+            raise AssertionError("I should not have been called")
+
+        monkeypatch.setattr(uninstall, "_break", mock_break)
+
+    @pytest.fixture
+    def call_logs(self, monkeypatch):
+        full_uninstall_calls = []
+        partial_uninstall_calls = []
+
+        def mock_full_uninstall(*args, **kwargs):
+            full_uninstall_calls.append((args, kwargs))
+
+        def mock_partial_uninstall(*args, **kwargs):
+            partial_uninstall_calls.append((args, kwargs))
+
+        monkeypatch.setattr(uninstall, "break_ender_chest", mock_full_uninstall)
+        monkeypatch.setattr(uninstall, "break_instances", mock_partial_uninstall)
+
+        return {"full": full_uninstall_calls, "partial": partial_uninstall_calls}
+
+    @pytest.mark.parametrize("extra_flags", ("-v", "-q", "--root minceraft"))
+    def test_no_instance_names_routes_to_complete_uninstall(
+        self, call_logs, extra_flags
+    ):
+        action, root, _, kwargs = cli.parse_args(
+            [
+                "enderchest",
+                *self.action.split(),
+                *extra_flags.split(),
+            ]
+        )
+        action(root, **kwargs)
+        assert len(call_logs["partial"]) == 0
+        assert len(call_logs["full"]) == 1
+
+    @pytest.mark.parametrize("n_instances", (1, 2))
+    @pytest.mark.parametrize("extra_flags", ("-v", "-q", "--root minceraft"))
+    def test_providing_instance_names_routes_to_partial_uninstall(
+        self, call_logs, extra_flags, n_instances
+    ):
+        args = ["potato", "infinity"][:n_instances]
+        action, root, _, kwargs = cli.parse_args(
+            [
+                "enderchest",
+                *self.action.split(),
+                *args,
+                *extra_flags.split(),
+            ]
+        )
+        action(root, **kwargs)
+        assert len(call_logs["full"]) == 0
+        assert len(call_logs["partial"]) == 1
+        assert call_logs["partial"][0][0][1:] == (["potato", "infinity"][:n_instances],)
+
+    def test_first_argument_is_root(self):
+        """Because it's not"""
+        pass
```

### Comparing `enderchest-0.1.6b1/enderchest/test/test_config.py` & `enderchest-0.1.6rc1/enderchest/test/test_config.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.6b1/enderchest/test/test_craft.py` & `enderchest-0.1.6rc1/enderchest/test/test_craft.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.6b1/enderchest/test/test_gather.py` & `enderchest-0.1.6rc1/enderchest/test/test_gather.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,15 +296,15 @@
         ):
             (centralized_jar_folder / jar_name).write_text("Correct jar\n")
             expected_metadata[centralized_jar_folder / jar_name] = i.InstanceSpec(
                 "ignoreme", Path("ignoreme"), ("1.20.4",), launcher, ("server",), ()
             )
         return expected_metadata
 
-    def test_parsing_metadata_from_jar(self, server_jars):
+    def test_parsing_metadata_from_jar(self, server_jars) -> None:
         expected: list[tuple[Path, tuple[str], str]] = [
             (jar, instance.minecraft_versions, instance.modloader)
             for jar, instance in server_jars.items()
         ]
         results: list[tuple[Path, tuple[str], str]] = []
         for jar in server_jars:
             meta = gather._gather_metadata_from_jar_filename(jar.name)
```

### Comparing `enderchest-0.1.6b1/enderchest/test/test_instance.py` & `enderchest-0.1.6rc1/enderchest/test/test_instance.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.6b1/enderchest/test/test_inventory.py` & `enderchest-0.1.6rc1/enderchest/test/test_inventory.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.6b1/enderchest/test/test_place.py` & `enderchest-0.1.6rc1/enderchest/test/test_place.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.6b1/enderchest/test/test_sync.py` & `enderchest-0.1.6rc1/enderchest/test/test_sync.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.6b1/enderchest/test/test_sync_utils.py` & `enderchest-0.1.6rc1/enderchest/test/test_sync_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests of the sync-helper utilities"""
+
 import importlib
 import logging
 import os
 import shutil
 import time
 from pathlib import Path
 from urllib.parse import urlparse
```

### Comparing `enderchest-0.1.6b1/enderchest/test/testing_files/__init__.py` & `enderchest-0.1.6rc1/enderchest/test/testing_files/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Subpackage containing all files and templates used for testing"""
+
 from importlib.resources import files
 
 __all__ = [
     "CLIENT_OPTIONS",
     "ENDERCHEST_CONFIG",
     "LSTAT_CACHE",
     "INSTGROUPS",
```

### Comparing `enderchest-0.1.6b1/enderchest/test/testing_files/enderchest.cfg` & `enderchest-0.1.6rc1/enderchest/test/testing_files/enderchest.cfg`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.6b1/enderchest/test/testing_files/launcher_profiles.json` & `enderchest-0.1.6rc1/enderchest/test/testing_files/launcher_profiles.json`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.6b1/enderchest/test/testing_files/lstat_cache.json` & `enderchest-0.1.6rc1/enderchest/test/testing_files/lstat_cache.json`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.6b1/enderchest/test/utils.py` & `enderchest-0.1.6rc1/enderchest/test/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Testing utilities"""
+
 import json
 import shutil
 from importlib.resources import as_file
 from pathlib import Path
 from typing import Callable, Iterable
 
 import pytest
```

### Comparing `enderchest-0.1.6b1/enderchest/uninstall.py` & `enderchest-0.1.6rc1/enderchest/uninstall.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Functionality for copying all files into their instances"""
 
+import logging
 import os
 import shutil
 from pathlib import Path
 from typing import Iterable
 
 from . import filesystem as fs
+from .enderchest import create_ender_chest
 from .instance import InstanceSpec
-from .inventory import load_ender_chest_instances
+from .inventory import load_ender_chest, load_ender_chest_instances
 from .loggers import BREAK_LOGGER, IMPORTANT
 from .prompt import confirm
 
 
 def break_ender_chest(minecraft_root: Path) -> None:
     """Replace all instance symlinks with their actual targets, effectively
     "uninstalling" EnderChest
@@ -33,22 +35,78 @@
         "\nwith copies of their EnderChest-linked targets."
         "\n\nTHIS CANNOT EASILY BE UNDONE!!"
     )
     if not confirm(default=False):
         BREAK_LOGGER.error("Aborting.")
         return
 
+    chest_folder = fs.ender_chest_folder(minecraft_root)
+    _break(chest_folder, instances)
+
+    BREAK_LOGGER.log(
+        IMPORTANT,
+        "EnderChest has been uninstalled."
+        "\nYou may now delete %s"
+        "\nand uninstall the EnderChest package",
+        chest_folder,
+    )
+
+
+def break_instances(minecraft_root: Path, instance_names: Iterable[str]) -> None:
+    """Deregister the specified instances from EnderChest, replacing all
+    instance symlinks with their actual targets, and then removing those
+    instances from the enderchest.cfg
+
+    Parameters
+    ----------
+    minecraft_root : Path
+        The root directory that your minecraft stuff (or, at least, the one
+        that's the parent of your EnderChest folder)
+    instance_names : list of str
+        The names of the instances to break
+    """
+    ender_chest = load_ender_chest(minecraft_root)
+
+    instance_lookup = {instance.name: instance for instance in ender_chest.instances}
+    instances: list[InstanceSpec] = []
+    for name in instance_names:
+        try:
+            instances.append(instance_lookup[name])
+        except KeyError:
+            BREAK_LOGGER.warning(
+                f'No instance named "{name}" is registered to this EnderChest.'
+                "\nSkipping."
+            )
+    if len(instances) == 0:
+        BREAK_LOGGER.error("No valid instances specified.\nAborting.")
+        return
+
+    BREAK_LOGGER.warning(
+        "Are you sure you want to remove the following instances from your EnderChest?"
+        + "\n"
+        + "\n".join((f"  - {instance.name}" for instance in instances))
+        + "\nDoing so will replace ALL the symlinks in each of the above instances"
+        "\nwith copies of their EnderChest-linked targets."
+        "\n\nTHIS CANNOT EASILY BE UNDONE!!"
+    )
+    if not confirm(default=False):
+        BREAK_LOGGER.error("Aborting.")
+        return
+
     _break(fs.ender_chest_folder(minecraft_root), instances)
+    for instance in instances:
+        ender_chest._instances.remove(instance)
+    create_ender_chest(minecraft_root, ender_chest)
 
 
 def _break(
     chest_folder: Path,
     instances: Iterable[InstanceSpec],
 ) -> None:
-    """Actually perform the uninstallation (separated out for ease of mocking / testing)
+    """Actually perform the uninstallation
 
     Parameters
     ----------
     chest_folder : Path
         The path of the EnderChest folder that's being "broken"
     instances : list of InstanceSpec
         The instances to clear of EnderChest links
@@ -107,15 +165,7 @@
             except OSError as copy_fail:
                 BREAK_LOGGER.warning(
                     "Failed to copy %s to %s:\n  %s",
                     final_target,
                     resource_path,
                     copy_fail,
                 )
-
-    BREAK_LOGGER.log(
-        IMPORTANT,
-        "EnderChest has been uninstalled."
-        "\nYou may now delete %s"
-        "\nand uninstall the EnderChest package",
-        chest_folder,
-    )
```

### Comparing `enderchest-0.1.6b1/enderchest.egg-info/PKG-INFO` & `enderchest-0.1.6rc1/enderchest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enderchest
-Version: 0.1.6b1
+Version: 0.1.6rc1
 Summary: syncing and linking for all your Minecraft instances
 Home-page: https://github.com/OpenBagTwo/EnderChest
 Author: Gili "OpenBagTwo" Barlev
 License: GPL v3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `enderchest-0.1.6b1/enderchest.egg-info/SOURCES.txt` & `enderchest-0.1.6rc1/enderchest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.6b1/setup.py` & `enderchest-0.1.6rc1/setup.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.6b1/versioneer.py` & `enderchest-0.1.6rc1/versioneer.py`

 * *Files identical despite different names*

