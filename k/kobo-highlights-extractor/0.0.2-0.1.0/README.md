# Comparing `tmp/kobo_highlights_extractor-0.0.2.tar.gz` & `tmp/kobo_highlights_extractor-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kobo_highlights_extractor-0.0.2.tar", last modified: Sat May  4 11:43:14 2024, max compression
+gzip compressed data, was "kobo_highlights_extractor-0.1.0.tar", last modified: Sat May  4 12:39:28 2024, max compression
```

## Comparing `kobo_highlights_extractor-0.0.2.tar` & `kobo_highlights_extractor-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-04 11:43:14.971337 kobo_highlights_extractor-0.0.2/
--rw-rw-rw-   0 root         (0) root         (0)    35100 2024-05-04 11:43:10.000000 kobo_highlights_extractor-0.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2837 2024-05-04 11:43:14.970420 kobo_highlights_extractor-0.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2146 2024-05-04 11:43:10.000000 kobo_highlights_extractor-0.0.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      753 2024-05-04 11:43:10.000000 kobo_highlights_extractor-0.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-04 11:43:14.971337 kobo_highlights_extractor-0.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      398 2024-05-04 11:43:10.000000 kobo_highlights_extractor-0.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-04 11:43:14.968587 kobo_highlights_extractor-0.0.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-04 11:43:14.969504 kobo_highlights_extractor-0.0.2/src/kobo_highlights_extractor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-04 11:43:11.000000 kobo_highlights_extractor-0.0.2/src/kobo_highlights_extractor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5719 2024-05-04 11:43:10.000000 kobo_highlights_extractor-0.0.2/src/kobo_highlights_extractor/extractor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-04 11:43:14.970420 kobo_highlights_extractor-0.0.2/src/kobo_highlights_extractor.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2837 2024-05-04 11:43:14.000000 kobo_highlights_extractor-0.0.2/src/kobo_highlights_extractor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      390 2024-05-04 11:43:14.000000 kobo_highlights_extractor-0.0.2/src/kobo_highlights_extractor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-04 11:43:14.000000 kobo_highlights_extractor-0.0.2/src/kobo_highlights_extractor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-05-04 11:43:14.000000 kobo_highlights_extractor-0.0.2/src/kobo_highlights_extractor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2024-05-04 11:43:14.000000 kobo_highlights_extractor-0.0.2/src/kobo_highlights_extractor.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-04 12:39:28.374877 kobo_highlights_extractor-0.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35100 2024-05-04 12:39:24.000000 kobo_highlights_extractor-0.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2837 2024-05-04 12:39:28.374877 kobo_highlights_extractor-0.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2146 2024-05-04 12:39:24.000000 kobo_highlights_extractor-0.1.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      753 2024-05-04 12:39:24.000000 kobo_highlights_extractor-0.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-04 12:39:28.374877 kobo_highlights_extractor-0.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      398 2024-05-04 12:39:24.000000 kobo_highlights_extractor-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-04 12:39:28.371877 kobo_highlights_extractor-0.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-04 12:39:28.372877 kobo_highlights_extractor-0.1.0/src/kobo_highlights_extractor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-04 12:39:24.000000 kobo_highlights_extractor-0.1.0/src/kobo_highlights_extractor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5719 2024-05-04 12:39:24.000000 kobo_highlights_extractor-0.1.0/src/kobo_highlights_extractor/extractor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-04 12:39:28.373877 kobo_highlights_extractor-0.1.0/src/kobo_highlights_extractor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2837 2024-05-04 12:39:28.000000 kobo_highlights_extractor-0.1.0/src/kobo_highlights_extractor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      390 2024-05-04 12:39:28.000000 kobo_highlights_extractor-0.1.0/src/kobo_highlights_extractor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-04 12:39:28.000000 kobo_highlights_extractor-0.1.0/src/kobo_highlights_extractor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-04 12:39:28.000000 kobo_highlights_extractor-0.1.0/src/kobo_highlights_extractor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-05-04 12:39:28.000000 kobo_highlights_extractor-0.1.0/src/kobo_highlights_extractor.egg-info/top_level.txt
```

### Comparing `kobo_highlights_extractor-0.0.2/LICENSE` & `kobo_highlights_extractor-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kobo_highlights_extractor-0.0.2/PKG-INFO` & `kobo_highlights_extractor-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kobo-highlights-extractor
-Version: 0.0.2
+Version: 0.1.0
 Summary: A package to extract highlights from kobo books
 Author-email: Toni Miquel Llull <tonimiquel.llull@gmail.com>
 Project-URL: Homepage, https://gitlab.com/tmllull/kobo-highlights-extractor
 Project-URL: Bug Tracker, https://gitlab.com/tmllull/kobo-highlights-extractor/issues
 Project-URL: Documentation, https://kobo-highlights-extractor.readthedocs.io
 Keywords: kobo,ereader
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `kobo_highlights_extractor-0.0.2/README.md` & `kobo_highlights_extractor-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `kobo_highlights_extractor-0.0.2/pyproject.toml` & `kobo_highlights_extractor-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kobo_highlights_extractor-0.0.2/src/kobo_highlights_extractor/extractor.py` & `kobo_highlights_extractor-0.1.0/src/kobo_highlights_extractor/extractor.py`

 * *Files identical despite different names*

### Comparing `kobo_highlights_extractor-0.0.2/src/kobo_highlights_extractor.egg-info/PKG-INFO` & `kobo_highlights_extractor-0.1.0/src/kobo_highlights_extractor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kobo-highlights-extractor
-Version: 0.0.2
+Version: 0.1.0
 Summary: A package to extract highlights from kobo books
 Author-email: Toni Miquel Llull <tonimiquel.llull@gmail.com>
 Project-URL: Homepage, https://gitlab.com/tmllull/kobo-highlights-extractor
 Project-URL: Bug Tracker, https://gitlab.com/tmllull/kobo-highlights-extractor/issues
 Project-URL: Documentation, https://kobo-highlights-extractor.readthedocs.io
 Keywords: kobo,ereader
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

