# Comparing `tmp/py-memoize-1.2.0.tar.gz` & `tmp/py-memoize-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-memoize-1.2.0.tar", last modified: Sat May  4 06:11:50 2024, max compression
+gzip compressed data, was "py-memoize-1.2.1.tar", last modified: Sat May  4 07:14:12 2024, max compression
```

## Comparing `py-memoize-1.2.0.tar` & `py-memoize-1.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:11:50.894727 py-memoize-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-04 06:11:42.000000 py-memoize-1.2.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-04 06:11:42.000000 py-memoize-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    18899 2024-05-04 06:11:50.894727 py-memoize-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17881 2024-05-04 06:11:42.000000 py-memoize-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:11:50.894727 py-memoize-1.2.0/memoize/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-04 06:11:42.000000 py-memoize-1.2.0/memoize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-05-04 06:11:42.000000 py-memoize-1.2.0/memoize/coerced.py
--rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-05-04 06:11:42.000000 py-memoize-1.2.0/memoize/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-04 06:11:42.000000 py-memoize-1.2.0/memoize/entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-04 06:11:42.000000 py-memoize-1.2.0/memoize/entrybuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-04 06:11:42.000000 py-memoize-1.2.0/memoize/eviction.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-04 06:11:42.000000 py-memoize-1.2.0/memoize/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-04 06:11:42.000000 py-memoize-1.2.0/memoize/invalidation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-04 06:11:42.000000 py-memoize-1.2.0/memoize/key.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-04 06:11:42.000000 py-memoize-1.2.0/memoize/memoize_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-04 06:11:42.000000 py-memoize-1.2.0/memoize/serde.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-04 06:11:42.000000 py-memoize-1.2.0/memoize/statuses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-04 06:11:42.000000 py-memoize-1.2.0/memoize/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-05-04 06:11:42.000000 py-memoize-1.2.0/memoize/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 06:11:50.894727 py-memoize-1.2.0/py_memoize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18899 2024-05-04 06:11:50.000000 py-memoize-1.2.0/py_memoize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-04 06:11:50.000000 py-memoize-1.2.0/py_memoize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 06:11:50.000000 py-memoize-1.2.0/py_memoize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-04 06:11:50.000000 py-memoize-1.2.0/py_memoize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 06:11:50.000000 py-memoize-1.2.0/py_memoize.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 06:11:50.894727 py-memoize-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-04 06:11:42.000000 py-memoize-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:14:12.755412 py-memoize-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-04 07:14:03.000000 py-memoize-1.2.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-04 07:14:03.000000 py-memoize-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18899 2024-05-04 07:14:12.755412 py-memoize-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17881 2024-05-04 07:14:03.000000 py-memoize-1.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:14:12.751412 py-memoize-1.2.1/memoize/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-04 07:14:03.000000 py-memoize-1.2.1/memoize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-05-04 07:14:03.000000 py-memoize-1.2.1/memoize/coerced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-05-04 07:14:03.000000 py-memoize-1.2.1/memoize/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-04 07:14:03.000000 py-memoize-1.2.1/memoize/entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-04 07:14:03.000000 py-memoize-1.2.1/memoize/entrybuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-04 07:14:03.000000 py-memoize-1.2.1/memoize/eviction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-04 07:14:03.000000 py-memoize-1.2.1/memoize/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-04 07:14:03.000000 py-memoize-1.2.1/memoize/invalidation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-04 07:14:03.000000 py-memoize-1.2.1/memoize/key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-04 07:14:03.000000 py-memoize-1.2.1/memoize/memoize_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-04 07:14:03.000000 py-memoize-1.2.1/memoize/serde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-04 07:14:03.000000 py-memoize-1.2.1/memoize/statuses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-04 07:14:03.000000 py-memoize-1.2.1/memoize/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-05-04 07:14:03.000000 py-memoize-1.2.1/memoize/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:14:12.755412 py-memoize-1.2.1/py_memoize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18899 2024-05-04 07:14:12.000000 py-memoize-1.2.1/py_memoize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-04 07:14:12.000000 py-memoize-1.2.1/py_memoize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 07:14:12.000000 py-memoize-1.2.1/py_memoize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-04 07:14:12.000000 py-memoize-1.2.1/py_memoize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 07:14:12.000000 py-memoize-1.2.1/py_memoize.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 07:14:12.755412 py-memoize-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-04 07:14:03.000000 py-memoize-1.2.1/setup.py
```

### Comparing `py-memoize-1.2.0/LICENCE` & `py-memoize-1.2.1/LICENCE`

 * *Files identical despite different names*

### Comparing `py-memoize-1.2.0/PKG-INFO` & `py-memoize-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-memoize
-Version: 1.2.0
+Version: 1.2.1
 Summary: Caching library for asynchronous Python applications (both based on asyncio and Tornado) that handles dogpiling properly and provides a configurable & extensible API.
 Home-page: https://github.com/DreamLab/memoize
 Author: Michal Zmuda
 Author-email: zmu.michal@gmail.com
 Maintainer: DreamLab
 License: Apache License 2.0
 Keywords: python cache tornado asyncio
