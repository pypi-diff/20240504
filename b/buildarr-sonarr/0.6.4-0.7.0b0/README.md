# Comparing `tmp/buildarr_sonarr-0.6.4.tar.gz` & `tmp/buildarr_sonarr-0.7.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildarr_sonarr-0.6.4.tar", max compression
+gzip compressed data, was "buildarr_sonarr-0.7.0b0.tar", last modified: Sat May  4 12:48:29 2024, max compression
```

## Comparing `buildarr_sonarr-0.6.4.tar` & `buildarr_sonarr-0.7.0b0.tar`

### file list

```diff
@@ -1,33 +1,110 @@
--rw-r--r--   0        0        0    35149 2024-03-02 02:34:38.306944 buildarr_sonarr-0.6.4/LICENSE
--rw-r--r--   0        0        0    19787 2024-03-02 02:34:38.306944 buildarr_sonarr-0.6.4/README.md
--rw-r--r--   0        0        0      971 2024-03-02 02:34:38.306944 buildarr_sonarr-0.6.4/buildarr_sonarr/__init__.py
--rw-r--r--   0        0        0    10334 2024-03-02 02:34:38.306944 buildarr_sonarr-0.6.4/buildarr_sonarr/api.py
--rw-r--r--   0        0        0     2869 2024-03-02 02:34:38.306944 buildarr_sonarr-0.6.4/buildarr_sonarr/cli.py
--rw-r--r--   0        0        0    12556 2024-03-02 02:34:38.306944 buildarr_sonarr-0.6.4/buildarr_sonarr/config/__init__.py
--rw-r--r--   0        0        0    51190 2024-03-02 02:34:38.306944 buildarr_sonarr-0.6.4/buildarr_sonarr/config/connect.py
--rw-r--r--   0        0        0    10198 2024-03-02 02:34:38.306944 buildarr_sonarr-0.6.4/buildarr_sonarr/config/download_clients/__init__.py
--rw-r--r--   0        0        0    48958 2024-03-02 02:34:38.306944 buildarr_sonarr-0.6.4/buildarr_sonarr/config/download_clients/download_clients.py
--rw-r--r--   0        0        0    10104 2024-03-02 02:34:38.306944 buildarr_sonarr-0.6.4/buildarr_sonarr/config/download_clients/remote_path_mappings.py
--rw-r--r--   0        0        0    18829 2024-03-02 02:34:38.306944 buildarr_sonarr-0.6.4/buildarr_sonarr/config/general.py
--rw-r--r--   0        0        0    45328 2024-03-02 02:34:38.306944 buildarr_sonarr-0.6.4/buildarr_sonarr/config/import_lists.py
--rw-r--r--   0        0        0    34871 2024-03-02 02:34:38.306944 buildarr_sonarr-0.6.4/buildarr_sonarr/config/indexers.py
--rw-r--r--   0        0        0    19730 2024-03-02 02:34:38.306944 buildarr_sonarr-0.6.4/buildarr_sonarr/config/media_management.py
--rw-r--r--   0        0        0    11018 2024-03-02 02:34:38.306944 buildarr_sonarr-0.6.4/buildarr_sonarr/config/metadata.py
--rw-r--r--   0        0        0     1527 2024-03-02 02:34:38.306944 buildarr_sonarr-0.6.4/buildarr_sonarr/config/profiles/__init__.py
--rw-r--r--   0        0        0    13160 2024-03-02 02:34:38.306944 buildarr_sonarr-0.6.4/buildarr_sonarr/config/profiles/delay.py
--rw-r--r--   0        0        0    12850 2024-03-02 02:34:38.306944 buildarr_sonarr-0.6.4/buildarr_sonarr/config/profiles/language.py
--rw-r--r--   0        0        0    16787 2024-03-02 02:34:38.306944 buildarr_sonarr-0.6.4/buildarr_sonarr/config/profiles/quality.py
--rw-r--r--   0        0        0    17315 2024-03-02 02:34:38.310944 buildarr_sonarr-0.6.4/buildarr_sonarr/config/profiles/release.py
--rw-r--r--   0        0        0     8312 2024-03-02 02:34:38.310944 buildarr_sonarr-0.6.4/buildarr_sonarr/config/quality.py
--rw-r--r--   0        0        0     2710 2024-03-02 02:34:38.310944 buildarr_sonarr-0.6.4/buildarr_sonarr/config/tags.py
--rw-r--r--   0        0        0     1229 2024-03-02 02:34:38.310944 buildarr_sonarr-0.6.4/buildarr_sonarr/config/types.py
--rw-r--r--   0        0        0     6150 2024-03-02 02:34:38.310944 buildarr_sonarr-0.6.4/buildarr_sonarr/config/ui.py
--rw-r--r--   0        0        0     1537 2024-03-02 02:34:38.310944 buildarr_sonarr-0.6.4/buildarr_sonarr/config/util.py
--rw-r--r--   0        0        0     1373 2024-03-02 02:34:38.310944 buildarr_sonarr-0.6.4/buildarr_sonarr/exceptions.py
--rw-r--r--   0        0        0      938 2024-03-02 02:34:38.310944 buildarr_sonarr-0.6.4/buildarr_sonarr/manager.py
--rw-r--r--   0        0        0     1165 2024-03-02 02:34:38.310944 buildarr_sonarr-0.6.4/buildarr_sonarr/plugin.py
--rw-r--r--   0        0        0        0 2024-03-02 02:34:38.310944 buildarr_sonarr-0.6.4/buildarr_sonarr/py.typed
--rw-r--r--   0        0        0     5691 2024-03-02 02:34:38.310944 buildarr_sonarr-0.6.4/buildarr_sonarr/secrets.py
--rw-r--r--   0        0        0     2100 2024-03-02 02:34:38.310944 buildarr_sonarr-0.6.4/buildarr_sonarr/types.py
--rw-r--r--   0        0        0     2116 2024-03-02 02:34:38.310944 buildarr_sonarr-0.6.4/pyproject.toml
--rw-r--r--   0        0        0    21168 1970-01-01 00:00:00.000000 buildarr_sonarr-0.6.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:29.218919 buildarr_sonarr-0.7.0b0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:29.198918 buildarr_sonarr-0.7.0b0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:29.202919 buildarr_sonarr-0.7.0b0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/.github/ISSUE_TEMPLATE/release.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:29.202919 buildarr_sonarr-0.7.0b0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21078 2024-05-04 12:48:29.218919 buildarr_sonarr-0.7.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19682 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:29.202919 buildarr_sonarr-0.7.0b0/buildarr_sonarr/
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10333 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:29.206919 buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/
+-rw-r--r--   0 runner    (1001) docker     (127)    12074 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51768 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/connect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:29.206919 buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/download_clients/
+-rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/download_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49190 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/download_clients/download_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10152 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/download_clients/remote_path_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17679 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44706 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/import_lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34974 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/indexers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19619 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/media_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10997 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:29.210919 buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13172 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/profiles/delay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12928 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/profiles/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16865 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/profiles/quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17279 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/profiles/release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:29.218919 buildarr_sonarr-0.7.0b0/buildarr_sonarr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21078 2024-05-04 12:48:29.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-04 12:48:29.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 12:48:29.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-04 12:48:29.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 12:48:29.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-04 12:48:29.000000 buildarr_sonarr-0.7.0b0/buildarr_sonarr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:29.210919 buildarr_sonarr-0.7.0b0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:29.210919 buildarr_sonarr-0.7.0b0/docs/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/docs/configuration/connect.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/docs/configuration/download-clients.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/docs/configuration/general.md
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/docs/configuration/host.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/docs/configuration/import-lists.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/docs/configuration/indexers.md
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/docs/configuration/media-management.md
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/docs/configuration/metadata.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:29.210919 buildarr_sonarr-0.7.0b0/docs/configuration/profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/docs/configuration/profiles/delay.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/docs/configuration/profiles/language.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/docs/configuration/profiles/quality.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/docs/configuration/profiles/release.md
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/docs/configuration/quality.md
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/docs/configuration/tags.md
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/docs/configuration/ui.md
+-rw-r--r--   0 runner    (1001) docker     (127)    19097 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    24700 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/docs/release-notes.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    94611 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/pdm.lock
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 12:48:29.218919 buildarr_sonarr-0.7.0b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:29.214919 buildarr_sonarr-0.7.0b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:29.214919 buildarr_sonarr-0.7.0b0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:29.214919 buildarr_sonarr-0.7.0b0/tests/unit/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/tests/unit/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:29.214919 buildarr_sonarr-0.7.0b0/tests/unit/config/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/tests/unit/config/settings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:29.214919 buildarr_sonarr-0.7.0b0/tests/unit/config/settings/general/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/tests/unit/config/settings/general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/tests/unit/config/settings/general/test_from_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27348 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/tests/unit/config/settings/general/test_update_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/tests/unit/config/settings/general/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:29.214919 buildarr_sonarr-0.7.0b0/tests/unit/config/settings/media_management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/tests/unit/config/settings/media_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/tests/unit/config/settings/media_management/test_delete_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24934 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/tests/unit/config/settings/media_management/test_from_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36438 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/tests/unit/config/settings/media_management/test_update_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/tests/unit/config/settings/media_management/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:29.214919 buildarr_sonarr-0.7.0b0/tests/unit/config/settings/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/tests/unit/config/settings/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/tests/unit/config/settings/metadata/test_from_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12124 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/tests/unit/config/settings/metadata/test_update_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/tests/unit/config/settings/metadata/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:29.214919 buildarr_sonarr-0.7.0b0/tests/unit/config/settings/tags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/tests/unit/config/settings/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/tests/unit/config/settings/tags/test_from_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/tests/unit/config/settings/tags/test_update_remote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:29.218919 buildarr_sonarr-0.7.0b0/tests/unit/config/settings/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/tests/unit/config/settings/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/tests/unit/config/settings/ui/test_from_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9581 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/tests/unit/config/settings/ui/test_update_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-04 12:48:13.000000 buildarr_sonarr-0.7.0b0/tests/unit/config/settings/ui/util.py
```

### Comparing `buildarr_sonarr-0.6.4/LICENSE` & `buildarr_sonarr-0.7.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `buildarr_sonarr-0.6.4/README.md` & `buildarr_sonarr-0.7.0b0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Buildarr Sonarr Plugin
 
-[![PyPI](https://img.shields.io/pypi/v/buildarr-sonarr)](https://pypi.org/project/buildarr-sonarr) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/buildarr-sonarr)  [![GitHub](https://img.shields.io/github/license/buildarr/buildarr-sonarr)](https://github.com/buildarr/buildarr-sonarr/blob/main/LICENSE) ![Pre-commit hooks](https://github.com/buildarr/buildarr-sonarr/actions/workflows/pre-commit.yml/badge.svg) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![PyPI](https://img.shields.io/pypi/v/buildarr-sonarr)](https://pypi.org/project/buildarr-sonarr) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/buildarr-sonarr)  [![GitHub](https://img.shields.io/github/license/buildarr/buildarr-sonarr)](https://github.com/buildarr/buildarr-sonarr/blob/main/LICENSE) ![Test Status](https://img.shields.io/github/actions/workflow/status/buildarr/buildarr-sonarr/test.yml?label=tests)
 
 The Buildarr Sonarr plugin (`buildarr-sonarr`) is a plugin for Buildarr that adds the capability to configure and manage [Sonarr](http://sonarr.tv) instances.
 
 Sonarr is a PVR application which downloads, renames and manages the lifecycle of TV shows in your media library. It is capable of scanning for higher quality versions of your media and automatically upgrading them when a suitable version is available.
 
 Currently, Sonarr V3 is the only supported version. Sonarr V4 support is planned for the future.
```

### Comparing `buildarr_sonarr-0.6.4/buildarr_sonarr/__init__.py` & `buildarr_sonarr-0.7.0b0/buildarr_sonarr/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Sonarr plugin for Buildarr root module.
 """
 
-
 from __future__ import annotations
 
 from importlib_metadata import PackageNotFoundError, version as package_version
 
 __all__ = ["__version__"]
 
 try:
```

### Comparing `buildarr_sonarr-0.6.4/buildarr_sonarr/api.py` & `buildarr_sonarr-0.7.0b0/buildarr_sonarr/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Sonarr plugin API functions.
 """
 
-
 from __future__ import annotations
 
 import re
 
 from http import HTTPStatus
 from logging import getLogger
 from typing import TYPE_CHECKING
```

### Comparing `buildarr_sonarr-0.6.4/buildarr_sonarr/cli.py` & `buildarr_sonarr-0.7.0b0/buildarr_sonarr/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Sonarr plugin CLI commands.
 """
 
-
 from __future__ import annotations
 
 import functools
 
 from getpass import getpass
 from typing import TYPE_CHECKING
 from urllib.parse import urlparse
@@ -77,31 +76,32 @@
         int(hostname_port[1])
         if len(hostname_port) == HOSTNAME_PORT_TUPLE_LENGTH
         else (443 if protocol == "https" else 80)
     )
     url_base = url.path
 
     instance_config = SonarrInstanceConfig(
-        **{  # type: ignore[arg-type]
-            "hostname": hostname,
-            "port": port,
-            "protocol": protocol,
-            "url_base": url_base,
-        },
+        hostname=hostname,
+        port=port,
+        protocol=protocol,  # type: ignore[arg-type]
+        url_base=url_base,
     )
 
     click.echo(
-        SonarrManager()
-        .from_remote(
-            instance_config=instance_config,
-            secrets=SonarrSecrets.get_from_url(
-                hostname=hostname,
-                port=port,
-                protocol=protocol,
-                url_base=url_base,
-                api_key=api_key if api_key else None,
-            ),
-        )
-        .yaml(exclude_unset=True),
+        (
+            SonarrManager()
+            .from_remote(
+                instance_config=instance_config,
+                secrets=SonarrSecrets.get_from_url(
+                    hostname=hostname,
+                    port=port,
+                    protocol=protocol,
+                    url_base=url_base,
+                    api_key=api_key if api_key else None,
+                ),
+            )
+            .model_dump_yaml(exclude_unset=True)
+        ),
+        nl=False,
     )
 
     return 0
```

### Comparing `buildarr_sonarr-0.6.4/buildarr_sonarr/config/__init__.py` & `buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,22 +12,20 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Sonarr plugin configuration.
 """
 
-
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Dict, Optional
 
 from buildarr.config import ConfigPlugin
 from buildarr.types import NonEmptyStr, Port
-from pydantic import validator
 from typing_extensions import Self
 
 from ..types import SonarrApiKey, SonarrProtocol
 from .connect import SonarrConnectSettingsConfig
 from .download_clients import SonarrDownloadClientsSettingsConfig
 from .general import SonarrGeneralSettingsConfig
 from .import_lists import SonarrImportListsSettingsConfig
@@ -39,39 +37,31 @@
 from .tags import SonarrTagsSettingsConfig
 from .types import SonarrConfigBase
 from .ui import SonarrUISettingsConfig
 
 if TYPE_CHECKING:
     from ..secrets import SonarrSecrets
 
-    class _SonarrInstanceConfig(ConfigPlugin[SonarrSecrets]):
-        ...
-
-else:
-
-    class _SonarrInstanceConfig(ConfigPlugin):
-        ...
-
 
 class SonarrSettingsConfig(SonarrConfigBase):
     """
     Sonarr settings, used to configure a remote Sonarr instance.
     """
 
-    media_management = SonarrMediaManagementSettingsConfig()  # type: ignore[call-arg]
-    profiles = SonarrProfilesSettingsConfig()
-    quality = SonarrQualitySettingsConfig()
-    indexers = SonarrIndexersSettingsConfig()  # type: ignore[call-arg]
-    download_clients = SonarrDownloadClientsSettingsConfig()
-    import_lists = SonarrImportListsSettingsConfig()
-    connect = SonarrConnectSettingsConfig()
-    metadata = SonarrMetadataSettingsConfig()
-    tags = SonarrTagsSettingsConfig()
-    general = SonarrGeneralSettingsConfig()
-    ui = SonarrUISettingsConfig()
+    media_management: SonarrMediaManagementSettingsConfig = SonarrMediaManagementSettingsConfig()
+    profiles: SonarrProfilesSettingsConfig = SonarrProfilesSettingsConfig()
+    quality: SonarrQualitySettingsConfig = SonarrQualitySettingsConfig()
+    indexers: SonarrIndexersSettingsConfig = SonarrIndexersSettingsConfig()
+    download_clients: SonarrDownloadClientsSettingsConfig = SonarrDownloadClientsSettingsConfig()
+    import_lists: SonarrImportListsSettingsConfig = SonarrImportListsSettingsConfig()
+    connect: SonarrConnectSettingsConfig = SonarrConnectSettingsConfig()
+    metadata: SonarrMetadataSettingsConfig = SonarrMetadataSettingsConfig()
+    tags: SonarrTagsSettingsConfig = SonarrTagsSettingsConfig()
+    general: SonarrGeneralSettingsConfig = SonarrGeneralSettingsConfig()
+    ui: SonarrUISettingsConfig = SonarrUISettingsConfig()
 
     def update_remote(
         self,
         tree: str,
         secrets: SonarrSecrets,
         remote: Self,
         check_unmanaged: bool = False,
@@ -181,15 +171,15 @@
                 self.metadata.delete_remote(f"{tree}.metadata", secrets, remote.metadata),
                 self.general.delete_remote(f"{tree}.general", secrets, remote.general),
                 self.ui.delete_remote(f"{tree}.ui", secrets, remote.ui),
             ],
         )
 
 
-class SonarrInstanceConfig(_SonarrInstanceConfig):
+class SonarrInstanceConfig(ConfigPlugin["SonarrSecrets"]):
     """
     By default, Buildarr will look for a single instance at `http://sonarr:8989`.
     Most configurations are different, and to accommodate those, you can configure
     how Buildarr connects to individual Sonarr instances.
 
     Configuration of a single Sonarr instance:
 
@@ -221,15 +211,15 @@
           hostname: "sonarr2.example.com"
           api_key: "..." # Explicitly define API key
           settings:
             ...
     ```
     """
 
-    hostname: NonEmptyStr = "sonarr"  # type: ignore[assignment]
+    hostname: NonEmptyStr = "sonarr"
     """
     Hostname of the Sonarr instance to connect to.
 
     When defining a single instance using the global `sonarr` configuration block,
     the default hostname is `sonarr`.
 
     When using multiple instance-specific configurations, the default hostname
@@ -239,45 +229,35 @@
     sonarr:
       instances:
         sonarr1: # <--- This becomes the default hostname
           ...
     ```
     """
 
-    port: Port = 8989  # type: ignore[assignment]
+    port: Port = 8989
     """
     Port number of the Sonarr instance to connect to.
     """
 
-    protocol: SonarrProtocol = "http"  # type: ignore[assignment]
+    protocol: SonarrProtocol = "http"
     """
     Communication protocol to use to connect to Sonarr.
     """
 
-    url_base: Optional[str] = None
-    """
-    The URL path the Sonarr instance API is available under, if behind a reverse proxy.
-
-    API URLs are rendered like this: `<protocol>://<hostname>:<port><url_base>/api/v3/...`
-
-    When unset, the URL root will be used as the API endpoint
-    (e.g. `<protocol>://<hostname>:<port>/api/v3/...`).
-
-    *Added in version 0.6.3.*
-    """
+    # url_base is defined in the configuration plugin base class.
 
     api_key: Optional[SonarrApiKey] = None
     """
     API key to use to authenticate with the Sonarr instance.
 
     If undefined or set to `None`, automatically retrieve the API key.
     This can only be done on Sonarr instances with authentication disabled.
     """
 
