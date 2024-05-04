# Comparing `tmp/kobo_highlights_extractor-0.0.1.tar.gz` & `tmp/kobo_highlights_extractor-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kobo_highlights_extractor-0.0.1.tar", last modified: Thu May  2 20:25:23 2024, max compression
+gzip compressed data, was "kobo_highlights_extractor-0.0.11.tar", last modified: Fri May  3 16:50:52 2024, max compression
```

## Comparing `kobo_highlights_extractor-0.0.1.tar` & `kobo_highlights_extractor-0.0.11.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:25:23.550459 kobo_highlights_extractor-0.0.1/
--rw-rw-rw-   0 root         (0) root         (0)    35100 2024-05-02 20:25:18.000000 kobo_highlights_extractor-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2808 2024-05-02 20:25:23.550459 kobo_highlights_extractor-0.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2146 2024-05-02 20:25:18.000000 kobo_highlights_extractor-0.0.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      788 2024-05-02 20:25:18.000000 kobo_highlights_extractor-0.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-02 20:25:23.550459 kobo_highlights_extractor-0.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      700 2024-05-02 20:25:18.000000 kobo_highlights_extractor-0.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:25:23.547459 kobo_highlights_extractor-0.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:25:23.549459 kobo_highlights_extractor-0.0.1/src/kobo_highlights_extractor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-02 20:25:19.000000 kobo_highlights_extractor-0.0.1/src/kobo_highlights_extractor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5236 2024-05-02 20:25:18.000000 kobo_highlights_extractor-0.0.1/src/kobo_highlights_extractor/extractor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:25:23.550459 kobo_highlights_extractor-0.0.1/src/kobo_highlights_extractor.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2808 2024-05-02 20:25:23.000000 kobo_highlights_extractor-0.0.1/src/kobo_highlights_extractor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      338 2024-05-02 20:25:23.000000 kobo_highlights_extractor-0.0.1/src/kobo_highlights_extractor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:25:23.000000 kobo_highlights_extractor-0.0.1/src/kobo_highlights_extractor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       26 2024-05-02 20:25:23.000000 kobo_highlights_extractor-0.0.1/src/kobo_highlights_extractor.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:50:52.843857 kobo_highlights_extractor-0.0.11/
+-rw-rw-rw-   0 root         (0) root         (0)    35100 2024-05-03 16:50:48.000000 kobo_highlights_extractor-0.0.11/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2838 2024-05-03 16:50:52.842857 kobo_highlights_extractor-0.0.11/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2146 2024-05-03 16:50:48.000000 kobo_highlights_extractor-0.0.11/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      753 2024-05-03 16:50:48.000000 kobo_highlights_extractor-0.0.11/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-03 16:50:52.843857 kobo_highlights_extractor-0.0.11/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      460 2024-05-03 16:50:48.000000 kobo_highlights_extractor-0.0.11/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:50:52.839857 kobo_highlights_extractor-0.0.11/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:50:52.841857 kobo_highlights_extractor-0.0.11/src/kobo_highlights_extractor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 16:50:48.000000 kobo_highlights_extractor-0.0.11/src/kobo_highlights_extractor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5236 2024-05-03 16:50:48.000000 kobo_highlights_extractor-0.0.11/src/kobo_highlights_extractor/extractor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 16:50:52.842857 kobo_highlights_extractor-0.0.11/src/kobo_highlights_extractor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2838 2024-05-03 16:50:52.000000 kobo_highlights_extractor-0.0.11/src/kobo_highlights_extractor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      390 2024-05-03 16:50:52.000000 kobo_highlights_extractor-0.0.11/src/kobo_highlights_extractor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 16:50:52.000000 kobo_highlights_extractor-0.0.11/src/kobo_highlights_extractor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-03 16:50:52.000000 kobo_highlights_extractor-0.0.11/src/kobo_highlights_extractor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-05-03 16:50:52.000000 kobo_highlights_extractor-0.0.11/src/kobo_highlights_extractor.egg-info/top_level.txt
```

### Comparing `kobo_highlights_extractor-0.0.1/LICENSE` & `kobo_highlights_extractor-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `kobo_highlights_extractor-0.0.1/PKG-INFO` & `kobo_highlights_extractor-0.0.11/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: kobo-highlights-extractor
-Version: 0.0.1
+Version: 0.0.11
 Summary: A package to extract highlights from kobo books
 Author-email: Toni Miquel Llull <tonimiquel.llull@gmail.com>
 Project-URL: Homepage, https://gitlab.com/tmllull/kobo-highlights-extractor
 Project-URL: Bug Tracker, https://gitlab.com/tmllull/kobo-highlights-extractor/issues
 Project-URL: Documentation, https://kobo-highlights-extractor.readthedocs.io
 Keywords: kobo,ereader
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Jinja2==3.1.3
 
 # Description
 
 With this script you can get the highlights from Kobo reader using the sqlite file. The reason I made it is because when you export the highlights, a basic information as the page where are located is not exported. Oh, thanks, Kobo, for this useless option. When I highlight something usually I want to reference in other place, so maybe I need to search in the original content to expand the context.
 
 ## Basic Usage
```

### Comparing `kobo_highlights_extractor-0.0.1/README.md` & `kobo_highlights_extractor-0.0.11/README.md`

 * *Files identical despite different names*

### Comparing `kobo_highlights_extractor-0.0.1/src/kobo_highlights_extractor/extractor.py` & `kobo_highlights_extractor-0.0.11/src/kobo_highlights_extractor/extractor.py`

 * *Files identical despite different names*

### Comparing `kobo_highlights_extractor-0.0.1/src/kobo_highlights_extractor.egg-info/PKG-INFO` & `kobo_highlights_extractor-0.0.11/src/kobo_highlights_extractor.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: kobo-highlights-extractor
-Version: 0.0.1
+Version: 0.0.11
 Summary: A package to extract highlights from kobo books
 Author-email: Toni Miquel Llull <tonimiquel.llull@gmail.com>
 Project-URL: Homepage, https://gitlab.com/tmllull/kobo-highlights-extractor
 Project-URL: Bug Tracker, https://gitlab.com/tmllull/kobo-highlights-extractor/issues
 Project-URL: Documentation, https://kobo-highlights-extractor.readthedocs.io
 Keywords: kobo,ereader
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Jinja2==3.1.3
 
 # Description
 
 With this script you can get the highlights from Kobo reader using the sqlite file. The reason I made it is because when you export the highlights, a basic information as the page where are located is not exported. Oh, thanks, Kobo, for this useless option. When I highlight something usually I want to reference in other place, so maybe I need to search in the original content to expand the context.
 
 ## Basic Usage
```

