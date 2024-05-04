# Comparing `tmp/mo_streams-1.620.24125.tar.gz` & `tmp/mo_streams-1.624.24125.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo_streams-1.620.24125.tar", last modified: Sat May  4 18:00:13 2024, max compression
+gzip compressed data, was "mo_streams-1.624.24125.tar", last modified: Sat May  4 20:19:34 2024, max compression
```

## Comparing `mo_streams-1.620.24125.tar` & `mo_streams-1.624.24125.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 18:00:13.354850 mo_streams-1.620.24125/
--rw-rw-rw-   0        0        0    17098 2022-11-20 01:40:59.000000 mo_streams-1.620.24125/LICENSE
--rw-rw-rw-   0        0        0     4418 2024-05-04 18:00:13.350459 mo_streams-1.620.24125/PKG-INFO
--rw-rw-rw-   0        0        0     2878 2024-03-02 21:57:33.000000 mo_streams-1.620.24125/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 18:00:13.325498 mo_streams-1.620.24125/mo_streams/
--rw-rw-rw-   0        0        0     5332 2024-05-04 17:59:55.000000 mo_streams-1.620.24125/mo_streams/__init__.py
--rw-rw-rw-   0        0        0     3617 2023-10-31 01:14:42.000000 mo_streams-1.620.24125/mo_streams/_utils.py
--rw-rw-rw-   0        0        0     3867 2023-11-15 00:25:37.000000 mo_streams-1.620.24125/mo_streams/byte_stream.py
--rw-rw-rw-   0        0        0     1158 2023-04-02 14:04:44.000000 mo_streams-1.620.24125/mo_streams/empty_stream.py
--rw-rw-rw-   0        0        0     1758 2024-02-15 02:58:09.000000 mo_streams-1.620.24125/mo_streams/files.py
--rw-rw-rw-   0        0        0    17030 2024-02-15 02:58:09.000000 mo_streams-1.620.24125/mo_streams/function_factory.py
--rw-rw-rw-   0        0        0    11348 2024-02-15 02:58:09.000000 mo_streams-1.620.24125/mo_streams/object_stream.py
--rw-rw-rw-   0        0        0     2300 2024-01-07 22:29:04.000000 mo_streams-1.620.24125/mo_streams/string_stream.py
--rw-rw-rw-   0        0        0      881 2023-04-02 14:04:44.000000 mo_streams-1.620.24125/mo_streams/type_parser.py
--rw-rw-rw-   0        0        0     7911 2024-02-15 02:58:09.000000 mo_streams-1.620.24125/mo_streams/type_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-04 18:00:13.348944 mo_streams-1.620.24125/mo_streams.egg-info/
--rw-rw-rw-   0        0        0     4418 2024-05-04 18:00:13.000000 mo_streams-1.620.24125/mo_streams.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      483 2024-05-04 18:00:13.000000 mo_streams-1.620.24125/mo_streams.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 18:00:13.000000 mo_streams-1.620.24125/mo_streams.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-21 02:42:10.000000 mo_streams-1.620.24125/mo_streams.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      248 2024-05-04 18:00:13.000000 mo_streams-1.620.24125/mo_streams.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-04 18:00:13.000000 mo_streams-1.620.24125/mo_streams.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 18:00:13.354850 mo_streams-1.620.24125/setup.cfg
--rw-rw-rw-   0        0        0     4211 2024-05-04 18:00:02.000000 mo_streams-1.620.24125/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:19:34.244331 mo_streams-1.624.24125/
+-rw-rw-rw-   0        0        0    17098 2022-11-20 01:40:59.000000 mo_streams-1.624.24125/LICENSE
+-rw-rw-rw-   0        0        0     4418 2024-05-04 20:19:34.244331 mo_streams-1.624.24125/PKG-INFO
+-rw-rw-rw-   0        0        0     2878 2024-03-02 21:57:33.000000 mo_streams-1.624.24125/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 20:19:34.233092 mo_streams-1.624.24125/mo_streams/
+-rw-rw-rw-   0        0        0     5332 2024-05-04 18:03:55.000000 mo_streams-1.624.24125/mo_streams/__init__.py
+-rw-rw-rw-   0        0        0     3617 2023-10-31 01:14:42.000000 mo_streams-1.624.24125/mo_streams/_utils.py
+-rw-rw-rw-   0        0        0     3867 2023-11-15 00:25:37.000000 mo_streams-1.624.24125/mo_streams/byte_stream.py
+-rw-rw-rw-   0        0        0     1158 2023-04-02 14:04:44.000000 mo_streams-1.624.24125/mo_streams/empty_stream.py
+-rw-rw-rw-   0        0        0     1758 2024-02-15 02:58:09.000000 mo_streams-1.624.24125/mo_streams/files.py
+-rw-rw-rw-   0        0        0    17030 2024-02-15 02:58:09.000000 mo_streams-1.624.24125/mo_streams/function_factory.py
+-rw-rw-rw-   0        0        0    11348 2024-02-15 02:58:09.000000 mo_streams-1.624.24125/mo_streams/object_stream.py
+-rw-rw-rw-   0        0        0     2300 2024-01-07 22:29:04.000000 mo_streams-1.624.24125/mo_streams/string_stream.py
+-rw-rw-rw-   0        0        0      881 2023-04-02 14:04:44.000000 mo_streams-1.624.24125/mo_streams/type_parser.py
+-rw-rw-rw-   0        0        0     7911 2024-02-15 02:58:09.000000 mo_streams-1.624.24125/mo_streams/type_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:19:34.242322 mo_streams-1.624.24125/mo_streams.egg-info/
+-rw-rw-rw-   0        0        0     4418 2024-05-04 20:19:34.000000 mo_streams-1.624.24125/mo_streams.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      483 2024-05-04 20:19:34.000000 mo_streams-1.624.24125/mo_streams.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 20:19:34.000000 mo_streams-1.624.24125/mo_streams.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-03-21 02:42:10.000000 mo_streams-1.624.24125/mo_streams.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      248 2024-05-04 20:19:34.000000 mo_streams-1.624.24125/mo_streams.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-04 20:19:34.000000 mo_streams-1.624.24125/mo_streams.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 20:19:34.245331 mo_streams-1.624.24125/setup.cfg
+-rw-rw-rw-   0        0        0     4211 2024-05-04 20:19:29.000000 mo_streams-1.624.24125/setup.py
```

### Comparing `mo_streams-1.620.24125/LICENSE` & `mo_streams-1.624.24125/LICENSE`

 * *Files identical despite different names*

### Comparing `mo_streams-1.620.24125/PKG-INFO` & `mo_streams-1.624.24125/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-streams
-Version: 1.620.24125
+Version: 1.624.24125
 Summary: More Streams! Chained function calls
 Home-page: https://github.com/klahnakoski/mo-streams
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development :: Libraries
@@ -13,28 +13,28 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots==10.615.24125
-Requires-Dist: mo-files==6.619.24125
+Requires-Dist: mo-dots==10.623.24125
+Requires-Dist: mo-files==6.624.24125
 Requires-Dist: mo-future==7.584.24095
