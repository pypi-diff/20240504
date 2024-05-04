# Comparing `tmp/requake-0.5.tar.gz` & `tmp/requake-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requake-0.5.tar", last modified: Tue Apr 23 07:53:32 2024, max compression
+gzip compressed data, was "requake-0.6.tar", last modified: Sat May  4 15:24:05 2024, max compression
```

## Comparing `requake-0.5.tar` & `requake-0.6.tar`

### file list

```diff
@@ -1,69 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:53:32.114781 requake-0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-23 07:53:29.000000 requake-0.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-23 07:53:29.000000 requake-0.5/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-23 07:53:29.000000 requake-0.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-23 07:53:29.000000 requake-0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7740 2024-04-23 07:53:32.114781 requake-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6358 2024-04-23 07:53:29.000000 requake-0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:53:32.114781 requake-0.5/requake/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-23 07:53:29.000000 requake-0.5/requake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-23 07:53:32.114781 requake-0.5/requake/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:53:32.110781 requake-0.5/requake/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-23 07:53:29.000000 requake-0.5/requake/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10387 2024-04-23 07:53:29.000000 requake-0.5/requake/catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-04-23 07:53:29.000000 requake-0.5/requake/catalog/read_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-04-23 07:53:29.000000 requake-0.5/requake/catalog/read_catalog_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-04-23 07:53:29.000000 requake-0.5/requake/catalog/read_catalog_from_fdsnws.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-23 07:53:29.000000 requake-0.5/requake/catalog/read_catalog_from_quakeml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:53:32.110781 requake-0.5/requake/config/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-23 07:53:29.000000 requake-0.5/requake/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-23 07:53:29.000000 requake-0.5/requake/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:53:32.110781 requake-0.5/requake/config/configobj/
--rw-r--r--   0 runner    (1001) docker     (127)    88030 2024-04-23 07:53:29.000000 requake-0.5/requake/config/configobj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 07:53:29.000000 requake-0.5/requake/config/configobj/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    46990 2024-04-23 07:53:29.000000 requake-0.5/requake/config/configobj/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-04-23 07:53:29.000000 requake-0.5/requake/config/configspec.conf
--rw-r--r--   0 runner    (1001) docker     (127)    10513 2024-04-23 07:53:29.000000 requake-0.5/requake/config/parse_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     9080 2024-04-23 07:53:29.000000 requake-0.5/requake/config/rq_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-04-23 07:53:29.000000 requake-0.5/requake/config/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:53:32.110781 requake-0.5/requake/families/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-23 07:53:29.000000 requake-0.5/requake/families/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8141 2024-04-23 07:53:29.000000 requake-0.5/requake/families/build_families.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-23 07:53:29.000000 requake-0.5/requake/families/build_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-23 07:53:29.000000 requake-0.5/requake/families/families.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-23 07:53:29.000000 requake-0.5/requake/families/flag_family.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-23 07:53:29.000000 requake-0.5/requake/families/print_families.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:53:32.114781 requake-0.5/requake/formulas/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-23 07:53:29.000000 requake-0.5/requake/formulas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-23 07:53:29.000000 requake-0.5/requake/formulas/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-23 07:53:29.000000 requake-0.5/requake/formulas/slip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-23 07:53:29.000000 requake-0.5/requake/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:53:32.114781 requake-0.5/requake/plot/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-23 07:53:29.000000 requake-0.5/requake/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-23 07:53:29.000000 requake-0.5/requake/plot/cached_tiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-04-23 07:53:29.000000 requake-0.5/requake/plot/map_families.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-23 07:53:29.000000 requake-0.5/requake/plot/map_tiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-04-23 07:53:29.000000 requake-0.5/requake/plot/plot_families.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-23 07:53:29.000000 requake-0.5/requake/plot/plot_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-04-23 07:53:29.000000 requake-0.5/requake/plot/plot_slip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-23 07:53:29.000000 requake-0.5/requake/plot/plot_timespans.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-23 07:53:29.000000 requake-0.5/requake/plot/plot_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:53:32.114781 requake-0.5/requake/scan/
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-23 07:53:29.000000 requake-0.5/requake/scan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-23 07:53:29.000000 requake-0.5/requake/scan/scan_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-04-23 07:53:29.000000 requake-0.5/requake/scan/scan_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:53:32.114781 requake-0.5/requake/waveforms/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 07:53:29.000000 requake-0.5/requake/waveforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-23 07:53:29.000000 requake-0.5/requake/waveforms/arrivals.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-23 07:53:29.000000 requake-0.5/requake/waveforms/station_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    10159 2024-04-23 07:53:29.000000 requake-0.5/requake/waveforms/waveforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:53:32.114781 requake-0.5/requake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7740 2024-04-23 07:53:32.000000 requake-0.5/requake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-23 07:53:32.000000 requake-0.5/requake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 07:53:32.000000 requake-0.5/requake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-23 07:53:32.000000 requake-0.5/requake.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-23 07:53:32.000000 requake-0.5/requake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 07:53:32.000000 requake-0.5/requake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-23 07:53:32.114781 requake-0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-23 07:53:29.000000 requake-0.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    70144 2024-04-23 07:53:29.000000 requake-0.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:24:05.030727 requake-0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-04 15:24:01.000000 requake-0.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-04 15:24:01.000000 requake-0.6/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-04 15:24:01.000000 requake-0.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-04 15:24:01.000000 requake-0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-05-04 15:24:05.030727 requake-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-05-04 15:24:01.000000 requake-0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:24:05.030727 requake-0.6/requake/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-04 15:24:01.000000 requake-0.6/requake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-04 15:24:05.030727 requake-0.6/requake/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:24:05.022727 requake-0.6/requake/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-04 15:24:01.000000 requake-0.6/requake/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10477 2024-05-04 15:24:01.000000 requake-0.6/requake/catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-04 15:24:01.000000 requake-0.6/requake/catalog/print_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-04 15:24:01.000000 requake-0.6/requake/catalog/read_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-05-04 15:24:01.000000 requake-0.6/requake/catalog/read_catalog_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-04 15:24:01.000000 requake-0.6/requake/catalog/read_catalog_from_fdsnws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-04 15:24:01.000000 requake-0.6/requake/catalog/read_catalog_from_quakeml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:24:05.026727 requake-0.6/requake/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-04 15:24:01.000000 requake-0.6/requake/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-04 15:24:01.000000 requake-0.6/requake/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:24:05.026727 requake-0.6/requake/config/configobj/
+-rw-r--r--   0 runner    (1001) docker     (127)    88030 2024-05-04 15:24:01.000000 requake-0.6/requake/config/configobj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-04 15:24:01.000000 requake-0.6/requake/config/configobj/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46990 2024-05-04 15:24:01.000000 requake-0.6/requake/config/configobj/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7057 2024-05-04 15:24:01.000000 requake-0.6/requake/config/configspec.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-04 15:24:01.000000 requake-0.6/requake/config/generic_printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12802 2024-05-04 15:24:01.000000 requake-0.6/requake/config/parse_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9686 2024-05-04 15:24:01.000000 requake-0.6/requake/config/rq_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6705 2024-05-04 15:24:01.000000 requake-0.6/requake/config/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:24:05.026727 requake-0.6/requake/families/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-04 15:24:01.000000 requake-0.6/requake/families/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-05-04 15:24:01.000000 requake-0.6/requake/families/build_families.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-04 15:24:01.000000 requake-0.6/requake/families/build_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8955 2024-05-04 15:24:01.000000 requake-0.6/requake/families/families.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-04 15:24:01.000000 requake-0.6/requake/families/flag_family.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-05-04 15:24:01.000000 requake-0.6/requake/families/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-04 15:24:01.000000 requake-0.6/requake/families/print_families.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-04 15:24:01.000000 requake-0.6/requake/families/print_pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:24:05.026727 requake-0.6/requake/formulas/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-04 15:24:01.000000 requake-0.6/requake/formulas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-04 15:24:01.000000 requake-0.6/requake/formulas/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-04 15:24:01.000000 requake-0.6/requake/formulas/moment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-04 15:24:01.000000 requake-0.6/requake/formulas/slip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-04 15:24:01.000000 requake-0.6/requake/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:24:05.030727 requake-0.6/requake/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-04 15:24:01.000000 requake-0.6/requake/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-04 15:24:01.000000 requake-0.6/requake/plot/cached_tiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-05-04 15:24:01.000000 requake-0.6/requake/plot/map_families.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-04 15:24:01.000000 requake-0.6/requake/plot/map_tiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-05-04 15:24:01.000000 requake-0.6/requake/plot/plot_cumulative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-05-04 15:24:01.000000 requake-0.6/requake/plot/plot_families.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-04 15:24:01.000000 requake-0.6/requake/plot/plot_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-05-04 15:24:01.000000 requake-0.6/requake/plot/plot_timespans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-05-04 15:24:01.000000 requake-0.6/requake/plot/plot_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:24:05.030727 requake-0.6/requake/scan/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-04 15:24:01.000000 requake-0.6/requake/scan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-04 15:24:01.000000 requake-0.6/requake/scan/scan_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-05-04 15:24:01.000000 requake-0.6/requake/scan/scan_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:24:05.030727 requake-0.6/requake/waveforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-04 15:24:01.000000 requake-0.6/requake/waveforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-04 15:24:01.000000 requake-0.6/requake/waveforms/arrivals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-04 15:24:01.000000 requake-0.6/requake/waveforms/station_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10159 2024-05-04 15:24:01.000000 requake-0.6/requake/waveforms/waveforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:24:05.030727 requake-0.6/requake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-05-04 15:24:05.000000 requake-0.6/requake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-04 15:24:05.000000 requake-0.6/requake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 15:24:05.000000 requake-0.6/requake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-04 15:24:05.000000 requake-0.6/requake.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-04 15:24:05.000000 requake-0.6/requake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 15:24:05.000000 requake-0.6/requake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-04 15:24:05.030727 requake-0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-04 15:24:01.000000 requake-0.6/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70144 2024-05-04 15:24:01.000000 requake-0.6/versioneer.py
```

### Comparing `requake-0.5/LICENSE.txt` & `requake-0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `requake-0.5/PKG-INFO` & `requake-0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requake
-Version: 0.5
+Version: 0.6
 Summary: Repeating earthquakes search and analysis
 Home-page: https://requake.seismicsource.org
 Author: Claudio Satriano
 Author-email: satriano@ipgp.fr
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Homepage, https://requake.seismicsource.org
 Project-URL: Source, https://github.com/SeismicSource/requake
@@ -29,15 +29,15 @@
 License-File: LICENSE.txt
 Requires-Dist: scipy>=1.5.0
 Requires-Dist: obspy>=1.2.0
 Requires-Dist: argcomplete
 Requires-Dist: tqdm
 Requires-Dist: tabulate
 
-<img src="imgs/Requake_logo.svg" width="400">
+<img src="https://cdn.jsdelivr.net/gh/SeismicSource/requake@dc9a6e6fd818e57e0c0d74f9c16f2bfc6d4d148c/imgs/Requake_logo.svg" width="400">
 
 # Requake
 
 Repeating earthquakes search and analysis.
 
 [![changelog-badge]][changelog-link]
 [![PyPI-badge]][PyPI-link]
@@ -118,41 +118,42 @@
 
 Requake is based on a single executable, aptly named `requake` 😉.
 
 To get help, use:
 
     requake -h
 
-The different running modes are specified as "verbs" (positional arguments).
-Currently supported verbs are:
+Different commands are available:
 
     sample_config       write sample config file to current directory and exit
+    update_config       update an existing config file to the latest version
     read_catalog        read an event catalog from web services or from a file
+    print_catalog       print the event catalog to screen
     scan_catalog        scan an existing catalog for earthquake pairs
+    print_pairs         print pairs to screen
     plot_pair           plot traces for a given event pair
     build_families      build families of repeating earthquakes from a catalog
                         of pairs
     print_families      print families to screen
     plot_families       plot traces for one ore more event families
     plot_timespans      plot family timespans
-    plot_slip           plot cumulative slip for one or more families
+    plot_cumulative     cumulative plot for one or more families
     map_families        plot families on a map
     flag_family         flag a family of repeating earthquakes as valid or not
-                        valid. Note that all families are valid by default
-                        when first created
+                        valid.
     build_templates     build waveform templates for one or more event
                         families
     scan_templates      scan a continuous waveform stream using one or more
                         templates
 
-Certain running modes (e.g., `plot_pair`) require further arguments (use, e.g.,
+Certain commands (e.g., `plot_pair`) require further arguments (use, e.g.,
 `requake plot_pair -h` to get help).
 
-Requake supports command line tab completion for arguments, thanks to
-[argcomplete](https://kislyuk.github.io/argcomplete/).
+Requake supports command line tab completion for commands and arguments, thanks
+to [argcomplete](https://kislyuk.github.io/argcomplete/).
 To enable command line tab completion, add the following line to your `.bashrc`
 or `.zshrc`:
 
     eval "$(register-python-argcomplete requake)"
 
 ### Typical workflow
```

