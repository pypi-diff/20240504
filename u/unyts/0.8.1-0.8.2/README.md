# Comparing `tmp/unyts-0.8.1.tar.gz` & `tmp/unyts-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unyts-0.8.1.tar", last modified: Fri May  3 22:26:41 2024, max compression
+gzip compressed data, was "unyts-0.8.2.tar", last modified: Fri May  3 22:40:02 2024, max compression
```

## Comparing `unyts-0.8.1.tar` & `unyts-0.8.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 22:26:40.950000 unyts-0.8.1/
--rw-rw-rw-   0        0        0     1077 2020-11-01 00:39:44.000000 unyts-0.8.1/LICENSE
--rw-rw-rw-   0        0        0       66 2024-02-11 22:13:34.000000 unyts-0.8.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6631 2024-05-03 22:26:42.000000 unyts-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     4522 2024-05-03 22:25:22.000000 unyts-0.8.1/README.md
--rw-rw-rw-   0        0        0      982 2024-05-03 22:26:32.000000 unyts-0.8.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-03 22:26:42.000000 unyts-0.8.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-03 22:26:40.960000 unyts-0.8.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-03 22:26:40.970000 unyts-0.8.1/src/unyts/
--rw-rw-rw-   0        0        0      495 2023-12-30 23:46:12.000000 unyts-0.8.1/src/unyts/Empty.py
--rw-rw-rw-   0        0        0     1400 2024-05-03 22:24:46.000000 unyts-0.8.1/src/unyts/__init__.py
--rw-rw-rw-   0        0        0      146 2024-05-03 22:18:52.000000 unyts-0.8.1/src/unyts/__main__.py
--rw-rw-rw-   0        0        0    26470 2024-05-03 22:18:52.000000 unyts-0.8.1/src/unyts/converter.py
--rw-rw-rw-   0        0        0    48716 2024-05-03 22:18:52.000000 unyts-0.8.1/src/unyts/database.py
--rw-rw-rw-   0        0        0    23518 2024-05-03 22:18:52.000000 unyts-0.8.1/src/unyts/dictionaries.py
--rw-rw-rw-   0        0        0      862 2022-12-29 13:49:38.000000 unyts-0.8.1/src/unyts/errors.py
--rw-rw-rw-   0        0        0     7147 2024-05-03 22:18:52.000000 unyts-0.8.1/src/unyts/gui.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:26:40.970000 unyts-0.8.1/src/unyts/helpers/
--rw-rw-rw-   0        0        0      158 2022-09-20 21:54:58.000000 unyts-0.8.1/src/unyts/helpers/__init__.py
--rw-rw-rw-   0        0        0     7475 2023-12-30 23:46:12.000000 unyts-0.8.1/src/unyts/helpers/caster.py
--rw-rw-rw-   0        0        0     2100 2023-12-30 23:46:12.000000 unyts-0.8.1/src/unyts/helpers/common_classes.py
--rw-rw-rw-   0        0        0      952 2023-12-30 23:46:12.000000 unyts-0.8.1/src/unyts/helpers/is_number.py
--rw-rw-rw-   0        0        0     1142 2023-01-18 21:37:24.000000 unyts-0.8.1/src/unyts/helpers/is_unit.py
--rw-rw-rw-   0        0        0     1987 2023-01-17 21:17:22.000000 unyts-0.8.1/src/unyts/helpers/multi_split.py
--rw-rw-rw-   0        0        0     3538 2023-12-30 23:46:12.000000 unyts-0.8.1/src/unyts/helpers/unit_string_tools.py
--rw-rw-rw-   0        0        0     6576 2024-05-03 22:18:52.000000 unyts-0.8.1/src/unyts/network.py
--rw-rw-rw-   0        0        0    11085 2023-07-24 18:15:20.000000 unyts-0.8.1/src/unyts/operations.py
--rw-rw-rw-   0        0        0      149 2024-05-03 22:18:52.000000 unyts-0.8.1/src/unyts/parameters.ini
--rw-rw-rw-   0        0        0     6289 2024-05-03 22:18:52.000000 unyts-0.8.1/src/unyts/parameters.py
--rw-rw-rw-   0        0        0     2695 2024-02-11 22:13:34.000000 unyts-0.8.1/src/unyts/searches.py
--rw-rw-rw-   0        0        0    28535 2023-12-30 23:46:12.000000 unyts-0.8.1/src/unyts/unit_class.py
--rw-rw-rw-   0        0        0     2078 2023-01-30 12:24:34.000000 unyts-0.8.1/src/unyts/unitary.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:26:40.970000 unyts-0.8.1/src/unyts/units/
--rw-rw-rw-   0        0        0      129 2022-09-08 15:55:48.000000 unyts-0.8.1/src/unyts/units/__init__.py
--rw-rw-rw-   0        0        0     3087 2023-12-30 23:46:12.000000 unyts-0.8.1/src/unyts/units/custom.py
--rw-rw-rw-   0        0        0      726 2023-12-30 23:46:12.000000 unyts-0.8.1/src/unyts/units/data.py
--rw-rw-rw-   0        0        0     1230 2023-12-30 23:46:12.000000 unyts-0.8.1/src/unyts/units/date.py
--rw-rw-rw-   0        0        0     2288 2023-12-30 23:46:12.000000 unyts-0.8.1/src/unyts/units/define.py
--rw-rw-rw-   0        0        0     6288 2023-12-30 23:46:12.000000 unyts-0.8.1/src/unyts/units/energy.py
--rw-rw-rw-   0        0        0     2301 2023-12-30 23:46:12.000000 unyts-0.8.1/src/unyts/units/force.py
--rw-rw-rw-   0        0        0     1881 2023-12-30 23:46:12.000000 unyts-0.8.1/src/unyts/units/geometry.py
--rw-rw-rw-   0        0        0      726 2023-12-30 23:46:12.000000 unyts-0.8.1/src/unyts/units/mass.py
--rw-rw-rw-   0        0        0     1629 2023-12-30 23:46:12.000000 unyts-0.8.1/src/unyts/units/rates.py
--rw-rw-rw-   0        0        0     1999 2023-12-30 23:46:12.000000 unyts-0.8.1/src/unyts/units/ratios.py
--rw-rw-rw-   0        0        0     1198 2023-12-30 23:46:12.000000 unyts-0.8.1/src/unyts/units/temperature.py
--rw-rw-rw-   0        0        0     1328 2023-12-30 23:46:12.000000 unyts-0.8.1/src/unyts/units/time.py
--rw-rw-rw-   0        0        0     2601 2023-12-30 23:46:12.000000 unyts-0.8.1/src/unyts/units/unitless.py
--rw-rw-rw-   0        0        0   248691 2024-05-03 22:18:52.000000 unyts-0.8.1/src/unyts/unyts_icon.ico
-drwxrwxrwx   0        0        0        0 2024-05-03 22:26:40.970000 unyts-0.8.1/src/unyts.egg-info/
--rw-rw-rw-   0        0        0     6631 2024-05-03 22:26:42.000000 unyts-0.8.1/src/unyts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1282 2024-05-03 22:26:42.000000 unyts-0.8.1/src/unyts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 22:26:42.000000 unyts-0.8.1/src/unyts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-03 22:26:42.000000 unyts-0.8.1/src/unyts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-03 22:26:42.000000 unyts-0.8.1/src/unyts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-03 22:26:40.980000 unyts-0.8.1/tests/
--rw-rw-rw-   0        0        0     5512 2023-05-23 22:04:30.000000 unyts-0.8.1/tests/test_converter.py
--rw-rw-rw-   0        0        0     2241 2023-01-30 12:24:34.000000 unyts-0.8.1/tests/test_dictionaries.py
--rw-rw-rw-   0        0        0     1597 2023-01-17 21:17:22.000000 unyts-0.8.1/tests/test_operations.py
--rw-rw-rw-   0        0        0      808 2023-01-30 12:24:34.000000 unyts-0.8.1/tests/test_uncertain_units.py
--rw-rw-rw-   0        0        0     6368 2024-05-03 22:18:52.000000 unyts-0.8.1/tests/test_units.py
+drwxrwxrwx   0        0        0        0 2024-05-03 22:40:02.080000 unyts-0.8.2/
+-rw-rw-rw-   0        0        0     1077 2020-11-01 00:39:44.000000 unyts-0.8.2/LICENSE
+-rw-rw-rw-   0        0        0       66 2024-02-11 22:13:34.000000 unyts-0.8.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6631 2024-05-03 22:40:04.000000 unyts-0.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4522 2024-05-03 22:25:22.000000 unyts-0.8.2/README.md
+-rw-rw-rw-   0        0        0      982 2024-05-03 22:39:46.000000 unyts-0.8.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-03 22:40:04.000000 unyts-0.8.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-03 22:40:02.090000 unyts-0.8.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-03 22:40:02.090000 unyts-0.8.2/src/unyts/
+-rw-rw-rw-   0        0        0      495 2023-12-30 23:46:12.000000 unyts-0.8.2/src/unyts/Empty.py
+-rw-rw-rw-   0        0        0     1400 2024-05-03 22:39:46.000000 unyts-0.8.2/src/unyts/__init__.py
+-rw-rw-rw-   0        0        0      146 2024-05-03 22:18:52.000000 unyts-0.8.2/src/unyts/__main__.py
+-rw-rw-rw-   0        0        0    26470 2024-05-03 22:18:52.000000 unyts-0.8.2/src/unyts/converter.py
+-rw-rw-rw-   0        0        0    48716 2024-05-03 22:18:52.000000 unyts-0.8.2/src/unyts/database.py
+-rw-rw-rw-   0        0        0    23518 2024-05-03 22:18:52.000000 unyts-0.8.2/src/unyts/dictionaries.py
+-rw-rw-rw-   0        0        0      862 2022-12-29 13:49:38.000000 unyts-0.8.2/src/unyts/errors.py
+-rw-rw-rw-   0        0        0     7147 2024-05-03 22:18:52.000000 unyts-0.8.2/src/unyts/gui.py
+drwxrwxrwx   0        0        0        0 2024-05-03 22:40:02.100000 unyts-0.8.2/src/unyts/helpers/
+-rw-rw-rw-   0        0        0      158 2022-09-20 21:54:58.000000 unyts-0.8.2/src/unyts/helpers/__init__.py
+-rw-rw-rw-   0        0        0     7475 2023-12-30 23:46:12.000000 unyts-0.8.2/src/unyts/helpers/caster.py
+-rw-rw-rw-   0        0        0     2100 2023-12-30 23:46:12.000000 unyts-0.8.2/src/unyts/helpers/common_classes.py
+-rw-rw-rw-   0        0        0      952 2023-12-30 23:46:12.000000 unyts-0.8.2/src/unyts/helpers/is_number.py
+-rw-rw-rw-   0        0        0     1142 2023-01-18 21:37:24.000000 unyts-0.8.2/src/unyts/helpers/is_unit.py
+-rw-rw-rw-   0        0        0     1987 2023-01-17 21:17:22.000000 unyts-0.8.2/src/unyts/helpers/multi_split.py
+-rw-rw-rw-   0        0        0     3538 2023-12-30 23:46:12.000000 unyts-0.8.2/src/unyts/helpers/unit_string_tools.py
+-rw-rw-rw-   0        0        0     6576 2024-05-03 22:18:52.000000 unyts-0.8.2/src/unyts/network.py
+-rw-rw-rw-   0        0        0    11085 2023-07-24 18:15:20.000000 unyts-0.8.2/src/unyts/operations.py
+-rw-rw-rw-   0        0        0      149 2024-05-03 22:18:52.000000 unyts-0.8.2/src/unyts/parameters.ini
+-rw-rw-rw-   0        0        0     6289 2024-05-03 22:18:52.000000 unyts-0.8.2/src/unyts/parameters.py
+-rw-rw-rw-   0        0        0     2695 2024-02-11 22:13:34.000000 unyts-0.8.2/src/unyts/searches.py
+-rw-rw-rw-   0        0        0    28535 2023-12-30 23:46:12.000000 unyts-0.8.2/src/unyts/unit_class.py
+-rw-rw-rw-   0        0        0     2078 2023-01-30 12:24:34.000000 unyts-0.8.2/src/unyts/unitary.py
+drwxrwxrwx   0        0        0        0 2024-05-03 22:40:02.100000 unyts-0.8.2/src/unyts/units/
+-rw-rw-rw-   0        0        0      129 2022-09-08 15:55:48.000000 unyts-0.8.2/src/unyts/units/__init__.py
+-rw-rw-rw-   0        0        0     3087 2023-12-30 23:46:12.000000 unyts-0.8.2/src/unyts/units/custom.py
+-rw-rw-rw-   0        0        0      726 2023-12-30 23:46:12.000000 unyts-0.8.2/src/unyts/units/data.py
+-rw-rw-rw-   0        0        0     1230 2023-12-30 23:46:12.000000 unyts-0.8.2/src/unyts/units/date.py
+-rw-rw-rw-   0        0        0     2288 2023-12-30 23:46:12.000000 unyts-0.8.2/src/unyts/units/define.py
+-rw-rw-rw-   0        0        0     6288 2023-12-30 23:46:12.000000 unyts-0.8.2/src/unyts/units/energy.py
+-rw-rw-rw-   0        0        0     2301 2023-12-30 23:46:12.000000 unyts-0.8.2/src/unyts/units/force.py
+-rw-rw-rw-   0        0        0     1881 2023-12-30 23:46:12.000000 unyts-0.8.2/src/unyts/units/geometry.py
+-rw-rw-rw-   0        0        0      726 2023-12-30 23:46:12.000000 unyts-0.8.2/src/unyts/units/mass.py
+-rw-rw-rw-   0        0        0     1629 2023-12-30 23:46:12.000000 unyts-0.8.2/src/unyts/units/rates.py
+-rw-rw-rw-   0        0        0     1999 2023-12-30 23:46:12.000000 unyts-0.8.2/src/unyts/units/ratios.py
+-rw-rw-rw-   0        0        0     1198 2023-12-30 23:46:12.000000 unyts-0.8.2/src/unyts/units/temperature.py
+-rw-rw-rw-   0        0        0     1328 2023-12-30 23:46:12.000000 unyts-0.8.2/src/unyts/units/time.py
+-rw-rw-rw-   0        0        0     2601 2023-12-30 23:46:12.000000 unyts-0.8.2/src/unyts/units/unitless.py
+-rw-rw-rw-   0        0        0   248691 2024-05-03 22:18:52.000000 unyts-0.8.2/src/unyts/unyts_icon.ico
+drwxrwxrwx   0        0        0        0 2024-05-03 22:40:02.090000 unyts-0.8.2/src/unyts.egg-info/
+-rw-rw-rw-   0        0        0     6631 2024-05-03 22:40:04.000000 unyts-0.8.2/src/unyts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1282 2024-05-03 22:40:04.000000 unyts-0.8.2/src/unyts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 22:40:04.000000 unyts-0.8.2/src/unyts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-03 22:40:04.000000 unyts-0.8.2/src/unyts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-03 22:40:04.000000 unyts-0.8.2/src/unyts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 22:40:02.100000 unyts-0.8.2/tests/
+-rw-rw-rw-   0        0        0     5512 2023-05-23 22:04:30.000000 unyts-0.8.2/tests/test_converter.py
+-rw-rw-rw-   0        0        0     2241 2023-01-30 12:24:34.000000 unyts-0.8.2/tests/test_dictionaries.py
+-rw-rw-rw-   0        0        0     1597 2023-01-17 21:17:22.000000 unyts-0.8.2/tests/test_operations.py
+-rw-rw-rw-   0        0        0      808 2023-01-30 12:24:34.000000 unyts-0.8.2/tests/test_uncertain_units.py
+-rw-rw-rw-   0        0        0     6368 2024-05-03 22:18:52.000000 unyts-0.8.2/tests/test_units.py
```

### Comparing `unyts-0.8.1/LICENSE` & `unyts-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/PKG-INFO` & `unyts-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unyts
-Version: 0.8.1
+Version: 0.8.2
 Summary: a unit converter based on graph network and classes to operate with units.
 Author-email: Martin Carlos Araya <martinaraya@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Martín Carlos Araya
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `unyts-0.8.1/README.md` & `unyts-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/pyproject.toml` & `unyts-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 2022 7365 7475 7074 6f6f 6c73 2e62 7569   "setuptools.bui
 00000050: 6c64 5f6d 6574 6122 0d0a 0d0a 5b74 6f6f  ld_meta"....[too
 00000060: 6c2e 7365 7475 7074 6f6f 6c73 2e70 6163  l.setuptools.pac
 00000070: 6b61 6765 732e 6669 6e64 5d0d 0a77 6865  kages.find]..whe
 00000080: 7265 203d 205b 2273 7263 225d 0d0a 0d0a  re = ["src"]....
 00000090: 5b70 726f 6a65 6374 5d0d 0a6e 616d 6520  [project]..name 
 000000a0: 3d20 2275 6e79 7473 220d 0a76 6572 7369  = "unyts"..versi
-000000b0: 6f6e 203d 2022 302e 382e 3122 0d0a 6175  on = "0.8.1"..au
+000000b0: 6f6e 203d 2022 302e 382e 3222 0d0a 6175  on = "0.8.2"..au
 000000c0: 7468 6f72 7320 3d20 5b0d 0a20 207b 206e  thors = [..  { n
 000000d0: 616d 653d 224d 6172 7469 6e20 4361 726c  ame="Martin Carl
 000000e0: 6f73 2041 7261 7961 222c 2065 6d61 696c  os Araya", email
 000000f0: 3d22 6d61 7274 696e 6172 6179 6140 676d  ="martinaraya@gm
 00000100: 6169 6c2e 636f 6d22 207d 2c0d 0a5d 0d0a  ail.com" },..]..
 00000110: 6465 7363 7269 7074 696f 6e20 3d20 2261  description = "a
 00000120: 2075 6e69 7420 636f 6e76 6572 7465 7220   unit converter
```