-    image: NonEmptyStr = "lscr.io/linuxserver/sonarr"  # type: ignore[assignment]
+    image: NonEmptyStr = "lscr.io/linuxserver/sonarr"
     """
     The default Docker image URI when generating a Docker Compose file.
     """
 
     version: Optional[str] = None
     """
     The expected version of the Sonarr instance.
@@ -289,30 +269,26 @@
 
     settings: SonarrSettingsConfig = SonarrSettingsConfig()
     """
     Sonarr settings.
     Configuration options for Sonarr itself are set within this structure.
     """
 
-    @validator("url_base")
-    def validate_url_base(cls, value: Optional[str]) -> Optional[str]:
-        return f"/{value.strip('/')}" if value and value.strip("/") else None
-
     def uses_trash_metadata(self) -> bool:
         if self.settings.quality.uses_trash_metadata():
             return True
         for release_profile in self.settings.profiles.release_profiles.definitions.values():
             if release_profile.uses_trash_metadata():
                 return True
         return False
 
     def render(self) -> Self:
         if not self.uses_trash_metadata():
             return self
-        copy = self.copy(deep=True)
+        copy = self.model_copy(deep=True)
         copy._render()
         return copy
 
     def _render(self) -> None:
         for rp in self.settings.profiles.release_profiles.definitions.values():
             if rp.uses_trash_metadata():
                 rp._render()
```

### Comparing `buildarr_sonarr-0.6.4/buildarr_sonarr/config/connect.py` & `buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/connect.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,29 +12,28 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Sonarr plugin connect settings configuration.
 """
 
-
 from __future__ import annotations
 
 from datetime import datetime
 from logging import getLogger
-from typing import Any, Dict, List, Literal, Mapping, Optional, Set, Tuple, Type, Union
+from typing import Any, ClassVar, Dict, List, Literal, Mapping, Optional, Set, Tuple, Type, Union
 
 from buildarr.config import RemoteMapEntry
 from buildarr.types import BaseEnum, NonEmptyStr, Password, Port
-from pydantic import AnyHttpUrl, ConstrainedInt, EmailStr, Field, SecretStr
+from pydantic import AnyHttpUrl, EmailStr, Field, NonNegativeInt
 from typing_extensions import Annotated, Self
 
 from ..api import api_delete, api_get, api_post, api_put
 from ..secrets import SonarrSecrets
-from .types import SonarrConfigBase, TraktAuthUser
+from .types import SonarrConfigBase
 from .util import trakt_expires_encoder
 
 logger = getLogger(__name__)
 
 
 class OnGrabField(BaseEnum):
     """
@@ -116,22 +115,14 @@
     silent = -2
     quiet = -1
     normal = 0
     high = 1
     emergency = 2
 
 
-class PushoverRetry(ConstrainedInt):
-    """
-    Constrained integer type to enforce Pushover retry field limits.
-    """
-
-    ge = 30
-
-
 class WebhookMethod(BaseEnum):
     """
     HTTP method to use on a webhook connection.
     """
 
     POST = 1
     PUT = 2
@@ -239,15 +230,15 @@
     """
 
     on_application_update: bool = False
     """
     Be notified when Sonarr gets updated to a new version.
     """
 
-    _remote_map: List[RemoteMapEntry] = [
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("on_grab", "onGrab", {}),
         ("on_import", "onDownload", {}),
         ("on_upgrade", "onUpgrade", {}),
         ("on_rename", "onRename", {}),
         ("on_series_delete", "onSeriesDelete", {}),
         ("on_episode_file_delete", "onEpisodeFileDelete", {}),
         ("on_episode_file_delete_for_upgrade", "onEpisodeFileDeleteForUpgrade", {}),
@@ -268,18 +259,18 @@
     """
 
     tags: List[NonEmptyStr] = []
     """
     Sonarr tags to associate this connection with.
     """
 
-    _implementation_name: str
-    _implementation: str
-    _config_contract: str
-    _remote_map: List[RemoteMapEntry]
+    _implementation_name: ClassVar[str]
+    _implementation: ClassVar[str]
+    _config_contract: ClassVar[str]
+    _remote_map: ClassVar[List[RemoteMapEntry]]
 
     @classmethod
     def _get_base_remote_map(
         cls,
         tag_ids: Mapping[str, int],
     ) -> List[RemoteMapEntry]:
         return [
@@ -409,18 +400,18 @@
     """
 
     access_token: Password
     """
     Access token for authenticating with Boxcar.
     """
 
-    _implementation_name: str = "Boxcar"
-    _implementation: str = "Boxcar"
-    _config_contract: str = "BoxcarSettings"
-    _remote_map: List[RemoteMapEntry] = [("access_token", "token", {"is_field": True})]
+    _implementation_name: ClassVar[str] = "Boxcar"
+    _implementation: ClassVar[str] = "Boxcar"
+    _config_contract: ClassVar[str] = "BoxcarSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [("access_token", "token", {"is_field": True})]
 
 
 class CustomscriptConnection(Connection):
     """
     Execute a local script on the Sonarr instance when events occur.
 
     Supported notification triggers: All
@@ -432,18 +423,18 @@
     """
 
     path: NonEmptyStr
     """
     Path of the script to execute.
     """
 
-    _implementation_name: str = "Custom Script"
-    _implementation: str = "CustomScript"
-    _config_contract: str = "CustomScriptSettings"
-    _remote_map: List[RemoteMapEntry] = [("path", "path", {"is_field": True})]
+    _implementation_name: ClassVar[str] = "Custom Script"
+    _implementation: ClassVar[str] = "CustomScript"
+    _config_contract: ClassVar[str] = "CustomScriptSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [("path", "path", {"is_field": True})]
 
 
 class DiscordConnection(Connection):
     """
     Send media update and health alert messages to a Discord server.
 
     Supported notification triggers: All
@@ -572,18 +563,18 @@
             on_import_fields:
               - "overview"
               - "quality"
               - "release"
     ```
     """
 
-    _implementation_name: str = "Discord"
-    _implementation: str = "Discord"
-    _config_contract: str = "DiscordSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation_name: ClassVar[str] = "Discord"
+    _implementation: ClassVar[str] = "Discord"
+    _config_contract: ClassVar[str] = "DiscordSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("webhook_url", "webHookUrl", {"is_field": True}),
         (
             "username",
             "username",
             {"is_field": True, "decoder": lambda v: v or None, "encoder": lambda v: v or ""},
         ),
         (
@@ -622,15 +613,15 @@
     """
 
     server: NonEmptyStr
     """
     Hostname or IP address of the SMTP server to send outbound mail to.
     """
 
-    port: Port = 587  # type: ignore[assignment]
+    port: Port = 587
     """
     The port number on the SMTP server to use to submit mail.
 
     The default is to use STARTTLS on the standard SMTP submission port.
     """
 
     use_encryption: bool = True
@@ -658,56 +649,56 @@
     Email address to send the mail as.
 
     *Changed in version 0.5.3*: Disallow RFC-5322 formatted mailbox addresses
     (e.g. `Sonarr Notifications <sonarr@example.com>`), as they are **not**
     supported by Sonarr V3 (the currently supported version).
     """
 
-    recipient_addresses: Annotated[List[EmailStr], Field(min_items=1, unique_items=True)]
+    recipient_addresses: Annotated[Set[EmailStr], Field(min_length=1)]
     """
     List of email addresses to directly address the mail to.
 
     At least one address must be provided.
 
     *Changed in version 0.5.3*: Disallow RFC-5322 formatted mailbox addresses
     (e.g. `Sonarr Notifications <sonarr@example.com>`), as they are **not**
     supported by Sonarr V3 (the currently supported version).
     """
 
-    cc_addresses: Annotated[List[EmailStr], Field(unique_items=True)] = []
+    cc_addresses: Set[EmailStr] = set()
     """
     Optional list of email addresses to copy (CC) the mail to.
 
     *Changed in version 0.5.3*: Disallow RFC-5322 formatted mailbox addresses
     (e.g. `Sonarr Notifications <sonarr@example.com>`), as they are **not**
     supported by Sonarr V3 (the currently supported version).
     """
 
-    bcc_addresses: Annotated[List[EmailStr], Field(unique_items=True)] = []
+    bcc_addresses: Set[EmailStr] = set()
     """
     Optional list of email addresses to blind copy (BCC) the mail to.
 
     *Changed in version 0.5.3*: Disallow RFC-5322 formatted mailbox addresses
     (e.g. `Sonarr Notifications <sonarr@example.com>`), as they are **not**
     supported by Sonarr V3 (the currently supported version).
     """
 
-    _implementation_name: str = "Email"
-    _implementation: str = "Email"
-    _config_contract: str = "EmailSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation_name: ClassVar[str] = "Email"
+    _implementation: ClassVar[str] = "Email"
+    _config_contract: ClassVar[str] = "EmailSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("server", "server", {"is_field": True}),
         ("port", "port", {"is_field": True}),
         ("use_encryption", "requireEncryption", {"is_field": True}),
         ("username", "username", {"is_field": True}),
         ("password", "password", {"is_field": True}),
         ("from_address", "from", {"is_field": True}),
-        ("recipient_addresses", "to", {"is_field": True}),
-        ("cc_addresses", "cc", {"is_field": True}),
-        ("bcc_addresses", "bcc", {"is_field": True}),
+        ("recipient_addresses", "to", {"is_field": True, "encoder": lambda v: sorted(v)}),
+        ("cc_addresses", "cc", {"is_field": True, "encoder": lambda v: sorted(v)}),
+        ("bcc_addresses", "bcc", {"is_field": True, "encoder": lambda v: sorted(v)}),
     ]
 
 
 class EmbyConnection(Connection):
     """
     Send media update and health alert notifications to an Emby server.
 
@@ -720,15 +711,15 @@
     """
 
     host: NonEmptyStr
     """
     Emby server hostname or IP address.
     """
 
-    port: Port = 8096  # type: ignore[assignment]
+    port: Port = 8096
     """
     Emby server port.
     """
 
     use_ssl: bool = False
     """
     Use HTTPS to connect to Emby, instead of HTTP.
@@ -745,18 +736,18 @@
     """
 
     update_library: bool = False
     """
     Update the Emby library on import, rename, or delete.
     """
 
-    _implementation_name: str = "Emby"
-    _implementation: str = "MediaBrowser"
-    _config_contract: str = "MediaBrowserSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation_name: ClassVar[str] = "Emby"
+    _implementation: ClassVar[str] = "MediaBrowser"
+    _config_contract: ClassVar[str] = "MediaBrowserSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("host", "host", {"is_field": True}),
         ("port", "port", {"is_field": True}),
         ("use_ssl", "useSsl", {"is_field": True}),
         ("api_key", "apiKey", {"is_field": True}),
         ("send_notifications", "notify", {"is_field": True}),
         ("update_library", "updateLibrary", {"is_field": True}),
     ]
@@ -792,18 +783,18 @@
 
     * `min`
     * `low`
     * `normal`
     * `high`
     """
 
-    _implementation: str = "Gotify"
-    _implementation_name: str = "Gotify"
-    _config_contract: str = "GotifySettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation: ClassVar[str] = "Gotify"
+    _implementation_name: ClassVar[str] = "Gotify"
+    _config_contract: ClassVar[str] = "GotifySettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("server", "server", {"is_field": True}),
         ("app_token", "appToken", {"is_field": True}),
         ("priority", "priority", {"is_field": True}),
     ]
 
 
 class JoinConnection(Connection):
@@ -842,18 +833,18 @@
     * `silent`
     * `quiet`
     * `normal`
     * `high`
     * `emergency`
     """
 
-    _implementation: str = "Join"
-    _implementation_name: str = "Join"
-    _config_contract: str = "JoinSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation: ClassVar[str] = "Join"
+    _implementation_name: ClassVar[str] = "Join"
+    _config_contract: ClassVar[str] = "JoinSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("api_key", "apiKey", {"is_field": True}),
         # ("device_ids", "deviceIds", {"is_field": True}),
         (
             "device_names",
             "deviceNames",
             {
                 "is_field": True,
@@ -880,15 +871,15 @@
     """
 
     host: NonEmptyStr
     """
     Kodi hostname or IP address.
     """
 
-    port: Port = 8080  # type: ignore[assignment]
+    port: Port = 8080
     """
     Kodi API port.
     """
 
     use_ssl: bool = False
     """
     Connect to Kodi over HTTPS instead of HTTP.
@@ -905,15 +896,15 @@
     """
 
     gui_notification: bool = False
     """
     Enable showing notifications from Sonarr in the Kodi GUI.
     """
 
-    display_time: int = Field(5, ge=0)  # seconds
+    display_time: NonNegativeInt = 5  # seconds
     """
     How long the notification will be displayed for (in seconds).
     """
 
     update_library: bool = False
     """
     Update the Kodi library on import/rename.
@@ -925,18 +916,18 @@
     """
 
     always_update: bool = False
     """
     Update the Kodi library even when a video is playing.
     """
 
-    _implementation_name: str = "Kodi"
-    _implementation: str = "Xbmc"
-    _config_contract: str = "XbmcSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation_name: ClassVar[str] = "Kodi"
+    _implementation: ClassVar[str] = "Xbmc"
+    _config_contract: ClassVar[str] = "XbmcSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("host", "host", {"is_field": True}),
         ("port", "port", {"is_field": True}),
         ("use_ssl", "useSsl", {"is_field": True}),
         ("username", "username", {"is_field": True}),
         ("password", "password", {"is_field": True}),
         ("gui_notification", "notify", {"is_field": True}),
         ("display_time", "displayTime", {"is_field": True}),
@@ -978,34 +969,34 @@
     """
 
     sender_domain: NonEmptyStr
     """
     The domain from which the mail will be sent.
     """
 
-    recipient_addresses: Annotated[List[EmailStr], Field(min_items=1, unique_items=True)]
+    recipient_addresses: Annotated[Set[EmailStr], Field(min_length=1)]
     """
     The recipient email addresses of the notification mail.
 
     At least one recipient address is required.
 
     *Changed in version 0.5.3*: Disallow RFC-5322 formatted mailbox addresses
     (e.g. `Sonarr Notifications <sonarr@example.com>`), as they are **not**
     supported by Sonarr V3 (the currently supported version).
     """
 
-    _implementation: str = "Mailgun"
-    _implementation_name: str = "MailGun"
-    _config_contract: str = "MailgunSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation: ClassVar[str] = "Mailgun"
+    _implementation_name: ClassVar[str] = "MailGun"
+    _config_contract: ClassVar[str] = "MailgunSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("api_key", "apiKey", {"is_field": True}),
         ("use_eu_endpoint", "useEuEndpoint", {"is_field": True}),
         ("from_address", "from", {"is_field": True}),
         ("sender_domain", "senderDomain", {"is_field": True}),
-        ("recipient_addresses", "recipients", {"is_field": True}),
+        ("recipient_addresses", "recipients", {"is_field": True, "encoder": lambda v: sorted(v)}),
     ]
 
 
 class PlexHomeTheaterConnection(Connection):
     """
     Send media update notifications to a Plex Home Theater instance.
 
@@ -1018,15 +1009,15 @@
     """
 
     host: NonEmptyStr
     """
     Plex Home Theater hostname or IP address.
     """
 
-    port: Port = 3005  # type: ignore[assignment]
+    port: Port = 3005
     """
     Plex Home Theater API port.
     """
 
     use_ssl: bool = False
     """
     Connect to Plex Home Theater over HTTPS instead of HTTP.
@@ -1043,15 +1034,15 @@
     """
 
     gui_notification: bool = False
     """
     Enable showing notifications from Sonarr in the Plex Home Theater GUI.
     """
 
-    display_time: int = Field(5, ge=0)  # seconds
+    display_time: NonNegativeInt = 5  # seconds
     """
     How long the notification will be displayed for (in seconds).
     """
 
     update_library: bool = False
     """
     Update the Plex Home Theater library on import/rename.
@@ -1063,18 +1054,18 @@
     """
 
     always_update: bool = False
     """
     Update the Plex Home THeater library even when a video is playing.
     """
 
-    _implementation_name: str = "Plex Home Theater"
-    _implementation: str = "PlexHomeTheater"
-    _config_contract: str = "PlexHomeTheaterSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation_name: ClassVar[str] = "Plex Home Theater"
+    _implementation: ClassVar[str] = "PlexHomeTheater"
+    _config_contract: ClassVar[str] = "PlexHomeTheaterSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("host", "host", {"is_field": True}),
         ("port", "port", {"is_field": True}),
         ("use_ssl", "useSsl", {"is_field": True}),
         ("username", "username", {"is_field": True}),
         ("password", "password", {"is_field": True}),
         ("gui_notification", "notify", {"is_field": True}),
         ("display_time", "displayTime", {"is_field": True}),
@@ -1097,33 +1088,33 @@
     """
 
     host: NonEmptyStr
     """
     Plex Media Center hostname or IP address.
     """
 
-    port: Port = 3000  # type: ignore[assignment]
+    port: Port = 3000
     """
     Plex Media Center API port.
     """
 
     username: NonEmptyStr
     """
     Username to use to login to Plex Media Center.
     """
 
     password: Password
     """
     Password to use to login to Plex Media Center.
     """
 
-    _implementation_name: str = "Plex Media Center"
-    _implementation: str = "PlexClient"
-    _config_contract: str = "PlexClientSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation_name: ClassVar[str] = "Plex Media Center"
+    _implementation: ClassVar[str] = "PlexClient"
+    _config_contract: ClassVar[str] = "PlexClientSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("host", "host", {"is_field": True}),
         ("port", "port", {"is_field": True}),
         ("username", "username", {"is_field": True}),
         ("password", "password", {"is_field": True}),
     ]
 
 
@@ -1141,15 +1132,15 @@
     """
 
     host: NonEmptyStr
     """
     Plex Media Server hostname or IP address.
     """
 
-    port: Port = 32400  # type: ignore[assignment]
+    port: Port = 32400
     """
     Plex Media Server API port.
     """
 
     use_ssl: bool = False
     """
     Connect to Plex Media Server over HTTPS instead of HTTP.
@@ -1169,18 +1160,18 @@
     # sign_in: Literal["startOAuth"] = "startOAuth"
 
     update_library: bool = True
     """
     Update the Plex Media Server library on import, rename or delete.
     """
 
-    _implementation_name: str = "Plex Media Server"
-    _implementation: str = "PlexServer"
-    _config_contract: str = "PlexServerSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation_name: ClassVar[str] = "Plex Media Server"
+    _implementation: ClassVar[str] = "PlexServer"
+    _config_contract: ClassVar[str] = "PlexServerSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("host", "host", {"is_field": True}),
         ("port", "port", {"is_field": True}),
         ("use_ssl", "useSsl", {"is_field": True}),
         ("auth_token", "authToken", {"is_field": True}),
         ("update_library", "updateLibrary", {"is_field": True}),
     ]
 
@@ -1211,18 +1202,18 @@
     * `verylow`
     * `low`
     * `normal`
     * `high`
     * `emergency`
     """
 
-    _implementation: str = "Prowl"
-    _implementation_name: str = "Prowl"
-    _config_contract: str = "ProwlSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation: ClassVar[str] = "Prowl"
+    _implementation_name: ClassVar[str] = "Prowl"
+    _config_contract: ClassVar[str] = "ProwlSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("api_key", "apiKey", {"is_field": True}),
         ("priority", "priority", {"is_field": True}),
     ]
 
 
 class PushbulletConnection(Connection):
     """
@@ -1257,18 +1248,18 @@
     """
     The device ID to send notifications from
     (`device_iden` in the device's URL on [pushbullet.com](https://pushbullet.com)).
 
     Leave unset, blank or set to `None` to send from yourself.
     """
 
-    _implementation: str = "Pushbullet"
-    _implementation_name: str = "PushBullet"
-    _config_contract: str = "PushBulletSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation: ClassVar[str] = "Pushbullet"
+    _implementation_name: ClassVar[str] = "PushBullet"
+    _config_contract: ClassVar[str] = "PushBulletSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("api_key", "apiKey", {"is_field": True}),
         ("device_ids", "deviceIds", {"is_field": True}),
         ("channel_tags", "channelTags", {"is_field": True}),
         (
             "sender_id",
             "senderId",
             {"is_field": True, "decoder": lambda v: v or None, "encoder": lambda v: v or ""},
@@ -1284,20 +1275,20 @@
     """
 
     type: Literal["pushover"] = "pushover"
     """
     Type value associated with this kind of connection.
     """
 
-    user_key: Annotated[SecretStr, Field(min_length=30, max_length=30)]
+    user_key: Password
     """
     User key to use to authenticate with your Pushover account.
     """
 
-    api_key: Annotated[SecretStr, Field(min_length=30, max_length=30)]
+    api_key: Password
     """
     API key assigned to Sonarr in Pushover.
     """
 
     devices: Set[NonEmptyStr] = set()
     """
     List of device names to send notifications to.
@@ -1314,41 +1305,41 @@
     * `silent`
     * `quiet`
     * `normal`
     * `high`
     * `emergency`
     """
 
-    retry: Union[Literal[0], PushoverRetry] = 0
+    retry: Union[Literal[0], Annotated[int, Field(ge=30)]] = 0
     """
     Interval to retry emergency alerts, in seconds.
 
     Minimum 30 seconds. Set to 0 to disable retrying emergency alerts.
     """
 
     # TODO: Enforce "expire > retry if retry > 0" constraint
-    expire: int = Field(0, ge=0, le=86400)
+    expire: Annotated[int, Field(ge=0, le=86400)] = 0
     """
     Threshold for retrying emergency alerts, in seconds.
     If `retry` is set, this should be set to a higher value.
 
     Maximum 86400 seconds (1 day).
     """
 
     sound: Optional[str] = None
     """
     Notification sound to use on devices.
 
     Leave unset, blank or set to `None` to use the default.
     """
 
-    _implementation_name: str = "Pushover"
-    _implementation: str = "Pushover"
-    _config_contract: str = "PushoverSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation_name: ClassVar[str] = "Pushover"
+    _implementation: ClassVar[str] = "Pushover"
+    _config_contract: ClassVar[str] = "PushoverSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("user_key", "userKey", {"is_field": True}),
         ("api_key", "apiKey", {"is_field": True}),
         ("devices", "devices", {"is_field": True, "encoder": lambda v: sorted(v)}),
         ("priority", "priority", {"is_field": True}),
         ("retry", "retry", {"is_field": True}),
         ("expire", "expire", {"is_field": True}),
         (
@@ -1381,32 +1372,32 @@
     Email address to send the mail as.
 
     *Changed in version 0.5.3*: Disallow RFC-5322 formatted mailbox addresses
     (e.g. `Sonarr Notifications <sonarr@example.com>`), as they are **not**
     supported by Sonarr V3 (the currently supported version).
     """
 
-    recipient_addresses: Annotated[List[EmailStr], Field(min_items=1, unique_items=True)]
+    recipient_addresses: Annotated[Set[EmailStr], Field(min_length=1)]
     """
     The recipient email addresses of the notification mail.
 
     At least one recipient address is required.
 
     *Changed in version 0.5.3*: Disallow RFC-5322 formatted mailbox addresses
     (e.g. `Sonarr Notifications <sonarr@example.com>`), as they are **not**
     supported by Sonarr V3 (the currently supported version).
     """
 
-    _implementation: str = "SendGrid"
-    _implementation_name: str = "SendGrid"
-    _config_contract: str = "SendGridSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation: ClassVar[str] = "SendGrid"
+    _implementation_name: ClassVar[str] = "SendGrid"
+    _config_contract: ClassVar[str] = "SendGridSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("api_key", "apiKey", {"is_field": True}),
         ("from_address", "from", {"is_field": True}),
-        ("recipient_addresses", "recipients", {"is_field": True}),
+        ("recipient_addresses", "recipients", {"is_field": True, "encoder": lambda v: sorted(v)}),
     ]
 
 
 class SlackConnection(Connection):
     """
     Send media update and health alert messages to a Slack channel.
 
@@ -1436,18 +1427,18 @@
     """
 
     channel: Optional[str] = None
     """
     If set, overrides the default channel in the webhook.
     """
 
-    _implementation: str = "Slack"
-    _implementation_name: str = "Slack"
-    _config_contract: str = "SlackSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation: ClassVar[str] = "Slack"
+    _implementation_name: ClassVar[str] = "Slack"
+    _config_contract: ClassVar[str] = "SlackSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("webhook_url", "webHookUrl", {"is_field": True}),
         ("username", "username", {"is_field": True}),
         (
             "icon",
             "icon",
             {"is_field": True, "decoder": lambda v: v or None, "encoder": lambda v: v or ""},
         ),
@@ -1473,18 +1464,20 @@
     """
 
     update_library: bool = True
     """
     Update the library on media import/rename/delete.
     """
 
-    _implementation_name: str = "Synology Indexer"
-    _implementation: str = "SynologyIndexer"
-    _config_contract: str = "SynologyIndexerSettings"
-    _remote_map: List[RemoteMapEntry] = [("update_library", "updateLibrary", {"is_field": True})]
+    _implementation_name: ClassVar[str] = "Synology Indexer"
+    _implementation: ClassVar[str] = "SynologyIndexer"
+    _config_contract: ClassVar[str] = "SynologyIndexerSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
+        ("update_library", "updateLibrary", {"is_field": True}),
+    ]
 
 
 class TelegramConnection(Connection):
     """
     Send media update and health alert messages to a Telegram chat room.
 
     Supported notification triggers: All
@@ -1508,18 +1501,18 @@
     """
 
     send_silently: bool = False
     """
     Sends the message silently. Users will receive a notification with no sound.
     """
 
-    _implementation: str = "Telegram"
-    _implementation_name: str = "Telegram"
-    _config_contract: str = "TelegramSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation: ClassVar[str] = "Telegram"
+    _implementation_name: ClassVar[str] = "Telegram"
+    _config_contract: ClassVar[str] = "TelegramSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("bot_token", "botToken", {"is_field": True}),
         ("chat_id", "chatId", {"is_field": True}),
         ("send_silently", "sendSilently", {"is_field": True}),
     ]
 
 
 class TraktConnection(Connection):
