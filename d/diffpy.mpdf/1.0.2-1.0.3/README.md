# Comparing `tmp/diffpy.mpdf-1.0.2.tar.gz` & `tmp/diffpy_mpdf-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffpy.mpdf-1.0.2.tar", last modified: Fri Apr  5 21:50:35 2024, max compression
+gzip compressed data, was "diffpy_mpdf-1.0.3.tar", last modified: Fri May  3 22:22:51 2024, max compression
```

## Comparing `diffpy.mpdf-1.0.2.tar` & `diffpy_mpdf-1.0.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 21:50:35.777231 diffpy.mpdf-1.0.2/
--rw-rw-rw-   0        0        0      125 2022-06-07 23:05:44.000000 diffpy.mpdf-1.0.2/AUTHORS.txt
--rw-rw-rw-   0        0        0     1467 2022-06-07 23:05:44.000000 diffpy.mpdf-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      120 2021-06-28 23:33:25.000000 diffpy.mpdf-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6673 2024-04-05 21:50:35.561863 diffpy.mpdf-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4156 2024-04-05 21:45:28.000000 diffpy.mpdf-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 21:50:24.530565 diffpy.mpdf-1.0.2/diffpy/
--rw-rw-rw-   0        0        0      584 2022-06-07 23:05:44.000000 diffpy.mpdf-1.0.2/diffpy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 21:50:30.560575 diffpy.mpdf-1.0.2/diffpy/mpdf/
--rw-rw-rw-   0        0        0     1003 2022-08-13 03:54:16.000000 diffpy.mpdf-1.0.2/diffpy/mpdf/__init__.py
--rw-rw-rw-   0        0        0       99 2021-06-28 23:33:25.000000 diffpy.mpdf-1.0.2/diffpy/mpdf/gitarchive.cfg
--rw-rw-rw-   0        0        0    47885 2024-02-17 07:33:42.000000 diffpy.mpdf-1.0.2/diffpy/mpdf/magstructure.py
--rw-rw-rw-   0        0        0    78098 2024-04-05 04:57:49.000000 diffpy.mpdf-1.0.2/diffpy/mpdf/magutils.py
--rw-rw-rw-   0        0        0    30689 2024-04-05 04:57:49.000000 diffpy.mpdf-1.0.2/diffpy/mpdf/mciftools.py
--rw-rw-rw-   0        0        0     6536 2022-06-07 23:05:45.000000 diffpy.mpdf-1.0.2/diffpy/mpdf/mpdf3Dcalculator.py
--rw-rw-rw-   0        0        0    17740 2024-02-18 01:35:21.000000 diffpy.mpdf-1.0.2/diffpy/mpdf/mpdfcalculator.py
--rw-rw-rw-   0        0        0    23512 2023-11-24 06:03:18.000000 diffpy.mpdf-1.0.2/diffpy/mpdf/mpdftransformer.py
--rw-rw-rw-   0        0        0     3919 2022-05-28 05:28:31.000000 diffpy.mpdf-1.0.2/diffpy/mpdf/simpleparser.py
-drwxrwxrwx   0        0        0        0 2024-04-05 21:50:33.758931 diffpy.mpdf-1.0.2/diffpy/mpdf/tests/
--rw-rw-rw-   0        0        0     5608 2021-06-28 23:33:25.000000 diffpy.mpdf-1.0.2/diffpy/mpdf/tests/MnO_cubic.cif
--rw-rw-rw-   0        0        0     1708 2021-06-28 23:33:25.000000 diffpy.mpdf-1.0.2/diffpy/mpdf/tests/__init__.py
--rw-rw-rw-   0        0        0      869 2021-06-28 23:33:25.000000 diffpy.mpdf-1.0.2/diffpy/mpdf/tests/run.py
--rw-rw-rw-   0        0        0      648 2021-06-28 23:33:25.000000 diffpy.mpdf-1.0.2/diffpy/mpdf/tests/testbasicmpdf.py
-drwxrwxrwx   0        0        0        0 2024-04-05 21:50:34.360631 diffpy.mpdf-1.0.2/diffpy/mpdf/tests/testdata/
--rw-rw-rw-   0        0        0     5608 2021-06-28 23:33:26.000000 diffpy.mpdf-1.0.2/diffpy/mpdf/tests/testdata/MnO_cubic.cif
--rw-rw-rw-   0        0        0    71748 2021-06-28 23:33:26.000000 diffpy.mpdf-1.0.2/diffpy/mpdf/tests/testdata/testdata.fgr
--rw-rw-rw-   0        0        0    71748 2021-06-28 23:33:26.000000 diffpy.mpdf-1.0.2/diffpy/mpdf/tests/testdata.fgr
--rw-rw-rw-   0        0        0      544 2021-06-28 23:33:26.000000 diffpy.mpdf-1.0.2/diffpy/mpdf/tests/testformfactor.py
--rw-rw-rw-   0        0        0      709 2021-06-28 23:33:26.000000 diffpy.mpdf-1.0.2/diffpy/mpdf/tests/testgetdiffdata.py
--rw-rw-rw-   0        0        0     1240 2021-06-28 23:33:26.000000 diffpy.mpdf-1.0.2/diffpy/mpdf/tests/testmpdffromcif.py
--rw-rw-rw-   0        0        0      947 2021-06-28 23:33:26.000000 diffpy.mpdf-1.0.2/diffpy/mpdf/tests/testmpdffromselfcreated.py
--rw-rw-rw-   0        0        0     1071 2021-06-28 23:33:26.000000 diffpy.mpdf-1.0.2/diffpy/mpdf/tests/testspinsatoms.py
--rw-rw-rw-   0        0        0      128 2021-06-28 23:33:26.000000 diffpy.mpdf-1.0.2/diffpy/mpdf/version.cfg
--rw-rw-rw-   0        0        0     1216 2022-06-07 23:05:45.000000 diffpy.mpdf-1.0.2/diffpy/mpdf/version.py
--rw-rw-rw-   0        0        0     7011 2022-06-07 23:05:45.000000 diffpy.mpdf-1.0.2/diffpy/mpdf/visualize3D.py
-drwxrwxrwx   0        0        0        0 2024-04-05 21:50:35.218114 diffpy.mpdf-1.0.2/diffpy.mpdf.egg-info/
--rw-rw-rw-   0        0        0     6673 2024-04-05 21:50:20.000000 diffpy.mpdf-1.0.2/diffpy.mpdf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      976 2024-04-05 21:50:21.000000 diffpy.mpdf-1.0.2/diffpy.mpdf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 21:50:20.000000 diffpy.mpdf-1.0.2/diffpy.mpdf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-05 21:50:21.000000 diffpy.mpdf-1.0.2/diffpy.mpdf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      940 2024-04-05 21:42:02.000000 diffpy.mpdf-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 21:50:35.855408 diffpy.mpdf-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     4654 2024-04-05 21:42:23.000000 diffpy.mpdf-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 22:22:51.369852 diffpy_mpdf-1.0.3/
+-rw-rw-rw-   0        0        0      125 2022-06-07 23:05:44.000000 diffpy_mpdf-1.0.3/AUTHORS.txt
+-rw-rw-rw-   0        0        0     1467 2022-06-07 23:05:44.000000 diffpy_mpdf-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      120 2021-06-28 23:33:25.000000 diffpy_mpdf-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     6673 2024-05-03 22:22:51.247849 diffpy_mpdf-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4156 2024-04-05 21:45:28.000000 diffpy_mpdf-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 22:22:44.299281 diffpy_mpdf-1.0.3/diffpy/
+-rw-rw-rw-   0        0        0      584 2022-06-07 23:05:44.000000 diffpy_mpdf-1.0.3/diffpy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 22:22:48.293226 diffpy_mpdf-1.0.3/diffpy/mpdf/
+-rw-rw-rw-   0        0        0     1003 2022-08-13 03:54:16.000000 diffpy_mpdf-1.0.3/diffpy/mpdf/__init__.py
+-rw-rw-rw-   0        0        0       99 2021-06-28 23:33:25.000000 diffpy_mpdf-1.0.3/diffpy/mpdf/gitarchive.cfg
+-rw-rw-rw-   0        0        0    47885 2024-02-17 07:33:42.000000 diffpy_mpdf-1.0.3/diffpy/mpdf/magstructure.py
+-rw-rw-rw-   0        0        0    78098 2024-04-05 04:57:49.000000 diffpy_mpdf-1.0.3/diffpy/mpdf/magutils.py
+-rw-rw-rw-   0        0        0    30689 2024-04-05 04:57:49.000000 diffpy_mpdf-1.0.3/diffpy/mpdf/mciftools.py
+-rw-rw-rw-   0        0        0     6536 2022-06-07 23:05:45.000000 diffpy_mpdf-1.0.3/diffpy/mpdf/mpdf3Dcalculator.py
+-rw-rw-rw-   0        0        0    17740 2024-02-18 01:35:21.000000 diffpy_mpdf-1.0.3/diffpy/mpdf/mpdfcalculator.py
+-rw-rw-rw-   0        0        0    23512 2023-11-24 06:03:18.000000 diffpy_mpdf-1.0.3/diffpy/mpdf/mpdftransformer.py
+-rw-rw-rw-   0        0        0     3919 2022-05-28 05:28:31.000000 diffpy_mpdf-1.0.3/diffpy/mpdf/simpleparser.py
+drwxrwxrwx   0        0        0        0 2024-05-03 22:22:50.141280 diffpy_mpdf-1.0.3/diffpy/mpdf/tests/
+-rw-rw-rw-   0        0        0     5608 2021-06-28 23:33:25.000000 diffpy_mpdf-1.0.3/diffpy/mpdf/tests/MnO_cubic.cif
+-rw-rw-rw-   0        0        0     1708 2021-06-28 23:33:25.000000 diffpy_mpdf-1.0.3/diffpy/mpdf/tests/__init__.py
+-rw-rw-rw-   0        0        0      869 2021-06-28 23:33:25.000000 diffpy_mpdf-1.0.3/diffpy/mpdf/tests/run.py
+-rw-rw-rw-   0        0        0      648 2021-06-28 23:33:25.000000 diffpy_mpdf-1.0.3/diffpy/mpdf/tests/testbasicmpdf.py
+drwxrwxrwx   0        0        0        0 2024-05-03 22:22:50.498292 diffpy_mpdf-1.0.3/diffpy/mpdf/tests/testdata/
+-rw-rw-rw-   0        0        0     5608 2021-06-28 23:33:26.000000 diffpy_mpdf-1.0.3/diffpy/mpdf/tests/testdata/MnO_cubic.cif
+-rw-rw-rw-   0        0        0    71748 2021-06-28 23:33:26.000000 diffpy_mpdf-1.0.3/diffpy/mpdf/tests/testdata/testdata.fgr
+-rw-rw-rw-   0        0        0    71748 2021-06-28 23:33:26.000000 diffpy_mpdf-1.0.3/diffpy/mpdf/tests/testdata.fgr
+-rw-rw-rw-   0        0        0      544 2021-06-28 23:33:26.000000 diffpy_mpdf-1.0.3/diffpy/mpdf/tests/testformfactor.py
+-rw-rw-rw-   0        0        0      709 2021-06-28 23:33:26.000000 diffpy_mpdf-1.0.3/diffpy/mpdf/tests/testgetdiffdata.py
+-rw-rw-rw-   0        0        0     1240 2021-06-28 23:33:26.000000 diffpy_mpdf-1.0.3/diffpy/mpdf/tests/testmpdffromcif.py
+-rw-rw-rw-   0        0        0      947 2021-06-28 23:33:26.000000 diffpy_mpdf-1.0.3/diffpy/mpdf/tests/testmpdffromselfcreated.py
+-rw-rw-rw-   0        0        0     1071 2021-06-28 23:33:26.000000 diffpy_mpdf-1.0.3/diffpy/mpdf/tests/testspinsatoms.py
+-rw-rw-rw-   0        0        0      128 2021-06-28 23:33:26.000000 diffpy_mpdf-1.0.3/diffpy/mpdf/version.cfg
+-rw-rw-rw-   0        0        0     1216 2022-06-07 23:05:45.000000 diffpy_mpdf-1.0.3/diffpy/mpdf/version.py
+-rw-rw-rw-   0        0        0     7700 2024-05-03 22:07:37.000000 diffpy_mpdf-1.0.3/diffpy/mpdf/visualize3D.py
+drwxrwxrwx   0        0        0        0 2024-05-03 22:22:51.010841 diffpy_mpdf-1.0.3/diffpy.mpdf.egg-info/
+-rw-rw-rw-   0        0        0     6673 2024-05-03 22:22:43.000000 diffpy_mpdf-1.0.3/diffpy.mpdf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      976 2024-05-03 22:22:44.000000 diffpy_mpdf-1.0.3/diffpy.mpdf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 22:22:43.000000 diffpy_mpdf-1.0.3/diffpy.mpdf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-03 22:22:43.000000 diffpy_mpdf-1.0.3/diffpy.mpdf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      940 2024-05-03 22:19:44.000000 diffpy_mpdf-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-03 22:22:51.430854 diffpy_mpdf-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     4654 2024-05-03 22:20:03.000000 diffpy_mpdf-1.0.3/setup.py
```

### Comparing `diffpy.mpdf-1.0.2/LICENSE.txt` & `diffpy_mpdf-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `diffpy.mpdf-1.0.2/PKG-INFO` & `diffpy_mpdf-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffpy.mpdf
-Version: 1.0.2
+Version: 1.0.3
 Summary: Tools for magnetic PDF analysis.
 Author-email: Benjamin Frandsen <benfrandsen@byu.edu>
 License: Copyright 2022 BENJAMIN ALLEN FRANDSEN
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
```

