# Comparing `tmp/mo_collections-5.608.24119.tar.gz` & `tmp/mo_collections-5.623.24125.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo_collections-5.608.24119.tar", last modified: Sun Apr 28 20:24:33 2024, max compression
+gzip compressed data, was "mo_collections-5.623.24125.tar", last modified: Sat May  4 19:56:33 2024, max compression
```

## Comparing `mo_collections-5.608.24119.tar` & `mo_collections-5.623.24125.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 20:24:33.424678 mo_collections-5.608.24119/
--rw-rw-rw-   0        0        0    16725 2019-09-12 20:44:42.000000 mo_collections-5.608.24119/LICENSE
--rw-rw-rw-   0        0        0     1908 2024-04-28 20:24:33.421668 mo_collections-5.608.24119/PKG-INFO
--rw-rw-rw-   0        0        0      844 2024-03-10 19:12:26.000000 mo_collections-5.608.24119/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 20:24:33.405826 mo_collections-5.608.24119/mo_collections/
--rw-rw-rw-   0        0        0     1110 2023-05-30 00:24:58.000000 mo_collections-5.608.24119/mo_collections/__init__.py
--rw-rw-rw-   0        0        0     5399 2023-05-30 00:24:58.000000 mo_collections-5.608.24119/mo_collections/array.py
--rw-rw-rw-   0        0        0     4453 2023-05-30 00:24:58.000000 mo_collections-5.608.24119/mo_collections/index.py
--rw-rw-rw-   0        0        0    11472 2024-02-15 02:40:43.000000 mo_collections-5.608.24119/mo_collections/matrix.py
--rw-rw-rw-   0        0        0     5639 2023-05-30 00:24:58.000000 mo_collections-5.608.24119/mo_collections/multiset.py
--rw-rw-rw-   0        0        0     7493 2023-08-29 02:53:00.000000 mo_collections-5.608.24119/mo_collections/persistent_queue.py
--rw-rw-rw-   0        0        0     2215 2024-04-23 00:07:44.000000 mo_collections-5.608.24119/mo_collections/queue.py
--rw-rw-rw-   0        0        0     2700 2023-05-30 00:24:59.000000 mo_collections-5.608.24119/mo_collections/relation.py
--rw-rw-rw-   0        0        0     5389 2024-01-28 14:42:31.000000 mo_collections-5.608.24119/mo_collections/unique_index.py
-drwxrwxrwx   0        0        0        0 2024-04-28 20:24:33.421668 mo_collections-5.608.24119/mo_collections.egg-info/
--rw-rw-rw-   0        0        0     1908 2024-04-28 20:24:33.000000 mo_collections-5.608.24119/mo_collections.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2024-04-28 20:24:33.000000 mo_collections-5.608.24119/mo_collections.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 20:24:33.000000 mo_collections-5.608.24119/mo_collections.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      121 2024-04-28 20:24:33.000000 mo_collections-5.608.24119/mo_collections.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-28 20:24:33.000000 mo_collections-5.608.24119/mo_collections.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 20:24:33.424678 mo_collections-5.608.24119/setup.cfg
--rw-rw-rw-   0        0        0     1950 2024-04-28 20:24:27.000000 mo_collections-5.608.24119/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 19:56:33.861480 mo_collections-5.623.24125/
+-rw-rw-rw-   0        0        0    16725 2019-09-12 20:44:42.000000 mo_collections-5.623.24125/LICENSE
+-rw-rw-rw-   0        0        0     1909 2024-05-04 19:56:33.860405 mo_collections-5.623.24125/PKG-INFO
+-rw-rw-rw-   0        0        0      844 2024-03-10 19:12:26.000000 mo_collections-5.623.24125/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 19:56:33.848848 mo_collections-5.623.24125/mo_collections/
+-rw-rw-rw-   0        0        0     1110 2023-05-30 00:24:58.000000 mo_collections-5.623.24125/mo_collections/__init__.py
+-rw-rw-rw-   0        0        0     5399 2023-05-30 00:24:58.000000 mo_collections-5.623.24125/mo_collections/array.py
+-rw-rw-rw-   0        0        0     4453 2023-05-30 00:24:58.000000 mo_collections-5.623.24125/mo_collections/index.py
+-rw-rw-rw-   0        0        0    11472 2024-02-15 02:40:43.000000 mo_collections-5.623.24125/mo_collections/matrix.py
+-rw-rw-rw-   0        0        0     5639 2023-05-30 00:24:58.000000 mo_collections-5.623.24125/mo_collections/multiset.py
+-rw-rw-rw-   0        0        0     7493 2023-08-29 02:53:00.000000 mo_collections-5.623.24125/mo_collections/persistent_queue.py
+-rw-rw-rw-   0        0        0     2217 2024-05-04 19:56:26.000000 mo_collections-5.623.24125/mo_collections/queue.py
+-rw-rw-rw-   0        0        0     2700 2023-05-30 00:24:59.000000 mo_collections-5.623.24125/mo_collections/relation.py
+-rw-rw-rw-   0        0        0     5419 2024-05-04 19:56:26.000000 mo_collections-5.623.24125/mo_collections/unique_index.py
+drwxrwxrwx   0        0        0        0 2024-05-04 19:56:33.859402 mo_collections-5.623.24125/mo_collections.egg-info/
+-rw-rw-rw-   0        0        0     1909 2024-05-04 19:56:33.000000 mo_collections-5.623.24125/mo_collections.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2024-05-04 19:56:33.000000 mo_collections-5.623.24125/mo_collections.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 19:56:33.000000 mo_collections-5.623.24125/mo_collections.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2024-05-04 19:56:33.000000 mo_collections-5.623.24125/mo_collections.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-04 19:56:33.000000 mo_collections-5.623.24125/mo_collections.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 19:56:33.861480 mo_collections-5.623.24125/setup.cfg
+-rw-rw-rw-   0        0        0     1951 2024-05-04 19:56:29.000000 mo_collections-5.623.24125/setup.py
```

### Comparing `mo_collections-5.608.24119/LICENSE` & `mo_collections-5.623.24125/LICENSE`

 * *Files identical despite different names*

### Comparing `mo_collections-5.608.24119/PKG-INFO` & `mo_collections-5.623.24125/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-collections
-Version: 5.608.24119
+Version: 5.623.24125
 Summary: More Collections! Some useful data structures for dealing with Data
 Home-page: https://github.com/klahnakoski/mo-collections
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -12,18 +12,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots==9.606.24115
+Requires-Dist: mo-dots==10.623.24125
 Requires-Dist: mo-future==7.584.24095
