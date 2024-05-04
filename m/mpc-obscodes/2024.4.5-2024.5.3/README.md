# Comparing `tmp/mpc_obscodes-2024.4.5.tar.gz` & `tmp/mpc_obscodes-2024.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpc_obscodes-2024.4.5.tar", last modified: Fri Apr  5 02:22:26 2024, max compression
+gzip compressed data, was "mpc_obscodes-2024.5.3.tar", last modified: Fri May  3 02:24:06 2024, max compression
```

## Comparing `mpc_obscodes-2024.4.5.tar` & `mpc_obscodes-2024.5.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:22:26.244371 mpc_obscodes-2024.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-05 02:22:17.000000 mpc_obscodes-2024.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-05 02:22:26.244371 mpc_obscodes-2024.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-05 02:22:17.000000 mpc_obscodes-2024.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:22:26.240371 mpc_obscodes-2024.4.5/mpc_obscodes/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-05 02:22:17.000000 mpc_obscodes-2024.4.5/mpc_obscodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-05 02:22:17.000000 mpc_obscodes-2024.4.5/mpc_obscodes/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-04-05 02:22:17.000000 mpc_obscodes-2024.4.5/mpc_obscodes/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)   253345 2024-04-05 02:22:20.000000 mpc_obscodes-2024.4.5/mpc_obscodes/obscodes_extended.json
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-05 02:22:20.000000 mpc_obscodes-2024.4.5/mpc_obscodes/obscodes_extended.md5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:22:26.244371 mpc_obscodes-2024.4.5/mpc_obscodes/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 02:22:17.000000 mpc_obscodes-2024.4.5/mpc_obscodes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-05 02:22:17.000000 mpc_obscodes-2024.4.5/mpc_obscodes/tests/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-05 02:22:17.000000 mpc_obscodes-2024.4.5/mpc_obscodes/tests/test_fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-05 02:22:17.000000 mpc_obscodes-2024.4.5/mpc_obscodes/tests/test_mpc_obscodes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 02:22:26.244371 mpc_obscodes-2024.4.5/mpc_obscodes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-05 02:22:26.000000 mpc_obscodes-2024.4.5/mpc_obscodes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-05 02:22:26.000000 mpc_obscodes-2024.4.5/mpc_obscodes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 02:22:26.000000 mpc_obscodes-2024.4.5/mpc_obscodes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-05 02:22:26.000000 mpc_obscodes-2024.4.5/mpc_obscodes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 02:22:26.000000 mpc_obscodes-2024.4.5/mpc_obscodes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-05 02:22:20.000000 mpc_obscodes-2024.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 02:22:26.244371 mpc_obscodes-2024.4.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:24:06.184181 mpc_obscodes-2024.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-03 02:23:55.000000 mpc_obscodes-2024.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-03 02:24:06.184181 mpc_obscodes-2024.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-03 02:23:55.000000 mpc_obscodes-2024.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:24:06.180181 mpc_obscodes-2024.5.3/mpc_obscodes/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-03 02:23:55.000000 mpc_obscodes-2024.5.3/mpc_obscodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-03 02:23:55.000000 mpc_obscodes-2024.5.3/mpc_obscodes/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-03 02:23:55.000000 mpc_obscodes-2024.5.3/mpc_obscodes/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)   254258 2024-05-03 02:24:00.000000 mpc_obscodes-2024.5.3/mpc_obscodes/obscodes_extended.json
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-03 02:24:00.000000 mpc_obscodes-2024.5.3/mpc_obscodes/obscodes_extended.md5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:24:06.180181 mpc_obscodes-2024.5.3/mpc_obscodes/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 02:23:55.000000 mpc_obscodes-2024.5.3/mpc_obscodes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-03 02:23:55.000000 mpc_obscodes-2024.5.3/mpc_obscodes/tests/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-03 02:23:55.000000 mpc_obscodes-2024.5.3/mpc_obscodes/tests/test_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-03 02:23:55.000000 mpc_obscodes-2024.5.3/mpc_obscodes/tests/test_mpc_obscodes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:24:06.180181 mpc_obscodes-2024.5.3/mpc_obscodes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-03 02:24:06.000000 mpc_obscodes-2024.5.3/mpc_obscodes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-03 02:24:06.000000 mpc_obscodes-2024.5.3/mpc_obscodes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 02:24:06.000000 mpc_obscodes-2024.5.3/mpc_obscodes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 02:24:06.000000 mpc_obscodes-2024.5.3/mpc_obscodes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 02:24:06.000000 mpc_obscodes-2024.5.3/mpc_obscodes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-03 02:24:00.000000 mpc_obscodes-2024.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 02:24:06.184181 mpc_obscodes-2024.5.3/setup.cfg
```

### Comparing `mpc_obscodes-2024.4.5/PKG-INFO` & `mpc_obscodes-2024.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpc_obscodes
-Version: 2024.4.5
+Version: 2024.5.3
 Summary: Minor Planet Center Observatory Codes
 Author-email: B612 Asteroid Institute <info@b612foundation.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
