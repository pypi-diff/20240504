# Comparing `tmp/EAP-1.1.8.tar.gz` & `tmp/EAP-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EAP-1.1.8.tar", last modified: Wed Sep 28 09:04:04 2022, max compression
+gzip compressed data, was "EAP-1.1.9.tar", last modified: Wed Sep 28 09:33:48 2022, max compression
```

## Comparing `EAP-1.1.8.tar` & `EAP-1.1.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2022-09-28 09:04:04.474459 EAP-1.1.8/
-drwxrwxrwx   0        0        0        0 2022-09-28 09:04:04.312394 EAP-1.1.8/EAP/
--rw-rw-rw-   0        0        0      280 2022-01-30 16:33:17.000000 EAP-1.1.8/EAP/__init__.py
--rw-rw-rw-   0        0        0     4301 2022-09-28 08:52:49.000000 EAP-1.1.8/EAP/adjust.py
--rw-rw-rw-   0        0        0      540 2022-09-15 15:18:04.000000 EAP-1.1.8/EAP/api.py
--rw-rw-rw-   0        0        0     2736 2021-12-28 12:29:35.000000 EAP-1.1.8/EAP/autoencoder.py
--rw-rw-rw-   0        0        0     7767 2022-09-28 08:26:23.000000 EAP-1.1.8/EAP/cross_section_regress.py
--rw-rw-rw-   0        0        0    15570 2022-09-28 08:56:49.000000 EAP-1.1.8/EAP/fama_macbeth.py
--rw-rw-rw-   0        0        0    71115 2022-09-28 08:59:34.000000 EAP-1.1.8/EAP/portfolio_analysis.py
-drwxrwxrwx   0        0        0        0 2022-09-28 09:04:04.452518 EAP-1.1.8/EAP/test/
--rw-rw-rw-   0        0        0        0 2021-05-20 03:02:12.000000 EAP-1.1.8/EAP/test/__init__.py
--rw-rw-rw-   0        0        0     3178 2022-02-14 16:48:38.000000 EAP-1.1.8/EAP/test/test_adjust.py
--rw-rw-rw-   0        0        0     4771 2021-12-28 13:03:14.000000 EAP-1.1.8/EAP/test/test_autoencoder.py
--rw-rw-rw-   0        0        0     2960 2021-05-31 09:18:16.000000 EAP-1.1.8/EAP/test/test_cross_section_regress.py
--rw-rw-rw-   0        0        0     2684 2022-09-20 08:46:37.000000 EAP-1.1.8/EAP/test/test_fama_macbeth.py
--rw-rw-rw-   0        0        0    15642 2022-09-26 12:46:18.000000 EAP-1.1.8/EAP/test/test_portfolio_analysis.py
--rw-rw-rw-   0        0        0     1933 2022-08-28 13:12:55.000000 EAP-1.1.8/EAP/test/test_time_frequency.py
--rw-rw-rw-   0        0        0      725 2022-01-02 06:23:25.000000 EAP-1.1.8/EAP/test/test_time_series_regress.py
--rw-rw-rw-   0        0        0     9328 2022-07-06 15:11:29.000000 EAP-1.1.8/EAP/time_frequency.py
--rw-rw-rw-   0        0        0     4892 2022-09-28 09:01:01.000000 EAP-1.1.8/EAP/time_series_regress.py
-drwxrwxrwx   0        0        0        0 2022-09-28 09:04:04.366747 EAP-1.1.8/EAP.egg-info/
--rw-rw-rw-   0        0        0   699417 2022-09-28 09:04:02.000000 EAP-1.1.8/EAP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      592 2022-09-28 09:04:03.000000 EAP-1.1.8/EAP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-28 09:04:02.000000 EAP-1.1.8/EAP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2022-09-28 09:04:02.000000 EAP-1.1.8/EAP.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2022-09-28 09:04:02.000000 EAP-1.1.8/EAP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2022-02-12 09:18:10.000000 EAP-1.1.8/LICENSE
--rw-rw-rw-   0        0        0   699417 2022-09-28 09:04:04.462490 EAP-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0       59 2022-02-12 09:19:43.000000 EAP-1.1.8/README.md
--rw-rw-rw-   0        0        0       42 2022-09-28 09:04:04.474459 EAP-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1385 2022-09-28 08:48:28.000000 EAP-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-09-28 09:33:48.169965 EAP-1.1.9/
+drwxrwxrwx   0        0        0        0 2022-09-28 09:33:48.086190 EAP-1.1.9/EAP/
+-rw-rw-rw-   0        0        0      234 2022-09-28 09:30:57.000000 EAP-1.1.9/EAP/__init__.py
+-rw-rw-rw-   0        0        0     4301 2022-09-28 08:52:49.000000 EAP-1.1.9/EAP/adjust.py
+-rw-rw-rw-   0        0        0      540 2022-09-15 15:18:04.000000 EAP-1.1.9/EAP/api.py
+-rw-rw-rw-   0        0        0     2736 2021-12-28 12:29:35.000000 EAP-1.1.9/EAP/autoencoder.py
+-rw-rw-rw-   0        0        0     7767 2022-09-28 08:26:23.000000 EAP-1.1.9/EAP/cross_section_regress.py
+-rw-rw-rw-   0        0        0    15571 2022-09-28 09:31:12.000000 EAP-1.1.9/EAP/fama_macbeth.py
+-rw-rw-rw-   0        0        0    71115 2022-09-28 08:59:34.000000 EAP-1.1.9/EAP/portfolio_analysis.py
+drwxrwxrwx   0        0        0        0 2022-09-28 09:33:48.161986 EAP-1.1.9/EAP/test/
+-rw-rw-rw-   0        0        0        0 2021-05-20 03:02:12.000000 EAP-1.1.9/EAP/test/__init__.py
+-rw-rw-rw-   0        0        0     3178 2022-02-14 16:48:38.000000 EAP-1.1.9/EAP/test/test_adjust.py
+-rw-rw-rw-   0        0        0     4771 2021-12-28 13:03:14.000000 EAP-1.1.9/EAP/test/test_autoencoder.py
+-rw-rw-rw-   0        0        0     2960 2021-05-31 09:18:16.000000 EAP-1.1.9/EAP/test/test_cross_section_regress.py
+-rw-rw-rw-   0        0        0     2684 2022-09-20 08:46:37.000000 EAP-1.1.9/EAP/test/test_fama_macbeth.py
+-rw-rw-rw-   0        0        0    15642 2022-09-26 12:46:18.000000 EAP-1.1.9/EAP/test/test_portfolio_analysis.py
+-rw-rw-rw-   0        0        0     1933 2022-08-28 13:12:55.000000 EAP-1.1.9/EAP/test/test_time_frequency.py
+-rw-rw-rw-   0        0        0      725 2022-01-02 06:23:25.000000 EAP-1.1.9/EAP/test/test_time_series_regress.py
+-rw-rw-rw-   0        0        0     9328 2022-07-06 15:11:29.000000 EAP-1.1.9/EAP/time_frequency.py
+-rw-rw-rw-   0        0        0     4892 2022-09-28 09:01:01.000000 EAP-1.1.9/EAP/time_series_regress.py
+drwxrwxrwx   0        0        0        0 2022-09-28 09:33:48.136057 EAP-1.1.9/EAP.egg-info/
+-rw-rw-rw-   0        0        0   699417 2022-09-28 09:33:47.000000 EAP-1.1.9/EAP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      592 2022-09-28 09:33:47.000000 EAP-1.1.9/EAP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-09-28 09:33:47.000000 EAP-1.1.9/EAP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2022-09-28 09:33:47.000000 EAP-1.1.9/EAP.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2022-09-28 09:33:47.000000 EAP-1.1.9/EAP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2022-02-12 09:18:10.000000 EAP-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0   699417 2022-09-28 09:33:48.168992 EAP-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       59 2022-02-12 09:19:43.000000 EAP-1.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2022-09-28 09:33:48.169965 EAP-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1385 2022-09-28 09:32:20.000000 EAP-1.1.9/setup.py
```

### Comparing `EAP-1.1.8/EAP/adjust.py` & `EAP-1.1.9/EAP/adjust.py`

 * *Files identical despite different names*

### Comparing `EAP-1.1.8/EAP/api.py` & `EAP-1.1.9/EAP/api.py`

 * *Files identical despite different names*

### Comparing `EAP-1.1.8/EAP/autoencoder.py` & `EAP-1.1.9/EAP/autoencoder.py`

 * *Files identical despite different names*

### Comparing `EAP-1.1.8/EAP/cross_section_regress.py` & `EAP-1.1.9/EAP/cross_section_regress.py`

 * *Files identical despite different names*

### Comparing `EAP-1.1.8/EAP/fama_macbeth.py` & `EAP-1.1.9/EAP/fama_macbeth.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 1. specify the model and take cross-sectional regression 确定模型，进行截面回归 
 2. take the time-series average of regress coefficient 对系数在时间序列上取平均
 
 For more academic reference: 
 Empirical Asset Pricing: The Cross Section of Stock Returns. Bali, Engle, Murray. 2016.
 '''
 
-from adjust import newey_west_t
+from .adjust import newey_west_t
 
 class Fama_macbeth_regress():
     '''
     fama_macbeth_regress follwing two steps
     Need Package: numpy,statsmodels,scipy,prettytable
     '''
     def __init__(self, sample):
```

### Comparing `EAP-1.1.8/EAP/portfolio_analysis.py` & `EAP-1.1.9/EAP/portfolio_analysis.py`

 * *Files identical despite different names*

### Comparing `EAP-1.1.8/EAP/test/test_adjust.py` & `EAP-1.1.9/EAP/test/test_adjust.py`

 * *Files identical despite different names*

### Comparing `EAP-1.1.8/EAP/test/test_autoencoder.py` & `EAP-1.1.9/EAP/test/test_autoencoder.py`

 * *Files identical despite different names*

### Comparing `EAP-1.1.8/EAP/test/test_cross_section_regress.py` & `EAP-1.1.9/EAP/test/test_cross_section_regress.py`

 * *Files identical despite different names*

### Comparing `EAP-1.1.8/EAP/test/test_fama_macbeth.py` & `EAP-1.1.9/EAP/test/test_fama_macbeth.py`

 * *Files identical despite different names*

### Comparing `EAP-1.1.8/EAP/test/test_portfolio_analysis.py` & `EAP-1.1.9/EAP/test/test_portfolio_analysis.py`

 * *Files identical despite different names*

### Comparing `EAP-1.1.8/EAP/test/test_time_frequency.py` & `EAP-1.1.9/EAP/test/test_time_frequency.py`

 * *Files identical despite different names*

### Comparing `EAP-1.1.8/EAP/test/test_time_series_regress.py` & `EAP-1.1.9/EAP/test/test_time_series_regress.py`

 * *Files identical despite different names*

### Comparing `EAP-1.1.8/EAP/time_frequency.py` & `EAP-1.1.9/EAP/time_frequency.py`

 * *Files identical despite different names*

### Comparing `EAP-1.1.8/EAP/time_series_regress.py` & `EAP-1.1.9/EAP/time_series_regress.py`

 * *Files identical despite different names*

### Comparing `EAP-1.1.8/EAP.egg-info/PKG-INFO` & `EAP-1.1.9/EAP.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2045 4150  : 2.1..Name: EAP
-00000020: 0d0a 5665 7273 696f 6e3a 2031 2e31 2e38  ..Version: 1.1.8
+00000020: 0d0a 5665 7273 696f 6e3a 2031 2e31 2e39  ..Version: 1.1.9
 00000030: 0d0a 5375 6d6d 6172 793a 2054 6869 7320  ..Summary: This 
 00000040: 7061 636b 6167 6520 6973 2064 6573 6967  package is desig
 00000050: 6e65 6420 666f 7220 656d 7069 7269 6361  ned for empirica
 00000060: 6c20 6173 7365 7420 7072 6963 696e 670d  l asset pricing.
 00000070: 0a48 6f6d 652d 7061 6765 3a20 6874 7470  .Home-page: http
 00000080: 733a 2f2f 7768 7965 636f 6669 6c69 7465  s://whyecofilite
 00000090: 722e 6769 7468 7562 2e69 6f2f 4541 502f  r.github.io/EAP/
```

### Comparing `EAP-1.1.8/EAP.egg-info/SOURCES.txt` & `EAP-1.1.9/EAP.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EAP-1.1.8/LICENSE` & `EAP-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `EAP-1.1.8/PKG-INFO` & `EAP-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2045 4150  : 2.1..Name: EAP
-00000020: 0d0a 5665 7273 696f 6e3a 2031 2e31 2e38  ..Version: 1.1.8
+00000020: 0d0a 5665 7273 696f 6e3a 2031 2e31 2e39  ..Version: 1.1.9
 00000030: 0d0a 5375 6d6d 6172 793a 2054 6869 7320  ..Summary: This 
 00000040: 7061 636b 6167 6520 6973 2064 6573 6967  package is desig
 00000050: 6e65 6420 666f 7220 656d 7069 7269 6361  ned for empirica
 00000060: 6c20 6173 7365 7420 7072 6963 696e 670d  l asset pricing.
 00000070: 0a48 6f6d 652d 7061 6765 3a20 6874 7470  .Home-page: http
 00000080: 733a 2f2f 7768 7965 636f 6669 6c69 7465  s://whyecofilite
 00000090: 722e 6769 7468 7562 2e69 6f2f 4541 502f  r.github.io/EAP/
```

### Comparing `EAP-1.1.8/setup.py` & `EAP-1.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("./EAP/Documentation.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "EAP", # package name
-    version = "1.1.8", # version
+    version = "1.1.9", # version
     author = "whyecofiliter", # author name
     author_email = "why_ecofiliter@126.com",
     description = "This package is designed for empirical asset pricing", # description
     long_description = long_description, # documnetation
     long_description_content_type = "text/markdown", # documentation type
     url = "https://whyecofiliter.github.io/EAP/", # url in Github
     packages = setuptools.find_packages(), # automatic package searching
```