-Requires-Dist: mo-kwargs==7.606.24115
-Requires-Dist: mo-logs==8.608.24119
+Requires-Dist: mo-kwargs==7.623.24125
+Requires-Dist: mo-logs==8.623.24125
 Provides-Extra: tests
 Requires-Dist: mo-testing>=8.591.24112; extra == "tests"
 
 # More Collections
 
 Some useful data structures for collections of data
```

### Comparing `mo_collections-5.608.24119/README.md` & `mo_collections-5.623.24125/README.md`

 * *Files identical despite different names*

### Comparing `mo_collections-5.608.24119/mo_collections/__init__.py` & `mo_collections-5.623.24125/mo_collections/__init__.py`

 * *Files identical despite different names*

### Comparing `mo_collections-5.608.24119/mo_collections/array.py` & `mo_collections-5.623.24125/mo_collections/array.py`

 * *Files identical despite different names*

### Comparing `mo_collections-5.608.24119/mo_collections/index.py` & `mo_collections-5.623.24125/mo_collections/index.py`

 * *Files identical despite different names*

### Comparing `mo_collections-5.608.24119/mo_collections/matrix.py` & `mo_collections-5.623.24125/mo_collections/matrix.py`

 * *Files identical despite different names*

### Comparing `mo_collections-5.608.24119/mo_collections/multiset.py` & `mo_collections-5.623.24125/mo_collections/multiset.py`

 * *Files identical despite different names*

### Comparing `mo_collections-5.608.24119/mo_collections/persistent_queue.py` & `mo_collections-5.623.24125/mo_collections/persistent_queue.py`

 * *Files identical despite different names*

### Comparing `mo_collections-5.608.24119/mo_collections/queue.py` & `mo_collections-5.623.24125/mo_collections/queue.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
 
 
 from collections import deque
 from copy import copy
