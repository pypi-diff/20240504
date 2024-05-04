# Comparing `tmp/mo_files-6.609.24119.tar.gz` & `tmp/mo_files-6.619.24125.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo_files-6.609.24119.tar", last modified: Sun Apr 28 22:30:08 2024, max compression
+gzip compressed data, was "mo_files-6.619.24125.tar", last modified: Sat May  4 17:38:01 2024, max compression
```

## Comparing `mo_files-6.609.24119.tar` & `mo_files-6.619.24125.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 22:30:08.348011 mo_files-6.609.24119/
--rw-rw-rw-   0        0        0    16725 2019-09-12 21:03:36.000000 mo_files-6.609.24119/LICENSE
--rw-rw-rw-   0        0        0     2203 2024-04-28 22:30:08.346975 mo_files-6.609.24119/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2024-03-15 11:56:17.000000 mo_files-6.609.24119/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 22:30:08.337784 mo_files-6.609.24119/mo_files/
--rw-rw-rw-   0        0        0    19265 2024-03-02 21:33:58.000000 mo_files-6.609.24119/mo_files/__init__.py
--rw-rw-rw-   0        0        0      431 2024-01-28 14:54:30.000000 mo_files-6.609.24119/mo_files/mimetype.py
--rw-rw-rw-   0        0        0    11596 2024-03-10 19:21:39.000000 mo_files-6.609.24119/mo_files/url.py
-drwxrwxrwx   0        0        0        0 2024-04-28 22:30:08.345919 mo_files-6.609.24119/mo_files.egg-info/
--rw-rw-rw-   0        0        0     2203 2024-04-28 22:30:08.000000 mo_files-6.609.24119/mo_files.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-04-28 22:30:08.000000 mo_files-6.609.24119/mo_files.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 22:30:08.000000 mo_files-6.609.24119/mo_files.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-21 02:35:58.000000 mo_files-6.609.24119/mo_files.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      140 2024-04-28 22:30:08.000000 mo_files-6.609.24119/mo_files.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-28 22:30:08.000000 mo_files-6.609.24119/mo_files.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 22:30:08.348011 mo_files-6.609.24119/setup.cfg
--rw-rw-rw-   0        0        0     2236 2024-04-28 22:30:04.000000 mo_files-6.609.24119/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 17:38:01.784180 mo_files-6.619.24125/
+-rw-rw-rw-   0        0        0    16725 2019-09-12 21:03:36.000000 mo_files-6.619.24125/LICENSE
+-rw-rw-rw-   0        0        0     2204 2024-05-04 17:38:01.783116 mo_files-6.619.24125/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2024-03-15 11:56:17.000000 mo_files-6.619.24125/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 17:38:01.767095 mo_files-6.619.24125/mo_files/
+-rw-rw-rw-   0        0        0    19265 2024-03-02 21:33:58.000000 mo_files-6.619.24125/mo_files/__init__.py
+-rw-rw-rw-   0        0        0      431 2024-01-28 14:54:30.000000 mo_files-6.619.24125/mo_files/mimetype.py
+-rw-rw-rw-   0        0        0    11596 2024-03-10 19:21:39.000000 mo_files-6.619.24125/mo_files/url.py
+drwxrwxrwx   0        0        0        0 2024-05-04 17:38:01.781661 mo_files-6.619.24125/mo_files.egg-info/
+-rw-rw-rw-   0        0        0     2204 2024-05-04 17:38:01.000000 mo_files-6.619.24125/mo_files.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-05-04 17:38:01.000000 mo_files-6.619.24125/mo_files.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 17:38:01.000000 mo_files-6.619.24125/mo_files.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-03-21 02:35:58.000000 mo_files-6.619.24125/mo_files.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      141 2024-05-04 17:38:01.000000 mo_files-6.619.24125/mo_files.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-04 17:38:01.000000 mo_files-6.619.24125/mo_files.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 17:38:01.784180 mo_files-6.619.24125/setup.cfg
+-rw-rw-rw-   0        0        0     2237 2024-05-04 17:37:56.000000 mo_files-6.619.24125/setup.py
```

### Comparing `mo_files-6.609.24119/LICENSE` & `mo_files-6.619.24125/LICENSE`

 * *Files identical despite different names*

### Comparing `mo_files-6.609.24119/PKG-INFO` & `mo_files-6.619.24125/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,20 @@
-Metadata-Version: 2.1
-Name: mo-files
-Version: 6.609.24119
-Summary: More Files! Steamlined for UTF8 and JSON.
-Home-page: https://github.com/klahnakoski/mo-files
-Author: Kyle Lahnakoski
-Author-email: kyle@lahnakoski.com
-License: MPL 2.0
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: mo-dots==9.606.24115
-Requires-Dist: mo-future==7.584.24095
-Requires-Dist: mo-json==6.609.24119
-Requires-Dist: mo-logs==8.608.24119
-Requires-Dist: mo-math==7.606.24115
-Provides-Extra: tests
-Requires-Dist: mo-testing>=8.591.24112; extra == "tests"
-
-# More Files!
-
-[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-files.svg)](https://pypi.org/project/mo-files/)
-[![Build Status](https://github.com/klahnakoski/mo-files/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-files/actions/workflows/build.yml)
-[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-files/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-files?branch=dev)
-[![Downloads](https://pepy.tech/badge/mo-files/month)](https://pepy.tech/project/mo-files)
-
-The `File` class makes the default assumption all files have cr-delimited unicode content that is UTF-8 encoded. This is great for JSON files. It also provides better operators over some common file manipulations.
-
-
-
-
-## Recent changes
-
-**Version 6.x**
-
-Get a little closer to Python's pathlib module standards
-
-* `stem` - to refer file name without extension
-* `os_path` - to get the os-specific absolute path for use in other Python modules
-* `rel_path` - the given path 
-* `abs_path` - was `abspath`, added underscore for consistency 
-
-
-
+# encoding: utf-8
+# THIS FILE IS AUTOGENERATED!
+from setuptools import setup
+setup(
+    author='Kyle Lahnakoski',
+    author_email='kyle@lahnakoski.com',
+    classifiers=["Development Status :: 4 - Beta","Programming Language :: Python :: 3.8","Programming Language :: Python :: 3.9","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules","License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)","Programming Language :: Python :: 3.10","Programming Language :: Python :: 3.11","Programming Language :: Python :: 3.12"],
+    description='More Files! Steamlined for UTF8 and JSON.',
+    extras_require={"tests":["mo-testing>=8.608.24119"]},
+    include_package_data=True,
+    install_requires=["mo-dots==10.615.24125","mo-future==7.584.24095","mo-json==6.619.24125","mo-logs==8.618.24125","mo-math==7.616.24125"],
+    license='MPL 2.0',
+    long_description="# More Files!\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-files.svg)](https://pypi.org/project/mo-files/)\n[![Build Status](https://github.com/klahnakoski/mo-files/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-files/actions/workflows/build.yml)\n[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-files/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-files?branch=dev)\n[![Downloads](https://pepy.tech/badge/mo-files/month)](https://pepy.tech/project/mo-files)\n\nThe `File` class makes the default assumption all files have cr-delimited unicode content that is UTF-8 encoded. This is great for JSON files. It also provides better operators over some common file manipulations.\n\n\n\n\n## Recent changes\n\n**Version 6.x**\n\nGet a little closer to Python's pathlib module standards\n\n* `stem` - to refer file name without extension\n* `os_path` - to get the os-specific absolute path for use in other Python modules\n* `rel_path` - the given path \n* `abs_path` - was `abspath`, added underscore for consistency \n\n\n\n",
+    long_description_content_type='text/markdown',
+    name='mo-files',
+    packages=["mo_files"],
+    url='https://github.com/klahnakoski/mo-files',
+    version='6.619.24125',
+    zip_safe=False
+)
```

### Comparing `mo_files-6.609.24119/README.md` & `mo_files-6.619.24125/README.md`

 * *Files identical despite different names*

### Comparing `mo_files-6.609.24119/mo_files/__init__.py` & `mo_files-6.619.24125/mo_files/__init__.py`

 * *Files identical despite different names*

### Comparing `mo_files-6.609.24119/mo_files/url.py` & `mo_files-6.619.24125/mo_files/url.py`

 * *Files identical despite different names*

### Comparing `mo_files-6.609.24119/mo_files.egg-info/PKG-INFO` & `mo_files-6.619.24125/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-files
-Version: 6.609.24119
+Version: 6.619.24125
 Summary: More Files! Steamlined for UTF8 and JSON.
 Home-page: https://github.com/klahnakoski/mo-files
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.8
@@ -13,21 +13,21 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots==9.606.24115
+Requires-Dist: mo-dots==10.615.24125
 Requires-Dist: mo-future==7.584.24095
-Requires-Dist: mo-json==6.609.24119
-Requires-Dist: mo-logs==8.608.24119
-Requires-Dist: mo-math==7.606.24115
+Requires-Dist: mo-json==6.619.24125
+Requires-Dist: mo-logs==8.618.24125
+Requires-Dist: mo-math==7.616.24125
 Provides-Extra: tests
-Requires-Dist: mo-testing>=8.591.24112; extra == "tests"
+Requires-Dist: mo-testing>=8.608.24119; extra == "tests"
 
 # More Files!
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/mo-files.svg)](https://pypi.org/project/mo-files/)
 [![Build Status](https://github.com/klahnakoski/mo-files/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-files/actions/workflows/build.yml)
 [![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-files/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-files?branch=dev)
 [![Downloads](https://pepy.tech/badge/mo-files/month)](https://pepy.tech/project/mo-files)
```

