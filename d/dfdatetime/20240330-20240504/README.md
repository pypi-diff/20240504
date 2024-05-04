# Comparing `tmp/dfdatetime-20240330.tar.gz` & `tmp/dfdatetime-20240504.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfdatetime-20240330.tar", last modified: Sat Mar 30 07:29:05 2024, max compression
+gzip compressed data, was "dfdatetime-20240504.tar", last modified: Sat May  4 05:16:55 2024, max compression
```

## Comparing `dfdatetime-20240330.tar` & `dfdatetime-20240504.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-30 07:29:05.572706 dfdatetime-20240330/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-30 07:29:05.554706 dfdatetime-20240330/.github/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-30 07:29:05.559707 dfdatetime-20240330/.github/workflows/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2607 2024-03-30 05:09:36.000000 dfdatetime-20240330/.github/workflows/test_docker.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1342 2024-03-29 13:32:32.000000 dfdatetime-20240330/.github/workflows/test_docs.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4024 2024-03-29 13:32:32.000000 dfdatetime-20240330/.github/workflows/test_tox.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23143 2024-03-29 13:32:18.000000 dfdatetime-20240330/.pylintrc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      322 2024-03-29 13:32:18.000000 dfdatetime-20240330/.readthedocs.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      661 2023-12-03 10:50:32.000000 dfdatetime-20240330/ACKNOWLEDGEMENTS
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      368 2023-12-03 10:50:32.000000 dfdatetime-20240330/AUTHORS
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11358 2023-12-03 10:50:32.000000 dfdatetime-20240330/LICENSE
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      497 2023-12-03 10:50:32.000000 dfdatetime-20240330/MANIFEST.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      659 2024-03-30 07:29:05.572706 dfdatetime-20240330/PKG-INFO
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      213 2023-12-03 10:50:32.000000 dfdatetime-20240330/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2321 2024-03-29 13:32:18.000000 dfdatetime-20240330/appveyor.yml
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-30 07:29:05.555707 dfdatetime-20240330/config/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-30 07:29:05.559707 dfdatetime-20240330/config/appveyor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      798 2024-03-29 13:32:18.000000 dfdatetime-20240330/config/appveyor/install.ps1
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2024-03-29 13:32:18.000000 dfdatetime-20240330/config/appveyor/install.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2024-03-29 13:32:18.000000 dfdatetime-20240330/config/appveyor/runtests.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-30 07:29:05.560706 dfdatetime-20240330/config/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      173 2024-03-30 05:09:36.000000 dfdatetime-20240330/config/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       23 2023-12-03 10:55:02.000000 dfdatetime-20240330/config/dpkg/clean
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        2 2024-03-29 13:32:18.000000 dfdatetime-20240330/config/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      554 2024-03-29 13:32:18.000000 dfdatetime-20240330/config/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      968 2023-12-03 10:55:02.000000 dfdatetime-20240330/config/dpkg/copyright
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2024-03-29 13:32:18.000000 dfdatetime-20240330/config/dpkg/rules
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-30 07:29:05.561706 dfdatetime-20240330/config/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2023-12-03 10:55:02.000000 dfdatetime-20240330/config/dpkg/source/format
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-30 07:29:05.561706 dfdatetime-20240330/config/pylint/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      229 2023-12-03 10:55:01.000000 dfdatetime-20240330/config/pylint/spelling-private-dict
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-12-03 10:50:32.000000 dfdatetime-20240330/dependencies.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-30 07:29:05.565706 dfdatetime-20240330/dfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      870 2024-03-30 05:09:36.000000 dfdatetime-20240330/dfdatetime/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2595 2024-02-20 18:00:00.000000 dfdatetime-20240330/dfdatetime/apfs_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4524 2024-02-23 17:55:36.000000 dfdatetime-20240330/dfdatetime/cocoa_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      710 2024-02-20 18:00:00.000000 dfdatetime-20240330/dfdatetime/decorators.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2438 2024-02-20 18:00:00.000000 dfdatetime-20240330/dfdatetime/definitions.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5313 2024-02-23 17:55:36.000000 dfdatetime-20240330/dfdatetime/delphi_date_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4812 2024-02-23 17:55:36.000000 dfdatetime-20240330/dfdatetime/dotnet_datetime.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1846 2024-02-20 18:00:00.000000 dfdatetime-20240330/dfdatetime/factory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4273 2024-02-23 17:55:36.000000 dfdatetime-20240330/dfdatetime/fake_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10557 2024-02-23 17:55:36.000000 dfdatetime-20240330/dfdatetime/fat_date_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4895 2024-02-23 17:55:36.000000 dfdatetime-20240330/dfdatetime/filetime.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7664 2024-02-23 17:55:36.000000 dfdatetime-20240330/dfdatetime/golang_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4379 2024-02-23 17:55:36.000000 dfdatetime-20240330/dfdatetime/hfs_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31580 2024-03-30 04:44:58.000000 dfdatetime-20240330/dfdatetime/interface.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1977 2024-02-20 18:00:00.000000 dfdatetime-20240330/dfdatetime/java_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5061 2024-02-23 17:55:36.000000 dfdatetime-20240330/dfdatetime/ole_automation_date.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16377 2024-02-23 17:55:36.000000 dfdatetime-20240330/dfdatetime/posix_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9864 2024-02-20 18:00:00.000000 dfdatetime-20240330/dfdatetime/precisions.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8173 2024-02-23 17:55:36.000000 dfdatetime-20240330/dfdatetime/rfc2579_date_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9079 2024-02-20 18:00:00.000000 dfdatetime-20240330/dfdatetime/semantic_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7583 2024-02-20 18:00:00.000000 dfdatetime-20240330/dfdatetime/serializer.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7313 2024-02-23 17:55:36.000000 dfdatetime-20240330/dfdatetime/systemtime.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    46561 2024-03-30 05:09:36.000000 dfdatetime-20240330/dfdatetime/time_elements.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5092 2024-02-23 17:55:36.000000 dfdatetime-20240330/dfdatetime/uuid_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4752 2024-02-23 17:55:36.000000 dfdatetime-20240330/dfdatetime/webkit_time.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-30 07:29:05.565706 dfdatetime-20240330/dfdatetime.egg-info/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      659 2024-03-30 07:29:05.000000 dfdatetime-20240330/dfdatetime.egg-info/PKG-INFO
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2186 2024-03-30 07:29:05.000000 dfdatetime-20240330/dfdatetime.egg-info/SOURCES.txt
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        1 2024-03-30 07:29:05.000000 dfdatetime-20240330/dfdatetime.egg-info/dependency_links.txt
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       11 2024-03-30 07:29:05.000000 dfdatetime-20240330/dfdatetime.egg-info/top_level.txt
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      760 2023-12-03 10:50:32.000000 dfdatetime-20240330/dfdatetime.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-30 07:29:05.566707 dfdatetime-20240330/docs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5115 2024-03-29 13:32:18.000000 dfdatetime-20240330/docs/conf.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      593 2023-12-03 10:55:02.000000 dfdatetime-20240330/docs/index.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      118 2024-03-29 13:32:18.000000 dfdatetime-20240330/docs/requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-30 07:29:05.566707 dfdatetime-20240330/docs/sources/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16776 2024-02-23 17:55:36.000000 dfdatetime-20240330/docs/sources/Date-and-time-values.md
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-30 07:29:05.566707 dfdatetime-20240330/docs/sources/api/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3945 2023-12-03 10:55:02.000000 dfdatetime-20240330/docs/sources/api/dfdatetime.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 10:55:02.000000 dfdatetime-20240330/docs/sources/api/modules.rst
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-30 07:29:05.566707 dfdatetime-20240330/docs/sources/user/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1662 2024-02-11 07:44:31.000000 dfdatetime-20240330/docs/sources/user/Installation-instructions.md
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      292 2023-12-03 10:55:02.000000 dfdatetime-20240330/docs/sources/user/index.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      296 2024-03-29 13:32:18.000000 dfdatetime-20240330/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-29 13:32:18.000000 dfdatetime-20240330/requirements.txt
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1018 2023-12-03 10:50:32.000000 dfdatetime-20240330/run_tests.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      888 2024-03-30 07:29:05.572706 dfdatetime-20240330/setup.cfg
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      128 2024-03-29 13:32:18.000000 dfdatetime-20240330/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-12-03 10:50:32.000000 dfdatetime-20240330/test_dependencies.ini
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-29 13:32:18.000000 dfdatetime-20240330/test_requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-30 07:29:05.571706 dfdatetime-20240330/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2024-02-20 18:03:28.000000 dfdatetime-20240330/tests/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2219 2024-02-20 18:03:28.000000 dfdatetime-20240330/tests/apfs_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6053 2024-02-23 17:55:36.000000 dfdatetime-20240330/tests/cocoa_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8316 2024-02-23 17:55:36.000000 dfdatetime-20240330/tests/delphi_date_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3591 2024-02-23 17:55:36.000000 dfdatetime-20240330/tests/dotnet_datetime.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2646 2024-02-20 18:03:28.000000 dfdatetime-20240330/tests/factory.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6031 2024-02-23 17:55:36.000000 dfdatetime-20240330/tests/fake_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12242 2024-02-23 17:55:36.000000 dfdatetime-20240330/tests/fat_date_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5550 2024-02-23 17:55:36.000000 dfdatetime-20240330/tests/filetime.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8431 2024-02-23 17:55:36.000000 dfdatetime-20240330/tests/golang_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5525 2024-02-23 17:55:36.000000 dfdatetime-20240330/tests/hfs_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22873 2024-03-30 05:09:36.000000 dfdatetime-20240330/tests/interface.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5014 2024-02-23 17:55:36.000000 dfdatetime-20240330/tests/java_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6506 2024-02-23 17:55:36.000000 dfdatetime-20240330/tests/ole_automation_date.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24682 2024-02-23 17:55:36.000000 dfdatetime-20240330/tests/posix_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5838 2024-02-20 18:03:28.000000 dfdatetime-20240330/tests/precisions.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12039 2024-02-23 17:55:36.000000 dfdatetime-20240330/tests/rfc2579_date_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7979 2024-02-20 18:03:28.000000 dfdatetime-20240330/tests/semantic_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11261 2024-02-20 18:03:28.000000 dfdatetime-20240330/tests/serializer.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9420 2024-02-23 17:55:36.000000 dfdatetime-20240330/tests/systemtime.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69348 2024-03-30 05:09:36.000000 dfdatetime-20240330/tests/time_elements.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7131 2024-02-23 17:55:36.000000 dfdatetime-20240330/tests/uuid_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5686 2024-02-23 17:55:36.000000 dfdatetime-20240330/tests/webkit_time.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1297 2024-03-29 13:32:18.000000 dfdatetime-20240330/tox.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-30 07:29:05.571706 dfdatetime-20240330/utils/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:55:04.000000 dfdatetime-20240330/utils/__init__.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2024-03-29 13:32:18.000000 dfdatetime-20240330/utils/check_dependencies.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2024-03-29 13:32:18.000000 dfdatetime-20240330/utils/dependencies.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      779 2024-01-28 09:26:26.000000 dfdatetime-20240330/utils/update_release.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 05:16:55.373897 dfdatetime-20240504/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 05:16:55.358897 dfdatetime-20240504/.github/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 05:16:55.360897 dfdatetime-20240504/.github/workflows/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2024-05-04 05:02:31.000000 dfdatetime-20240504/.github/workflows/test_docker.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1359 2024-05-04 05:02:31.000000 dfdatetime-20240504/.github/workflows/test_docs.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4131 2024-05-04 05:02:31.000000 dfdatetime-20240504/.github/workflows/test_tox.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23143 2024-05-04 05:02:31.000000 dfdatetime-20240504/.pylintrc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      322 2024-05-04 05:02:31.000000 dfdatetime-20240504/.readthedocs.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      661 2023-12-03 10:50:32.000000 dfdatetime-20240504/ACKNOWLEDGEMENTS
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      368 2023-12-03 10:50:32.000000 dfdatetime-20240504/AUTHORS
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11358 2023-12-03 10:50:32.000000 dfdatetime-20240504/LICENSE
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      497 2023-12-03 10:50:32.000000 dfdatetime-20240504/MANIFEST.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      659 2024-05-04 05:16:55.373897 dfdatetime-20240504/PKG-INFO
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      213 2023-12-03 10:50:32.000000 dfdatetime-20240504/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2321 2024-05-04 05:02:31.000000 dfdatetime-20240504/appveyor.yml
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 05:16:55.358897 dfdatetime-20240504/config/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 05:16:55.360897 dfdatetime-20240504/config/appveyor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      798 2024-05-04 05:02:31.000000 dfdatetime-20240504/config/appveyor/install.ps1
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2024-05-04 05:02:31.000000 dfdatetime-20240504/config/appveyor/install.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2024-05-04 05:02:31.000000 dfdatetime-20240504/config/appveyor/runtests.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 05:16:55.361897 dfdatetime-20240504/config/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      173 2024-05-04 05:03:35.000000 dfdatetime-20240504/config/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       23 2023-12-03 10:55:02.000000 dfdatetime-20240504/config/dpkg/clean
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        2 2024-05-04 05:02:31.000000 dfdatetime-20240504/config/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      554 2024-05-04 05:02:31.000000 dfdatetime-20240504/config/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      968 2023-12-03 10:55:02.000000 dfdatetime-20240504/config/dpkg/copyright
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2024-05-04 05:02:31.000000 dfdatetime-20240504/config/dpkg/rules
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 05:16:55.361897 dfdatetime-20240504/config/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2023-12-03 10:55:02.000000 dfdatetime-20240504/config/dpkg/source/format
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 05:16:55.362897 dfdatetime-20240504/config/pylint/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      229 2023-12-03 10:55:01.000000 dfdatetime-20240504/config/pylint/spelling-private-dict
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-12-03 10:50:32.000000 dfdatetime-20240504/dependencies.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 05:16:55.366897 dfdatetime-20240504/dfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      870 2024-05-04 05:03:35.000000 dfdatetime-20240504/dfdatetime/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2595 2024-02-20 18:00:00.000000 dfdatetime-20240504/dfdatetime/apfs_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4524 2024-02-23 17:55:36.000000 dfdatetime-20240504/dfdatetime/cocoa_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      710 2024-02-20 18:00:00.000000 dfdatetime-20240504/dfdatetime/decorators.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2585 2024-05-04 04:46:35.000000 dfdatetime-20240504/dfdatetime/definitions.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5313 2024-02-23 17:55:36.000000 dfdatetime-20240504/dfdatetime/delphi_date_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4812 2024-02-23 17:55:36.000000 dfdatetime-20240504/dfdatetime/dotnet_datetime.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1846 2024-02-20 18:00:00.000000 dfdatetime-20240504/dfdatetime/factory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4273 2024-02-23 17:55:36.000000 dfdatetime-20240504/dfdatetime/fake_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10557 2024-02-23 17:55:36.000000 dfdatetime-20240504/dfdatetime/fat_date_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4895 2024-02-23 17:55:36.000000 dfdatetime-20240504/dfdatetime/filetime.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7664 2024-02-23 17:55:36.000000 dfdatetime-20240504/dfdatetime/golang_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4379 2024-02-23 17:55:36.000000 dfdatetime-20240504/dfdatetime/hfs_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31580 2024-03-30 04:44:58.000000 dfdatetime-20240504/dfdatetime/interface.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1977 2024-02-20 18:00:00.000000 dfdatetime-20240504/dfdatetime/java_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5061 2024-02-23 17:55:36.000000 dfdatetime-20240504/dfdatetime/ole_automation_date.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16377 2024-02-23 17:55:36.000000 dfdatetime-20240504/dfdatetime/posix_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13969 2024-05-04 04:46:35.000000 dfdatetime-20240504/dfdatetime/precisions.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8173 2024-02-23 17:55:36.000000 dfdatetime-20240504/dfdatetime/rfc2579_date_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9079 2024-02-20 18:00:00.000000 dfdatetime-20240504/dfdatetime/semantic_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7583 2024-02-20 18:00:00.000000 dfdatetime-20240504/dfdatetime/serializer.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7313 2024-02-23 17:55:36.000000 dfdatetime-20240504/dfdatetime/systemtime.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    51813 2024-05-04 04:58:39.000000 dfdatetime-20240504/dfdatetime/time_elements.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5092 2024-02-23 17:55:36.000000 dfdatetime-20240504/dfdatetime/uuid_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4752 2024-02-23 17:55:36.000000 dfdatetime-20240504/dfdatetime/webkit_time.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 05:16:55.373897 dfdatetime-20240504/dfdatetime.egg-info/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      659 2024-05-04 05:16:55.000000 dfdatetime-20240504/dfdatetime.egg-info/PKG-INFO
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2186 2024-05-04 05:16:55.000000 dfdatetime-20240504/dfdatetime.egg-info/SOURCES.txt
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        1 2024-05-04 05:16:55.000000 dfdatetime-20240504/dfdatetime.egg-info/dependency_links.txt
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       11 2024-05-04 05:16:55.000000 dfdatetime-20240504/dfdatetime.egg-info/top_level.txt
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      760 2023-12-03 10:50:32.000000 dfdatetime-20240504/dfdatetime.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 05:16:55.367897 dfdatetime-20240504/docs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5115 2024-05-04 05:02:31.000000 dfdatetime-20240504/docs/conf.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      593 2023-12-03 10:55:02.000000 dfdatetime-20240504/docs/index.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      118 2024-05-04 05:02:31.000000 dfdatetime-20240504/docs/requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 05:16:55.367897 dfdatetime-20240504/docs/sources/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16776 2024-02-23 17:55:36.000000 dfdatetime-20240504/docs/sources/Date-and-time-values.md
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 05:16:55.367897 dfdatetime-20240504/docs/sources/api/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3945 2023-12-03 10:55:02.000000 dfdatetime-20240504/docs/sources/api/dfdatetime.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 10:55:02.000000 dfdatetime-20240504/docs/sources/api/modules.rst
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 05:16:55.368897 dfdatetime-20240504/docs/sources/user/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1662 2024-02-11 07:44:31.000000 dfdatetime-20240504/docs/sources/user/Installation-instructions.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      292 2023-12-03 10:55:02.000000 dfdatetime-20240504/docs/sources/user/index.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      296 2024-05-04 05:02:31.000000 dfdatetime-20240504/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 05:02:31.000000 dfdatetime-20240504/requirements.txt
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1018 2023-12-03 10:50:32.000000 dfdatetime-20240504/run_tests.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      888 2024-05-04 05:16:55.375897 dfdatetime-20240504/setup.cfg
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      128 2024-05-04 05:02:31.000000 dfdatetime-20240504/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-12-03 10:50:32.000000 dfdatetime-20240504/test_dependencies.ini
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 05:02:31.000000 dfdatetime-20240504/test_requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 05:16:55.371897 dfdatetime-20240504/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2024-02-20 18:03:28.000000 dfdatetime-20240504/tests/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2219 2024-02-20 18:03:28.000000 dfdatetime-20240504/tests/apfs_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6053 2024-02-23 17:55:36.000000 dfdatetime-20240504/tests/cocoa_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8316 2024-02-23 17:55:36.000000 dfdatetime-20240504/tests/delphi_date_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3591 2024-02-23 17:55:36.000000 dfdatetime-20240504/tests/dotnet_datetime.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2646 2024-02-20 18:03:28.000000 dfdatetime-20240504/tests/factory.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6031 2024-02-23 17:55:36.000000 dfdatetime-20240504/tests/fake_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12242 2024-02-23 17:55:36.000000 dfdatetime-20240504/tests/fat_date_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5550 2024-02-23 17:55:36.000000 dfdatetime-20240504/tests/filetime.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8431 2024-02-23 17:55:36.000000 dfdatetime-20240504/tests/golang_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5525 2024-02-23 17:55:36.000000 dfdatetime-20240504/tests/hfs_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22873 2024-03-30 05:09:36.000000 dfdatetime-20240504/tests/interface.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5014 2024-02-23 17:55:36.000000 dfdatetime-20240504/tests/java_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6506 2024-02-23 17:55:36.000000 dfdatetime-20240504/tests/ole_automation_date.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24682 2024-02-23 17:55:36.000000 dfdatetime-20240504/tests/posix_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8079 2024-05-04 04:46:35.000000 dfdatetime-20240504/tests/precisions.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12039 2024-02-23 17:55:36.000000 dfdatetime-20240504/tests/rfc2579_date_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7979 2024-02-20 18:03:28.000000 dfdatetime-20240504/tests/semantic_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11261 2024-02-20 18:03:28.000000 dfdatetime-20240504/tests/serializer.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9420 2024-02-23 17:55:36.000000 dfdatetime-20240504/tests/systemtime.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98297 2024-05-04 05:00:53.000000 dfdatetime-20240504/tests/time_elements.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7131 2024-02-23 17:55:36.000000 dfdatetime-20240504/tests/uuid_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5686 2024-02-23 17:55:36.000000 dfdatetime-20240504/tests/webkit_time.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1297 2024-05-04 05:02:31.000000 dfdatetime-20240504/tox.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-04 05:16:55.372897 dfdatetime-20240504/utils/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 10:55:04.000000 dfdatetime-20240504/utils/__init__.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2024-05-04 05:02:31.000000 dfdatetime-20240504/utils/check_dependencies.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2024-05-04 05:02:31.000000 dfdatetime-20240504/utils/dependencies.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      779 2024-01-28 09:26:26.000000 dfdatetime-20240504/utils/update_release.sh
```

### Comparing `dfdatetime-20240330/.github/workflows/test_docker.yml` & `dfdatetime-20240504/.github/workflows/test_docker.yml`

 * *Files 15% similar despite different names*

```diff
@@ -7,78 +7,67 @@
     runs-on: ubuntu-latest
     strategy:
       matrix:
         version: ['39', '40']
     container:
       image: registry.fedoraproject.org/fedora:${{ matrix.version }}
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up container
       run: |
         dnf install -y dnf-plugins-core langpacks-en
     - name: Install dependencies
       run: |
         dnf copr -y enable @gift/dev
