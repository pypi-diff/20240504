# Comparing `tmp/mo_testing-8.610.24119.tar.gz` & `tmp/mo_testing-8.623.24125.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo_testing-8.610.24119.tar", last modified: Sun Apr 28 22:45:15 2024, max compression
+gzip compressed data, was "mo_testing-8.623.24125.tar", last modified: Sat May  4 20:03:09 2024, max compression
```

## Comparing `mo_testing-8.610.24119.tar` & `mo_testing-8.623.24125.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 22:45:15.696121 mo_testing-8.610.24119/
--rw-rw-rw-   0        0        0    16725 2019-11-12 20:39:14.000000 mo_testing-8.610.24119/LICENSE
--rw-rw-rw-   0        0        0     2881 2024-04-28 22:45:15.696065 mo_testing-8.610.24119/PKG-INFO
--rw-rw-rw-   0        0        0     1630 2024-04-21 13:20:38.000000 mo_testing-8.610.24119/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 22:45:15.686726 mo_testing-8.610.24119/mo_testing/
--rw-rw-rw-   0        0        0      493 2024-04-28 20:32:37.000000 mo_testing-8.610.24119/mo_testing/__init__.py
--rw-rw-rw-   0        0        0    11685 2024-04-28 20:32:37.000000 mo_testing-8.610.24119/mo_testing/fuzzytestcase.py
-drwxrwxrwx   0        0        0        0 2024-04-28 22:45:15.693650 mo_testing-8.610.24119/mo_testing.egg-info/
--rw-rw-rw-   0        0        0     2881 2024-04-28 22:45:15.000000 mo_testing-8.610.24119/mo_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-04-28 22:45:15.000000 mo_testing-8.610.24119/mo_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 22:45:15.000000 mo_testing-8.610.24119/mo_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      164 2024-04-28 22:45:15.000000 mo_testing-8.610.24119/mo_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-28 22:45:15.000000 mo_testing-8.610.24119/mo_testing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 22:45:15.696121 mo_testing-8.610.24119/setup.cfg
--rw-rw-rw-   0        0        0     2850 2024-04-28 22:45:10.000000 mo_testing-8.610.24119/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:03:09.910337 mo_testing-8.623.24125/
+-rw-rw-rw-   0        0        0    16725 2019-11-12 20:39:14.000000 mo_testing-8.623.24125/LICENSE
+-rw-rw-rw-   0        0        0     2882 2024-05-04 20:03:09.909275 mo_testing-8.623.24125/PKG-INFO
+-rw-rw-rw-   0        0        0     1630 2024-04-21 13:20:38.000000 mo_testing-8.623.24125/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 20:03:09.901396 mo_testing-8.623.24125/mo_testing/
+-rw-rw-rw-   0        0        0      493 2024-04-28 20:32:37.000000 mo_testing-8.623.24125/mo_testing/__init__.py
+-rw-rw-rw-   0        0        0    11685 2024-04-28 20:32:37.000000 mo_testing-8.623.24125/mo_testing/fuzzytestcase.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:03:09.908215 mo_testing-8.623.24125/mo_testing.egg-info/
+-rw-rw-rw-   0        0        0     2882 2024-05-04 20:03:09.000000 mo_testing-8.623.24125/mo_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-05-04 20:03:09.000000 mo_testing-8.623.24125/mo_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 20:03:09.000000 mo_testing-8.623.24125/mo_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      165 2024-05-04 20:03:09.000000 mo_testing-8.623.24125/mo_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-04 20:03:09.000000 mo_testing-8.623.24125/mo_testing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 20:03:09.910337 mo_testing-8.623.24125/setup.cfg
+-rw-rw-rw-   0        0        0     2851 2024-05-04 20:03:05.000000 mo_testing-8.623.24125/setup.py
```

### Comparing `mo_testing-8.610.24119/LICENSE` & `mo_testing-8.623.24125/LICENSE`

 * *Files identical despite different names*

### Comparing `mo_testing-8.610.24119/PKG-INFO` & `mo_testing-8.623.24125/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-testing
-Version: 8.610.24119
+Version: 8.623.24125
 Summary: More Testing! Extends the `unittest.TestCase` to provide deep, yet fuzzy, structural comparisons
 Home-page: https://github.com/klahnakoski/mo-testing
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
@@ -13,20 +13,20 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-collections==5.608.24119
-Requires-Dist: mo-dots==9.606.24115
+Requires-Dist: mo-collections==5.623.24125
+Requires-Dist: mo-dots==10.623.24125
 Requires-Dist: mo-future==7.584.24095