### Comparing `diffpy.mpdf-1.0.2/README.md` & `diffpy_mpdf-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `diffpy.mpdf-1.0.2/diffpy/__init__.py` & `diffpy_mpdf-1.0.3/diffpy/__init__.py`

 * *Files identical despite different names*

### Comparing `diffpy.mpdf-1.0.2/diffpy/mpdf/__init__.py` & `diffpy_mpdf-1.0.3/diffpy/mpdf/__init__.py`

 * *Files identical despite different names*

### Comparing `diffpy.mpdf-1.0.2/diffpy/mpdf/magstructure.py` & `diffpy_mpdf-1.0.3/diffpy/mpdf/magstructure.py`

 * *Files identical despite different names*

### Comparing `diffpy.mpdf-1.0.2/diffpy/mpdf/magutils.py` & `diffpy_mpdf-1.0.3/diffpy/mpdf/magutils.py`

 * *Files identical despite different names*

### Comparing `diffpy.mpdf-1.0.2/diffpy/mpdf/mciftools.py` & `diffpy_mpdf-1.0.3/diffpy/mpdf/mciftools.py`

 * *Files identical despite different names*

### Comparing `diffpy.mpdf-1.0.2/diffpy/mpdf/mpdf3Dcalculator.py` & `diffpy_mpdf-1.0.3/diffpy/mpdf/mpdf3Dcalculator.py`

 * *Files identical despite different names*

