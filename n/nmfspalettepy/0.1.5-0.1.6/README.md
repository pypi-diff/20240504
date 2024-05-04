# Comparing `tmp/nmfspalettepy-0.1.5.tar.gz` & `tmp/nmfspalettepy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmfspalettepy-0.1.5.tar", last modified: Fri May  3 23:07:41 2024, max compression
+gzip compressed data, was "nmfspalettepy-0.1.6.tar", last modified: Fri May  3 23:12:29 2024, max compression
```

## Comparing `nmfspalettepy-0.1.5.tar` & `nmfspalettepy-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 23:07:41.421859 nmfspalettepy-0.1.5/
--rw-rw-rw-   0        0        0      523 2023-12-06 21:45:16.000000 nmfspalettepy-0.1.5/LICENSE.md
--rw-rw-rw-   0        0        0     3902 2024-05-03 23:07:41.421859 nmfspalettepy-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     3652 2024-05-03 23:06:55.000000 nmfspalettepy-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 23:07:41.406327 nmfspalettepy-0.1.5/nmfspalettepy/
--rw-rw-rw-   0        0        0      141 2024-05-01 19:42:52.000000 nmfspalettepy-0.1.5/nmfspalettepy/__init__.py
--rw-rw-rw-   0        0        0     1924 2024-05-01 19:34:30.000000 nmfspalettepy-0.1.5/nmfspalettepy/palettes.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:07:41.421859 nmfspalettepy-0.1.5/nmfspalettepy.egg-info/
--rw-rw-rw-   0        0        0     3902 2024-05-03 23:07:40.000000 nmfspalettepy-0.1.5/nmfspalettepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-05-03 23:07:40.000000 nmfspalettepy-0.1.5/nmfspalettepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 23:07:40.000000 nmfspalettepy-0.1.5/nmfspalettepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-03 23:07:40.000000 nmfspalettepy-0.1.5/nmfspalettepy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-03 23:07:40.000000 nmfspalettepy-0.1.5/nmfspalettepy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 23:07:41.421859 nmfspalettepy-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      538 2024-05-03 23:06:26.000000 nmfspalettepy-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:12:29.294912 nmfspalettepy-0.1.6/
+-rw-rw-rw-   0        0        0      523 2023-12-06 21:45:16.000000 nmfspalettepy-0.1.6/LICENSE.md
+-rw-rw-rw-   0        0        0     3866 2024-05-03 23:12:29.294912 nmfspalettepy-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3616 2024-05-03 23:12:10.000000 nmfspalettepy-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 23:12:29.263663 nmfspalettepy-0.1.6/nmfspalettepy/
+-rw-rw-rw-   0        0        0      141 2024-05-01 19:42:52.000000 nmfspalettepy-0.1.6/nmfspalettepy/__init__.py
+-rw-rw-rw-   0        0        0     1924 2024-05-01 19:34:30.000000 nmfspalettepy-0.1.6/nmfspalettepy/palettes.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:12:29.279289 nmfspalettepy-0.1.6/nmfspalettepy.egg-info/
+-rw-rw-rw-   0        0        0     3866 2024-05-03 23:12:29.000000 nmfspalettepy-0.1.6/nmfspalettepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-05-03 23:12:29.000000 nmfspalettepy-0.1.6/nmfspalettepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 23:12:29.000000 nmfspalettepy-0.1.6/nmfspalettepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-03 23:12:29.000000 nmfspalettepy-0.1.6/nmfspalettepy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-03 23:12:29.000000 nmfspalettepy-0.1.6/nmfspalettepy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 23:12:29.294912 nmfspalettepy-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      538 2024-05-03 23:12:21.000000 nmfspalettepy-0.1.6/setup.py
```

### Comparing `nmfspalettepy-0.1.5/LICENSE.md` & `nmfspalettepy-0.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nmfspalettepy-0.1.5/PKG-INFO` & `nmfspalettepy-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: nmfspalettepy
-Version: 0.1.5
+Version: 0.1.6
 Summary: NMFS color palettes handling library
 Author: Michael Akridge
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 
 # nmfspalettepy
 
 <a href="https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/tree/nmfspalettepy">