```

### Comparing `mpc_obscodes-2024.4.5/README.md` & `mpc_obscodes-2024.5.3/README.md`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2024.4.5/mpc_obscodes/compare.py` & `mpc_obscodes-2024.5.3/mpc_obscodes/compare.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2024.4.5/mpc_obscodes/fetch.py` & `mpc_obscodes-2024.5.3/mpc_obscodes/fetch.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2024.4.5/mpc_obscodes/obscodes_extended.json` & `mpc_obscodes-2024.5.3/mpc_obscodes/obscodes_extended.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9955001988862371%*

 * *Differences: {"'033'": "{'cos': 0.630904, 'sin': 0.773338}",*

 * * "'073'": "{'cos': 0.715515, 'sin': 0.696285}",*

 * * "'461'": "{'Longitude': 19.89367, 'cos': 0.671543, 'sin': 0.738689}",*

 * * "'561'": "{'Longitude': 19.89367, 'cos': 0.671543, 'sin': 0.738689}",*

 * * "'693'": "{'cos': 0.845313, 'sin': 0.533209}",*

 * * "'C58'": "OrderedDict([('Name', 'NEO Surveyor')])",*

 * * "'D47'": "OrderedDict([('Longitude', 11.56366), ('cos', 0.738665), ('sin', 0.671859), ('Name', "*

 * *          "'BigBang Observatory, Manciano')])",*

 * * "'D60'": "OrderedDict([('L […]*

```diff
@@ -196,16 +196,16 @@
         "Name": "Jena",
         "cos": 0.631624,
         "sin": 0.772706
     },
     "033": {
         "Longitude": 11.71124,
         "Name": "Karl Schwarzschild Observatory, Tautenburg",
-        "cos": 0.6309,
-        "sin": 0.773333
+        "cos": 0.630904,
+        "sin": 0.773338
     },
     "034": {
         "Longitude": 12.45246,
         "Name": "Monte Mario Observatory, Rome",
         "cos": 0.745176,
         "sin": 0.664656
     },
@@ -436,16 +436,16 @@
         "Name": "Scheuren Observatory",
         "cos": 0.629,
         "sin": 0.774
     },
     "073": {
         "Longitude": 26.09391,
         "Name": "Bucharest",
-        "cos": 0.715519,
-        "sin": 0.696289
+        "cos": 0.715515,
+        "sin": 0.696285
     },
     "074": {
         "Longitude": 26.4058,
         "Name": "Boyden Observatory, Bloemfontein",
         "cos": 0.87518,
         "sin": -0.48263
     },
@@ -2585,18 +2585,18 @@
     "460": {
         "Longitude": 265.9981,
         "Name": "Area 52 Observatory, Nashville",
         "cos": 0.8301,
         "sin": 0.55579
     },
     "461": {
-        "Longitude": 19.8943,
+        "Longitude": 19.89367,
         "Name": "University of Szeged, Piszkesteto Stn. (Konkoly)",
-        "cos": 0.67153,
-        "sin": 0.73869
+        "cos": 0.671543,
+        "sin": 0.738689
     },
     "462": {
         "Longitude": 283.0842,
         "Name": "Mount Belleview Observatory",
         "cos": 0.77905,
         "sin": 0.62488
     },
@@ -3185,18 +3185,18 @@
     "560": {
         "Longitude": 10.931,
         "Name": "Madonna di Dossobuono",
         "cos": 0.703262,
         "sin": 0.708561
     },
     "561": {
-        "Longitude": 19.8943,
+        "Longitude": 19.89367,
         "Name": "Piszkesteto Stn. (Konkoly)",
-        "cos": 0.67153,
-        "sin": 0.73869
+        "cos": 0.671543,
+        "sin": 0.738689
     },
     "562": {
         "Longitude": 15.9236,
         "Name": "Figl Observatory, Vienna",
         "cos": 0.66938,
         "sin": 0.74062
     },
