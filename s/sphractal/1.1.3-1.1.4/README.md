# Comparing `tmp/sphractal-1.1.3.tar.gz` & `tmp/sphractal-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphractal-1.1.3.tar", max compression
+gzip compressed data, was "sphractal-1.1.4.tar", max compression
```

## Comparing `sphractal-1.1.3.tar` & `sphractal-1.1.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1082 2024-04-12 05:29:19.560581 sphractal-1.1.3/LICENSE
--rw-r--r--   0        0        0     5258 2024-04-12 05:29:19.560581 sphractal-1.1.3/README.md
--rw-r--r--   0        0        0     2056 2024-04-12 05:29:51.756526 sphractal-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      743 2024-04-12 05:29:51.756526 sphractal-1.1.3/setup.py
--rw-r--r--   0        0        0     1684 2024-04-12 05:29:19.580581 sphractal-1.1.3/src/sphractal/__init__.py
--rw-r--r--   0        0        0    14972 2024-04-12 05:29:19.580581 sphractal-1.1.3/src/sphractal/boxCnt.py
--rw-r--r--   0        0        0     4534 2024-04-12 05:29:19.580581 sphractal-1.1.3/src/sphractal/constants.py
--rw-r--r--   0        0        0      429 2024-04-12 05:29:19.580581 sphractal-1.1.3/src/sphractal/data/__init__.py
--rw-r--r--   0        0        0    96018 2024-04-12 05:29:19.580581 sphractal-1.1.3/src/sphractal/data/caseStudyOTS1T000.xyz
--rw-r--r--   0        0        0    96018 2024-04-12 05:29:19.580581 sphractal-1.1.3/src/sphractal/data/caseStudyOTS1T323.xyz
--rw-r--r--   0        0        0    96018 2024-04-12 05:29:19.580581 sphractal-1.1.3/src/sphractal/data/caseStudyOTS1T523.xyz
--rw-r--r--   0        0        0   123297 2024-04-12 05:29:19.580581 sphractal-1.1.3/src/sphractal/data/caseStudyOTS2T000.xyz
--rw-r--r--   0        0        0   123297 2024-04-12 05:29:19.580581 sphractal-1.1.3/src/sphractal/data/caseStudyOTS2T323.xyz
--rw-r--r--   0        0        0   123297 2024-04-12 05:29:19.584581 sphractal-1.1.3/src/sphractal/data/caseStudyOTS2T523.xyz
--rw-r--r--   0        0        0    96018 2024-04-12 05:29:19.584581 sphractal-1.1.3/src/sphractal/data/caseStudyRDS1T000.xyz
--rw-r--r--   0        0        0    96018 2024-04-12 05:29:19.584581 sphractal-1.1.3/src/sphractal/data/caseStudyRDS1T323.xyz
--rw-r--r--   0        0        0    96018 2024-04-12 05:29:19.584581 sphractal-1.1.3/src/sphractal/data/caseStudyRDS1T523.xyz
--rw-r--r--   0        0        0   123297 2024-04-12 05:29:19.584581 sphractal-1.1.3/src/sphractal/data/caseStudyRDS2T000.xyz
--rw-r--r--   0        0        0   123297 2024-04-12 05:29:19.584581 sphractal-1.1.3/src/sphractal/data/caseStudyRDS2T323.xyz
--rw-r--r--   0        0        0   123297 2024-04-12 05:29:19.584581 sphractal-1.1.3/src/sphractal/data/caseStudyRDS2T523.xyz
--rw-r--r--   0        0        0    61052 2024-04-12 05:29:19.584581 sphractal-1.1.3/src/sphractal/data/caseStudyTHS1T000.xyz
--rw-r--r--   0        0        0    61052 2024-04-12 05:29:19.584581 sphractal-1.1.3/src/sphractal/data/caseStudyTHS1T323.xyz
--rw-r--r--   0        0        0    61052 2024-04-12 05:29:19.584581 sphractal-1.1.3/src/sphractal/data/caseStudyTHS1T523.xyz
--rw-r--r--   0        0        0    83796 2024-04-12 05:29:19.584581 sphractal-1.1.3/src/sphractal/data/caseStudyTHS2T000.xyz
--rw-r--r--   0        0        0    83796 2024-04-12 05:29:19.584581 sphractal-1.1.3/src/sphractal/data/caseStudyTHS2T323.xyz
--rw-r--r--   0        0        0    83796 2024-04-12 05:29:19.584581 sphractal-1.1.3/src/sphractal/data/caseStudyTHS2T523.xyz
--rw-r--r--   0        0        0    44360 2024-04-12 05:29:19.584581 sphractal-1.1.3/src/sphractal/data/dna.xyz
--rw-r--r--   0        0        0    42215 2024-04-12 05:29:19.584581 sphractal-1.1.3/src/sphractal/data/exampleOT.xyz
--rw-r--r--   0        0        0    17795 2024-04-12 05:29:19.584581 sphractal-1.1.3/src/sphractal/data/graphene.xyz
--rw-r--r--   0        0        0     1152 2024-04-12 05:29:19.584581 sphractal-1.1.3/src/sphractal/data/paracetamol.xyz
--rw-r--r--   0        0        0       60 2024-04-12 05:29:19.584581 sphractal-1.1.3/src/sphractal/data/singleAtom.xyz
--rw-r--r--   0        0        0  2128669 2024-04-12 05:29:19.592581 sphractal-1.1.3/src/sphractal/data/strongScalingSP.xyz
--rw-r--r--   0        0        0     2584 2024-04-12 05:29:19.592581 sphractal-1.1.3/src/sphractal/data/weakScalingSP00.xyz
--rw-r--r--   0        0        0     5224 2024-04-12 05:29:19.592581 sphractal-1.1.3/src/sphractal/data/weakScalingSP01.xyz
--rw-r--r--   0        0        0    10625 2024-04-12 05:29:19.592581 sphractal-1.1.3/src/sphractal/data/weakScalingSP02.xyz
--rw-r--r--   0        0        0    19265 2024-04-12 05:29:19.592581 sphractal-1.1.3/src/sphractal/data/weakScalingSP03.xyz
--rw-r--r--   0        0        0    40922 2024-04-12 05:29:19.592581 sphractal-1.1.3/src/sphractal/data/weakScalingSP04.xyz
--rw-r--r--   0        0        0    63099 2024-04-12 05:29:19.592581 sphractal-1.1.3/src/sphractal/data/weakScalingSP05.xyz
--rw-r--r--   0        0        0   116940 2024-04-12 05:29:19.596581 sphractal-1.1.3/src/sphractal/data/weakScalingSP06.xyz
--rw-r--r--   0        0        0   249165 2024-04-12 05:29:19.600581 sphractal-1.1.3/src/sphractal/data/weakScalingSP07.xyz
--rw-r--r--   0        0        0   476181 2024-04-12 05:29:19.600581 sphractal-1.1.3/src/sphractal/data/weakScalingSP08.xyz
--rw-r--r--   0        0        0   965188 2024-04-12 05:29:19.600581 sphractal-1.1.3/src/sphractal/data/weakScalingSP09.xyz
--rw-r--r--   0        0        0  2010709 2024-04-12 05:29:19.604581 sphractal-1.1.3/src/sphractal/data/weakScalingSP10.xyz
--rw-r--r--   0        0        0  3987214 2024-04-12 05:29:19.612581 sphractal-1.1.3/src/sphractal/data/weakScalingSP11.xyz
--rw-r--r--   0        0        0     2507 2024-04-12 05:29:19.612581 sphractal-1.1.3/src/sphractal/datasets.py
--rw-r--r--   0        0        0    14295 2024-04-12 05:29:19.612581 sphractal-1.1.3/src/sphractal/surfExact.py
--rw-r--r--   0        0        0    14641 2024-04-12 05:29:19.616581 sphractal-1.1.3/src/sphractal/surfVoxel.py
--rw-r--r--   0        0        0    12336 2024-04-12 05:29:19.616581 sphractal-1.1.3/src/sphractal/utils.py
--rw-r--r--   0        0        0    93084 2024-04-12 05:29:19.616581 sphractal-1.1.3/tests/fixtures.py
--rw-r--r--   0        0        0    19919 2024-04-12 05:29:19.616581 sphractal-1.1.3/tests/test_sphractal.py
--rw-r--r--   0        0        0     6578 1970-01-01 00:00:00.000000 sphractal-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-05-03 22:37:34.370242 sphractal-1.1.4/LICENSE
+-rw-r--r--   0        0        0     5258 2024-05-03 22:37:34.370242 sphractal-1.1.4/README.md
+-rw-r--r--   0        0        0     2056 2024-05-03 22:38:06.994202 sphractal-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0      743 2024-05-03 22:38:06.994202 sphractal-1.1.4/setup.py
+-rw-r--r--   0        0        0     1684 2024-05-03 22:37:34.390242 sphractal-1.1.4/src/sphractal/__init__.py
+-rw-r--r--   0        0        0    14972 2024-05-03 22:37:34.390242 sphractal-1.1.4/src/sphractal/boxCnt.py
+-rw-r--r--   0        0        0     4534 2024-05-03 22:37:34.390242 sphractal-1.1.4/src/sphractal/constants.py
+-rw-r--r--   0        0        0      429 2024-05-03 22:37:34.390242 sphractal-1.1.4/src/sphractal/data/__init__.py
+-rw-r--r--   0        0        0    96018 2024-05-03 22:37:34.390242 sphractal-1.1.4/src/sphractal/data/caseStudyOTS1T000.xyz
+-rw-r--r--   0        0        0    96018 2024-05-03 22:37:34.390242 sphractal-1.1.4/src/sphractal/data/caseStudyOTS1T323.xyz
+-rw-r--r--   0        0        0    96018 2024-05-03 22:37:34.390242 sphractal-1.1.4/src/sphractal/data/caseStudyOTS1T523.xyz
+-rw-r--r--   0        0        0   123297 2024-05-03 22:37:34.390242 sphractal-1.1.4/src/sphractal/data/caseStudyOTS2T000.xyz
+-rw-r--r--   0        0        0   123297 2024-05-03 22:37:34.390242 sphractal-1.1.4/src/sphractal/data/caseStudyOTS2T323.xyz
+-rw-r--r--   0        0        0   123297 2024-05-03 22:37:34.394242 sphractal-1.1.4/src/sphractal/data/caseStudyOTS2T523.xyz
+-rw-r--r--   0        0        0    96018 2024-05-03 22:37:34.394242 sphractal-1.1.4/src/sphractal/data/caseStudyRDS1T000.xyz
+-rw-r--r--   0        0        0    96018 2024-05-03 22:37:34.394242 sphractal-1.1.4/src/sphractal/data/caseStudyRDS1T323.xyz
+-rw-r--r--   0        0        0    96018 2024-05-03 22:37:34.394242 sphractal-1.1.4/src/sphractal/data/caseStudyRDS1T523.xyz
+-rw-r--r--   0        0        0   123297 2024-05-03 22:37:34.394242 sphractal-1.1.4/src/sphractal/data/caseStudyRDS2T000.xyz
+-rw-r--r--   0        0        0   123297 2024-05-03 22:37:34.394242 sphractal-1.1.4/src/sphractal/data/caseStudyRDS2T323.xyz
+-rw-r--r--   0        0        0   123297 2024-05-03 22:37:34.394242 sphractal-1.1.4/src/sphractal/data/caseStudyRDS2T523.xyz
+-rw-r--r--   0        0        0    61052 2024-05-03 22:37:34.394242 sphractal-1.1.4/src/sphractal/data/caseStudyTHS1T000.xyz
+-rw-r--r--   0        0        0    61052 2024-05-03 22:37:34.394242 sphractal-1.1.4/src/sphractal/data/caseStudyTHS1T323.xyz
+-rw-r--r--   0        0        0    61052 2024-05-03 22:37:34.394242 sphractal-1.1.4/src/sphractal/data/caseStudyTHS1T523.xyz
+-rw-r--r--   0        0        0    83796 2024-05-03 22:37:34.394242 sphractal-1.1.4/src/sphractal/data/caseStudyTHS2T000.xyz
+-rw-r--r--   0        0        0    83796 2024-05-03 22:37:34.394242 sphractal-1.1.4/src/sphractal/data/caseStudyTHS2T323.xyz
+-rw-r--r--   0        0        0    83796 2024-05-03 22:37:34.394242 sphractal-1.1.4/src/sphractal/data/caseStudyTHS2T523.xyz
+-rw-r--r--   0        0        0    44360 2024-05-03 22:37:34.394242 sphractal-1.1.4/src/sphractal/data/dna.xyz
+-rw-r--r--   0        0        0    42215 2024-05-03 22:37:34.394242 sphractal-1.1.4/src/sphractal/data/exampleOT.xyz
+-rw-r--r--   0        0        0    17795 2024-05-03 22:37:34.394242 sphractal-1.1.4/src/sphractal/data/graphene.xyz
+-rw-r--r--   0        0        0     1152 2024-05-03 22:37:34.394242 sphractal-1.1.4/src/sphractal/data/paracetamol.xyz
+-rw-r--r--   0        0        0       60 2024-05-03 22:37:34.394242 sphractal-1.1.4/src/sphractal/data/singleAtom.xyz
+-rw-r--r--   0        0        0  2128669 2024-05-03 22:37:34.402242 sphractal-1.1.4/src/sphractal/data/strongScalingSP.xyz
+-rw-r--r--   0        0        0     2584 2024-05-03 22:37:34.402242 sphractal-1.1.4/src/sphractal/data/weakScalingSP00.xyz
+-rw-r--r--   0        0        0     5224 2024-05-03 22:37:34.402242 sphractal-1.1.4/src/sphractal/data/weakScalingSP01.xyz
+-rw-r--r--   0        0        0    10625 2024-05-03 22:37:34.402242 sphractal-1.1.4/src/sphractal/data/weakScalingSP02.xyz
+-rw-r--r--   0        0        0    19265 2024-05-03 22:37:34.402242 sphractal-1.1.4/src/sphractal/data/weakScalingSP03.xyz
+-rw-r--r--   0        0        0    40922 2024-05-03 22:37:34.402242 sphractal-1.1.4/src/sphractal/data/weakScalingSP04.xyz
+-rw-r--r--   0        0        0    63099 2024-05-03 22:37:34.402242 sphractal-1.1.4/src/sphractal/data/weakScalingSP05.xyz
+-rw-r--r--   0        0        0   116940 2024-05-03 22:37:34.406242 sphractal-1.1.4/src/sphractal/data/weakScalingSP06.xyz
+-rw-r--r--   0        0        0   249165 2024-05-03 22:37:34.410242 sphractal-1.1.4/src/sphractal/data/weakScalingSP07.xyz
+-rw-r--r--   0        0        0   476181 2024-05-03 22:37:34.410242 sphractal-1.1.4/src/sphractal/data/weakScalingSP08.xyz
+-rw-r--r--   0        0        0   965188 2024-05-03 22:37:34.410242 sphractal-1.1.4/src/sphractal/data/weakScalingSP09.xyz
+-rw-r--r--   0        0        0  2010709 2024-05-03 22:37:34.414242 sphractal-1.1.4/src/sphractal/data/weakScalingSP10.xyz
+-rw-r--r--   0        0        0  3987214 2024-05-03 22:37:34.422242 sphractal-1.1.4/src/sphractal/data/weakScalingSP11.xyz
+-rw-r--r--   0        0        0     2507 2024-05-03 22:37:34.422242 sphractal-1.1.4/src/sphractal/datasets.py
+-rw-r--r--   0        0        0    14295 2024-05-03 22:37:34.426242 sphractal-1.1.4/src/sphractal/surfExact.py
+-rw-r--r--   0        0        0    14641 2024-05-03 22:37:34.426242 sphractal-1.1.4/src/sphractal/surfVoxel.py
+-rw-r--r--   0        0        0    12336 2024-05-03 22:37:34.426242 sphractal-1.1.4/src/sphractal/utils.py
+-rw-r--r--   0        0        0    93084 2024-05-03 22:37:34.426242 sphractal-1.1.4/tests/fixtures.py
+-rw-r--r--   0        0        0    19919 2024-05-03 22:37:34.426242 sphractal-1.1.4/tests/test_sphractal.py
+-rw-r--r--   0        0        0     6578 1970-01-01 00:00:00.000000 sphractal-1.1.4/PKG-INFO
```

### Comparing `sphractal-1.1.3/LICENSE` & `sphractal-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/README.md` & `sphractal-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/pyproject.toml` & `sphractal-1.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphractal"
-version = "1.1.3"
+version = "1.1.4"
 description = "Package to estimate fractal dimension of 3D surfaces formed from overlapping spheres via box-counting algorithm."
 authors = ["Jonathan Yik Chang Ting <jonting97@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Jon-Ting/sphractal"
 repository = "https://github.com/Jon-Ting/sphractal"
 documentation = "https://sphractal.readthedocs.io/en/latest/"
```

### Comparing `sphractal-1.1.3/setup.py` & `sphractal-1.1.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-__version__ = '1.1.3'
+__version__ = '1.1.4'
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sphractal",
     version=__version__,
     author="Jonathan Yik Chang Ting",
```

### Comparing `sphractal-1.1.3/src/sphractal/__init__.py` & `sphractal-1.1.4/src/sphractal/__init__.py`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/boxCnt.py` & `sphractal-1.1.4/src/sphractal/boxCnt.py`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/constants.py` & `sphractal-1.1.4/src/sphractal/constants.py`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/caseStudyOTS1T000.xyz` & `sphractal-1.1.4/src/sphractal/data/caseStudyOTS1T000.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/caseStudyOTS1T323.xyz` & `sphractal-1.1.4/src/sphractal/data/caseStudyOTS1T323.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/caseStudyOTS1T523.xyz` & `sphractal-1.1.4/src/sphractal/data/caseStudyOTS1T523.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/caseStudyOTS2T000.xyz` & `sphractal-1.1.4/src/sphractal/data/caseStudyOTS2T000.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/caseStudyOTS2T323.xyz` & `sphractal-1.1.4/src/sphractal/data/caseStudyOTS2T323.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/caseStudyOTS2T523.xyz` & `sphractal-1.1.4/src/sphractal/data/caseStudyOTS2T523.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/caseStudyRDS1T000.xyz` & `sphractal-1.1.4/src/sphractal/data/caseStudyRDS1T000.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/caseStudyRDS1T323.xyz` & `sphractal-1.1.4/src/sphractal/data/caseStudyRDS1T323.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/caseStudyRDS1T523.xyz` & `sphractal-1.1.4/src/sphractal/data/caseStudyRDS1T523.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/caseStudyRDS2T000.xyz` & `sphractal-1.1.4/src/sphractal/data/caseStudyRDS2T000.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/caseStudyRDS2T323.xyz` & `sphractal-1.1.4/src/sphractal/data/caseStudyRDS2T323.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/caseStudyRDS2T523.xyz` & `sphractal-1.1.4/src/sphractal/data/caseStudyRDS2T523.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/caseStudyTHS1T000.xyz` & `sphractal-1.1.4/src/sphractal/data/caseStudyTHS1T000.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/caseStudyTHS1T323.xyz` & `sphractal-1.1.4/src/sphractal/data/caseStudyTHS1T323.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/caseStudyTHS1T523.xyz` & `sphractal-1.1.4/src/sphractal/data/caseStudyTHS1T523.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/caseStudyTHS2T000.xyz` & `sphractal-1.1.4/src/sphractal/data/caseStudyTHS2T000.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/caseStudyTHS2T323.xyz` & `sphractal-1.1.4/src/sphractal/data/caseStudyTHS2T323.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/caseStudyTHS2T523.xyz` & `sphractal-1.1.4/src/sphractal/data/caseStudyTHS2T523.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/dna.xyz` & `sphractal-1.1.4/src/sphractal/data/dna.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/exampleOT.xyz` & `sphractal-1.1.4/src/sphractal/data/exampleOT.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/graphene.xyz` & `sphractal-1.1.4/src/sphractal/data/graphene.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/paracetamol.xyz` & `sphractal-1.1.4/src/sphractal/data/paracetamol.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/strongScalingSP.xyz` & `sphractal-1.1.4/src/sphractal/data/strongScalingSP.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/weakScalingSP00.xyz` & `sphractal-1.1.4/src/sphractal/data/weakScalingSP00.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/weakScalingSP01.xyz` & `sphractal-1.1.4/src/sphractal/data/weakScalingSP01.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/weakScalingSP02.xyz` & `sphractal-1.1.4/src/sphractal/data/weakScalingSP02.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/weakScalingSP03.xyz` & `sphractal-1.1.4/src/sphractal/data/weakScalingSP03.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/weakScalingSP04.xyz` & `sphractal-1.1.4/src/sphractal/data/weakScalingSP04.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/weakScalingSP05.xyz` & `sphractal-1.1.4/src/sphractal/data/weakScalingSP05.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/weakScalingSP06.xyz` & `sphractal-1.1.4/src/sphractal/data/weakScalingSP06.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/weakScalingSP07.xyz` & `sphractal-1.1.4/src/sphractal/data/weakScalingSP07.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/weakScalingSP08.xyz` & `sphractal-1.1.4/src/sphractal/data/weakScalingSP08.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/weakScalingSP09.xyz` & `sphractal-1.1.4/src/sphractal/data/weakScalingSP09.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/weakScalingSP10.xyz` & `sphractal-1.1.4/src/sphractal/data/weakScalingSP10.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/data/weakScalingSP11.xyz` & `sphractal-1.1.4/src/sphractal/data/weakScalingSP11.xyz`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/datasets.py` & `sphractal-1.1.4/src/sphractal/datasets.py`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/surfExact.py` & `sphractal-1.1.4/src/sphractal/surfExact.py`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/surfVoxel.py` & `sphractal-1.1.4/src/sphractal/surfVoxel.py`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/src/sphractal/utils.py` & `sphractal-1.1.4/src/sphractal/utils.py`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/tests/fixtures.py` & `sphractal-1.1.4/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/tests/test_sphractal.py` & `sphractal-1.1.4/tests/test_sphractal.py`

 * *Files identical despite different names*

### Comparing `sphractal-1.1.3/PKG-INFO` & `sphractal-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphractal
-Version: 1.1.3
+Version: 1.1.4
 Summary: Package to estimate fractal dimension of 3D surfaces formed from overlapping spheres via box-counting algorithm.
 Home-page: https://github.com/Jon-Ting/sphractal
 License: MIT
 Keywords: box-counting,box-count,fractal,dimension,sphere,surface
 Author: Jonathan Yik Chang Ting
 Author-email: jonting97@gmail.com
 Requires-Python: >=3.9
```