@@ -1561,23 +1554,23 @@
     expires: datetime
     """
     Expiry date-time of the access token, preferably in ISO-8601 format and in UTC.
 
     Example: `2023-05-10T15:34:08.117451Z`
     """
 
-    auth_user: TraktAuthUser
+    auth_user: NonEmptyStr
     """
     The username being authenticated in Trakt.
     """
 
-    _implementation_name: str = "Trakt"
-    _implementation: str = "Trakt"
-    _config_contract: str = "TraktSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation_name: ClassVar[str] = "Trakt"
+    _implementation: ClassVar[str] = "Trakt"
+    _config_contract: ClassVar[str] = "TraktSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("access_token", "accessToken", {"is_field": True}),
         ("refresh_token", "refreshToken", {"is_field": True}),
         ("expires", "expires", {"is_field": True, "encoder": trakt_expires_encoder}),
         ("auth_user", "authUser", {"is_field": True}),
     ]
 
 
@@ -1628,18 +1621,18 @@
     """
 
     direct_message: bool = True
     """
     Send a direct message instead of a public message.
     """
 
-    _implementation_name: str = "Twitter"
-    _implementation: str = "Twitter"
-    _config_contract: str = "TwitterSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation_name: ClassVar[str] = "Twitter"
+    _implementation: ClassVar[str] = "Twitter"
+    _config_contract: ClassVar[str] = "TwitterSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("consumer_key", "consumerKey", {"is_field": True}),
         ("consumer_secret", "consumerSecret", {"is_field": True}),
         ("access_token", "accessToken", {"is_field": True}),
         ("access_token_secret", "accessTokenSecret", {"is_field": True}),
         ("mention", "mention", {"is_field": True}),
         ("direct_message", "direct_message", {"is_field": True}),
     ]
@@ -1678,18 +1671,18 @@
     """
 
     password: Password
     """
     Webhook API password.
     """
 
-    _implementation_name: str = "Webhook"
-    _implementation: str = "Webhook"
-    _config_contract: str = "WebhookSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation_name: ClassVar[str] = "Webhook"
+    _implementation: ClassVar[str] = "Webhook"
+    _config_contract: ClassVar[str] = "WebhookSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("url", "url", {"is_field": True}),
         ("method", "method", {"is_field": True}),
         ("username", "username", {"is_field": True}),
         ("password", "password", {"is_field": True}),
     ]
```

### Comparing `buildarr_sonarr-0.6.4/buildarr_sonarr/config/download_clients/__init__.py` & `buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/download_clients/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,18 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Sonarr plugin download client settings.
 """
 
-
 from __future__ import annotations
 
 from logging import getLogger
-from typing import Dict, List, Mapping, Union
+from typing import ClassVar, Dict, List, Mapping, Union
 
 from buildarr.config import RemoteMapEntry
 from pydantic import Field
 from typing_extensions import Annotated, Self
 
 from ...api import api_get, api_put
 from ...secrets import SonarrSecrets
@@ -123,23 +122,25 @@
     """
 
     definitions: Dict[str, Annotated[DownloadClientType, Field(discriminator="type")]] = {}
     """
     Download client definitions, for connecting with external media downloaders.
     """
 
-    remote_path_mappings = SonarrRemotePathMappingsSettingsConfig()
+    remote_path_mappings: SonarrRemotePathMappingsSettingsConfig = (
+        SonarrRemotePathMappingsSettingsConfig()
+    )
     """
     Configuration for mapping paths on download client hosts to their counterparts
     on this Sonarr instance.
 
     For more information, refer to "Configuring remote path mappings".
     """
 
-    _remote_map: List[RemoteMapEntry] = [
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("enable_completed_download_handling", "enableCompletedDownloadHandling", {}),
         ("redownload_failed", "autoRedownloadFailed", {}),
     ]
 
     @classmethod
     def from_remote(cls, secrets: SonarrSecrets) -> Self:
         downloadclient_config = api_get(secrets, "/api/v3/config/downloadclient")
```

### Comparing `buildarr_sonarr-0.6.4/buildarr_sonarr/config/download_clients/download_clients.py` & `buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/download_clients/download_clients.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,23 +12,22 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Sonarr plugin download client definition.
 """
 
-
 from __future__ import annotations
 
 from logging import getLogger
-from typing import Any, Dict, List, Literal, Mapping, Optional, Set, Tuple, Type
+from typing import Any, ClassVar, Dict, List, Literal, Mapping, Optional, Set, Tuple, Type
 
 from buildarr.config import RemoteMapEntry
-from buildarr.types import BaseEnum, NonEmptyStr, Password, Port
-from pydantic import SecretStr, validator
+from buildarr.types import BaseEnum, NonEmptyStr, Password, Port, SecretStr
+from pydantic import ValidationInfo, field_validator
 from typing_extensions import Self
 
 from ...api import api_delete, api_post, api_put
 from ...secrets import SonarrSecrets
 from ..types import SonarrConfigBase
 
 logger = getLogger(__name__)
@@ -289,18 +288,18 @@
     """
     Sonarr tags to assign to the download clients.
     Only media under those tags will be assigned to this client.
 
     If no tags are assigned, all media can use the client.
     """
 
-    _implementation_name: str
-    _implementation: str
-    _config_contract: str
-    _remote_map: List[RemoteMapEntry]
+    _implementation_name: ClassVar[str]
+    _implementation: ClassVar[str]
+    _config_contract: ClassVar[str]
+    _remote_map: ClassVar[List[RemoteMapEntry]]
 
     @classmethod
     def _get_base_remote_map(cls, tag_ids: Mapping[str, int]) -> List[RemoteMapEntry]:
         return [
             ("enable", "enable", {}),
             ("priority", "priority", {}),
             ("remove_completed_downloads", "removeCompletedDownloads", {}),
@@ -411,15 +410,15 @@
     """
 
     host: NonEmptyStr
     """
     Download Station host name.
     """
 
-    port: Port = 5000  # type: ignore[assignment]
+    port: Port = 5000
     """
     Download client access port.
     """
 
     use_ssl: bool = False
     """
     Use a secure connection when connecting to the download client.
@@ -447,18 +446,18 @@
     directory: Optional[str] = None
     """
     Optional shared folder to put downloads into.
 
     Leave blank, set to `null` or undefined to use the default download client location.
     """
 
-    _implementation_name: str = "Download Station"
-    _implementation: str = "UsenetDownloadStation"
-    _config_contract: str = "DownloadStationSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation_name: ClassVar[str] = "Download Station"
+    _implementation: ClassVar[str] = "UsenetDownloadStation"
+    _config_contract: ClassVar[str] = "DownloadStationSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("host", "host", {"is_field": True}),
         ("port", "port", {"is_field": True}),
         ("use_ssl", "useSsl", {"is_field": True}),
         ("username", "username", {"is_field": True}),
         ("password", "password", {"is_field": True}),
         (
             "category",
@@ -484,15 +483,15 @@
     """
 
     host: NonEmptyStr
     """
     NZBGet host name.
     """
 
-    port: Port = 5000  # type: ignore[assignment]
+    port: Port = 5000
     """
     Download client access port.
     """
 
     use_ssl: bool = False
     """
     Use a secure connection when connecting to the download client.
@@ -552,18 +551,18 @@
     add_paused: bool = False
     """
     Add media to the download client in the paused state.
 
     This option requires NZBGet version 16.0 or later.
     """
 
-    _implementation_name: str = "NZBGet"
-    _implementation: str = "Nzbget"
-    _config_contract: str = "NzbgetSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation_name: ClassVar[str] = "NZBGet"
+    _implementation: ClassVar[str] = "Nzbget"
+    _config_contract: ClassVar[str] = "NzbgetSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("host", "host", {"is_field": True}),
         ("port", "port", {"is_field": True}),
         ("use_ssl", "useSsl", {"is_field": True}),
         (
             "url_base",
             "urlBase",
             {"is_field": True, "decoder": lambda v: v or None, "encoder": lambda v: v or ""},
@@ -592,15 +591,15 @@
     """
 
     host: NonEmptyStr
     """
     NZBVortex host name.
     """
 
-    port: Port = 4321  # type: ignore[assignment]
+    port: Port = 4321
     """
     Download client access port.
     """
 
     use_ssl: bool = False
     """
     Use a secure connection when connecting to the download client.
@@ -642,18 +641,18 @@
     Values:
 
     * `low`
     * `normal`
     * `high`
     """
 
-    _implementation_name: str = "NZBVortex"
-    _implementation: str = "NzbVortex"
-    _config_contract: str = "NzbVortexSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation_name: ClassVar[str] = "NZBVortex"
+    _implementation: ClassVar[str] = "NzbVortex"
+    _config_contract: ClassVar[str] = "NzbVortexSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("host", "host", {"is_field": True}),
         ("port", "port", {"is_field": True}),
         ("use_ssl", "useSsl", {"is_field": True}),
         (
             "url_base",
             "urlBase",
             {"is_field": True, "decoder": lambda v: v or None, "encoder": lambda v: v or ""},
@@ -687,18 +686,18 @@
     """
 
     strm_folder: NonEmptyStr
     """
     Folder from which `.strm` files will be imported by Drone.
     """
 
-    _implementation_name: str = "Pneumatic"
-    _implementation: str = "Pneumatic"
-    _config_contract: str = "PneumaticSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation_name: ClassVar[str] = "Pneumatic"
+    _implementation: ClassVar[str] = "Pneumatic"
+    _config_contract: ClassVar[str] = "PneumaticSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("nzb_folder", "nzbFolder", {"is_field": True}),
         ("strm_folder", "strmFolder", {"is_field": True}),
     ]
 
 
 class SabnzbdDownloadClient(UsenetDownloadClient):
     """
@@ -711,15 +710,15 @@
     """
 
     host: NonEmptyStr
     """
     SABnzbd host name.
     """
 
-    port: Port = 4321  # type: ignore[assignment]
+    port: Port = 4321
     """
     Download client access port.
     """
 
     use_ssl: bool = False
     """
     Use a secure connection when connecting to the download client.
@@ -767,18 +766,18 @@
     * `paused`
     * `low`
     * `normal`
     * `high`
     * `force`
     """
 
-    _implementation_name: str = "SABnzbd"
-    _implementation: str = "Sabnzbd"
-    _config_contract: str = "SabnzbdSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation_name: ClassVar[str] = "SABnzbd"
+    _implementation: ClassVar[str] = "Sabnzbd"
+    _config_contract: ClassVar[str] = "SabnzbdSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("host", "host", {"is_field": True}),
         ("port", "port", {"is_field": True}),
         ("use_ssl", "useSsl", {"is_field": True}),
         (
             "url_base",
             "urlBase",
             {
@@ -815,18 +814,18 @@
     """
 
     watch_folder: NonEmptyStr
     """
     Folder from which Sonarr should import completed downloads.
     """
 
-    _implementation_name: str = "Usenet Blackhole"
-    _implementation: str = "UsenetBlackhole"
-    _config_contract: str = "UsenetBlackholeSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation_name: ClassVar[str] = "Usenet Blackhole"
+    _implementation: ClassVar[str] = "UsenetBlackhole"
+    _config_contract: ClassVar[str] = "UsenetBlackholeSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("nzb_folder", "nzbFolder", {"is_field": True}),
         ("watch_folder", "watchFolder", {"is_field": True}),
     ]
 
 
 class Aria2DownloadClient(TorrentDownloadClient):
     """
@@ -839,38 +838,38 @@
     """
 
     host: NonEmptyStr
     """
     Aria2 host name.
     """
 
-    port: Port = 6800  # type: ignore[assignment]
+    port: Port = 6800
     """
     Download client access port.
     """
 
     use_ssl: bool = False
     """
     Use a secure connection when connecting to the download client.
     """
 
-    rpc_path: NonEmptyStr = "/rpc"  # type: ignore[assignment]
+    rpc_path: NonEmptyStr = "/rpc"
     """
     XML RPC path in the Aria2 client URL.
     """
 
     secret_token: Password
     """
     Secret token to use to authenticate with the download client.
     """
 
-    _implementation_name: str = "Aria2"
-    _implementation: str = "Aria2"
-    _config_contract: str = "Aria2Settings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation_name: ClassVar[str] = "Aria2"
+    _implementation: ClassVar[str] = "Aria2"
+    _config_contract: ClassVar[str] = "Aria2Settings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("host", "host", {"is_field": True}),
         ("port", "port", {"is_field": True}),
         ("use_ssl", "useSsl", {"is_field": True}),
         ("rpc_path", "rpcPath", {"is_field": True}),
         ("secret_token", "secretToken", {"is_field": True}),
     ]
 