@@ -3979,16 +3979,16 @@
         "Name": "Steward Observatory, Tucson",
         "cos": 0.84679,
         "sin": 0.53036
     },
     "693": {
         "Longitude": 249.26745,
         "Name": "Catalina Station, Tucson",
-        "cos": 0.845317,
-        "sin": 0.533211
+        "cos": 0.845313,
+        "sin": 0.533209
     },
     "694": {
         "Longitude": 248.9943,
         "Name": "Tumamoc Hill, Tucson",
         "cos": 0.847,
         "sin": 0.53009
     },
@@ -7339,14 +7339,17 @@
     },
     "C56": {
         "Name": "LISA-Pathfinder"
     },
     "C57": {
         "Name": "TESS"
     },
+    "C58": {
+        "Name": "NEO Surveyor"
+    },
     "C59": {
         "Name": "Yangwang-1"
     },
     "C60": {
         "Longitude": 7.06926,
         "Name": "Argelander Institute for Astronomy Obs., Bonn",
         "cos": 0.634261,
@@ -7864,14 +7867,20 @@
     },
     "D46": {
         "Longitude": 9.90265,
         "Name": "Observatory Bad Wurzach",
         "cos": 0.671664,
         "sin": 0.738525
     },
+    "D47": {
+        "Longitude": 11.56366,
+        "Name": "BigBang Observatory, Manciano",
+        "cos": 0.738665,
+        "sin": 0.671859
+    },
     "D53": {
         "Longitude": 127.482,
         "Name": "ISON-Blagoveschensk Observatory",
         "cos": 0.63981,
         "sin": 0.766
     },
     "D54": {
@@ -7894,14 +7903,20 @@
     },
     "D58": {
         "Longitude": 129.025,
         "Name": "KSA SEM Observatory, Danggam-dong",
         "cos": 0.818419,
         "sin": 0.572736
     },
+    "D60": {
+        "Longitude": 13.54989,
+        "Name": "Masseris, Savogna",
+        "cos": 0.693656,
+        "sin": 0.718065
+    },
     "D61": {
         "Longitude": 134.9131,
         "Name": "Suntopia Marina, Sumoto",
         "cos": 0.82671,
         "sin": 0.56075
     },
     "D62": {
@@ -7912,14 +7927,20 @@
     },
     "D63": {
         "Longitude": 10.46138,
         "Name": "G. Pascoli Observatory, Barga (since June 2023)",
         "cos": 0.719553,
         "sin": 0.692176
     },
+    "D64": {
+        "Longitude": 14.10967,
+        "Name": "Fucama, Casalincontrada",
+        "cos": 0.740711,
+        "sin": 0.669613
+    },
     "D67": {
         "Longitude": 37.62472,
         "Name": "Tula Rooftop Observatory, Tula",
         "cos": 0.586136,
         "sin": 0.80753
     },
     "D70": {
@@ -8503,34 +8524,34 @@
         "Name": "Wickede",
         "cos": 0.623411,
         "sin": 0.779293
     },
     "G34": {
         "Longitude": 13.7015,
         "Name": "Oberfrauendorf",
-        "cos": 0.63254,
-        "sin": 0.77203
+        "cos": 0.632547,
+        "sin": 0.772037
     },
     "G35": {
         "Longitude": 249.15789,
         "Name": "Elephant Head Obsevatory, Sahuarita",
         "cos": 0.849476,
         "sin": 0.526134
     },
     "G36": {
         "Longitude": 357.4525,
         "Name": "Calar Alto-CASADO",
         "cos": 0.797538,
         "sin": 0.601812
     },
     "G37": {
-        "Longitude": 248.57749,
+        "Longitude": 248.57779,
         "Name": "Lowell Discovery Telescope",
-        "cos": 0.822887,
-        "sin": 0.566916
+        "cos": 0.8229,
+        "sin": 0.566927
     },
     "G38": {
         "Longitude": 356.76842,
         "Name": "Observatorio La Senda, Cabanillas del Campo",
         "cos": 0.759967,
         "sin": 0.647951
     },
@@ -8875,16 +8896,16 @@
         "Name": "Hereford Arizona Observatory, Hereford",
         "cos": 0.85404,
         "sin": 0.51888
     },
     "G96": {
         "Longitude": 249.21128,
         "Name": "Mt. Lemmon Survey",
-        "cos": 0.845111,
-        "sin": 0.533614
+        "cos": 0.845107,
+        "sin": 0.533611
     },
     "G97": {
         "Longitude": 250.8694,
         "Name": "Astronomical League Alpha Observatory, Portal",
         "cos": 0.84965,
         "sin": 0.526
     },
