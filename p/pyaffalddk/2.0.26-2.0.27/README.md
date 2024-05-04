# Comparing `tmp/pyaffalddk-2.0.26.tar.gz` & `tmp/pyaffalddk-2.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaffalddk-2.0.26.tar", last modified: Mon Apr 22 12:09:39 2024, max compression
+gzip compressed data, was "pyaffalddk-2.0.27.tar", last modified: Sat May  4 06:01:52 2024, max compression
```

## Comparing `pyaffalddk-2.0.26.tar` & `pyaffalddk-2.0.27.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:09:39.913727 pyaffalddk-2.0.26/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-22 12:09:29.000000 pyaffalddk-2.0.26/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-22 12:09:39.913727 pyaffalddk-2.0.26/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-22 12:09:29.000000 pyaffalddk-2.0.26/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:09:39.913727 pyaffalddk-2.0.26/pyaffalddk/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-22 12:09:29.000000 pyaffalddk-2.0.26/pyaffalddk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-04-22 12:09:29.000000 pyaffalddk-2.0.26/pyaffalddk/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-04-22 12:09:29.000000 pyaffalddk-2.0.26/pyaffalddk/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-22 12:09:29.000000 pyaffalddk-2.0.26/pyaffalddk/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-22 12:09:29.000000 pyaffalddk-2.0.26/pyaffalddk/images.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 12:09:39.913727 pyaffalddk-2.0.26/pyaffalddk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-22 12:09:39.000000 pyaffalddk-2.0.26/pyaffalddk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-22 12:09:39.000000 pyaffalddk-2.0.26/pyaffalddk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 12:09:39.000000 pyaffalddk-2.0.26/pyaffalddk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-22 12:09:39.000000 pyaffalddk-2.0.26/pyaffalddk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 12:09:39.913727 pyaffalddk-2.0.26/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-22 12:09:29.000000 pyaffalddk-2.0.26/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:01:52.708320 pyaffalddk-2.0.27/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-04 06:01:48.000000 pyaffalddk-2.0.27/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-04 06:01:52.708320 pyaffalddk-2.0.27/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-04 06:01:48.000000 pyaffalddk-2.0.27/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:01:52.708320 pyaffalddk-2.0.27/pyaffalddk/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-04 06:01:48.000000 pyaffalddk-2.0.27/pyaffalddk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-05-04 06:01:48.000000 pyaffalddk-2.0.27/pyaffalddk/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12418 2024-05-04 06:01:48.000000 pyaffalddk-2.0.27/pyaffalddk/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-04 06:01:48.000000 pyaffalddk-2.0.27/pyaffalddk/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-04 06:01:48.000000 pyaffalddk-2.0.27/pyaffalddk/images.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:01:52.708320 pyaffalddk-2.0.27/pyaffalddk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-04 06:01:52.000000 pyaffalddk-2.0.27/pyaffalddk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-04 06:01:52.000000 pyaffalddk-2.0.27/pyaffalddk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 06:01:52.000000 pyaffalddk-2.0.27/pyaffalddk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 06:01:52.000000 pyaffalddk-2.0.27/pyaffalddk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 06:01:52.712320 pyaffalddk-2.0.27/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-04 06:01:48.000000 pyaffalddk-2.0.27/setup.py
```

### Comparing `pyaffalddk-2.0.26/LICENSE` & `pyaffalddk-2.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaffalddk-2.0.26/PKG-INFO` & `pyaffalddk-2.0.27/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaffalddk
-Version: 2.0.26
+Version: 2.0.27
 Summary: Gets garbage collection data from danish Municipalities
 Home-page: https://github.com/briis/pyaffalddk
 Author: briis
 Author-email: bjarne@briis.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyaffalddk-2.0.26/pyaffalddk/__init__.py` & `pyaffalddk-2.0.27/pyaffalddk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,10 +11,10 @@
     AffaldDKNoConnection,
 )
 from pyaffalddk.data import PickupEvents, PickupType, AffaldDKAddressInfo
 
 from pyaffalddk.const import ICON_LIST, MUNICIPALITIES_ARRAY, NAME_ARRAY, NAME_LIST, WEEKDAYS, WEEKDAYS_SHORT
 
 __title__ = "pyaffalddk"
-__version__ = "2.0.26"
+__version__ = "2.0.27"
 __author__ = "briis"
 __license__ = "MIT"