-Requires-Dist: mo-logs==8.608.24119
-Requires-Dist: mo-math==7.606.24115
-Requires-Dist: mo-threads==6.610.24119
+Requires-Dist: mo-logs==8.623.24125
+Requires-Dist: mo-math==7.623.24125
+Requires-Dist: mo-threads==6.623.24125
 Provides-Extra: tests
 Requires-Dist: mo_times; extra == "tests"
 Requires-Dist: mo_logs; extra == "tests"
 
 # More Testing
```

### Comparing `mo_testing-8.610.24119/README.md` & `mo_testing-8.623.24125/README.md`

 * *Files identical despite different names*

### Comparing `mo_testing-8.610.24119/mo_testing/fuzzytestcase.py` & `mo_testing-8.623.24125/mo_testing/fuzzytestcase.py`

 * *Files identical despite different names*

### Comparing `mo_testing-8.610.24119/mo_testing.egg-info/PKG-INFO` & `mo_testing-8.623.24125/mo_testing.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-testing
-Version: 8.610.24119
+Version: 8.623.24125
 Summary: More Testing! Extends the `unittest.TestCase` to provide deep, yet fuzzy, structural comparisons
 Home-page: https://github.com/klahnakoski/mo-testing
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
@@ -13,20 +13,20 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-collections==5.608.24119
-Requires-Dist: mo-dots==9.606.24115
+Requires-Dist: mo-collections==5.623.24125
+Requires-Dist: mo-dots==10.623.24125
 Requires-Dist: mo-future==7.584.24095
-Requires-Dist: mo-logs==8.608.24119
-Requires-Dist: mo-math==7.606.24115
-Requires-Dist: mo-threads==6.610.24119
+Requires-Dist: mo-logs==8.623.24125
+Requires-Dist: mo-math==7.623.24125
+Requires-Dist: mo-threads==6.623.24125
 Provides-Extra: tests
 Requires-Dist: mo_times; extra == "tests"
 Requires-Dist: mo_logs; extra == "tests"
 
 # More Testing
```

### Comparing `mo_testing-8.610.24119/setup.py` & `mo_testing-8.623.24125/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 setup(
     author='Kyle Lahnakoski',
     author_email='kyle@lahnakoski.com',
     classifiers=["Development Status :: 4 - Beta","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules","License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)","Programming Language :: Python :: 3.8","Programming Language :: Python :: 3.9","Programming Language :: Python :: 3.10","Programming Language :: Python :: 3.11","Programming Language :: Python :: 3.12"],
     description='More Testing! Extends the `unittest.TestCase` to provide deep, yet fuzzy, structural comparisons',
     extras_require={"tests":["mo_times","mo_logs"]},
     include_package_data=True,
-    install_requires=["mo-collections==5.608.24119","mo-dots==9.606.24115","mo-future==7.584.24095","mo-logs==8.608.24119","mo-math==7.606.24115","mo-threads==6.610.24119"],
+    install_requires=["mo-collections==5.623.24125","mo-dots==10.623.24125","mo-future==7.584.24095","mo-logs==8.623.24125","mo-math==7.623.24125","mo-threads==6.623.24125"],
     license='MPL 2.0',
     long_description='# More Testing\n\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-testing.svg)](https://pypi.org/project/mo-testing/)\n[![Build Status](https://github.com/klahnakoski/mo-testing/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-testing/actions/workflows/build.yml)\n[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-testing/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-testing?branch=dev)\n[![Downloads](https://pepy.tech/badge/mo-testing/month)](https://pepy.tech/project/mo-testing)\n\n\n`FuzzyTestCase` extends the `unittest.TestCase` to provide deep, yet fuzzy, structural comparisons; intended for use in test cases dealing with JSON.\n\n\n## Details\n\nThe primary method is the `assertAlmostEqual` method with the following arguments:\n\n* `test_value` - the value, or structure being tested\n* `expected` - the expected value or structure.  In the case of a number, the accuracy is controlled by the following parameters.  In the case of a structure, only the not-null parameters of `expected` are tested for existence.\n* `msg` - Detailed error message if there is no match\n\nKeyword arguments:\n* `digits` - number of decimal places of accuracy required to consider two values equal\n* `places` - number of significant digits used to compare values for accuracy\n* `delta` - maximum difference between values for them to be equal\n\nThis method `assertEqual` is recursive; it does a deep comparison; it can not handle cycles in the data structure.\n\n## Major Changes\n\n### Version 8\n\n* `digits`, `places`, and `delta` must be specified as keyword arguments\n',
     long_description_content_type='text/markdown',
     name='mo-testing',
     packages=["mo_testing"],
     url='https://github.com/klahnakoski/mo-testing',
-    version='8.610.24119'
+    version='8.623.24125'
 )
```