-from mo_dots import register_many
+
+from mo_dots import register_list
 
 
 class Queue:
     """
     A SET WITH ADDED ORDER MAINTAINED
 
     +------------+---------+----------+
@@ -89,8 +90,8 @@
             return None
 
         output = self.list.popleft()
         self.set.remove(output)
         return output
 
 
-register_many(Queue)
+register_list(Queue)
```

### Comparing `mo_collections-5.608.24119/mo_collections/relation.py` & `mo_collections-5.623.24125/mo_collections/relation.py`

 * *Files identical despite different names*

### Comparing `mo_collections-5.608.24119/mo_collections/unique_index.py` & `mo_collections-5.623.24125/mo_collections/unique_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
-from mo_dots import is_data, is_sequence, tuplewrap, from_data, to_data, list_to_data
-from mo_future import iteritems, Set, Mapping, Iterable, first
+from mo_dots import is_data, is_sequence, tuplewrap, from_data, to_data, list_to_data, register_list
+from mo_future import Set, Mapping, Iterable, first
 from mo_logs import Log
 from mo_logs.exceptions import suppress_exception
 
 DEBUG = False
 
 
 class UniqueIndex(Set, Mapping):
@@ -62,15 +62,15 @@
         # except Exception as e:
         #     Log.error("something went wrong", e)
 
     def keys(self):
         return self._data.keys()
 
     def pop(self):
-        output = first(iteritems(self._data))[1]
+        output = first(self._data.items())[1]
         self.remove(output)
         return to_data(output)
 
     def add(self, val):
         val = to_data(val)
         key = value2key(self._keys, val)
         if key == None:
@@ -162,14 +162,17 @@
     def subtract(self, other):
         return self.__sub__(other)
 
     def intersect(self, other):
         return self.__and__(other)
 
 
+register_list(UniqueIndex)
+
+
 def value2key(keys, val):
     if len(keys) == 1:
         if is_data(val):
             return val[keys[0]]
         elif is_sequence(val):
             return val[0]
         else:
```

### Comparing `mo_collections-5.608.24119/mo_collections.egg-info/PKG-INFO` & `mo_collections-5.623.24125/mo_collections.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-collections
-Version: 5.608.24119
+Version: 5.623.24125
 Summary: More Collections! Some useful data structures for dealing with Data
 Home-page: https://github.com/klahnakoski/mo-collections
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -12,18 +12,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots==9.606.24115
+Requires-Dist: mo-dots==10.623.24125
 Requires-Dist: mo-future==7.584.24095
-Requires-Dist: mo-kwargs==7.606.24115
-Requires-Dist: mo-logs==8.608.24119
+Requires-Dist: mo-kwargs==7.623.24125
+Requires-Dist: mo-logs==8.623.24125
 Provides-Extra: tests
 Requires-Dist: mo-testing>=8.591.24112; extra == "tests"
 
 # More Collections
 
 Some useful data structures for collections of data
```

### Comparing `mo_collections-5.608.24119/setup.py` & `mo_collections-5.623.24125/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 setup(
     author='Kyle Lahnakoski',
     author_email='kyle@lahnakoski.com',
     classifiers=["Development Status :: 4 - Beta","License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)","Programming Language :: Python :: 3.8","Programming Language :: Python :: 3.9","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules","Programming Language :: Python :: 3.11","Programming Language :: Python :: 3.12"],
     description='More Collections! Some useful data structures for dealing with Data',
     extras_require={"tests":["mo-testing>=8.591.24112"]},
     include_package_data=True,
-    install_requires=["mo-dots==9.606.24115","mo-future==7.584.24095","mo-kwargs==7.606.24115","mo-logs==8.608.24119"],
+    install_requires=["mo-dots==10.623.24125","mo-future==7.584.24095","mo-kwargs==7.623.24125","mo-logs==8.623.24125"],
     license='MPL 2.0',
     long_description="# More Collections\n\nSome useful data structures for collections of data\n\n\n### Class `Index`\n\nProvide indexing for a list. Inner properties can be used for keys, and keys can be tuples of properties.  \n\n### Class `UniqueIndex`\n\nSame as Index, but includes checks and optimization to ensure members' keys are unique.\n\n### Class `Queue`\n\nA `Queue` is a list, with `add()` and `pop()`. It ensures members in the queue are not duplicated by not adding the ones already found in the queue.\n\n### Class `Matrix`\n\nA multidimensional grid of values that can be used like a `Mapping` from a-tuple-of-coordinates to the value at that coordinate. Plus a few other convenience methods.\n\nThis is a naive implementation. The hope it is a simple facade to a faster implementation.\n\n### Class `Relation`\n\nStore the many-to-many relations between two domains     ",
     long_description_content_type='text/markdown',
     name='mo-collections',
     packages=["mo_collections"],
     url='https://github.com/klahnakoski/mo-collections',
-    version='5.608.24119'
+    version='5.623.24125'
 )
```