@@ -886,15 +885,15 @@
     """
 
     host: NonEmptyStr
     """
     Deluge host name.
     """
 
-    port: Port = 8112  # type: ignore[assignment]
+    port: Port = 8112
     """
     Download client access port.
     """
 
     use_ssl: bool = False
     """
     Use a secure connection when connecting to the download client.
@@ -942,18 +941,18 @@
 
     Values:
 
     * `last`
     * `first`
     """
 
-    _implementation_name: str = "Deluge"
-    _implementation: str = "Deluge"
-    _config_contract: str = "DelugeSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation_name: ClassVar[str] = "Deluge"
+    _implementation: ClassVar[str] = "Deluge"
+    _config_contract: ClassVar[str] = "DelugeSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("host", "host", {"is_field": True}),
         ("port", "port", {"is_field": True}),
         ("use_ssl", "useSsl", {"is_field": True}),
         (
             "url_base",
             "urlBase",
             {"is_field": True, "decoder": lambda v: v or None, "encoder": lambda v: v or ""},
@@ -985,15 +984,15 @@
     """
 
     host: NonEmptyStr
     """
     Download Station host name.
     """
 
-    port: Port = 5000  # type: ignore[assignment]
+    port: Port = 5000
     """
     Download client access port.
     """
 
     use_ssl: bool = False
     """
     Use a secure connection when connecting to the download client.
@@ -1021,18 +1020,18 @@
     directory: Optional[str] = None
     """
     Optional shared folder to put downloads into.
 
     Leave blank, set to `null` or undefined to use the default download client location.
     """
 
-    _implementation_name: str = "Download Station"
-    _implementation: str = "TorrentDownloadStation"
-    _config_contract: str = "DownloadStationSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation_name: ClassVar[str] = "Download Station"
+    _implementation: ClassVar[str] = "TorrentDownloadStation"
+    _config_contract: ClassVar[str] = "DownloadStationSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("host", "host", {"is_field": True}),
         ("port", "port", {"is_field": True}),
         ("use_ssl", "useSsl", {"is_field": True}),
         ("username", "username", {"is_field": True}),
         ("password", "password", {"is_field": True}),
         (
             "category",
@@ -1058,15 +1057,15 @@
     """
 
     host: NonEmptyStr
     """
     Flood host name.
     """
 
-    port: Port = 3000  # type: ignore[assignment]
+    port: Port = 3000
     """
     Download client access port.
     """
 
     use_ssl: bool = False
     """
     Use a secure connection when connecting to the download client.
@@ -1088,15 +1087,15 @@
     """
 
     destination: Optional[str] = None
     """
     Manually specified download destination.
     """
 
-    flood_tags: Set[NonEmptyStr] = {"sonarr"}  # type: ignore[arg-type]
+    flood_tags: Set[NonEmptyStr] = {"sonarr"}
     """
     Initial tags of a download within Flood.
 
     To be recognized, a download must have all initial tags.
     This avoids conflicts with unrelated downloads.
     """
 
@@ -1111,18 +1110,18 @@
     """
 
     start_on_add: bool = True
     """
     Immediately start download once the media has been added to the client.
     """
 
-    _implementation_name: str = "Flood"
-    _implementation: str = "Flood"
-    _config_contract: str = "FloodSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation_name: ClassVar[str] = "Flood"
+    _implementation: ClassVar[str] = "Flood"
+    _config_contract: ClassVar[str] = "FloodSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("host", "host", {"is_field": True}),
         ("port", "port", {"is_field": True}),
         ("use_ssl", "useSsl", {"is_field": True}),
         (
             "url_base",
             "urlBase",
             {"is_field": True, "decoder": lambda v: v or None, "encoder": lambda v: v or ""},
@@ -1161,15 +1160,15 @@
     """
 
     host: NonEmptyStr
     """
     Hadouken host name.
     """
 
-    port: Port = 7070  # type: ignore[assignment]
+    port: Port = 7070
     """
     Download client access port.
     """
 
     use_ssl: bool = False
     """
     Use a secure connection when connecting to the download client.
@@ -1186,26 +1185,26 @@
     """
 
     password: Password
     """
     Password to use to authenticate the download client user.
     """
 
-    category: NonEmptyStr = "sonarr-tv"  # type: ignore[assignment]
+    category: NonEmptyStr = "sonarr-tv"
     """
     Associate media from Sonarr with a category.
 
     Adding a category specific to Sonarr avoids conflicts with unrelated non-Sonarr downloads.
     Using a category is optional, but strongly recommended.
     """
 
