# Comparing `tmp/mo_times-5.609.24119.tar.gz` & `tmp/mo_times-5.617.24125.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo_times-5.609.24119.tar", last modified: Sun Apr 28 22:27:05 2024, max compression
+gzip compressed data, was "mo_times-5.617.24125.tar", last modified: Sat May  4 15:59:54 2024, max compression
```

## Comparing `mo_times-5.609.24119.tar` & `mo_times-5.617.24125.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 22:27:05.364520 mo_times-5.609.24119/
--rw-rw-rw-   0        0        0    16725 2019-09-12 20:49:14.000000 mo_times-5.609.24119/LICENSE
--rw-rw-rw-   0        0        0     5813 2024-04-28 22:27:05.363512 mo_times-5.609.24119/PKG-INFO
--rw-rw-rw-   0        0        0     4520 2024-03-02 21:24:19.000000 mo_times-5.609.24119/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 22:27:05.355366 mo_times-5.609.24119/mo_times/
--rw-rw-rw-   0        0        0      442 2023-11-12 15:00:31.000000 mo_times-5.609.24119/mo_times/__init__.py
--rw-rw-rw-   0        0        0    17226 2024-04-28 22:26:58.000000 mo_times-5.609.24119/mo_times/dates.py
--rw-rw-rw-   0        0        0    11814 2024-04-23 00:09:34.000000 mo_times-5.609.24119/mo_times/durations.py
--rw-rw-rw-   0        0        0     2737 2024-02-03 17:42:09.000000 mo_times-5.609.24119/mo_times/timer.py
-drwxrwxrwx   0        0        0        0 2024-04-28 22:27:05.362453 mo_times-5.609.24119/mo_times.egg-info/
--rw-rw-rw-   0        0        0     5813 2024-04-28 22:27:05.000000 mo_times-5.609.24119/mo_times.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2024-04-28 22:27:05.000000 mo_times-5.609.24119/mo_times.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 22:27:05.000000 mo_times-5.609.24119/mo_times.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      164 2024-04-28 22:27:05.000000 mo_times-5.609.24119/mo_times.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-28 22:27:05.000000 mo_times-5.609.24119/mo_times.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 22:27:05.364520 mo_times-5.609.24119/setup.cfg
--rw-rw-rw-   0        0        0     5777 2024-04-28 22:27:00.000000 mo_times-5.609.24119/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 15:59:54.325731 mo_times-5.617.24125/
+-rw-rw-rw-   0        0        0    16725 2019-09-12 20:49:14.000000 mo_times-5.617.24125/LICENSE
+-rw-rw-rw-   0        0        0     5814 2024-05-04 15:59:54.324454 mo_times-5.617.24125/PKG-INFO
+-rw-rw-rw-   0        0        0     4520 2024-03-02 21:24:19.000000 mo_times-5.617.24125/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 15:59:54.312301 mo_times-5.617.24125/mo_times/
+-rw-rw-rw-   0        0        0      442 2023-11-12 15:00:31.000000 mo_times-5.617.24125/mo_times/__init__.py
+-rw-rw-rw-   0        0        0    17226 2024-04-28 22:26:58.000000 mo_times-5.617.24125/mo_times/dates.py
+-rw-rw-rw-   0        0        0    11814 2024-04-23 00:09:34.000000 mo_times-5.617.24125/mo_times/durations.py
+-rw-rw-rw-   0        0        0     2737 2024-02-03 17:42:09.000000 mo_times-5.617.24125/mo_times/timer.py
+drwxrwxrwx   0        0        0        0 2024-05-04 15:59:54.322165 mo_times-5.617.24125/mo_times.egg-info/
+-rw-rw-rw-   0        0        0     5814 2024-05-04 15:59:54.000000 mo_times-5.617.24125/mo_times.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2024-05-04 15:59:54.000000 mo_times-5.617.24125/mo_times.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 15:59:54.000000 mo_times-5.617.24125/mo_times.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      165 2024-05-04 15:59:54.000000 mo_times-5.617.24125/mo_times.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-04 15:59:54.000000 mo_times-5.617.24125/mo_times.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 15:59:54.325731 mo_times-5.617.24125/setup.cfg
+-rw-rw-rw-   0        0        0     5778 2024-05-04 15:59:48.000000 mo_times-5.617.24125/setup.py
```

### Comparing `mo_times-5.609.24119/LICENSE` & `mo_times-5.617.24125/LICENSE`

 * *Files identical despite different names*

### Comparing `mo_times-5.609.24119/PKG-INFO` & `mo_times-5.617.24125/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-times
-Version: 5.609.24119
+Version: 5.617.24125
 Summary: More Time! Time as a vector space, the way it was meant to be.
 Home-page: https://github.com/klahnakoski/mo-times
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.9
@@ -13,22 +13,22 @@
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots==9.606.24115
+Requires-Dist: mo-dots==10.615.24125
 Requires-Dist: mo-future==7.584.24095