-        dnf install -y @development-tools python3 python3-devel python3-setuptools
+        dnf install -y @development-tools python3 python3-build python3-devel python3-setuptools python3-wheel
     - name: Run tests
       env:
         LANG: C.utf8
       run: |
         python3 ./run_tests.py
     - name: Run end-to-end tests
       run: |
         if test -f tests/end-to-end.py; then PYTHONPATH=. python3 ./tests/end-to-end.py --debug -c config/end-to-end.ini; fi
-    - name: Build source distribution
+    - name: Build source distribution (sdist)
       run: |
-        python3 ./setup.py sdist
-    - name: Build binary distribution
+        python3 -m build --no-isolation --sdist
+    - name: Build binary distribution (wheel)
       run: |
-        python3 ./setup.py bdist
-    - name: Run build and install test
-      run: |
-        python3 ./setup.py build
-        python3 ./setup.py install
+        python3 -m build --no-isolation --wheel
   test_ubuntu:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         version: ['24.04']
     container:
       image: ubuntu:${{ matrix.version }}
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         apt-get update -q
         apt-get install -y libterm-readline-gnu-perl locales software-properties-common
         locale-gen en_US.UTF-8
         ln -f -s /usr/share/zoneinfo/UTC /etc/localtime
     - name: Install dependencies
       run: |
         add-apt-repository -y ppa:gift/dev
         apt-get update -q