```

### Comparing `py-memoize-1.2.0/README.rst` & `py-memoize-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `py-memoize-1.2.0/memoize/coerced.py` & `py-memoize-1.2.1/memoize/coerced.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.2.0/memoize/configuration.py` & `py-memoize-1.2.1/memoize/configuration.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.2.0/memoize/entry.py` & `py-memoize-1.2.1/memoize/entry.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.2.0/memoize/entrybuilder.py` & `py-memoize-1.2.1/memoize/entrybuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         self._update_after = update_after
 
     def update_timeouts(self, update_after: datetime.timedelta, expire_after: datetime.timedelta) -> None:
         self._expires_after = expire_after
         self._update_after = update_after
 
     def build(self, key: CacheKey, value: CachedValue) -> CacheEntry:
-        now = datetime.datetime.utcnow()
+        now = datetime.datetime.now(datetime.timezone.utc)
         return CacheEntry(created=now,
                           update_after=now + self._update_after,
                           expires_after=now + self._expires_after,
                           value=value)
 
     def __str__(self) -> str:
         return "{}[update_after={},expire_after={}]".format(self.__class__, self._update_after, self._expires_after)
```

### Comparing `py-memoize-1.2.0/memoize/eviction.py` & `py-memoize-1.2.1/memoize/eviction.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.2.0/memoize/invalidation.py` & `py-memoize-1.2.1/memoize/invalidation.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.2.0/memoize/key.py` & `py-memoize-1.2.1/memoize/key.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.2.0/memoize/serde.py` & `py-memoize-1.2.1/memoize/serde.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 try:
     import ujson as json
 except:
     # ignoring type error as mypy falsely reports json is already imported
     import json  # type: ignore
 from abc import ABCMeta, abstractmethod
-from datetime import datetime
+from datetime import datetime, timezone
 
 from typing import Callable, Any
 
 from memoize.entry import CacheEntry, CachedValue
 
 
 class SerDe(metaclass=ABCMeta):
@@ -58,17 +58,17 @@
         self.__string_encoding = string_encoding
         self.__reversible_repr_to_value = reversible_repr_to_value
         self.__value_to_reversible_repr = value_to_reversible_repr
 
     def deserialize(self, data: bytes) -> CacheEntry:
         as_dict = json.loads(codecs.decode(data, self.__string_encoding))
         return CacheEntry(
-            created=datetime.utcfromtimestamp(as_dict['created']),
-            update_after=datetime.utcfromtimestamp(as_dict['update_after']),
-            expires_after=datetime.utcfromtimestamp(as_dict['expires_after']),
+            created=datetime.fromtimestamp(as_dict['created'], timezone.utc),
+            update_after=datetime.fromtimestamp(as_dict['update_after'], timezone.utc),
+            expires_after=datetime.fromtimestamp(as_dict['expires_after'], timezone.utc),
             value=self.__reversible_repr_to_value(as_dict['value']),
         )
 
     def serialize(self, entry: CacheEntry) -> bytes:
         return codecs.encode(json.dumps({
             'created': entry.created.timestamp(),
             'update_after': entry.update_after.timestamp(),
```

### Comparing `py-memoize-1.2.0/memoize/statuses.py` & `py-memoize-1.2.1/memoize/statuses.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.2.0/memoize/storage.py` & `py-memoize-1.2.1/memoize/storage.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.2.0/memoize/wrapper.py` & `py-memoize-1.2.1/memoize/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         force_refresh = kwargs.pop('force_refresh_memoized', False)
         key = configuration_snapshot.key_extractor().format_key(method, args, kwargs)
 
         current_entry = await configuration_snapshot.storage().get(key)  # type: Optional[CacheEntry]
         if current_entry is not None:
             configuration_snapshot.eviction_strategy().mark_read(key)
 
-        now = datetime.datetime.utcnow()
+        now = datetime.datetime.now(datetime.timezone.utc)
 
         def value_future_provider():
             return _apply_timeout(configuration_snapshot.method_timeout(), method(*args, **kwargs))
 
         if current_entry is None:
             logger.debug('Creating (blocking) entry for key %s', key)
             result = await refresh(current_entry, key, value_future_provider, configuration_snapshot)
```

### Comparing `py-memoize-1.2.0/py_memoize.egg-info/PKG-INFO` & `py-memoize-1.2.1/py_memoize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-memoize
-Version: 1.2.0
+Version: 1.2.1
 Summary: Caching library for asynchronous Python applications (both based on asyncio and Tornado) that handles dogpiling properly and provides a configurable & extensible API.
 Home-page: https://github.com/DreamLab/memoize
 Author: Michal Zmuda
 Author-email: zmu.michal@gmail.com
 Maintainer: DreamLab
 License: Apache License 2.0
 Keywords: python cache tornado asyncio
```

### Comparing `py-memoize-1.2.0/setup.py` & `py-memoize-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     # but don't work at PyPi - therefore are removed
     description = description.replace(":class:", "")
     return description
 
 
 setup(
     name='py-memoize',
-    version='1.2.0',
+    version='1.2.1',
     author='Michal Zmuda',
     author_email='zmu.michal@gmail.com',
     url='https://github.com/DreamLab/memoize',
     maintainer='DreamLab',
     packages=['memoize'],
     test_suite='tests',
     license='Apache License 2.0',
```

