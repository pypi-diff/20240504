# Comparing `tmp/herbie-data-2024.3.1.tar.gz` & `tmp/herbie_data-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "herbie-data-2024.3.1.tar", last modified: Tue Mar 26 22:49:16 2024, max compression
+gzip compressed data, was "herbie_data-2024.5.0.tar", last modified: Sat May  4 04:49:16 2024, max compression
```

## Comparing `herbie-data-2024.3.1.tar` & `herbie_data-2024.5.0.tar`

### file list

```diff
@@ -1,68 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:49:16.272246 herbie-data-2024.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/HOW-TO-RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (127)     9399 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/Herbie.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14531 2024-03-26 22:49:16.272246 herbie-data-2024.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11022 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/environment-dev.yml
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/environment-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:49:16.264245 herbie-data-2024.3.1/herbie/
--rw-r--r--   0 runner    (1001) docker     (127)     8966 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/herbie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-26 22:49:15.000000 herbie-data-2024.3.1/herbie/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    17621 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/herbie/accessors.py
--rw-r--r--   0 runner    (1001) docker     (127)    47107 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/herbie/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10207 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/herbie/fast.py
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/herbie/help.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/herbie/hrrr_zarr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/herbie/latest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/herbie/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:49:16.268246 herbie-data-2024.3.1/herbie/models/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/herbie/models/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/herbie/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/herbie/models/ecmwf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/herbie/models/gefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/herbie/models/gfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/herbie/models/hafs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/herbie/models/hrdps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/herbie/models/hrrr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/herbie/models/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/herbie/models/nam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/herbie/models/navgem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/herbie/models/nbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/herbie/models/nexrad.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/herbie/models/nogaps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/herbie/models/rap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/herbie/models/rrfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/herbie/models/rtma.py
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/herbie/models/urma.py
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/herbie/wgrib2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:49:16.272246 herbie-data-2024.3.1/herbie_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14531 2024-03-26 22:49:16.000000 herbie-data-2024.3.1/herbie_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-26 22:49:16.000000 herbie-data-2024.3.1/herbie_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 22:49:16.000000 herbie-data-2024.3.1/herbie_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-26 22:49:16.000000 herbie-data-2024.3.1/herbie_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-26 22:49:16.000000 herbie-data-2024.3.1/herbie_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 22:49:16.272246 herbie-data-2024.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/test.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:49:16.272246 herbie-data-2024.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/tests/test_accessors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/tests/test_ecmwf.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/tests/test_fast.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/tests/test_first.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/tests/test_gefs.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/tests/test_gfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/tests/test_hrrr.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/tests/test_rap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-03-26 22:49:04.000000 herbie-data-2024.3.1/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:49:16.235300 herbie_data-2024.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/HOW-TO-RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14614 2024-05-04 04:49:16.235300 herbie_data-2024.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11037 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/environment-dev.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/environment-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:49:16.227300 herbie_data-2024.5.0/herbie/
+-rw-r--r--   0 runner    (1001) docker     (127)     9297 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/herbie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-04 04:49:15.000000 herbie_data-2024.5.0/herbie/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28278 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/herbie/accessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46708 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/herbie/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9890 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/herbie/fast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/herbie/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/herbie/hrrr_zarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/herbie/latest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/herbie/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:49:16.231300 herbie_data-2024.5.0/herbie/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/herbie/models/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/herbie/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/herbie/models/ecmwf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/herbie/models/gdps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/herbie/models/gefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/herbie/models/gfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/herbie/models/hafs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/herbie/models/hrdps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/herbie/models/hrrr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/herbie/models/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/herbie/models/nam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/herbie/models/navgem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/herbie/models/nbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/herbie/models/nexrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/herbie/models/nogaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/herbie/models/rap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/herbie/models/rdps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/herbie/models/rrfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/herbie/models/rtma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/herbie/models/urma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/herbie/wgrib2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:49:16.235300 herbie_data-2024.5.0/herbie_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14614 2024-05-04 04:49:15.000000 herbie_data-2024.5.0/herbie_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-04 04:49:16.000000 herbie_data-2024.5.0/herbie_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 04:49:15.000000 herbie_data-2024.5.0/herbie_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-04 04:49:15.000000 herbie_data-2024.5.0/herbie_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-04 04:49:15.000000 herbie_data-2024.5.0/herbie_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 04:49:16.235300 herbie_data-2024.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:49:16.235300 herbie_data-2024.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/tests/test_accessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/tests/test_ecmwf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/tests/test_fast.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/tests/test_first.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/tests/test_gefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/tests/test_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/tests/test_hrrr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/tests/test_pick_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/tests/test_rap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-04 04:49:06.000000 herbie_data-2024.5.0/tests/util.py
```

### Comparing `herbie-data-2024.3.1/.readthedocs.yml` & `herbie_data-2024.5.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `herbie-data-2024.3.1/CITATION.cff` & `herbie_data-2024.5.0/CITATION.cff`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 message: "If you use this software, please cite it as below."
 authors:
   - family-names: Blaylock
     given-names: Brian K.
     email: blaylockbk@gmail.com
     orcid: "https://orcid.org/0000-0003-2133-9313"
 title: "Herbie: Retrieve Numerical Weather Prediction Model Data"
-version: 2024.3.0
+version: 2024.5.0
 date-released: "2023-03-02"
 url: "https://herbie.readthedocs.io/"
 repository-code: "https://github.com/blaylockbk/Herbie"
 type: software
 keywords:
   - meteorology
   - weather
```

### Comparing `herbie-data-2024.3.1/HOW-TO-RELEASE.md` & `herbie_data-2024.5.0/HOW-TO-RELEASE.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ## Pre-step
 
 Update Herbie version number in
 
 - Update `./CITATION.cff` citation document
 - Update `./docs/_static/switcher.json` with a new item for the version you will soon create
