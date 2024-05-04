# Comparing `tmp/pdfplumber-aemc-0.7.6.tar.gz` & `tmp/pdfplumber-aemc-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfplumber-aemc-0.7.6.tar", last modified: Tue Jan 10 12:46:57 2023, max compression
+gzip compressed data, was "pdfplumber-aemc-0.7.7.tar", last modified: Tue Jan 10 13:10:57 2023, max compression
```

## Comparing `pdfplumber-aemc-0.7.6.tar` & `pdfplumber-aemc-0.7.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jun        (502) staff       (20)        0 2023-01-10 12:46:57.410232 pdfplumber-aemc-0.7.6/
--rw-rw-r--   0 jun        (502) staff       (20)     1086 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.6/LICENSE.txt
--rw-rw-r--   0 jun        (502) staff       (20)       66 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.6/MANIFEST.in
--rw-r--r--   0 jun        (502) staff       (20)    32927 2023-01-10 12:46:57.410563 pdfplumber-aemc-0.7.6/PKG-INFO
--rw-rw-r--   0 jun        (502) staff       (20)    32263 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.6/README.md
-drwxr-xr-x   0 jun        (502) staff       (20)        0 2023-01-10 12:46:57.406459 pdfplumber-aemc-0.7.6/pdfplumber/
--rw-rw-r--   0 jun        (502) staff       (20)      226 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.6/pdfplumber/__init__.py
--rw-rw-r--   0 jun        (502) staff       (20)      263 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.6/pdfplumber/_typing.py
--rw-rw-r--   0 jun        (502) staff       (20)       72 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.6/pdfplumber/_version.py
--rw-rw-r--   0 jun        (502) staff       (20)     2150 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.6/pdfplumber/cli.py
--rw-rw-r--   0 jun        (502) staff       (20)     5150 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.6/pdfplumber/container.py
--rw-rw-r--   0 jun        (502) staff       (20)     3501 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.6/pdfplumber/convert.py
--rw-rw-r--   0 jun        (502) staff       (20)      816 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.6/pdfplumber/ctm.py
--rw-rw-r--   0 jun        (502) staff       (20)    11859 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.6/pdfplumber/display.py
--rw-rw-r--   0 jun        (502) staff       (20)    15540 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.6/pdfplumber/page.py
--rw-rw-r--   0 jun        (502) staff       (20)     4878 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.6/pdfplumber/pdf.py
--rw-rw-r--   0 jun        (502) staff       (20)        0 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.6/pdfplumber/py.typed
--rw-rw-r--   0 jun        (502) staff       (20)    23058 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.6/pdfplumber/table.py
--rw-rw-r--   0 jun        (502) staff       (20)    28534 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.6/pdfplumber/utils.py
-drwxr-xr-x   0 jun        (502) staff       (20)        0 2023-01-10 12:46:57.409741 pdfplumber-aemc-0.7.6/pdfplumber_aemc.egg-info/
--rw-r--r--   0 jun        (502) staff       (20)    32927 2023-01-10 12:46:57.000000 pdfplumber-aemc-0.7.6/pdfplumber_aemc.egg-info/PKG-INFO
--rw-r--r--   0 jun        (502) staff       (20)      557 2023-01-10 12:46:57.000000 pdfplumber-aemc-0.7.6/pdfplumber_aemc.egg-info/SOURCES.txt
--rw-r--r--   0 jun        (502) staff       (20)        1 2023-01-10 12:46:57.000000 pdfplumber-aemc-0.7.6/pdfplumber_aemc.egg-info/dependency_links.txt
--rw-r--r--   0 jun        (502) staff       (20)       51 2023-01-10 12:46:57.000000 pdfplumber-aemc-0.7.6/pdfplumber_aemc.egg-info/entry_points.txt
--rw-r--r--   0 jun        (502) staff       (20)       49 2023-01-10 12:46:57.000000 pdfplumber-aemc-0.7.6/pdfplumber_aemc.egg-info/requires.txt
--rw-r--r--   0 jun        (502) staff       (20)       11 2023-01-10 12:46:57.000000 pdfplumber-aemc-0.7.6/pdfplumber_aemc.egg-info/top_level.txt
--rw-rw-r--   0 jun        (502) staff       (20)      494 2023-01-10 12:46:57.411483 pdfplumber-aemc-0.7.6/setup.cfg
--rw-rw-r--   0 jun        (502) staff       (20)     1092 2023-01-10 12:45:33.000000 pdfplumber-aemc-0.7.6/setup.py
+drwxr-xr-x   0 jun        (502) staff       (20)        0 2023-01-10 13:10:57.954408 pdfplumber-aemc-0.7.7/
+-rw-rw-r--   0 jun        (502) staff       (20)     1086 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.7/LICENSE.txt
+-rw-rw-r--   0 jun        (502) staff       (20)       66 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.7/MANIFEST.in
+-rw-r--r--   0 jun        (502) staff       (20)    32927 2023-01-10 13:10:57.954714 pdfplumber-aemc-0.7.7/PKG-INFO
+-rw-rw-r--   0 jun        (502) staff       (20)    32263 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.7/README.md
+drwxr-xr-x   0 jun        (502) staff       (20)        0 2023-01-10 13:10:57.951269 pdfplumber-aemc-0.7.7/pdfplumber/
+-rw-rw-r--   0 jun        (502) staff       (20)      226 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.7/pdfplumber/__init__.py
+-rw-rw-r--   0 jun        (502) staff       (20)      263 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.7/pdfplumber/_typing.py
+-rw-rw-r--   0 jun        (502) staff       (20)       72 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.7/pdfplumber/_version.py
+-rw-rw-r--   0 jun        (502) staff       (20)     2150 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.7/pdfplumber/cli.py
+-rw-rw-r--   0 jun        (502) staff       (20)     5150 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.7/pdfplumber/container.py
+-rw-rw-r--   0 jun        (502) staff       (20)     3501 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.7/pdfplumber/convert.py
+-rw-rw-r--   0 jun        (502) staff       (20)      816 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.7/pdfplumber/ctm.py
+-rw-rw-r--   0 jun        (502) staff       (20)    11859 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.7/pdfplumber/display.py
+-rw-rw-r--   0 jun        (502) staff       (20)    15540 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.7/pdfplumber/page.py
+-rw-rw-r--   0 jun        (502) staff       (20)     4878 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.7/pdfplumber/pdf.py
+-rw-rw-r--   0 jun        (502) staff       (20)        0 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.7/pdfplumber/py.typed
+-rw-rw-r--   0 jun        (502) staff       (20)    23058 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.7/pdfplumber/table.py
+-rw-rw-r--   0 jun        (502) staff       (20)    28534 2023-01-10 08:55:55.000000 pdfplumber-aemc-0.7.7/pdfplumber/utils.py
+drwxr-xr-x   0 jun        (502) staff       (20)        0 2023-01-10 13:10:57.953955 pdfplumber-aemc-0.7.7/pdfplumber_aemc.egg-info/
+-rw-r--r--   0 jun        (502) staff       (20)    32927 2023-01-10 13:10:57.000000 pdfplumber-aemc-0.7.7/pdfplumber_aemc.egg-info/PKG-INFO
+-rw-r--r--   0 jun        (502) staff       (20)      557 2023-01-10 13:10:57.000000 pdfplumber-aemc-0.7.7/pdfplumber_aemc.egg-info/SOURCES.txt
+-rw-r--r--   0 jun        (502) staff       (20)        1 2023-01-10 13:10:57.000000 pdfplumber-aemc-0.7.7/pdfplumber_aemc.egg-info/dependency_links.txt
+-rw-r--r--   0 jun        (502) staff       (20)       51 2023-01-10 13:10:57.000000 pdfplumber-aemc-0.7.7/pdfplumber_aemc.egg-info/entry_points.txt
+-rw-r--r--   0 jun        (502) staff       (20)       49 2023-01-10 13:10:57.000000 pdfplumber-aemc-0.7.7/pdfplumber_aemc.egg-info/requires.txt
+-rw-r--r--   0 jun        (502) staff       (20)       11 2023-01-10 13:10:57.000000 pdfplumber-aemc-0.7.7/pdfplumber_aemc.egg-info/top_level.txt
+-rw-rw-r--   0 jun        (502) staff       (20)      494 2023-01-10 13:10:57.955718 pdfplumber-aemc-0.7.7/setup.cfg
+-rw-rw-r--   0 jun        (502) staff       (20)     1092 2023-01-10 13:10:12.000000 pdfplumber-aemc-0.7.7/setup.py
```

### Comparing `pdfplumber-aemc-0.7.6/LICENSE.txt` & `pdfplumber-aemc-0.7.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pdfplumber-aemc-0.7.6/PKG-INFO` & `pdfplumber-aemc-0.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfplumber-aemc
-Version: 0.7.6
+Version: 0.7.7
 Summary: Plumb a PDF for detailed information about each char, rectangle, and line.
 Home-page: https://github.com/wargreymon28/pdfplumber-aemc
 Author: Jeremy Singer-Vine + Liew Chun Fui
 Author-email: wargreymon28@gmail.com
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pdfplumber-aemc-0.7.6/README.md` & `pdfplumber-aemc-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `pdfplumber-aemc-0.7.6/pdfplumber/cli.py` & `pdfplumber-aemc-0.7.7/pdfplumber/cli.py`

 * *Files identical despite different names*