-Requires-Dist: mo-json==6.619.24125
+Requires-Dist: mo-json==6.624.24125
 Provides-Extra: tests
-Requires-Dist: mo-files>=6.589.24111; extra == "tests"
-Requires-Dist: mo-logs>=8.584.24095; extra == "tests"
+Requires-Dist: mo-files>=6.609.24119; extra == "tests"
+Requires-Dist: mo-logs>=8.608.24119; extra == "tests"
 Requires-Dist: zstandard>=0.22.0; extra == "tests"
-Requires-Dist: boto3>=1.34.91; extra == "tests"
+Requires-Dist: boto3>=1.34.98; extra == "tests"
 Requires-Dist: moto>=4.2.14; extra == "tests"
 Requires-Dist: pandas>=2.0.3; extra == "tests"
-Requires-Dist: mo-threads>=6.589.24111; extra == "tests"
-Requires-Dist: mo-testing>=8.591.24112; extra == "tests"
-Requires-Dist: mo-threads>=6.589.24111; extra == "tests"
+Requires-Dist: mo-threads>=6.610.24119; extra == "tests"
+Requires-Dist: mo-testing>=8.610.24119; extra == "tests"
+Requires-Dist: mo-threads>=6.610.24119; extra == "tests"
 
 # More Streams!!
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/mo-streams.svg)](https://pypi.org/project/mo-streams/)
  [![Build Status](https://github.com/klahnakoski/mo-streams/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-streams/actions/workflows/build.yml)
  [![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-streams/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-streams?branch=dev)
 [![Downloads](https://pepy.tech/badge/mo-streams/month)](https://pepy.tech/project/mo-streams)
```

### Comparing `mo_streams-1.620.24125/README.md` & `mo_streams-1.624.24125/README.md`

 * *Files identical despite different names*

### Comparing `mo_streams-1.620.24125/mo_streams/__init__.py` & `mo_streams-1.624.24125/mo_streams/__init__.py`

 * *Files identical despite different names*

### Comparing `mo_streams-1.620.24125/mo_streams/_utils.py` & `mo_streams-1.624.24125/mo_streams/_utils.py`

 * *Files identical despite different names*

### Comparing `mo_streams-1.620.24125/mo_streams/byte_stream.py` & `mo_streams-1.624.24125/mo_streams/byte_stream.py`

 * *Files identical despite different names*

### Comparing `mo_streams-1.620.24125/mo_streams/empty_stream.py` & `mo_streams-1.624.24125/mo_streams/empty_stream.py`

 * *Files identical despite different names*

### Comparing `mo_streams-1.620.24125/mo_streams/files.py` & `mo_streams-1.624.24125/mo_streams/files.py`

 * *Files identical despite different names*

### Comparing `mo_streams-1.620.24125/mo_streams/function_factory.py` & `mo_streams-1.624.24125/mo_streams/function_factory.py`

 * *Files identical despite different names*

### Comparing `mo_streams-1.620.24125/mo_streams/object_stream.py` & `mo_streams-1.624.24125/mo_streams/object_stream.py`

 * *Files identical despite different names*

### Comparing `mo_streams-1.620.24125/mo_streams/string_stream.py` & `mo_streams-1.624.24125/mo_streams/string_stream.py`

 * *Files identical despite different names*

### Comparing `mo_streams-1.620.24125/mo_streams/type_parser.py` & `mo_streams-1.624.24125/mo_streams/type_parser.py`

 * *Files identical despite different names*

### Comparing `mo_streams-1.620.24125/mo_streams/type_utils.py` & `mo_streams-1.624.24125/mo_streams/type_utils.py`

 * *Files identical despite different names*

### Comparing `mo_streams-1.620.24125/mo_streams.egg-info/PKG-INFO` & `mo_streams-1.624.24125/mo_streams.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-streams
-Version: 1.620.24125
+Version: 1.624.24125
 Summary: More Streams! Chained function calls
 Home-page: https://github.com/klahnakoski/mo-streams
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development :: Libraries
@@ -13,28 +13,28 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots==10.615.24125
-Requires-Dist: mo-files==6.619.24125
+Requires-Dist: mo-dots==10.623.24125
+Requires-Dist: mo-files==6.624.24125
 Requires-Dist: mo-future==7.584.24095
-Requires-Dist: mo-json==6.619.24125
+Requires-Dist: mo-json==6.624.24125
 Provides-Extra: tests
-Requires-Dist: mo-files>=6.589.24111; extra == "tests"
-Requires-Dist: mo-logs>=8.584.24095; extra == "tests"
+Requires-Dist: mo-files>=6.609.24119; extra == "tests"
+Requires-Dist: mo-logs>=8.608.24119; extra == "tests"
 Requires-Dist: zstandard>=0.22.0; extra == "tests"
-Requires-Dist: boto3>=1.34.91; extra == "tests"
+Requires-Dist: boto3>=1.34.98; extra == "tests"
 Requires-Dist: moto>=4.2.14; extra == "tests"
 Requires-Dist: pandas>=2.0.3; extra == "tests"
-Requires-Dist: mo-threads>=6.589.24111; extra == "tests"
-Requires-Dist: mo-testing>=8.591.24112; extra == "tests"
-Requires-Dist: mo-threads>=6.589.24111; extra == "tests"
+Requires-Dist: mo-threads>=6.610.24119; extra == "tests"
+Requires-Dist: mo-testing>=8.610.24119; extra == "tests"
+Requires-Dist: mo-threads>=6.610.24119; extra == "tests"
 
 # More Streams!!
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/mo-streams.svg)](https://pypi.org/project/mo-streams/)
  [![Build Status](https://github.com/klahnakoski/mo-streams/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-streams/actions/workflows/build.yml)
  [![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-streams/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-streams?branch=dev)
 [![Downloads](https://pepy.tech/badge/mo-streams/month)](https://pepy.tech/project/mo-streams)
```

### Comparing `mo_streams-1.620.24125/setup.py` & `mo_streams-1.624.24125/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 # THIS FILE IS AUTOGENERATED!
 from setuptools import setup
 setup(
     author='Kyle Lahnakoski',
     author_email='kyle@lahnakoski.com',
     classifiers=["Development Status :: 3 - Alpha","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules","License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)","Programming Language :: Python :: 3.8","Programming Language :: Python :: 3.9","Programming Language :: Python :: 3.10","Programming Language :: Python :: 3.11","Programming Language :: Python :: 3.12"],
     description='More Streams! Chained function calls',
-    extras_require={"tests":["mo-files>=6.589.24111","mo-logs>=8.584.24095","zstandard>=0.22.0","boto3>=1.34.91","moto>=4.2.14","pandas>=2.0.3","mo-threads>=6.589.24111","mo-testing>=8.591.24112","mo-threads>=6.589.24111"]},
+    extras_require={"tests":["mo-files>=6.609.24119","mo-logs>=8.608.24119","zstandard>=0.22.0","boto3>=1.34.98","moto>=4.2.14","pandas>=2.0.3","mo-threads>=6.610.24119","mo-testing>=8.610.24119","mo-threads>=6.610.24119"]},
     include_package_data=True,
-    install_requires=["mo-dots==10.615.24125","mo-files==6.619.24125","mo-future==7.584.24095","mo-json==6.619.24125"],
+    install_requires=["mo-dots==10.623.24125","mo-files==6.624.24125","mo-future==7.584.24095","mo-json==6.624.24125"],
     license='MPL 2.0',
     long_description='# More Streams!!\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-streams.svg)](https://pypi.org/project/mo-streams/)\n [![Build Status](https://github.com/klahnakoski/mo-streams/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-streams/actions/workflows/build.yml)\n [![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-streams/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-streams?branch=dev)\n[![Downloads](https://pepy.tech/badge/mo-streams/month)](https://pepy.tech/project/mo-streams)\n\n\nPython code is more elegant with method chaining!\n\n\n## Overview\n\nThere are two families of "streams" in this library, both are lazy:\n\n1. `ByteStream` - a traditional stream of bytes intended to pipe bytes through various byte transformers, like compression, encoding and encyrption.  \n2. `ObjectStream`: An iterator/generator with a number of useful methods.\n\n### Example\n\nIn this case I am iterating through all files in a tar and parsing them:\n\n    results = (\n        File("tests/so_queries/so_queries.tar.zst")\n        .content()\n        .content()\n        .exists()\n        .utf8()\n        .to_str()\n        .map(parse)\n        .to_list()\n    )\n    \n Each of the steps constructs a generator, and no work is done until the last step\n \n \n * `File().content()` - will unzst and untar the file content to an `ObjectStream` of file-like objects.  It is short form for `stream(File().read_bytes()).from_zst().from_tar()`\n * The second `.content()` is applied to each of the file-like objects, returning `ByteStream` of the content for each\n * `.exists()` - some of the files (aka directories) in the tar file do not have content, we only include content that exists.\n * `.utf8` - convert to a `StringStream`\n * `.to_str` - convert to a Python `str`, we trust the content is not too large\n * `.map(parse)` - run the parser on each string\n * `.to_list()` - a "terminator", which executes the chain and returns a Python `list` with the results\n \n## Project Status\n\nAlive and in use, but \n\n* basic functions missing\n* inefficient - written using generators\n* generators not properly closed\n\n\n## Optional Reading\n\nThe method chaining style has two distinct benefits\n\n* functions are in the order they are applied \n* intermediate values need no temporary variables\n\nThe detriments are the same that we find in any declarative language: Incorrect code can be difficult to debug because you can not step through it to isolate the problem.  For this reason, the majority of the code in this library is dedicated to validating the links in the function chain before they are run.\n\n### Lessons\n\nThe function chaining style, called "streams" in Java or "linq" in C#, leans heavly on the strict typed nature of those langauges.  This is missing in Python, but type annotations help support this style of programming.\n\n',
     long_description_content_type='text/markdown',
     name='mo-streams',
     packages=["mo_streams"],
     url='https://github.com/klahnakoski/mo-streams',
-    version='1.620.24125',
+    version='1.624.24125',
     zip_safe=False
 )
```