-Requires-Dist: mo-logs==8.608.24119
-Requires-Dist: mo-math==7.606.24115
+Requires-Dist: mo-logs==8.617.24125
+Requires-Dist: mo-math==7.616.24125
 Provides-Extra: tests
-Requires-Dist: mo-testing>=8.591.24112; extra == "tests"
-Requires-Dist: mo-math>=7.589.24111; extra == "tests"
-Requires-Dist: mo-threads>=6.589.24111; extra == "tests"
+Requires-Dist: mo-testing>=8.608.24119; extra == "tests"
+Requires-Dist: mo-math>=7.606.24115; extra == "tests"
+Requires-Dist: mo-threads>=6.608.24119; extra == "tests"
 
 # More Times!
 
 Assume time forms an algebraic field over GMT. Finally! 
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/mo-times.svg)](https://pypi.org/project/mo-times/)
  [![Build Status](https://github.com/klahnakoski/mo-times/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-times/actions/workflows/build.yml)
```

### Comparing `mo_times-5.609.24119/README.md` & `mo_times-5.617.24125/README.md`

 * *Files identical despite different names*

### Comparing `mo_times-5.609.24119/mo_times/dates.py` & `mo_times-5.617.24125/mo_times/dates.py`

 * *Files identical despite different names*

### Comparing `mo_times-5.609.24119/mo_times/durations.py` & `mo_times-5.617.24125/mo_times/durations.py`

 * *Files identical despite different names*

### Comparing `mo_times-5.609.24119/mo_times/timer.py` & `mo_times-5.617.24125/mo_times/timer.py`

 * *Files identical despite different names*

### Comparing `mo_times-5.609.24119/mo_times.egg-info/PKG-INFO` & `mo_times-5.617.24125/mo_times.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-times
-Version: 5.609.24119
+Version: 5.617.24125
 Summary: More Time! Time as a vector space, the way it was meant to be.
 Home-page: https://github.com/klahnakoski/mo-times
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.9
@@ -13,22 +13,22 @@
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots==9.606.24115
+Requires-Dist: mo-dots==10.615.24125
 Requires-Dist: mo-future==7.584.24095
-Requires-Dist: mo-logs==8.608.24119
-Requires-Dist: mo-math==7.606.24115
+Requires-Dist: mo-logs==8.617.24125
+Requires-Dist: mo-math==7.616.24125
 Provides-Extra: tests
-Requires-Dist: mo-testing>=8.591.24112; extra == "tests"
-Requires-Dist: mo-math>=7.589.24111; extra == "tests"
-Requires-Dist: mo-threads>=6.589.24111; extra == "tests"
+Requires-Dist: mo-testing>=8.608.24119; extra == "tests"
+Requires-Dist: mo-math>=7.606.24115; extra == "tests"
+Requires-Dist: mo-threads>=6.608.24119; extra == "tests"
 
 # More Times!
 
 Assume time forms an algebraic field over GMT. Finally! 
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/mo-times.svg)](https://pypi.org/project/mo-times/)
  [![Build Status](https://github.com/klahnakoski/mo-times/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-times/actions/workflows/build.yml)
```

### Comparing `mo_times-5.609.24119/setup.py` & `mo_times-5.617.24125/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 # THIS FILE IS AUTOGENERATED!
 from setuptools import setup
 setup(
     author='Kyle Lahnakoski',
     author_email='kyle@lahnakoski.com',
     classifiers=["Development Status :: 4 - Beta","Programming Language :: Python :: 3.9","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules","License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)","Programming Language :: Python :: 3.10","Programming Language :: Python :: 3.8","Programming Language :: Python :: 3.11","Programming Language :: Python :: 3.12"],
     description='More Time! Time as a vector space, the way it was meant to be.',
-    extras_require={"tests":["mo-testing>=8.591.24112","mo-math>=7.589.24111","mo-threads>=6.589.24111"]},
+    extras_require={"tests":["mo-testing>=8.608.24119","mo-math>=7.606.24115","mo-threads>=6.608.24119"]},
     include_package_data=True,
-    install_requires=["mo-dots==9.606.24115","mo-future==7.584.24095","mo-logs==8.608.24119","mo-math==7.606.24115"],
+    install_requires=["mo-dots==10.615.24125","mo-future==7.584.24095","mo-logs==8.617.24125","mo-math==7.616.24125"],
     license='MPL 2.0',
     long_description='# More Times!\n\nAssume time forms an algebraic field over GMT. Finally! \n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-times.svg)](https://pypi.org/project/mo-times/)\n [![Build Status](https://github.com/klahnakoski/mo-times/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-times/actions/workflows/build.yml)\n [![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-times/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-times?branch=dev)\n[![Downloads](https://pepy.tech/badge/mo-times)](https://pepy.tech/project/mo-times)\n\n\n## Details \n\n`Date` is a simplified class for time manipulation. This library is intended for personal and business applications where assuming every solar day has 24 * 60 * 60 seconds is considered accurate. [See *GMT vs UTC* below](//#GMT%20vs%20UTC).\n\n\n### Assumptions\n\n* **All time is in GMT** - Timezone math is left to be resolved at the human endpoints: Machines should only be dealing with one type of time; without holes, without overlap, and with minimal context.\n* **Single time type** - There is no distinction between dates, datetime and times; all measurements in the time dimension are handled by one type called `Date`. This is important for treating time as a vector space.\n* **Standard range comparision** - All time range comparisons have been standardized to `min <= value < max`. The minimum is inclusive (`<=`), and the maximum is exclusive (`<`). \n\n\n## `Date` class \n\nThe `Date()` method will convert unix timestamps, millisecond timestamps, various string formats and simple time formulas to create a GMT time\n\n### `Date.now()`\n\nReturn `Date` instance with millisecond resolution (in GMT).\n\n### `Date.eod()` \n\nReturn end-of-day: Smallest `Date` which is greater than all time points in today. Think of it as tomorrow. Same as `now().ceiling(DAY)`\n\n### `Date.today()`\n\nThe beginning of today. Same as `now().floor(DAY)`\n\n### Date.range(min, max, interval)\n\nReturn an explicit list of `Dates` starting with `min`, each `interval` more than the last, but now including `max`.   Used in defining partitions in time domains.\n\n### `floor(duration=None)`\n\nThis method is usually used to perform date comparisons at the given resolution (aka `duration`). Round down to the nearest whole duration. `duration` as assumed to be `DAY` if not provided.\n\n### `format(format="%Y-%m-%d %H:%M:%S")`\n\nJust like `strftime`\n\n### `milli`\n\nNumber of milliseconds since epoch\n\n### `unix`\n\nNumber of seconds since epoch\n\n\n### `add(duration)`\n\nAdd a `duration` to the time to get a new `Date` instance. The `self` is not modified.\n\n### `addDay()`\n\nConvenience method for `self.add(DAY)`\n\n\n## `Duration` class\n\nRepresents the difference between two `Dates`. There are two scales:\n\n*  **`DAY` scale** - includes seconds, minutes, hours, days and weeks.\n*  **`YEAR` scale** - includes months, quarters, years, and centuries.\n\n### `floor(interval=None)`\n\nRound down to nearest `interval` size.\n\n### `seconds` \n\nreturn total number of seconds (including partial) in this duration (estimate given for `YEAR` scale)\n\n### `total_seconds()`\n\nSame as the `seconds` property\n\n### `round(interval, decimal=0)`\n\nReturn number of given `interval` rounded to given `decimal` places\n\n### `format(interval, decimal=0)`\n\nReturn a string representing `self` using given `interval` and `decimal` rounding\n\n\n# Time as an algebraic field\n\nThe `Date` and `Duration` objects are the point and vectors in a one dimensional vector space. As such, the `+` and `-` operators are allowed. Comparisons with (`>`, `>=`, `<=`, `<`) are also supported.\n\n\n## GMT vs UTC\n\nThe solar day is he most popular timekeeping unit. This library chose GMT (UT1) for its base clock because of its consistent seconds in a solar day. UTC suffers from inconsistent leap seconds and makes time-math difficult, even while forcing us to make pedantic conclusions like some minutes do not have 60 seconds. Lucky for us Python\'s implementation of UTC (`datetime.utcnow()`) is wrong, and implements GMT: Which is what we use.\n\n## Error Analysis\n\nAssuming we need a generous leap second each 6 months (the past decade saw only 4 leap seconds), then GMT deviates from UTC by up to 1 seconds over 181 days (December to June, 15,638,400 seconds) which is an error rate `error = 1/15,638,400 = 0.000006395%`. If we want to call the error "noise", we have a 70dB signal/noise ratio. All applications that can tolerate this level of error should use GMT as their time basis.\n\n\n',
     long_description_content_type='text/markdown',
     name='mo-times',
     packages=["mo_times"],
     url='https://github.com/klahnakoski/mo-times',
-    version='5.609.24119'
+    version='5.617.24125'
 )
```