@@ -9745,16 +9766,16 @@
         "Name": "La Silla--TRAPPIST",
         "cos": 0.873472,
         "sin": -0.485986
     },
     "I41": {
         "Longitude": 243.14022,
         "Name": "Palomar Mountain--ZTF",
-        "cos": 0.836325,
-        "sin": 0.546877
+        "cos": 0.836322,
+        "sin": 0.546875
     },
     "I42": {
         "Longitude": 288.9081,
         "Name": "Westport Observatory",
         "cos": 0.74895,
         "sin": 0.66041
     },
@@ -9811,16 +9832,16 @@
         "Name": "Clinton",
         "cos": 0.78133,
         "sin": 0.62203
     },
     "I52": {
         "Longitude": 249.21108,
         "Name": "Steward Observatory, Mt. Lemmon Station",
-        "cos": 0.845113,
-        "sin": 0.533611
+        "cos": 0.845109,
+        "sin": 0.533609
     },
     "I53": {
         "Longitude": 356.3783,
         "Name": "Armilla",
         "cos": 0.79822,
         "sin": 0.60052
     },
@@ -11003,18 +11024,18 @@
     "K50": {
         "Longitude": 11.133,
         "Name": "Sternwarte Feuerstein, Ebermannstadt",
         "cos": 0.646903,
         "sin": 0.760116
     },
     "K51": {
-        "Longitude": 11.6579,
+        "Longitude": 11.65789,
         "Name": "Osservatorio del Celado, Castello Tesino",
-        "cos": 0.69563,
-        "sin": 0.71626
+        "cos": 0.695636,
+        "sin": 0.716268
     },
     "K52": {
         "Longitude": 7.6478,
         "Name": "Gwen Observatory, San Francesco al Campo",
         "cos": 0.70548,
         "sin": 0.70642
     },
@@ -11225,18 +11246,18 @@
     "K87": {
         "Longitude": 10.17011,
         "Name": "Dettelbach Vineyard Observatory",
         "cos": 0.646647,
         "sin": 0.760288
     },
     "K88": {
-        "Longitude": 19.8936,
+        "Longitude": 19.89367,
         "Name": "GINOP-KHK, Piszkesteto",
-        "cos": 0.67154,
-        "sin": 0.73869
+        "cos": 0.671543,
+        "sin": 0.738689
     },
     "K89": {
         "Longitude": 11.56339,
         "Name": "Digital Stargate Observatory, Manciano",
         "cos": 0.738665,
         "sin": 0.67186
     },
@@ -12110,15 +12131,15 @@
         "cos": 0.696956,
         "sin": 0.714892
     },
     "M38": {
         "Longitude": 21.76719,
         "Name": "Harsona Observatory, Nyiregyhaza",
         "cos": 0.671089,
-        "sin": 0.738923
+        "sin": 0.738924
     },
     "M39": {
         "Longitude": 22.95888,
         "Name": "AUTH Observatory, Thessaloniki",
         "cos": 0.760013,
         "sin": 0.64775
     },
@@ -12268,14 +12289,20 @@
     },
     "M64": {
         "Longitude": 0.23964,
         "Name": "Holbrook, Heathfield",
         "cos": 0.631065,
         "sin": 0.77317
     },
+    "M65": {
+        "Longitude": 28.32494,
+        "Name": "Mustola Observatory, Lappeenranta",
+        "cos": 0.485072,
+        "sin": 0.871558
+    },
     "M90": {
         "Longitude": 65.4286,
         "Name": "Chervishevo",
         "cos": 0.54672,
         "sin": 0.83452
     },
     "N27": {
@@ -12919,15 +12946,15 @@
         "Name": "Haleakala-LCO OGG B #2",
         "cos": 0.936241,
         "sin": 0.351538
     },
     "T05": {
         "Longitude": 203.74299,
         "Name": "ATLAS-HKO, Haleakala",
-        "cos": 0.936235,
+        "cos": 0.936236,
         "sin": 0.351547
     },
     "T07": {
         "Longitude": 204.42387,
         "Name": "ATLAS-MLO Auxiliary Camera, Mauna Loa",
         "cos": 0.94329,
         "sin": 0.332467
@@ -13219,16 +13246,16 @@
         "Name": "Rusty Mountain Observatory, Gold Canyon",
         "cos": 0.836631,
         "sin": 0.546101
     },
     "V06": {
         "Longitude": 249.26745,
         "Name": "Catalina Sky Survey-Kuiper",
-        "cos": 0.845317,
-        "sin": 0.533211
+        "cos": 0.845313,
+        "sin": 0.533209
     },
     "V07": {
         "Longitude": 249.1219,
         "Name": "Whipple Observatory, Mount Hopkins-PAIRITEL",
         "cos": 0.85208,
         "sin": 0.52234
     },