### Comparing `diffpy.mpdf-1.0.2/diffpy/mpdf/mpdfcalculator.py` & `diffpy_mpdf-1.0.3/diffpy/mpdf/mpdfcalculator.py`

 * *Files identical despite different names*

### Comparing `diffpy.mpdf-1.0.2/diffpy/mpdf/mpdftransformer.py` & `diffpy_mpdf-1.0.3/diffpy/mpdf/mpdftransformer.py`

 * *Files identical despite different names*

### Comparing `diffpy.mpdf-1.0.2/diffpy/mpdf/simpleparser.py` & `diffpy_mpdf-1.0.3/diffpy/mpdf/simpleparser.py`

 * *Files identical despite different names*

### Comparing `diffpy.mpdf-1.0.2/diffpy/mpdf/tests/MnO_cubic.cif` & `diffpy_mpdf-1.0.3/diffpy/mpdf/tests/MnO_cubic.cif`

 * *Files identical despite different names*

### Comparing `diffpy.mpdf-1.0.2/diffpy/mpdf/tests/__init__.py` & `diffpy_mpdf-1.0.3/diffpy/mpdf/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `diffpy.mpdf-1.0.2/diffpy/mpdf/tests/run.py` & `diffpy_mpdf-1.0.3/diffpy/mpdf/tests/run.py`

 * *Files identical despite different names*