-  - (You will need to go into the readthedocs.org dashboard and activate the version later.)
+  - (You will need to go into the _readthedocs.org_ dashboard and activate the version later.)
 - Make sure all leftover changes on main are committed that you want.
 - **Create a tag and release in GitHub**.
 
 > Note: The tag name should follow the pattern `YYYY.MM.0`
 >
 > - `YYYY` is the four-digit year the tag is created.
 > - `MM` is the month number the tag is created with _no leading zeros_ (PyPI doesn't care about leading zeros).
@@ -30,15 +30,17 @@
 1. The action uses the [build](https://github.com/pypa/build) tool to build my package following the steps from [here](https://towardsdatascience.com/how-to-package-your-python-code-df5a7739ab2e).
 1. The action then uses [pypa/gh-action-pypi-publish](https://github.com/pypa/gh-action-pypi-publish#specifying-a-different-username) to upload the package to PyPI
 
 After the action completes, confirm the file was uploaded to PyPI at <https://pypi.org/project/herbie-data/>.
 
 ## 🐍 Publish to Conda
 
-Updating the Conda package involves updating the herbie-data feedstock, specifically updating the version in the `meta.yml` file.
+Updating the Conda package involves updating the herbie-data feedstock, specifically updating the version in the `meta.yml` file. You should get a notification from the herbie-data feedstock repo saying that it detected a new version and open a pull request. If it looks good, merge the pull request.
+
+Manually updating the package on conda-forge involves the following steps:
 
 1. Fork the [herbie-data Conda feedstock](https://github.com/conda-forge/herbie-data-feedstock/pull/1/checks?check_run_id=11936300099)
 1. Follow the instructions in the README to update the build
    - Update version
    - Update sha256 has for the `herbie-data-{version}.tar.gz` file (found on PyPI) in the "Download files" tab.
    - Set build to 0 for releasing a new version.
 1. Create pull request.
```

### Comparing `herbie-data-2024.3.1/LICENSE` & `herbie_data-2024.5.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019-2022 Brian K. Blaylock
+Copyright (c) 2019-2024 Brian K. Blaylock
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `herbie-data-2024.3.1/PKG-INFO` & `herbie_data-2024.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: herbie-data
-Version: 2024.3.1
+Version: 2024.5.0
 Summary: Download numerical weather prediction GRIB2 model data.
 Author-email: "Brian K. Blaylock" <blaylockbk@gmail.com>
 Maintainer-email: "Brian K. Blaylock" <blaylockbk@gmail.com>
 License: MIT License
         
-        Copyright (c) 2019-2022 Brian K. Blaylock
+        Copyright (c) 2019-2024 Brian K. Blaylock
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -43,25 +43,27 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cartopy
+Requires-Dist: cfgrib
 Requires-Dist: matplotlib
+Requires-Dist: metpy
 Requires-Dist: numpy
 Requires-Dist: pandas
-Requires-Dist: xarray
-Requires-Dist: cfgrib
-Requires-Dist: metpy
-Requires-Dist: cartopy
-Requires-Dist: toml
 Requires-Dist: pygrib
+Requires-Dist: scikit-learn
+Requires-Dist: toml
+Requires-Dist: xarray
 Provides-Extra: docs
 Requires-Dist: autodocsumm; extra == "docs"
+Requires-Dist: ipython; extra == "docs"
 Requires-Dist: linkify-it-py; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: nbconvert; extra == "docs"
 Requires-Dist: nbsphinx; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: pydata-sphinx-theme; extra == "docs"
 Requires-Dist: recommonmark; extra == "docs"
@@ -103,15 +105,17 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/herbie-data?label=pypi|downloads)
 
 
 <!-- (Badges) -->
 
 </div>
 
-**Herbie** is a python package that downloads recent and archived numerical weather prediction (NWP) model output from different cloud archive sources. **Its most popular capability is to download HRRR model data.** NWP data in GRIB2 format can be read with xarray+cfgrib. Much of this data is made available through the [NOAA Open Data Dissemination](https://www.noaa.gov/information-technology/open-data-dissemination) (NODD) Program (formerly the Big Data Program) which has made weather data more accessible than ever before.
+**Herbie** is a python package that downloads recent and archived numerical weather prediction (NWP) model output from different cloud archive sources. NWP data is distributed in GRIB2 format and can be read with xarray+cfgrib. 
+
+# 📓 [Herbie Documentation](https://herbie.readthedocs.io/)
 
 Herbie helps you discover, download, and read data from:
 
 - [High Resolution Rapid Refresh (HRRR)](https://herbie.readthedocs.io/en/latest/user_guide/_model_notebooks/hrrr.html) | [HRRR-Alaska](https://herbie.readthedocs.io/en/latest/user_guide/_model_notebooks/hrrrak.html)
 - [Rapid Refresh (RAP)](https://herbie.readthedocs.io/en/latest/user_guide/_model_notebooks/rap.html)
 - [Global Forecast System (GFS)](https://herbie.readthedocs.io/en/latest/user_guide/_model_notebooks/gfs.html)
 - [Global Ensemble Forecast System (GEFS)](https://herbie.readthedocs.io/en/latest/user_guide/_model_notebooks/gefs.html)
@@ -120,15 +124,16 @@
 - [North American Mesoscale Model (NAM)](https://github.com/blaylockbk/Herbie/blob/main/docs/user_guide/_model_notebooks/nam.ipynb)
 - [National Blend of Models (NBM)](https://herbie.readthedocs.io/en/latest/user_guide/_model_notebooks/nbm.html)
 - [Rapid Refresh Forecast System (RRFS)](https://herbie.readthedocs.io/en/latest/user_guide/_model_notebooks/rrfs.html) _prototype_
 - [Real-Time/Un-Restricted Mesoscale Analysis (RTMA/URMA)](https://herbie.readthedocs.io/en/latest/user_guide/_model_notebooks/rtma.html)
 - [Hurricane Analysis And Forecast System (HAFS)](https://herbie.readthedocs.io/en/latest/user_guide/_model_notebooks/hafs.html)
 - [High Resolution Deterministic Prediction System (HRDPS)](https://herbie.readthedocs.io/en/latest/user_guide/_model_notebooks/hrdps.html)
 
-# 📓 [Herbie Documentation](https://herbie.readthedocs.io/)
+Much of this data is made available through the [NOAA Open Data Dissemination](https://www.noaa.gov/information-technology/open-data-dissemination) (NODD) program (formerly the Big Data Program) which has made weather data more accessible than ever before.
+
 
 ## Installation
 
 The easiest way to instal Herbie and its dependencies is with [Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) from conda-forge.
 
 ```bash
 conda install -c conda-forge herbie-data
@@ -147,17 +152,16 @@
 
 # Activate the environment
 conda activate herbie
 ```
 
 Alternatively, Herbie is published on PyPI and you can install it with pip, _but_ it requires some dependencies that you will have to install yourself:
 
-- Python 3.8 to 3.11
+- Python 3.9+
 - cURL
-- [Cartopy](https://scitools.org.uk/cartopy/docs/latest/installing.html), which requires GEOS and Proj.
 - [cfgrib](https://github.com/ecmwf/cfgrib), which requires eccodes.
 - _Optional:_ wgrib2
 - _Optional:_ [Carpenter Workshop](https://github.com/blaylockbk/Carpenter_Workshop)
 
 When those are installed within your environment, _then_ you can install Herbie with pip.
 
 ```bash
@@ -219,14 +223,16 @@
 # Download a subset, like all fields at 500 mb
 H.download(":500 mb")
 
 # Read subset with xarray, like 2-m temperature.
 H.xarray("TMP:2 m")
 ```
 
+Herbie also provides some custom xarray accessors to help you get the grid projection or pick points from the grid nearest a latitude-longitude location.
+
 ## Data Sources
 
 Herbie downloads model data from the following sources, but can be extended to include others:
 
 - [NOMADS](https://nomads.ncep.noaa.gov/)
 - [NOAA Open Data Dissemination Program (NODD)](https://www.noaa.gov/information-technology/open-data-dissemination) partners (i.e., AWS, Google, Azure).
 - [ECMWF Open Data Forecasts](https://www.ecmwf.int/en/forecasts/datasets/open-data)
@@ -263,15 +269,15 @@
 
 **Thanks for using Herbie, and happy racing!**
 
 🏁 Brian
 
 |     |                                                                                                     |
 | :-: | --------------------------------------------------------------------------------------------------- |
-| 👨🏻‍💻  | [Contributing Guide/Disclaimer](https://herbie.readthedocs.io/en/stable/user_guide/disclaimer.html) |
+| 👨🏻‍💻  | [Contributing Guide/Disclaimer](https://herbie.readthedocs.io/en/stable/user_guide/housekeeping/disclaimer.html) |
 | 💬  | [GitHub Discussions](https://github.com/blaylockbk/Herbie/discussions)                              |
 | 🚑  | [GitHub Issues](https://github.com/blaylockbk/Herbie/issues)                                        |
 | 🌐  | [Personal Webpage](http://home.chpc.utah.edu/~u0553130/Brian_Blaylock/home.html)                    |
 | 🌐  | [University of Utah HRRR archive](http://hrrr.chpc.utah.edu/)                                       |
 
 <br>
```

### Comparing `herbie-data-2024.3.1/README.md` & `herbie_data-2024.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/herbie-data?label=pypi|downloads)
 
 
 <!-- (Badges) -->
 
 </div>
 
-**Herbie** is a python package that downloads recent and archived numerical weather prediction (NWP) model output from different cloud archive sources. **Its most popular capability is to download HRRR model data.** NWP data in GRIB2 format can be read with xarray+cfgrib. Much of this data is made available through the [NOAA Open Data Dissemination](https://www.noaa.gov/information-technology/open-data-dissemination) (NODD) Program (formerly the Big Data Program) which has made weather data more accessible than ever before.
+**Herbie** is a python package that downloads recent and archived numerical weather prediction (NWP) model output from different cloud archive sources. NWP data is distributed in GRIB2 format and can be read with xarray+cfgrib. 
+
+# 📓 [Herbie Documentation](https://herbie.readthedocs.io/)
 
 Herbie helps you discover, download, and read data from:
 
 - [High Resolution Rapid Refresh (HRRR)](https://herbie.readthedocs.io/en/latest/user_guide/_model_notebooks/hrrr.html) | [HRRR-Alaska](https://herbie.readthedocs.io/en/latest/user_guide/_model_notebooks/hrrrak.html)
 - [Rapid Refresh (RAP)](https://herbie.readthedocs.io/en/latest/user_guide/_model_notebooks/rap.html)
 - [Global Forecast System (GFS)](https://herbie.readthedocs.io/en/latest/user_guide/_model_notebooks/gfs.html)
 - [Global Ensemble Forecast System (GEFS)](https://herbie.readthedocs.io/en/latest/user_guide/_model_notebooks/gefs.html)
@@ -44,15 +46,16 @@
 - [North American Mesoscale Model (NAM)](https://github.com/blaylockbk/Herbie/blob/main/docs/user_guide/_model_notebooks/nam.ipynb)
 - [National Blend of Models (NBM)](https://herbie.readthedocs.io/en/latest/user_guide/_model_notebooks/nbm.html)
 - [Rapid Refresh Forecast System (RRFS)](https://herbie.readthedocs.io/en/latest/user_guide/_model_notebooks/rrfs.html) _prototype_
 - [Real-Time/Un-Restricted Mesoscale Analysis (RTMA/URMA)](https://herbie.readthedocs.io/en/latest/user_guide/_model_notebooks/rtma.html)
 - [Hurricane Analysis And Forecast System (HAFS)](https://herbie.readthedocs.io/en/latest/user_guide/_model_notebooks/hafs.html)
 - [High Resolution Deterministic Prediction System (HRDPS)](https://herbie.readthedocs.io/en/latest/user_guide/_model_notebooks/hrdps.html)
 
-# 📓 [Herbie Documentation](https://herbie.readthedocs.io/)
+Much of this data is made available through the [NOAA Open Data Dissemination](https://www.noaa.gov/information-technology/open-data-dissemination) (NODD) program (formerly the Big Data Program) which has made weather data more accessible than ever before.
+
 
 ## Installation
 
 The easiest way to instal Herbie and its dependencies is with [Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) from conda-forge.
 
 ```bash
 conda install -c conda-forge herbie-data
@@ -71,17 +74,16 @@
 
 # Activate the environment
 conda activate herbie
 ```
 
 Alternatively, Herbie is published on PyPI and you can install it with pip, _but_ it requires some dependencies that you will have to install yourself:
 
-- Python 3.8 to 3.11
+- Python 3.9+
 - cURL
-- [Cartopy](https://scitools.org.uk/cartopy/docs/latest/installing.html), which requires GEOS and Proj.
 - [cfgrib](https://github.com/ecmwf/cfgrib), which requires eccodes.
 - _Optional:_ wgrib2
 - _Optional:_ [Carpenter Workshop](https://github.com/blaylockbk/Carpenter_Workshop)
 
 When those are installed within your environment, _then_ you can install Herbie with pip.
 
 ```bash
@@ -143,14 +145,16 @@
 # Download a subset, like all fields at 500 mb
 H.download(":500 mb")
 
 # Read subset with xarray, like 2-m temperature.
 H.xarray("TMP:2 m")
 ```
 
+Herbie also provides some custom xarray accessors to help you get the grid projection or pick points from the grid nearest a latitude-longitude location.
+
 ## Data Sources
 
 Herbie downloads model data from the following sources, but can be extended to include others:
 
 - [NOMADS](https://nomads.ncep.noaa.gov/)
 - [NOAA Open Data Dissemination Program (NODD)](https://www.noaa.gov/information-technology/open-data-dissemination) partners (i.e., AWS, Google, Azure).
 - [ECMWF Open Data Forecasts](https://www.ecmwf.int/en/forecasts/datasets/open-data)
@@ -187,15 +191,15 @@
 
 **Thanks for using Herbie, and happy racing!**
 
 🏁 Brian
 
 |     |                                                                                                     |
 | :-: | --------------------------------------------------------------------------------------------------- |
-| 👨🏻‍💻  | [Contributing Guide/Disclaimer](https://herbie.readthedocs.io/en/stable/user_guide/disclaimer.html) |
+| 👨🏻‍💻  | [Contributing Guide/Disclaimer](https://herbie.readthedocs.io/en/stable/user_guide/housekeeping/disclaimer.html) |
 | 💬  | [GitHub Discussions](https://github.com/blaylockbk/Herbie/discussions)                              |
 | 🚑  | [GitHub Issues](https://github.com/blaylockbk/Herbie/issues)                                        |
 | 🌐  | [Personal Webpage](http://home.chpc.utah.edu/~u0553130/Brian_Blaylock/home.html)                    |
 | 🌐  | [University of Utah HRRR archive](http://hrrr.chpc.utah.edu/)                                       |
 
 <br>
```

### Comparing `herbie-data-2024.3.1/environment-dev.yml` & `herbie_data-2024.5.0/environment-dev.yml`

 * *Files 7% similar despite different names*

```diff
@@ -28,14 +28,15 @@
   - pandas>=2.0
   - pygrib>=2.1.4
   - pylint
   - pyproj>=3.6
   - requests>=2.31
   - s3fs
   - scipy
+  - scikit-learn
   - toml
   - xarray>=2023.7
   - zarr
 
   # ===================
   # Formatter & Testing
   # ===================
```

### Comparing `herbie-data-2024.3.1/environment.yml` & `herbie_data-2024.5.0/environment.yml`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,15 @@
   - numpy>=1.25
   - pandas>=2.0
   - pygrib>=2.1.4
   - pylint
   - pyproj>=3.6
   - requests>=2.31
   - s3fs
+  - scikit-learn
   - toml
   #- wgrib2 # ONLY AVAILABLE ON LINUX. Uncomment if you want this optional dependency.
   - jupyter
   - jupyterlab
   - xarray>=2023.7
   - zarr
```

### Comparing `herbie-data-2024.3.1/herbie/__init__.py` & `herbie_data-2024.5.0/herbie/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """
+Herbie is your model output download assistant with a mind of his own.
+
 ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██
   ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██
 ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██
   ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██
 
                 █ ██
                 █ ██ ┏━┓ ┏━┓            ┏━┓   ┏━┓
@@ -13,26 +15,32 @@
                 █ ██
                        🏁 Retrieve NWP Model Data 🏁
 
 ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██
   ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██
 ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██
   ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██  ██
+
+Herbie might look small on the outside, but he has a big heart on the
+inside and will get you to the finish line. Happy racing! 🏁
 """
 
 import os
 from pathlib import Path
 
 import toml
 
 from herbie.misc import ANSI
 
 __author__ = "Brian K. Blaylock"
 __meet_Herbie__ = "https://en.wikipedia.org/wiki/Herbie"
 __movie_clips__ = "https://youtube.com/playlist?list=PLrSOkJxBTv53gvwbw9pVlMm-1C2PUHJx7"
+__Herbie_wins__ = "https://www.youtube.com/watch?v=4XWufUZ1mxQ&t=189s"
+__documentation__ = "https://herbie.readthedocs.io/"
+
 
 try:
     ## TODO: Will the `_version.py` file *always* be present?
     ## TODO: What if the person doesn't do "pip install"
     from ._version import __version__, __version_tuple__
 except:
     __version__ = "unknown"
```

### Comparing `herbie-data-2024.3.1/herbie/accessors.py` & `herbie_data-2024.5.0/herbie/accessors.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,36 @@
 ## Brian Blaylock
 ## April 23, 2021
 
-"""
-==================================
-Herbie Extension: xarray accessors
-==================================
-
-Extend the xarray capabilities with a custom accessor.
-http://xarray.pydata.org/en/stable/internals.html#extending-xarray
-
-To use the herbie xarray accessor, do this...
+"""Herbie's xarray accessors.
 
-.. code-block:: python
+Other useful packages
 
-    H = Herbie('2021-01-01', model='hrrr')
-    ds = H.xarray('TMP:2 m')
-    ds.herbie.crs
-    ds.herbie.plot()
-
-# TODO: I like the idea in Salem to mask data by a geographic region
-# TODO: Maybe can use that in Herbie. https://github.com/fmaussion/salem
+- salem: mask data by a geographic region: https://github.com/fmaussion/salem
+- xoak: xarray nearest neighbor https://github.com/xarray-contrib/xoak
 """
 
 import functools
+import pickle
 import re
+import warnings
 from pathlib import Path
 
 import cartopy.crs as ccrs
-import metpy  # noqa: F401
+import metpy  # * Needed for metpy accessor  # noqa: F401
 import numpy as np
 import pandas as pd
 import pygrib
 import shapely
 import xarray as xr
 from pyproj import CRS
 from shapely.geometry import MultiPoint, Point, Polygon
+from sklearn.neighbors import BallTree
+
+import herbie
 
 _level_units = dict(
     adiabaticCondensation="adiabatic condensation",
     atmosphere="atmosphere",
     atmosphereSingleLayer="atmosphere single layer",
     boundaryLayerCloudLayer="boundary layer cloud layer",
     cloudBase="cloud base",
@@ -63,15 +55,15 @@
     sigma="sigma",
     sigmaLayer="sigmaLayer",
     surface="surface",
 )
 
 
 def add_proj_info(ds):
-    """Add projection info to a Dataset"""
+    """Add projection info to a Dataset."""
     match = re.search(r'"source": "(.*?)"', ds.history)
     FILE = Path(match.group(1))
 
     # Get CF grid projection information with pygrib and pyproj because
     # this is something cfgrib doesn't do (https://github.com/ecmwf/cfgrib/issues/251)
     # NOTE: Assumes the projection is the same for all variables
     with pygrib.open(str(FILE)) as grb:
@@ -140,17 +132,15 @@
 
         ds = ds.metpy.parse_cf(varname=variables)
         crs = ds.metpy_crs.item().to_cartopy()
         return crs
 
     @functools.cached_property
     def polygon(self):
-        """
-        Get a polygon of the domain boundary.
-        """
+        """Get a polygon of the domain boundary."""
         ds = self._obj
 
         LON = ds.longitude.data
         LAT = ds.latitude.data
 
         # Path of array outside border starting from the lower left corner
         # and going around the array counter-clockwise.
@@ -176,14 +166,281 @@
         transform = transform[~np.isinf(transform).any(axis=1)]
         x = transform[:, 0]
         y = transform[:, 1]
         domain_polygon = Polygon(zip(x, y))
 
         return domain_polygon, domain_polygon_latlon
 
+    def pick_points(
+        self,
+        points,
+        method="nearest",
+        *,
+        k=None,
+        max_distance=500,
+        use_cached_tree=True,
+        tree_name=None,
+        verbose=False,
+    ):
+        """Pick nearest neighbor grid values at selected  points.
+
+        Parameters
+        ----------
+        points : Pandas DataFrame
+            A DataFrame with columns 'latitude' and 'longitude'
+            representing the points to match to the model grid.
+        method : {'nearest', 'weighted'}
+            Method used to pick points.
+            - `nearest` : Gets grid value nearest the requested point.
+            - `weighted`: Gets four grid value nearest the requested
+                point and compute the inverse-distance-weighted mean.
+        k : None or int
+            If None and method is nearest, `k=1`.
+            If None and method is weighted, `k=4`.
+            Else, specify the number of neighbors to find.
+        max_distance : int or float
+            Maximum distance in kilometers allowed for nearest neighbor
+            search. Default is 500 km, which is very generous for any
+            model grid. This can help the case when a requested point
+            is off the grid.
+        use_cached_tree : {True, False, "replant"}
+            Controls if the BallTree object is caches for later use.
+            By "plant", I mean, "create a new BallTree object."
+            - `True` : Plant+save BallTree if it doesn't exist; load
+                saved BallTree if one exists.
+            - `False`: Plant the BallTree, even if one exists.
+            - `"replant"` : Plant a new BallTree and save a new pickle.
+        tree_name : str
+            If None, use the ds.model and domain size as the tree's name.
+            If ds.model does not exists, then the BallTree will not be
+            cached, unless you provide the tree_name.
+
+        Examples
+        --------
+        >>> H = Herbie("2024-03-28 00:00", model="hrrr")
+        >>> ds = H.xarray("TMP:[5,6,7,8,9][0,5]0 mb", remove_grib=False)
+        >>> points = pd.DataFrame(
+        ...     {
+        ...         "longitude": [-100, -105, -98.4],
+        ...         "latitude": [40, 29, 42.3],
+        ...         "stid": ["aa", "bb", "cc"],
+        ...     }
+        ... )
+
+        Pick value at the nearest neighbor point
+        >>> dsp = ds.herbie.pick_points(points, method="nearest")
+
+        Get the weighted mean of the four nearest neighbor points
+        >>> dsp = ds.herbie.pick_points(points, method="weighted")
+
+        A Dataset is returned of the original grid reduced to the
+        requested points, with the values from the `points` dataset
+        added as new coordinates.
+
+        A user can easily convert the result to a Pandas DataFrame
+        >>> dsp.to_dataframe()
+
+        If you want to select points by a station name, swap the
+        dimension.
+        >>> dsp = dsp.swap_dims({"point": "point_stid"})
+        """
+
+        def plant_tree(save_pickle=None):
+            """Grow a new BallTree object from seedling."""
+            timer = pd.Timestamp("now")
+            print("INFO: 🌱 Growing new BallTree...", end="")
+            tree = BallTree(np.deg2rad(df_grid), metric="haversine")
+            print(
+                f"🌳 BallTree grew in {(pd.Timestamp('now')-timer).total_seconds():.2} seconds."
+            )
+            if save_pickle:
+                try:
+                    Path(save_pickle).parent.mkdir(parents=True, exist_ok=True)
+                    with open(save_pickle, "wb") as f:
+                        pickle.dump(tree, f)
+                    print(f"INFO: Saved BallTree to {save_pickle}")
+                except OSError:
+                    print(f"ERROR: Could not save BallTree to {save_pickle}.")
+            return tree
+
+        ds = self._obj
+
+        # ---------------------
+        # Validate points input
+        if ("latitude" not in points) and ("longitude" not in points):
+            raise ValueError(
+                "`points` DataFrame must have columns 'latitude' and 'longitude'"
+            )
+
+        if not all(points.latitude.between(-90, 90, inclusive="both")):
+            raise ValueError("All latitude points must be [-90,90]")
+
+        if not all(points.longitude.between(0, 360, inclusive="both")):
+            if not all(points.longitude.between(-180, 180, inclusive="both")):
+                raise ValueError("All longitude points must be [-180,180] or [0,360]")
+
+        # ---------------------
+        # Validate method input
+        _method = set(["nearest", "weighted"])
+
+        if method == "nearest" and k is None:
+            # Get the value at the nearest grid point using BallTree
+            k = 1
+        elif method == "weighted" and k is None:
+            # Compute the value of each variable from the inverse-
+            # weighted distance of the values of the four nearest
+            # neighbors.
+            k = 4
+        elif method in _method and isinstance(k, int):
+            # Get the k nearest neighbors and return the values (nearest)
+            # or compute the distance-weighted mean (weighted).
+            pass
+        else:
+            raise ValueError(
+                f"`method` must be one of {_method} and `k` must be an int or None."
+            )
+
+        # Only consider variables that have dimensions.
+        ds = ds[[i for i in ds if ds[i].dims != ()]]
+
+        if "latitude" in ds.dims and "longitude" in ds.dims:
+            # Rename dims to x and y
+            # This is needed for regular latitude-longitude grids like
+            # GFS and IFS model data.
+            ds = ds.rename_dims({"latitude": "y", "longitude": "x"})
+
+        # Get Dataset's lat/lon grid and coordinate indices as a DataFrame.
+        df_grid = (
+            ds[["latitude", "longitude"]]
+            .drop_vars([i for i, j in ds.coords.items() if not j.ndim])
+            .to_dataframe()
+        )
+
+        # ---------------
+        # BallTree object
+        # Plant, plant+Save, or load
+
+        if tree_name is None:
+            tree_name = getattr(ds, "model", "UNKNOWN")
+
+        if use_cached_tree and tree_name == "UNKNOWN":
+            use_cached_tree = False
+            print(
+                "WARNING: Herbie won't cache the BallTree because it\n"
+                "         doesn't know what to name it. Please specify\n"
+                "         `tree_name` to cache the tree for use later."
+            )
+
+        pkl_BallTree_file = (
+            herbie.config["default"]["save_dir"]
+            / "BallTree"
+            / f"{tree_name}_{ds.x.size}-{ds.y.size}.pkl"
+        )
+
+        if not use_cached_tree:
+            # Create a new BallTree. Do not save pickle.
+            tree = plant_tree(save_pickle=False)
+        elif use_cached_tree == "replant" or not pkl_BallTree_file.exists():
+            # Create a new BallTree and save pickle.
+            tree = plant_tree(save_pickle=pkl_BallTree_file)
+        elif use_cached_tree:
+            # Load BallTree from pickle.
+            with open(pkl_BallTree_file, "rb") as f:
+                tree = pickle.load(f)
+
+        # -------------------------------------
+        # Query points to find nearest neighbor
+        # Note: Order matters, and lat/long must be in radians.
+        # TODO: Maybe add option to use MultiProcessing here, to split
+        # TODO:   the Dataset into chunks; or maybe not needed because
+        # TODO:   the method is fast enough without the added complexity.
+        dist, ind = tree.query(np.deg2rad(points[["latitude", "longitude"]]), k=k)
+
+        # Convert distance to km by multiplying by the radius of the Earth
+        dist *= 6371
+
+        # Pick grid values for each value of k
+        k_points = []
+        df_grid = df_grid.reset_index()
+        for i in range(k):
+            a = points.copy()
+            a["point_grid_distance"] = dist[:, i]
+            a["grid_index"] = ind[:, i]
+
+            a = pd.concat(
+                [
+                    a,
+                    df_grid.iloc[a.grid_index]
+                    .add_suffix("_grid")
+                    .reset_index(drop=True),
+                ],
+                axis=1,
+            )
+            a.index.name = "point"
+
+            if max_distance:
+                flagged = a.loc[a.point_grid_distance > max_distance]
+                a = a.loc[a.point_grid_distance <= max_distance]
+                if len(flagged):
+                    print(
+                        f"WARNING: {len(flagged)} points removed for exceeding {max_distance=} km threshold."
+                    )
+                    print(f"{flagged}")
+                    print("")
+
+            # Get corresponding values from xarray
+            # https://docs.xarray.dev/en/stable/user-guide/indexing.html#more-advanced-indexing
+            ds_points = ds.sel(
+                x=a.x_grid.to_xarray(),
+                y=a.y_grid.to_xarray(),
+            )
+            ds_points.coords["point_grid_distance"] = a.point_grid_distance.to_xarray()
+            ds_points["point_grid_distance"].attrs["long_name"] = (
+                "Distance between requested point and nearest grid point."
+            )
+            ds_points["point_grid_distance"].attrs["units"] = "km"
+
+            for i in points.columns:
+                ds_points.coords[f"point_{i}"] = a[i].to_xarray()
+                ds_points[f"point_{i}"].attrs["long_name"] = f"Requested grid point {i}"
+
+            k_points.append(ds_points.drop_vars("point"))
+
+        if method == "nearest" and k == 1:
+            return k_points[0]
+
+        elif method == "nearest" and k > 1:
+            # New dimension k is the index of the n-th nearest neighbor
+            return xr.concat(k_points, dim="k")
+
+        elif method == "weighted":
+            # Compute the inverse-distance weighted mean for each
+            # variable from the four nearest points.
+            b = xr.concat(k_points, dim="k")
+
+            # Note: clipping accounts for the "divide by zero" case when
+            # the requested point is exactly the nearest grid point.
+            weights = (1 / b.point_grid_distance).clip(max=1e6)
+
+            # Compute weighted mean of variables
+            sum_of_weights = weights.sum(dim="k")
+            weighted_sum = (b * weights).sum(dim="k")
+
+            c = weighted_sum / sum_of_weights
+
+            # Include some coordinates that were dropped as a result of
+            # the line `weights.sum(dim='k')`.
+            c.coords["latitude"] = b.coords["latitude"]
+            c.coords["longitude"] = b.coords["longitude"]
+            c.coords["point_grid_distance"] = b.coords["point_grid_distance"]
+
+            return c
+        else:
+            raise ValueError("I didn't expect to be here.")
+
     def nearest_points(self, points, names=None, verbose=True):
         """
         Get the nearest latitude/longitude points from a xarray Dataset.
 
         - Stack Overflow: https://stackoverflow.com/questions/58758480/xarray-select-nearest-lat-lon-with-multi-dimension-coordinates
         - MetPy Details: https://unidata.github.io/MetPy/latest/tutorials/xarray_tutorial.html?highlight=assign_y_x
 
@@ -215,14 +472,22 @@
 
             TODO: Explore alternatives
             - Could Shapely nearest_points be used
             https://shapely.readthedocs.io/en/latest/manual.html#nearest-points
             - Or possibly scipy BallTree method.
 
         """
+        warnings.warn(
+            "The accessor `ds.herbie.nearest_points` is deprecated in "
+            "favor of the `ds.herbie.pick_points` which uses the "
+            "BallTree algorithm instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+
         ds = self._obj
 
         # Longitude and Latitude point DataFrame
         if isinstance(points, pd.DataFrame):
             point_df = points[["longitude", "latitude"]]
             if names is not None:
                 point_df.index = names
@@ -266,26 +531,26 @@
         # We want to index the dataset at a single point.
         # We can do this by transforming a lat/lon point to the grid location
         crs = ds.metpy_crs.item().to_cartopy()
 
         transformed_data = crs.transform_points(
             ccrs.PlateCarree(), point_df.longitude, point_df.latitude
         )
-        xs = transformed_data[:, 0]
-        ys = transformed_data[:, 1]
+
+        a = pd.DataFrame({"x": transformed_data[:, 0], "y": transformed_data[:, 1]})
+        a.index.name = "point"
 
         # Select the nearest points from the projection coordinates.
-        # TODO: Is there a better way?
-        # There doesn't seem to be a way to get just the points like this
-        # ds = ds.sel(x=xs, y=ys, method='nearest')
-        # because it gives a 2D array, and not a point-by-point index.
-        # Instead, I have too loop the ds.sel method
-        new_ds = xr.concat(
-            [ds.sel(x=xi, y=yi, method="nearest") for xi, yi in zip(xs, ys)],
-            dim="point",
+        # Get corresponding values from xarray
+        # https://docs.xarray.dev/en/stable/user-guide/indexing.html#more-advanced-indexing
+        #
+        new_ds = ds.sel(
+            x=a["x"].to_xarray(),
+            y=a["y"].to_xarray(),
+            method="nearest",
         )
 
         new_ds.coords["point"] = ("point", point_df.index.to_list())
         new_ds.coords["point_latitude"] = ("point", point_df.latitude)
         new_ds.coords["point_longitude"] = ("point", point_df.longitude)
 
         return new_ds
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `herbie-data-2024.3.1/herbie/core.py` & `herbie_data-2024.5.0/herbie/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,15 @@
-#!/usr/bin/env python3
-
-## Brian Blaylock
-## May 6, 2022
-
 """
+You are looking under Herbie's hood, his engine.
 
-===============================
-Herbie: Retrieve NWP Model Data
-===============================
-
-Herbie is your model output download assistant with a mind of his own!
-Herbie might look small on the outside, but he has a big heart on the
-inside and will get you to the
-`finish line <https://www.youtube.com/watch?v=4XWufUZ1mxQ&t=189s>`_.
-Happy racing! 🏁
-
-`📓 Documentation <https://herbie.readthedocs.io/>`_
-
-With Herbie's API, you can search and download GRIB2 model output files
-from different archive sources for the High-Resolution Rapid Refresh
-(HRRR) HRRR-Alaska, Rapid Refresh (RAP), Global Forecast System (GFS),
-and others.
-
-Herbie looks for GRIB2 model output data from NOMADS, NOAA's Big Data
-Project partners (Amazon Web Services, Google Cloud Platform, and
-Microsoft Azure), and the CHPC Pando archive at the University of Utah.
-
-Herbie supports subsetting of GRIB2 files by individual GRIB
-messages (i.e. variable and level) when the index (.idx) file exist and
-help you open them with xarray/cfgrib.
-
-Herbie is extendable to support other models. Simply create a template
-file in the ``herbie/models`` directory and make a pull-request.
-
-For more details, see https://herbie.readthedocs.io/user_guide/data_sources.html
-
-
-TODO: Rename 'searchString' to 'subset' (and rename subset function to??) - REJECTED, for now
-TODO: Rename 'fxx' to 'lead' and allow pandas-parsable timedelta string like "6H".
+TODO: Rename 'fxx' to 'step' and allow pandas-parsable timedelta string like "6h".
 TODO: add `idx_to_df()` and `df_to_idx()` methods.
 TODO: There are probably use cases for the `Path().suffixes` method
 """
+
 import functools
 import hashlib
 import itertools
 import json
 import logging
 import os
 import subprocess
@@ -59,25 +24,25 @@
 import pygrib
 import requests
 import xarray as xr
 from pyproj import CRS
 
 import herbie.models as model_templates
 from herbie import Path, config
-from herbie.help import _searchString_help
+from herbie.help import _search_help
 from herbie.misc import ANSI
 
 # NOTE: The config dict values are retrieved from __init__ and read
 # from the file ${HOME}/.config/herbie/config.toml
 # Path is imported from __init__ because it has my custom methods.
 
 try:
     # Load custom xarray accessors
     import herbie.accessors  # noqa: F401
-except:
+except Exception:
     warnings.warn(
         "herbie xarray accessors could not be imported."
         "Probably missing a dependency like MetPy."
         "If you want to use these functions, try"
         "`pip install metpy`"
     )
 
@@ -155,15 +120,15 @@
     Parameters
     ----------
     date : pandas-parsable datetime
         Model *initialization* datetime. If None, then must set
         ``valid_date``.
     valid_date : pandas-parsable datetime
         Model *valid* datetime. Must set when ``date`` is None.
-    fxx : int or pandas-parsable timedelta (e.g. "6H")
+    fxx : int or pandas-parsable timedelta (e.g. "6h")
         Forecast lead time *in hours*. Available lead times depend on
         the model type and model version.
     model : {'hrrr', 'hrrrak', 'rap', 'gfs', 'ecmwf', etc.}
         Model name as defined in the models template folder.
         CASE INSENSITIVE; e.g., "HRRR" is the same as "hrrr".
     product : {'sfc', 'prs', 'nat', 'subh', etc.}
         Output variable product file type. If not specified, will
@@ -216,15 +181,15 @@
         **kwargs,
     ):
         """Specify model output and find GRIB2 file at one of the sources."""
         self.fxx = fxx
 
         if isinstance(self.fxx, (str, pd.Timedelta)):
             # Convert pandas-parsable timedelta string to int in hours.
-            self.fxx = pd.to_timedelta(fxx).round("1H").total_seconds() / 60 / 60
+            self.fxx = pd.to_timedelta(fxx).round("1h").total_seconds() / 60 / 60
             self.fxx = int(self.fxx)
 
         if date:
             # User supplied `date`, which is the model initialization datetime.
             self.date = pd.to_datetime(date)
             self.valid_date = self.date + timedelta(hours=self.fxx)
         elif valid_date:
@@ -283,15 +248,15 @@
 
         # Specify the index file type. By default, Herbie assumes the
         # index file was created with wgrib2.
         # But for ecmwf files with index files created with eccodes
         # the index files are in a different style.
         self.IDX_STYLE = getattr(self, "IDX_STYLE", "wgrib2")
 
-        self.searchString_help = _searchString_help(self.IDX_STYLE)
+        self.search_help = _search_help(self.IDX_STYLE)
 
         # Check the user input
         self._validate()
 
         # Ok, now we are ready to look for the GRIB2 file at each of the remote sources.
         # self.grib is the first existing GRIB2 file discovered.
         # self.idx is the first existing index file discovered.
@@ -329,14 +294,18 @@
 
     def __str__(self):
         """When Herbie class object is printed, print all properties."""
         # * Keep this simple so it runs fast.
         msg = (f"║HERBIE╠ {self.model.upper()}:{self.product}",)
         return " ".join(msg)
 
+    def __bool__(self):
+        """Herbie evaluated True if the GRIB file exists."""
+        return bool(self.grib)
+
     def help(self):
         """Print help message if available."""
         if hasattr(self, "HELP"):
             HELP = self.HELP.strip().replace("\n", "\n│ ")
         else:
             HELP = "│"
         print("╭─ Herbie ────────────────────────────────")
@@ -369,15 +338,17 @@
         # Accept model alias
         if self.model.lower() == "alaska":
             self.model = "hrrrak"
 
         _models = {m for m in dir(model_templates) if not m.startswith("__")}
         _products = set(self.PRODUCTS)
 
-        assert self.date < datetime.utcnow(), "🔮 `date` cannot be in the future."
+        assert self.date < pd.Timestamp.utcnow().tz_localize(
+            None
+        ), "🔮 `date` cannot be in the future."
         assert self.model in _models, f"`model` must be one of {_models}"
         assert self.product in _products, f"`product` must be one of {_products}"
 
         if isinstance(self.IDX_SUFFIX, str):
             self.IDX_SUFFIX = [self.IDX_SUFFIX]
 
         if isinstance(self.priority, str):
@@ -395,15 +366,15 @@
                 if self.date < expired:
                     self.priority.remove("nomads")
 
     def _ping_pando(self):
         """Pinging the Pando server before downloading can prevent a bad handshake."""
         try:
             requests.head("https://pando-rgw01.chpc.utah.edu/")
-        except:
+        except Exception:
             print("🤝🏻⛔ Bad handshake with pando? Am I able to move on?")
             pass
 
     def _check_grib(self, url, min_content_length=10):
         """
         Check that the GRIB2 URL exist and is of useful length.
 
@@ -546,16 +517,25 @@
         return self.SOURCES[source].split("/")[-1]
 
     @property
     def get_localFileName(self):
         """Predict the local file name."""
         return self.LOCALFILE
 
-    def get_localFilePath(self, searchString=None):
+    def get_localFilePath(self, search=None, *, searchString=None):
         """Get full path to the local file."""
+        # TODO: Remove this eventually
+        if searchString is not None:
+            warnings.warn(
+                "The argument `searchString` was renamed `search`. Please update your scripts.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+            search = searchString
+
         # Predict the localFileName from the first model template SOURCE.
         localFilePath = (
             self.save_dir.expand()
             / self.model
             / f"{self.date:%Y%m%d}"
             / self.get_localFileName
         )
@@ -568,17 +548,17 @@
                     Path(self.SOURCES[i]).expand()
                     for i in self.SOURCES
                     if i.startswith("local") and Path(self.SOURCES[i]).expand().exists()
                 ),
                 localFilePath,
             )
 
-        if searchString is not None:
-            # Reassign the index DataFrame with the requested searchString
-            idx_df = self.inventory(searchString)
+        if search is not None:
+            # Reassign the index DataFrame with the requested search
+            idx_df = self.inventory(search)
 
             # ======================================
             # Make a unique filename for the subset
 
             # Get a list of all GRIB message numbers. We will use this
             # in the output file name as a unique identifier.
             all_grib_msg = "-".join([f"{i:g}" for i in idx_df.index])
@@ -730,27 +710,27 @@
             df = df.reset_index()
             df["start_byte"] = df["_offset"]
             df["end_byte"] = df["_offset"] + df["_length"]
             df["range"] = df.start_byte.astype(str) + "-" + df.end_byte.astype(str)
             df["reference_time"] = pd.to_datetime(
                 df.date + df.time, format="%Y%m%d%H%M"
             )
-            df["step"] = pd.to_timedelta(df.step.astype(int), unit="H")
+            df["step"] = pd.to_timedelta(df.step.astype(int), unit="h")
             df["valid_time"] = df.reference_time + df.step
 
             df = df.reindex(
                 columns=[
                     "grib_message",
                     "start_byte",
                     "end_byte",
                     "range",
                     "reference_time",
                     "valid_time",
                     "step",
-                    # ---- Used for searchString ------------------------------
+                    # ---- Used for search ------------------------------
                     "param",  # parameter field (variable)
                     "levelist",  # level
                     "levtype",  # sfc=surface, pl=pressure level, pt=potential vorticity
                     "number",  # model number (used in ensemble products)
                     "domain",  # g=global
                     "expver",  # experiment version
                     "class",  # classification (od=routing operations, rd=research, )
@@ -777,71 +757,72 @@
             product=self.product,
             lead_time=self.fxx,
             datetime=self.date,
         )
 
         return df
 
-    # TODO : Remove this in a future Herbie version
-    def read_idx(self, searchString=None):
-        warnings.warn(
-            "The `read_idx` method has been renamed `inventory`.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        return self.inventory(searchString=None)
-
-    def inventory(self, searchString=None, verbose=None):
+    def inventory(self, search=None, *, searchString=None, verbose=None):
         """
         Inspect the GRIB2 file contents by reading the index file.
 
         This reads index files created with the wgrib2 utility.
 
         Parameters
         ----------
-        searchString : str
-            Filter dataframe by a searchString regular expression.
+        search : str
+            Filter dataframe by a search regular expression.
             Searches for strings in the index file lines, specifically
             the variable, level, and forecast_time columns.
-            Execute ``_searchString_help()`` for examples of a good
-            searchString.
+            Execute ``_search_help()`` for examples of a good
+            search.
 
             Read more in the user guide at
-            https://herbie.readthedocs.io/en/latest/user_guide/searchString.html
+            https://herbie.readthedocs.io/en/latest/user_guide/search.html
         verbose : None, bool
             If True, then print a help message if no messages are found.
             If False, does not print a help message if no messages are found.
             If None (default), then verbose is set in the Herbie.__init__.
 
         Returns
         -------
         A Pandas DataFrame of the index file.
 
         """
         df = self.index_as_dataframe
 
+        # TODO: Remove this eventually
+        if searchString is not None:
+            warnings.warn(
+                "The argument `searchString` was renamed `search`. Please update your scripts.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+            search = searchString
+
         # This overrides the verbose specified in __init__
         if verbose is not None:
             self.verbose = verbose
 
-        # Filter DataFrame by searchString
-        if searchString not in [None, ":"]:
-            logic = df.search_this.str.contains(searchString)
+        # Filter DataFrame by regex search
+        if search not in [None, ":"]:
+            logic = df.search_this.str.contains(search)
             if (logic.sum() == 0) and verbose:
                 print(
-                    f"No GRIB messages found. There might be something wrong with {searchString=}"
+                    f"No GRIB messages found. There might be something wrong with {search=}"
                 )
-                print(_searchString_help(kind=self.IDX_STYLE))
+                print(_search_help(kind=self.IDX_STYLE))
             df = df.loc[logic]
         return df
 
     def download(
         self,
-        searchString=None,
+        search=None,
         *,
+        searchString=None,
         source=None,
         save_dir=None,
         overwrite=None,
         verbose=None,
         errors="warn",
     ):
         """
@@ -851,33 +832,33 @@
         TODO:   self.grib_source should change to represent the local file.
 
         Subsetting by variable follows the same principles described here:
         https://www.cpc.ncep.noaa.gov/products/wesley/fast_downloading_grib.html
 
         Parameters
         ----------
-        searchString : str
+        search : str
             If None, download the full file. Else, use regex to subset
             the file by specific variables and levels.
             Read more in the user guide:
-            https://herbie.readthedocs.io/en/latest/user_guide/searchString.html
+            https://herbie.readthedocs.io/en/latest/user_guide/search.html
         source : {'nomads', 'aws', 'google', 'azure', 'pando', 'pando2'}
             If None, download GRIB2 file from self.grib2 which is
             the first location the GRIB2 file was found from the
             priority lists when this class was initialized. Else, you
             may specify the source to force downloading it from a
             different location.
         save_dir : str or pathlib.Path
             Location to save the model output files.
             If None, uses the default or path specified in __init__.
             Else, changes the path files are saved.
         overwrite : bool
             If True, overwrite existing files. Default will skip
             downloading if the full file exists. Not applicable when
-            when searchString is not None because file subsets might
+            when search is not None because file subsets might
             be unique.
         errors : {'warn', 'raise'}
             When an error occurs, send a warning or raise a value error.
 
         """
 
         def _reporthook(a, b, c):
@@ -894,16 +875,16 @@
             total_size_MB = c / 1000000.0
             if verbose:
                 print(
                     f"\r🚛💨  Download Progress: {chunk_progress:.2f}% of {total_size_MB:.1f} MB\r",
                     end="",
                 )
 
-        def subset(searchString, outFile):
-            """Download a subset specified by the regex searchString."""
+        def subset(search, outFile):
+            """Download a subset specified by the regex search."""
             # TODO: Maybe optimize downloading multiple subsets with MultiThreading
 
             # TODO An alternative to downloadling subset with curl is
             # TODO  to use the request module directly.
             # TODO  >> headers = dict(Range=f"bytes={start_bytes}-{end_bytes}")
             # TODO  >> r = requests.get(grib_url, headers=headers)
 
@@ -919,15 +900,15 @@
 
             # -----------------------------------------------------
             # Download subsets of the file by byte range with cURL.
             #  Instead of using a single curl command for each row,
             #  group adjacent messages in the same curl command.
 
             # Find index groupings
-            idx_df = self.inventory(searchString).copy()
+            idx_df = self.inventory(search).copy()
             if verbose:
                 print(
                     f"Found {ANSI.bold}{ANSI.green}{len(idx_df)}{ANSI.reset} grib messages."
                 )
             idx_df["download_groups"] = idx_df.grib_message.diff().ne(1).cumsum()
 
             # cURL subsets of each group
@@ -963,24 +944,33 @@
                 if verbose:
                     print(curl)
                 os.system(curl)
 
             if verbose:
                 print(f"💾 Saved the subset to {outFile}")
 
+        # TODO: Remove this eventually
+        if searchString is not None:
+            warnings.warn(
+                "The argument `searchString` was renamed `search`. Please update your scripts.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+            search = searchString
+
         # This overrides the save_dir specified in __init__
         if save_dir is not None:
             self.save_dir = Path(save_dir).expand()
 
         if not hasattr(Path(self.save_dir).expand(), "exists"):
             self.save_dir = Path(self.save_dir).expand()
 
         # If the file exists in the localPath and we don't want to
         # overwrite, then we don't need to download it.
-        outFile = self.get_localFilePath(searchString=searchString)
+        outFile = self.get_localFilePath(search)
 
         if save_dir is not None:
             # Looks like the save_dir was changed.
             outFile = (
                 self.save_dir.expand()
                 / self.model
                 / f"{self.date:%Y%m%d}"
@@ -1010,15 +1000,15 @@
         if self.grib is None:
             msg = f"🦨 GRIB2 file not found: {self.model=} {self.date=} {self.fxx=}"
             if errors == "warn":
                 log.warning(msg)
                 return  # Can't download anything without a GRIB file URL.
             elif errors == "raise":
                 raise ValueError(msg)
-        if self.idx is None and searchString is not None:
+        if self.idx is None and search is not None:
             msg = f"🦨 Index file not found; cannot download subset: {self.model=} {self.date=} {self.fxx=}"
             if errors == "warn":
                 log.warning(
                     msg + " I will download the full file because I cannot subset."
                 )
             elif errors == "raise":
                 raise ValueError(msg)
@@ -1031,15 +1021,15 @@
         if not outFile.parent.is_dir():
             outFile.parent.mkdir(parents=True, exist_ok=True)
             print(f"👨🏻‍🏭 Created directory: [{outFile.parent}]")
 
         # ===============
         # Do the Download
         # ===============
-        if searchString in [None, ":"] or self.idx is None:
+        if search in [None, ":"] or self.idx is None:
             # Download the full file from remote source
             urllib.request.urlretrieve(self.grib, outFile, _reporthook)
 
             original_source = self.grib
 
             self.grib = outFile
             # self.grib_source = "local"  # ?? Why did I turn this off?
@@ -1047,39 +1037,50 @@
             if verbose:
                 print(
                     f"✅ Success! Downloaded {self.model.upper()} from \033[38;5;202m{self.grib_source:20s}\033[0m\n\tsrc: {original_source}\n\tdst: {outFile}"
                 )
 
         else:
             # Download a subset of the file
-            subset(searchString, outFile)
+            subset(search, outFile)
 
         return outFile
 
     def xarray(
         self,
+        search=None,
+        *,
         searchString=None,
         backend_kwargs={},
         remove_grib=True,
         **download_kwargs,
     ):
         """
         Open GRIB2 data as xarray DataSet.
 
         Parameters
         ----------
-        searchString : str
+        search : str
             Variables to read into xarray Dataset
         remove_grib : bool
             If True, grib file will be removed ONLY IF it didn't exist
             before we downloaded it.
         """
+        # TODO: Remove this eventually
+        if searchString is not None:
+            warnings.warn(
+                "The argument `searchString` was renamed `search`. Please update your scripts.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+            search = searchString
+
         download_kwargs = {**dict(overwrite=False), **download_kwargs}
 
-        local_file = self.get_localFilePath(searchString=searchString)
+        local_file = self.get_localFilePath(search)
 
         if "save_dir" in download_kwargs:
             # Looks like the save_dir was changed.
             self.save_dir = Path(download_kwargs["save_dir"]).expand()
             local_file = (
                 self.save_dir.expand()
                 / self.model
@@ -1093,24 +1094,24 @@
         #! File cannot be removed if it previously existed.
         #! (We don't want to remove previously downloaded content).
         if local_file.exists() and remove_grib:
             warnings.warn("Will not remove GRIB file because it previously existed.")
             remove_grib = False
         #! File can only be be removed if it is a subsetted file.
         #! (We don't want to remove full local files.)
-        if searchString is None and remove_grib:
+        if search is None and remove_grib:
             warnings.warn(
                 "Will not remove GRIB file because Herbie will only remove subsetted files (not full files)."
             )
             remove_grib = False
         #!==============================================================
 
         # Download file if local file does not exists
         if not local_file.exists() or download_kwargs["overwrite"]:
-            self.download(searchString=searchString, **download_kwargs)
+            self.download(search=search, **download_kwargs)
 
         # Backend kwargs for cfgrib
         backend_kwargs.setdefault("indexpath", "")
         backend_kwargs.setdefault(
             "read_keys", ["parameterName", "parameterUnits", "stepRange"]
         )
         backend_kwargs.setdefault("errors", "raise")
@@ -1143,30 +1144,28 @@
             # ----------------
             # Note: all attributes should still work with the `ds.to_netcdf()` method.
             ds.attrs["model"] = self.model
             ds.attrs["product"] = self.product
             ds.attrs["description"] = self.DESCRIPTION
             ds.attrs["remote_grib"] = self.grib
             ds.attrs["local_grib"] = str(local_file)
-            ds.attrs["searchString"] = searchString
+            ds.attrs["search"] = search
 
             # ----------------------
             # Attach CF grid mapping
             # ----------------------
             # http://cfconventions.org/Data/cf-conventions/cf-conventions-1.8/cf-conventions.html#appendix-grid-mappings
-            ds["gribfile_projection"] = None
-            ds["gribfile_projection"].attrs = cf_params
-            ds["gribfile_projection"].attrs[
-                "long_name"
-            ] = f"{self.model.upper()} model grid projection"
+            ds.coords["gribfile_projection"] = None
+            ds.coords["gribfile_projection"].attrs = cf_params
+            ds.coords["gribfile_projection"].attrs["long_name"] = (
+                f"{self.model.upper()} model grid projection"
+            )
 
             # Assign this grid_mapping for all variables
             for var in list(ds):
-                if var == "gribfile_projection":
-                    continue
                 ds[var].attrs["grid_mapping"] = "gribfile_projection"
 
         if remove_grib:
             # Load the datasets into memory before removing the file
             Hxr = [ds.load() for ds in Hxr]
             _ = [ds.close() for ds in Hxr]
             local_file.unlink()
@@ -1176,21 +1175,20 @@
         else:
             # cfgrib returned multiple hypercubes.
             try:
                 # Handle case where HRRR subh returns multiple hypercubes (see #73)
                 data_vars = set(itertools.chain(*[list(i) for i in Hxr]))
                 data_vars.remove("gribfile_projection")
                 Hxr = xr.concat(Hxr, dim="step", data_vars=data_vars)
-            except:
+            except Exception:
                 if self.verbose:
                     print(
                         f"Note: Returning a list of [{len(Hxr)}] xarray.Datasets because cfgrib opened with multiple hypercubes."
                     )
             return Hxr
 
-    # Shortcut Methods below
     def terrain(self, water_masked=True):
-        """Return model terrain as an xarray.Dataset."""
+        """Shortcut method to return model terrain as an xarray.Dataset."""
         ds = self.xarray(":(?:HGT|LAND):surface")
         if water_masked:
             ds["orog"] = ds.orog.where(ds.lsm > 0)
         return ds
```

### Comparing `herbie-data-2024.3.1/herbie/fast.py` & `herbie_data-2024.5.0/herbie/fast.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,29 +2,24 @@
 ## May 3, 2021
 
 """
 ============
 Herbie Tools
 ============
 """
-from datetime import datetime, timedelta
 
 import logging
-import cartopy.crs as ccrs
-import metpy  # accessor needed to parse crs
-import numpy as np
+
+# Multithreading :)
+from concurrent.futures import ThreadPoolExecutor, as_completed
+
 import pandas as pd
 import xarray as xr
 
-from herbie.core import Herbie, wgrib2_idx
-from . import Path
-
-# Multithreading :)
-from concurrent.futures import ThreadPoolExecutor
-from concurrent.futures import as_completed, wait
+from herbie.core import Herbie
 
 log = logging.getLogger(__name__)
 
 
 """
 🧵🤹🏻‍♂️ Notice! Multithreading and Multiprocessing is use
 
@@ -57,15 +52,15 @@
         raise ValueError(
             f"DATES must be a pandas-parsable datetime string or a list. Gave {DATES}"
         )
 
     return DATES
 
 
-def Herbie_latest(n=6, freq="1H", **kwargs):
+def Herbie_latest(n=6, freq="1h", **kwargs):
     """Search for the most recent GRIB2 file (using multithreading).
 
     Parameters
     ----------
     n : int
         Number of attempts to try.
     freq : pandas-parsable timedelta string
@@ -173,36 +168,36 @@
             self.objects[x : x + len(self.fxx)]
             for x in range(0, len(self.objects), len(self.fxx))
         ]
         return pd.DataFrame(
             ds_list, index=self.DATES, columns=[f"F{i:02d}" for i in self.fxx]
         )
 
-    def inventory(self, searchString=None):
+    def inventory(self, search=None):
         """Get combined inventory DataFrame.
 
-        Useful for data discovery and checking your searchString before
+        Useful for data discovery and checking your search before
         doing a download.
         """
         # NOTE: In my quick test, you don't gain much speed using multithreading here.
         dfs = []
         for i in self.file_exists:
-            df = i.inventory(searchString)
+            df = i.inventory(search)
             df = df.assign(FILE=i.grib)
             dfs.append(df)
         return pd.concat(dfs, ignore_index=True)
 
-    def download(self, searchString=None, *, max_threads=20, **download_kwargs):
+    def download(self, search=None, *, max_threads=20, **download_kwargs):
         r"""Download many Herbie objects
 
         Uses multithreading.
 
         Parameters
         ----------
-        searchString : string
+        search : string
             Regular expression string to specify which GRIB messages to
             download.
         **download_kwargs :
             Any kwarg for Herbie's download method.
 
         Benchmark
         ---------
@@ -217,30 +212,30 @@
         # Multithread the downloads
         threads = min(self.tasks, max_threads)
         log.info(f"🧵 Working on {self.tasks} tasks with {threads} threads.")
 
         outFiles = []
         with ThreadPoolExecutor(threads) as exe:
             futures = [
-                exe.submit(H.download, searchString, **download_kwargs)
+                exe.submit(H.download, search, **download_kwargs)
                 for H in self.file_exists
             ]
 
             # Return list of Herbie objects in order completed
             for future in as_completed(futures):
                 if future.exception() is None:
                     outFiles.append(future.result())
                 else:
                     log.error(f"Exception has occured : {future.exception()}")
 
         return outFiles
 
     def xarray(
         self,
-        searchString,
+        search,
         *,
         max_threads=None,
         **xarray_kwargs,
     ):
         """Read many Herbie objects into an xarray Dataset.
 
         # TODO: Sometimes the Jupyter Cell always crashes when I run this.
@@ -260,15 +255,15 @@
         Opening 48 files with 1 variable (TMP:2 m)
             - 1 thread took 1 min 45 s
             - 2 threads took 55 s
             - 5 threads took 39 s
             - 10 threads took 39 s
             - 50 threads took 37 s
         """
-        xarray_kwargs = dict(searchString=searchString, **xarray_kwargs)
+        xarray_kwargs = dict(search=search, **xarray_kwargs)
 
         # NOTE: Multiprocessing does not seem to work because it looks
         # NOTE: like xarray objects are not pickleable.
         # NOTE: ``Reason: 'TypeError("cannot pickle '_thread.lock' object"``
 
         if max_threads:
             ###########################
@@ -310,11 +305,10 @@
         except:
             # TODO: I'm not sure why some cases doesn't like the combine_attrs argument
             ds = xr.combine_nested(
                 ds_list,
                 concat_dim=["time", "step"],
             )
 
-        ds["gribfile_projection"] = ds.gribfile_projection[0][0]
         ds = ds.squeeze()
 
         return ds
```

### Comparing `herbie-data-2024.3.1/herbie/help.py` & `herbie_data-2024.5.0/herbie/help.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,29 @@
-## Brian Blaylock
-## April 12, 2022
-
-"""
-================
-Some Herbie Help
-================
-"""
+"""Some help messages from Herbie."""
 
 
-def _searchString_help(kind="wgrib2"):
-    """
-    Help/Error Message for `searchString`
+def _search_help(kind="wgrib2"):
+    """Help/Error Message for `search` argument.
 
     Parameters
     ----------
     kind : {"wgrib2", "eccodes"}
         There are two different utilities used to create index files and
         they create different file output.
 
         - **wgrib2** is the NCEP-style grib messages
         - **eccodes** is the ECMWF-style grib messages
     """
-
     if kind == "wgrib2":
         msg = r"""
 Use regular expression to search for lines in the index file.
-Here are some examples you can use for the wgrib2-style `searchString`
+Here are some examples you can use for the wgrib2-style `search`
 
     ==================================== ==========================================================
-    ``searchString=``                    GRIB messages that will be downloaded
+    search=                              GRIB messages that will be downloaded
     ==================================== ==========================================================
     ":TMP:2 m"                           Temperature at 2 m.
     ":TMP:"                              Temperature fields at all levels.
     ":UGRD:\d+ mb"                       U Wind at all pressure levels.
     ":500 mb:"                           All variables on the 500 mb level.
     ":APCP:"                             All accumulated precipitation fields.
     ":APCP:surface:0-[1-9]*"             Accumulated precip since initialization time
@@ -48,57 +39,79 @@
     ":REFC:"                             Composite Reflectivity
     ":surface:"                          All variables at the surface.
     "^TMP:2 m.*fcst$"                    Beginning of string (^), end of string ($) wildcard (.*)
     ==================================== ==========================================================
 
 If you need help with regular expression, search the web or look at
 this cheatsheet: https://www.petefreitag.com/cheatsheets/regex/.
+
+Here is an example: https://regex101.com/r/1Dku20/1
 """
 
     elif kind == "eccodes":
-        msg = """
+        msg = r"""
 Use regular expression to search for lines in the index file.
-Here are some examples you can use for the ecCodes-style `searchString`
+Here are some examples you can use for the ecCodes-style `search`
 
 Look at the ECMWF GRIB Parameter Database
 https://apps.ecmwf.int/codes/grib/param-db
 
+
+product=`oper` or `enfo`
 ======================== ==============================================
-searchString (oper/enso) Messages that will be downloaded
+search=                  GRIB messages that will be downloaded
 ======================== ==============================================
 ":2t:"                   2-m temperature
+":2d:"                   2-m dew point temperature
 ":10u:"                  10-m u wind vector
 ":10v:"                  10-m v wind vector
-":10(u|v):               **10m u and 10m v wind**
+":10[uv]:                10-m u and 10-m v wind
+":[tuvr]:"               Temp, u/v wind, RH (all levels)
+":500:"                  All variables on the 500 hPa level
+":gh:500"                Geopotential height only at 500 hPa
+":gh:"                   Geopotential height (all pressure levels)
+":t:"                    Temperature (all pressure levels)
+":q:"                    Specific Humidity (all pressure levels)
+":r:"                    Relative humidity (all pressure levels)
+":v:"                    v wind vector (all pressure levels)
+":u:"                    u wind vector (all pressure levels)
+":w:"                    Vertical velocity (Pascals per second)
+":lsm:"                  Land-sea mask
+":ttr:"                  Top net long-wave (thermal) radiation
+":ssrd:"                 Surface short-wave (solar) radiation downwards
+":ssr:"                  Surface net short-wave (solar) radiation
+":strd:"                 Surface long-wave (thermal) radiation downwards
+":str:"                  Surface net long-wave (thermal) radiation
+":swvl1:"                Volumetric soil water layer 1 (depth 0 meters)
+":swvl2:"                Volumetric soil water layer 2 (depth 7 meters)
+":swvl3:"                Volumetric soil water layer 3 (depth 28 meters)
+":swvl4:"                Volumetric soil water layer 4 (depth 100 meters)
+":skt:"                  Skin (surface) temperature
 ":d:"                    Divergence (all levels)
-":gh:"                   geopotential height (all levels)
-":gh:500"                geopotential height only at 500 hPa
-":st:"                   soil temperature
-":tp:"                   total precipitation
-":msl:"                  mean sea level pressure
-":q:"                    Specific Humidity
-":r:"                    relative humidity
-":ro:"                   Runn-off
-":skt:"                  skin temperature
-":sp:"                   surface pressure
-":t:"                    temperature
+":st:"                   Soil temperature
+":stl2:"                 Soil temperature level 2 (depth 7 meters)
+":tp:"                   Total precipitation
+":ro:"                   Run-off
+":asn:"                  Snow albedo
+":msl:"                  Mean sea level pressure
+":sp:"                   Surface pressure
+":cape:"                 CAPE
 ":tcwv:"                 Total column vertically integrated water vapor
 ":vo:"                   Relative vorticity
-":v:"                    v wind vector
-":u:"                    u wind vector
-":(t|u|v|r):"            Temp, u/v wind, RH (all levels)
-":500:"                  All variables on the 500 hPa level
 
+product=`wave` or `waef`
 ======================== ==============================================
-searchString (wave/waef) Messages that will be downloaded
+search=                  GRIB messages that will be downloaded
 ======================== ==============================================
 ":swh:"                  Significant height of wind waves + swell
 ":mwp:"                  Mean wave period
 ":mwd:"                  Mean wave direction
 ":pp1d:"                 Peak wave period
 ":mp2:"                  Mean zero-crossing wave period
 
 If you need help with regular expression, search the web or look at
 this cheatsheet: https://www.petefreitag.com/cheatsheets/regex/.
+
+Here is an example: https://regex101.com/r/niNjwp/1
 """
 
     return msg
```

### Comparing `herbie-data-2024.3.1/herbie/hrrr_zarr.py` & `herbie_data-2024.5.0/herbie/hrrr_zarr.py`

 * *Files identical despite different names*

### Comparing `herbie-data-2024.3.1/herbie/latest.py` & `herbie_data-2024.5.0/herbie/latest.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,17 @@
         but I also know AWS gets the data pretty quick. So, check AWS
         first, then check NOMADS (because if you make too many downloads
         from NOMADS your IP address will get blocked.)
     **kwargs
         Any other input you want passed to the Herbie class.
     """
     if model.lower() in ["hrrr", "rap", "rrfs"]:
-        freq = "1H"
+        freq = "1h"
     else:
-        freq = "6H"
+        freq = "6h"
 
     # Create a list of recent dates to try
     dates = pd.date_range(
         pd.Timestamp.utcnow().floor(freq).tz_localize(None),
         periods=4,
         freq=f"-{freq}",
     )
```

### Comparing `herbie-data-2024.3.1/herbie/misc.py` & `herbie_data-2024.5.0/herbie/misc.py`

 * *Files identical despite different names*

### Comparing `herbie-data-2024.3.1/herbie/models/README.md` & `herbie_data-2024.5.0/herbie/models/README.md`

 * *Files identical despite different names*

### Comparing `herbie-data-2024.3.1/herbie/models/__init__.py` & `herbie_data-2024.5.0/herbie/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,25 +13,27 @@
 from herbie import _config_path
 from herbie.misc import ANSI
 
 # ======================================================================
 #                     Import Public Model Templates
 # ======================================================================
 from .ecmwf import *
+from .gdps import *
 from .gefs import *
 from .gfs import *
 from .hafs import *
 from .hrdps import *
 from .hrrr import *
 from .nam import *
 from .navgem import *
 from .nbm import *
 from .nexrad import *
 from .nogaps import *
 from .rap import *
+from .rdps import *
 from .rrfs import *
 from .rtma import *
 from .urma import *
 
 # ======================================================================
 #                     Import Private Model Templates
 # ======================================================================
```

### Comparing `herbie-data-2024.3.1/herbie/models/ecmwf.py` & `herbie_data-2024.5.0/herbie/models/ecmwf.py`

 * *Files identical despite different names*

### Comparing `herbie-data-2024.3.1/herbie/models/gefs.py` & `herbie_data-2024.5.0/herbie/models/gefs.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
     These grib files are organized different from other model types.
     The files are grouped into variables and clumped by forecast range.
     Thus, instead of a one file having all the variables for that lead time,
     a file has one variable for many lead times. This changes the way
     a user would use Herbie to access GEFS data. A user will need to supply
     the "variable". For getting specific grib messages, you will use the
-    "searchString" argument to key in on the variable of interest. However,
+    "search" argument to key in on the variable of interest. However,
     you will still need to give a value for "fxx" to tell Herbie which
     directory to look for. Yeah, it's a little different paradigm for Herbie,
     but we can work with it.
 
     Provide arguments for
 
     - date (2000-2019)
```

### Comparing `herbie-data-2024.3.1/herbie/models/gfs.py` & `herbie_data-2024.5.0/herbie/models/gfs.py`

 * *Files identical despite different names*

### Comparing `herbie-data-2024.3.1/herbie/models/hafs.py` & `herbie_data-2024.5.0/herbie/models/hafs.py`

 * *Files identical despite different names*

### Comparing `herbie-data-2024.3.1/herbie/models/hrdps.py` & `herbie_data-2024.5.0/herbie/models/hrdps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 ## Added by Brian Blaylock
 ## June 21, 2023
+## Updated by Bryan Guarente
+## April 9, 2024
 
 """
 A Herbie template for the High Resolution Deterministic Prediction System (HRDPS)
 
 Meteorological Service of Canada (MSC)
 The HRDPS is Canada's 2.5 km deterministic model
 
@@ -36,99 +38,112 @@
     {'0250', '0500', '0700', '0850', '1000', '0050', '0100', '0150',
     '0175', '0200', '0225', '0275', '0300', '0350', '0400', '0450',
     '0550', '0600', '0650', '0750', '0800', '0875', '0900', '0925',
 '0950', '0970', '0985', '1015'}
 """
 
 _variable = {
+    "ABSV",
+    "ACPCP",
     "ALBDO",
+    "APCP",
     "CAPE",
     "CWAT",
     "DEN",
+    "GUST_MAX",
+    "GUST_MIN",
     "DEPR",
     "DLWRF",
     "DPT",
     "DSWRF",
     "GUST-Max",
     "GUST-Min",
     "GUST",
     "HGT",
     "HLCY",
     "HPBL",
-    "ICEC",
-    "LAND",
     "LHTFL",
+    "MU-VT-LI",
     "NLWRS",
     "NSWRS",
+    "PRATE",
     "PRES",
     "PRMSL",
+    "PTYPE",
     "RH",
     "SDEN",
     "SDWE",
     "SFCWRO",
     "SHTFL",
+    "SHWINX",
     "SKINT",
     "SNOD",
     "SOILVIC",
     "SOILW",
     "SPFH",
     "TCDC",
     "TMP",
     "TSOIL",
     "UGRD",
     "ULWRF",
     "USWRF",
     "UTCI",
     "VGRD",
+    "VI",
+    "VVEL",
     "WDIR",
+    "WEAFR",
+    "WEAPE",
+    "WEARN",
+    "WEASN",
     "WIND",
-    "WTMP",
 }
 
 _level = {
-    "Sfc",
-    "EATM",
+    "AGL-10m",
     "AGL-120m",
+    "AGL-2m",
     "AGL-40m",
     "AGL-80m",
-    "AGL-2m",
-    "NTAT",
-    "AGL-10m",
-    "ISBY-1000-500",
-    "MSL",
     "DBS-0-10cm",
     "DBS-0-1cm",
-    "ISBL_0250",
-    "ISBL_0500",
-    "ISBL_0700",
-    "ISBL_0850",
+    "EATM",
+    "ISBL_100",
     "ISBL_1000",
-    "ISBL_0050",
-    "ISBL_0100",
-    "ISBL_0150",
-    "ISBL_0175",
-    "ISBL_0200",
-    "ISBL_0225",
-    "ISBL_0275",
-    "ISBL_0300",
-    "ISBL_0350",
-    "ISBL_0400",
-    "ISBL_0450",
-    "ISBL_0550",
-    "ISBL_0600",
-    "ISBL_0650",
-    "ISBL_0750",
-    "ISBL_0800",
-    "ISBL_0875",
-    "ISBL_0900",
-    "ISBL_0925",
-    "ISBL_0950",
-    "ISBL_0970",
-    "ISBL_0985",
     "ISBL_1015",
+    "ISBL_150",
+    "ISBL_175",
+    "ISBL_200",
+    "ISBL_225",
+    "ISBL_250",
+    "ISBL_275",
+    "ISBL_300",
+    "ISBL_350",
+    "ISBL_400",
+    "ISBL_450",
+    "ISBL_50",
+    "ISBL_500",
+    "ISBL_550",
+    "ISBL_600",
+    "ISBL_650",
+    "ISBL_700",
+    "ISBL_750",
+    "ISBL_800",
+    "ISBL_850",
+    "ISBL_875",
+    "ISBL_900",
+    "ISBL_925",
+    "ISBL_950",
+    "ISBL_970",
+    "ISBL_985",
+    "ISBY-1000-500",
+    "MSL",
+    "NTAT",
+    "Sfc",
+    "TGL_10",
 }
 
 
 class hrdps:
     def template(self):
         if not hasattr(self, "variable"):
             print(
@@ -184,12 +199,12 @@
             "Datamart product description": "https://eccc-msc.github.io/open-data/msc-data/nwp_hrdps/readme_hrdps-datamart_en",
         }
         self.PRODUCTS = {
             "north/grib2": "North domain (experimental)",
         }
         PATH = f"{self.date:%H}/{self.fxx:03d}/CMC_hrdps_north_{self.variable}_{self.level}_ps2.5km_{self.date:%Y%m%d%H}_P{self.fxx:03d}-00.grib2"
         self.SOURCES = {
-            "msc": f"https://dd.weather.gc.ca/model_hrdps/{self.product}/{PATH}",
+            "msc": f"https://dd.weather.gc.ca/model_hrdps/{self.product}/{PATH}"
         }
 
         self.IDX_SUFFIX = [".grb2.idx", ".idx", ".grib.idx"]
         self.LOCALFILE = f"{self.get_remoteFileName}"
```

### Comparing `herbie-data-2024.3.1/herbie/models/hrrr.py` & `herbie_data-2024.5.0/herbie/models/hrrr.py`

 * *Files identical despite different names*

### Comparing `herbie-data-2024.3.1/herbie/models/local.py` & `herbie_data-2024.5.0/herbie/models/local.py`

 * *Files identical despite different names*

### Comparing `herbie-data-2024.3.1/herbie/models/nam.py` & `herbie_data-2024.5.0/herbie/models/nam.py`

 * *Files identical despite different names*

### Comparing `herbie-data-2024.3.1/herbie/models/navgem.py` & `herbie_data-2024.5.0/herbie/models/navgem.py`

 * *Files identical despite different names*

### Comparing `herbie-data-2024.3.1/herbie/models/nbm.py` & `herbie_data-2024.5.0/herbie/models/nbm.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,7 +19,30 @@
             "pr": "Puerto Rico 13-km resolution",
         }
         self.SOURCES = {
             "nomads": f"https://nomads.ncep.noaa.gov/pub/data/nccf/com/blend/prod/blend.{self.date:%Y%m%d/%H}/core/blend.t{self.date:%H}z.core.f{self.fxx:03d}.{self.product}.grib2",
             "aws": f"https://noaa-nbm-grib2-pds.s3.amazonaws.com/blend.{self.date:%Y%m%d/%H}/core/blend.t{self.date:%H}z.core.f{self.fxx:03d}.{self.product}.grib2",
         }
         self.LOCALFILE = f"{self.get_remoteFileName}"
+
+
+class nbmqmd:
+    def template(self):
+        self.DESCRIPTION = "National Blend of Models - QMD"
+        self.DETAILS = {
+            "NOMADS product description": "https://www.nco.ncep.noaa.gov/pmb/products/blend/",
+            "AWS Registry": "https://registry.opendata.aws/noaa-nbm/",
+            "NWS National Blend of Models Home": "https://www.weather.gov/mdl/nbm_home",
+            "MDL NBM Page": "https://vlab.noaa.gov/web/mdl/nbm",
+        }
+        self.PRODUCTS = {
+            "ak": "Alaska; 13-km resolution",
+            "co": "CONUS 13-km resolution",
+            "gu": "Guam 13-km resolution",
+            "hi": "Hawaii 13-km resolution",
+            "pr": "Puerto Rico 13-km resolution",
+        }
+        self.SOURCES = {
+            "nomads": f"https://nomads.ncep.noaa.gov/pub/data/nccf/com/blend/prod/blend.{self.date:%Y%m%d/%H}/qmd/blend.t{self.date:%H}z.qmd.f{self.fxx:03d}.{self.product}.grib2",
+            "aws": f"https://noaa-nbm-grib2-pds.s3.amazonaws.com/blend.{self.date:%Y%m%d/%H}/qmd/blend.t{self.date:%H}z.qmd.f{self.fxx:03d}.{self.product}.grib2",
+        }
+        self.LOCALFILE = f"{self.get_remoteFileName}"
```

### Comparing `herbie-data-2024.3.1/herbie/models/nexrad.py` & `herbie_data-2024.5.0/herbie/models/nexrad.py`

 * *Files identical despite different names*

### Comparing `herbie-data-2024.3.1/herbie/models/nogaps.py` & `herbie_data-2024.5.0/herbie/models/nogaps.py`

 * *Files identical despite different names*

### Comparing `herbie-data-2024.3.1/herbie/models/rap.py` & `herbie_data-2024.5.0/herbie/models/rap.py`

 * *Files identical despite different names*

### Comparing `herbie-data-2024.3.1/herbie/models/rrfs.py` & `herbie_data-2024.5.0/herbie/models/rrfs.py`

 * *Files identical despite different names*

### Comparing `herbie-data-2024.3.1/herbie/models/rtma.py` & `herbie_data-2024.5.0/herbie/models/rtma.py`

 * *Files identical despite different names*

### Comparing `herbie-data-2024.3.1/herbie/models/urma.py` & `herbie_data-2024.5.0/herbie/models/urma.py`

 * *Files identical despite different names*

### Comparing `herbie-data-2024.3.1/herbie/wgrib2.py` & `herbie_data-2024.5.0/herbie/wgrib2.py`

 * *Files identical despite different names*

### Comparing `herbie-data-2024.3.1/herbie_data.egg-info/PKG-INFO` & `herbie_data-2024.5.0/herbie_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: herbie-data
-Version: 2024.3.1
+Version: 2024.5.0
 Summary: Download numerical weather prediction GRIB2 model data.
 Author-email: "Brian K. Blaylock" <blaylockbk@gmail.com>
 Maintainer-email: "Brian K. Blaylock" <blaylockbk@gmail.com>
 License: MIT License
         
-        Copyright (c) 2019-2022 Brian K. Blaylock
+        Copyright (c) 2019-2024 Brian K. Blaylock
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -43,25 +43,27 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cartopy
+Requires-Dist: cfgrib
 Requires-Dist: matplotlib
+Requires-Dist: metpy
 Requires-Dist: numpy
 Requires-Dist: pandas
-Requires-Dist: xarray
-Requires-Dist: cfgrib
-Requires-Dist: metpy
-Requires-Dist: cartopy
-Requires-Dist: toml
 Requires-Dist: pygrib
+Requires-Dist: scikit-learn
+Requires-Dist: toml
+Requires-Dist: xarray
 Provides-Extra: docs
 Requires-Dist: autodocsumm; extra == "docs"
+Requires-Dist: ipython; extra == "docs"
 Requires-Dist: linkify-it-py; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: nbconvert; extra == "docs"
 Requires-Dist: nbsphinx; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: pydata-sphinx-theme; extra == "docs"
 Requires-Dist: recommonmark; extra == "docs"
@@ -103,15 +105,17 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/herbie-data?label=pypi|downloads)
 
 
 <!-- (Badges) -->
 
 </div>
 
-**Herbie** is a python package that downloads recent and archived numerical weather prediction (NWP) model output from different cloud archive sources. **Its most popular capability is to download HRRR model data.** NWP data in GRIB2 format can be read with xarray+cfgrib. Much of this data is made available through the [NOAA Open Data Dissemination](https://www.noaa.gov/information-technology/open-data-dissemination) (NODD) Program (formerly the Big Data Program) which has made weather data more accessible than ever before.
+**Herbie** is a python package that downloads recent and archived numerical weather prediction (NWP) model output from different cloud archive sources. NWP data is distributed in GRIB2 format and can be read with xarray+cfgrib. 
+
+# 📓 [Herbie Documentation](https://herbie.readthedocs.io/)
 
 Herbie helps you discover, download, and read data from:
 
 - [High Resolution Rapid Refresh (HRRR)](https://herbie.readthedocs.io/en/latest/user_guide/_model_notebooks/hrrr.html) | [HRRR-Alaska](https://herbie.readthedocs.io/en/latest/user_guide/_model_notebooks/hrrrak.html)
 - [Rapid Refresh (RAP)](https://herbie.readthedocs.io/en/latest/user_guide/_model_notebooks/rap.html)
 - [Global Forecast System (GFS)](https://herbie.readthedocs.io/en/latest/user_guide/_model_notebooks/gfs.html)
 - [Global Ensemble Forecast System (GEFS)](https://herbie.readthedocs.io/en/latest/user_guide/_model_notebooks/gefs.html)
@@ -120,15 +124,16 @@
 - [North American Mesoscale Model (NAM)](https://github.com/blaylockbk/Herbie/blob/main/docs/user_guide/_model_notebooks/nam.ipynb)
 - [National Blend of Models (NBM)](https://herbie.readthedocs.io/en/latest/user_guide/_model_notebooks/nbm.html)
 - [Rapid Refresh Forecast System (RRFS)](https://herbie.readthedocs.io/en/latest/user_guide/_model_notebooks/rrfs.html) _prototype_
 - [Real-Time/Un-Restricted Mesoscale Analysis (RTMA/URMA)](https://herbie.readthedocs.io/en/latest/user_guide/_model_notebooks/rtma.html)
 - [Hurricane Analysis And Forecast System (HAFS)](https://herbie.readthedocs.io/en/latest/user_guide/_model_notebooks/hafs.html)
 - [High Resolution Deterministic Prediction System (HRDPS)](https://herbie.readthedocs.io/en/latest/user_guide/_model_notebooks/hrdps.html)
 
-# 📓 [Herbie Documentation](https://herbie.readthedocs.io/)
+Much of this data is made available through the [NOAA Open Data Dissemination](https://www.noaa.gov/information-technology/open-data-dissemination) (NODD) program (formerly the Big Data Program) which has made weather data more accessible than ever before.
+
 
 ## Installation
 
 The easiest way to instal Herbie and its dependencies is with [Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) from conda-forge.
 
 ```bash
 conda install -c conda-forge herbie-data
@@ -147,17 +152,16 @@
 
 # Activate the environment
 conda activate herbie
 ```
 
 Alternatively, Herbie is published on PyPI and you can install it with pip, _but_ it requires some dependencies that you will have to install yourself:
 
-- Python 3.8 to 3.11
+- Python 3.9+
 - cURL
-- [Cartopy](https://scitools.org.uk/cartopy/docs/latest/installing.html), which requires GEOS and Proj.
 - [cfgrib](https://github.com/ecmwf/cfgrib), which requires eccodes.
 - _Optional:_ wgrib2
 - _Optional:_ [Carpenter Workshop](https://github.com/blaylockbk/Carpenter_Workshop)
 
 When those are installed within your environment, _then_ you can install Herbie with pip.
 
 ```bash
@@ -219,14 +223,16 @@
 # Download a subset, like all fields at 500 mb
 H.download(":500 mb")
 
 # Read subset with xarray, like 2-m temperature.
 H.xarray("TMP:2 m")
 ```
 
+Herbie also provides some custom xarray accessors to help you get the grid projection or pick points from the grid nearest a latitude-longitude location.
+
 ## Data Sources
 
 Herbie downloads model data from the following sources, but can be extended to include others:
 
 - [NOMADS](https://nomads.ncep.noaa.gov/)
 - [NOAA Open Data Dissemination Program (NODD)](https://www.noaa.gov/information-technology/open-data-dissemination) partners (i.e., AWS, Google, Azure).
 - [ECMWF Open Data Forecasts](https://www.ecmwf.int/en/forecasts/datasets/open-data)
@@ -263,15 +269,15 @@
 
 **Thanks for using Herbie, and happy racing!**
 
 🏁 Brian
 
 |     |                                                                                                     |
 | :-: | --------------------------------------------------------------------------------------------------- |
-| 👨🏻‍💻  | [Contributing Guide/Disclaimer](https://herbie.readthedocs.io/en/stable/user_guide/disclaimer.html) |
+| 👨🏻‍💻  | [Contributing Guide/Disclaimer](https://herbie.readthedocs.io/en/stable/user_guide/housekeeping/disclaimer.html) |
 | 💬  | [GitHub Discussions](https://github.com/blaylockbk/Herbie/discussions)                              |
 | 🚑  | [GitHub Issues](https://github.com/blaylockbk/Herbie/issues)                                        |
 | 🌐  | [Personal Webpage](http://home.chpc.utah.edu/~u0553130/Brian_Blaylock/home.html)                    |
 | 🌐  | [University of Utah HRRR archive](http://hrrr.chpc.utah.edu/)                                       |
 
 <br>
```

### Comparing `herbie-data-2024.3.1/herbie_data.egg-info/SOURCES.txt` & `herbie_data-2024.5.0/herbie_data.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,63 @@
 .gitattributes
 .gitignore
 .readthedocs.yml
 CITATION.cff
 HOW-TO-RELEASE.md
-Herbie.svg
 LICENSE
 MANIFEST.in
 README.md
 environment-dev.yml
 environment-test.yml
 environment.yml
 makefile
 pyproject.toml
 requirements-test.txt
 requirements.txt
-test.toml
 herbie/__init__.py
 herbie/_version.py
 herbie/accessors.py
 herbie/core.py
 herbie/fast.py
 herbie/help.py
 herbie/hrrr_zarr.py
 herbie/latest.py
 herbie/misc.py
 herbie/wgrib2.py
 herbie/models/README.md
 herbie/models/__init__.py
 herbie/models/ecmwf.py
+herbie/models/gdps.py
 herbie/models/gefs.py
 herbie/models/gfs.py
 herbie/models/hafs.py
 herbie/models/hrdps.py
 herbie/models/hrrr.py
 herbie/models/local.py
 herbie/models/nam.py
 herbie/models/navgem.py
 herbie/models/nbm.py
 herbie/models/nexrad.py
 herbie/models/nogaps.py
 herbie/models/rap.py
+herbie/models/rdps.py
 herbie/models/rrfs.py
 herbie/models/rtma.py
 herbie/models/urma.py
 herbie_data.egg-info/PKG-INFO
 herbie_data.egg-info/SOURCES.txt
 herbie_data.egg-info/dependency_links.txt
 herbie_data.egg-info/requires.txt
 herbie_data.egg-info/top_level.txt
 tests/__init__.py
 tests/test_accessors.py
+tests/test_core.py
 tests/test_ecmwf.py
 tests/test_fast.py
 tests/test_first.py
 tests/test_gefs.py
 tests/test_gfs.py
 tests/test_hrrr.py
 tests/test_init.py
+tests/test_pick_points.py
 tests/test_rap.py
 tests/util.py
```

### Comparing `herbie-data-2024.3.1/makefile` & `herbie_data-2024.5.0/makefile`

 * *Files identical despite different names*

### Comparing `herbie-data-2024.3.1/pyproject.toml` & `herbie_data-2024.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,36 +26,38 @@
     "forecast",
     "atmosphere",
     "GRIB2",
     "xarray",
     "HRRR",
 ]
 dependencies = [
+    "cartopy",
+    "cfgrib",
     "matplotlib",
+    "metpy",
     "numpy",
     "pandas",
-    "xarray",
-    "cfgrib",
-    "metpy",
-    "cartopy",
-    "toml",
     "pygrib",
+    "scikit-learn",
+    "toml",
+    "xarray",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/blaylockbk/Herbie"
 "Documentation" = "https://herbie.readthedocs.io/"
 "Repository" = "https://github.com/blaylockbk/Herbie"
 "Changelog" = "https://github.com/blaylockbk/Herbie/releases"
 "Bug Tracker" = "https://github.com/blaylockbk/Herbie/issues"
 
 [project.optional-dependencies]
 docs = [
     "autodocsumm",
+    "ipython",
     "linkify-it-py",
     "myst-parser",
     "nbconvert",
     "nbsphinx",
     "sphinx-copybutton",
     "pydata-sphinx-theme",
     "recommonmark",
```

### Comparing `herbie-data-2024.3.1/tests/test_gefs.py` & `herbie_data-2024.5.0/tests/test_gefs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 ## Brian Blaylock
 ## February 9, 2022
 
-"""
-Tests for downloading GFS model
-"""
+"""Tests for downloading GEFS model."""
 
-from herbie import Herbie
+from herbie import Herbie, config
 
-save_dir = "$TMPDIR/Herbie-Tests/"
+save_dir = config["default"]["save_dir"] / "Herbie-Tests-Data/"
 
 
 def test_gefs():
     H = Herbie(
         "2023-01-01 06:00",
         model="gefs",
         fxx=12,
         member="mean",
         save_dir=save_dir,
+        overwrite=True,
     )
 
     assert H.grib, "GEFS grib2 file not found"
     assert H.idx, "GEFS index file not found"
 
 
 def test_gefs_reforecast():
     H = Herbie(
         "2017-03-14",
         model="gefs_reforecast",
         fxx=12,
         member=0,
         variable_level="tmp_2m",
         save_dir=save_dir,
+        overwrite=True,
     )
 
     assert H.grib, "GEFS grib2 file not found"
     assert H.idx, "GEFS index file not found"
```

### Comparing `herbie-data-2024.3.1/tests/test_gfs.py` & `herbie_data-2024.5.0/tests/test_gfs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 ## Brian Blaylock
 ## February 9, 2022
 
-"""
-Tests for downloading GFS model
-"""
+"""Tests for downloading GFS model."""
 
 from datetime import datetime, timedelta
 
-from herbie import Herbie
+from herbie import Herbie, config
 
 now = datetime.now()
 today = datetime(now.year, now.month, now.day) - timedelta(hours=12)
 today_str = today.strftime("%Y-%m-%d %H:%M")
 
-save_dir = "$TMPDIR/Herbie-Tests/"
+save_dir = config["default"]["save_dir"] / "Herbie-Tests-Data/"
 
 
 def test_gfs():
     H = Herbie(
         today,
         priority="aws",
         product="pgrb2.0p25",
         model="gfs",
-        save_dir="$TMPDIR/Herbie-Tests/",
+        save_dir=save_dir,
+        overwrite=True,
     )
 
     assert H.grib, "GFS grib2 file not found"
     assert H.idx, "GFS index file not found"
 
-    H.download()
-    assert H.get_localFilePath().exists()
+    filter = ":TMP:2 m"
+    f = H.download(filter)
+    assert H.get_localFilePath(filter).exists(), "File doesn't exist!"
+    f.unlink()
 
-    H.xarray("TMP:2 m", remove_grib=False)
-    assert H.get_localFilePath("TMP:2 m").exists()
+    H.xarray(filter)
```

### Comparing `herbie-data-2024.3.1/tests/test_hrrr.py` & `herbie_data-2024.5.0/tests/test_hrrr.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,46 +5,68 @@
 Tests for downloading HRRR model
 """
 from datetime import datetime, timedelta
 from shutil import which
 
 import pytest
 
-from herbie import Herbie, Path
+from herbie import Herbie, Path, config
 import os
 import requests
 import pandas as pd
 
 now = datetime.now()
 today = datetime(now.year, now.month, now.day, now.hour) - timedelta(hours=6)
 yesterday = today - timedelta(days=1)
 today_str = today.strftime("%Y-%m-%d %H:%M")
 yesterday_str = yesterday.strftime("%Y-%m-%d %H:%M")
-save_dir = Path("$TMPDIR/Herbie-Tests/").expand()
+
+save_dir = config["default"]["save_dir"] / "Herbie-Tests-Data/"
+
+# Remove all previous test data
+for i in (save_dir / "hrrr").rglob("*"):
+    if i.is_file():
+        i.unlink()
 
 # Location of wgrib2 command, if it exists
 wgrib2 = which("wgrib2")
 
 
-def test_hrrr_aws1():
-    # Test HRRR with datetime.datetime date
+def test_hrrr_download():
     H = Herbie(
         today,
         model="hrrr",
         product="sfc",
+        overwrite=True,
         save_dir=save_dir,
     )
-    H.download()
+    f = H.download()
     assert H.get_localFilePath().exists()
+    f.unlink()
+
+
+def test_hrrr_xarray():
+    H = Herbie(
+        today,
+        model="hrrr",
+        product="sfc",
+        overwrite=True,
+        save_dir=save_dir,
+    )
     H.xarray("TMP:2 m", remove_grib=False)
     assert H.get_localFilePath("TMP:2 m").exists()
+    H.get_localFilePath("TMP:2 m").unlink()
 
 
 def test_hrrr_to_netcdf():
-    """Check that a xarray Dataset can be written to a NetCDF file."""
+    """Check that a xarray Dataset can be written to a NetCDF file.
+
+    It is important that I have haven't put any python objects in the
+    xarray Dataset attributes.
+    """
     H = Herbie(
         "2022-01-01 06:00",
         model="hrrr",
         product="sfc",
         save_dir=save_dir,
     )
     ds = H.xarray("TMP:2 m", remove_grib=False)
```

### Comparing `herbie-data-2024.3.1/tests/test_init.py` & `herbie_data-2024.5.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `herbie-data-2024.3.1/tests/test_rap.py` & `herbie_data-2024.5.0/tests/test_rap.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 ## Brian Blaylock
 ## October 13, 2021
 
-"""
-Tests for downloading RAP model
-"""
+"""Tests for downloading RAP model."""
+
 import pandas as pd
 import pytest
 
-from herbie import Herbie
+from herbie import Herbie, config
 from tests.util import is_time_between
 
 today = pd.to_datetime("today").floor("1D") - pd.to_timedelta("1D")
-save_dir = "$TMPDIR/Herbie-Tests/"
+save_dir = config["default"]["save_dir"] / "Herbie-Tests-Data/"
+
+# Remove all previous test data
+for i in (save_dir / "rap").rglob("*"):
+    if i.is_file():
+        i.unlink()
 
 
 @pytest.mark.skipif(
     is_time_between("00:00", "02:30"),
     reason="Test hibernated between 00:00 and 02:30 UTC, "
     "because upstream data not available or incomplete at night.",
 )
 def test_rap_aws():
     # Test
-    H = Herbie(
-        today,
-        model="rap",
-        save_dir=save_dir,
-    )
+    H = Herbie(today, model="rap", save_dir=save_dir, overwrite=True)
     assert H.grib is not None
 
     # Test downloading the file
     H = Herbie(
         today,
         model="rap",
         save_dir=save_dir,
@@ -38,15 +38,15 @@
     assert H.get_localFilePath().exists()
 
     H.xarray("TMP:2 m", remove_grib=False)
     assert H.get_localFilePath("TMP:2 m").exists()
 
 
 def test_rap_historical():
-    """Search for RAP urls on NCEI that I know exist"""
+    """Search for RAP urls on NCEI that I know exist."""
 
     H = Herbie(
         "2019-11-23",
         model="rap_historical",
         product="analysis",
         save_dir=save_dir,
     )
```

### Comparing `herbie-data-2024.3.1/tests/util.py` & `herbie_data-2024.5.0/tests/util.py`

 * *Files identical despite different names*