```

### Comparing `pyaffalddk-2.0.26/pyaffalddk/api.py` & `pyaffalddk-2.0.27/pyaffalddk/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,15 @@
                         for group in [
                             "genbrug", "storskrald", "papir og glas/dåser","miljøkasse/tekstiler"
                         ]) and self._municipality.lower() == "gladsaxe":
                     key = get_garbage_type_from_material(row["materielnavn"], self._municipality, self._address_id)
                 elif  any(
                         group in row["ordningnavn"].lower()
                         for group in [
-                            "genbrug", "papir og glas/dåser","miljøkasse/tekstiler"
+                            "genbrug", "papir og glas/dåser","miljøkasse/tekstiler", "standpladser"
                         ]):
                     key = get_garbage_type_from_material(row["materielnavn"], self._municipality, self._address_id)
                 else:
                     key = get_garbage_type(row["ordningnavn"])
 
                 if key == row["ordningnavn"] and key != "Bestillerordning":
                     _LOGGER.warning(
```

### Comparing `pyaffalddk-2.0.26/pyaffalddk/const.py` & `pyaffalddk-2.0.27/pyaffalddk/const.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         "Rest / Mad",
         "Rest Mad",
         "Energispand - Obligatorisk min. 1 spand",
         "Rest/madaffald",
         "Energibeholder (mad/rest)",
         "Rest- og Madaffald",
     ],
+    "madaffald": [""],
     "batterier": ["Batterier"],
     "dagrenovation": ["Dagrenovation"],
     "elektronik": [""],
     "glas": ["Industri Genbrugeligt"],
     "metalglas": ["Glas og metal", "Metal-Glas", "Glas/Metal", "Metal og Glas"],
     "pappi": [
         "Plast MDK og papir",
@@ -94,14 +95,15 @@
         "Plast & Metal",
         "Plast, metal & MDK 660L",
         "Plast/ Metal",
         "Plast/MDK/Metal",
         "Plast-metal",
         "Plast/Metal",
     ],