### Comparing `diffpy.mpdf-1.0.2/diffpy/mpdf/tests/testbasicmpdf.py` & `diffpy_mpdf-1.0.3/diffpy/mpdf/tests/testbasicmpdf.py`

 * *Files identical despite different names*

### Comparing `diffpy.mpdf-1.0.2/diffpy/mpdf/tests/testdata/MnO_cubic.cif` & `diffpy_mpdf-1.0.3/diffpy/mpdf/tests/testdata/MnO_cubic.cif`

 * *Files identical despite different names*

### Comparing `diffpy.mpdf-1.0.2/diffpy/mpdf/tests/testdata/testdata.fgr` & `diffpy_mpdf-1.0.3/diffpy/mpdf/tests/testdata/testdata.fgr`

 * *Files identical despite different names*

### Comparing `diffpy.mpdf-1.0.2/diffpy/mpdf/tests/testdata.fgr` & `diffpy_mpdf-1.0.3/diffpy/mpdf/tests/testdata.fgr`

 * *Files identical despite different names*

### Comparing `diffpy.mpdf-1.0.2/diffpy/mpdf/tests/testformfactor.py` & `diffpy_mpdf-1.0.3/diffpy/mpdf/tests/testformfactor.py`

 * *Files identical despite different names*

### Comparing `diffpy.mpdf-1.0.2/diffpy/mpdf/tests/testgetdiffdata.py` & `diffpy_mpdf-1.0.3/diffpy/mpdf/tests/testgetdiffdata.py`

 * *Files identical despite different names*