### Comparing `pdfplumber-aemc-0.7.6/pdfplumber/container.py` & `pdfplumber-aemc-0.7.7/pdfplumber/container.py`

 * *Files identical despite different names*

### Comparing `pdfplumber-aemc-0.7.6/pdfplumber/convert.py` & `pdfplumber-aemc-0.7.7/pdfplumber/convert.py`

 * *Files identical despite different names*

### Comparing `pdfplumber-aemc-0.7.6/pdfplumber/ctm.py` & `pdfplumber-aemc-0.7.7/pdfplumber/ctm.py`

 * *Files identical despite different names*

### Comparing `pdfplumber-aemc-0.7.6/pdfplumber/display.py` & `pdfplumber-aemc-0.7.7/pdfplumber/display.py`

 * *Files identical despite different names*

### Comparing `pdfplumber-aemc-0.7.6/pdfplumber/page.py` & `pdfplumber-aemc-0.7.7/pdfplumber/page.py`

 * *Files identical despite different names*

### Comparing `pdfplumber-aemc-0.7.6/pdfplumber/pdf.py` & `pdfplumber-aemc-0.7.7/pdfplumber/pdf.py`

 * *Files identical despite different names*

### Comparing `pdfplumber-aemc-0.7.6/pdfplumber/table.py` & `pdfplumber-aemc-0.7.7/pdfplumber/table.py`

 * *Files identical despite different names*

