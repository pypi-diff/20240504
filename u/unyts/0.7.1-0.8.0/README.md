# Comparing `tmp/unyts-0.7.1.tar.gz` & `tmp/unyts-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unyts-0.7.1.tar", last modified: Sun Feb 11 21:03:50 2024, max compression
+gzip compressed data, was "unyts-0.8.0.tar", last modified: Fri May  3 22:14:21 2024, max compression
```

## Comparing `unyts-0.7.1.tar` & `unyts-0.8.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2024-02-11 21:03:50.530000 unyts-0.7.1/
--rw-rw-rw-   0        0        0     1077 2020-11-01 00:39:44.000000 unyts-0.7.1/LICENSE
--rw-rw-rw-   0        0        0       66 2024-02-11 20:59:06.000000 unyts-0.7.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6326 2024-02-11 21:03:52.000000 unyts-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     4245 2023-12-30 23:46:12.000000 unyts-0.7.1/README.md
--rw-rw-rw-   0        0        0      962 2024-02-11 20:56:02.000000 unyts-0.7.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-11 21:03:52.000000 unyts-0.7.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-11 21:03:50.530000 unyts-0.7.1/src/
-drwxrwxrwx   0        0        0        0 2024-02-11 21:03:50.540000 unyts-0.7.1/src/unyts/
--rw-rw-rw-   0        0        0      495 2023-12-30 23:46:12.000000 unyts-0.7.1/src/unyts/Empty.py
--rw-rw-rw-   0        0        0     1373 2024-02-11 19:45:24.000000 unyts-0.7.1/src/unyts/__init__.py
--rw-rw-rw-   0        0        0      115 2024-02-11 17:42:32.000000 unyts-0.7.1/src/unyts/__main__.py
--rw-rw-rw-   0        0        0    25731 2024-02-11 16:19:58.000000 unyts-0.7.1/src/unyts/converter.py
--rw-rw-rw-   0        0        0    46580 2023-07-24 18:15:20.000000 unyts-0.7.1/src/unyts/database.py
--rw-rw-rw-   0        0        0    23404 2023-07-24 18:15:20.000000 unyts-0.7.1/src/unyts/dictionaries.py
--rw-rw-rw-   0        0        0      862 2022-12-29 13:49:38.000000 unyts-0.7.1/src/unyts/errors.py
--rw-rw-rw-   0        0        0     5551 2024-02-11 20:48:22.000000 unyts-0.7.1/src/unyts/gui.py
-drwxrwxrwx   0        0        0        0 2024-02-11 21:03:50.540000 unyts-0.7.1/src/unyts/helpers/
--rw-rw-rw-   0        0        0      158 2022-09-20 21:54:58.000000 unyts-0.7.1/src/unyts/helpers/__init__.py
--rw-rw-rw-   0        0        0     7475 2023-12-30 23:46:12.000000 unyts-0.7.1/src/unyts/helpers/caster.py
--rw-rw-rw-   0        0        0     2100 2023-12-30 23:46:12.000000 unyts-0.7.1/src/unyts/helpers/common_classes.py
--rw-rw-rw-   0        0        0      952 2023-12-30 23:46:12.000000 unyts-0.7.1/src/unyts/helpers/is_number.py
--rw-rw-rw-   0        0        0     1142 2023-01-18 21:37:24.000000 unyts-0.7.1/src/unyts/helpers/is_unit.py
--rw-rw-rw-   0        0        0     1987 2023-01-17 21:17:22.000000 unyts-0.7.1/src/unyts/helpers/multi_split.py
--rw-rw-rw-   0        0        0     3538 2023-12-30 23:46:12.000000 unyts-0.7.1/src/unyts/helpers/unit_string_tools.py
--rw-rw-rw-   0        0        0     6425 2023-12-30 23:46:12.000000 unyts-0.7.1/src/unyts/network.py
--rw-rw-rw-   0        0        0    67646 2024-02-11 13:51:34.000000 unyts-0.7.1/src/unyts/openbook.ico
--rw-rw-rw-   0        0        0    11085 2023-07-24 18:15:20.000000 unyts-0.7.1/src/unyts/operations.py
--rw-rw-rw-   0        0        0      159 2024-02-11 19:32:02.000000 unyts-0.7.1/src/unyts/parameters.ini
--rw-rw-rw-   0        0        0     6248 2023-05-23 06:41:04.000000 unyts-0.7.1/src/unyts/parameters.py
--rw-rw-rw-   0        0        0     2695 2024-02-11 17:26:22.000000 unyts-0.7.1/src/unyts/searches.py
--rw-rw-rw-   0        0        0    28535 2023-12-30 23:46:12.000000 unyts-0.7.1/src/unyts/unit_class.py
--rw-rw-rw-   0        0        0     2078 2023-01-30 12:24:34.000000 unyts-0.7.1/src/unyts/unitary.py
-drwxrwxrwx   0        0        0        0 2024-02-11 21:03:50.540000 unyts-0.7.1/src/unyts/units/
--rw-rw-rw-   0        0        0      129 2022-09-08 15:55:48.000000 unyts-0.7.1/src/unyts/units/__init__.py
--rw-rw-rw-   0        0        0     3087 2023-12-30 23:46:12.000000 unyts-0.7.1/src/unyts/units/custom.py
--rw-rw-rw-   0        0        0      726 2023-12-30 23:46:12.000000 unyts-0.7.1/src/unyts/units/data.py
--rw-rw-rw-   0        0        0     1230 2023-12-30 23:46:12.000000 unyts-0.7.1/src/unyts/units/date.py
--rw-rw-rw-   0        0        0     2288 2023-12-30 23:46:12.000000 unyts-0.7.1/src/unyts/units/define.py
--rw-rw-rw-   0        0        0     6288 2023-12-30 23:46:12.000000 unyts-0.7.1/src/unyts/units/energy.py
--rw-rw-rw-   0        0        0     2301 2023-12-30 23:46:12.000000 unyts-0.7.1/src/unyts/units/force.py
--rw-rw-rw-   0        0        0     1881 2023-12-30 23:46:12.000000 unyts-0.7.1/src/unyts/units/geometry.py
--rw-rw-rw-   0        0        0      726 2023-12-30 23:46:12.000000 unyts-0.7.1/src/unyts/units/mass.py
--rw-rw-rw-   0        0        0     1629 2023-12-30 23:46:12.000000 unyts-0.7.1/src/unyts/units/rates.py
--rw-rw-rw-   0        0        0     1999 2023-12-30 23:46:12.000000 unyts-0.7.1/src/unyts/units/ratios.py
--rw-rw-rw-   0        0        0     1198 2023-12-30 23:46:12.000000 unyts-0.7.1/src/unyts/units/temperature.py
--rw-rw-rw-   0        0        0     1328 2023-12-30 23:46:12.000000 unyts-0.7.1/src/unyts/units/time.py
--rw-rw-rw-   0        0        0     2601 2023-12-30 23:46:12.000000 unyts-0.7.1/src/unyts/units/unitless.py
-drwxrwxrwx   0        0        0        0 2024-02-11 21:03:50.540000 unyts-0.7.1/src/unyts.egg-info/
--rw-rw-rw-   0        0        0     6326 2024-02-11 21:03:52.000000 unyts-0.7.1/src/unyts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1280 2024-02-11 21:03:52.000000 unyts-0.7.1/src/unyts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-11 21:03:52.000000 unyts-0.7.1/src/unyts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-02-11 21:03:52.000000 unyts-0.7.1/src/unyts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-02-11 21:03:52.000000 unyts-0.7.1/src/unyts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-11 21:03:50.540000 unyts-0.7.1/tests/
--rw-rw-rw-   0        0        0     5512 2023-05-23 22:04:30.000000 unyts-0.7.1/tests/test_converter.py
--rw-rw-rw-   0        0        0     2241 2023-01-30 12:24:34.000000 unyts-0.7.1/tests/test_dictionaries.py
--rw-rw-rw-   0        0        0     1597 2023-01-17 21:17:22.000000 unyts-0.7.1/tests/test_operations.py
--rw-rw-rw-   0        0        0      808 2023-01-30 12:24:34.000000 unyts-0.7.1/tests/test_uncertain_units.py
--rw-rw-rw-   0        0        0     6317 2023-01-30 12:24:34.000000 unyts-0.7.1/tests/test_units.py
+drwxrwxrwx   0        0        0        0 2024-05-03 22:14:21.750000 unyts-0.8.0/
+-rw-rw-rw-   0        0        0     1077 2020-11-01 00:39:44.000000 unyts-0.8.0/LICENSE
+-rw-rw-rw-   0        0        0       66 2024-02-11 22:13:34.000000 unyts-0.8.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6631 2024-05-03 22:14:22.000000 unyts-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4522 2024-05-03 22:13:38.000000 unyts-0.8.0/README.md
+-rw-rw-rw-   0        0        0      982 2024-05-03 22:04:08.000000 unyts-0.8.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-03 22:14:22.000000 unyts-0.8.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-03 22:14:21.760000 unyts-0.8.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-03 22:14:21.760000 unyts-0.8.0/src/unyts/
+-rw-rw-rw-   0        0        0      495 2023-12-30 23:46:12.000000 unyts-0.8.0/src/unyts/Empty.py
+-rw-rw-rw-   0        0        0     1400 2024-05-02 23:00:30.000000 unyts-0.8.0/src/unyts/__init__.py
+-rw-rw-rw-   0        0        0      146 2024-03-19 22:00:58.000000 unyts-0.8.0/src/unyts/__main__.py
+-rw-rw-rw-   0        0        0    26470 2024-05-02 20:39:36.000000 unyts-0.8.0/src/unyts/converter.py
+-rw-rw-rw-   0        0        0    48716 2024-05-02 23:09:54.000000 unyts-0.8.0/src/unyts/database.py
+-rw-rw-rw-   0        0        0    23518 2024-05-02 23:13:16.000000 unyts-0.8.0/src/unyts/dictionaries.py
+-rw-rw-rw-   0        0        0      862 2022-12-29 13:49:38.000000 unyts-0.8.0/src/unyts/errors.py
+-rw-rw-rw-   0        0        0     7147 2024-05-02 22:00:28.000000 unyts-0.8.0/src/unyts/gui.py
+drwxrwxrwx   0        0        0        0 2024-05-03 22:14:21.770000 unyts-0.8.0/src/unyts/helpers/
+-rw-rw-rw-   0        0        0      158 2022-09-20 21:54:58.000000 unyts-0.8.0/src/unyts/helpers/__init__.py
+-rw-rw-rw-   0        0        0     7475 2023-12-30 23:46:12.000000 unyts-0.8.0/src/unyts/helpers/caster.py
+-rw-rw-rw-   0        0        0     2100 2023-12-30 23:46:12.000000 unyts-0.8.0/src/unyts/helpers/common_classes.py
+-rw-rw-rw-   0        0        0      952 2023-12-30 23:46:12.000000 unyts-0.8.0/src/unyts/helpers/is_number.py
+-rw-rw-rw-   0        0        0     1142 2023-01-18 21:37:24.000000 unyts-0.8.0/src/unyts/helpers/is_unit.py
+-rw-rw-rw-   0        0        0     1987 2023-01-17 21:17:22.000000 unyts-0.8.0/src/unyts/helpers/multi_split.py
+-rw-rw-rw-   0        0        0     3538 2023-12-30 23:46:12.000000 unyts-0.8.0/src/unyts/helpers/unit_string_tools.py
+-rw-rw-rw-   0        0        0     6576 2024-05-02 22:28:00.000000 unyts-0.8.0/src/unyts/network.py
+-rw-rw-rw-   0        0        0    11085 2023-07-24 18:15:20.000000 unyts-0.8.0/src/unyts/operations.py
+-rw-rw-rw-   0        0        0      149 2024-05-03 16:23:30.000000 unyts-0.8.0/src/unyts/parameters.ini
+-rw-rw-rw-   0        0        0     6289 2024-05-02 20:39:36.000000 unyts-0.8.0/src/unyts/parameters.py
+-rw-rw-rw-   0        0        0     2695 2024-02-11 22:13:34.000000 unyts-0.8.0/src/unyts/searches.py
+-rw-rw-rw-   0        0        0    28535 2023-12-30 23:46:12.000000 unyts-0.8.0/src/unyts/unit_class.py
+-rw-rw-rw-   0        0        0     2078 2023-01-30 12:24:34.000000 unyts-0.8.0/src/unyts/unitary.py
+drwxrwxrwx   0        0        0        0 2024-05-03 22:14:21.770000 unyts-0.8.0/src/unyts/units/
+-rw-rw-rw-   0        0        0      129 2022-09-08 15:55:48.000000 unyts-0.8.0/src/unyts/units/__init__.py
+-rw-rw-rw-   0        0        0     3087 2023-12-30 23:46:12.000000 unyts-0.8.0/src/unyts/units/custom.py
+-rw-rw-rw-   0        0        0      726 2023-12-30 23:46:12.000000 unyts-0.8.0/src/unyts/units/data.py
+-rw-rw-rw-   0        0        0     1230 2023-12-30 23:46:12.000000 unyts-0.8.0/src/unyts/units/date.py
+-rw-rw-rw-   0        0        0     2288 2023-12-30 23:46:12.000000 unyts-0.8.0/src/unyts/units/define.py
+-rw-rw-rw-   0        0        0     6288 2023-12-30 23:46:12.000000 unyts-0.8.0/src/unyts/units/energy.py
+-rw-rw-rw-   0        0        0     2301 2023-12-30 23:46:12.000000 unyts-0.8.0/src/unyts/units/force.py
+-rw-rw-rw-   0        0        0     1881 2023-12-30 23:46:12.000000 unyts-0.8.0/src/unyts/units/geometry.py
+-rw-rw-rw-   0        0        0      726 2023-12-30 23:46:12.000000 unyts-0.8.0/src/unyts/units/mass.py
+-rw-rw-rw-   0        0        0     1629 2023-12-30 23:46:12.000000 unyts-0.8.0/src/unyts/units/rates.py
+-rw-rw-rw-   0        0        0     1999 2023-12-30 23:46:12.000000 unyts-0.8.0/src/unyts/units/ratios.py
+-rw-rw-rw-   0        0        0     1198 2023-12-30 23:46:12.000000 unyts-0.8.0/src/unyts/units/temperature.py
+-rw-rw-rw-   0        0        0     1328 2023-12-30 23:46:12.000000 unyts-0.8.0/src/unyts/units/time.py
+-rw-rw-rw-   0        0        0     2601 2023-12-30 23:46:12.000000 unyts-0.8.0/src/unyts/units/unitless.py
+-rw-rw-rw-   0        0        0   248691 2024-05-01 18:29:50.000000 unyts-0.8.0/src/unyts/unyts_icon.ico
+drwxrwxrwx   0        0        0        0 2024-05-03 22:14:21.760000 unyts-0.8.0/src/unyts.egg-info/
+-rw-rw-rw-   0        0        0     6631 2024-05-03 22:14:22.000000 unyts-0.8.0/src/unyts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1282 2024-05-03 22:14:22.000000 unyts-0.8.0/src/unyts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 22:14:22.000000 unyts-0.8.0/src/unyts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-03 22:14:22.000000 unyts-0.8.0/src/unyts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-03 22:14:22.000000 unyts-0.8.0/src/unyts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 22:14:21.770000 unyts-0.8.0/tests/
+-rw-rw-rw-   0        0        0     5512 2023-05-23 22:04:30.000000 unyts-0.8.0/tests/test_converter.py
+-rw-rw-rw-   0        0        0     2241 2023-01-30 12:24:34.000000 unyts-0.8.0/tests/test_dictionaries.py
+-rw-rw-rw-   0        0        0     1597 2023-01-17 21:17:22.000000 unyts-0.8.0/tests/test_operations.py
+-rw-rw-rw-   0        0        0      808 2023-01-30 12:24:34.000000 unyts-0.8.0/tests/test_uncertain_units.py
+-rw-rw-rw-   0        0        0     6368 2024-05-02 23:01:26.000000 unyts-0.8.0/tests/test_units.py
```

### Comparing `unyts-0.7.1/LICENSE` & `unyts-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unyts-0.7.1/PKG-INFO` & `unyts-0.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unyts
-Version: 0.7.1
+Version: 0.8.0
 Summary: a unit converter based on graph network and classes to operate with units.
 Author-email: Martin Carlos Araya <martinaraya@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Martín Carlos Araya
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,36 +34,43 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: stringthings
+Requires-Dist: cloudpickle
 
 [![Run tests](https://github.com/ayaranitram/unyts/actions/workflows/test-package.yml/badge.svg)](https://github.com/ayaranitram/unyts/actions/workflows/test-package.yml)
 [![PyPI version](https://img.shields.io/pypi/v/unyts.svg)](https://pypi.org/project/unyts/)
 [![PyPI versions](https://img.shields.io/pypi/pyversions/unyts.svg)](https://pypi.org/project/unyts//)
 [![PyPI license](https://img.shields.io/pypi/l/unyts.svg)](https://pypi.org/project/unyts/)
 
-# `unyts`
-  
-After culminating a project for a class from MITx courses, I saw the opportunity to use a *digraph network* to build a units converter able to convert from any units to any units without the need to populate a huge but finite table of possible conversions. Powered by the _Breadth First Search_, or _BFS_, algorithm to search through the network, this converter can find conversions from a particular Unit (or ratio of units) to any other Unit (or ratio) as long as a path connecting them exists.
+# `unyts`  
+
+<p align="center"><img src="unyts_icon_web.png" /></p>  
 
+I saw the opportunity to use a *digraph network* to build a units converter able to convert from any units to any units without the need to populate an endless table of possible conversions. Powered by the _Breadth First Search_, or _BFS_, algorithm to search through the network, this converter can find conversions from a particular Unit (or ratio of units) to any other Unit (or ratio) as long as a path connecting them exists.  
 This package is under development and is regularly updated. Back compatibility is intended to be maintained when possible.
   
 ## What do this package contains:
 - It is loaded with a network of units preloaded for distances, area, volume, mass and time conversions defined for SI and Imperial systems according to the definition of each Unit, i.e.: _1_foot = 12_inches_.
 - Prefixes applied to the basic units, like in SI units _k_ to _m_ to make _km_, are loaded as a network of conversion paths allowing the algorithm to apply the prefix to any other unit in the same system.
 - It provides a class _Unit_ powered with arithmetic and logic operations to intrinsically consider unit conversions when making calculations.  
   
 ## How to use this package:
-This package is intended to be used in two ways:  
+This package is intended to be used in three ways:  
 - Calling the function `units()` to define instances of the __Units__ class, that holds _values associated to units_, or, _quantities_.  
-- As unit converter with the function `convert()` to explicitly make conversion of numeric variables and instances.  
-  
+- As unit converter with the function `convert()` to explicitly make conversion of numeric variables and instances.
+- As unit converter for single numerical values, using the GUI.
+
+### To launch the GUI
+From an OS terminal or console, execute `python -m unyts`
+In the interface, simpy type in the units to convert and the value to be converted and click the *convert* button or hit _Enter_ key. 
+
 ### To use the _units converter_ function `convert()`:  
 `from unyts import convert`  
 `convert(value, from_units, to_units)`  
 where:  
 - _value_ is a number (int, float, numpy.array, etc)  
 - *from_units* is a string defining the units of _value_ (i.e.: 'ft')  
 - *to_units* is a string representing the units to convert _value_ (i.e.: 'km')
```

### Comparing `unyts-0.7.1/README.md` & `unyts-0.8.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 [![Run tests](https://github.com/ayaranitram/unyts/actions/workflows/test-package.yml/badge.svg)](https://github.com/ayaranitram/unyts/actions/workflows/test-package.yml)
 [![PyPI version](https://img.shields.io/pypi/v/unyts.svg)](https://pypi.org/project/unyts/)
 [![PyPI versions](https://img.shields.io/pypi/pyversions/unyts.svg)](https://pypi.org/project/unyts//)
 [![PyPI license](https://img.shields.io/pypi/l/unyts.svg)](https://pypi.org/project/unyts/)
 
-# `unyts`
-  
-After culminating a project for a class from MITx courses, I saw the opportunity to use a *digraph network* to build a units converter able to convert from any units to any units without the need to populate a huge but finite table of possible conversions. Powered by the _Breadth First Search_, or _BFS_, algorithm to search through the network, this converter can find conversions from a particular Unit (or ratio of units) to any other Unit (or ratio) as long as a path connecting them exists.
+# `unyts`  
+
+<p align="center"><img src="unyts_icon_web.png" /></p>  
 
+I saw the opportunity to use a *digraph network* to build a units converter able to convert from any units to any units without the need to populate an endless table of possible conversions. Powered by the _Breadth First Search_, or _BFS_, algorithm to search through the network, this converter can find conversions from a particular Unit (or ratio of units) to any other Unit (or ratio) as long as a path connecting them exists.  
 This package is under development and is regularly updated. Back compatibility is intended to be maintained when possible.
   
 ## What do this package contains:
 - It is loaded with a network of units preloaded for distances, area, volume, mass and time conversions defined for SI and Imperial systems according to the definition of each Unit, i.e.: _1_foot = 12_inches_.
 - Prefixes applied to the basic units, like in SI units _k_ to _m_ to make _km_, are loaded as a network of conversion paths allowing the algorithm to apply the prefix to any other unit in the same system.
 - It provides a class _Unit_ powered with arithmetic and logic operations to intrinsically consider unit conversions when making calculations.  
   
 ## How to use this package:
-This package is intended to be used in two ways:  
+This package is intended to be used in three ways:  
 - Calling the function `units()` to define instances of the __Units__ class, that holds _values associated to units_, or, _quantities_.  
-- As unit converter with the function `convert()` to explicitly make conversion of numeric variables and instances.  
-  
+- As unit converter with the function `convert()` to explicitly make conversion of numeric variables and instances.
+- As unit converter for single numerical values, using the GUI.
+
+### To launch the GUI
+From an OS terminal or console, execute `python -m unyts`
+In the interface, simpy type in the units to convert and the value to be converted and click the *convert* button or hit _Enter_ key. 
+
 ### To use the _units converter_ function `convert()`:  
 `from unyts import convert`  
 `convert(value, from_units, to_units)`  
 where:  
 - _value_ is a number (int, float, numpy.array, etc)  
 - *from_units* is a string defining the units of _value_ (i.e.: 'ft')  
 - *to_units* is a string representing the units to convert _value_ (i.e.: 'km')
```

#### html2text {}

```diff
@@ -1,52 +1,57 @@
 [![Run tests](https://github.com/ayaranitram/unyts/actions/workflows/test-
 package.yml/badge.svg)](https://github.com/ayaranitram/unyts/actions/workflows/
 test-package.yml) [![PyPI version](https://img.shields.io/pypi/v/unyts.svg)]
 (https://pypi.org/project/unyts/) [![PyPI versions](https://img.shields.io/
 pypi/pyversions/unyts.svg)](https://pypi.org/project/unyts//) [![PyPI license]
 (https://img.shields.io/pypi/l/unyts.svg)](https://pypi.org/project/unyts/) #
-`unyts` After culminating a project for a class from MITx courses, I saw the
-opportunity to use a *digraph network* to build a units converter able to
-convert from any units to any units without the need to populate a huge but
-finite table of possible conversions. Powered by the _Breadth First Search_, or
-_BFS_, algorithm to search through the network, this converter can find
+`unyts`
+                             [unyts_icon_web.png]
+I saw the opportunity to use a *digraph network* to build a units converter
+able to convert from any units to any units without the need to populate an
+endless table of possible conversions. Powered by the _Breadth First Search_,
+or _BFS_, algorithm to search through the network, this converter can find
 conversions from a particular Unit (or ratio of units) to any other Unit (or
 ratio) as long as a path connecting them exists. This package is under
 development and is regularly updated. Back compatibility is intended to be
 maintained when possible. ## What do this package contains: - It is loaded with
 a network of units preloaded for distances, area, volume, mass and time
 conversions defined for SI and Imperial systems according to the definition of
 each Unit, i.e.: _1_foot = 12_inches_. - Prefixes applied to the basic units,
 like in SI units _k_ to _m_ to make _km_, are loaded as a network of conversion
 paths allowing the algorithm to apply the prefix to any other unit in the same
 system. - It provides a class _Unit_ powered with arithmetic and logic
 operations to intrinsically consider unit conversions when making calculations.
-## How to use this package: This package is intended to be used in two ways: -
-Calling the function `units()` to define instances of the __Units__ class, that
-holds _values associated to units_, or, _quantities_. - As unit converter with
-the function `convert()` to explicitly make conversion of numeric variables and
-instances. ### To use the _units converter_ function `convert()`: `from unyts
-import convert` `convert(value, from_units, to_units)` where: - _value_ is a
-number (int, float, numpy.array, etc) - *from_units* is a string defining the
-units of _value_ (i.e.: 'ft') - *to_units* is a string representing the units
-to convert _value_ (i.e.: 'km') ### To create instances of the _Unit_ class
-using the `units()` function: `from unyts import units` `variable = units
-(value, units)` - _value_ is a number (`int`, `float`, `numpy.array`, etc) -
-_units_ is a string defining the units of _value_ (i.e.: 'ft') Then simply
-operate with the **Unit** instances or the variables related to them: In: units
-(6, 'in') + units(1, 'ft') Out: 18_in ### Referring to the `Unit` class: `from
-unyts import Unit` - The `Unit` class is not intended to be used to create
-**Unit _instances_**, but to allow checking if other object `isinstance` of
-**Unit**: i.e.: `isinstance(variable, Unit)` - In order to create instances of
-**Unit** it is convenient to use the `units()` function as it will return the
-appropriate **Unit _subclass_**. ### Uses examples: For further examples of
-use, the following Jupyter notebook _*_*_u_n_y_t_s___d_e_m_o_*_* intends to be a guide on how
-to use this converter and units classes. ## To install this package: Install it
-from the _p_y_p_i_._o_r_g repository: `pip install unyts` or upgrade to the latest
-version: `pip install --upgrade unyts` ## Optional requisites: The main
-functionalities are purely Python powered and does not require any other
-package to work but, if present, some commonly known packages are used to
-improve the operability of `unyts`: - `NumPy` to be able to deal with iterables
-not of nparray type, like (list of values) - `Pandas` to be able to recognize
-Series and DataFrames - `cloudpickle` to be able to save internal dictionaries
-and network to cache file, for faster loading - `openpyxl` if willing to export
-the units network to a pandas DataFrame
+## How to use this package: This package is intended to be used in three ways:
+- Calling the function `units()` to define instances of the __Units__ class,
+that holds _values associated to units_, or, _quantities_. - As unit converter
+with the function `convert()` to explicitly make conversion of numeric
+variables and instances. - As unit converter for single numerical values, using
+the GUI. ### To launch the GUI From an OS terminal or console, execute `python
+-m unyts` In the interface, simpy type in the units to convert and the value to
+be converted and click the *convert* button or hit _Enter_ key. ### To use the
+_units converter_ function `convert()`: `from unyts import convert` `convert
+(value, from_units, to_units)` where: - _value_ is a number (int, float,
+numpy.array, etc) - *from_units* is a string defining the units of _value_
+(i.e.: 'ft') - *to_units* is a string representing the units to convert _value_
+(i.e.: 'km') ### To create instances of the _Unit_ class using the `units()`
+function: `from unyts import units` `variable = units(value, units)` - _value_
+is a number (`int`, `float`, `numpy.array`, etc) - _units_ is a string defining
+the units of _value_ (i.e.: 'ft') Then simply operate with the **Unit**
+instances or the variables related to them: In: units(6, 'in') + units(1, 'ft')
+Out: 18_in ### Referring to the `Unit` class: `from unyts import Unit` - The
+`Unit` class is not intended to be used to create **Unit _instances_**, but to
+allow checking if other object `isinstance` of **Unit**: i.e.: `isinstance
+(variable, Unit)` - In order to create instances of **Unit** it is convenient
+to use the `units()` function as it will return the appropriate **Unit
+_subclass_**. ### Uses examples: For further examples of use, the following
+Jupyter notebook _*_*_u_n_y_t_s___d_e_m_o_*_* intends to be a guide on how to use this
+converter and units classes. ## To install this package: Install it from the
+_p_y_p_i_._o_r_g repository: `pip install unyts` or upgrade to the latest version: `pip
+install --upgrade unyts` ## Optional requisites: The main functionalities are
+purely Python powered and does not require any other package to work but, if
+present, some commonly known packages are used to improve the operability of
+`unyts`: - `NumPy` to be able to deal with iterables not of nparray type, like
+(list of values) - `Pandas` to be able to recognize Series and DataFrames -
+`cloudpickle` to be able to save internal dictionaries and network to cache
+file, for faster loading - `openpyxl` if willing to export the units network to
+a pandas DataFrame
```

### Comparing `unyts-0.7.1/pyproject.toml` & `unyts-0.8.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 2022 7365 7475 7074 6f6f 6c73 2e62 7569   "setuptools.bui
 00000050: 6c64 5f6d 6574 6122 0d0a 0d0a 5b74 6f6f  ld_meta"....[too
 00000060: 6c2e 7365 7475 7074 6f6f 6c73 2e70 6163  l.setuptools.pac
 00000070: 6b61 6765 732e 6669 6e64 5d0d 0a77 6865  kages.find]..whe
 00000080: 7265 203d 205b 2273 7263 225d 0d0a 0d0a  re = ["src"]....
 00000090: 5b70 726f 6a65 6374 5d0d 0a6e 616d 6520  [project]..name 
 000000a0: 3d20 2275 6e79 7473 220d 0a76 6572 7369  = "unyts"..versi
-000000b0: 6f6e 203d 2022 302e 372e 3122 0d0a 6175  on = "0.7.1"..au
+000000b0: 6f6e 203d 2022 302e 382e 3022 0d0a 6175  on = "0.8.0"..au
 000000c0: 7468 6f72 7320 3d20 5b0d 0a20 207b 206e  thors = [..  { n
 000000d0: 616d 653d 224d 6172 7469 6e20 4361 726c  ame="Martin Carl
 000000e0: 6f73 2041 7261 7961 222c 2065 6d61 696c  os Araya", email
 000000f0: 3d22 6d61 7274 696e 6172 6179 6140 676d  ="martinaraya@gm
 00000100: 6169 6c2e 636f 6d22 207d 2c0d 0a5d 0d0a  ail.com" },..]..
 00000110: 6465 7363 7269 7074 696f 6e20 3d20 2261  description = "a
 00000120: 2075 6e69 7420 636f 6e76 6572 7465 7220   unit converter 
@@ -45,17 +45,18 @@
 000002c0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
 000002d0: 203a 3a20 4d49 5420 4c69 6365 6e73 6522   :: MIT License"
 000002e0: 2c0d 0a20 2020 2022 4f70 6572 6174 696e  ,..    "Operatin
 000002f0: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
 00000300: 6e64 6570 656e 6465 6e74 222c 0d0a 5d0d  ndependent",..].
 00000310: 0a64 6570 656e 6465 6e63 6965 7320 3d20  .dependencies = 
 00000320: 5b0d 0a20 2020 2027 7374 7269 6e67 7468  [..    'stringth
-00000330: 696e 6773 270d 0a20 2020 205d 0d0a 5b70  ings'..    ]..[p
-00000340: 726f 6a65 6374 2e75 726c 735d 0d0a 2248  roject.urls].."H
-00000350: 6f6d 6570 6167 6522 203d 2022 6874 7470  omepage" = "http
-00000360: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
-00000370: 7961 7261 6e69 7472 616d 2f75 6e79 7473  yaranitram/unyts
-00000380: 220d 0a22 4275 6720 5472 6163 6b65 7222  ".."Bug Tracker"
-00000390: 203d 2022 6874 7470 733a 2f2f 6769 7468   = "https://gith
-000003a0: 7562 2e63 6f6d 2f61 7961 7261 6e69 7472  ub.com/ayaranitr
-000003b0: 616d 2f75 6e79 7473 2f69 7373 7565 7322  am/unyts/issues"
-000003c0: 0d0a                                     ..
+00000330: 696e 6773 272c 0d0a 2020 2020 2763 6c6f  ings',..    'clo
+00000340: 7564 7069 636b 6c65 270d 0a20 2020 205d  udpickle'..    ]
+00000350: 0d0a 5b70 726f 6a65 6374 2e75 726c 735d  ..[project.urls]
+00000360: 0d0a 2248 6f6d 6570 6167 6522 203d 2022  .."Homepage" = "
+00000370: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000380: 6f6d 2f61 7961 7261 6e69 7472 616d 2f75  om/ayaranitram/u
+00000390: 6e79 7473 220d 0a22 4275 6720 5472 6163  nyts".."Bug Trac
+000003a0: 6b65 7222 203d 2022 6874 7470 733a 2f2f  ker" = "https://
+000003b0: 6769 7468 7562 2e63 6f6d 2f61 7961 7261  github.com/ayara
+000003c0: 6e69 7472 616d 2f75 6e79 7473 2f69 7373  nitram/unyts/iss
+000003d0: 7565 7322 0d0a                           ues"..
```

### Comparing `unyts-0.7.1/src/unyts/__init__.py` & `unyts-0.8.0/src/unyts/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 # -*- coding: utf-8 -*-
 """
 Created on Sat Oct 24 18:24:20 2020
 
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
-__version__ = '0.7.1'
-__release__ = 20240211
+__version__ = '0.8.0'
+__release__ = 20240502
 __all__ = ['units', 'convert', 'convertible', 'Unit', 'is_Unit',
            'set_unit', 'set_conversion', 'set_density',
-           'save', 'start_gui']
+           'save', 'start_gui', 'set_fvf']
 
 from .parameters import unyts_parameters_, print_path, reload, raise_error, cache, set_density, get_density
-from .database import network_to_frame, save_memory, load_memory
+from .database import network_to_frame, save_memory, load_memory, set_fvf
 from .units.define import units
 from .converter import convert, convertible
 from .Empty import Empty
 from .unit_class import Unit, is_Unit
 from .units.custom import set_unit, set_conversion
 from .gui import start_gui
 
 if unyts_parameters_.show_version_:
-    print("loaded unyts version", __version__)
+    print(f"loaded unyts version {str(__version__)}")
     unyts_parameters_.show_version_ = False
     unyts_parameters_.save_params()
 
 from .unitary import *
 
 
 def save(path=None) -> None:
```

### Comparing `unyts-0.7.1/src/unyts/converter.py` & `unyts-0.8.0/src/unyts/converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 # -*- coding: utf-8 -*-
 """
 Created on Sat Oct 24 15:57:27 2020
 
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
-__version__ = '0.6.2'
-__release__ = 20240211
+__version__ = '0.6.4'
+__release__ = 20240502
 __all__ = ['convert', 'convertible']
 
 from .database import units_network
 from .dictionaries import dictionary, temperatureRatioConversions, uncertain_names
 from .Empty import Empty, str_Empty
 from .searches import BFS, print_path
 from .errors import NoConversionFoundError
 from .parameters import unyts_parameters_, _get_density
 from .helpers.unit_string_tools import split_unit as _split_unit, reduce_parentheses as _reduce_parentheses
 from functools import reduce
 from typing import Union
+from sys import getrecursionlimit
 import logging
 
 try:
     import numpy as np
     from numpy import ndarray
 
     _numpy_ = True
@@ -198,29 +199,38 @@
                 pair_child = sorted(pair_grandchild, key=len)[0]
                 break
 
     if type(pair_child) is str:
         return pair_child
 
 
-def _get_conversion(value, from_unit, to_unit):
+def _get_conversion(value, from_unit, to_unit, recursion=None):
     """
     Helper function to handle looking for the conversion factor of special cases and through the units network.
 
     Parameters
     ----------
     value: numeric or None
     from_unit: str
     to_unit: str
 
     Returns
     -------
         (conversion, conversion_path)
 
     """
+    # get and set recursion limit
+    if recursion is None:
+        recursion = min(getrecursionlimit()-15, 250)
+    elif recursion == 1:
+        return None, None
+    else:
+        recursion -= 1
+    # print(f"_get_conversion: {from_unit=}, {to_unit=}")
+
     # check if already solved and memorized
     if (from_unit, to_unit) in units_network.memory:
         conversion_lambda, conversion_path = units_network.memory[(from_unit, to_unit)]
         return (conversion_lambda, conversion_path) if (conversion_lambda is None or value is None) \
             else (conversion_lambda(value), conversion_path)
 
     # specific cases for quick conversions
@@ -256,15 +266,15 @@
 
     # special case for Temperature ratios
     if '/' in from_unit and len(from_unit.split('/')) == 2 and from_unit.split('/')[0] in dictionary['Temperature'] \
             and '/' in to_unit and len(to_unit.split('/')) == 2 and to_unit.split('/')[0] in dictionary['Temperature']:
         t1, d1 = from_unit.split('/')
         t2, d2 = to_unit.split('/')
         num = temperatureRatioConversions[(t1, t2)]
-        den, den_path = _get_conversion(1, d1, d2)
+        den, den_path = _get_conversion(1, d1, d2, recursion=recursion)
         if num is None or den is None:
             if unyts_parameters_.raise_error_:
                 raise NoConversionFoundError("from '" + str(d1) + "' to '" + str(d2) + "'")
             else:
                 return None, None
         den_path = [1] + den_path
         if value is None:
@@ -300,15 +310,15 @@
             return units_network.memory[(from_unit, to_unit)]
         else:
             return _apply_conversion(value, conversion_path), conversion_path
     else:
         return None, None
 
 
-def _converter(value, from_unit, to_unit):
+def _converter(value, from_unit, to_unit, recursion=None):
     """
     Transform the received value (integer, float, array, series, frame, ...)
     from the units `from_unit` to the units `to_units`
     as well as conversion path.
 
     Parameters
     ----------
@@ -316,19 +326,28 @@
     from_unit: str
     to_unit: str
 
     Returns
     -------
         (conversion, conversion_path)
     """
+    # get and set recursion limit
+    if recursion is None:
+        recursion = min(getrecursionlimit()-15, 250)
+    elif recursion == 1:
+        return None, None
+    else:
+        recursion -= 1
+    # print(f"_converter: {from_unit=}, {to_unit=}")
+
     # reset memory for this variable
     units_network.previous = []
 
     # try to convert
-    conv, conv_path = _get_conversion(value, from_unit, to_unit)
+    conv, conv_path = _get_conversion(value, from_unit, to_unit, recursion=recursion)
 
     # if Conversion found
     if conv is not None:
         return conv, conv_path
 
     units_network.previous.append((from_unit, to_unit))
 
@@ -343,15 +362,15 @@
         if split_from[f] in '*/':
             continue
         for t in range(len(split_to)):
             if t in used_to:
                 continue
             if split_to[t] in '*/':
                 continue
-            conv, conv_path = _get_conversion(1, split_from[f], split_to[t])
+            conv, conv_path = _get_conversion(1, split_from[f], split_to[t], recursion=recursion)
             if conv is not None:
                 flag = True
                 if len(list_conversion_path) > 0:
                     conv_path = [1] + conv_path
                 if (f > 0 and split_from[f - 1] == '/') or (t > 0 and split_to[t - 1] == '/'):
                     conv = 1 / conv
                     conv_path = ['/'] + conv_path
@@ -372,31 +391,31 @@
         else:
             return value * conversion_factor, conversion_path
 
     # look for one to pair conversion path
     if ('/' in to_unit or '*' in to_unit) and ('/' not in from_unit and '*' not in from_unit):
         from_unit_child = _get_pair_child(from_unit)
         if from_unit_child is not None:
-            base_conversion, base_conversion_path = _get_conversion(None, from_unit, from_unit_child)
-            pair_conversion, pair_conversion_path = _converter(None, from_unit_child, to_unit)
+            base_conversion, base_conversion_path = _get_conversion(None, from_unit, from_unit_child, recursion=recursion)
+            pair_conversion, pair_conversion_path = _converter(None, from_unit_child, to_unit, recursion=recursion)
             if pair_conversion is not None and base_conversion is not None:
                 conversion_path = base_conversion_path + pair_conversion_path
                 conversion = lambda x: pair_conversion(base_conversion(x))
                 units_network.memory[(from_unit, to_unit)] = conversion, conversion_path
                 if value is None:
                     return units_network.memory[(from_unit, to_unit)]
                 else:
                     return conversion(value), conversion_path
 
     # look for pair to one conversion path
     elif ('/' in from_unit or '*' in from_unit) and ('/' not in to_unit or '*' not in to_unit):
         to_unit_child = _get_pair_child(to_unit)
         if to_unit_child is not None:
-            final_conversion, final_conversion_path = _get_conversion(None, to_unit_child, to_unit)
-            pair_conversion, pair_conversion_path = _converter(None, from_unit, to_unit_child)
+            final_conversion, final_conversion_path = _get_conversion(None, to_unit_child, to_unit, recursion=recursion)
+            pair_conversion, pair_conversion_path = _converter(None, from_unit, to_unit_child, recursion=recursion)
             if pair_conversion is not None and final_conversion is not None:
                 conversion_path = pair_conversion_path + final_conversion_path
                 conversion = lambda x: final_conversion(pair_conversion(x))
                 units_network.memory[(from_unit, to_unit)] = conversion, conversion_path
                 if value is None:
                     return units_network.memory[(from_unit, to_unit)]
                 else:
```

### Comparing `unyts-0.7.1/src/unyts/database.py` & `unyts-0.8.0/src/unyts/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 # -*- coding: utf-8 -*-
 """
 Created on Sat Oct 24 12:36:48 2020
 
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
-__version__ = '0.5.30'
-__release__ = 20230724
-__all__ = ['units_network', 'network_to_frame', 'save_memory', 'load_memory']
+__version__ = '0.5.32'
+__release__ = 20240502
+__all__ = ['units_network', 'network_to_frame', 'save_memory', 'load_memory', 'clean_memory', 'delete_cache']
 
 import logging
+import os
+
 from .dictionaries import SI, SI_order, OGF, OGF_order, DATA, DATA_order, dictionary, StandardAirDensity, \
     StandardEarthGravity
 from .network import UDigraph, UNode, Conversion
 from .parameters import unyts_parameters_, dir_path
 from os.path import isfile
 from json import dump as json_dump
 
@@ -33,14 +35,58 @@
     units_network.save_memory(path)
 
 
 def load_memory(path=None) -> None:
     units_network.load_memory(path)
 
 
+def clean_memory(path=None) -> None:
+    units_network.clean_memory()
+
+
+def delete_cache() -> None:
+    for each in ('units/search_memory.cache', 'units/units_network.cache', 'units/units_dictionary.cache',
+                 'units/temperature_ratio_conversions.cache', 'units/unitless_names.cache'):
+        path = dir_path + each
+        if os.path.exists(path):
+            os.remove(path)
+
+
+def set_fvf(fvf=None) -> None:
+    def valid_fvf(fvf):
+        if type(fvf) is str:
+            try:
+                fvf = float(fvf)
+            except ValueError:
+                return False
+        if type(fvf) in (int, float):
+            if fvf <= 0:
+                return False
+            else:
+                return fvf
+        else:
+            return False
+    if fvf is None:
+        print('Please enter formation Volume factor (FVF) in reservoir_volume/standard_volume:')
+        while fvf is None:
+            fvf = input(' FVF (rV/stV) = ')
+            if not valid_fvf(fvf):
+                fvf = None
+            else:
+                fvf = valid_fvf(fvf)
+    units_network.set_fvf(fvf)
+
+
+def get_fvf() -> None:
+    if units_network.fvf is not None:
+        return str(round(units_network.fvf, 3))
+    else:
+        return ""
+
+
 def _load_network():
     logging.info('preparing units network...')
     network = UDigraph()
 
     for unit_kind in dictionary:
         if '_' not in unit_kind:
             for unit_name in dictionary[unit_kind]:
@@ -104,38 +150,50 @@
                     network.add_node(UNode(prefix + unit_name))
                     network.add_edge(
                         Conversion(network.get_node(prefix + unit_name), network.get_node(unit_name), SI[prefix][0]))
                     network.add_edge(
                         Conversion(network.get_node(unit_name), network.get_node(prefix + unit_name), SI[prefix][0],
                                    True))
                     dictionary[unit_kind.split('_')[0]].append(prefix + unit_name)
-        if '_SI' in unit_kind and unit_kind.split('_')[0] in SI_order[1]:
+        elif '_SI' in unit_kind and unit_kind.split('_')[0] in SI_order[1]:
             for unit_name in dictionary[unit_kind]:
                 network.add_node(UNode(unit_name))
                 dictionary[unit_kind.split('_')[0]].append(unit_name)
                 for prefix in SI:
                     network.add_node(UNode(prefix + unit_name))
                     network.add_edge(
                         Conversion(network.get_node(prefix + unit_name), network.get_node(unit_name), SI[prefix][1]))
                     network.add_edge(
                         Conversion(network.get_node(unit_name), network.get_node(prefix + unit_name), SI[prefix][1],
                                    True))
                     dictionary[unit_kind.split('_')[0]].append(prefix + unit_name)
-        if '_SI' in unit_kind and unit_kind.split('_')[0] in SI_order[2]:
+        elif '_SI' in unit_kind and unit_kind.split('_')[0] in SI_order[2]:
             for unit_name in dictionary[unit_kind]:
                 network.add_node(UNode(unit_name))
                 dictionary[unit_kind.split('_')[0]].append(unit_name)
                 for prefix in SI:
                     network.add_node(UNode(prefix + unit_name))
                     network.add_edge(
                         Conversion(network.get_node(prefix + unit_name), network.get_node(unit_name), SI[prefix][2]))
                     network.add_edge(
                         Conversion(network.get_node(unit_name), network.get_node(prefix + unit_name), SI[prefix][2],
                                    True))
                     dictionary[unit_kind.split('_')[0]].append(prefix + unit_name)
+        elif '_linearSI' in unit_kind and unit_kind.split('_')[0] in SI_order[2]:
+            for unit_name in dictionary[unit_kind]:
+                network.add_node(UNode(unit_name))
+                dictionary[unit_kind.split('_')[0]].append(unit_name)
+                for prefix in SI:
+                    network.add_node(UNode(prefix + unit_name))
+                    network.add_edge(
+                        Conversion(network.get_node(prefix + unit_name), network.get_node(unit_name), SI[prefix][0]))
+                    network.add_edge(
+                        Conversion(network.get_node(unit_name), network.get_node(prefix + unit_name), SI[prefix][0],
+                                   True))
+                    dictionary[unit_kind.split('_')[0]].append(prefix + unit_name)
         if '_DATA' in unit_kind and unit_kind.split('_')[0] in DATA_order[0]:
             for unit_name in dictionary[unit_kind]:
                 network.add_node(UNode(unit_name))
                 dictionary[unit_kind.split('_')[0]].append(unit_name)
                 for prefix in DATA:
                     network.add_node(UNode(prefix + unit_name))
                     network.add_edge(
@@ -453,15 +511,15 @@
     # Density Conversion
     network.add_edge(Conversion(network.get_node('API'), network.get_node('SgO'), lambda d: 141.5 / (131.5 + d)))
     network.add_edge(Conversion(network.get_node('SgO'), network.get_node('API'), lambda d: 141.5 / d - 131.5))
     network.add_edge(Conversion(network.get_node('API'), network.get_node('g/cc'), lambda d: 141.5 / (131.5 + d)))
     network.add_edge(Conversion(network.get_node('g/cc'), network.get_node('API'), lambda d: 141.5 / d - 131.5))
     network.add_edge(Conversion(network.get_node('SgO'), network.get_node('g/cc'), lambda d: d))
     network.add_edge(Conversion(network.get_node('SgW'), network.get_node('g/cc'), lambda d: d))
-    network.add_edge(Conversion(network.get_node('SgG'), network.get_node('g/cc'), lambda d: d * StandardAirDensity))
+    network.add_edge(Conversion(network.get_node('SgG'), network.get_node('kg/m3'), lambda d: d * StandardAirDensity))
     network.add_edge(Conversion(network.get_node('psia/ft'), network.get_node('lb/ft3'), lambda d: d * 144))
     network.add_edge(
         Conversion(network.get_node('g/cm3'), network.get_node('lb/ft3'), lambda d: d * 62.427960576144606))
     network.add_edge(Conversion(network.get_node('lb/ft3'), network.get_node('lb/stb'), lambda d: d * 5.614584))
 
     # viscosity conversions
     network.add_edge(Conversion(network.get_node('Pa*s'), network.get_node('Poise'), lambda v: v * 10))
```

### Comparing `unyts-0.7.1/src/unyts/dictionaries.py` & `unyts-0.8.0/src/unyts/dictionaries.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 # -*- coding: utf-8 -*-
 """
 Created on Sat Oct 24 12:14:51 2020
 
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
-__version__ = '0.5.30'
-__release__ = 20230724
+__version__ = '0.5.31'
+__release__ = 20240502
 __all__ = ['dictionary', 'SI', 'OGF', 'DATA', 'StandardAirDensity', 'StandardEarthGravity', 'unitless_names',
            'uncertain_names']
 
 import logging
 from json import load as json_load
 from pickle import load as pickle_load, dump as pickle_dump
 from os.path import isfile
@@ -44,15 +44,15 @@
     'p': (lambda X: X * 1E-12, lambda X: X * 1E-24, lambda X: X * 1E-36),  # pico
     'f': (lambda X: X * 1E-15, lambda X: X * 1E-30, lambda X: X * 1E-45),  # femto
     'a': (lambda X: X * 1E-18, lambda X: X * 1E-36, lambda X: X * 1E-54),  # atto
     'z': (lambda X: X * 1E-21, lambda X: X * 1E-42, lambda X: X * 1E-63),  # zepto
     'y': (lambda X: X * 1E-24, lambda X: X * 1E-48, lambda X: X * 1E-72),  # yocto
 }
 
-SI_order = (('Length', 'Pressure', 'Weight', 'Mass', 'Time', 'Frequency', 'Power', 'Voltage', 'Current', 'Resistance'),
+SI_order = (('Length', 'Pressure', 'Weight', 'Mass', 'Time', 'Frequency', 'Power', 'Voltage', 'Current', 'Resistance',),
             ('Area',),
             ('Rate', 'Volume',),)
 
 DATA = {
     'Y': (lambda X: X * 1E+24, lambda X: X * 2 ** 80),  # yotta
     'Z': (lambda X: X * 1E+21, lambda X: X * 2 ** 70),  # zetta
     'E': (lambda X: X * 1E+18, lambda X: X * 2 ** 60),  # exa
@@ -122,15 +122,15 @@
                                                   for key in dictionary['Temperature_NAMES']
                                                   for t in dictionary['Temperature_NAMES'][key] if len(t) > 1)
     dictionary['TemperatureGradient'] = []
 
     # Volume
     dictionary['Volume'] = []
     dictionary['Volume_SI_UPPER'] = (
-        'm3', 'sm3', 'stm3', 'rm3',)  # 'l' # litre is Volume but the Conversion of SI prefixes is linear
+        'm3',)  # 'l', 'sm3', 'rm3' are Volume but the conversion of SI prefixes is linear
     dictionary['Volume_UK_NAMES_REVERSE'] = {
         'fluid ounce': ('fl oz', 'oz', 'ounce', 'ozUS'),
         'gill': ('gi', 'gillUS', 'giUS', 'USgill'),
         'pint': ('pt', 'pintUS', 'ptUS', 'USpint'),
         'quart': ('qt', 'quartUS', 'qtUS', 'USquart'),
         'gallonUS': ('gal', 'galUS', 'USgal', 'USgallon', 'gallon', 'gallonsUS'),
         'gallonUK': ('imperial gallon', 'galUK', 'UKgal', 'UKgallon', 'gallonsUK'),  # 'gal', 'gallon'
@@ -141,52 +141,53 @@
     }
     dictionary['Volume_NAMES_SPACES_REVERSE'] = {
         'litre': ('l', 'liter', 'litro'),
         'millilitre': ('ml', 'milliliter', 'cubic centimeter'),
         'centilitre': ('cl', 'centiliter'),
         'decilitre': ('dl', 'deciliter'),
         'cubic meter': ('CM', 'm3'),
-        'standard cubic meter': ('scm', 'sm3', 'stm3', 'm3'),
+        'standard cubic meter': ('scm', 'sm3', 'stm3', 'm3', 'Sm3'),
         'cubic centimeter': ('cc', 'cm3', 'standard cubic centimeter'),
         'standard cubic centimeter': ('scc', 'scm3'),
-        'reservoir cubic meter': ('rm3',),
+        'reservoir cubic meter': ('rm3', 'Rm3'),
         'reservoir cubic centimeter': ('rcc', 'rcm3'),
         'cubic foot': ('cubic feet', 'ft3', 'cf', 'pie cúbico', 'pie cubico', 'pc', 'pies cúbicos', 'pies cubicos'),
         'standard cubic foot': ('scf', 'cf'),
         'cubic inch': ('in3', 'cubic inches'),
         'barrel': ('bbl', 'stb', 'oil barrel'),
         'reservoir barrel': ('rb',),
         'standard barrel': ('stb', 'stbo', 'stbw', 'stbl', 'oil barrel'),
     }
-    dictionary['Volume_UPPER'] = ('kstm3', 'Mstm3')
+    dictionary['Volume_UPPER'] = ('sm3', 'rm3', 'kstm3', 'Mstm3')
     dictionary['Volume_PLURALwS_UPPER_LOWER'] = tuple(dictionary['Volume_NAMES_SPACES_REVERSE'].keys()) + \
                                                 tuple(dictionary['Volume_UK_NAMES_REVERSE'].keys()) + \
                                                 ('fl oz', 'oz', 'ounce', 'gallon', 'imperial gallon', 'barrel', 'gal',
                                                  'oil barrel', 'oil gallon',
                                                  'USgallon', 'UKgallon', 'USounce', 'UKounce',
                                                  'cubic centimeter', 'standard cubic centimeter',
                                                  'liter', 'milliliter', 'centiliter', 'deciliter')
     dictionary['Volume_OGF'] = ('scf', 'cf', 'ft3', 'stb', 'bbl', 'rb', 'stbo', 'stbw', 'stbl')
     # dictionary['Volume_oilgas_NAMES'] = ('scf','cf','ft3','stb','bbl','rb','stbo','stbw','stbl')
-    dictionary['Volume_oilgas_UPPER'] = ('sm3', 'm3', 'rm3', 'ksm3', 'Msm3', 'Gsm3',
+    dictionary['Volume_oilgas_UPPER'] = ('sm3', 'Sm3', 'm3', 'rm3', 'Rm3', 'ksm3', 'Msm3', 'Gsm3',
                                          'scf', 'cf', 'ft3', 'Mscf', 'MMscf', 'Bscf', 'Tscf', 'Mcf', 'MMcf', 'Bcf',
                                          'Tcf',
                                          'stb', 'bbl', 'rb', 'Mstb', 'MMstb', 'Bstb', 'Tstb', 'Mbbl', 'MMbbl', 'Mrb',
                                          'MMrb')
     dictionary['Volume_product_NAMES_REVERSE'] = {
         'm3': ('m2*m',),
         'cm3': ('cm2*cm',),
         'ft3': ('ft2*ft',),
         'in3': ('in2*in',)
     }
+    dictionary['Volume_linearSI'] = ('sm3', 'rm3',)
 
     # Length
     dictionary['Length'] = []
     dictionary['Length_NAMES_REVERSE_UPPER'] = {'meter': ('m', 'meter', 'metro')}
-    dictionary['Length_SI'] = ('m', 'l')  # litre is Volume but the Conversion of SI prefixes is linear
+    dictionary['Length_SI'] = ('m', 'l',)  # litre, sm3 and rm3 are Volume but the conversion of SI prefixes is linear
     dictionary['Length_UK_NAMES_REVERSE'] = {
         'thou': ('th',),
         'tenth': ('te', '0.1 in', '0.1in', '.1in'),
         'inch': ('in', '"'),
         'foot': ('feet', 'ft', "'"),
         'yard': ('yd',),
         'chain': ('ch',),
@@ -274,17 +275,17 @@
     }
 
     # Density
     dictionary['Density'] = []
     dictionary['Density_oilgas'] = {}
     dictionary['Density_NAMES_REVERSE_LOWER_UPPER'] = {
         'API': ('degrees',),
-        'SgG': ('gas gravity', 'gas specific gravity'),
-        'SgW': ('water gravity',),
-        'SgO': ('oil gravity',),
+        'SgG': ('gas gravity', 'gas specific gravity', 'sgg'),
+        'SgW': ('water gravity', 'sgw'),
+        'SgO': ('oil gravity', 'sgo'),
     }
     dictionary['Density_NAMES_REVERSE_UPPER'] = {
         'g/cm3': ('g/cc',),
         'kg/m3': ('Kg/m3',),
         'lb/ft3': tuple(),
         'psi/ft': tuple(),
         'kJ/rm3': ('KJ/rm3',),
```

### Comparing `unyts-0.7.1/src/unyts/errors.py` & `unyts-0.8.0/src/unyts/errors.py`

 * *Files identical despite different names*

### Comparing `unyts-0.7.1/src/unyts/gui.py` & `unyts-0.8.0/src/unyts/gui.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,28 +2,34 @@
 # -*- coding: utf-8 -*-
 """
 Created on Sat Feb 11 10:38:47 2024
 
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
-__version__ = '0.1.0'
-__release__ = 20240211
+__version__ = '0.2.1'
+__release__ = 20240502
 __all__ = ['start_gui']
 
+import logging
 import tkinter as tk
 from tkinter import ttk
 from stringthings import get_number, is_numeric
 from .converter import convert
 from .dictionaries import _all_units
 from .errors import NoConversionFoundError
+from .database import save_memory, load_memory, clean_memory, delete_cache, unyts_parameters_, set_fvf
 import pathlib, os
 
+
 _all_units_str = _all_units()
+
+
 class UnytsApp(tk.Frame):
+
     def __init__(self, master=None):
         super().__init__(master)
         self.pack()
 
         ttk.Label(text="Unyts converter", font=(None, 16, 'bold'), padding=5).pack()
 
         frame = ttk.Frame(padding=5)
@@ -49,15 +55,14 @@
         self.to_unit.grid(column=1, row=2, pady=3, padx=1)
         self.to_unit.bind('<Key-Return>', self._calculate)
         self.to_value_val = tk.StringVar()
         self.to_value = ttk.Entry(frame, textvariable=self.to_value_val)
         self.to_value.grid(column=2, row=2, pady=3, padx=1)
         self.to_value.bind('<Key-Return>', self._rcalculate)
 
-
         self.button_text = tk.StringVar()
         self.button_text.set("convert")
         self.convert_button = ttk.Button(frame, textvariable=self.button_text)
         self.convert_button.grid(columnspan=3, row=3, pady=7)
         self.convert_button.bind('<ButtonRelease>', self._calculate)
         self.frame.bind('<Motion>', lambda x: self.button_text.set("convert"))
 
@@ -104,42 +109,75 @@
                 self.to_unit_val.set(to_unit)
                 return None, None
         return to_unit, to_value
 
     def _calculate(self, *args):
         from_unit, from_value = self._get_from()
         to_unit = self.to_unit_val.get()
+        self.to_value_val.set("")
         try:
             to_value = convert(from_value, from_unit, to_unit,
                                print_conversion_path=False)
             self.to_value_val.set(str(to_value))
         except NoConversionFoundError:
             self.button_text.set("no conversion found!")
 
     def _rcalculate(self, *args):
         from_unit, from_value = self._get_to()
         to_unit = self.from_unit_val.get()
+        self.from_value_val.set("")
         try:
             to_value = convert(from_value, from_unit, to_unit,
                                print_conversion_path=False)
             self.from_value_val.set(str(to_value))
         except NoConversionFoundError:
             self.button_text.set("no conversion found!")
 
+
 def start_gui():
     def close_gui():
-        print("INFO:shutting down Unyts.")
+        logging.info("saving memory...")
+        save_memory()
+        logging.info("INFO:shutting down Unyts.")
         root.destroy()
-    w, h = 325, 175
+    if unyts_parameters_.memory_:
+        load_memory()
+    else:
+        delete_cache()
+
+    logging.info("starting Unyts GUI...")
+    w, h = 325, 185
     root = tk.Tk(screenName='Unyts')
     root.geometry(f"{w}x{h}")
     root.maxsize(w, h)
     root.minsize(w, h)
     root.resizable(False, False)
-    icon_file = 'openbook.ico'
+    icon_file = 'unyts_icon.ico'
     current_dir = pathlib.Path(__file__).parent.resolve()
     icon_path = os.path.join(current_dir, icon_file)
     root.iconbitmap(icon_path)
+
+    # setting menu
+    root.option_add('*tearOff', False)
+    unyts_menu = tk.Menu(root)
+    root.config(menu=unyts_menu)
+    # File menu
+    file_menu = tk.Menu(unyts_menu)
+    unyts_menu.add_cascade(label='File', menu=file_menu)
+    file_menu.add_command(label='Save memory', command=save_memory)
+    file_menu.add_command(label='Reload memory', command=load_memory)
+    file_menu.add_command(label='Clean memory', command=clean_memory)
+    file_menu.add_command(label='Delete cache', command=delete_cache)
+    file_menu.add_separator()
+    file_menu.add_command(label='Exit', command=close_gui)
+    # Options menu
+    options_menu = tk.Menu(unyts_menu)
+    unyts_menu.add_cascade(label='Options', menu=options_menu)
+    options_menu.add_command(label="Set FVF in CMD", command=set_fvf)
+    # options_menu.add_checkbutton(label='Print path', onvalue=True, offvalue=False, variable=unyts_parameters_.print_path_)
+    # options_menu.add_checkbutton(label='Cache', onvalue=True, offvalue=False, variable=unyts_parameters_.cache_)
+    # options_menu.add_checkbutton(label='Reload on next start', onvalue=True, offvalue=False, variable=unyts_parameters_.reload_)
+
     unyts_gui = UnytsApp()
     unyts_gui.master.title("Unyts converter")
     root.protocol("WM_DELETE_WINDOW", close_gui)
     unyts_gui.mainloop()
```

### Comparing `unyts-0.7.1/src/unyts/helpers/caster.py` & `unyts-0.8.0/src/unyts/helpers/caster.py`

 * *Files identical despite different names*

### Comparing `unyts-0.7.1/src/unyts/helpers/common_classes.py` & `unyts-0.8.0/src/unyts/helpers/common_classes.py`

 * *Files identical despite different names*

### Comparing `unyts-0.7.1/src/unyts/helpers/is_number.py` & `unyts-0.8.0/src/unyts/helpers/is_number.py`

 * *Files identical despite different names*

### Comparing `unyts-0.7.1/src/unyts/helpers/is_unit.py` & `unyts-0.8.0/src/unyts/helpers/is_unit.py`

 * *Files identical despite different names*

### Comparing `unyts-0.7.1/src/unyts/helpers/multi_split.py` & `unyts-0.8.0/src/unyts/helpers/multi_split.py`

 * *Files identical despite different names*

### Comparing `unyts-0.7.1/src/unyts/helpers/unit_string_tools.py` & `unyts-0.8.0/src/unyts/helpers/unit_string_tools.py`

 * *Files identical despite different names*

### Comparing `unyts-0.7.1/src/unyts/network.py` & `unyts-0.8.0/src/unyts/network.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 # -*- coding: utf-8 -*-
 """
 Created on Sat Oct 24 12:36:48 2020
 
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 import logging
-import os.path
+from os.path import isfile
 from .parameters import unyts_parameters_, dir_path
 
 try:
     from cloudpickle import dump as cloudpickle_dump, load as cloudpickle_load
 
     _cloudpickle_ = True
 except ModuleNotFoundError:
     _cloudpickle_ = False
 
 logging.basicConfig(format='%(levelname)s:%(message)s', level=logging.INFO)
 
-__version__ = '0.4.9'
-__release__ = 20230127
+__version__ = '0.4.12'
+__release__ = 20240502
 __all__ = ['UNode', 'UDigraph', 'Conversion']
 
 
 class UNode(object):
     __slots__ = ('name',)
 
     def __init__(self, name):
@@ -44,40 +44,45 @@
         self.edges = {}
         self.previous = [(None, None)]
         self.recursion_limit = 5
         self.fvf = None
         self.memory = {}
         self.print = False
         self._cloudpickle_ = _cloudpickle_
-        if unyts_parameters_.cache_:
+        if unyts_parameters_.cache_ and unyts_parameters_.memory_:
             self.load_memory()
 
     def save_memory(self, path=None) -> None:
         if path is None:
             path = dir_path + 'units/search_memory.cache'
         if self._cloudpickle_:
-            print('saving search memory to cache...')
+            logging.info('saving search memory to cache...')
             with open(path, 'wb') as f:
                 cloudpickle_dump(self.memory, f)
         else:
             logging.warning("Missing `cloudpickle` package. Not able to cache search memory.")
 
     def load_memory(self, path=None) -> None:
         if path is None:
             path = dir_path + 'units/search_memory.cache'
-        if self._cloudpickle_ and os.path.isfile(dir_path + 'units/search_memory.cache'):
+        if not self._cloudpickle_:
+            logging.warning("Missing `cloudpickle` package. Not able to cache search memory.")
+        if not isfile(dir_path + 'units/search_memory.cache'):
+            logging.info("starting clean memory...")
+        else:
+            logging.info('loading memory from cache...')
             try:
-                print('loading search memory from cache...')
-                with open(path, 'wb') as f:
+                with open(path, 'rb') as f:
                     cached_memory = cloudpickle_load(f)
                     self.memory.update(cached_memory)
             except:
-                print('not able to load memory from cache.')
-        elif not self._cloudpickle_:
-            logging.warning("Missing `cloudpickle` package. Not able to cache search memory.")
+                logging.error('not able to load memory from cache.')
+
+    def clean_memory(self):
+        self.memory = {}
 
     def add_node(self, node) -> None:
         if node in self.edges:
             raise ValueError('Duplicate node')
         else:
             self.edges[node] = [], []
 
@@ -133,15 +138,15 @@
         return result[:-1]  # remove final \n
 
     def set_fvf(self, FVF) -> None:
         if type(FVF) is str:
             try:
                 FVF = float(FVF)
             except ValueError:
-                print('received FVF value is not a number: ' + str(FVF))
+                print(f'received FVF value is not a number: {str(FVF)}')
         if type(FVF) in (int, float):
             if FVF <= 0:
                 logging.error('FVF should be a positive number...')
             self.fvf = FVF
 
     def get_fvf(self):
         def valid_fvf(FVF):
```

### Comparing `unyts-0.7.1/src/unyts/operations.py` & `unyts-0.8.0/src/unyts/operations.py`

 * *Files identical despite different names*

### Comparing `unyts-0.7.1/src/unyts/parameters.py` & `unyts-0.8.0/src/unyts/parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 # -*- coding: utf-8 -*-
 """
 Created on Sat Oct 24 18:24:20 2020
 
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
-__version__ = '0.5.2'
-__release__ = 20230107
+__version__ = '0.5.3'
+__release__ = 20240502
 __all__ = ['unyts_parameters_', 'print_path', 'reload', 'raise_error', 'cache', 'dir_path', 'set_density']
 
 import logging
 import os.path
 from json import load as json_load, dump as json_dump
 from os.path import isfile
 from pathlib import Path
@@ -32,14 +32,15 @@
         self.raise_error_ = True
         self.verbose_ = False
         self.reduce_parentheses_ = True
         self.show_version_ = True
         self.density_ = None
         self.load_params()
         self.reload_ = self.reload_ if reload is None else bool(reload)
+        self.memory_ = not self.reload_
 
     def load_params(self) -> None:
         if isfile(ini_path):
             with open(ini_path, 'r') as f:
                 params = json_load(f)
         else:
             params = {'print_path_': False,
```

### Comparing `unyts-0.7.1/src/unyts/searches.py` & `unyts-0.8.0/src/unyts/searches.py`

 * *Files identical despite different names*

### Comparing `unyts-0.7.1/src/unyts/unit_class.py` & `unyts-0.8.0/src/unyts/unit_class.py`

 * *Files identical despite different names*

### Comparing `unyts-0.7.1/src/unyts/unitary.py` & `unyts-0.8.0/src/unyts/unitary.py`

 * *Files identical despite different names*

### Comparing `unyts-0.7.1/src/unyts/units/custom.py` & `unyts-0.8.0/src/unyts/units/custom.py`

 * *Files identical despite different names*

### Comparing `unyts-0.7.1/src/unyts/units/data.py` & `unyts-0.8.0/src/unyts/units/data.py`

 * *Files identical despite different names*

### Comparing `unyts-0.7.1/src/unyts/units/date.py` & `unyts-0.8.0/src/unyts/units/date.py`

 * *Files identical despite different names*

### Comparing `unyts-0.7.1/src/unyts/units/define.py` & `unyts-0.8.0/src/unyts/units/define.py`

 * *Files identical despite different names*

### Comparing `unyts-0.7.1/src/unyts/units/energy.py` & `unyts-0.8.0/src/unyts/units/energy.py`

 * *Files identical despite different names*

### Comparing `unyts-0.7.1/src/unyts/units/force.py` & `unyts-0.8.0/src/unyts/units/force.py`

 * *Files identical despite different names*

### Comparing `unyts-0.7.1/src/unyts/units/geometry.py` & `unyts-0.8.0/src/unyts/units/geometry.py`

 * *Files identical despite different names*

### Comparing `unyts-0.7.1/src/unyts/units/mass.py` & `unyts-0.8.0/src/unyts/units/mass.py`

 * *Files identical despite different names*

### Comparing `unyts-0.7.1/src/unyts/units/rates.py` & `unyts-0.8.0/src/unyts/units/rates.py`

 * *Files identical despite different names*

### Comparing `unyts-0.7.1/src/unyts/units/ratios.py` & `unyts-0.8.0/src/unyts/units/ratios.py`

 * *Files identical despite different names*

### Comparing `unyts-0.7.1/src/unyts/units/temperature.py` & `unyts-0.8.0/src/unyts/units/temperature.py`

 * *Files identical despite different names*

### Comparing `unyts-0.7.1/src/unyts/units/time.py` & `unyts-0.8.0/src/unyts/units/time.py`

 * *Files identical despite different names*

### Comparing `unyts-0.7.1/src/unyts/units/unitless.py` & `unyts-0.8.0/src/unyts/units/unitless.py`

 * *Files identical despite different names*

### Comparing `unyts-0.7.1/src/unyts.egg-info/PKG-INFO` & `unyts-0.8.0/src/unyts.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unyts
-Version: 0.7.1
+Version: 0.8.0
 Summary: a unit converter based on graph network and classes to operate with units.
 Author-email: Martin Carlos Araya <martinaraya@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Martín Carlos Araya
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,36 +34,43 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: stringthings
+Requires-Dist: cloudpickle
 
 [![Run tests](https://github.com/ayaranitram/unyts/actions/workflows/test-package.yml/badge.svg)](https://github.com/ayaranitram/unyts/actions/workflows/test-package.yml)
 [![PyPI version](https://img.shields.io/pypi/v/unyts.svg)](https://pypi.org/project/unyts/)
 [![PyPI versions](https://img.shields.io/pypi/pyversions/unyts.svg)](https://pypi.org/project/unyts//)
 [![PyPI license](https://img.shields.io/pypi/l/unyts.svg)](https://pypi.org/project/unyts/)
 
-# `unyts`
-  
-After culminating a project for a class from MITx courses, I saw the opportunity to use a *digraph network* to build a units converter able to convert from any units to any units without the need to populate a huge but finite table of possible conversions. Powered by the _Breadth First Search_, or _BFS_, algorithm to search through the network, this converter can find conversions from a particular Unit (or ratio of units) to any other Unit (or ratio) as long as a path connecting them exists.
+# `unyts`  
+
+<p align="center"><img src="unyts_icon_web.png" /></p>  
 
+I saw the opportunity to use a *digraph network* to build a units converter able to convert from any units to any units without the need to populate an endless table of possible conversions. Powered by the _Breadth First Search_, or _BFS_, algorithm to search through the network, this converter can find conversions from a particular Unit (or ratio of units) to any other Unit (or ratio) as long as a path connecting them exists.  
 This package is under development and is regularly updated. Back compatibility is intended to be maintained when possible.
   
 ## What do this package contains:
 - It is loaded with a network of units preloaded for distances, area, volume, mass and time conversions defined for SI and Imperial systems according to the definition of each Unit, i.e.: _1_foot = 12_inches_.
 - Prefixes applied to the basic units, like in SI units _k_ to _m_ to make _km_, are loaded as a network of conversion paths allowing the algorithm to apply the prefix to any other unit in the same system.
 - It provides a class _Unit_ powered with arithmetic and logic operations to intrinsically consider unit conversions when making calculations.  
   
 ## How to use this package:
-This package is intended to be used in two ways:  
+This package is intended to be used in three ways:  
 - Calling the function `units()` to define instances of the __Units__ class, that holds _values associated to units_, or, _quantities_.  
-- As unit converter with the function `convert()` to explicitly make conversion of numeric variables and instances.  
-  
+- As unit converter with the function `convert()` to explicitly make conversion of numeric variables and instances.
+- As unit converter for single numerical values, using the GUI.
+
+### To launch the GUI
+From an OS terminal or console, execute `python -m unyts`
+In the interface, simpy type in the units to convert and the value to be converted and click the *convert* button or hit _Enter_ key. 
+
 ### To use the _units converter_ function `convert()`:  
 `from unyts import convert`  
 `convert(value, from_units, to_units)`  
 where:  
 - _value_ is a number (int, float, numpy.array, etc)  
 - *from_units* is a string defining the units of _value_ (i.e.: 'ft')  
 - *to_units* is a string representing the units to convert _value_ (i.e.: 'km')
```

### Comparing `unyts-0.7.1/src/unyts.egg-info/SOURCES.txt` & `unyts-0.8.0/src/unyts.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 src/unyts/__main__.py
 src/unyts/converter.py
 src/unyts/database.py
 src/unyts/dictionaries.py
 src/unyts/errors.py
 src/unyts/gui.py
 src/unyts/network.py
-src/unyts/openbook.ico
 src/unyts/operations.py
 src/unyts/parameters.ini
 src/unyts/parameters.py
 src/unyts/searches.py
 src/unyts/unit_class.py
 src/unyts/unitary.py
+src/unyts/unyts_icon.ico
 src/unyts.egg-info/PKG-INFO
 src/unyts.egg-info/SOURCES.txt
 src/unyts.egg-info/dependency_links.txt
 src/unyts.egg-info/requires.txt
 src/unyts.egg-info/top_level.txt
 src/unyts/helpers/__init__.py
 src/unyts/helpers/caster.py
```

### Comparing `unyts-0.7.1/tests/test_converter.py` & `unyts-0.8.0/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `unyts-0.7.1/tests/test_dictionaries.py` & `unyts-0.8.0/tests/test_dictionaries.py`

 * *Files identical despite different names*

### Comparing `unyts-0.7.1/tests/test_operations.py` & `unyts-0.8.0/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `unyts-0.7.1/tests/test_uncertain_units.py` & `unyts-0.8.0/tests/test_uncertain_units.py`

 * *Files identical despite different names*

### Comparing `unyts-0.7.1/tests/test_units.py` & `unyts-0.8.0/tests/test_units.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # -*- coding: utf-8 -*-
 """
 Created on Fri Aug 26 21:34:21 2022
 
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
-from unyts import units, convert
+from unyts import units, convert, set_fvf
 from unyts.dictionaries import dictionary
 from unyts.units.unitless import Dimensionless, Percentage
 from unyts.operations import unit_product, unit_division
 import numpy as np
 
 num = 3
 array = np.array([1, 2, 3, 4, 5])
 limit_dict_units = 3
 
+set_fvf(1.10)  # set FVF for these tests
 
 for kind in [k for k in dictionary if k in ['Length']]:
     for unit1 in range(len(dictionary[kind][:limit_dict_units])-1):
         if len(dictionary[kind][unit1]) <= 2 and dictionary[kind][unit1].endswith('l'):
             continue
         print(dictionary[kind][unit1])
         u0 = units(2.78, dictionary[kind][unit1])
```