-        apt-get install -y build-essential python3 python3-dev python3-distutils python3-pip python3-setuptools python3-wheel
+        apt-get install -y build-essential python3 python3-build python3-dev python3-pip python3-setuptools python3-wheel
     - name: Run tests
       env:
         LANG: en_US.UTF-8
       run: |
         python3 ./run_tests.py
     - name: Run end-to-end tests
       env:
         LANG: en_US.UTF-8
       run: |
         if test -f tests/end-to-end.py; then PYTHONPATH=. python3 ./tests/end-to-end.py --debug -c config/end-to-end.ini; fi
-    - name: Update setuptools
-      run: |
-        python3 -m pip install -U setuptools
-    - name: Build source distribution
-      run: |
-        python3 ./setup.py sdist
-    - name: Build binary distribution
+    - name: Build source distribution (sdist)
       run: |
-        python3 ./setup.py bdist
-    - name: Run build and install test
+        python3 -m build --no-isolation --sdist
+    - name: Build binary distribution (wheel)
       run: |
-        python3 ./setup.py build
-        python3 ./setup.py install
+        python3 -m build --no-isolation --wheel
```

### Comparing `dfdatetime-20240330/.github/workflows/test_docs.yml` & `dfdatetime-20240504/.github/workflows/test_docs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       matrix:
         include:
         - python-version: '3.12'
           toxenv: 'docs'
     container:
       image: ubuntu:22.04
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         apt-get update -q
         apt-get install -y libterm-readline-gnu-perl locales software-properties-common
         locale-gen en_US.UTF-8
@@ -32,15 +32,15 @@
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         add-apt-repository -y universe
         add-apt-repository -y ppa:deadsnakes/ppa
         add-apt-repository -y ppa:gift/dev
         apt-get update -q
-        apt-get install -y build-essential git python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv python3-distutils python3-pip python3-setuptools
+        apt-get install -y build-essential git  python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv python3-distutils python3-lib2to3 python3-pip python3-setuptools
     - name: Install tox
       run: |
         python3 -m pip install tox
     - name: Run tests
       env:
         LANG: en_US.UTF-8
       run: |
```

### Comparing `dfdatetime-20240330/.github/workflows/test_tox.yml` & `dfdatetime-20240504/.github/workflows/test_tox.yml`

 * *Files 12% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         - python-version: '3.11'
           toxenv: 'py311,wheel'
         - python-version: '3.12'
           toxenv: 'py312,wheel'
     container:
       image: ubuntu:22.04
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         apt-get update -q
         apt-get install -y libterm-readline-gnu-perl locales software-properties-common
         locale-gen en_US.UTF-8
@@ -40,15 +40,15 @@
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         add-apt-repository -y universe
         add-apt-repository -y ppa:deadsnakes/ppa
         add-apt-repository -y ppa:gift/dev
         apt-get update -q
-        apt-get install -y build-essential git python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv python3-distutils python3-pip python3-setuptools
+        apt-get install -y build-essential git  python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv python3-distutils python3-lib2to3 python3-pip python3-setuptools
     - name: Install tox
       run: |
         python3 -m pip install tox
     - name: Run tests
       env:
         LANG: en_US.UTF-8
       run: |
@@ -59,15 +59,15 @@
       matrix:
         include:
         - python-version: '3.10'
           toxenv: 'coverage'
     container:
       image: ubuntu:22.04
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         apt-get update -q
         apt-get install -y libterm-readline-gnu-perl locales software-properties-common
         locale-gen en_US.UTF-8
@@ -76,36 +76,38 @@
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         add-apt-repository -y universe
         add-apt-repository -y ppa:deadsnakes/ppa
         add-apt-repository -y ppa:gift/dev
         apt-get update -q
-        apt-get install -y build-essential git python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv python3-distutils python3-pip python3-setuptools
+        apt-get install -y build-essential git  python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv python3-distutils python3-lib2to3 python3-pip python3-setuptools
     - name: Install tox
       run: |
         python3 -m pip install tox
     - name: Run tests with coverage
       env:
         LANG: en_US.UTF-8
       run: |
         tox -e${{ matrix.toxenv }}
     - name: Upload coverage report to Codecov
-      uses: codecov/codecov-action@v3
+      uses: codecov/codecov-action@v4
+      with:
+        token: ${{ secrets.CODECOV_TOKEN }}
   lint:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         include:
         - python-version: '3.12'
           toxenv: 'lint'
     container:
       image: ubuntu:22.04
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up container
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         apt-get update -q
         apt-get install -y libterm-readline-gnu-perl locales software-properties-common
         locale-gen en_US.UTF-8
@@ -114,15 +116,15 @@
       env:
         DEBIAN_FRONTEND: noninteractive
       run: |
         add-apt-repository -y universe
         add-apt-repository -y ppa:deadsnakes/ppa
         add-apt-repository -y ppa:gift/dev
         apt-get update -q
-        apt-get install -y build-essential git python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv python3-distutils python3-pip python3-setuptools
+        apt-get install -y build-essential git  python${{ matrix.python-version }} python${{ matrix.python-version }}-dev python${{ matrix.python-version }}-venv python3-distutils python3-lib2to3 python3-pip python3-setuptools
     - name: Install tox
       run: |
         python3 -m pip install tox
     - name: Run linter
       env:
         LANG: en_US.UTF-8
       run: |
```

### Comparing `dfdatetime-20240330/.pylintrc` & `dfdatetime-20240504/.pylintrc`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/ACKNOWLEDGEMENTS` & `dfdatetime-20240504/ACKNOWLEDGEMENTS`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/LICENSE` & `dfdatetime-20240504/LICENSE`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/PKG-INFO` & `dfdatetime-20240504/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfdatetime
-Version: 20240330
+Version: 20240504
 Summary: Digital Forensics date and time (dfDateTime).
 Home-page: https://github.com/log2timeline/dfdatetime
 Maintainer: Log2Timeline maintainers
 Maintainer-email: log2timeline-maintainers@googlegroups.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
```

### Comparing `dfdatetime-20240330/appveyor.yml` & `dfdatetime-20240504/appveyor.yml`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/config/appveyor/install.ps1` & `dfdatetime-20240504/config/appveyor/install.ps1`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/config/appveyor/runtests.sh` & `dfdatetime-20240504/config/appveyor/runtests.sh`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/config/dpkg/control` & `dfdatetime-20240504/config/dpkg/control`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/config/dpkg/copyright` & `dfdatetime-20240504/config/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/dfdatetime/__init__.py` & `dfdatetime-20240504/dfdatetime/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 from dfdatetime import semantic_time
 from dfdatetime import systemtime
 from dfdatetime import time_elements
 from dfdatetime import uuid_time
 from dfdatetime import webkit_time
 
 
-__version__ = '20240330'
+__version__ = '20240504'
```

### Comparing `dfdatetime-20240330/dfdatetime/apfs_time.py` & `dfdatetime-20240504/dfdatetime/apfs_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/dfdatetime/cocoa_time.py` & `dfdatetime-20240504/dfdatetime/cocoa_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/dfdatetime/decorators.py` & `dfdatetime-20240504/dfdatetime/decorators.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/dfdatetime/definitions.py` & `dfdatetime-20240504/dfdatetime/definitions.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,25 +9,31 @@
 
 DAYS_PER_MONTH = (31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31)
 
 SECONDS_PER_DAY = 86400
 
 DECISECONDS_PER_SECOND = 10
 
+CENTISECONDS_PER_SECOND = 100
+
 MILLISECONDS_PER_SECOND = 1000
 
+DECIMICROSECONDS_PER_SECOND = 10000
+
 MICROSECONDS_PER_DAY = 86400000000
 MICROSECONDS_PER_SECOND = 1000000
 MICROSECONDS_PER_DECISECOND = 100000
 MICROSECONDS_PER_MILLISECOND = 1000
 
 NANOSECONDS_PER_DAY = 86400000000000
 NANOSECONDS_PER_SECOND = 1000000000
 NANOSECONDS_PER_DECISECOND = 100000000
+NANOSECONDS_PER_CENTISECOND = 10000000
 NANOSECONDS_PER_MILLISECOND = 1000000
+NANOSECONDS_PER_DECIMILISECOND = 100000
 NANOSECONDS_PER_MICROSECOND = 1000
 
 PRECISION_1_DAY = '1d'
 PRECISION_1_HOUR = '1h'
 PRECISION_1_NANOSECOND = '1ns'
 PRECISION_10_NANOSECONDS = '10s'
 PRECISION_100_NANOSECONDS = '100ns'