### Comparing `diffpy.mpdf-1.0.2/diffpy/mpdf/tests/testmpdffromcif.py` & `diffpy_mpdf-1.0.3/diffpy/mpdf/tests/testmpdffromcif.py`

 * *Files identical despite different names*

### Comparing `diffpy.mpdf-1.0.2/diffpy/mpdf/tests/testmpdffromselfcreated.py` & `diffpy_mpdf-1.0.3/diffpy/mpdf/tests/testmpdffromselfcreated.py`

 * *Files identical despite different names*

### Comparing `diffpy.mpdf-1.0.2/diffpy/mpdf/tests/testspinsatoms.py` & `diffpy_mpdf-1.0.3/diffpy/mpdf/tests/testspinsatoms.py`

 * *Files identical despite different names*

### Comparing `diffpy.mpdf-1.0.2/diffpy/mpdf/version.py` & `diffpy_mpdf-1.0.3/diffpy/mpdf/version.py`

 * *Files identical despite different names*

### Comparing `diffpy.mpdf-1.0.2/diffpy/mpdf/visualize3D.py` & `diffpy_mpdf-1.0.3/diffpy/mpdf/visualize3D.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,33 +25,48 @@
     
     Args:
         m (numpy array): signal array (3D)
         x (numpy array): x-dimension coordinates (1D)
         y (numpy array): y-dimension coordinates (1D)
         z (numpy array): z-dimension coordinates (1D)
     """
-    def __init__(self, m=None, x=None, y=None, z=None, sliceAvailable=False):
+    def __init__(self, m=None, x=None, y=None, z=None):
             
         self.m = m
         self.x = x
         self.y = y
         self.z = z
-        self.a = None # these two instance attributes will construct an arbitrary grid
-        self.b = None
-        self.slice = None # this will become the data slice
+        self.dataslice = None # this will become the data slice
         if m is None:
             self.m = np.array([])
         if x is None:
             self.x = np.array([])
         if y is None:
             self.y = np.array([])
         if z is None:
             self.z = np.array([])
-        self.sliceAvailable = sliceAvailable
-        
+        self._sliceAvailable = False
+        self._a = None # these two instance attributes will construct an arbitrary grid
+        self._b = None
+    
+    @property
+    def sliceAvailable(self):
+        """whether or not a data slice has been made"""
+        return self._sliceAvailable
+
+    @property
+    def a(self):
+        """internally used grid coordinate"""
+        return self._a
+        
+    @property
+    def b(self):
+        """internally used grid coordinate"""
+        return self._b
+
     def three_points(self, p1, p2, p3):
         """find normal vector to the plane created by the three given points
         """
         
         # find two vectors from the three points which lie on the desired plane
         vec1 = p2 - p1
         vec2 = p3 - p1
@@ -124,50 +139,58 @@
         # now reflect v1 using m_norm
         v1 = m_norm.dot(v1)
         # and create a new vector v2 that is orthogonal to both v1 and normal
         v2 = np.cross(normal, v1)
         # we now have 2 vectors to form our plane
     
         # now create and normalize Q, which will rotate an arbitrary 
-            # slice to the orientation we desire
+        # slice to the orientation we desire
         Q = np.column_stack((v1, v2, np.zeros_like(v1)))
         Q[:,:2] /= np.linalg.norm(Q[:,:2], axis = 0)
     
         # now create an arbitrary slice
-        self.a = np.arange(-len_a / 2, len_a / 2, dr)
-        self.b = np.arange(-len_b / 2, len_b / 2, dr)
-        self.a = np.append(self.a, len_a / 2)
-        self.b = np.append(self.b, len_b / 2)
-        A,B = np.meshgrid(self.a, self.b)
+        self._a = np.arange(-len_a / 2, len_a / 2, dr)
+        self._b = np.arange(-len_b / 2, len_b / 2, dr)
+        self._a = np.append(self._a, len_a / 2)
+        self._b = np.append(self._b, len_b / 2)
+        A,B = np.meshgrid(self._a, self._b)
         locations = np.array([A.reshape(-1), B.reshape(-1), np.zeros(A.size)])  # the slice starts on the x-y plane
         # now move locations onto our two vectors, and add cen_pt to move slice into position
         locations = Q.dot(locations).T + (cen_pt)
     
         # now we need to interpolate our 3Dmpdf function over this slice
         points = (self.x, self.y, self.z)
         interp = interpn(points, self.m, locations)  # list of values of 3Dmpdf at locations
-        self.slice = interp.reshape(len(self.b),len(self.a))
+        self.dataslice = interp.reshape(len(self._b),len(self._a))
         
-        self.sliceAvailable = True
+        self._sliceAvailable = True
         
         if returnSlice:
-            return self.slice, self.a, self.b
+            return self.dataslice, self._a, self._b
         
-    def visualize(self):
+    def visualize(self, cmap='bwr'):
         """Visualize the current slice.