@@ -14122,14 +14149,20 @@
     },
     "X17": {
         "Longitude": 289.26208,
         "Name": "BlackGEM",
         "cos": 0.873456,
         "sin": -0.486033
     },
+    "X18": {
+        "Longitude": 291.82053,
+        "Name": "6R-POL2, San Pedro de Atacama",
+        "cos": 0.921646,
+        "sin": -0.38771
+    },
     "X31": {
         "Longitude": 299.47934,
         "Name": "Galileo Galilei Observatory, Oro Verde",
         "cos": 0.850485,
         "sin": -0.524263
     },
     "X33": {
@@ -14278,14 +14311,32 @@
     },
     "Y66": {
         "Longitude": 343.49053,
         "Name": "Two-Meter Twin Telescope, TTT2, Teide",
         "cos": 0.881484,
         "sin": 0.471429
     },
+    "Y82": {
+        "Longitude": 358.06548,
+        "Name": "LPMR Observatory, Broad Chalke",
+        "cos": 0.630258,
+        "sin": 0.77381
+    },
+    "Y83": {
+        "Longitude": 359.04761,
+        "Name": "Observatorio Arcosur, Zaragoza",
+        "cos": 0.748699,
+        "sin": 0.660768
+    },
+    "Y84": {
+        "Longitude": 358.11972,
+        "Name": "Observatoire de Saint Domineuc",
+        "cos": 0.665503,
+        "sin": 0.743909
+    },
     "Y85": {
         "Longitude": 351.85389,
         "Name": "Magalofes Observatory, Fene",
         "cos": 0.727084,
         "sin": 0.684321
     },
     "Y86": {
@@ -14497,16 +14548,16 @@
         "Name": "La Palma-MERCATOR",
         "cos": 0.87763,
         "sin": 0.4785
     },
     "Z21": {
         "Longitude": 343.4883,
         "Name": "Tenerife-LCO Aqawan A #1",
-        "cos": 0.881468,
-        "sin": 0.471452
+        "cos": 0.881475,
+        "sin": 0.471455
     },
     "Z22": {
         "Longitude": 343.4894,
         "Name": "MASTER-IAC Observatory, Tenerife",
         "cos": 0.88148,
         "sin": 0.47143
     },
@@ -14557,16 +14608,16 @@
         "Name": "Glyn Marsh Observatory, Douglas",
         "cos": 0.586571,
         "sin": 0.807215
     },
     "Z31": {
         "Longitude": 343.48835,
         "Name": "Tenerife Observatory-LCO A, Tenerife",
-        "cos": 0.881476,
-        "sin": 0.471458
+        "cos": 0.881474,
+        "sin": 0.471457
     },
     "Z32": {
         "Longitude": 358.98372,
         "Name": "Observatorio Astrofisico de Javalambre",
         "cos": 0.766879,
         "sin": 0.64013
     },
```

### Comparing `mpc_obscodes-2024.4.5/mpc_obscodes/tests/test_compare.py` & `mpc_obscodes-2024.5.3/mpc_obscodes/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2024.4.5/mpc_obscodes/tests/test_fetch.py` & `mpc_obscodes-2024.5.3/mpc_obscodes/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2024.4.5/mpc_obscodes/tests/test_mpc_obscodes.py` & `mpc_obscodes-2024.5.3/mpc_obscodes/tests/test_mpc_obscodes.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2024.4.5/mpc_obscodes.egg-info/PKG-INFO` & `mpc_obscodes-2024.5.3/mpc_obscodes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpc_obscodes
-Version: 2024.4.5
+Version: 2024.5.3
 Summary: Minor Planet Center Observatory Codes
 Author-email: B612 Asteroid Institute <info@b612foundation.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
```

### Comparing `mpc_obscodes-2024.4.5/pyproject.toml` & `mpc_obscodes-2024.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires =  ["setuptools>=45", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mpc_obscodes"
-version = "2024.04.05"
+version = "2024.05.03"
 authors = [
     {name = "B612 Asteroid Institute", email = "info@b612foundation.org"},
 ]
 description = "Minor Planet Center Observatory Codes"
 readme = "README.md"
 requires-python = ">=3.7"
```