```

### Comparing `dfdatetime-20240330/dfdatetime/delphi_date_time.py` & `dfdatetime-20240504/dfdatetime/delphi_date_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/dfdatetime/dotnet_datetime.py` & `dfdatetime-20240504/dfdatetime/dotnet_datetime.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/dfdatetime/factory.py` & `dfdatetime-20240504/dfdatetime/factory.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/dfdatetime/fake_time.py` & `dfdatetime-20240504/dfdatetime/fake_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/dfdatetime/fat_date_time.py` & `dfdatetime-20240504/dfdatetime/fat_date_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/dfdatetime/filetime.py` & `dfdatetime-20240504/dfdatetime/filetime.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/dfdatetime/golang_time.py` & `dfdatetime-20240504/dfdatetime/golang_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/dfdatetime/hfs_time.py` & `dfdatetime-20240504/dfdatetime/hfs_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/dfdatetime/interface.py` & `dfdatetime-20240504/dfdatetime/interface.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/dfdatetime/java_time.py` & `dfdatetime-20240504/dfdatetime/java_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/dfdatetime/ole_automation_date.py` & `dfdatetime-20240504/dfdatetime/ole_automation_date.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/dfdatetime/posix_time.py` & `dfdatetime-20240504/dfdatetime/posix_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/dfdatetime/precisions.py` & `dfdatetime-20240504/dfdatetime/precisions.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,16 +21,16 @@
   def CopyNanosecondsToFractionOfSecond(cls, nanoseconds):
     """Copies the number of nanoseconds to a fraction of second value.
 
     Args:
       nanoseconds (int): number of nanoseconds.
 
     Returns:
-      decimal.Decimal: fraction of second, which must be a value between 0.0
-          and 1.0.
+      decimal.Decimal: fraction of second, which must be a value between 0.0 and
+          1.0.
     """
     raise NotImplementedError()
 
   @classmethod
   def CopyToDateTimeString(cls, time_elements_tuple, fraction_of_second):
     """Copies the time elements and fraction of second to a string.
 
@@ -95,14 +95,68 @@
 
     year, month, day_of_month, hours, minutes, seconds = time_elements_tuple
 
     return (f'{year:04d}-{month:02d}-{day_of_month:02d} '
             f'{hours:02d}:{minutes:02d}:{seconds:02d}')
 
 
+class CentisecondsPrecisionHelper(DateTimePrecisionHelper):
+  """Centiseconds (10 ms) precision helper."""
+
+  @classmethod
+  def CopyNanosecondsToFractionOfSecond(cls, nanoseconds):
+    """Copies the number of nanoseconds to a fraction of second value.
+
+    Args:
+      nanoseconds (int): number of nanoseconds.
+
+    Returns:
+      decimal.Decimal: fraction of second, which must be a value between 0.0 and
+          1.0.
+
+    Raises:
+      ValueError: if the number of nanoseconds is out of bounds.
+    """
+    if nanoseconds < 0 or nanoseconds >= definitions.NANOSECONDS_PER_SECOND:
+      raise ValueError(
+          f'Number of nanoseconds value: {nanoseconds:d} out of bounds.')
+
+    centiseconds, _ = divmod(
+        nanoseconds, definitions.NANOSECONDS_PER_CENTISECOND)
+    return decimal.Decimal(centiseconds) / definitions.CENTISECONDS_PER_SECOND
+
+  @classmethod
+  def CopyToDateTimeString(cls, time_elements_tuple, fraction_of_second):
+    """Copies the time elements and fraction of second to a string.
+
+    Args:
+      time_elements_tuple (tuple[int, int, int, int, int, int]):
+          time elements, contains year, month, day of month, hours, minutes and
+          seconds.
+      fraction_of_second (decimal.Decimal): fraction of second, which must be a
+          value between 0.0 and 1.0.
+
+    Returns:
+      str: date and time value formatted as:
+          YYYY-MM-DD hh:mm:ss.##
+
+    Raises:
+      ValueError: if the fraction of second is out of bounds.
+    """
+    if fraction_of_second < 0.0 or fraction_of_second >= 1.0:
+      raise ValueError(
+          f'Fraction of second value: {fraction_of_second:f} out of bounds.')
+
+    year, month, day_of_month, hours, minutes, seconds = time_elements_tuple
+    centiseconds = int(fraction_of_second * definitions.CENTISECONDS_PER_SECOND)
+
+    return (f'{year:04d}-{month:02d}-{day_of_month:02d} '
+            f'{hours:02d}:{minutes:02d}:{seconds:02d}.{centiseconds:02d}')
+
+
 class MillisecondsPrecisionHelper(DateTimePrecisionHelper):
   """Milliseconds precision helper."""
 
   @classmethod
   def CopyNanosecondsToFractionOfSecond(cls, nanoseconds):
     """Copies the number of nanoseconds to a fraction of second value.
 
@@ -149,14 +203,71 @@
     year, month, day_of_month, hours, minutes, seconds = time_elements_tuple
     milliseconds = int(fraction_of_second * definitions.MILLISECONDS_PER_SECOND)
 
     return (f'{year:04d}-{month:02d}-{day_of_month:02d} '
             f'{hours:02d}:{minutes:02d}:{seconds:02d}.{milliseconds:03d}')
 
 
+class DecimillisecondsPrecisionHelper(DateTimePrecisionHelper):
+  """Decimilliseconds (100 microseconds) precision helper."""
+
+  @classmethod
+  def CopyNanosecondsToFractionOfSecond(cls, nanoseconds):
+    """Copies the number of nanoseconds to a fraction of second value.
+
+    Args:
+      nanoseconds (int): number of nanoseconds.
+
+    Returns:
+      decimal.Decimal: fraction of second, which must be a value between 0.0
+          and 1.0.
+
+    Raises:
+      ValueError: if the number of nanoseconds is out of bounds.
+    """
+    if nanoseconds < 0 or nanoseconds >= definitions.NANOSECONDS_PER_SECOND:
+      raise ValueError(
+          f'Number of nanoseconds value: {nanoseconds:d} out of bounds.')
+
+    decimiliseconds, _ = divmod(
+        nanoseconds, definitions.NANOSECONDS_PER_DECIMILISECOND)
+    return (
+        decimal.Decimal(decimiliseconds) /
+        definitions.DECIMICROSECONDS_PER_SECOND)
+
+  @classmethod
+  def CopyToDateTimeString(cls, time_elements_tuple, fraction_of_second):
+    """Copies the time elements and fraction of second to a string.
+
+    Args:
+      time_elements_tuple (tuple[int, int, int, int, int, int]):
+          time elements, contains year, month, day of month, hours, minutes and
+          seconds.
+      fraction_of_second (decimal.Decimal): fraction of second, which must be a
+          value between 0.0 and 1.0.
+
+    Returns:
+      str: date and time value formatted as:
+          YYYY-MM-DD hh:mm:ss.####
+
+    Raises:
+      ValueError: if the fraction of second is out of bounds.
+    """
+    if fraction_of_second < 0.0 or fraction_of_second >= 1.0:
+      raise ValueError(
+          f'Fraction of second value: {fraction_of_second:f} out of bounds.')
+
+    year, month, day_of_month, hours, minutes, seconds = time_elements_tuple
+    decimicroseconds = int(
+        fraction_of_second * definitions.DECIMICROSECONDS_PER_SECOND)
+
+    return (f'{year:04d}-{month:02d}-{day_of_month:02d} '
+            f'{hours:02d}:{minutes:02d}:{seconds:02d}.{decimicroseconds:04d}')
+
+
 class MicrosecondsPrecisionHelper(DateTimePrecisionHelper):
   """Microseconds precision helper."""
 
   @classmethod
   def CopyNanosecondsToFractionOfSecond(cls, nanoseconds):
     """Copies the number of nanoseconds to a fraction of second value.
 
@@ -259,14 +370,16 @@
             f'{hours:02d}:{minutes:02d}:{seconds:02d}.{nanoseconds:09d}')
 
 
 class PrecisionHelperFactory(object):
   """Date time precision helper factory."""
 
   _PRECISION_CLASSES = {
+      definitions.PRECISION_10_MILLISECONDS: CentisecondsPrecisionHelper,
+      definitions.PRECISION_100_MICROSECONDS: DecimillisecondsPrecisionHelper,
       definitions.PRECISION_1_MICROSECOND: MicrosecondsPrecisionHelper,
       definitions.PRECISION_1_MILLISECOND: MillisecondsPrecisionHelper,
       definitions.PRECISION_1_NANOSECOND: NanosecondsPrecisionHelper,
       definitions.PRECISION_1_SECOND: SecondsPrecisionHelper}
 
   @classmethod
   def CreatePrecisionHelper(cls, precision):
```

### Comparing `dfdatetime-20240330/dfdatetime/rfc2579_date_time.py` & `dfdatetime-20240504/dfdatetime/rfc2579_date_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/dfdatetime/semantic_time.py` & `dfdatetime-20240504/dfdatetime/semantic_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/dfdatetime/serializer.py` & `dfdatetime-20240504/dfdatetime/serializer.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/dfdatetime/systemtime.py` & `dfdatetime-20240504/dfdatetime/systemtime.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/dfdatetime/time_elements.py` & `dfdatetime-20240504/dfdatetime/time_elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -1400,10 +1400,158 @@
 
     Raises:
       ValueError: if the instance is not a date time delta.
     """
     return self.NewFromDeltaAndDate(year, 0, 0)
 
 
+class TimeElementsInNanoseconds(TimeElementsWithFractionOfSecond):
+  """Time elements in nanoseconds.
+
+  Attributes:
+    fraction_of_second (decimal.Decimal): fraction of second, which must be a
+        value between 0.0 and 1.0.
+    is_local_time (bool): True if the date and time value is in local time.
+    precision (str): precision of the date of the date and time value, that
+        represents 1 nanosecond (PRECISION_1_NANOSECOND).
+  """
+
+  def __init__(
+      self, is_delta=False, precision=None, time_elements_tuple=None,
+      time_zone_offset=None):
+    """Initializes time elements.
+
+    Args:
+      is_delta (Optional[bool]): True if the date and time value is relative to
+          another date and time value.
+      precision (Optional[str]): precision of the date and time value, which
+          should be one of the PRECISION_VALUES in definitions.
+      time_elements_tuple (Optional[tuple[int, int, int, int, int, int, int]]):
+          time elements, contains year, month, day of month, hours, minutes,
+          seconds and nanoseconds.
+      time_zone_offset (Optional[int]): time zone offset in number of minutes
+          from UTC or None if not set.
+
+    Raises:
+      ValueError: if the time elements tuple is invalid.
+    """
+    fraction_of_second = None
+    if time_elements_tuple:
+      number_of_elements = len(time_elements_tuple)
+      if number_of_elements < 7:
+        raise ValueError((
+            f'Invalid time elements tuple at least 7 elements required,'
+            f'got: {number_of_elements:d}'))
+
+      nanoseconds = time_elements_tuple[6]
+      time_elements_tuple = time_elements_tuple[:6]
+
+      if (nanoseconds < 0 or
+          nanoseconds >= definitions.NANOSECONDS_PER_SECOND):
+        raise ValueError('Invalid number of nanoseconds.')
+
+      fraction_of_second = (
+          decimal.Decimal(nanoseconds) / definitions.NANOSECONDS_PER_SECOND)
+
+    super(TimeElementsInNanoseconds, self).__init__(
+        fraction_of_second=fraction_of_second, is_delta=is_delta,
+        precision=precision or definitions.PRECISION_1_NANOSECOND,
+        time_elements_tuple=time_elements_tuple,
+        time_zone_offset=time_zone_offset)
+
+  @property
+  def nanoseconds(self):
+    """int: number of nanoseconds."""
+    return int(self.fraction_of_second * definitions.NANOSECONDS_PER_SECOND)
+
+  def CopyFromStringTuple(self, time_elements_tuple):
+    """Copies time elements from string-based time elements tuple.
+
+    Args:
+      time_elements_tuple (Optional[tuple[str, str, str, str, str, str, str]]):
+          time elements, contains year, month, day of month, hours, minutes,
+          seconds and nanoseconds.
+
+    Raises:
+      ValueError: if the time elements tuple is invalid.
+    """
+    number_of_elements = len(time_elements_tuple)
+    if len(time_elements_tuple) < 7:
+      raise ValueError((
+          f'Invalid time elements tuple at least 7 elements required,'
+          f'got: {number_of_elements:d}'))
+
+    year, month, day_of_month, hours, minutes, seconds, nanoseconds = (
+        time_elements_tuple)
+
+    try:
+      nanoseconds = int(nanoseconds, 10)
+    except (TypeError, ValueError):
+      raise ValueError(f'Invalid nanosecond value: {nanoseconds!s}')
+
+    if nanoseconds < 0 or nanoseconds >= definitions.NANOSECONDS_PER_SECOND:
+      raise ValueError('Invalid number of nanoseconds.')
+
+    fraction_of_second = (
+        decimal.Decimal(nanoseconds) / definitions.NANOSECONDS_PER_SECOND)
+
+    time_elements_tuple = (
+        year, month, day_of_month, hours, minutes, seconds,
+        str(fraction_of_second))
+
+    super(TimeElementsInNanoseconds, self).CopyFromStringTuple(
+        time_elements_tuple)
+
+  def NewFromDeltaAndDate(self, year, month, day_of_month):
+    """Creates a new time elements instance from a date time delta and a year.
+
+    Args:
+      year (int): year.
+      month (int): month, where 1 represents January and 0 if not set.
+      day_of_month (int): day of month, where 1 represents the first day and 0
+          if not set.
+
+    Returns:
+      TimeElementsInNanoseconds: time elements or None if time elements are
+          missing.
+
+    Raises:
+      ValueError: if the instance is not a date time delta.
+    """
+    if not self._is_delta:
+      raise ValueError('Not a date time delta.')
+
+    if self._time_elements_tuple is None:
+      return None
+
+    delta_year, delta_month, delta_day_of_month, hours, minutes, seconds = (
+        self._time_elements_tuple)
+
+    time_elements_tuple = (
+        year + delta_year, month + delta_month,
+        day_of_month + delta_day_of_month, hours, minutes, seconds,
+        self.nanoseconds)
+
+    return TimeElementsInNanoseconds(
+        precision=self._precision, time_elements_tuple=time_elements_tuple,
+        time_zone_offset=self._time_zone_offset)
+
+  def NewFromDeltaAndYear(self, year):
+    """Creates a new time elements instance from a date time delta and a year.
+
+    Args:
+      year (int): year.
+
+    Returns:
+      TimeElementsInNanoseconds: time elements or None if time elements are
+          missing.
+
+    Raises:
+      ValueError: if the instance is not a date time delta.
+    """
+    return self.NewFromDeltaAndDate(year, 0, 0)
+
+
 factory.Factory.RegisterDateTimeValues(TimeElements)
 factory.Factory.RegisterDateTimeValues(TimeElementsInMilliseconds)
 factory.Factory.RegisterDateTimeValues(TimeElementsInMicroseconds)