+        
+        Args:
+            cmap (str): Name of matplotlib colormap to be used for visualization.
+                See https://matplotlib.org/stable/users/explain/colors/colormaps.html
+                for complete list. Default is 'bwr', which works well for
+                3D-PDF data.
+
         """
         if self.sliceAvailable:
             fig = plt.figure()
             ax = fig.add_subplot(111)
             ax.set_xlabel(r'$\mathdefault{\AA}$')
             ax.set_ylabel(r'$\mathdefault{\AA}$')
-            amin, amax = min(self.a), max(self.a)
-            bmin, bmax = min(self.b), max(self.b)
-            im = ax.imshow(self.slice,
-                           extent=[amin, amax, bmin, bmax])
+            amin, amax = min(self._a), max(self._a)
+            bmin, bmax = min(self._b), max(self._b)
+            im = ax.imshow(self.dataslice,
+                           extent=[amin, amax, bmin, bmax],
+                           cmap=cmap)
             colorbar(im)
             plt.tight_layout()
             plt.show()
             
         else:
             print('No data slice available for visualization.')
             print('Please generate a slice using the makeSlice method.')
```

### Comparing `diffpy.mpdf-1.0.2/diffpy.mpdf.egg-info/PKG-INFO` & `diffpy_mpdf-1.0.3/diffpy.mpdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffpy.mpdf
-Version: 1.0.2
+Version: 1.0.3
 Summary: Tools for magnetic PDF analysis.
 Author-email: Benjamin Frandsen <benfrandsen@byu.edu>
 License: Copyright 2022 BENJAMIN ALLEN FRANDSEN
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
```

### Comparing `diffpy.mpdf-1.0.2/diffpy.mpdf.egg-info/SOURCES.txt` & `diffpy_mpdf-1.0.3/diffpy.mpdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diffpy.mpdf-1.0.2/pyproject.toml` & `diffpy_mpdf-1.0.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "diffpy.mpdf"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Benjamin Frandsen", email="benfrandsen@byu.edu" },
 ]
 readme = "README.md"
 requires-python = ">=3.7"
 description = "Tools for magnetic PDF analysis."
 license = {file = "LICENSE.txt"}
```

### Comparing `diffpy.mpdf-1.0.2/setup.py` & `diffpy_mpdf-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
 #versiondata = getversioncfg()  ### python3 incompatible
 
 # define distribution
 setup_args = dict(
         name = "diffpy.mpdf",
         #version = versiondata.get('DEFAULT', 'version'),
-        version = '1.0.2',
+        version = '1.0.3',
         #namespace_packages = ['diffpy'],
         packages = find_packages(),
         #test_suite = 'diffpy.mpdf.tests',
         #include_package_data = True,
         #zip_safe = False,
         #author = 'Benjamin A. Frandsen group',
         #author_email = 'benfrandsen@byu.edu',
```