-    <img src="https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/blob/7cff3005063c4bc7d55ab60857a106ec13d5abd5/docs/nmfspalettepy_250.png" align="right" alt="logo"/>
+    <img src="https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/raw/main/logos/nmfspalettepy_250.png" align="right" alt="logo"/>
 </a>
 
 `nmfspalettepy` is a Python library designed to facilitate the use of National Marine Fisheries Service (NMFS) color palettes for data visualization. It provides easy access to a series of NMFS color schemes.
 
 ## Source:
 - view on Github: https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/tree/nmfspalettepy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nmfspalettepy Version: 0.1.5 Summary: NMFS color
+Metadata-Version: 2.1 Name: nmfspalettepy Version: 0.1.6 Summary: NMFS color
 palettes handling library Author: Michael Akridge Description-Content-Type:
 text/markdown License-File: LICENSE.md Requires-Dist: numpy Requires-Dist:
 matplotlib # nmfspalettepy _[_l_o_g_o_]`nmfspalettepy` is a Python library designed
 to facilitate the use of National Marine Fisheries Service (NMFS) color
 palettes for data visualization. It provides easy access to a series of NMFS
 color schemes. ## Source: - view on Github: https://github.com/MichaelAkridge-
 NOAA/NOAA-NMFS-Brand-Resources/tree/nmfspalettepy ## Features - Provides a set
```

### Comparing `nmfspalettepy-0.1.5/README.md` & `nmfspalettepy-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # nmfspalettepy
 
 <a href="https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/tree/nmfspalettepy">
-    <img src="https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/blob/7cff3005063c4bc7d55ab60857a106ec13d5abd5/docs/nmfspalettepy_250.png" align="right" alt="logo"/>
+    <img src="https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/raw/main/logos/nmfspalettepy_250.png" align="right" alt="logo"/>
 </a>
 
 `nmfspalettepy` is a Python library designed to facilitate the use of National Marine Fisheries Service (NMFS) color palettes for data visualization. It provides easy access to a series of NMFS color schemes.
 
 ## Source:
 - view on Github: https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/tree/nmfspalettepy
```

### Comparing `nmfspalettepy-0.1.5/nmfspalettepy/palettes.py` & `nmfspalettepy-0.1.6/nmfspalettepy/palettes.py`

 * *Files identical despite different names*

### Comparing `nmfspalettepy-0.1.5/nmfspalettepy.egg-info/PKG-INFO` & `nmfspalettepy-0.1.6/nmfspalettepy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: nmfspalettepy
-Version: 0.1.5
+Version: 0.1.6
 Summary: NMFS color palettes handling library
 Author: Michael Akridge
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 
 # nmfspalettepy
 
 <a href="https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/tree/nmfspalettepy">
-    <img src="https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/blob/7cff3005063c4bc7d55ab60857a106ec13d5abd5/docs/nmfspalettepy_250.png" align="right" alt="logo"/>
+    <img src="https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/raw/main/logos/nmfspalettepy_250.png" align="right" alt="logo"/>
 </a>
 
 `nmfspalettepy` is a Python library designed to facilitate the use of National Marine Fisheries Service (NMFS) color palettes for data visualization. It provides easy access to a series of NMFS color schemes.
 
 ## Source:
 - view on Github: https://github.com/MichaelAkridge-NOAA/NOAA-NMFS-Brand-Resources/tree/nmfspalettepy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nmfspalettepy Version: 0.1.5 Summary: NMFS color
+Metadata-Version: 2.1 Name: nmfspalettepy Version: 0.1.6 Summary: NMFS color
 palettes handling library Author: Michael Akridge Description-Content-Type:
 text/markdown License-File: LICENSE.md Requires-Dist: numpy Requires-Dist:
 matplotlib # nmfspalettepy _[_l_o_g_o_]`nmfspalettepy` is a Python library designed
 to facilitate the use of National Marine Fisheries Service (NMFS) color
 palettes for data visualization. It provides easy access to a series of NMFS
 color schemes. ## Source: - view on Github: https://github.com/MichaelAkridge-
 NOAA/NOAA-NMFS-Brand-Resources/tree/nmfspalettepy ## Features - Provides a set
```

### Comparing `nmfspalettepy-0.1.5/setup.py` & `nmfspalettepy-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='nmfspalettepy',
-    version='0.1.5',
+    version='0.1.6',
     description='NMFS color palettes handling library',
     long_description=long_description,
     long_description_content_type='text/markdown',  # This is important
     packages=['nmfspalettepy'],
     install_requires=[
         'numpy',
         'matplotlib'
```