+    "restaffald": ["",],
     "storskrald": [
         "Storskrald",
         "Stort elektronik",
         "Storskrald og genbrug",
         "Pap og Storskrald",
     ],
     "storskraldogtekstilaffald": [
@@ -109,14 +111,15 @@
     ],
     "haveaffald": [
         "Haveaffald, flishugning",
         "Haveaffald",
         "Trærødder og stammer",
         "Haveaffald - Frivilligt",
         "Haveaffald 140 L",
+        "Frivillig Haveaffald tømmes fra mandag til onsdag",
     ],
     "papirglas": ["Papir og pap/Glas", "Glas-papir", "Papir, Pap/Glas"],
     "plastmadkarton": [
         "Plast/MDK",
         "Plast & mad- og drikkekartoner",
         "Plast/ Mad- og drikkekartoner",
         "Plast og MDK",
@@ -155,19 +158,24 @@
 ]
 
 MATERIAL_LIST = {
     "restaffaldmadaffald": [""],
     "batterier": [
         "Batterier i pose på låg (1 stk.)",
     ],
-    "dagrenovation": [""],
+    "dagrenovation": [
+        "240 l. container 1 x ugentligt (12 stk.)",
+    ],
     "elektronik": [
         "Småt elektronik i pose på låg (1 stk.)",
     ],
-    "glas": [""],
+    "glas": [
+        "240 L glas (1 stk.)",
+        "Glas, 660 liter (2 stk.)",
+    ],
     "metalglas": [
         "Glas/metal (1 stk.)",
         "240 l Glas/metal Egenløsning (1 stk.)",
         "Metal/Glas 240 l - 2-kammer (1 stk.)",
         "Glas/metal, afstand over 5 meter (1 stk.)",
         "240 L - Metal og Glas (1 stk.)",
         "240 l glas/metal - 4 tømninger (1 stk.)",
@@ -188,44 +196,53 @@
     ],
     "farligtaffaldmiljoboks": [
         "Miljøkasse (1 stk.)",
         "Miljøboks",
         "Rød kasse henteordning (1 stk.)",
     ],
     "flis": [""],
-    "jern": [""],
+    "jern": [
+        "240 L metal (1 stk.)",
+        "Metal, 660 liter (1 stk.)",
+    ],
     "genbrug": [
         "Tekstiler",
         "Genbrug",
         "Genbrugsøer",
         "Genanvendeligt",
         "Genbrug 240 L",
         "Genbrugshal (1 stk.)",
     ],
-    "papir": [""],
+    "papir": [
+        "660 L papir (1 stk.)",
+        "Papir, 660 liter (3 stk.)",
+    ],
     "papirmetal": [
         "Metal og papir 240 L (ejer.kommune) (1 stk.)",
     ],
     "pap": [
         "Pap 240 L (villa) (1 stk.)",
         "240 l Pap Egenløsning (1 stk.)",
         "Pap 240 L (1 stk.)",
         "Pap 240 L (ejer:kommune) (h) (1 stk.)",
         "Pap - 240 l.  (1 stk.)",
         "Indsamling af pap (løst og beholder) (1 stk.)",
         "240 L - Pap - Skel (1 stk.)",
         "Beholder til pap (1 stk.)",
+        "770 L pap (1 stk.)",
+        "Pap, 660 liter (3 stk.)",
     ],
     "plastmetal": [
         "Plast, småt metal & MDK - 240 l. (1 stk.)",
     ],
     "plastmdkglasmetal": ["240 L todelt genbrugsspand hver 4. uge (1 stk.)",
     ],
     "plast": [
         "Plast og MDK 240 L (ejer.kommune) (1 stk.)",
+        "Plast, 660 liter (2 stk.)",
     ],
     "storskrald": [
         "Storskrald - fortovsindsamling (1 stk.)",
         "Storskrald (1 stk.)",
         "Storskrald enfamiliehus (1 stk.)",
         "Storskrald",
         "Stort elektronik",
@@ -240,14 +257,15 @@
     ],
     "papirglas": [
         "Papir/glas - 240 l. fortovsindsamling (1 stk.)",
     ],
     "plastmadkarton": [
         "Genbrugsbeholder PMDK/MG-240L/3uge (1 stk.)",
         "Genbrug henteordning (1 stk.)",
+        "660 L plast, mad- og drikkekartoner (1 stk.)",
     ],
     "papirglasdaaser": [
         "240 L 2-delt Papir/glas-dåser en-familie (1 stk.)",
     ],
     "pappapirglasmetal": [
         "240L metal, glas, plast/papir gl. (1 stk.)",
         "240 l genbrug 2-kammer (2023) (1 stk.)",
@@ -266,14 +284,16 @@
     "glasplast": [""],
     "plastmetalpapir": [""],
     "papirglasmetalplast": [
         "4-kammer (370 l) (1 stk.)",
         "Pap og papir/metal, glas og hård plast - 240 L (1 stk.)",
         "240 l genbrug låg i låg (1 stk.)"
     ],
+    "madaffald": ["140 L madaffald (1 stk.)",],
+    "restaffald": ["9505: 770 L restaffald uge (2 stk.)",],
 }
 
 ICON_LIST = {
     "batterier": "mdi:battery",
     "elektronik": "mdi:power-plug",
     "restaffaldmadaffald": "mdi:trash-can",
     "dagrenovation": "mdi:trash-can",
@@ -300,28 +320,31 @@
     "plastmdkglasmetal": "mdi:trash-can",
     "plastmetalmadmdk": "mdi:trash-can",
     "pappapir": "mdi:file",
     "tekstil": "mdi:recycle",
     "glasplast": "mdi:trash-can",
     "plastmetalpapir": "mdi:trash-can",
     "plast": "mdi:trash-can",
+    "madaffald": "mdi:trash-can",
+    "restaffald": "mdi:trash-can",
 }
 
 NAME_LIST = {
     "batterier": "Batterier",
     "elektronik": "Elektronik",
     "dagrenovation": "Dagrenovation",
     "farligtaffald": "Farligt affald",
     "farligtaffaldmiljoboks": "Farligt affald & Miljøboks",
     "flis": "Flis",
     "genbrug": "Genbrug",
     "glas": "Glas",
     "glasplast": "Glas, Plast & Madkartoner",
     "haveaffald": "Haveaffald",
-    "jern": "Jern",
+    "jern": "Metal",
+    "madaffald": "Madaffald",
     "metalglas": "Metal & Glas",
     "pap": "Pap",
     "papir": "Papir",
     "papirglas": "Papir, Pap & Glas",
     "papirglasdaaser": "Papir, Glas & Dåser",
     "papirglasmetalplast": "Papir, Glas, Metal & Plast",
     "papirmetal": "Papir & Metal",
@@ -330,14 +353,15 @@
     "pappi": "Papir & Plast",
     "plast": "Plast",
     "plastmadkarton": "Plast & Madkarton",
     "plastmdkglasmetal": "Plast, Madkarton, Glas & Metal",
     "plastmetal": "Plast & Metal",
     "plastmetalmadmdk": "Plast, Metal, Mad & Drikkekartoner",
     "plastmetalpapir": "Plast, Metal & Papir",
+    "restaffald": "Restaffald",
     "restaffaldmadaffald": "Rest & Madaffald",
     "storskrald": "Storskrald",
     "storskraldogtekstilaffald": "Storskrald & Tekstilaffald",
     "tekstil": "Tekstilaffald",
 }
 
 NAME_ARRAY = list(NAME_LIST.keys())
```

### Comparing `pyaffalddk-2.0.26/pyaffalddk/data.py` & `pyaffalddk-2.0.27/pyaffalddk/data.py`

 * *Files identical despite different names*

### Comparing `pyaffalddk-2.0.26/pyaffalddk/images.py` & `pyaffalddk-2.0.27/pyaffalddk/images.py`

 * *Files identical despite different names*

### Comparing `pyaffalddk-2.0.26/pyaffalddk.egg-info/PKG-INFO` & `pyaffalddk-2.0.27/pyaffalddk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaffalddk
-Version: 2.0.26
+Version: 2.0.27
 Summary: Gets garbage collection data from danish Municipalities
 Home-page: https://github.com/briis/pyaffalddk
 Author: briis
 Author-email: bjarne@briis.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyaffalddk-2.0.26/setup.py` & `pyaffalddk-2.0.27/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyaffalddk",
-    version="2.0.26",
+    version="2.0.27",
     author="briis",
     author_email="bjarne@briis.com",
     description="Gets garbage collection data from danish Municipalities",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/briis/pyaffalddk",
```