+factory.Factory.RegisterDateTimeValues(TimeElementsInNanoseconds)
```

### Comparing `dfdatetime-20240330/dfdatetime/uuid_time.py` & `dfdatetime-20240504/dfdatetime/uuid_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/dfdatetime/webkit_time.py` & `dfdatetime-20240504/dfdatetime/webkit_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/dfdatetime.egg-info/PKG-INFO` & `dfdatetime-20240504/dfdatetime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfdatetime
-Version: 20240330
+Version: 20240504
 Summary: Digital Forensics date and time (dfDateTime).
 Home-page: https://github.com/log2timeline/dfdatetime
 Maintainer: Log2Timeline maintainers
 Maintainer-email: log2timeline-maintainers@googlegroups.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
```

### Comparing `dfdatetime-20240330/dfdatetime.egg-info/SOURCES.txt` & `dfdatetime-20240504/dfdatetime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/dfdatetime.ini` & `dfdatetime-20240504/dfdatetime.ini`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/docs/conf.py` & `dfdatetime-20240504/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/docs/index.rst` & `dfdatetime-20240504/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/docs/sources/Date-and-time-values.md` & `dfdatetime-20240504/docs/sources/Date-and-time-values.md`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/docs/sources/api/dfdatetime.rst` & `dfdatetime-20240504/docs/sources/api/dfdatetime.rst`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/docs/sources/user/Installation-instructions.md` & `dfdatetime-20240504/docs/sources/user/Installation-instructions.md`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/run_tests.py` & `dfdatetime-20240504/run_tests.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/setup.cfg` & `dfdatetime-20240504/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dfdatetime
-version = 20240330
+version = 20240504
 description = Digital Forensics date and time (dfDateTime).
 long_description = dfDateTime, or Digital Forensics date and time, provides date and time objects to preserve accuracy and precision.
 long_description_content_type = text/plain
 url = https://github.com/log2timeline/dfdatetime
 maintainer = Log2Timeline maintainers
 maintainer_email = log2timeline-maintainers@googlegroups.com
 license = Apache License, Version 2.0
```

### Comparing `dfdatetime-20240330/tests/apfs_time.py` & `dfdatetime-20240504/tests/apfs_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/tests/cocoa_time.py` & `dfdatetime-20240504/tests/cocoa_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/tests/delphi_date_time.py` & `dfdatetime-20240504/tests/delphi_date_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/tests/dotnet_datetime.py` & `dfdatetime-20240504/tests/dotnet_datetime.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/tests/factory.py` & `dfdatetime-20240504/tests/factory.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/tests/fake_time.py` & `dfdatetime-20240504/tests/fake_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/tests/fat_date_time.py` & `dfdatetime-20240504/tests/fat_date_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/tests/filetime.py` & `dfdatetime-20240504/tests/filetime.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/tests/golang_time.py` & `dfdatetime-20240504/tests/golang_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/tests/hfs_time.py` & `dfdatetime-20240504/tests/hfs_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/tests/interface.py` & `dfdatetime-20240504/tests/interface.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/tests/java_time.py` & `dfdatetime-20240504/tests/java_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/tests/ole_automation_date.py` & `dfdatetime-20240504/tests/ole_automation_date.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/tests/posix_time.py` & `dfdatetime-20240504/tests/posix_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/tests/precisions.py` & `dfdatetime-20240504/tests/precisions.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,14 +52,43 @@
         (2018, 1, 2, 19, 45, 12), 0.123456)
     self.assertEqual(date_time_string, '2018-01-02 19:45:12')
 
     with self.assertRaises(ValueError):
       precision_helper.CopyToDateTimeString((2018, 1, 2, 19, 45, 12), 4.123456)
 
 
+class CentisecondsPrevisionHelperTest(unittest.TestCase):
+  """Tests for the centiseconds prevision helper."""
+
+  def testCopyNanosecondsToFractionOfSecond(self):
+    """Tests the CopyNanosecondsToFractionOfSecond function."""
+    precision_helper = precisions.CentisecondsPrecisionHelper
+
+    fraction_of_second = precision_helper.CopyNanosecondsToFractionOfSecond(
+        123456789)
+    self.assertEqual(fraction_of_second, decimal.Decimal('0.12'))
+
+    with self.assertRaises(ValueError):
+      precision_helper.CopyNanosecondsToFractionOfSecond(-1)
+
+    with self.assertRaises(ValueError):
+      precision_helper.CopyNanosecondsToFractionOfSecond(1000000000)
+
+  def testCopyToDateTimeString(self):
+    """Tests the CopyToDateTimeString function."""
+    precision_helper = precisions.CentisecondsPrecisionHelper
+
+    date_time_string = precision_helper.CopyToDateTimeString(
+        (2018, 1, 2, 19, 45, 12), 0.123456)
+    self.assertEqual(date_time_string, '2018-01-02 19:45:12.12')
+
+    with self.assertRaises(ValueError):
+      precision_helper.CopyToDateTimeString((2018, 1, 2, 19, 45, 12), 4.123456)
+
+
 class MillisecondsPrecisionHelperTest(unittest.TestCase):
   """Tests for the milliseconds precision helper."""
 
   def testCopyNanosecondsToFractionOfSecond(self):
     """Tests the CopyNanosecondsToFractionOfSecond function."""
     precision_helper = precisions.MillisecondsPrecisionHelper
 
@@ -81,14 +110,42 @@
         (2018, 1, 2, 19, 45, 12), 0.123456)
     self.assertEqual(date_time_string, '2018-01-02 19:45:12.123')
 
     with self.assertRaises(ValueError):
       precision_helper.CopyToDateTimeString((2018, 1, 2, 19, 45, 12), 4.123456)
 
 
+class DeciMillisecondsPrevisionHelperTest(unittest.TestCase):
+  """Tests for the decimilliseconds precision helper."""
+  def testCopyNanosecondsToFractionOfSecond(self):
+    """Tests the CopyNanosecondsToFractionOfSecond function."""
+    precision_helper = precisions.DecimillisecondsPrecisionHelper
+
+    fraction_of_second = precision_helper.CopyNanosecondsToFractionOfSecond(
+        123456789)
+    self.assertEqual(fraction_of_second, decimal.Decimal('0.1234'))
+
+    with self.assertRaises(ValueError):
+      precision_helper.CopyNanosecondsToFractionOfSecond(-1)
+
+    with self.assertRaises(ValueError):
+      precision_helper.CopyNanosecondsToFractionOfSecond(1000000000)
+
+  def testCopyToDateTimeString(self):
+    """Tests the CopyToDateTimeString function."""
+    precision_helper = precisions.DecimillisecondsPrecisionHelper
+
+    date_time_string = precision_helper.CopyToDateTimeString(
+        (2018, 1, 2, 19, 45, 12), 0.123456)
+    self.assertEqual(date_time_string, '2018-01-02 19:45:12.1234')
+
+    with self.assertRaises(ValueError):
+      precision_helper.CopyToDateTimeString((2018, 1, 2, 19, 45, 12), 4.123456)
+
+
 class MicrosecondsPrecisionHelperTest(unittest.TestCase):
   """Tests for the microseconds precision helper."""
 
   def testCopyNanosecondsToFractionOfSecond(self):
     """Tests the CopyNanosecondsToFractionOfSecond function."""
     precision_helper = precisions.MicrosecondsPrecisionHelper
```

### Comparing `dfdatetime-20240330/tests/rfc2579_date_time.py` & `dfdatetime-20240504/tests/rfc2579_date_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/tests/semantic_time.py` & `dfdatetime-20240504/tests/semantic_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/tests/serializer.py` & `dfdatetime-20240504/tests/serializer.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/tests/systemtime.py` & `dfdatetime-20240504/tests/systemtime.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/tests/time_elements.py` & `dfdatetime-20240504/tests/time_elements.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 """Tests for the time elements implementation."""
 
 import datetime
 import decimal
 import unittest
 
+from dfdatetime import definitions
 from dfdatetime import time_elements
 
 
 class TimeElementsTest(unittest.TestCase):
   """Tests for the time elements."""
 
   # pylint: disable=protected-access
@@ -811,14 +812,252 @@
 
     time_elements_object = time_elements.TimeElements(is_delta=False)
 
     with self.assertRaises(ValueError):
       time_elements_object.NewFromDeltaAndYear(2009)
 
 