### Comparing `requake-0.5/README.md` & `requake-0.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -83,41 +83,42 @@
 
 Requake is based on a single executable, aptly named `requake` 😉.
 
 To get help, use:
 
     requake -h
 
-The different running modes are specified as "verbs" (positional arguments).
-Currently supported verbs are:
+Different commands are available:
 
     sample_config       write sample config file to current directory and exit
+    update_config       update an existing config file to the latest version
     read_catalog        read an event catalog from web services or from a file
+    print_catalog       print the event catalog to screen
     scan_catalog        scan an existing catalog for earthquake pairs
+    print_pairs         print pairs to screen
     plot_pair           plot traces for a given event pair
     build_families      build families of repeating earthquakes from a catalog
                         of pairs
     print_families      print families to screen
     plot_families       plot traces for one ore more event families
     plot_timespans      plot family timespans
-    plot_slip           plot cumulative slip for one or more families
+    plot_cumulative     cumulative plot for one or more families
     map_families        plot families on a map
     flag_family         flag a family of repeating earthquakes as valid or not
-                        valid. Note that all families are valid by default
-                        when first created
+                        valid.
     build_templates     build waveform templates for one or more event
                         families
     scan_templates      scan a continuous waveform stream using one or more
                         templates
 
-Certain running modes (e.g., `plot_pair`) require further arguments (use, e.g.,
+Certain commands (e.g., `plot_pair`) require further arguments (use, e.g.,
 `requake plot_pair -h` to get help).
 
-Requake supports command line tab completion for arguments, thanks to
-[argcomplete](https://kislyuk.github.io/argcomplete/).
+Requake supports command line tab completion for commands and arguments, thanks
+to [argcomplete](https://kislyuk.github.io/argcomplete/).
 To enable command line tab completion, add the following line to your `.bashrc`
 or `.zshrc`:
 
     eval "$(register-python-argcomplete requake)"
 
 ### Typical workflow
```

### Comparing `requake-0.5/requake/catalog/catalog.py` & `requake-0.6/requake/catalog/catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,18 +260,21 @@
 
     :raises ValueError: if error reading catalog file
     :raises FileNotFoundError: if catalog file not found
     """
     try:
         cat = RequakeCatalog()
         cat.read(config.scan_catalog_file)
+        cat.sort()
+        if not cat:
+            raise ValueError('Empty catalog')
         return cat
     except ValueError as m:
         raise ValueError(
-            f'Error reading catalog file {config.scan_catalog_file}'
+            f'Error reading catalog file {config.scan_catalog_file}: {m}'
         ) from m
     except FileNotFoundError as m:
         raise FileNotFoundError(
             f'Catalog file {config.scan_catalog_file} not found'
         ) from m
```

### Comparing `requake-0.5/requake/catalog/read_catalog.py` & `requake-0.6/requake/catalog/read_catalog.py`

 * *Files identical despite different names*

### Comparing `requake-0.5/requake/catalog/read_catalog_from_csv.py` & `requake-0.6/requake/catalog/read_catalog_from_csv.py`

 * *Files identical despite different names*

### Comparing `requake-0.5/requake/catalog/read_catalog_from_fdsnws.py` & `requake-0.6/requake/catalog/read_catalog_from_fdsnws.py`

 * *Files identical despite different names*

### Comparing `requake-0.5/requake/catalog/read_catalog_from_quakeml.py` & `requake-0.6/requake/catalog/read_catalog_from_quakeml.py`

 * *Files identical despite different names*

### Comparing `requake-0.5/requake/config/config.py` & `requake-0.6/requake/config/config.py`

 * *Files identical despite different names*

### Comparing `requake-0.5/requake/config/configobj/__init__.py` & `requake-0.6/requake/config/configobj/__init__.py`

 * *Files identical despite different names*

### Comparing `requake-0.5/requake/config/configobj/validate.py` & `requake-0.6/requake/config/configobj/validate.py`

 * *Files identical despite different names*

### Comparing `requake-0.5/requake/config/configspec.conf` & `requake-0.6/requake/config/configspec.conf`

 * *Files 4% similar despite different names*

```diff
@@ -124,7 +124,23 @@
 distance_from_lat = float(default=None)
 ## Templates are built by averaging the traces in the family.
 ## Set the following paramter to True if you want to normalize the traces
 ## before averaging.
 ## Normalization will produce an average trace which is more representative
 ## of the family, but will be less effective in reducing noise.
 normalize_traces_before_averaging = boolean(default=False)
+
+#### Post-processing parameters
+## Estimation of fault slip (in cm) from repetater's magnitude
+## Choose between:
+##  NJ1998 : Nadeau and Johnson (1998)
+##  B2001 : Beeler et al. (2001)
+##  E1957 : Eshelby (1957), circular crack model
+## See Uchida (2019, https://doi.org/10.1186/s40645-019-0284-z) for details
+## on the models.
+mag_to_slip_model = string(default='NJ1998')
+## Static stress drop value for B2001 and E1957 models (MPa)
+static_stress_drop = float(default=10.0)
+## Rigidity value for B2001 and E1957 models (GPa)
+rigidity = float(default=30.0)
+## Strain hardening coefficient for B2001 model (MPa/cm)
+strain_hardening = float(default=0.5)
```

### Comparing `requake-0.5/requake/config/parse_arguments.py` & `requake-0.6/requake/config/parse_arguments.py`

 * *Files 19% similar despite different names*

```diff
@@ -30,27 +30,48 @@
                 lines.extend(wrap_lines)
             else:
                 # For lines that are short enough, just add them as they are
                 lines.append(line)
         return lines
 
 
+class SubcommandHelpFormatter(argparse.RawDescriptionHelpFormatter):
+    """
+    Custom help formatter that removes the list of subcommands from the help
+    message.
+
+    See: https://stackoverflow.com/a/13429281/2021880
+    """
+    def _format_action(self, action):
+        parts = super(
+            argparse.RawDescriptionHelpFormatter, self
+        )._format_action(action)
+        if action.nargs == argparse.PARSER:
+            parts = '\n'.join(parts.split('\n')[1:])
+        return parts
+
+
 def parse_arguments(progname='requake'):
     """
     Parse command line arguments.
 
     :param progname: Program name (default: "requake").
     :type progname: str
     :return: Parsed arguments.
     :rtype: argparse.Namespace
     """
     parser = argparse.ArgumentParser(
-        description=f'{progname}: Repeating earthquakes search and analysis.'
+        description=f'{progname}: Repeating earthquakes search and analysis.',
+        epilog='Use "%(prog)s <command> -h" for help on a specific command\n'
+               '(example: "%(prog)s read_catalog -h").\n'
+               '\nFull documentation at https://requake.readthedocs.io',
+        formatter_class=SubcommandHelpFormatter
     )
-    subparser = parser.add_subparsers(dest='action')
+    subparser = parser.add_subparsers(dest='action', title='commands')
+    subparser.metavar = '<command> [options]'
     parser.add_argument(
         '-c',
         '--configfile',
         type=str,
         default=f'{progname}.conf',
         help=f'config file (default: {progname}.conf)',
     )
@@ -69,14 +90,24 @@
     )
     # --- sample_config
     subparser.add_parser(
         'sample_config',
         help='write sample config file to current directory and exit'
     )
     # ---
+    # --- update_config
+    updateconfig = subparser.add_parser(
+        'update_config',
+        help='update an existing config file to the latest version'
+    )
+    updateconfig.add_argument(
+        'config_file', default='requake.conf', nargs='?',
+        help='config file to be updated (default: %(default)s)'
+    )
+    # ---
     # --- read catalog
     readcatalog = subparser.add_parser(
         'read_catalog',
         help='read an event catalog from web services or from a file',
         formatter_class=NewlineHelpFormatter
     )
     readcatalog.add_argument(
@@ -99,21 +130,54 @@
             'the code will exit with an error.'
         )
     )
     readcatalog.add_argument(
         '-a', '--append', action='store_true',
         help='append events to existing catalog'
     )
+    # --- printformat
+    #     a parent parser for the "format" option,
+    #     used by the "print" subparsers
+    printformat = argparse.ArgumentParser(add_help=False)
+    printformat.add_argument(
+        '-f', '--format', type=str, default='simple',
+        choices=['simple', 'markdown', 'csv'],
+        help='format for the output table (default: %(default)s)'
+    )
+    # ---
+    # --- print_catalog
+    subparser.add_parser(
+        'print_catalog',
+        parents=[printformat],
+        help='print the event catalog to screen'
+    )
     # ---
     # --- scan_catalog
     subparser.add_parser(
         'scan_catalog',
         help='scan an existing catalog for earthquake pairs'
     )
     # ---
+    # --- print_pairs
+    printpairs = subparser.add_parser(
+        'print_pairs',
+        parents=[printformat],
+        help='print pairs to screen'
+    )
+    printpairs.add_argument(
+        '-c', '--cc_min',
+        type=float, default=None,
+        help='minimum cross-correlation coefficient (default: %(default)s)'
+    )
+    printpairs.add_argument(
+        '-C', '--cc_max',
+        type=float, default=None,
+        help='maximum cross-correlation coefficient (default: %(default)s)'
+    )
+    # ---
     # --- plot_pair
     plotpair = subparser.add_parser(
         'plot_pair',
         help='plot traces for a given event pair'
     )
     plotpair.add_argument('evid1')
     plotpair.add_argument('evid2')
@@ -162,24 +226,19 @@
     traceid = argparse.ArgumentParser(add_help=False)
     traceid.add_argument(
         '-t', '--traceid', type=str, default=None,
         help='use this traceid instead of the default one for the family'
     )
     # ---
     # --- print_families
-    printfamilies = subparser.add_parser(
+    subparser.add_parser(
         'print_families',
-        parents=[longerthan, minevents, familynumbers],
+        parents=[longerthan, minevents, familynumbers, printformat],
         help='print families to screen'
     )
-    printfamilies.add_argument(
-        '-f', '--format', type=str, default='simple',
-        choices=['simple', 'markdown', 'csv'],
-        help='format for the output table (default: %(default)s)'
-    )
     # ---
     # --- plot_families
     plotfamilies = subparser.add_parser(
         'plot_families',
         parents=[longerthan, minevents, familynumbers, traceid],
         help='plot traces for one ore more event families'
     )
@@ -203,19 +262,28 @@
         choices=[
             'time', 'latitude', 'longitude', 'depth', 'distance_from',
             'family_number'
         ],
         help='quantity to sort families by on y-axis (default: %(default)s)'
     )
     # ---
-    # --- plot_slip
-    subparser.add_parser(
-        'plot_slip',
+    # --- plot_cumulative
+    plotcumulative = subparser.add_parser(
+        'plot_cumulative',
         parents=[longerthan, minevents, familynumbers],
-        help='plot cumulative slip for one or more families'
+        help='cumulative plot for one or more families'
+    )
+    plotcumulative.add_argument(
+        '-q', '--quantity', type=str, default='slip',
+        choices=['slip', 'moment', 'number'],
+        help='cumulative quantity to plot on y-axis (default: %(default)s)'
+    )
+    plotcumulative.add_argument(
+        '-L', '--logscale', action='store_true',
+        help='use log scale for y-axis'
     )
     # ---
     # --- map_families
     mapfamilies = subparser.add_parser(
         'map_families',
         parents=[longerthan, minevents, familynumbers],
         help='plot families on a map'
@@ -238,16 +306,15 @@
         help='zoom level for the map tiles (default: None). Note that '
              'certain map tiles might not be available at all zoom levels'
     )
     # ---
     # --- flag_family
     flagfamily = subparser.add_parser(
         'flag_family',
-        help='flag a family of repeating earthquakes as valid or not valid. '
-             'Note that all families are valid by default when first created'
+        help='flag a family of repeating earthquakes as valid or not valid'
     )
     flagfamily.add_argument('family_number')
     flagfamily.add_argument(
         'is_valid',
         help='"true" (or "t") to flag family as valid, '
              '"false" (or "f") to flag family as not valid'
     )
```

### Comparing `requake-0.5/requake/config/rq_setup.py` & `requake-0.6/requake/config/rq_setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from obspy.clients.filesystem.sds import Client as SDSClient
 from obspy.clients.fdsn import Client as FDSNClient
 from obspy.clients.fdsn.header import FDSNNoServiceException
 from .._version import get_versions
 from .config import Config
 from .utils import (
     parse_configspec, read_config, validate_config, write_sample_config,
-    write_ok
+    update_config_file, write_ok
 )
 # pylint: disable=global-statement,import-outside-toplevel
 
 logger = None  # pylint: disable=invalid-name
 PYTHON_VERSION_STR = None
 NUMPY_VERSION_STR = None
 SCIPY_VERSION_STR = None
@@ -46,14 +46,28 @@
     global SCIPY_VERSION_STR
     SCIPY_VERSION_STR = scipy.__version__
     import obspy
     global OBSPY_VERSION_STR
     OBSPY_VERSION_STR = obspy.__version__
 
 
+def _make_outdir(outdir):
+    """Create the output directory if it doesn't exist."""
+    if not os.path.exists(outdir):
+        os.makedirs(outdir)
+    readme = os.path.join(outdir, 'README.txt')
+    if not os.path.exists(readme):
+        with open(readme, 'w', encoding='utf8') as fp:
+            fp.write('This is the Requake output directory.\n\n')
+            fp.write('''\
+Do not manually edit the files in this directory, unless you know what you
+are doing.
+''')
+
+
 def _setup_logging(config, progname, action_name):
     """Set up the logging infrastructure."""
     global logger
 
     logger_root = logging.getLogger()
     # captureWarnings is not supported in old versions of python
     with contextlib.suppress(Exception):
@@ -64,16 +78,15 @@
     logging_actions = [
         'read_catalog',
         'scan_catalog',
         'scan_templates',
         'build_families'
     ]
     if action_name in logging_actions:
-        if not os.path.exists(config.args.outdir):
-            os.makedirs(config.args.outdir)
+        _make_outdir(config.args.outdir)
         logfile = os.path.join(
             config.args.outdir, f'{progname}.{action_name}.log')
         filehand = logging.FileHandler(filename=logfile, mode='a')
         filehand.setLevel(logging.DEBUG)
         formatter = logging.Formatter('%(asctime)s %(name)-20s '
                                       '%(levelname)-8s %(message)s')
         filehand.setFormatter(formatter)
@@ -186,14 +199,17 @@
 
 def configure(args):
     """Read command line arguments. Read config file. Set up logging."""
     configspec = parse_configspec()
     if args.action == 'sample_config':
         write_sample_config(configspec, 'requake')
         sys.exit(0)
+    if args.action == 'update_config':
+        update_config_file(args.configfile, configspec)
+        sys.exit(0)
     config_obj = read_config(args.configfile, configspec)
     # Set to None all the 'None' strings
     for key, value in config_obj.dict().items():
         if value == 'None':
             config_obj[key] = None
     validate_config(config_obj)
     # Create a config class
@@ -257,16 +273,17 @@
     return config
 
 
 def rq_exit(retval=0, abort=False, progname='requake'):
     """Exit as gracefully as possible."""
     if abort:
         print('\nAborting.')
-        logger.debug(f'{progname} ABORTED\n\n')
-    else:
+        if logger is not None:
+            logger.debug(f'{progname} ABORTED\n\n')
+    elif logger is not None:
         logger.debug(f'{progname} END\n\n')
     logging.shutdown()
     sys.exit(retval)
 
 
 def sigint_handler(_sig, _frame):
     """Abort gracefully."""
```

### Comparing `requake-0.5/requake/config/utils.py` & `requake-0.6/requake/config/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 :license:
     GNU General Public License v3.0 or later
     (https://www.gnu.org/licenses/gpl-3.0-standalone.html)
 """
 import os
 import sys
 import locale
-import traceback
-from .. import __version__
+import shutil
+from datetime import datetime
 from .configobj import ConfigObj
 from .configobj.validate import Validator
 locale.setlocale(locale.LC_ALL, '')
 
 
 def err_exit(msg):
     """
@@ -129,21 +129,75 @@
                 sys.stderr.write(
                     f'Invalid value for "{entry}": "{config_obj[entry]}"\n')
         sys.exit(1)
     if not test:
         err_exit('No configuration value present!')
 
 
+def update_config_file(config_file, configspec):
+    """
+    Update a configuration file to the latest version.
+
+    :param config_file: Configuration file.
+    :type config_file: str
+    :param configspec: Configuration specification file.
+    :type configspec: str
+    """
+    config_obj = read_config(config_file, configspec)
+    val = Validator()
+    config_obj.validate(val)
+    mod_time = datetime.fromtimestamp(os.path.getmtime(config_file))
+    mod_time_str = mod_time.strftime('%Y%m%d_%H%M%S')
+    config_file_old = f'{config_file}.{mod_time_str}'
+    ans = input(
+        f'Ok to update {config_file}? [y/N]\n'
+        f'(Old file will be saved as {config_file_old}) '
+    )
+    if ans not in ['y', 'Y']:
+        sys.exit(0)
+    config_new = ConfigObj(configspec=configspec, default_encoding='utf8')
+    config_new = read_config(None, configspec)
+    config_new.validate(val)
+    config_new.defaults = []
+    config_new.comments = configspec.comments
+    config_new.initial_comment = config_obj.initial_comment
+    config_new.final_comment = configspec.final_comment
+    for k, v in config_obj.items():
+        if k not in config_new:
+            continue
+        # Fix for force_list(default=None)
+        if v == ['None', ]:
+            v = None
+        config_new[k] = v
+    migrate_options = {
+        # 'old_option': 'new_option'
+    }
+    for old_opt, new_opt in migrate_options.items():
+        if old_opt in config_obj and config_obj[old_opt] != 'None':
+            config_new[new_opt] = config_obj[old_opt]
+    shutil.copyfile(config_file, config_file_old)
+    with open(config_file, 'wb') as fp:
+        config_new.write(fp)
+        print(f'{config_file}: updated')
+
+
 def manage_uncaught_exception(exception):
     """
     Manage an uncaught exception.
 
     :param exception: Exception object.
     :type exception: Exception
     """
+    # pylint: disable=import-outside-toplevel
+    from .. import __version__
+    import traceback
+    import numpy as np
+    import scipy as sp
+    import obspy
+    import matplotlib
     sys.stderr.write("""
 # BEGIN TRACEBACK #############################################################
 """)
     sys.stderr.write('\n')
     traceback.print_exc()
     sys.stderr.write("""
 # END TRACEBACK ###############################################################
@@ -156,14 +210,18 @@
 or by email to satriano@ipgp.fr.
 
 Include the following information in your report:
 
 """)
     sys.stderr.write(f'  Requake version: {__version__}\n')
     sys.stderr.write(f'  Python version: {sys.version}\n')
+    sys.stderr.write(f'  NumPy version: {np.__version__}\n')
+    sys.stderr.write(f'  SciPy version: {sp.__version__}\n')
+    sys.stderr.write(f'  ObsPy version: {obspy.__version__}\n')
+    sys.stderr.write(f'  Matplotlib version: {matplotlib.__version__}\n')
     sys.stderr.write(f'  Platform: {sys.platform}\n')
     sys.stderr.write(f'  Command line: {" ".join(sys.argv)}\n')
     sys.stderr.write(f'  Error message: {str(exception)}\n')
     sys.stderr.write('\n')
     sys.stderr.write(
         'Also, please copy and paste the traceback above in your '
         'report.\n\n')
```

### Comparing `requake-0.5/requake/families/__init__.py` & `requake-0.6/requake/families/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,11 +6,12 @@
 
 :copyright:
     2021-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     GNU General Public License v3.0 or later
     (https://www.gnu.org/licenses/gpl-3.0-standalone.html)
 """
+from .print_pairs import print_pairs  # noqa
 from .build_families import build_families  # noqa
 from .print_families import print_families  # noqa
 from .flag_family import flag_family  # noqa
 from .build_templates import build_templates  # noqa
```

### Comparing `requake-0.5/requake/families/build_families.py` & `requake-0.6/requake/families/build_families.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,17 +9,15 @@
     GNU General Public License v3.0 or later
     (https://www.gnu.org/licenses/gpl-3.0-standalone.html)
 """
 import logging
 import csv
 from itertools import combinations
 from scipy.cluster.hierarchy import average, fcluster
-from obspy import UTCDateTime
-from ..formulas.conversion import float_or_none
-from ..catalog.catalog import RequakeEvent
+from .pairs import read_events_from_pairs_file
 from .families import Family
 from ..config.rq_setup import rq_exit
 logger = logging.getLogger(__name__.rsplit('.', maxsplit=1)[-1])
 
 
 def _check_options(config):
     """
@@ -35,65 +33,14 @@
     if sort_by == 'distance_from' and (lon0 is None or lat0 is None):
         raise ValueError(
             '"sort_families_by" set to "distance_from", '
             'but "distance_from_lon" and/or "distance_from_lat" '
             'are not specified')
 
 
-def _read_events_from_pairs_file(config):
-    """
-    Read events from pairs file.
-
-    :param config: configuration object
-    :type config: config.Config
-    :return: dictionary of events
-    :rtype: dict
-
-    :raises FileNotFoundError: if the pairs file is not found
-    """
-    events = {}
-    with open(config.scan_catalog_pairs_file, 'r', encoding='utf8') as fp:
-        reader = csv.DictReader(fp)
-        for row in reader:
-            cc_max = float(row['cc_max'])
-            evid1 = row['evid1']
-            try:
-                ev1 = events[evid1]
-            except KeyError:
-                ev1 = RequakeEvent(
-                    evid=evid1,
-                    orig_time=UTCDateTime(row['orig_time1']),
-                    lon=float_or_none(row['lon1']),
-                    lat=float_or_none(row['lat1']),
-                    depth=float_or_none(row['depth_km1']),
-                    mag_type=row['mag_type1'],
-                    mag=float_or_none(row['mag1']),
-                    trace_id=row['trace_id']
-                )
-                events[evid1] = ev1
-            evid2 = row['evid2']
-            try:
-                ev2 = events[evid2]
-            except KeyError:
-                ev2 = RequakeEvent(
-                    evid=evid2,
-                    orig_time=UTCDateTime(row['orig_time2']),
-                    lon=float_or_none(row['lon2']),
-                    lat=float_or_none(row['lat2']),
-                    depth=float_or_none(row['depth_km2']),
-                    mag_type=row['mag_type2'],
-                    mag=float_or_none(row['mag2']),
-                    trace_id=row['trace_id']
-                )
-                events[evid2] = ev2
-            # Store the correlation between the two events in both events
-            ev1.correlations[ev2.evid] = ev2.correlations[ev1.evid] = cc_max
-    return events
-
-
 def _build_families_from_shared_events(events, cc_min):
     """
     Build families by clustering all event pairs sharing an event.
 
     Valid event pairs are those with a correlation above cc_min.
 
     :param events: dictionary of events
@@ -210,15 +157,15 @@
     try:
         _check_options(config)
     except ValueError as e:
         logger.error(e)
         rq_exit(1)
     try:
         logger.info('Reading events from pairs file...')
-        events = _read_events_from_pairs_file(config)
+        events = read_events_from_pairs_file(config)
     except FileNotFoundError:
         logger.error(
             'Unable to find event pairs file: '
             f'{config.scan_catalog_pairs_file}'
         )
         rq_exit(1)
     if config.clustering_algorithm == 'shared':
```

### Comparing `requake-0.5/requake/families/build_templates.py` & `requake-0.6/requake/families/build_templates.py`

 * *Files identical despite different names*

### Comparing `requake-0.5/requake/families/families.py` & `requake-0.6/requake/families/families.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,23 +32,26 @@
     def __init__(self, number=-1):
         self.lon = None
         self.lat = None
         self.depth = None  # km
         self.starttime = None
         self.endtime = None
         self.duration = None  # years
+        self.magmin = None
+        self.magmax = None
         self.number = number
         self.valid = True
         self.trace_id = None
 
     def __str__(self):
         return (
             f'{self.number:2d} {len(self):2d} '
             f'{self.lon:8.4f} {self.lat:8.4f} {self.depth:7.3f} '
             f'{self.starttime} {self.endtime} {self.duration:4.1f} '
+            f'{self.magmin:3.1f} {self.magmax:3.1f} '
             f'{self.valid}'
         )
 
     def append(self, ev):
         """
         Append an event to the family and update family attributes.
 
@@ -66,18 +69,23 @@
         elif ev.trace_id != self.trace_id:
             raise ValueError('Event trace_id does not match family trace_id')
         super().append(ev)
         self.sort()
         self.lon = np.mean([e.lon for e in self])
         self.lat = np.mean([e.lat for e in self])
         self.depth = np.mean([e.depth for e in self])
-        self.starttime = np.min([e.orig_time for e in self])
-        self.endtime = np.max([e.orig_time for e in self])
+        self.starttime = min(ev.orig_time, self.starttime)\
+            if self.starttime else ev.orig_time
+        self.endtime = max(ev.orig_time, self.endtime)\
+            if self.endtime else ev.orig_time
         year = 365*24*60*60
         self.duration = (self.endtime - self.starttime)/year
+        if ev.mag is not None:
+            self.magmin = min(ev.mag, self.magmin) if self.magmin else ev.mag
+            self.magmax = max(ev.mag, self.magmax) if self.magmax else ev.mag
 
     def extend(self, ev_list):
         """
         Extend the family with a list of events.
 
         Events already in the family are not added.
 
@@ -132,15 +140,16 @@
                     families.append(family)
                 family = Family()
                 family.number = family_number
                 old_family_number = family_number
             family.append(ev)
             family.valid = row['valid'] in ['True', 'true']
         # append last family
-        families.append(family)
+        if family is not None:
+            families.append(family)
     return families
 
 
 def read_selected_families(config):
     """
     Read and select families based on family number, validity, length
     and number of events.
```

### Comparing `requake-0.5/requake/families/flag_family.py` & `requake-0.6/requake/families/flag_family.py`

 * *Files identical despite different names*

### Comparing `requake-0.5/requake/families/print_families.py` & `requake-0.6/requake/families/print_families.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,20 +5,18 @@
 
 :copyright:
     2021-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     GNU General Public License v3.0 or later
     (https://www.gnu.org/licenses/gpl-3.0-standalone.html)
 """
-import sys
-import csv
 import logging
 import numpy as np
-from tabulate import tabulate
 from .families import FamilyNotFoundError, read_selected_families
+from ..config.generic_printer import generic_printer
 from ..config.rq_setup import rq_exit
 from ..formulas.slip import mag_to_slip_in_cm
 logger = logging.getLogger(__name__.rsplit('.', maxsplit=1)[-1])
 
 
 def print_families(config):
     """
@@ -34,71 +32,51 @@
         rq_exit(1)
 
     # determine duration units
     average_duration = np.mean([f.duration for f in families])
     avg_duration_in_days = average_duration * 365
     if 30 < avg_duration_in_days < 365:
         duration_multiplier = 12
-        duration_units = 'm'
+        duration_units = 'mons'
     elif 1 < avg_duration_in_days < 30:
         duration_multiplier = 365
-        duration_units = 'd'
+        duration_units = 'days'
     elif avg_duration_in_days < 1:
         duration_multiplier = 365 * 24
-        duration_units = 'h'
+        duration_units = 'hours'
 
-    headers = [
-        'family',
-        'nevents',
-        'longitude',
-        'latitude',
-        'depth (km)',
-        'start time',
-        'end time',
-        f'duration ({duration_units})',
-        'slip rate (cm/y)'
+    headers_fmt = [
+        ('family', None),
+        ('nevents', None),
+        ('longitude', '.4f'),
+        ('latitude', '.4f'),
+        ('depth\n(km)', '.3f'),
+        ('start time', None),
+        ('end time', None),
+        (f'duration\n({duration_units})', '.2f'),
+        ('slip rate\n(cm/y)', '.1f'),
+        ('mag\nmin', '.1f'),
+        ('mag\nmax', '.1f')
     ]
-    table = []
-    tablefmt = config.args.format
-    if tablefmt == 'csv':
-        writer = csv.writer(sys.stdout)
-        writer.writerow(headers)
+    rows = []
     for family in families:
         row = [
             family.number,
             len(family),
             family.lon,
             family.lat,
             family.depth,
             family.starttime,
             family.endtime,
-            family.duration*duration_multiplier
+            family.duration*duration_multiplier,
         ]
-        slip = [mag_to_slip_in_cm(config, ev.mag) for ev in family]
+        try:
+            slip = [mag_to_slip_in_cm(config, ev.mag) for ev in family]
+        except ValueError as msg:
+            logger.error(msg)
+            rq_exit(1)
         cum_slip = np.cumsum(slip)
         d_slip = cum_slip[-1] - cum_slip[0]
-        slip_rate = d_slip/family.duration
-        row.append(slip_rate)
-        table.append(row)
-    if tablefmt == 'csv':
-        writer.writerows(table)
-    else:
-        format_dict = {
-            'simple': 'simple',
-            'markdown': 'github'
-        }
-        tablefmt = format_dict[config.args.format]
-        floatfmt = [
-            None,
-            None,
-            '.4f',
-            '.4f',
-            '.3f',
-            None,
-            None,
-            '.2f',
-            '.1f'
-        ]
-        print(
-            tabulate(
-                table, headers=headers, floatfmt=floatfmt, tablefmt=tablefmt)
-        )
+        slip_rate = np.inf if family.duration == 0 else d_slip/family.duration
+        row += [slip_rate, family.magmin, family.magmax]
+        rows.append(row)
+    generic_printer(config, rows, headers_fmt)
```

### Comparing `requake-0.5/requake/formulas/conversion.py` & `requake-0.6/requake/formulas/conversion.py`

 * *Files identical despite different names*

### Comparing `requake-0.5/requake/main.py` & `requake-0.6/requake/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,17 +19,23 @@
     from .config.parse_arguments import parse_arguments
     args = parse_arguments()
     from .config.rq_setup import configure, rq_exit
     config = configure(args)
     if config.args.action == 'read_catalog':
         from .catalog import read_catalog
         read_catalog(config)
+    if config.args.action == 'print_catalog':
+        from .catalog import print_catalog
+        print_catalog(config)
     if config.args.action == 'scan_catalog':
         from .scan import scan_catalog
         scan_catalog(config)
+    if config.args.action == 'print_pairs':
+        from .families import print_pairs
+        print_pairs(config)
     if config.args.action == 'scan_templates':
         from .scan import scan_templates
         scan_templates(config)
     if config.args.action == 'plot_pair':
         from .plot import plot_pair
         plot_pair(config)
     if config.args.action == 'build_families':
@@ -40,17 +46,17 @@
         print_families(config)
     if config.args.action == 'plot_families':
         from .plot import plot_families
         plot_families(config)
     if config.args.action == 'plot_timespans':
         from .plot import plot_timespans
         plot_timespans(config)
-    if config.args.action == 'plot_slip':
-        from .plot import plot_slip
-        plot_slip(config)
+    if config.args.action == 'plot_cumulative':
+        from .plot import plot_cumulative
+        plot_cumulative(config)
     if config.args.action == 'map_families':
         from .plot import map_families
         map_families(config)
     if config.args.action == 'flag_family':
         from .families import flag_family
         flag_family(config)
     if config.args.action == 'build_templates':
```

### Comparing `requake-0.5/requake/plot/__init__.py` & `requake-0.6/requake/plot/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 :license:
     GNU General Public License v3.0 or later
     (https://www.gnu.org/licenses/gpl-3.0-standalone.html)
 """
 from .plot_pair import plot_pair  # noqa
 from .plot_families import plot_families  # noqa
 from .plot_timespans import plot_timespans  # noqa
-from .plot_slip import plot_slip  # noqa
+from .plot_cumulative import plot_cumulative  # noqa
 from .map_families import map_families  # noqa
```

### Comparing `requake-0.5/requake/plot/cached_tiler.py` & `requake-0.6/requake/plot/cached_tiler.py`

 * *Files identical despite different names*

### Comparing `requake-0.5/requake/plot/map_families.py` & `requake-0.6/requake/plot/map_families.py`

 * *Files identical despite different names*

### Comparing `requake-0.5/requake/plot/map_tiles.py` & `requake-0.6/requake/plot/map_tiles.py`

 * *Files identical despite different names*

### Comparing `requake-0.5/requake/plot/plot_families.py` & `requake-0.6/requake/plot/plot_families.py`

 * *Files 6% similar despite different names*

```diff
@@ -212,14 +212,22 @@
     Plot traces for one or more event families.
     """
     try:
         families = read_selected_families(config)
     except (FileNotFoundError, FamilyNotFoundError) as m:
         logger.error(m)
         rq_exit(1)
+    if len(families) > 20:
+        logger.warning(
+            f'Too many families selected: {len(families)}. '
+            'Plotting only the first 20.')
+        logger.info(
+            'See "requake plot_families -h" for information on '
+            'how to select specific families.')
+        families = families[:20]
     for family in families:
         _plot_family(config, family)
     print('''
     Use left/right arrow keys to scroll backwards/forward in time.
     Use shift+left/shift+right to increase/decrease the time window.
     Use up/down arrow keys to increase/decrease trace amplitude.
     Press '0' to reset the view.
```

### Comparing `requake-0.5/requake/plot/plot_pair.py` & `requake-0.6/requake/plot/plot_pair.py`

 * *Files identical despite different names*

### Comparing `requake-0.5/requake/plot/plot_timespans.py` & `requake-0.6/requake/plot/plot_timespans.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,17 +102,18 @@
         rq_exit(1)
     trace_ids = []
     for family in families:
         if family.trace_id not in trace_ids and family.trace_id is not None:
             trace_ids.append(family.trace_id)
         color = cmap(norm(family.number % 10))
         _plot_family_timespans(family, ax, sort_by, lon0, lat0, color)
-    format_time_axis(ax, which='xaxis')
+    ax.callbacks.connect('xlim_changed', format_time_axis)
     if sort_by == 'time':
-        format_time_axis(ax, which='yaxis')
+        ax.callbacks.connect(
+            'ylim_changed', lambda ax: format_time_axis(ax, which='yaxis'))
     ax.set_xlabel('Time')
     ax.set_ylabel(ylabels[sort_by])
     plot_title(
         ax, len(families), trace_ids, vertical_position=1.05, fontsize=10)
     ax.hover_annotation_element = 'lines'
     sm = cm.ScalarMappable(cmap=cmap, norm=norm)
     cbar = fig.colorbar(sm, ticks=range(10), ax=ax)
```

### Comparing `requake-0.5/requake/plot/plot_utils.py` & `requake-0.6/requake/plot/plot_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,42 +8,46 @@
 :license:
     GNU General Public License v3.0 or later
     (https://www.gnu.org/licenses/gpl-3.0-standalone.html)
 """
 import matplotlib.dates as mdates
 
 
-def format_time_axis(ax, which='both'):
+def format_time_axis(ax, which='xaxis'):
     """
     Format the time axis of a Matplotlib plot.
     """
     if which == 'both':
         axes = [ax.xaxis, ax.yaxis]
     elif which == 'xaxis':
         axes = [ax.xaxis]
     elif which == 'yaxis':
         axes = [ax.yaxis]
     else:
         raise ValueError(f'Invalid value for "which": {which}')
     for axis in axes:
-        dmin, dmax = axis.get_data_interval()
+        dmin, dmax = axis.get_view_interval()
         timespan = dmax-dmin
-        if timespan > 365:
+        if timespan > 2*365:
             _major_locator = mdates.YearLocator()   # every year
             _major_fmt = mdates.DateFormatter('%Y')
             _minor_locator = mdates.MonthLocator()  # every month
         else:
             _major_locator = mdates.AutoDateLocator(minticks=3, maxticks=7)
             _major_fmt = mdates.ConciseDateFormatter(_major_locator)
-            _minor_locator = mdates.DayLocator()  # every day
+            if timespan > 365/2:
+                _minor_locator = mdates.MonthLocator()  # every month
+            else:
+                _minor_locator = mdates.DayLocator()  # every day
         axis.set_major_locator(_major_locator)
         axis.set_major_formatter(_major_fmt)
         axis.set_minor_locator(_minor_locator)
         axis.grid(True, which='major', linestyle='--', color='0.5')
         axis.grid(True, which='minor', linestyle=':', color='0.8')
+    ax.figure.canvas.draw()
 
 
 def plot_title(
         ax, nfamilies, trace_ids=None, vertical_position=1, fontsize=10):
     """
     Set the title of a plot.
```

### Comparing `requake-0.5/requake/scan/scan_catalog.py` & `requake-0.6/requake/scan/scan_catalog.py`

 * *Files identical despite different names*

### Comparing `requake-0.5/requake/scan/scan_templates.py` & `requake-0.6/requake/scan/scan_templates.py`

 * *Files identical despite different names*

### Comparing `requake-0.5/requake/waveforms/arrivals.py` & `requake-0.6/requake/waveforms/arrivals.py`

 * *Files identical despite different names*

### Comparing `requake-0.5/requake/waveforms/station_metadata.py` & `requake-0.6/requake/waveforms/station_metadata.py`

 * *Files identical despite different names*

### Comparing `requake-0.5/requake/waveforms/waveforms.py` & `requake-0.6/requake/waveforms/waveforms.py`

 * *Files identical despite different names*

### Comparing `requake-0.5/requake.egg-info/PKG-INFO` & `requake-0.6/requake.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requake
-Version: 0.5
+Version: 0.6
 Summary: Repeating earthquakes search and analysis
 Home-page: https://requake.seismicsource.org
 Author: Claudio Satriano
 Author-email: satriano@ipgp.fr
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Homepage, https://requake.seismicsource.org
 Project-URL: Source, https://github.com/SeismicSource/requake
@@ -29,15 +29,15 @@
 License-File: LICENSE.txt
 Requires-Dist: scipy>=1.5.0
 Requires-Dist: obspy>=1.2.0
 Requires-Dist: argcomplete
 Requires-Dist: tqdm
 Requires-Dist: tabulate
 
-<img src="imgs/Requake_logo.svg" width="400">
+<img src="https://cdn.jsdelivr.net/gh/SeismicSource/requake@dc9a6e6fd818e57e0c0d74f9c16f2bfc6d4d148c/imgs/Requake_logo.svg" width="400">
 
 # Requake
 
 Repeating earthquakes search and analysis.
 
 [![changelog-badge]][changelog-link]
 [![PyPI-badge]][PyPI-link]
@@ -118,41 +118,42 @@
 
 Requake is based on a single executable, aptly named `requake` 😉.
 
 To get help, use:
 
     requake -h
 
-The different running modes are specified as "verbs" (positional arguments).
-Currently supported verbs are:
+Different commands are available:
 
     sample_config       write sample config file to current directory and exit
+    update_config       update an existing config file to the latest version
     read_catalog        read an event catalog from web services or from a file
+    print_catalog       print the event catalog to screen
     scan_catalog        scan an existing catalog for earthquake pairs
+    print_pairs         print pairs to screen
     plot_pair           plot traces for a given event pair
     build_families      build families of repeating earthquakes from a catalog
                         of pairs
     print_families      print families to screen
     plot_families       plot traces for one ore more event families
     plot_timespans      plot family timespans
-    plot_slip           plot cumulative slip for one or more families
+    plot_cumulative     cumulative plot for one or more families
     map_families        plot families on a map
     flag_family         flag a family of repeating earthquakes as valid or not
-                        valid. Note that all families are valid by default
-                        when first created
+                        valid.
     build_templates     build waveform templates for one or more event
                         families
     scan_templates      scan a continuous waveform stream using one or more
                         templates
 
-Certain running modes (e.g., `plot_pair`) require further arguments (use, e.g.,
+Certain commands (e.g., `plot_pair`) require further arguments (use, e.g.,
 `requake plot_pair -h` to get help).
 
-Requake supports command line tab completion for arguments, thanks to
-[argcomplete](https://kislyuk.github.io/argcomplete/).
+Requake supports command line tab completion for commands and arguments, thanks
+to [argcomplete](https://kislyuk.github.io/argcomplete/).
 To enable command line tab completion, add the following line to your `.bashrc`
 or `.zshrc`:
 
     eval "$(register-python-argcomplete requake)"
 
 ### Typical workflow
```

### Comparing `requake-0.5/requake.egg-info/SOURCES.txt` & `requake-0.6/requake.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -13,43 +13,48 @@
 requake.egg-info/SOURCES.txt
 requake.egg-info/dependency_links.txt
 requake.egg-info/entry_points.txt
 requake.egg-info/requires.txt
 requake.egg-info/top_level.txt
 requake/catalog/__init__.py
 requake/catalog/catalog.py
+requake/catalog/print_catalog.py
 requake/catalog/read_catalog.py
 requake/catalog/read_catalog_from_csv.py
 requake/catalog/read_catalog_from_fdsnws.py
 requake/catalog/read_catalog_from_quakeml.py
 requake/config/__init__.py
 requake/config/config.py
 requake/config/configspec.conf
+requake/config/generic_printer.py
 requake/config/parse_arguments.py
 requake/config/rq_setup.py
 requake/config/utils.py
 requake/config/configobj/__init__.py
 requake/config/configobj/_version.py
 requake/config/configobj/validate.py
 requake/families/__init__.py
 requake/families/build_families.py
 requake/families/build_templates.py
 requake/families/families.py
 requake/families/flag_family.py
+requake/families/pairs.py
 requake/families/print_families.py
+requake/families/print_pairs.py
 requake/formulas/__init__.py
 requake/formulas/conversion.py
+requake/formulas/moment.py
 requake/formulas/slip.py
 requake/plot/__init__.py
 requake/plot/cached_tiler.py
 requake/plot/map_families.py
 requake/plot/map_tiles.py
+requake/plot/plot_cumulative.py
 requake/plot/plot_families.py
 requake/plot/plot_pair.py
-requake/plot/plot_slip.py
 requake/plot/plot_timespans.py
 requake/plot/plot_utils.py
 requake/scan/__init__.py
 requake/scan/scan_catalog.py
 requake/scan/scan_templates.py
 requake/waveforms/__init__.py
 requake/waveforms/arrivals.py
```

### Comparing `requake-0.5/setup.py` & `requake-0.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: GPL-3.0-or-later
 """setup.py: setuptools control."""
 from setuptools import setup, find_packages
 import versioneer
 
-
+revision = versioneer.get_versions()['full-revisionid']
+cdn_baseurl = 'https://cdn.jsdelivr.net/gh/SeismicSource/requake@{}'\
+    .format(revision)
 with open('README.md', 'rb') as f:
-    long_descr = f.read().decode('utf-8')
+    long_descr = f.read().decode('utf-8').replace(
+        'imgs/Requake_logo.svg',
+        '{}/imgs/Requake_logo.svg'.format(cdn_baseurl)
+    )
 
 project_urls = {
     'Homepage': 'https://requake.seismicsource.org',
     'Source': 'https://github.com/SeismicSource/requake',
     'Documentation': 'https://requake.readthedocs.io'
 }
```

### Comparing `requake-0.5/versioneer.py` & `requake-0.6/versioneer.py`

 * *Files identical despite different names*