-    _implementation_name: str = "Hadouken"
-    _implementation: str = "Hadouken"
-    _config_contract: str = "HadoukenSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation_name: ClassVar[str] = "Hadouken"
+    _implementation: ClassVar[str] = "Hadouken"
+    _config_contract: ClassVar[str] = "HadoukenSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("host", "host", {"is_field": True}),
         ("port", "port", {"is_field": True}),
         ("use_ssl", "useSsl", {"is_field": True}),
         (
             "url_base",
             "urlBase",
             {"is_field": True, "decoder": lambda v: v or None, "encoder": lambda v: v or ""},
@@ -1227,15 +1226,15 @@
     """
 
     host: NonEmptyStr
     """
     qBittorrent host name.
     """
 
-    port: Port = 8080  # type: ignore[assignment]
+    port: Port = 8080
     """
     Download client access port.
     """
 
     use_ssl: bool = False
     """
     Use a secure connection when connecting to the download client.
@@ -1309,18 +1308,18 @@
     first_and_last_first: bool = False
     """
     Download first and last pieces of a file first.
 
     This option requires qBittorrent version 4.1.0 or later.
     """
 
-    _implementation_name: str = "qBittorrent"
-    _implementation: str = "QBittorrent"
-    _config_contract: str = "QBittorrentSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation_name: ClassVar[str] = "qBittorrent"
+    _implementation: ClassVar[str] = "QBittorrent"
+    _config_contract: ClassVar[str] = "QBittorrentSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("host", "host", {"is_field": True}),
         ("port", "port", {"is_field": True}),
         ("use_ssl", "useSsl", {"is_field": True}),
         (
             "url_base",
             "urlBase",
             {
@@ -1389,25 +1388,25 @@
     """
 
     host: NonEmptyStr
     """
     RTorrent host name.
     """
 
-    port: Port = 8080  # type: ignore[assignment]
+    port: Port = 8080
     """
     Download client access port.
     """
 
     use_ssl: bool = False
     """
     Use a secure connection when connecting to the download client.
     """
 
-    url_base: NonEmptyStr = "RPC2"  # type: ignore[assignment]
+    url_base: NonEmptyStr = "RPC2"
     """
     Path to the XMLRPC endpoint, e.g. `http(s)://[host]:[port]/[url_base]`.
 
     When using RTorrent this usually is `RPC2` or `plugins/rpc/rpc.php`.
     """
 
     username: NonEmptyStr
@@ -1470,18 +1469,18 @@
     add_stopped: bool = False
     """
     Enabling will add torrents and magnets to RTorrent in a stopped state.
 
     This may break magnet files.
     """
 
-    _implementation_name: str = "rTorrent"
-    _implementation: str = "RTorrent"
-    _config_contract: str = "RTorrentSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation_name: ClassVar[str] = "rTorrent"
+    _implementation: ClassVar[str] = "RTorrent"
+    _config_contract: ClassVar[str] = "RTorrentSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("host", "host", {"is_field": True}),
         ("port", "port", {"is_field": True}),
         ("use_ssl", "useSsl", {"is_field": True}),
         ("url_base", "urlBase", {"is_field": True}),
         ("username", "username", {"is_field": True}),
         ("password", "password", {"is_field": True}),
         (
@@ -1528,29 +1527,29 @@
     save_magnet_files: bool = False
     """
     Save the magnet link if no `.torrent` file is available.
 
     Only useful if the download client supports magnets saved to a file.
     """
 
-    magnet_file_extension: NonEmptyStr = ".magnet"  # type: ignore[assignment]
+    magnet_file_extension: NonEmptyStr = ".magnet"
     """
     Extension to use for magnet links.
     """
 
     read_only: bool = True
     """
     Instead of moving files, this will instruct Sonarr to copy or hard link
     (depending on settings/system configuration).
     """
 
-    _implementation_name: str = "Torrent Blackhole"
-    _implementation: str = "TorrentBlackhole"
-    _config_contract: str = "TorrentBlackholeSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation_name: ClassVar[str] = "Torrent Blackhole"
+    _implementation: ClassVar[str] = "TorrentBlackhole"
+    _config_contract: ClassVar[str] = "TorrentBlackholeSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("host", "host", {"is_field": True}),
         ("port", "port", {"is_field": True}),
         ("use_ssl", "useSsl", {"is_field": True}),
         ("url_base", "urlBase", {"is_field": True}),
         ("username", "username", {"is_field": True}),
         ("password", "password", {"is_field": True}),
         (
@@ -1580,25 +1579,25 @@
     """
 
     host: NonEmptyStr
     """
     Transmission/Vuze host name.
     """
 
-    port: Port = 9091  # type: ignore[assignment]
+    port: Port = 9091
     """
     Download client access port.
     """
 
     use_ssl: bool = False
     """
     Use a secure connection when connecting to the download client.
     """
 
-    url_base: NonEmptyStr = "/transmission/"  # type: ignore[assignment]
+    url_base: NonEmptyStr = "/transmission/"
     """
     Adds a prefix to the Transmission/Vuze RPC url, e.g.`http://[host]:[port][url_base]rpc`.
 
     This is set by default in most clients to `/transmission/`.
     """
 
     username: Optional[str] = None
@@ -1652,16 +1651,16 @@
     """
 
     add_paused: bool = False
     """
     Add media to the download client in the Paused state.
     """
 
-    _config_contract: str = "TransmissionSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _config_contract: ClassVar[str] = "TransmissionSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("host", "host", {"is_field": True}),
         ("port", "port", {"is_field": True}),
         ("use_ssl", "useSsl", {"is_field": True}),
         ("url_base", "urlBase", {"is_field": True}),
         (
             "username",
             "username",
@@ -1679,56 +1678,58 @@
             {"is_field": True, "decoder": lambda v: v or None, "encoder": lambda v: v or ""},
         ),
         ("recent_priority", "recentTvPriority", {"is_field": True}),
         ("older_priority", "olderTvPriority", {"is_field": True}),
         ("add_paused", "addPaused", {"is_field": True}),
     ]
 
-    @validator("directory")
+    @field_validator("directory")
+    @classmethod
     def category_directory_mutual_exclusion(
         cls,
         value: Optional[str],
-        values: Mapping[str, Any],
+        info: ValidationInfo,
     ) -> Optional[str]:
-        directory = value
-        category: Optional[str] = values.get("category", None)
-        if directory and category:
+        category: Optional[str] = info.data.get("category", None)
+        if value and category:
             raise ValueError(
-                "'directory' and 'category' are mutually exclusive "
-                "on a Transmission download client",
+                (
+                    "'directory' and 'category' are mutually exclusive "
+                    "on a Transmission download client"
+                ),
             )
-        return directory
+        return value
 
 
 class TransmissionDownloadClient(TransmissionDownloadClientBase):
     """
     Tramsmission download client.
     """
 
     type: Literal["transmission"] = "transmission"
     """
     Type value associated with this kind of download client.
     """
 
-    _implementation_name: str = "Transmission"
-    _implementation: str = "Transmission"
+    _implementation_name: ClassVar[str] = "Transmission"
+    _implementation: ClassVar[str] = "Transmission"
 
 
 class VuzeDownloadClient(TransmissionDownloadClientBase):
     """
     Vuze download client.
     """
 
     type: Literal["vuze"] = "vuze"
     """
     Type value associated with this kind of download client.
     """
 
-    _implementation_name: str = "Vuze"
-    _implementation: str = "Vuze"
+    _implementation_name: ClassVar[str] = "Vuze"
+    _implementation: ClassVar[str] = "Vuze"
 
 
 class UtorrentDownloadClient(TorrentDownloadClient):
     """
     uTorrent download client.
     """
 
@@ -1738,15 +1739,15 @@
     """
 
     host: NonEmptyStr
     """
     uTorrent host name.
     """
 
-    port: Port = 8080  # type: ignore[assignment]
+    port: Port = 8080
     """
     Download client access port.
     """
 
     use_ssl: bool = False
     """
     Use a secure connection when connecting to the download client.
@@ -1804,18 +1805,18 @@
     """
 
     initial_state: UtorrentState = UtorrentState.start
     """
     Initial state for torrents added to uTorrent.
     """
 
-    _implementation_name: str = "uTorrent"
-    _implementation: str = "UTorrent"
-    _config_contract: str = "UTorrentSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation_name: ClassVar[str] = "uTorrent"
+    _implementation: ClassVar[str] = "UTorrent"
+    _config_contract: ClassVar[str] = "UTorrentSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("host", "host", {"is_field": True}),
         ("port", "port", {"is_field": True}),
         ("use_ssl", "useSsl", {"is_field": True}),
         (
             "url_base",
             "urlBase",
             {"is_field": True, "decoder": lambda v: v or None, "encoder": lambda v: v or ""},
```

### Comparing `buildarr_sonarr-0.6.4/buildarr_sonarr/config/download_clients/remote_path_mappings.py` & `buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/download_clients/remote_path_mappings.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,22 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Sonarr plugin download client remote path mappings.
 """
 
-
 from __future__ import annotations
 
 from logging import getLogger
-from typing import Any, Dict, List, Mapping, Tuple
+from typing import Any, ClassVar, Dict, List, Mapping, Tuple
 
 from buildarr.config import RemoteMapEntry
 from buildarr.types import BaseEnum, NonEmptyStr
-from pydantic import validator
+from pydantic import field_validator
 from typing_extensions import Self
 
 from ...api import api_delete, api_get, api_post, api_put
 from ...secrets import SonarrSecrets
 from ...types import OSAgnosticPath
 from ..types import SonarrConfigBase
 
@@ -91,21 +90,22 @@
     If set to `present`, the resource is created on the remote instance if it does not exist.
 
     If set to `absent`, the resource will be destroyed on the remote instance if it exists.
     This takes effect even if the  `delete_unmanaged` is set to `False`
     for all remote path mappings.
     """
 
-    _remote_map: List[RemoteMapEntry] = [
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("host", "host", {}),
         ("remote_path", "remotePath", {}),
         ("local_path", "localPath", {}),
     ]
 
-    @validator("remote_path", "local_path")
+    @field_validator("remote_path", "local_path")
+    @classmethod
     def add_trailing_slash(cls, value: OSAgnosticPath) -> OSAgnosticPath:
         if value.is_windows():
             return (value + "\\") if not value.endswith("\\\\") else value
         return (value + "/") if not value.endswith("/") else value
 
     @classmethod
     def _from_remote(cls, remote_attrs: Mapping[str, Any]) -> Self:
```

### Comparing `buildarr_sonarr-0.6.4/buildarr_sonarr/config/general.py` & `buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/general.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,24 +12,23 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Sonarr plugin general settings configuration.
 """
 
-
 from __future__ import annotations
 
 from ipaddress import IPv4Address
-from typing import Any, Dict, List, Literal, Mapping, Optional, Set, Tuple, Union
+from typing import Any, ClassVar, Dict, List, Literal, Mapping, Optional, Set, Tuple, Union
 
 from buildarr.config import RemoteMapEntry
-from buildarr.types import BaseEnum, NonEmptyStr, Password, Port
-from pydantic import Field, validator
-from typing_extensions import Self
+from buildarr.types import BaseEnum, NonEmptyStr, Port, SecretStr
+from pydantic import Field
+from typing_extensions import Annotated, Self
 
 from ..api import api_get, api_put
 from ..secrets import SonarrSecrets
 from .types import SonarrConfigBase
 
 
 class AuthenticationMethod(BaseEnum):
@@ -85,15 +84,15 @@
 
 
 class GeneralSettings(SonarrConfigBase):
     """
     Sonarr general settings base class.
     """
 
-    _remote_map: List[RemoteMapEntry]
+    _remote_map: ClassVar[List[RemoteMapEntry]]
 
     @classmethod
     def _from_remote(cls, remote_attrs: Mapping[str, Any]) -> Self:
         return cls(**cls.get_local_attrs(cls._remote_map, remote_attrs))
 
     def _update_remote_attrs(
         self,
@@ -129,25 +128,25 @@
     or `*` to bind on all interfaces.
 
     Unless you run Sonarr directly on a host machine (i.e. not via Docker) and
     want Sonarr to only be available on a specific network or interface,
     this generally should be left untouched.
     """
 
-    port: Port = 8989  # type: ignore[assignment]
+    port: Port = 8989
     """
     Unencrypted (HTTP) listening port for Sonarr.
 
     If Sonarr is being run via Docker in the default bridge mode,
     this setting shouldn't be changed.
     Instead, change the external port it is bound to using
     `--publish <port number>:8989`.
     """
 
-    ssl_port: Port = 9898  # type: ignore[assignment]
+    ssl_port: Port = 9898
     """
     Encrypted (HTTPS) listening port for Sonarr.
 
     If Sonarr is being run via Docker in the default bridge mode,
     this setting shouldn't be changed.
     Instead, change the external port it is bound to using
     `--publish <port number>:9898`.
@@ -165,21 +164,21 @@
     Add a prefix to all Sonarr URLs,
     e.g. `http://localhost:8989/<url_base>/settings/general`.
 
     Generally used to accommodate reverse proxies where Sonarr
     is assigned to a subfolder, e.g. `https://example.com/sonarr`.
     """
 
-    instance_name: NonEmptyStr = "Sonarr"  # type: ignore[assignment]
+    instance_name: NonEmptyStr = "Sonarr"
     """
     Instance name in the browser tab and in syslog.
     """
 
-    _remote_map: List[RemoteMapEntry] = [
-        ("bind_address", "bindAddress", {}),
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
+        ("bind_address", "bindAddress", {"encoder": lambda v: str(v)}),
         ("port", "port", {}),
         ("ssl_port", "sslPort", {}),
         ("use_ssl", "enableSsl", {}),
         ("url_base", "urlBase", {"decoder": lambda v: v or None, "encoder": lambda v: v or ""}),
         ("instance_name", "instanceName", {}),
     ]
 
@@ -206,15 +205,15 @@
     username: Optional[str] = None
     """
     Username for the administrator user. Required if authentication is enabled.
 
     Requires a restart of Sonarr to take effect.
     """
 
-    password: Optional[Password] = None
+    password: Optional[SecretStr] = None
     """
     Password for the administrator user. Required if authentication is enabled.
 
     Requires a restart of Sonarr to take effect.
     """
 
     certificate_validation: CertificateValidation = CertificateValidation.enabled
@@ -225,15 +224,15 @@
     Values:
 
     * `enabled` - Validate HTTPS certificates for all hosts
     * `local-disabled` - Disable HTTPS certificate validation for hosts on the local network
     * `disabled` - Disable HTTPS certificate validation completely
     """
 
-    _remote_map: List[RemoteMapEntry] = [
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("authentication", "authenticationMethod", {}),
         (
             "username",
             "username",
             {
                 # Set to default value (`None`) if not found on remote.
                 "optional": True,
@@ -256,46 +255,14 @@
                 # Sonarr isn't too picky about this, but replicate the behaviour of the UI.
                 "encoder": lambda v: v.get_secret_value() if v else "",
             },
         ),
         ("certificate_validation", "certificateValidation", {}),
     ]
 
-    @validator("username", "password")
-    def required_when_auth_enabled(
-        cls,
-        value: Optional[str],
-        values: Dict[str, Any],
-    ) -> Optional[str]:
-        """
-        Enforce the following constraints on the validated attributes:
-
-        * If `authentication` is `none`, set the attribute value to `None`.
-        * If `authentication` is a value other than `none` (i.e. require authentication),
-          ensure that the attribute set to a value other than `None`.
-
-        This will apply to both the local Buildarr configuration and
-        the remote Sonarr instance configuration.
-
-        Args:
-            value (Optional[str]): Value to validate
-            values (Dict[str, Any]): Configuration attributes
-
-        Raises:
-            ValueError: If the attribute is required but empty
-
-        Returns:
-            Validated attribute value
-        """
-        if values["authentication"] == AuthenticationMethod.none:
-            return None
-        elif not value:
-            raise ValueError("required when 'authentication' is not set to 'none'")
-        return value
-
 
 class ProxyGeneralSettings(GeneralSettings):
     """
     Proxy configuration for Sonarr.
     """
 
     enable: bool = False
@@ -318,26 +285,26 @@
     hostname: Optional[str] = None
     """
     Proxy server hostname.
 
     Required if using a proxy is enabled.
     """
 
-    port: Port = 8080  # type: ignore[assignment]
+    port: Port = 8080
     """
     Proxy server access port.
     """
 
     username: Optional[str] = None
     """
     Username to authenticate with.
     Only enter if authentication is required by the proxy.
     """
 
-    password: Optional[Password] = None
+    password: Optional[SecretStr] = None
     """
     Password for the proxy user.
     Only enter if authentication is required by the proxy.
     """
 
     ignored_addresses: Set[NonEmptyStr] = set()
     """
@@ -345,15 +312,15 @@
     """
 
     bypass_proxy_for_local_addresses: bool = True
     """
     Do not use the proxy to access local network addresses.
     """
 
-    _remote_map: List[RemoteMapEntry] = [
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("enable", "proxyEnabled", {}),
         ("proxy_type", "proxyType", {}),
         (
             "hostname",
             "proxyHostname",
             {"decoder": lambda v: v or None, "encoder": lambda v: v or ""},
         ),
@@ -397,15 +364,15 @@
     Values:
 
     * `INFO` - Standard log output
     * `DEBUG` - Debugging log output
     * `TRACE` - Trace diagnostics log output
     """
 
-    _remote_map: List[RemoteMapEntry] = [("log_level", "logLevel", {})]
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [("log_level", "logLevel", {})]
 
 
 class AnalyticsGeneralSettings(GeneralSettings):
     """
     Configuration of analytics and telemetry from within Sonarr.
     """
 
@@ -416,23 +383,25 @@
     This includes information on your browser, which Sonarr Web UI pages you use,
     error reporting and OS/runtime versions. This information is reportedly used
     to prioritise features and bug fixes.
 
     Requires a restart of Sonarr to take effect.
     """
 
-    _remote_map: List[RemoteMapEntry] = [("send_anonymous_usage_data", "analyticsEnabled", {})]
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
+        ("send_anonymous_usage_data", "analyticsEnabled", {}),
+    ]
 
 
 class UpdatesGeneralSettings(GeneralSettings):
     """
     Settings for updating Sonarr.
     """
 
-    branch: NonEmptyStr = "main"  # type: ignore[assignment]
+    branch: NonEmptyStr = "main"
     """
     Branch used by the external update mechanism.
     Changing this value has no effect on Docker installations.
 
     If unsure, leave this undefined in Buildarr and use the value already set in Sonarr.
     """
 
@@ -465,15 +434,15 @@
     """
     Path to a custom script that takes an extracted update package
     and handles the remainder of the update process.
 
     Required if `mechanism` is set to `script`.
     """
 
-    _remote_map: List[RemoteMapEntry] = [
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("branch", "branch", {}),
         ("automatic", "updateAutomatically", {}),
         ("mechanism", "updateMechanism", {}),
         (
             "script_path",
             "updateScriptPath",
             {"decoder": lambda v: v or None, "encoder": lambda v: v or ""},
@@ -482,37 +451,37 @@
 
 
 class BackupGeneralSettings(GeneralSettings):
     """
     Settings for Sonarr automatic backups.
     """
 
-    folder: NonEmptyStr = "Backups"  # type: ignore[assignment]
+    folder: NonEmptyStr = "Backups"
     """
     Folder to backup Sonarr data to.
 
     Relative paths will be under Sonarr's AppData directory.
     """
 
-    interval: int = Field(7, ge=1, le=7)  # days
+    interval: Annotated[int, Field(ge=1, le=7)] = 7  # days
     """
     Interval between automatic backups, in days.
 
     Must be set somewhere between 1 and 7 days.
     """
 
-    retention: int = Field(28, ge=1, le=90)  # days
+    retention: Annotated[int, Field(ge=1, le=90)] = 28  # days
     """
     Retention period for backups, in days.
     Backups older than the retention period will be cleaned up automatically.
 
     Must be set somewhere between 1 and 90 days.
     """
 
-    _remote_map: List[RemoteMapEntry] = [
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("folder", "backupFolder", {}),
         ("interval", "backupInterval", {}),
         ("retention", "backupRetention", {}),
     ]
 
 
 class SonarrGeneralSettingsConfig(SonarrConfigBase):
@@ -522,15 +491,15 @@
 
     host: HostGeneralSettings = HostGeneralSettings()
     security: SecurityGeneralSettings = SecurityGeneralSettings()
     proxy: ProxyGeneralSettings = ProxyGeneralSettings()
     logging: LoggingGeneralSettings = LoggingGeneralSettings()
     analytics: AnalyticsGeneralSettings = AnalyticsGeneralSettings()
     updates: UpdatesGeneralSettings = UpdatesGeneralSettings()
-    backup: BackupGeneralSettings = BackupGeneralSettings()  # type: ignore[call-arg]
+    backup: BackupGeneralSettings = BackupGeneralSettings()
 
     @classmethod
     def from_remote(cls, secrets: SonarrSecrets) -> Self:
         settings = api_get(secrets, "/api/v3/config/host")
         return cls(
             host=HostGeneralSettings._from_remote(settings),
             security=SecurityGeneralSettings._from_remote(settings),
```

### Comparing `buildarr_sonarr-0.6.4/buildarr_sonarr/config/import_lists.py` & `buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/import_lists.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,21 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Sonarr plugin import list settings configuration.
 """
 
-
 from __future__ import annotations
 
-import re
-
 from datetime import datetime
 from logging import getLogger
 from typing import (
     Any,
+    ClassVar,
     Dict,
     Iterable,
     List,
     Literal,
     Mapping,
     Optional,
     Set,
@@ -36,37 +34,35 @@
     Type,
     Union,
     cast,
 )
 
 from buildarr.config import RemoteMapEntry
 from buildarr.state import state
-from buildarr.types import BaseEnum, InstanceName, NonEmptyStr, Password
-from pydantic import AnyHttpUrl, ConstrainedStr, Field, PositiveInt, validator
+from buildarr.types import BaseEnum, InstanceReference, NonEmptyStr, Password, SecretStr
+from pydantic import (
+    AnyHttpUrl,
+    Field,
+    NonNegativeInt,
+    PositiveInt,
+    StringConstraints,
+    ValidationInfo,
+    field_validator,
+)
 from typing_extensions import Annotated, Self
 
 from ..api import api_delete, api_get, api_post, api_put
 from ..secrets import SonarrSecrets
 from ..types import SonarrApiKey
-from .types import SonarrConfigBase, TraktAuthUser
+from .types import SonarrConfigBase
 from .util import trakt_expires_encoder
 
 logger = getLogger(__name__)
 
 
-class YearRange(ConstrainedStr):
-    """
-    Constrained string type for a singular year or range of years.
-    """
-
-    regex = re.compile(r"[0-9]+(?:-[0-9]+)?")
-
-    # TODO: validate that the end year is higher than the start year
-
-
 class Monitor(BaseEnum):
     """
     Enumeration for what kind of monitoring should be done in an import list.
     """
 
     all_episodes = "all"
     future_episodes = "future"
@@ -184,18 +180,18 @@
     """
 
     tags: Set[NonEmptyStr] = set()
     """
     Tags to assign to items imported from this import list.
     """
 
-    _implementation_name: str
-    _implementation: str
-    _config_contract: str
-    _remote_map: List[RemoteMapEntry]
+    _implementation_name: ClassVar[str]
+    _implementation: ClassVar[str]
+    _config_contract: ClassVar[str]
+    _remote_map: ClassVar[List[RemoteMapEntry]]
 
     @classmethod
     def _get_base_remote_map(
         cls,
         quality_profile_ids: Mapping[str, int],
         language_profile_ids: Mapping[str, int],
         tag_ids: Mapping[str, int],
@@ -484,22 +480,21 @@
     expires: datetime
     """
     Expiry date-time of the access token, preferably in ISO-8601 format and in UTC.
 
     Example: `2023-05-10T15:34:08.117451Z`
     """
 
-    auth_user: TraktAuthUser
+    auth_user: NonEmptyStr
     """
     The username being authenticated in Trakt.
     """
 
-    # rating
     # TODO: constraints
-    rating: NonEmptyStr = "0-100"  # type: ignore[assignment]
+    rating: NonEmptyStr = "0-100"
     """
     Filter series by rating range, with a maximum range of 0-100.
     """
 
     username: Optional[str] = None
     """
     Username for the list to import from.
@@ -508,15 +503,15 @@
     """
 
     genres: Set[NonEmptyStr] = set()
     """
     Filter series by Trakt genre slug.
     """
 
-    years: Optional[YearRange] = None
+    years: Optional[Annotated[str, StringConstraints(pattern=r"[0-9]+(?:-[0-9]+)?")]] = None
     """
     Filter series by year or year range. (e.g. `2009` or `2009-2015`)
     """
 
     limit: PositiveInt = 100
     """
     Limit the number of series to get.
@@ -642,15 +637,15 @@
     """
 
     type: Literal["sonarr"] = "sonarr"
     """
     Type value associated with this kind of import list.
     """
 
-    instance_name: Optional[InstanceName] = Field(None, plugin="sonarr")
+    instance_name: Optional[Annotated[str, InstanceReference(plugin_name="sonarr")]] = None
     """
     The name of the Sonarr instance within Buildarr, if linking this Sonarr instance
     with another Buildarr-defined Sonarr instance.
 
     *New in version 0.3.0.*
     """
 
@@ -663,60 +658,63 @@
     """
     API key used to access the source Sonarr instance.
 
     If a Sonarr instance managed by Buildarr is not referenced using `instance_name`,
     this attribute is required.
     """
 
-    source_quality_profiles: Set[Union[PositiveInt, NonEmptyStr]] = Field(
-        set(),
-        alias="source_quality_profile_ids",
-    )
+    source_quality_profiles: Annotated[
+        Set[Union[NonNegativeInt, NonEmptyStr]],
+        Field(alias="source_quality_profile_ids"),
+    ] = set()
     """
     List of IDs (or names) of the quality profiles on the source instance to import from.
 
     Quality profile names can only be used if `instance_name` is used to
     link to a Buildarr-defined Sonarr instance.
     If linking to a Sonarr instance outside Buildarr, IDs must be used.
 
     *Changed in version 0.3.0*: Renamed from `source_quality_profile_ids`
     (which is still valid as an alias), and added support for quality profile names.
     """
 
-    source_language_profiles: Set[Union[PositiveInt, NonEmptyStr]] = Field(
-        set(),
-        alias="source_language_profile_ids",
-    )
+    source_language_profiles: Annotated[
+        Set[Union[NonNegativeInt, NonEmptyStr]],
+        Field(alias="source_language_profile_ids"),
+    ] = set()
     """
     List of IDs (or names) of the language profiles on the source instance to import from.
 
     Language profile names can only be used if `instance_name` is used to
     link to a Buildarr-defined Sonarr instance.
     If linking to a Sonarr instance outside Buildarr, IDs must be used.
 
     *Changed in version 0.3.0*: Renamed from `source_language_profile_ids`
     (which is still valid as an alias), and added support for language profile names.
     """
 
-    source_tags: Set[Union[PositiveInt, NonEmptyStr]] = Field(set(), alias="source_tag_ids")
+    source_tags: Annotated[
+        Set[Union[NonNegativeInt, NonEmptyStr]],
+        Field(alias="source_tag_ids"),
+    ] = set()
     """
     List of IDs (or names) of the tags on the source instance to import from.
 
     Tag names can only be used if `instance_name` is used to
     link to a Buildarr-defined Sonarr instance.
     If linking to a Sonarr instance outside Buildarr, IDs must be used.
 
     *Changed in version 0.3.0*: Renamed from `source_tag_ids`
     (which is still valid as an alias), and added support for tag names.
     """
 
-    _implementation_name: str = "Sonarr"
-    _implementation: str = "SonarrImport"
-    _config_contract: str = "SonarrSettings"
-    _remote_map: List[RemoteMapEntry] = []
+    _implementation_name: ClassVar[str] = "Sonarr"
+    _implementation: ClassVar[str] = "SonarrImport"
+    _config_contract: ClassVar[str] = "SonarrSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = []
 
     @classmethod
     def _get_base_remote_map(
         cls,
         quality_profile_ids: Mapping[str, int],
         language_profile_ids: Mapping[str, int],
         tag_ids: Mapping[str, int],
@@ -787,65 +785,38 @@
             profile_type (str): Name of the resource to get in the Sonarr API.
 
         Returns:
             List of resource API objects
         """
         return api_get(cls._get_secrets(instance_name), f"/api/v3/{resource_type}")
 
-    @validator("api_key", always=True)
+    @field_validator("api_key")
+    @classmethod
     def validate_api_key(
         cls,
-        value: Optional[SonarrApiKey],
-        values: Mapping[str, Any],
-    ) -> Optional[SonarrApiKey]:
-        """
-        Validate the `api_key` attribute after parsing.
-
-        Args:
-            value (Optional[str]): `api_key` value.
-            values (Mapping[str, Any]): Currently parsed attributes. `instance_name` is checked.
-
-        Raises:
-            ValueError: If `api_key` is undefined when `instance_name` is also undefined.
-
-        Returns:
-            Validated `api_key` value
-        """
-        if not values.get("instance_name", None) and not value:
+        value: Optional[SecretStr],
+        info: ValidationInfo,
+    ) -> Optional[SecretStr]:
+        if not info.data.get("instance_name") and not value:
             raise ValueError("required if 'instance_name' is undefined")
         return value
 
-    @validator(
-        "source_quality_profiles",
-        "source_language_profiles",
-        "source_tags",
-        each_item=True,
-    )
-    def validate_source_resource_ids(
+    @field_validator("source_quality_profiles", "source_language_profiles", "source_tags")
+    @classmethod
+    def validate_source_resources(
         cls,
-        value: Union[int, str],
-        values: Dict[str, Any],
-    ) -> Union[int, str]:
-        """
-        Validate that all resource references are IDs (integers) if `instance_name` is undefined.
-
-        Args:
-            value (Union[int, str]): Resource reference (ID or name).
-            values (Mapping[str, Any]): Currently parsed attributes. `instance_name` is checked.
-
-        Raises:
-            ValueError: If the resource reference is a name and `instance_name` is undefined.
-
-        Returns:
-            Validated resource reference
-        """
-        if not values.get("instance_name", None) and not isinstance(value, int):
-            raise ValueError(
-                "values must be IDs (not names) if 'instance_name' is undefined",
-            )
+        value: Set[Union[str, int]],
+        info: ValidationInfo,
+    ) -> Set[Union[str, int]]:
+        if not info.data.get("instance_name"):
+            for v in value:
+                if not isinstance(v, int):
+                    raise ValueError(
+                        "values must be IDs (not names) if 'instance_name' is undefined",
+                    )
         return value
 
     @classmethod
     def _encode_source_resources(
         cls,
         instance_name: Optional[str],
         resources: Iterable[Union[str, int]],
@@ -929,15 +900,15 @@
             source_resources=self.source_tags,
             resource_type_int="tag",
             resource_type_ext="tag",
             resource_description="tag",
             ignore_nonexistent_ids=ignore_nonexistent_ids,
             name_key="label",
         )
-        return self.copy(
+        return self.model_copy(
             update={
                 "instance_name": instance_name,
                 "api_key": api_key,
                 "source_quality_profiles": source_quality_profiles,
                 "source_language_profiles": source_language_profiles,
                 "source_tags": source_tags,
             },
@@ -1039,18 +1010,20 @@
     Plex authentication token.
 
     If unsure on where to find this token,
     [follow this guide from Plex.tv][PATH].
     [PATH]: https://support.plex.tv/articles/204059436-finding-an-authentication-token-x-plex-token
     """
 
-    _implementation_name: str = "Plex Watchlist"
-    _implementation: str = "PlexImport"
-    _config_contract: str = "PlexListSettings"
-    _remote_map: List[RemoteMapEntry] = [("access_token", "accessToken", {"is_field": True})]
+    _implementation_name: ClassVar[str] = "Plex Watchlist"
+    _implementation: ClassVar[str] = "PlexImport"
+    _config_contract: ClassVar[str] = "PlexListSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
+        ("access_token", "accessToken", {"is_field": True}),
+    ]
 
 
 class TraktListImportList(TraktImportList):
     """
     Import an arbitrary list from Trakt into Sonarr.
     """
 
@@ -1062,18 +1035,18 @@
     list_name: NonEmptyStr
     """
     Name of the list to import.
 
     The list must be public, or you must have access to the list.
     """
 
-    _implementation_name: str = "Trakt List"
-    _implementation: str = "TraktListImport"
-    _config_contract: str = "TraktListSettings"
-    _remote_map: List[RemoteMapEntry] = [("list_name", "listName", {"is_field": True})]
+    _implementation_name: ClassVar[str] = "Trakt List"
+    _implementation: ClassVar[str] = "TraktListImport"
+    _config_contract: ClassVar[str] = "TraktListSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [("list_name", "listName", {"is_field": True})]
 
 
 class TraktPopularlistImportList(TraktImportList):
     """
     Import media according to popularity-based lists on Trakt.
     """
 
@@ -1097,18 +1070,20 @@
     * `top_watched_by_alltime`
     * `recommended_by_week`
     * `recommended_by_month`
     * `recommended_by_year`
     * `recommended_by_alltime`
     """
 
-    _implementation_name: str = "Trakt Popular List"
-    _implementation: str = "TraktPopularImport"
-    _config_contract: str = "TraktPopularSettings"
-    _remote_map: List[RemoteMapEntry] = [("list_type", "traktListType", {"is_field": True})]
+    _implementation_name: ClassVar[str] = "Trakt Popular List"
+    _implementation: ClassVar[str] = "TraktPopularImport"
+    _config_contract: ClassVar[str] = "TraktPopularSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
+        ("list_type", "traktListType", {"is_field": True}),
+    ]
 
 
 class TraktUserImportList(TraktImportList):
     """
     Import a user-level list from Trakt.
     """
 
@@ -1124,18 +1099,20 @@
     Values:
 
     * `user_watch_list`
     * `user_watched_list`
     * `user_collection_list`
     """
 
-    _implementation_name: str = "Trakt User"
-    _implementation: str = "TraktUserImport"
-    _config_contract: str = "TraktUserSettings"
-    _remote_map: List[RemoteMapEntry] = [("list_type", "traktListType", {"is_field": True})]
+    _implementation_name: ClassVar[str] = "Trakt User"
+    _implementation: ClassVar[str] = "TraktUserImport"
+    _config_contract: ClassVar[str] = "TraktUserSettings"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
+        ("list_type", "traktListType", {"is_field": True}),
+    ]
 
 
 IMPORTLIST_TYPES: Tuple[Type[ImportList], ...] = (
     SonarrImportList,
     PlexWatchlistImportList,
     TraktListImportList,
     TraktPopularlistImportList,
```

### Comparing `buildarr_sonarr-0.6.4/buildarr_sonarr/config/indexers.py` & `buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/indexers.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Sonarr plugin indexers settings configuration.
 """
 
-
 from __future__ import annotations
 
 from logging import getLogger
 from typing import (
     Any,
+    ClassVar,
     Dict,
     Iterable,
     List,
     Literal,
     Mapping,
     Optional,
     Set,
@@ -33,15 +33,15 @@
     Type,
     Union,
     cast,
 )
 
 from buildarr.config import RemoteMapEntry
 from buildarr.types import BaseEnum, NonEmptyStr, Password, RssUrl
-from pydantic import AnyHttpUrl, Field, PositiveInt, validator
+from pydantic import AnyHttpUrl, Field, NonNegativeInt, PositiveInt, field_validator
 from typing_extensions import Annotated, Self
 
 from ..api import api_delete, api_get, api_post, api_put
 from ..secrets import SonarrSecrets
 from .types import SonarrConfigBase
 
 logger = getLogger(__name__)
@@ -129,15 +129,15 @@
     """
 
     enable_interactive_search: bool = True
     """
     If enabled, use this indexer for manual interactive searches.
     """
 
-    priority: int = Field(25, ge=1, le=50, alias="indexer_priority")
+    priority: Annotated[int, Field(ge=1, le=50, alias="indexer_priority")] = 25
     """
     Priority of this indexer to prefer one indexer over another in release tiebreaker scenarios.
 
     1 is highest priority and 50 is lowest priority.
 
     *Changed in version 0.4.1*: Renamed from `indexer_priority` to `priority`.
     The original name is still available as an alias.
@@ -150,18 +150,18 @@
 
     tags: List[NonEmptyStr] = []
     """
     Only use this indexer for series with at least one matching tag.
     Leave blank to use with all series.
     """
 
-    _implementation: str
-    _implementation_name: str
-    _config_contract: str
-    _remote_map: List[RemoteMapEntry]
+    _implementation: ClassVar[str]
+    _implementation_name: ClassVar[str]
+    _config_contract: ClassVar[str]
+    _remote_map: ClassVar[List[RemoteMapEntry]]
 
     @classmethod
     def _get_base_remote_map(
         cls,
         download_client_ids: Mapping[str, int],
         tag_ids: Mapping[str, int],
     ) -> List[RemoteMapEntry]:
@@ -342,15 +342,15 @@
     """
     Also search for anime using the standard numbering. Only applies for Anime series types.
     """
 
     _implementation = "Fanzub"
     _implementation_name = "Fanzub"
     _config_contract = "FanzubSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("rss_url", "rssUrl", {"is_field": True}),
         ("anime_standard_format_search", "animeStandardFormatSearch", {"is_field": True}),
     ]
 
 
 class NewznabIndexer(UsenetIndexer):
     """
@@ -365,15 +365,15 @@
     """
 
     url: AnyHttpUrl
     """
     URL of the Newznab-compatible indexing site.
     """
 
-    api_path: NonEmptyStr = "/api"  # type: ignore[assignment]
+    api_path: NonEmptyStr = "/api"
     """
     Newznab API endpoint. Usually `/api`.
     """
 
     api_key: Password
     """
     API key for use with the Newznab API.
@@ -436,15 +436,15 @@
     """
     Additional Newznab API parameters.
     """
 
     _implementation = "Newznab"
     _implementation_name = "Newznab"
     _config_contract = "NewznabSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("url", "baseUrl", {"is_field": True}),
         ("api_path", "apiPath", {"is_field": True}),
         ("api_key", "apiKey", {"is_field": True}),
         (
             "categories",
             "categories",
             {"is_field": True, "encoder": lambda v: sorted(NabCategory.encode(c) for c in v)},
@@ -458,15 +458,16 @@
         (
             "additional_parameters",
             "additionalParameters",
             {"is_field": True, "field_default": None, "decoder": lambda v: v or None},
         ),
     ]
 
-    @validator("categories", "anime_categories")
+    @field_validator("categories", "anime_categories")
+    @classmethod
     def validate_categories(
         cls,
         value: Iterable[Union[NabCategory, int]],
     ) -> Set[Union[NabCategory, int]]:
         return set(
             NabCategory.decode(category) if isinstance(category, int) else category
             for category in value
@@ -489,23 +490,23 @@
     """
 
     api_key: Password
     """
     API key for the OmgWtfNZBs API.
     """
 
-    delay: int = Field(30, ge=0)  # minutes
+    delay: NonNegativeInt = 30  # minutes
     """
     Time (in minutes) to delay new NZBs before they appear on the RSS feed.
     """
 
     _implementation = "Omgwtfnzbs"
     _implementation_name = "omgwtfnzbs"
     _config_contract = "OmgwtfnzbsSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("username", "username", {"is_field": True}),
         ("api_key", "apiKey", {"is_field": True}),
         ("delay", "delay", {"is_field": True}),
     ]
 
 
 class BroadcasthenetIndexer(TorrentIndexer):
@@ -514,28 +515,28 @@
     """
 
     type: Literal["broadcasthenet"] = "broadcasthenet"
     """
     Type value associated with this kind of indexer.
     """
 
-    api_url: AnyHttpUrl = "https://api.broadcasthe.net"  # type: ignore[assignment]
+    api_url: AnyHttpUrl = AnyHttpUrl("https://api.broadcasthe.net")
     """
     BroadcasTheNet API URL.
     """
 
     api_key: Password
     """
     BroadcasTheNet API key.
     """
 
     _implementation = "BroadcastheNet"
     _implementation_name = "BroadcasTheNet"
     _config_contract = "BroadcastheNetSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("api_url", "apiUrl", {"is_field": True}),
         ("api_key", "apiKey", {"is_field": True}),
     ]
 
 
 class FilelistIndexer(TorrentIndexer):
     """
@@ -553,15 +554,15 @@
     """
 
     passkey: Password
     """
     FileList account API key.
     """
 
-    api_url: AnyHttpUrl = "https://filelist.io"  # type: ignore[assignment]
+    api_url: AnyHttpUrl = AnyHttpUrl("https://filelist.io")
     """
     FileList API URL.
 
     Do not change this unless you know what you're doing,
     as your API key will be sent to this host.
     """
 
@@ -600,15 +601,15 @@
     * `TV SD`
     * `Sport`
     """
 
     _implementation = "FileList"
     _implementation_name = "FileList"
     _config_contract = "FilelistSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("username", "username", {"is_field": True}),
         ("passkey", "passKey", {"is_field": True}),
         ("api_url", "apiUrl", {"is_field": True}),
         (
             "categories",
             "categories",
             {"is_field": True, "encoder": lambda v: sorted(c.value for c in v)},
@@ -637,26 +638,26 @@
     """
 
     api_key: Password
     """
     HDBits API key assigned to the account.
     """
 
-    api_url: AnyHttpUrl = "https://hdbits.org"  # type: ignore[assignment]
+    api_url: AnyHttpUrl = AnyHttpUrl("https://hdbits.org")
     """
     HDBits API URL.
 
     Do not change this unless you know what you're doing,
     as your API key will be sent to this host.
     """
 
     _implementation = "HDBits"
     _implementation_name = "HDBits"
     _config_contract = "HDBitsSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("username", "username", {"is_field": True}),
         ("api_key", "apiKey", {"is_field": True}),
         ("api_url", "apiUrl", {"is_field": True}),
     ]
 
 
 class IptorrentsIndexer(TorrentIndexer):
@@ -681,15 +682,15 @@
     The full RSS feed url generated by IP Torrents, using only the categories
     you selected (HD, SD, x264, etc ...).
     """
 
     _implementation = "IPTorrents"
     _implementation_name = "IP Torrents"
     _config_contract = "IptorrentsSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("feed_url", "feedUrl", {"is_field": True}),
     ]
 
 
 class NyaaIndexer(TorrentIndexer):
     """
     Monitor for new anime releases on the configured Nyaa domain.
@@ -719,15 +720,15 @@
     Note that if you change the category, you will have to add
     required/restricted rules about the subgroups to avoid foreign language releases.
     """
 
     _implementation = "Nyaa"
     _implementation_name = "Nyaa"
     _config_contract = "NyaaSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("website_url", "websiteUrl", {"is_field": True}),
         ("anime_standard_format_search", "animeStandardFormatSearch", {"is_field": True}),
         (
             "additional_parameters",
             "additionalParameters",
             {"is_field": True, "field_default": None, "decoder": lambda v: v or None},
         ),
@@ -758,15 +759,15 @@
     """
     CAPTCHA clearance token used to handle CloudFlare anti-DDoS measures on shared-IP VPNs.
     """
 
     _implementation = "Rarbg"
     _implementation_name = "Rarbg"
     _config_contract = "RarbgSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("api_url", "apiUrl", {"is_field": True}),
         ("ranked_only", "rankedOnly", {"is_field": True}),
         (
             "captcha_token",
             "captchaToken",
             {"is_field": True, "decoder": lambda v: v or None, "encoder": lambda v: v or ""},
         ),
@@ -809,15 +810,15 @@
 
     As size checks will not be performed, be careful when enabling this option.
     """
 
     _implementation = "TorrentRssIndexer"
     _implementation_name = "Torrent RSS Feed"
     _config_contract = "TorrentRssIndexerSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("full_rss_feed_url", "feedUrl", {"is_field": True}),
         (
             "cookie",
             "cookie",
             {"is_field": True, "decoder": lambda v: v or None, "encoder": lambda v: v or ""},
         ),
         ("allow_zero_size", "allowZeroSize", {"is_field": True}),
@@ -836,28 +837,28 @@
     """
     Type value associated with this kind of indexer.
     """
 
     # NOTE: automatic_search and interactive_search are not supported
     # by this indexer, therefore its value is ignored.
 
-    website_url: AnyHttpUrl = "http://rss.torrentleech.org"  # type: ignore[assignment]
+    website_url: AnyHttpUrl = AnyHttpUrl("http://rss.torrentleech.org")
     """
     TorrentLeech feed API URL.
     """
 
     api_key: Password
     """
     TorrentLeech API key.
     """
 
     _implementation = "Torrentleech"
     _implementation_name = "TorrentLeech"
     _config_contract = "TorrentleechSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("website_url", "baseUrl", {"is_field": True}),
         ("api_key", "apiKey", {"is_field": True}),
     ]
 
 
 class TorznabIndexer(TorrentIndexer):
     """
@@ -872,15 +873,15 @@
     """
 
     url: AnyHttpUrl
     """
     URL of the Torznab-compatible indexing site.
     """
 
-    api_path: NonEmptyStr = "/api"  # type: ignore[assignment]
+    api_path: NonEmptyStr = "/api"
     """
     Tornab API endpoint. Usually `/api`.
     """
 
     api_key: Password
     """
     API key for use with the Torznab API.
@@ -942,15 +943,15 @@
     """
     Additional Torznab API parameters.
     """
 
     _implementation = "Torznab"
     _implementation_name = "Torznab"
     _config_contract = "TorznabSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("url", "baseUrl", {"is_field": True}),
         ("api_path", "apiPath", {"is_field": True}),
         ("api_key", "apiKey", {"is_field": True}),
         (
             "categories",
             "categories",
             {"is_field": True, "encoder": lambda v: sorted(NabCategory.encode(c) for c in v)},
@@ -964,15 +965,16 @@
         (
             "additional_parameters",
             "additionalParameters",
             {"is_field": True, "field_default": None, "decoder": lambda v: v or None},
         ),
     ]
 
-    @validator("categories", "anime_categories")
+    @field_validator("categories", "anime_categories")
+    @classmethod
     def validate_categories(
         cls,
         value: Iterable[Union[NabCategory, int]],
     ) -> Set[Union[NabCategory, int]]:
         return set(
             NabCategory.decode(category) if isinstance(category, int) else category
             for category in value
@@ -1049,37 +1051,36 @@
     The following parameters are available for configuring indexers and
     how they are handled by Sonarr.
 
     For more information on how Sonarr finds epsiodes, refer to the FAQ on
     [WikiArr](https://wiki.servarr.com/sonarr/faq#how-does-sonarr-find-episodes).
     """
 
-    minimum_age: int = Field(0, ge=0)  # minutes
+    minimum_age: NonNegativeInt = 0  # minutes
     """
     Minimum age (in minutes) of NZBs before they are grabbed. (Usenet only)
 
     Use this to give new releases time to propagate to your Usenet provider.
     """
 
-    retention: int = Field(0, ge=0)  # days
+    retention: NonNegativeInt = 0  # days
     """
     Retention of releases. (Usenet only)
 
     Set to `0` for unlimited retention.
     """
 
-    # Set to 0 for unlimited
-    maximum_size: int = Field(0, ge=0)  # MB
+    maximum_size: NonNegativeInt = 0  # MB
     """
     Maximum size for a release to be grabbed, in megabytes (MB).
 
     Set to `0` to set for unlimited size.
     """
 
-    rss_sync_interval: int = Field(15, ge=0)  # minutes
+    rss_sync_interval: NonNegativeInt = 15  # minutes
     """
     Interval (in minutes) to sync RSS feeds with indexers.
 
     Set to `0` to disable syncing. This also disables automatic release grabbing.
     """
 
     # TODO: Take into account the indexers created by Prowlarr instances.
@@ -1094,15 +1095,15 @@
     """
 
     definitions: Dict[str, Annotated[IndexerType, Field(discriminator="type")]] = {}
     """
     Indexers to manage via Buildarr are defined here.
     """
 
-    _remote_map: List[RemoteMapEntry] = [
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("minimum_age", "minimumAge", {}),
         ("retention", "retention", {}),
         ("maximum_size", "maximumSize", {}),
         ("rss_sync_interval", "rssSyncInterval", {}),
     ]
 
     @classmethod
```

### Comparing `buildarr_sonarr-0.6.4/buildarr_sonarr/config/media_management.py` & `buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/media_management.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,24 +12,23 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Sonarr plugin media management settings configuration.
 """
 
-
 from __future__ import annotations
 
 from logging import getLogger
-from typing import Any, Dict, List, Optional, Set, cast
+from typing import Any, ClassVar, Dict, List, Optional, Set, cast
 
 from buildarr.config import RemoteMapEntry
 from buildarr.types import BaseEnum, NonEmptyStr
-from pydantic import Field
-from typing_extensions import Self
+from pydantic import Field, NonNegativeInt
+from typing_extensions import Annotated, Self
 
 from ..api import api_delete, api_get, api_post, api_put
 from ..secrets import SonarrSecrets
 from .types import SonarrConfigBase
 
 logger = getLogger(__name__)
 
@@ -141,15 +140,15 @@
     """
     Replace illegal characters within the file name.
 
     If set to `False`, Sonarr will remove them instead.
     """
 
     standard_episode_format: NonEmptyStr = (
-        "{Series TitleYear} - "  # type: ignore[assignment]
+        "{Series TitleYear} - "
         "S{season:00}E{episode:00} - "
         "{Episode CleanTitle} "
         "[{Preferred Words }{Quality Full}]"
         "{[MediaInfo VideoDynamicRangeType]}"
         "{[Mediainfo AudioCodec}{ Mediainfo AudioChannels]}"
         "{MediaInfo AudioLanguages}"
         "{[MediaInfo VideoCodec]}"
@@ -160,15 +159,15 @@
 
     The default specified here is the current TRaSH-Guides recommended format,
     but it will not be applied to the Sonarr instance unless it is explicitly
     defined in the configuration file.
     """
 
     daily_episode_format: NonEmptyStr = (
-        "{Series TitleYear} - "  # type: ignore[assignment]
+        "{Series TitleYear} - "
         "{Air-Date} - "
         "{Episode CleanTitle} "
         "[{Preferred Words }{Quality Full}]"
         "{[MediaInfo VideoDynamicRangeType]}"
         "{[Mediainfo AudioCodec}{ Mediainfo AudioChannels]}"
         "{MediaInfo AudioLanguages}"
         "{[MediaInfo VideoCodec]}"
@@ -179,15 +178,15 @@
 
     The default specified here is the current TRaSH-Guides recommended format,
     but it will not be applied to the Sonarr instance unless it is explicitly
     defined in the configuration file.
     """
 
     anime_episode_format: NonEmptyStr = (
-        "{Series TitleYear} - "  # type: ignore[assignment]
+        "{Series TitleYear} - "
         "S{season:00}E{episode:00} - "
         "{absolute:000} - "
         "{Episode CleanTitle} "
         "[{Preferred Words }{Quality Full}]"
         "{[MediaInfo VideoDynamicRangeType]}"
         "[{MediaInfo VideoBitDepth}bit]"
         "{[MediaInfo VideoCodec]}"
@@ -199,33 +198,33 @@
     File renaming format for an anime episode file.
 
     The default specified here is the current TRaSH-Guides recommended format,
     but it will not be applied to the Sonarr instance unless it is explicitly
     defined in the configuration file.
     """
 
-    series_folder_format: NonEmptyStr = "{Series TitleYear}"  # type: ignore[assignment]
+    series_folder_format: NonEmptyStr = "{Series TitleYear}"
     """
     Renaming format for a series folder.
 
     The default specified here is the current TRaSH-Guides recommended format,
     but it will not be applied to the Sonarr instance unless it is explicitly
     defined in the configuration file.
     """
 
-    season_folder_format: NonEmptyStr = "Season {season:00}"  # type: ignore[assignment]
+    season_folder_format: NonEmptyStr = "Season {season:00}"
     """
     Renaming format for a season folder of a series.
 
     The default specified here is the current TRaSH-Guides recommended format,
     but it will not be applied to the Sonarr instance unless it is explicitly
     defined in the configuration file.
     """
 
-    specials_folder_format: NonEmptyStr = "Specials"  # type: ignore[assignment]
+    specials_folder_format: NonEmptyStr = "Specials"
     """
     Renaming format for a specials folder of a series.
 
     The default specified here is the current TRaSH-Guides recommended format,
     but it will not be applied to the Sonarr instance unless it is explicitly
     defined in the configuration file.
     """
@@ -270,15 +269,15 @@
     skip_free_space_check: bool = False
     """
     Skip the free space check for the series root folder.
 
     Only enable when Sonarr is unable to detect free space from your series root folder.
     """
 
-    minimum_free_space: int = Field(100, ge=100)  # MB
+    minimum_free_space: Annotated[int, Field(ge=100)] = 100  # MB
     """
     Prevent import if it would leave less than the specified
     amount of disk space (in megabytes) available.
 
     Minimum value is 100 MB.
     """
 
@@ -368,20 +367,20 @@
     sonarr:
       settings:
         media_management:
           change_file_date: "none"
     ```
     """
 
-    recycling_bin: Optional[NonEmptyStr] = None
+    recycling_bin: Optional[str] = None
     """
     Episode files will go here when deleted instead of being permanently deleted.
     """
 
-    recycling_bin_cleanup: int = Field(7, ge=0)  # days
+    recycling_bin_cleanup: NonNegativeInt = 7  # days
     """
     Files in the recycle bin older than the selected number of days
     will be cleaned up automatically.
 
     Set to 0 to disable automatic cleanup.
     """
 
@@ -449,27 +448,27 @@
     you want Sonarr to scan are defined in Buildarr,
     as Sonarr might remove imported media from its database
     when root folder definitions are deleted.
 
     *New in version 0.1.2.*
     """
 
-    _naming_remote_map: List[RemoteMapEntry] = [
+    _naming_remote_map: ClassVar[List[RemoteMapEntry]] = [
         # Episode Naming
         ("rename_episodes", "renameEpisodes", {}),
         ("replace_illegal_characters", "replaceIllegalCharacters", {}),
         ("standard_episode_format", "standardEpisodeFormat", {}),
         ("daily_episode_format", "dailyEpisodeFormat", {}),
         ("anime_episode_format", "animeEpisodeFormat", {}),
         ("series_folder_format", "seriesFolderFormat", {}),
         ("season_folder_format", "seasonFolderFormat", {}),
         ("specials_folder_format", "specialsFolderFormat", {}),
         ("multiepisode_style", "multiEpisodeStyle", {}),
     ]
-    _mediamanagement_remote_map: List[RemoteMapEntry] = [
+    _mediamanagement_remote_map: ClassVar[List[RemoteMapEntry]] = [
         # Folders
         ("create_empty_series_folders", "createEmptySeriesFolders", {}),
         ("delete_empty_folders", "deleteEmptyFolders", {}),
         # Importing
         ("episode_title_required", "episodeTitleRequired", {}),
         ("skip_free_space_check", "skipFreeSpaceCheckWhenImporting", {}),
         ("minimum_free_space", "minimumFreeSpaceWhenImporting", {}),
@@ -614,15 +613,15 @@
             else:
                 logger.info("%s[%i]: %s -> (created)", tree, i, repr(str(root_folder)))
                 api_post(secrets, "/api/v3/rootfolder", {"path": str(root_folder)})
                 changed = True
         return changed
 
     def delete_remote(self, tree: str, secrets: SonarrSecrets, remote: Self) -> bool:
-        return self._update_remote_rootfolder(
+        return self._delete_remote_rootfolder(
             tree=f"{tree}.root_folders",
             secrets=secrets,
             remote=remote,
         )
 
     def _delete_remote_rootfolder(self, tree: str, secrets: SonarrSecrets, remote: Self) -> bool:
         changed = False
```

### Comparing `buildarr_sonarr-0.6.4/buildarr_sonarr/config/metadata.py` & `buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,18 +12,17 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Sonarr plugin metadata settings configuration.
 """
 
-
 from __future__ import annotations
 
-from typing import Any, Dict, List, Mapping, Optional, Tuple, Type
+from typing import Any, ClassVar, Dict, List, Mapping, Optional, Tuple, Type
 
 from buildarr.config import RemoteMapEntry
 from typing_extensions import Self
 
 from ..api import api_get, api_put
 from ..secrets import SonarrSecrets
 from .types import SonarrConfigBase
@@ -35,50 +34,54 @@
     """
 
     enable: bool = False
     """
     When set to `True`, enables creating metadata files in the given format.
     """
 
-    _implementation_name: str
-    _implementation: str
-    _config_contract: str
-    _base_remote_map: List[RemoteMapEntry] = [("enable", "enable", {})]
-    _remote_map: List[RemoteMapEntry]
+    _implementation: ClassVar[str]
+    _base_remote_map: ClassVar[List[RemoteMapEntry]] = [("enable", "enable", {})]
+    _remote_map: ClassVar[List[RemoteMapEntry]]
 
     @classmethod
     def _from_remote(cls, metadata: Dict[str, Any]) -> Self:
         return cls(**cls.get_local_attrs(cls._base_remote_map + cls._remote_map, metadata))
 
     def _update_remote(
         self,
         tree: str,
         secrets: SonarrSecrets,
         remote: Self,
-        metadata: Mapping[str, Any],
+        api_metadata: Mapping[str, Any],
         check_unmanaged: bool = False,
     ) -> bool:
         updated, remote_attrs = self.get_update_remote_attrs(
             tree,
             remote,
             self._base_remote_map + self._remote_map,
             check_unmanaged=check_unmanaged,
             set_unchanged=True,
         )
         if updated:
+            updated_fields = {f["name"]: f["value"] for f in remote_attrs.pop("fields")}
+            fields = [
+                (
+                    {**field, "value": updated_fields[field["name"]]}
+                    if field["name"] in updated_fields
+                    else field
+                )
+                for field in api_metadata["fields"]
+            ]
             api_put(
                 secrets,
-                f"/api/v3/metadata/{metadata['id']}",
+                f"/api/v3/metadata/{api_metadata['id']}",
                 {
-                    "id": metadata["id"],
-                    "name": self._implementation_name,
-                    "implementationName": self._implementation_name,
-                    "implementation": self._implementation,
-                    "configContract": self._config_contract,
+                    **api_metadata,
                     **remote_attrs,
+                    "fields": fields,
                 },
             )
             return True
         return False
 
 
 class KodiEmbyMetadata(Metadata):
@@ -127,18 +130,16 @@
     """
 
     episode_images: bool = False
     """
     Save episode images to `<filename>-thumb.jpg`.
     """
 
-    _implementation_name: str = "Kodi (XBMC) / Emby"
-    _implementation: str = "XbmcMetadata"
-    _config_contract: str = "XbmcMetadataSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation: ClassVar[str] = "XbmcMetadata"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("series_metadata", "seriesMetadata", {"is_field": True}),
         ("series_metadata_url", "seriesMetadataUrl", {"is_field": True}),
         ("episode_metadata", "episodeMetadata", {"is_field": True}),
         ("series_images", "seriesImages", {"is_field": True}),
         ("season_images", "seasonImages", {"is_field": True}),
         ("episode_images", "episodeImages", {"is_field": True}),
     ]
@@ -177,18 +178,16 @@
     """
 
     episode_images: bool = False
     """
     Save episode images to `Season##/<filename>.jpg`.
     """
 
-    _implementation_name: str = "Roksbox"
-    _implementation: str = "RoksboxMetadata"
-    _config_contract: str = "RoksboxMetadataSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation: ClassVar[str] = "RoksboxMetadata"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("episode_metadata", "episodeMetadata", {"is_field": True}),
         ("series_images", "seriesImages", {"is_field": True}),
         ("season_images", "seasonImages", {"is_field": True}),
         ("episode_images", "episodeImages", {"is_field": True}),
     ]
 
 
@@ -226,18 +225,16 @@
     """
 
     episode_images: bool = False
     """
     Save episode images to `<filename>-thumb.jpg`.
     """
 
-    _implementation_name: str = "WDTV"
-    _implementation: str = "WdtvMetadata"
-    _config_contract: str = "WdtvMetadataSettings"
-    _remote_map: List[RemoteMapEntry] = [
+    _implementation: ClassVar[str] = "WdtvMetadata"
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("episode_metadata", "episodeMetadata", {"is_field": True}),
         ("series_images", "seriesImages", {"is_field": True}),
         ("season_images", "seasonImages", {"is_field": True}),
         ("episode_images", "episodeImages", {"is_field": True}),
     ]
 
 
@@ -249,17 +246,17 @@
 
 class SonarrMetadataSettingsConfig(SonarrConfigBase):
     """
     Sonarr metadata settings.
     Implementation wise each metadata is a unique object, updated using separate requests.
     """
 
-    kodi_emby = KodiEmbyMetadata()
-    roksbox = RoksboxMetadata()
-    wdtv = WdtvMetadata()
+    kodi_emby: KodiEmbyMetadata = KodiEmbyMetadata()
+    roksbox: RoksboxMetadata = RoksboxMetadata()
+    wdtv: WdtvMetadata = WdtvMetadata()
 
     @classmethod
     def from_remote(cls, secrets: SonarrSecrets) -> Self:
         kodi_emby_metadata: Optional[Dict[str, Any]] = None
         roksbox_metadata: Optional[Dict[str, Any]] = None
         wdtv_metadata: Optional[Dict[str, Any]] = None
         for metadata in api_get(secrets, "/api/v3/metadata"):
@@ -318,26 +315,26 @@
             )
         return any(
             [
                 self.kodi_emby._update_remote(
                     tree=f"{tree}.kodi_emby",
                     secrets=secrets,
                     remote=remote.kodi_emby,
-                    metadata=kodi_emby_metadata,
+                    api_metadata=kodi_emby_metadata,
                     check_unmanaged=check_unmanaged,
                 ),
                 self.roksbox._update_remote(
                     tree=f"{tree}.roksbox",
                     secrets=secrets,
                     remote=remote.roksbox,
-                    metadata=roksbox_metadata,
+                    api_metadata=roksbox_metadata,
                     check_unmanaged=check_unmanaged,
                 ),
                 self.wdtv._update_remote(
                     tree=f"{tree}.wdtv",
                     secrets=secrets,
                     remote=remote.wdtv,
-                    metadata=wdtv_metadata,
+                    api_metadata=wdtv_metadata,
                     check_unmanaged=check_unmanaged,
                 ),
             ],
         )
```

### Comparing `buildarr_sonarr-0.6.4/buildarr_sonarr/config/profiles/__init__.py` & `buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_sonarr-0.6.4/buildarr_sonarr/config/profiles/delay.py` & `buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/profiles/delay.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,23 +12,22 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Sonarr plugin delay profile configuration.
 """
 
-
 from __future__ import annotations
 
 from logging import getLogger
 from typing import Any, Dict, List, Mapping, Set
 
 from buildarr.config import RemoteMapEntry
 from buildarr.types import BaseEnum, NonEmptyStr
-from pydantic import Field
+from pydantic import NonNegativeInt
 from typing_extensions import Self
 
 from ...api import api_delete, api_get, api_post, api_put
 from ...secrets import SonarrSecrets
 from ..types import SonarrConfigBase
 
 logger = getLogger(__name__)
@@ -126,20 +125,20 @@
 
     * `usenet-prefer` (Prefer Usenet)
     * `torrent-prefer` (Prefer Torrent)
     * `usenet-only` (Only Usenet)
     * `torrent-only` (Only Torrent)
     """
 
-    usenet_delay: int = Field(0, ge=0)  # minutes
+    usenet_delay: NonNegativeInt = 0  # minutes
     """
     Delay (in minutes) to wait before grabbing a release from Usenet.
     """
 
-    torrent_delay: int = Field(0, ge=0)  # minutes
+    torrent_delay: NonNegativeInt = 0  # minutes
     """
     Delay (in minutes) to wait before grabbing a torrent.
     """
 
     bypass_if_highest_quality: bool = False
     """
     Bypass the delay if a found release is the highest quality allowed
@@ -269,15 +268,15 @@
 
 
 class SonarrDelayProfilesSettingsConfig(SonarrConfigBase):
     """
     Configuration parameters for controlling how Buildarr handles delay profiles.
     """
 
-    delete_unmanaged = False
+    delete_unmanaged: bool = False
     """
     Controls how Buildarr manages existing delay profiles in Sonarr when no delay profiles
     are defined in Buildarr.
 
     When set to `True` and there are no delay profiles defined in Buildarr,
     delete all delay profiles except the default delay profile (which can't be deleted).
 
@@ -320,15 +319,15 @@
     def update_remote(
         self,
         tree: str,
         secrets: SonarrSecrets,
         remote: Self,
         check_unmanaged: bool = False,
     ) -> bool:
-        if not self.delete_unmanaged and "definitions" not in self.__fields_set__:
+        if not self.delete_unmanaged and "definitions" not in self.model_fields_set:
             # TODO: Print current delay profile structure.
             if remote.definitions:
                 logger.debug("%s.definitions: [...] (unmanaged)", tree)
             else:
                 logger.debug("%s.definitions: [] (unmanaged)", tree)
             return False
         #
```

### Comparing `buildarr_sonarr-0.6.4/buildarr_sonarr/config/profiles/language.py` & `buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/profiles/language.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,22 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Sonarr plugin language profile configuration.
 """
 
-
 from __future__ import annotations
 
 from logging import getLogger
 from typing import Any, Dict, List, Mapping, Optional, Sequence, Set
 
 from buildarr.config import RemoteMapEntry
 from buildarr.types import BaseEnum
-from pydantic import Field, validator
+from pydantic import Field, ValidationInfo, field_validator
 from typing_extensions import Annotated, Self
 
 from ...api import api_delete, api_get, api_post, api_put
 from ...secrets import SonarrSecrets
 from ..types import SonarrConfigBase
 
 logger = getLogger(__name__)
@@ -124,15 +123,15 @@
     """
     Enable automatic upgrading if a version of a media file
     in a more preferred language becomes available.
 
     If disabled, languages will not be upgraded.
     """
 
-    languages: Annotated[List[Language], Field(min_items=1)]
+    languages: Annotated[List[Language], Field(min_length=1)]
     """
     The languages episodes are allowed to be in.
     The order of the list determines priority (highest priority first, lowest priority last).
 
     Use the name of the language in English (e.g. `Japanese`, not `Nihongo` or `日本語`).
 
     ```yaml
@@ -149,33 +148,35 @@
     """
     The highest priority language to upgrade an episode to.
     Usually this would be set to the highest priority language in the profile.
 
     This attribute is required if `upgrades_allowed` is set to `True`.
     """
 
-    @validator("languages")
+    @field_validator("languages")
+    @classmethod
     def validate_languages(cls, value: List[Language]) -> List[Language]:
         language_set: Set[Language] = set()
         for language in value:
             if language in language_set:
                 raise ValueError(f"duplicate entries of language '{language.value}' exist")
             else:
                 language_set.add(language)
         return value
 
-    @validator("upgrade_until")
+    @field_validator("upgrade_until")
+    @classmethod
     def validate_upgrade_until(
         cls,
         value: Optional[Language],
-        values: Dict[str, Any],
+        info: ValidationInfo,
     ) -> Optional[Language]:
         try:
-            upgrades_allowed: bool = values["upgrades_allowed"]
-            languages: Sequence[Language] = values["languages"]
+            upgrades_allowed: bool = info.data["upgrades_allowed"]
+            languages: Sequence[Language] = info.data["languages"]
         except KeyError:
             return value
         # If `upgrades_allowed` is `False`, set `upgrade_until` to `None`
         # to make sure Buildarr ignores whatever it is currently set to
         # on the remote instance.
         if not upgrades_allowed:
             return None
@@ -309,15 +310,15 @@
 
 
 class SonarrLanguageProfilesSettingsConfig(SonarrConfigBase):
     """
     Configuration parameters for controlling how Buildarr handles language profiles.
     """
 
-    delete_unmanaged = False
+    delete_unmanaged: bool = False
     """
     Automatically delete language profiles not defined in Buildarr.
     """
 
     definitions: Dict[str, LanguageProfile] = {}
     """
     Define language profiles to configure on Sonarr here.
```

### Comparing `buildarr_sonarr-0.6.4/buildarr_sonarr/config/profiles/quality.py` & `buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/profiles/quality.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,22 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Sonarr plugin quality profile configuration.
 """
 
-
 from __future__ import annotations
 
 from logging import getLogger
 from typing import Any, Dict, List, Mapping, Optional, Sequence, Set, Union, cast
 
 from buildarr.config import RemoteMapEntry
 from buildarr.types import NonEmptyStr
-from pydantic import Field, validator
+from pydantic import Field, ValidationInfo, field_validator
 from typing_extensions import Annotated, Self
 
 from ...api import api_delete, api_get, api_post, api_put
 from ...secrets import SonarrSecrets
 from ..types import SonarrConfigBase
 
 logger = getLogger(__name__)
@@ -38,15 +37,15 @@
     """
     Quality group.
 
     Allows groups of quality definitions to be given the same prorioty in qualtity profiles.
     """
 
     name: NonEmptyStr
-    members: Set[NonEmptyStr] = Field(..., min_items=1)
+    members: Annotated[Set[NonEmptyStr], Field(min_length=1)]
 
     def encode(self, group_id: int, quality_definitions: Mapping[str, Any]) -> Dict[str, Any]:
         return {
             "id": group_id,
             "name": self.name,
             "allowed": True,
             "items": [
@@ -93,15 +92,15 @@
     upgrades_allowed: bool = False
     """
     Enable automatic upgrading if a higher quality version of the media file becomes available.
 
     If disabled, media files will not be upgraded after they have been downloaded.
     """
 
-    qualities: Annotated[List[Union[NonEmptyStr, QualityGroup]], Field(min_items=1)]
+    qualities: Annotated[List[Union[NonEmptyStr, QualityGroup]], Field(min_length=1)]
     """
     The qualities to enable downloading episodes for. The order determines the priority
     (highest priority first, lowest priority last).
 
     Individual qualities can be specified using the name (e.g. `Bluray-480p`).
 
     Qualities can also be grouped together in a structure to give them the same
@@ -127,15 +126,16 @@
     For a quality group, specify the group name.
 
     Once this quality is reached Sonarr will no longer download episodes.
 
     This attribute is required if `upgrades_allowed` is set to `True`.
     """
 
-    @validator("qualities")
+    @field_validator("qualities")
+    @classmethod
     def validate_qualities(
         cls,
         value: List[Union[str, QualityGroup]],
     ) -> List[Union[str, QualityGroup]]:
         quality_name_map: Dict[str, Union[str, QualityGroup]] = {}
         for quality in value:
             for name in quality.members if isinstance(quality, QualityGroup) else [quality]:
@@ -156,23 +156,24 @@
                             else "another as a non-grouped quality value"
                         )
                     error_message += ")"
                     raise ValueError(error_message)
                 quality_name_map[name] = quality
         return value
 
-    @validator("upgrade_until")
+    @field_validator("upgrade_until")
+    @classmethod
     def validate_upgrade_until(
         cls,
         value: Optional[str],
-        values: Dict[str, Any],
+        info: ValidationInfo,
     ) -> Optional[str]:
         try:
-            upgrades_allowed: bool = values["upgrades_allowed"]
-            qualities: Sequence[Union[str, QualityGroup]] = values["qualities"]
+            upgrades_allowed: bool = info.data["upgrades_allowed"]
+            qualities: Sequence[Union[str, QualityGroup]] = info.data["qualities"]
         except KeyError:
             return value
         # If `upgrades_allowed` is `False`, set `upgrade_until` to `None`
         # to make sure Buildarr ignores whatever it is currently set to
         # on the remote instance.
         if not upgrades_allowed:
             return None
```

### Comparing `buildarr_sonarr-0.6.4/buildarr_sonarr/config/profiles/release.py` & `buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/profiles/release.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,25 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Sonarr plugin release profile configuration.
 """
 
-
 from __future__ import annotations
 
 import json
 
 from logging import getLogger
 from typing import Any, Dict, Iterable, List, Mapping, Optional, Set, cast
 
 from buildarr.config import ConfigTrashIDNotFoundError, RemoteMapEntry
 from buildarr.state import state
 from buildarr.types import NonEmptyStr, TrashID
-from pydantic import validator
+from pydantic import field_validator
 from typing_extensions import Self
 
 from ...api import api_delete, api_get, api_post, api_put
 from ...secrets import SonarrSecrets
 from ..types import SonarrConfigBase
 
 logger = getLogger(__name__)
@@ -191,17 +190,18 @@
     All tags on an existing release profile (if present) are removed
     and replaced with only the tags in this list.
 
     If an empty list is explicitly defined, no tags will be set on the release profile,
     and any existing tags (if present) are removed.
     """
 
-    @validator("preferred")
-    def sort_preferred(cls, preferred: Iterable[PreferredWord]) -> List[PreferredWord]:
-        return sorted(preferred, key=lambda p: (-p.score, p.term))
+    @field_validator("preferred")
+    @classmethod
+    def sort_preferred(cls, value: Iterable[PreferredWord]) -> List[PreferredWord]:
+        return sorted(value, key=lambda p: (-p.score, p.term))
 
     @classmethod
     def _get_remote_map(
         cls,
         indexer_ids: Mapping[str, int],
         tag_ids: Mapping[str, int],
     ) -> List[RemoteMapEntry]:
@@ -310,16 +310,16 @@
                             ):
                                 must_not_contain.add(term)
                             else:
                                 preferred.append(
                                     PreferredWord(term=cast(NonEmptyStr, term), score=score),
                                 )
                     #
-                    self.must_contain = must_contain  # type: ignore[assignment]
-                    self.must_not_contain = must_not_contain  # type: ignore[assignment]
+                    self.must_contain = must_contain
+                    self.must_not_contain = must_not_contain
                     self.preferred = preferred
                     return
         raise ConfigTrashIDNotFoundError(
             f"Unable to find Sonarr release profile file with trash ID '{self.trash_id}'",
         )
 
     def _create_remote(
```

### Comparing `buildarr_sonarr-0.6.4/buildarr_sonarr/config/quality.py` & `buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/quality.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,26 +12,25 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Sonarr plugin quality settings configuration object.
 """
 
-
 from __future__ import annotations
 
 import json
 
-from typing import Any, Dict, Mapping, Optional, cast
+from typing import Dict, Optional, cast
 
 from buildarr.config import ConfigTrashIDNotFoundError
 from buildarr.state import state
 from buildarr.types import TrashID
-from pydantic import Field, validator
-from typing_extensions import Self
+from pydantic import Field, ValidationInfo, field_validator
+from typing_extensions import Annotated, Self
 
 from ..api import api_get, api_put
 from ..secrets import SonarrSecrets
 from .types import SonarrConfigBase
 
 QUALITYDEFINITION_MAX = 400
 """
@@ -49,60 +48,49 @@
     The name of the quality in the GUI.
 
     If unset, set to an empty string or `None`, it will always be set to the
     name of the quality itself. (e.g. For the `Bluray-480p` quality, the GUI title
     will also be `Bluray-480p`)
     """
 
-    min: float = Field(..., ge=0, le=QUALITYDEFINITION_MAX - 1)
+    min: Annotated[float, Field(ge=0, le=QUALITYDEFINITION_MAX - 1)]
     """
     The minimum Megabytes per Minute (MB/min) a quality can have.
     Must be set at least 1MB/min lower than `max`.
 
     The minimum value is `0`, and the maximum value is `399`.
     """
 
     # Note: No 'pref' field like in Radarr until V4
 
-    max: Optional[float] = Field(..., ge=1, le=QUALITYDEFINITION_MAX)
+    max: Optional[Annotated[float, Field(ge=1, le=QUALITYDEFINITION_MAX)]]
     """
     The maximum Megabytes per Minute (MB/min) a quality can have.
     Must be set at least 1MB/min higher than `min`.
 
     If set to `None` or `400`, the maximum bit rate will be unlimited.
 
     If not set to `None`, the minimum value is `1`, and the maximum value is `400`.
     """
 
-    @validator("max")
-    def validate_min_max(
-        cls,
-        value: Optional[float],
-        values: Mapping[str, Any],
-    ) -> Optional[float]:
-        quality_max = value
-        quality_max_val = (
-            min(quality_max, QUALITYDEFINITION_MAX)
-            if quality_max is not None
-            else QUALITYDEFINITION_MAX
-        )
-        try:
-            quality_min: float = values["min"]
-            if quality_max_val - quality_min < 1:
-                raise ValueError(
-                    f"'max' ({quality_max_val}) is not "
-                    f"at least 1 greater than 'min' ({quality_min})",
-                )
-        except KeyError:
-            # `min` only doesn't exist when it failed type validation.
-            # If it doesn't exist, skip validation that uses it.
-            pass
-        if quality_max_val >= QUALITYDEFINITION_MAX:
-            return None
-        return quality_max
+    @field_validator("max")
+    @classmethod
+    def validate_max(cls, value: Optional[float], info: ValidationInfo) -> Optional[float]:
+        quality_min: float = info.data["min"]
+        if value is not None:
+            quality_max = min(value, QUALITYDEFINITION_MAX)
+            if quality_max >= QUALITYDEFINITION_MAX:
+                value = None
+        else:
+            quality_max = QUALITYDEFINITION_MAX
+        if (quality_max - quality_min) < 1:
+            raise ValueError(
+                f"'max' ({quality_max}) not greater than 'min' ({quality_min}) by at least 1",
+            )
+        return value
 
 
 class SonarrQualitySettingsConfig(SonarrConfigBase):
     """
     Quality definitions are used to set the permitted bit rates for each quality level.
 
     These can either be set manually within Buildarr, or pre-made profiles can be
```

### Comparing `buildarr_sonarr-0.6.4/buildarr_sonarr/config/tags.py` & `buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/tags.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,19 +12,18 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Sonarr plugin tags settings configuration.
 """
 
-
 from __future__ import annotations
 
 from logging import getLogger
-from typing import Dict, List
+from typing import Dict, Set
 
 from buildarr.types import NonEmptyStr
 from typing_extensions import Self
 
 from ..api import api_get, api_post
 from ..secrets import SonarrSecrets
 from .types import SonarrConfigBase
@@ -45,26 +44,26 @@
             - "example2"
     ```
 
     To be able to use those tags in Buildarr, they need to be defined
     in this configuration section.
     """
 
-    definitions: List[NonEmptyStr] = []
+    definitions: Set[NonEmptyStr] = set()
     """
     Define tags that are used within Buildarr here.
 
     If they are not defined here, you may get errors resulting from non-existent
     tags from either Buildarr or Sonarr.
     """
 
     @classmethod
     def from_remote(cls, secrets: SonarrSecrets) -> Self:
         return cls(
-            definitions=[tag["label"] for tag in api_get(secrets, "/api/v3/tag")],
+            definitions=set(tag["label"] for tag in api_get(secrets, "/api/v3/tag")),
         )
 
     def update_remote(
         self,
         tree: str,
         secrets: SonarrSecrets,
         remote: Self,
@@ -72,15 +71,15 @@
     ) -> bool:
         # This only does creations and updates, as Sonarr automatically cleans up unused tags.
         changed = False
         current_tags: Dict[str, int] = {
             tag["label"]: tag["id"] for tag in api_get(secrets, "/api/v3/tag")
         }
         if self.definitions:
-            for i, tag in enumerate(self.definitions):
+            for i, tag in enumerate(sorted(self.definitions)):
                 if tag in current_tags:
                     logger.debug("%s.definitions[%i]: %s (exists)", tree, i, repr(tag))
                 else:
                     logger.info("%s.definitions[%i]: %s -> (created)", tree, i, repr(tag))
                     api_post(secrets, "/api/v3/tag", {"label": tag})
                     changed = True
         return changed
```

### Comparing `buildarr_sonarr-0.6.4/buildarr_sonarr/config/types.py` & `buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,34 +12,19 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Sonarr plugin configuration utility classes and functions.
 """
 
-
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from buildarr.config import ConfigBase
-from pydantic import ConstrainedStr
 
 if TYPE_CHECKING:
-    from ..secrets import SonarrSecrets
-
-    class SonarrConfigBase(ConfigBase[SonarrSecrets]):
-        ...
-
-else:
-
-    class SonarrConfigBase(ConfigBase):
-        ...
-
+    from ..secrets import SonarrSecrets  # noqa: F401
 
-class TraktAuthUser(ConstrainedStr):
-    """
-    Constrained string type to make the Trakt auth user case-insensitive.
-    """
 
-    min_length = 1
-    to_lower = True
+class SonarrConfigBase(ConfigBase["SonarrSecrets"]):
+    pass
```

### Comparing `buildarr_sonarr-0.6.4/buildarr_sonarr/config/ui.py` & `buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,18 +12,17 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Sonarr plugin UI settings configuration object.
 """
 
-
 from __future__ import annotations
 
-from typing import List
+from typing import ClassVar, List
 
 from buildarr.config import RemoteMapEntry
 from buildarr.types import BaseEnum
 from typing_extensions import Self
 
 from ..api import api_get, api_put
 from ..secrets import SonarrSecrets
@@ -166,15 +165,15 @@
     # Style
     enable_color_impaired_mode: bool = False
     """
     Enable an altered view style to allow colour-impaired users to better distinguish
     colour-coded information.
     """
 
-    _remote_map: List[RemoteMapEntry] = [
+    _remote_map: ClassVar[List[RemoteMapEntry]] = [
         ("first_day_of_week", "firstDayOfWeek", {}),
         ("week_column_header", "calendarWeekColumnHeader", {}),
         ("short_date_format", "shortDateFormat", {}),
         ("long_date_format", "longDateFormat", {}),
         ("time_format", "timeFormat", {}),
         ("show_relative_dates", "showRelativeDates", {}),
         ("enable_color_impaired_mode", "enableColorImpairedMode", {}),
```

### Comparing `buildarr_sonarr-0.6.4/buildarr_sonarr/config/util.py` & `buildarr_sonarr-0.7.0b0/buildarr_sonarr/config/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Sonarr plugin configuration utility classes and functions.
 """
 
-
 from __future__ import annotations
 
 from datetime import datetime, timezone
 
 
 def trakt_expires_encoder(dt: datetime) -> str:
     """
```

### Comparing `buildarr_sonarr-0.6.4/buildarr_sonarr/exceptions.py` & `buildarr_sonarr-0.7.0b0/buildarr_sonarr/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Sonarr plugin exception classes.
 """
 
-
 from __future__ import annotations
 
 from buildarr.exceptions import BuildarrError
 
 
 class SonarrError(BuildarrError):
     """
```

### Comparing `buildarr_sonarr-0.6.4/buildarr_sonarr/manager.py` & `buildarr_sonarr-0.7.0b0/buildarr_sonarr/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Sonarr plugin manager class.
 """
 
-
 from __future__ import annotations
 
 from buildarr.manager import ManagerPlugin
 
 from .config import SonarrInstanceConfig
 from .secrets import SonarrSecrets
```

### Comparing `buildarr_sonarr-0.6.4/buildarr_sonarr/plugin.py` & `buildarr_sonarr-0.7.0b0/buildarr_sonarr/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Sonarr plugin interface.
 """
 
-
 from __future__ import annotations
 
 from buildarr.plugins import Plugin
 
 from . import __version__
 from .cli import sonarr
 from .config import SonarrConfig
```

### Comparing `buildarr_sonarr-0.6.4/buildarr_sonarr/secrets.py` & `buildarr_sonarr-0.7.0b0/buildarr_sonarr/secrets.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,43 +12,34 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Sonarr plugin secrets file model.
 """
 
-
 from __future__ import annotations
 
 from http import HTTPStatus
 from typing import TYPE_CHECKING, Any, Dict, Optional, cast
 
 from buildarr.secrets import SecretsPlugin
 from buildarr.types import NonEmptyStr, Port
-from pydantic import validator
+from pydantic import field_validator
 
 from .api import api_get, get_initialize_js
 from .exceptions import SonarrAPIError, SonarrSecretsUnauthorizedError
 from .types import SonarrApiKey, SonarrProtocol
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
     from .config import SonarrConfig
 
-    class _SonarrSecrets(SecretsPlugin[SonarrConfig]):
-        ...
-
-else:
-
-    class _SonarrSecrets(SecretsPlugin):
-        ...
 
-
-class SonarrSecrets(_SonarrSecrets):
+class SonarrSecrets(SecretsPlugin["SonarrConfig"]):
     """
     Sonarr API secrets.
     """
 
     hostname: NonEmptyStr
     port: Port
     protocol: SonarrProtocol
@@ -61,16 +52,21 @@
         return self._get_host_url(
             protocol=self.protocol,
             hostname=self.hostname,
             port=self.port,
             url_base=self.url_base,
         )
 
-    @validator("url_base")
+    @field_validator("url_base")
+    @classmethod
     def validate_url_base(cls, value: Optional[str]) -> Optional[str]:
+        return cls._validate_url_base(value)
+
+    @classmethod
+    def _validate_url_base(cls, value: Optional[str]) -> Optional[str]:
         return f"/{value.strip('/')}" if value and value.strip("/") else None
 
     @classmethod
     def _get_host_url(
         cls,
         protocol: str,
         hostname: str,
@@ -94,15 +90,15 @@
         cls,
         hostname: str,
         port: int,
         protocol: str,
         url_base: Optional[str] = None,
         api_key: Optional[str] = None,
     ) -> Self:
-        url_base = cls.validate_url_base(url_base)
+        url_base = cls._validate_url_base(url_base)
         host_url = cls._get_host_url(
             protocol=protocol,
             hostname=hostname,
             port=port,
             url_base=url_base,
         )
         if not api_key:
@@ -137,32 +133,32 @@
                         "configuration, and that it is set to the value as shown in "
                         "'Settings -> General -> API Key' on the Radarr instance."
                     ),
                 ) from None
             else:
                 raise
         try:
-            version = cast(NonEmptyStr, system_status["version"])
+            version = cast(str, system_status["version"])
         except KeyError:
             raise SonarrSecretsUnauthorizedError(
                 f"Unable to find Sonarr version in system status metadata: {system_status}",
             ) from None
         except TypeError as err:
             raise SonarrSecretsUnauthorizedError(
                 (
                     f"Unable to parse Sonarr system status metadata: {err} "
                     f"(metadata object: {system_status})"
                 ),
             ) from None
         return cls(
-            hostname=cast(NonEmptyStr, hostname),
-            port=cast(Port, port),
-            protocol=cast(SonarrProtocol, protocol),
+            hostname=hostname,
+            port=port,
+            protocol=protocol,  # type: ignore[arg-type]
             url_base=url_base,
-            api_key=cast(SonarrApiKey, api_key),
+            api_key=api_key,  # type: ignore[arg-type]
             version=version,
         )
 
     def test(self) -> bool:
         # We already perform API requests as part of instantiating the secrets object.
         # If the object exists, then the connection test is already successful.
         return True
```

### Comparing `buildarr_sonarr-0.6.4/buildarr_sonarr/types.py` & `buildarr_sonarr-0.7.0b0/buildarr_sonarr/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,26 +12,28 @@
 # If not, see <https://www.gnu.org/licenses/>.
 
 
 """
 Sonarr plugin type hints.
 """
 
-
 from __future__ import annotations
 
 import re
 
 from pathlib import PurePosixPath, PureWindowsPath
-from typing import Any, Callable, Generator, Literal
+from typing import Any, Literal, Type
 
-from pydantic import SecretStr
-from typing_extensions import Self
+from buildarr.types import SecretStr
+from pydantic import GetCoreSchemaHandler, StringConstraints
+from pydantic_core import core_schema
+from typing_extensions import Annotated, Self
 
 SonarrProtocol = Literal["http", "https"]
+SonarrApiKey = Annotated[SecretStr, StringConstraints(min_length=32, max_length=32)]
 
 
 class OSAgnosticPath(str):
     def is_windows(self) -> bool:
         return bool(re.match(r"^[A-Za-z]:", self) or self.startswith("\\\\"))
 
     def is_posix(self) -> bool:
@@ -52,22 +54,17 @@
     def __hash__(self) -> int:
         if self.is_windows():
             return hash(PureWindowsPath(self))
         else:
             return hash(PurePosixPath(self))
 
     @classmethod
-    def __get_validators__(cls) -> Generator[Callable[[Any], Self], None, None]:
-        yield cls.validate
+    def __get_pydantic_core_schema__(
+        cls,
+        source: Type[Any],
+        handler: GetCoreSchemaHandler,
+    ) -> core_schema.CoreSchema:
+        return core_schema.no_info_plain_validator_function(cls.validate)
 
     @classmethod
     def validate(cls, value: Any) -> Self:
         return cls(value)
-
-
-class SonarrApiKey(SecretStr):
-    """
-    Constrained secret string type for a Sonarr API key.
-    """
-
-    min_length = 32
-    max_length = 32
```

### Comparing `buildarr_sonarr-0.6.4/PKG-INFO` & `buildarr_sonarr-0.7.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: buildarr-sonarr
-Version: 0.6.4
+Version: 0.7.0b0
 Summary: Sonarr PVR plugin for Buildarr
-Home-page: https://buildarr.github.io
+Author-email: Callum Dickinson <callum.dickinson.nz@gmail.com>
 License: GPL-3.0-or-later
+Project-URL: Homepage, https://buildarr.github.io
+Project-URL: Documentation, https://buildarr.github.io/plugins/sonarr
+Project-URL: Repository, https://github.com/buildarr/buildarr-sonarr
+Project-URL: Issues, https://github.com/buildarr/buildarr-sonarr/issues
+Project-URL: Changelog, https://buildarr.github.io/plugins/sonarr/release-notes
 Keywords: buildarr,sonarr
-Author: Callum Dickinson
-Author-email: callum.dickinson.nz@gmail.com
-Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pydantic
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Systems Administration
 Classifier: Typing :: Typed
-Requires-Dist: buildarr (>=0.7.1,<0.8.0)
-Requires-Dist: json5 (>=0.9.7)
-Project-URL: Changes, https://buildarr.github.io/plugins/sonarr/release-notes
-Project-URL: Documentation, https://buildarr.github.io/plugins/sonarr
-Project-URL: Issue Tracker, https://github.com/buildarr/buildarr-sonarr/issues
-Project-URL: Repository, https://github.com/buildarr/buildarr-sonarr
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: buildarr<0.9.0,>=0.8.0b0
+Requires-Dist: json5>=0.9.7
 
 # Buildarr Sonarr Plugin
 
-[![PyPI](https://img.shields.io/pypi/v/buildarr-sonarr)](https://pypi.org/project/buildarr-sonarr) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/buildarr-sonarr)  [![GitHub](https://img.shields.io/github/license/buildarr/buildarr-sonarr)](https://github.com/buildarr/buildarr-sonarr/blob/main/LICENSE) ![Pre-commit hooks](https://github.com/buildarr/buildarr-sonarr/actions/workflows/pre-commit.yml/badge.svg) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![PyPI](https://img.shields.io/pypi/v/buildarr-sonarr)](https://pypi.org/project/buildarr-sonarr) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/buildarr-sonarr)  [![GitHub](https://img.shields.io/github/license/buildarr/buildarr-sonarr)](https://github.com/buildarr/buildarr-sonarr/blob/main/LICENSE) ![Test Status](https://img.shields.io/github/actions/workflow/status/buildarr/buildarr-sonarr/test.yml?label=tests)
 
 The Buildarr Sonarr plugin (`buildarr-sonarr`) is a plugin for Buildarr that adds the capability to configure and manage [Sonarr](http://sonarr.tv) instances.
 
 Sonarr is a PVR application which downloads, renames and manages the lifecycle of TV shows in your media library. It is capable of scanning for higher quality versions of your media and automatically upgrading them when a suitable version is available.
 
 Currently, Sonarr V3 is the only supported version. Sonarr V4 support is planned for the future.
 
@@ -527,8 +527,7 @@
     long_date_format: day-first
     short_date_format: word-month-second
     show_relative_dates: true
     time_format: twentyfour-hour
     week_column_header: day-first
 version: 3.0.9.1549
 ```
-
```

