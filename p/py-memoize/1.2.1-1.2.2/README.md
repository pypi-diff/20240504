# Comparing `tmp/py-memoize-1.2.1.tar.gz` & `tmp/py-memoize-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-memoize-1.2.1.tar", last modified: Sat May  4 07:14:12 2024, max compression
+gzip compressed data, was "py-memoize-1.2.2.tar", last modified: Sat May  4 16:28:16 2024, max compression
```

## Comparing `py-memoize-1.2.1.tar` & `py-memoize-1.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:14:12.755412 py-memoize-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-04 07:14:03.000000 py-memoize-1.2.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-04 07:14:03.000000 py-memoize-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    18899 2024-05-04 07:14:12.755412 py-memoize-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17881 2024-05-04 07:14:03.000000 py-memoize-1.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:14:12.751412 py-memoize-1.2.1/memoize/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-04 07:14:03.000000 py-memoize-1.2.1/memoize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-05-04 07:14:03.000000 py-memoize-1.2.1/memoize/coerced.py
--rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-05-04 07:14:03.000000 py-memoize-1.2.1/memoize/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-04 07:14:03.000000 py-memoize-1.2.1/memoize/entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-04 07:14:03.000000 py-memoize-1.2.1/memoize/entrybuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-04 07:14:03.000000 py-memoize-1.2.1/memoize/eviction.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-04 07:14:03.000000 py-memoize-1.2.1/memoize/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-04 07:14:03.000000 py-memoize-1.2.1/memoize/invalidation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-04 07:14:03.000000 py-memoize-1.2.1/memoize/key.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-04 07:14:03.000000 py-memoize-1.2.1/memoize/memoize_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-04 07:14:03.000000 py-memoize-1.2.1/memoize/serde.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-04 07:14:03.000000 py-memoize-1.2.1/memoize/statuses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-04 07:14:03.000000 py-memoize-1.2.1/memoize/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-05-04 07:14:03.000000 py-memoize-1.2.1/memoize/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:14:12.755412 py-memoize-1.2.1/py_memoize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18899 2024-05-04 07:14:12.000000 py-memoize-1.2.1/py_memoize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-04 07:14:12.000000 py-memoize-1.2.1/py_memoize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 07:14:12.000000 py-memoize-1.2.1/py_memoize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-04 07:14:12.000000 py-memoize-1.2.1/py_memoize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 07:14:12.000000 py-memoize-1.2.1/py_memoize.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 07:14:12.755412 py-memoize-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-04 07:14:03.000000 py-memoize-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:28:16.101258 py-memoize-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-04 16:28:03.000000 py-memoize-1.2.2/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-04 16:28:03.000000 py-memoize-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18917 2024-05-04 16:28:16.101258 py-memoize-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17899 2024-05-04 16:28:03.000000 py-memoize-1.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:28:16.097259 py-memoize-1.2.2/memoize/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-04 16:28:03.000000 py-memoize-1.2.2/memoize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-05-04 16:28:03.000000 py-memoize-1.2.2/memoize/coerced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-05-04 16:28:03.000000 py-memoize-1.2.2/memoize/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-04 16:28:03.000000 py-memoize-1.2.2/memoize/entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-04 16:28:03.000000 py-memoize-1.2.2/memoize/entrybuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-04 16:28:03.000000 py-memoize-1.2.2/memoize/eviction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-04 16:28:03.000000 py-memoize-1.2.2/memoize/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-04 16:28:03.000000 py-memoize-1.2.2/memoize/invalidation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-04 16:28:03.000000 py-memoize-1.2.2/memoize/key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-04 16:28:03.000000 py-memoize-1.2.2/memoize/memoize_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-04 16:28:03.000000 py-memoize-1.2.2/memoize/serde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-04 16:28:03.000000 py-memoize-1.2.2/memoize/statuses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-04 16:28:03.000000 py-memoize-1.2.2/memoize/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-05-04 16:28:03.000000 py-memoize-1.2.2/memoize/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:28:16.101258 py-memoize-1.2.2/py_memoize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18917 2024-05-04 16:28:16.000000 py-memoize-1.2.2/py_memoize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-04 16:28:16.000000 py-memoize-1.2.2/py_memoize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 16:28:16.000000 py-memoize-1.2.2/py_memoize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-04 16:28:16.000000 py-memoize-1.2.2/py_memoize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 16:28:16.000000 py-memoize-1.2.2/py_memoize.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 16:28:16.101258 py-memoize-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-04 16:28:03.000000 py-memoize-1.2.2/setup.py
```

### Comparing `py-memoize-1.2.1/LICENCE` & `py-memoize-1.2.2/LICENCE`

 * *Files identical despite different names*

### Comparing `py-memoize-1.2.1/PKG-INFO` & `py-memoize-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-memoize
-Version: 1.2.1
+Version: 1.2.2
 Summary: Caching library for asynchronous Python applications (both based on asyncio and Tornado) that handles dogpiling properly and provides a configurable & extensible API.
 Home-page: https://github.com/DreamLab/memoize
 Author: Michal Zmuda
 Author-email: zmu.michal@gmail.com
 Maintainer: DreamLab
 License: Apache License 2.0
 Keywords: python cache tornado asyncio