+class TimeElementsWithFractionOfSeconds(unittest.TestCase):
+  """Tests for the time elements with fractions of seconds."""
+
+  # pylint: disable=protected-access
+
+  def testInitialize(self):
+    """Tests the initialization function."""
+    time_elements_object = time_elements.TimeElementsWithFractionOfSecond()
+    self.assertIsNotNone(time_elements_object)
+
+    expected_time_elements_tuple = (2010, 8, 12, 20, 6, 31)
+    time_elements_object = time_elements.TimeElementsWithFractionOfSecond(
+        fraction_of_second=decimal.Decimal(0.87),
+        precision=definitions.PRECISION_10_MILLISECONDS,
+        time_elements_tuple=(2010, 8, 12, 20, 6, 31))
+    self.assertIsNotNone(time_elements_object)
+    self.assertEqual(
+        time_elements_object._time_elements_tuple, expected_time_elements_tuple)
+    self.assertEqual(time_elements_object.fraction_of_second, 0.87)
+
+    expected_time_elements_tuple = (2010, 8, 12, 20, 6, 31)
+    time_elements_object = time_elements.TimeElementsWithFractionOfSecond(
+        fraction_of_second=decimal.Decimal(0.8742),
+        precision=definitions.PRECISION_100_MICROSECONDS,
+        time_elements_tuple=(2010, 8, 12, 20, 6, 31))
+    self.assertIsNotNone(time_elements_object)
+    self.assertEqual(
+      time_elements_object._time_elements_tuple, expected_time_elements_tuple)
+    self.assertEqual(time_elements_object.fraction_of_second, 0.8742)
+
+    with self.assertRaises(ValueError):
+      time_elements.TimeElementsWithFractionOfSecond(
+          fraction_of_second=decimal.Decimal('1.87'),
+          precision=definitions.PRECISION_10_MILLISECONDS,
+          time_elements_tuple=(2010, 8, 12, 20, 6, 31))
+
+    with self.assertRaises(ValueError):
+      time_elements.TimeElementsWithFractionOfSecond(
+          fraction_of_second=decimal.Decimal('-1'),
+          precision=definitions.PRECISION_10_MILLISECONDS,
+          time_elements_tuple=(2010, 8, 12, 20, 6, 31))
+
+  def testGetNormalizedTimestamp(self):
+    """Tests the _GetNormalizedTimestamp function."""
+    time_elements_object = time_elements.TimeElementsWithFractionOfSecond(
+        fraction_of_second=decimal.Decimal('0.87'),
+        precision=definitions.PRECISION_10_MILLISECONDS,
+        time_elements_tuple=(2010, 8, 12, 20, 6, 31))
+    normalized_timestamp = time_elements_object._GetNormalizedTimestamp()
+    self.assertEqual(normalized_timestamp, decimal.Decimal('1281643591.87'))
+
+    time_elements_object = time_elements.TimeElementsWithFractionOfSecond(
+        fraction_of_second=decimal.Decimal('0.87'),
+        precision=definitions.PRECISION_10_MILLISECONDS,
+        time_elements_tuple=(2010, 8, 12, 20, 6, 31),
+        time_zone_offset=60)
+    normalized_timestamp = time_elements_object._GetNormalizedTimestamp()
+    self.assertEqual(normalized_timestamp, decimal.Decimal('1281639991.87'))
+
+    time_elements_object = time_elements.TimeElementsWithFractionOfSecond(
+        fraction_of_second=decimal.Decimal('0.87'),
+        precision=definitions.PRECISION_10_MILLISECONDS,
+        time_elements_tuple=(2010, 8, 12, 20, 6, 31))
+    time_elements_object.time_zone_offset = 60
+    normalized_timestamp = time_elements_object._GetNormalizedTimestamp()
+    self.assertEqual(normalized_timestamp, decimal.Decimal('1281639991.87'))
+
+    time_elements_object = time_elements.TimeElementsWithFractionOfSecond(
+        fraction_of_second=decimal.Decimal('0.8724'),
+        precision=definitions.PRECISION_100_MICROSECONDS,
+        time_elements_tuple=(2010, 8, 12, 20, 6, 31))
+    normalized_timestamp = time_elements_object._GetNormalizedTimestamp()
+    self.assertEqual(normalized_timestamp, decimal.Decimal('1281643591.8724'))
+
+    time_elements_object = time_elements.TimeElementsWithFractionOfSecond()
+    normalized_timestamp = time_elements_object._GetNormalizedTimestamp()
+    self.assertIsNone(normalized_timestamp)
+
+  def testCopyFromDateTimeValues(self):
+    """Tests the _CopyFromDateTimeValues function."""
+    date_time_values = {
+        'year': 2010,
+        'month': 8,
+        'day_of_month': 12,
+        'hours': 21,
+        'minutes': 6,
+        'seconds': 31,
+        'nanoseconds': 123456789,
+        'time_zone_offset': 60}
+
+    time_elements_object = time_elements.TimeElementsWithFractionOfSecond(
+        precision=definitions.PRECISION_10_MILLISECONDS)
+    time_elements_object._CopyFromDateTimeValues(date_time_values)
+
+    self.assertEqual(
+      time_elements_object._time_elements_tuple, (2010, 8, 12, 21, 6, 31))
+    self.assertEqual(
+      time_elements_object.fraction_of_second, decimal.Decimal('0.12'))
+
+    time_elements_object = time_elements.TimeElementsWithFractionOfSecond(
+        precision=definitions.PRECISION_1_MILLISECOND)
+    time_elements_object._CopyFromDateTimeValues(date_time_values)
+    self.assertEqual(
+      time_elements_object.fraction_of_second, decimal.Decimal('0.123'))
+
+    time_elements_object = time_elements.TimeElementsWithFractionOfSecond(
+        precision=definitions.PRECISION_100_MICROSECONDS)
+    time_elements_object._CopyFromDateTimeValues(date_time_values)
+    self.assertEqual(
+      time_elements_object.fraction_of_second, decimal.Decimal('0.1234'))
+
+  def testCopyFromDatetime(self):
+    """Tests the CopyFromDatetime function."""
+    datetime_object = datetime.datetime(2010, 8, 12, 21, 6, 31, 546875)
+    expected_time_elements_tuple = (2010, 8, 12, 21, 6, 31)
+    expected_number_of_seconds = 1281647191
+    expected_fraction_of_second = decimal.Decimal('0.54')
+
+    time_elements_object = time_elements.TimeElementsWithFractionOfSecond(
+      precision=definitions.PRECISION_10_MILLISECONDS)
+    time_elements_object.CopyFromDatetime(datetime_object)
+
+    self.assertEqual(
+        time_elements_object._time_elements_tuple, expected_time_elements_tuple)
+    self.assertEqual(
+        time_elements_object._number_of_seconds, expected_number_of_seconds)
+    self.assertEqual(
+        time_elements_object.fraction_of_second, expected_fraction_of_second)
+    self.assertTrue(time_elements_object.is_local_time)
+
+    datetime_object = datetime.datetime(
+        2010, 8, 12, 21, 6, 31, 546875, tzinfo=datetime.timezone.utc)
+    time_elements_object.CopyFromDatetime(datetime_object)
+    self.assertEqual(
+        time_elements_object._time_elements_tuple, expected_time_elements_tuple)
+    self.assertEqual(
+        time_elements_object._number_of_seconds, expected_number_of_seconds)
+    self.assertEqual(
+        time_elements_object.fraction_of_second, expected_fraction_of_second)
+    self.assertFalse(time_elements_object.is_local_time)
+
+  def testCopyFromStringTuple(self):
+    """Tests the CopyFromStringTuple function."""
+    time_elements_object = time_elements.TimeElementsWithFractionOfSecond(
+        precision=definitions.PRECISION_10_MILLISECONDS)
+
+    expected_time_elements_tuple = (2010, 8, 12, 20, 6, 31)
+    expected_fraction_of_second = decimal.Decimal('0.46')
+    time_elements_object.CopyFromStringTuple(
+        time_elements_tuple=('2010', '8', '12', '20', '6', '31', '0.46'))
+
+    self.assertEqual(
+        time_elements_object._time_elements_tuple, expected_time_elements_tuple)
+    self.assertEqual(
+        time_elements_object.fraction_of_second, expected_fraction_of_second)
+
+    time_elements_object = time_elements.TimeElementsWithFractionOfSecond(
+        precision=definitions.PRECISION_100_MICROSECONDS)
+    time_elements_object.CopyFromStringTuple(
+        time_elements_tuple=('2010', '8', '12', '20', '6', '31', '0.4671'))
+    self.assertEqual(
+        time_elements_object.fraction_of_second, decimal.Decimal('0.4671'))
+
+    with self.assertRaises(ValueError):
+      time_elements_object.CopyFromStringTuple(
+          time_elements_tuple=('2010', '8', '12', '20', '6', '31'))
+
+    with self.assertRaises(ValueError):
+      time_elements_object.CopyFromStringTuple(
+          time_elements_tuple=('2010', '8', '12', '20', '6', '31', '96'))
+
+  def testCopyToDateTimeString(self):
+    """Tests the CopyToDateTimeString function."""
+    time_elements_object = time_elements.TimeElementsWithFractionOfSecond(
+        fraction_of_second=decimal.Decimal('0.87'),
+        precision=definitions.PRECISION_10_MILLISECONDS,
+        time_elements_tuple=(2010, 8, 12, 20, 6, 31))
+
+    date_time_string = time_elements_object.CopyToDateTimeString()
+    self.assertEqual(date_time_string, '2010-08-12 20:06:31.87')
+
+    time_elements_object = time_elements.TimeElementsWithFractionOfSecond(
+        fraction_of_second=decimal.Decimal('0.874'),
+        precision=definitions.PRECISION_1_MILLISECOND,
+        time_elements_tuple=(2010, 8, 12, 20, 6, 31))
+
+    date_time_string = time_elements_object.CopyToDateTimeString()
+    self.assertEqual(date_time_string, '2010-08-12 20:06:31.874')
+
+    time_elements_object = time_elements.TimeElementsWithFractionOfSecond(
+        fraction_of_second=decimal.Decimal('0.8741'),
+        precision=definitions.PRECISION_100_MICROSECONDS,
+        time_elements_tuple=(2010, 8, 12, 20, 6, 31))
+
+    date_time_string = time_elements_object.CopyToDateTimeString()
+    self.assertEqual(date_time_string, '2010-08-12 20:06:31.8741')
+
+  def testNewFromDeltaAndDate(self):
+    """Tests the NewFromDeltaAndDate function."""
+    time_elements_object = time_elements.TimeElementsWithFractionOfSecond(
+        fraction_of_second=decimal.Decimal('0.87'),
+        is_delta=True,
+        precision=definitions.PRECISION_10_MILLISECONDS,
+        time_elements_tuple=(1, 0, 0, 20, 6, 31))
+
+    new_time_elements_object = time_elements_object.NewFromDeltaAndDate(
+        2009, 1, 12)
+    self.assertFalse(new_time_elements_object.is_delta)
+    self.assertEqual(new_time_elements_object.year, 2010)
+    self.assertEqual(new_time_elements_object.month, 1)
+    self.assertEqual(new_time_elements_object.day_of_month, 12)
+    self.assertEqual(
+        new_time_elements_object.fraction_of_second, decimal.Decimal('0.87'))
+
+    time_elements_object = time_elements.TimeElementsWithFractionOfSecond(
+        time_elements_tuple=(1, 0, 0, 20, 6, 31))
+
+    with self.assertRaises(ValueError):
+      time_elements_object.NewFromDeltaAndDate(2009, 1, 12)
+
+    time_elements_object = time_elements.TimeElementsWithFractionOfSecond()
+
+    with self.assertRaises(ValueError):
+      time_elements_object.NewFromDeltaAndDate(2009, 1, 12)
+
+  def testNewFromDeltaAndYear(self):
+    """Tests the NewFromDeltaAndYear function."""
+    time_elements_object = time_elements.TimeElementsWithFractionOfSecond(
+        fraction_of_second=decimal.Decimal('0.87'),
+        is_delta=True,
+        precision=definitions.PRECISION_10_MILLISECONDS,
+        time_elements_tuple=(1, 8, 12, 20, 6, 31))
+
+    new_time_elements_object = time_elements_object.NewFromDeltaAndYear(2009)
+    self.assertFalse(new_time_elements_object.is_delta)
+    self.assertEqual(new_time_elements_object.year, 2010)
+
+
 class TimeElementsInMillisecondsTest(unittest.TestCase):
   """Tests for the time elements in milliseconds."""
 
   # pylint: disable=protected-access
 
   def testInitialize(self):
     """Tests the initialization function."""