### Comparing `pdfplumber-aemc-0.7.6/pdfplumber/utils.py` & `pdfplumber-aemc-0.7.7/pdfplumber/utils.py`

 * *Files identical despite different names*

### Comparing `pdfplumber-aemc-0.7.6/pdfplumber_aemc.egg-info/PKG-INFO` & `pdfplumber-aemc-0.7.7/pdfplumber_aemc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfplumber-aemc
-Version: 0.7.6
+Version: 0.7.7
 Summary: Plumb a PDF for detailed information about each char, rectangle, and line.
 Home-page: https://github.com/wargreymon28/pdfplumber-aemc
 Author: Jeremy Singer-Vine + Liew Chun Fui
 Author-email: wargreymon28@gmail.com
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pdfplumber-aemc-0.7.6/pdfplumber_aemc.egg-info/SOURCES.txt` & `pdfplumber-aemc-0.7.7/pdfplumber_aemc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdfplumber-aemc-0.7.6/setup.py` & `pdfplumber-aemc-0.7.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,19 +9,19 @@
     name="pdfplumber-aemc",
     url="https://github.com/wargreymon28/pdfplumber-aemc",
     author="Jeremy Singer-Vine + Liew Chun Fui",
     author_email="wargreymon28@gmail.com",
     description="Plumb a PDF for detailed information about each char, rectangle, and line.",
     long_description=readme,
     long_description_content_type="text/markdown",
-    version="0.7.6",
+    version="0.7.7",
     packages=['pdfplumber'],
     python_requires=">=3.7",
     install_requires=[
-        'pdfminer.aemc==20221115',
+        'pdfminer.aemc==20221105',
         'Pillow>=9.1',
         'Wand>=0.6.10',
     ],
     entry_points={"console_scripts": ["pdfplumber = pdfplumber.cli:main"]},
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
```