### Comparing `unyts-0.8.1/src/unyts/__init__.py` & `unyts-0.8.2/src/unyts/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 # -*- coding: utf-8 -*-
 """
 Created on Sat Oct 24 18:24:20 2020
 
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
-__version__ = '0.8.1'
-__release__ = 20240502
+__version__ = '0.8.2'
+__release__ = 20240504
 __all__ = ['units', 'convert', 'convertible', 'Unit', 'is_Unit',
            'set_unit', 'set_conversion', 'set_density',
            'save', 'start_gui', 'set_fvf']
 
 from .parameters import unyts_parameters_, print_path, reload, raise_error, cache, set_density, get_density
 from .database import network_to_frame, save_memory, load_memory, set_fvf
 from .units.define import units
```

### Comparing `unyts-0.8.1/src/unyts/converter.py` & `unyts-0.8.2/src/unyts/converter.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts/database.py` & `unyts-0.8.2/src/unyts/database.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts/dictionaries.py` & `unyts-0.8.2/src/unyts/dictionaries.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts/errors.py` & `unyts-0.8.2/src/unyts/errors.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts/gui.py` & `unyts-0.8.2/src/unyts/gui.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts/helpers/caster.py` & `unyts-0.8.2/src/unyts/helpers/caster.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts/helpers/common_classes.py` & `unyts-0.8.2/src/unyts/helpers/common_classes.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts/helpers/is_number.py` & `unyts-0.8.2/src/unyts/helpers/is_number.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts/helpers/is_unit.py` & `unyts-0.8.2/src/unyts/helpers/is_unit.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts/helpers/multi_split.py` & `unyts-0.8.2/src/unyts/helpers/multi_split.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts/helpers/unit_string_tools.py` & `unyts-0.8.2/src/unyts/helpers/unit_string_tools.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts/network.py` & `unyts-0.8.2/src/unyts/network.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts/operations.py` & `unyts-0.8.2/src/unyts/operations.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts/parameters.py` & `unyts-0.8.2/src/unyts/parameters.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts/searches.py` & `unyts-0.8.2/src/unyts/searches.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts/unit_class.py` & `unyts-0.8.2/src/unyts/unit_class.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts/unitary.py` & `unyts-0.8.2/src/unyts/unitary.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts/units/custom.py` & `unyts-0.8.2/src/unyts/units/custom.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts/units/data.py` & `unyts-0.8.2/src/unyts/units/data.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts/units/date.py` & `unyts-0.8.2/src/unyts/units/date.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts/units/define.py` & `unyts-0.8.2/src/unyts/units/define.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts/units/energy.py` & `unyts-0.8.2/src/unyts/units/energy.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts/units/force.py` & `unyts-0.8.2/src/unyts/units/force.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts/units/geometry.py` & `unyts-0.8.2/src/unyts/units/geometry.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts/units/mass.py` & `unyts-0.8.2/src/unyts/units/mass.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts/units/rates.py` & `unyts-0.8.2/src/unyts/units/rates.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts/units/ratios.py` & `unyts-0.8.2/src/unyts/units/ratios.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts/units/temperature.py` & `unyts-0.8.2/src/unyts/units/temperature.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts/units/time.py` & `unyts-0.8.2/src/unyts/units/time.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts/units/unitless.py` & `unyts-0.8.2/src/unyts/units/unitless.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts/unyts_icon.ico` & `unyts-0.8.2/src/unyts/unyts_icon.ico`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/src/unyts.egg-info/PKG-INFO` & `unyts-0.8.2/src/unyts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unyts
-Version: 0.8.1
+Version: 0.8.2
 Summary: a unit converter based on graph network and classes to operate with units.
 Author-email: Martin Carlos Araya <martinaraya@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Martín Carlos Araya
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `unyts-0.8.1/src/unyts.egg-info/SOURCES.txt` & `unyts-0.8.2/src/unyts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/tests/test_converter.py` & `unyts-0.8.2/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/tests/test_dictionaries.py` & `unyts-0.8.2/tests/test_dictionaries.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/tests/test_operations.py` & `unyts-0.8.2/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/tests/test_uncertain_units.py` & `unyts-0.8.2/tests/test_uncertain_units.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.1/tests/test_units.py` & `unyts-0.8.2/tests/test_units.py`

 * *Files identical despite different names*