@@ -1217,19 +1456,19 @@
   def testInitialize(self):
     """Tests the initialization function."""
     time_elements_object = time_elements.TimeElements()
     self.assertIsNotNone(time_elements_object)
 
     expected_time_elements_tuple = (2010, 8, 12, 20, 6, 31)
     time_elements_object = time_elements.TimeElementsInMicroseconds(
-        time_elements_tuple=(2010, 8, 12, 20, 6, 31, 546))
+        time_elements_tuple=(2010, 8, 12, 20, 6, 31, 546875))
     self.assertIsNotNone(time_elements_object)
     self.assertEqual(
         time_elements_object._time_elements_tuple, expected_time_elements_tuple)
-    self.assertEqual(time_elements_object.microseconds, 546)
+    self.assertEqual(time_elements_object.microseconds, 546875)
 
     with self.assertRaises(ValueError):
       time_elements.TimeElementsInMicroseconds(
           time_elements_tuple=(2010, 13, 12, 20, 6, 31))
 
     with self.assertRaises(ValueError):
       time_elements.TimeElementsInMicroseconds(
@@ -1595,14 +1834,414 @@
 
     time_elements_object = time_elements.TimeElements(is_delta=True)
 
     new_time_elements_object = time_elements_object.NewFromDeltaAndYear(2009)
     self.assertIsNone(new_time_elements_object)
 
     time_elements_object = time_elements.TimeElements(is_delta=False)
+
+    with self.assertRaises(ValueError):
+      time_elements_object.NewFromDeltaAndYear(2009)
+
+
+class TimeElementsInNanosecondsTest(unittest.TestCase):
+  """Tests for the time elements in nanoseconds."""
+
+  # pylint: disable=protected-access
+
+  def testInitialize(self):
+    """Tests the initialization function."""
+    time_elements_object = time_elements.TimeElements()
+    self.assertIsNotNone(time_elements_object)
+
+    expected_time_elements_tuple = (2010, 8, 12, 20, 6, 31)
+    time_elements_object = time_elements.TimeElementsInNanoseconds(
+        time_elements_tuple=(2010, 8, 12, 20, 6, 31, 546875218))
+    self.assertIsNotNone(time_elements_object)
+    self.assertEqual(
+        time_elements_object._time_elements_tuple, expected_time_elements_tuple)
+    self.assertEqual(time_elements_object.nanoseconds, 546875218)
+
+    with self.assertRaises(ValueError):
+      time_elements.TimeElementsInNanoseconds(
+          time_elements_tuple=(2010, 13, 12, 20, 6, 31))
+
+    with self.assertRaises(ValueError):
+      time_elements.TimeElementsInNanoseconds(
+          time_elements_tuple=(2010, 13, 12, 20, 6, 31, 1001))
+
+  def testGetNormalizedTimestamp(self):
+    """Tests the _GetNormalizedTimestamp function."""
+    time_elements_object = time_elements.TimeElementsInNanoseconds(
+        time_elements_tuple=(2010, 8, 12, 20, 6, 31, 429876301))
+
+    normalized_timestamp = time_elements_object._GetNormalizedTimestamp()
+    self.assertEqual(
+        normalized_timestamp, decimal.Decimal('1281643591.429876301'))
+
+    time_elements_object = time_elements.TimeElementsInNanoseconds(
+        time_elements_tuple=(2010, 8, 12, 20, 6, 31, 429876301),
+        time_zone_offset=60)
+
+    normalized_timestamp = time_elements_object._GetNormalizedTimestamp()
+    self.assertEqual(
+        normalized_timestamp, decimal.Decimal('1281639991.429876301'))
+
+    time_elements_object = time_elements.TimeElementsInNanoseconds(
+        time_elements_tuple=(2010, 8, 12, 20, 6, 31, 429876301))
+    time_elements_object.time_zone_offset = 60
+
+    normalized_timestamp = time_elements_object._GetNormalizedTimestamp()
+    self.assertEqual(
+        normalized_timestamp, decimal.Decimal('1281639991.429876301'))
+
+    time_elements_object = time_elements.TimeElementsInNanoseconds()
+
+    normalized_timestamp = time_elements_object._GetNormalizedTimestamp()
+    self.assertIsNone(normalized_timestamp)
+
+  # TODO: add tests for _CopyFromDateTimeValues
+
+  def testCopyFromDatetime(self):
+    """Tests the CopyFromDatetime function."""
+    time_elements_object = time_elements.TimeElementsInNanoseconds()
+
+    expected_time_elements_tuple = (2010, 8, 12, 21, 6, 31)
+    expected_number_of_seconds = 1281647191
+
+    # Note that datetime has microsecond precision.
+    datetime_object = datetime.datetime(2010, 8, 12, 21, 6, 31, 546875)
+    time_elements_object.CopyFromDatetime(datetime_object)
+    self.assertEqual(
+        time_elements_object._time_elements_tuple, expected_time_elements_tuple)
+    self.assertEqual(
+        time_elements_object._number_of_seconds, expected_number_of_seconds)
+    self.assertEqual(time_elements_object.nanoseconds, 546875000)
+    self.assertTrue(time_elements_object.is_local_time)
+
+    expected_time_elements_tuple = (2010, 8, 12, 21, 6, 31)
+    expected_number_of_seconds = 1281647191
+
+    # Note that datetime has microsecond precision.
+    datetime_object = datetime.datetime(
+        2010, 8, 12, 21, 6, 31, 546875, tzinfo=datetime.timezone.utc)
+    time_elements_object.CopyFromDatetime(datetime_object)
+    self.assertEqual(
+        time_elements_object._time_elements_tuple, expected_time_elements_tuple)
+    self.assertEqual(
+        time_elements_object._number_of_seconds, expected_number_of_seconds)
+    self.assertEqual(time_elements_object.nanoseconds, 546875000)
+    self.assertFalse(time_elements_object.is_local_time)
+
+  def testCopyFromDateTimeString(self):
+    """Tests the CopyFromDateTimeString function."""
+    time_elements_object = time_elements.TimeElementsInNanoseconds()
+
+    expected_time_elements_tuple = (2010, 8, 12, 0, 0, 0)
+    time_elements_object.CopyFromDateTimeString('2010-08-12')
+    self.assertEqual(
+        time_elements_object._time_elements_tuple, expected_time_elements_tuple)
+    self.assertEqual(time_elements_object._number_of_seconds, 1281571200)
+    self.assertEqual(time_elements_object.nanoseconds, 0)
+    self.assertEqual(time_elements_object._time_zone_offset, None)
+
+    expected_time_elements_tuple = (2010, 8, 12, 21, 6, 31)
+    time_elements_object.CopyFromDateTimeString('2010-08-12 21:06:31')
+    self.assertEqual(
+        time_elements_object._time_elements_tuple, expected_time_elements_tuple)
+    self.assertEqual(time_elements_object._number_of_seconds, 1281647191)
+    self.assertEqual(time_elements_object.nanoseconds, 0)
+    self.assertEqual(time_elements_object._time_zone_offset, None)
+
+    expected_time_elements_tuple = (2010, 8, 12, 21, 6, 31)
+    time_elements_object.CopyFromDateTimeString('2010-08-12 21:06:31.546875218')
+    self.assertEqual(
+        time_elements_object._time_elements_tuple, expected_time_elements_tuple)
+    self.assertEqual(time_elements_object._number_of_seconds, 1281647191)
+    self.assertEqual(time_elements_object.nanoseconds, 546875218)
+    self.assertEqual(time_elements_object._time_zone_offset, None)
+
+    expected_time_elements_tuple = (2010, 8, 12, 21, 6, 31)
+    time_elements_object.CopyFromDateTimeString(
+        '2010-08-12 21:06:31.546875218-01:00')
+    self.assertEqual(
+        time_elements_object._time_elements_tuple, expected_time_elements_tuple)
+    self.assertEqual(time_elements_object._number_of_seconds, 1281647191)
+    self.assertEqual(time_elements_object.nanoseconds, 546875218)
+    self.assertEqual(time_elements_object._time_zone_offset, -60)
+
+    expected_time_elements_tuple = (2010, 8, 12, 21, 6, 31)
+    time_elements_object.CopyFromDateTimeString(
+        '2010-08-12 21:06:31.546875218+01:00')
+    self.assertEqual(
+        time_elements_object._time_elements_tuple, expected_time_elements_tuple)
+    self.assertEqual(time_elements_object._number_of_seconds, 1281647191)
+    self.assertEqual(time_elements_object.nanoseconds, 546875218)
+    self.assertEqual(time_elements_object._time_zone_offset, 60)
+
+    expected_time_elements_tuple = (1601, 1, 2, 0, 0, 0)
+    time_elements_object.CopyFromDateTimeString('1601-01-02 00:00:00')
+    self.assertEqual(
+        time_elements_object._time_elements_tuple, expected_time_elements_tuple)
+    self.assertEqual(time_elements_object._number_of_seconds, -11644387200)
+    self.assertEqual(time_elements_object.nanoseconds, 0)
+    self.assertEqual(time_elements_object._time_zone_offset, None)
+
+  def testCopyFromStringISO8601(self):
+    """Tests the CopyFromStringISO8601 function."""
+    time_elements_object = time_elements.TimeElementsInNanoseconds()
+
+    expected_time_elements_tuple = (2010, 8, 12, 0, 0, 0)
+    time_elements_object.CopyFromStringISO8601('2010-08-12')
+    self.assertEqual(
+        time_elements_object._time_elements_tuple, expected_time_elements_tuple)
+    self.assertEqual(time_elements_object._number_of_seconds, 1281571200)
+    self.assertEqual(time_elements_object.nanoseconds, 0)
+    self.assertEqual(time_elements_object._time_zone_offset, None)
+
+    expected_time_elements_tuple = (2010, 8, 12, 21, 6, 31)
+    time_elements_object.CopyFromStringISO8601('2010-08-12T21:06:31')
+    self.assertEqual(
+        time_elements_object._time_elements_tuple, expected_time_elements_tuple)
+    self.assertEqual(time_elements_object._number_of_seconds, 1281647191)
+    self.assertEqual(time_elements_object.nanoseconds, 0)
+    self.assertEqual(time_elements_object._time_zone_offset, None)
+
+    expected_time_elements_tuple = (2010, 8, 12, 21, 6, 31)
+    time_elements_object.CopyFromStringISO8601('2010-08-12T21:06:31+00:00')
+    self.assertEqual(
+        time_elements_object._time_elements_tuple, expected_time_elements_tuple)
+    self.assertEqual(time_elements_object._number_of_seconds, 1281647191)
+    self.assertEqual(time_elements_object.nanoseconds, 0)
+    self.assertEqual(time_elements_object._time_zone_offset, 0)
+
+    expected_time_elements_tuple = (2010, 8, 12, 21, 6, 31)
+    time_elements_object.CopyFromStringISO8601('2010-08-12T21:06:31.5')
+    self.assertEqual(
+        time_elements_object._time_elements_tuple, expected_time_elements_tuple)
+    self.assertEqual(time_elements_object._number_of_seconds, 1281647191)
+    self.assertEqual(time_elements_object.nanoseconds, 500000000)
+    self.assertEqual(time_elements_object._time_zone_offset, None)
+
+    expected_time_elements_tuple = (2010, 8, 12, 21, 6, 31)
+    time_elements_object.CopyFromStringISO8601('2010-08-12T21:06:31.546875218')
+    self.assertEqual(
+        time_elements_object._time_elements_tuple, expected_time_elements_tuple)
+    self.assertEqual(time_elements_object._number_of_seconds, 1281647191)
+    self.assertEqual(time_elements_object.nanoseconds, 546875218)
+    self.assertEqual(time_elements_object._time_zone_offset, None)
+
+    expected_time_elements_tuple = (2010, 8, 12, 21, 6, 31)
+    time_elements_object.CopyFromStringISO8601('2010-08-12T21:06:31,546875218')
+    self.assertEqual(
+        time_elements_object._time_elements_tuple, expected_time_elements_tuple)
+    self.assertEqual(time_elements_object._number_of_seconds, 1281647191)
+    self.assertEqual(time_elements_object.nanoseconds, 546875218)
+    self.assertEqual(time_elements_object._time_zone_offset, None)
+
+    expected_time_elements_tuple = (2010, 8, 12, 21, 6, 31)
+    time_elements_object.CopyFromStringISO8601(
+        '2010-08-12T21:06:31.546875218-01:00')
+    self.assertEqual(
+        time_elements_object._time_elements_tuple, expected_time_elements_tuple)
+    self.assertEqual(time_elements_object._number_of_seconds, 1281647191)
+    self.assertEqual(time_elements_object.nanoseconds, 546875218)
+    self.assertEqual(time_elements_object._time_zone_offset, -60)
+
+    expected_time_elements_tuple = (2010, 8, 12, 21, 6, 31)
+    time_elements_object.CopyFromStringISO8601(
+        '2010-08-12T21:06:31.546875218+01:00')
+    self.assertEqual(
+        time_elements_object._time_elements_tuple, expected_time_elements_tuple)
+    self.assertEqual(time_elements_object._number_of_seconds, 1281647191)
+    self.assertEqual(time_elements_object.nanoseconds, 546875218)
+    self.assertEqual(time_elements_object._time_zone_offset, 60)
+
+    expected_time_elements_tuple = (2012, 3, 5, 20, 40, 0)
+    time_elements_object.CopyFromStringISO8601(
+        '2012-03-05T20:40:00.0000000+00:00')
+    self.assertEqual(
+        time_elements_object._time_elements_tuple, expected_time_elements_tuple)
+    self.assertEqual(time_elements_object._number_of_seconds, 1330980000)
+    self.assertEqual(time_elements_object.nanoseconds, 0)
+    self.assertEqual(time_elements_object._time_zone_offset, 0)
+
+    with self.assertRaises(ValueError):
+      time_elements_object.CopyFromStringISO8601(None)
+
+    with self.assertRaises(ValueError):
+      time_elements_object.CopyFromStringISO8601(
+          '2010-08-12 21:06:31.546875218+01:00')
+
+    # Valid ISO 8601 notations currently not supported.
+    with self.assertRaises(ValueError):
+      time_elements_object.CopyFromStringISO8601('2016-W33')
+
+    with self.assertRaises(ValueError):
+      time_elements_object.CopyFromStringISO8601('2016-W33-3')
+
+    with self.assertRaises(ValueError):
+      time_elements_object.CopyFromStringISO8601('--08-17')
+
+    with self.assertRaises(ValueError):
+      time_elements_object.CopyFromStringISO8601('2016-230')
+
+  def testCopyFromStringTuple(self):
+    """Tests the CopyFromStringTuple function."""
+    time_elements_object = time_elements.TimeElementsInNanoseconds()
+
+    expected_time_elements_tuple = (2010, 8, 12, 20, 6, 31)
+    time_elements_object.CopyFromStringTuple(
+        time_elements_tuple=('2010', '8', '12', '20', '6', '31', '546'))
+    self.assertIsNotNone(time_elements_object)
+    self.assertEqual(
+        time_elements_object._time_elements_tuple, expected_time_elements_tuple)
+    self.assertEqual(time_elements_object.nanoseconds, 546)
+
+    with self.assertRaises(ValueError):
+      time_elements_object.CopyFromStringTuple(
+          time_elements_tuple=('2010', '8', '12', '20', '6', '31'))
+
+    with self.assertRaises(ValueError):
+      time_elements_object.CopyFromStringTuple(
+          time_elements_tuple=('2010', '8', '12', '20', '6', '31', '9S'))
+
+  def testCopyToDateTimeString(self):
+    """Tests the CopyToDateTimeString function."""
+    time_elements_object = time_elements.TimeElementsInNanoseconds(
+        time_elements_tuple=(2010, 8, 12, 20, 6, 31, 429876301))
+
+    date_time_string = time_elements_object.CopyToDateTimeString()
+    self.assertEqual(date_time_string, '2010-08-12 20:06:31.429876301')
+
+    time_elements_object = time_elements.TimeElementsInNanoseconds()
+
+    date_time_string = time_elements_object.CopyToDateTimeString()
+    self.assertIsNone(date_time_string)
+
+  def testCopyToDateTimeStringISO8601(self):
+    """Tests the CopyToDateTimeStringISO8601 function."""
+    time_elements_object = time_elements.TimeElementsInNanoseconds(
+        time_elements_tuple=(2010, 8, 12, 20, 6, 31, 429876301))
+
+    date_time_string = time_elements_object.CopyToDateTimeStringISO8601()
+    self.assertEqual(date_time_string, '2010-08-12T20:06:31.429876301+00:00')
+
+  def testCopyToPosixTimestamp(self):
+    """Tests the CopyToPosixTimestamp function."""
+    time_elements_object = time_elements.TimeElementsInNanoseconds(
+        time_elements_tuple=(2010, 8, 12, 20, 6, 31, 429876301))
+
+    posix_timestamp = time_elements_object.CopyToPosixTimestamp()
+    self.assertEqual(posix_timestamp, 1281643591)
+
+    time_elements_object = time_elements.TimeElements()
+
+    posix_timestamp = time_elements_object.CopyToPosixTimestamp()
+    self.assertIsNone(posix_timestamp)
+
+  def testCopyToPosixTimestampWithFractionOfSecond(self):
+    """Tests the CopyToPosixTimestampWithFractionOfSecond function."""
+    time_elements_object = time_elements.TimeElementsInNanoseconds(
+        time_elements_tuple=(2010, 8, 12, 20, 6, 31, 429876301))
+
+    posix_timestamp, fraction_of_second = (
+        time_elements_object.CopyToPosixTimestampWithFractionOfSecond())
+    self.assertEqual(posix_timestamp, 1281643591)
+    self.assertEqual(fraction_of_second, 429876301)
+
+    time_elements_object = time_elements.TimeElements()
+
+    posix_timestamp, fraction_of_second = (
+        time_elements_object.CopyToPosixTimestampWithFractionOfSecond())
+    self.assertIsNone(posix_timestamp)
+    self.assertIsNone(fraction_of_second)
+
+  def testGetDate(self):
+    """Tests the GetDate function."""
+    time_elements_object = time_elements.TimeElementsInNanoseconds(
+        time_elements_tuple=(2010, 8, 12, 20, 6, 31, 429876301))
+
+    date_tuple = time_elements_object.GetDate()
+    self.assertEqual(date_tuple, (2010, 8, 12))
+
+    time_elements_object = time_elements.TimeElementsInNanoseconds()
+
+    date_tuple = time_elements_object.GetDate()
+    self.assertEqual(date_tuple, (None, None, None))
+
+  def testGetDateWithTimeOfDay(self):
+    """Tests the GetDateWithTimeOfDay function."""
+    time_elements_object = time_elements.TimeElementsInNanoseconds(
+        time_elements_tuple=(2010, 8, 12, 20, 6, 31, 429876301))
+
+    date_with_time_of_day_tuple = time_elements_object.GetDateWithTimeOfDay()
+    self.assertEqual(date_with_time_of_day_tuple, (2010, 8, 12, 20, 6, 31))
+
+    time_elements_object = time_elements.TimeElementsInNanoseconds()
+
+    date_with_time_of_day_tuple = time_elements_object.GetDateWithTimeOfDay()
+    self.assertEqual(
+        date_with_time_of_day_tuple, (None, None, None, None, None, None))
+
+  def testGetTimeOfDay(self):
+    """Tests the GetTimeOfDay function."""
+    time_elements_object = time_elements.TimeElementsInNanoseconds(
+        time_elements_tuple=(2010, 8, 12, 20, 6, 31, 429876301))
+
+    time_of_day_tuple = time_elements_object.GetTimeOfDay()
+    self.assertEqual(time_of_day_tuple, (20, 6, 31))
+
+    time_elements_object = time_elements.TimeElementsInNanoseconds()
+
+    time_of_day_tuple = time_elements_object.GetTimeOfDay()
+    self.assertEqual(time_of_day_tuple, (None, None, None))
+
+  def testNewFromDeltaAndDate(self):
+    """Tests the NewFromDeltaAndDate function."""
+    time_elements_object = time_elements.TimeElementsInNanoseconds(
+        is_delta=True, time_elements_tuple=(1, 0, 0, 20, 6, 31, 429876301))
+
+    new_time_elements_object = time_elements_object.NewFromDeltaAndDate(
+        2009, 1, 12)
+    self.assertIsNotNone(new_time_elements_object)
+    self.assertFalse(new_time_elements_object.is_delta)
+    self.assertEqual(new_time_elements_object.year, 2010)
+    self.assertEqual(new_time_elements_object.month, 1)
+    self.assertEqual(new_time_elements_object.day_of_month, 12)
+    self.assertEqual(new_time_elements_object.nanoseconds, 429876301)
+
+    time_elements_object = time_elements.TimeElements(is_delta=True)
+
+    new_time_elements_object = time_elements_object.NewFromDeltaAndDate(
+        2009, 1, 12)
+    self.assertIsNone(new_time_elements_object)
+
+    time_elements_object = time_elements.TimeElements(is_delta=False)
+
+    with self.assertRaises(ValueError):
+      time_elements_object.NewFromDeltaAndDate(2009, 1, 12)
+
+  def testNewFromDeltaAndYear(self):
+    """Tests the NewFromDeltaAndYear function."""
+    time_elements_object = time_elements.TimeElementsInNanoseconds(
+        is_delta=True, time_elements_tuple=(1, 8, 12, 20, 6, 31, 429876301))
+
+    new_time_elements_object = time_elements_object.NewFromDeltaAndYear(2009)
+    self.assertIsNotNone(new_time_elements_object)
+    self.assertFalse(new_time_elements_object.is_delta)
+    self.assertEqual(new_time_elements_object.year, 2010)
+    self.assertEqual(new_time_elements_object.nanoseconds, 429876301)
+
+    time_elements_object = time_elements.TimeElements(is_delta=True)
+
+    new_time_elements_object = time_elements_object.NewFromDeltaAndYear(2009)
+    self.assertIsNone(new_time_elements_object)
+
+    time_elements_object = time_elements.TimeElements(is_delta=False)
 
     with self.assertRaises(ValueError):
       time_elements_object.NewFromDeltaAndYear(2009)
 
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `dfdatetime-20240330/tests/uuid_time.py` & `dfdatetime-20240504/tests/uuid_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/tests/webkit_time.py` & `dfdatetime-20240504/tests/webkit_time.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/tox.ini` & `dfdatetime-20240504/tox.ini`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/utils/dependencies.py` & `dfdatetime-20240504/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `dfdatetime-20240330/utils/update_release.sh` & `dfdatetime-20240504/utils/update_release.sh`

 * *Files identical despite different names*