@@ -483,15 +483,15 @@
     class ValueWithTTL:
         value: str
         ttl_seconds: int  # for instance, it could be derived from Cache-Control response header
 
 
     class TtlRespectingCacheEntryBuilder(CacheEntryBuilder):
         def build(self, key: CacheKey, value: ValueWithTTL):
-            now = datetime.datetime.utcnow()
+            now = datetime.datetime.now(datetime.timezone.utc)
             ttl_ends_at = now + datetime.timedelta(seconds=value.ttl_seconds)
             return CacheEntry(
                 created=now,
                 update_after=ttl_ends_at,
                 # allowing stale data for 10% of TTL
                 expires_after=ttl_ends_at + datetime.timedelta(seconds=value.ttl_seconds // 10),
                 value=value
```

### Comparing `py-memoize-1.2.1/README.rst` & `py-memoize-1.2.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -456,15 +456,15 @@
     class ValueWithTTL:
         value: str
         ttl_seconds: int  # for instance, it could be derived from Cache-Control response header
 
 
     class TtlRespectingCacheEntryBuilder(CacheEntryBuilder):
         def build(self, key: CacheKey, value: ValueWithTTL):
-            now = datetime.datetime.utcnow()
+            now = datetime.datetime.now(datetime.timezone.utc)
             ttl_ends_at = now + datetime.timedelta(seconds=value.ttl_seconds)
             return CacheEntry(
                 created=now,
                 update_after=ttl_ends_at,
                 # allowing stale data for 10% of TTL
                 expires_after=ttl_ends_at + datetime.timedelta(seconds=value.ttl_seconds // 10),
                 value=value
```

### Comparing `py-memoize-1.2.1/memoize/coerced.py` & `py-memoize-1.2.2/memoize/coerced.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.2.1/memoize/configuration.py` & `py-memoize-1.2.2/memoize/configuration.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.2.1/memoize/entry.py` & `py-memoize-1.2.2/memoize/entry.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.2.1/memoize/entrybuilder.py` & `py-memoize-1.2.2/memoize/entrybuilder.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.2.1/memoize/eviction.py` & `py-memoize-1.2.2/memoize/eviction.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.2.1/memoize/invalidation.py` & `py-memoize-1.2.2/memoize/invalidation.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.2.1/memoize/key.py` & `py-memoize-1.2.2/memoize/key.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.2.1/memoize/serde.py` & `py-memoize-1.2.2/memoize/serde.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.2.1/memoize/statuses.py` & `py-memoize-1.2.2/memoize/statuses.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.2.1/memoize/storage.py` & `py-memoize-1.2.2/memoize/storage.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.2.1/memoize/wrapper.py` & `py-memoize-1.2.2/memoize/wrapper.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.2.1/py_memoize.egg-info/PKG-INFO` & `py-memoize-1.2.2/py_memoize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-memoize
-Version: 1.2.1
+Version: 1.2.2
 Summary: Caching library for asynchronous Python applications (both based on asyncio and Tornado) that handles dogpiling properly and provides a configurable & extensible API.
 Home-page: https://github.com/DreamLab/memoize
 Author: Michal Zmuda
 Author-email: zmu.michal@gmail.com
 Maintainer: DreamLab
 License: Apache License 2.0
 Keywords: python cache tornado asyncio
@@ -483,15 +483,15 @@
     class ValueWithTTL:
         value: str
         ttl_seconds: int  # for instance, it could be derived from Cache-Control response header
 
 
     class TtlRespectingCacheEntryBuilder(CacheEntryBuilder):
         def build(self, key: CacheKey, value: ValueWithTTL):
-            now = datetime.datetime.utcnow()
+            now = datetime.datetime.now(datetime.timezone.utc)
             ttl_ends_at = now + datetime.timedelta(seconds=value.ttl_seconds)
             return CacheEntry(
                 created=now,
                 update_after=ttl_ends_at,
                 # allowing stale data for 10% of TTL
                 expires_after=ttl_ends_at + datetime.timedelta(seconds=value.ttl_seconds // 10),
                 value=value
```

### Comparing `py-memoize-1.2.1/setup.py` & `py-memoize-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     # but don't work at PyPi - therefore are removed
     description = description.replace(":class:", "")
     return description
 
 
 setup(
     name='py-memoize',
-    version='1.2.1',
+    version='1.2.2',
     author='Michal Zmuda',
     author_email='zmu.michal@gmail.com',
     url='https://github.com/DreamLab/memoize',
     maintainer='DreamLab',
     packages=['memoize'],
     test_suite='tests',
     license='Apache License 2.0',
```

