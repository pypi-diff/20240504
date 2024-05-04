# Comparing `tmp/py-memoize-1.1.4.tar.gz` & `tmp/py-memoize-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-memoize-1.1.4.tar", last modified: Thu Feb 15 18:39:35 2024, max compression
+gzip compressed data, was "py-memoize-1.1.5.tar", last modified: Fri May  3 19:42:30 2024, max compression
```

## Comparing `py-memoize-1.1.4.tar` & `py-memoize-1.1.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 18:39:35.404994 py-memoize-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-02-15 18:39:27.000000 py-memoize-1.1.4/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-15 18:39:27.000000 py-memoize-1.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16115 2024-02-15 18:39:35.404994 py-memoize-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15141 2024-02-15 18:39:27.000000 py-memoize-1.1.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 18:39:35.404994 py-memoize-1.1.4/memoize/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-15 18:39:27.000000 py-memoize-1.1.4/memoize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-02-15 18:39:27.000000 py-memoize-1.1.4/memoize/coerced.py
--rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-02-15 18:39:27.000000 py-memoize-1.1.4/memoize/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-02-15 18:39:27.000000 py-memoize-1.1.4/memoize/entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-02-15 18:39:27.000000 py-memoize-1.1.4/memoize/entrybuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-02-15 18:39:27.000000 py-memoize-1.1.4/memoize/eviction.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-15 18:39:27.000000 py-memoize-1.1.4/memoize/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-02-15 18:39:27.000000 py-memoize-1.1.4/memoize/invalidation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-02-15 18:39:27.000000 py-memoize-1.1.4/memoize/key.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-02-15 18:39:27.000000 py-memoize-1.1.4/memoize/memoize_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-02-15 18:39:27.000000 py-memoize-1.1.4/memoize/serde.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-02-15 18:39:27.000000 py-memoize-1.1.4/memoize/statuses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-02-15 18:39:27.000000 py-memoize-1.1.4/memoize/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-02-15 18:39:27.000000 py-memoize-1.1.4/memoize/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 18:39:35.404994 py-memoize-1.1.4/py_memoize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16115 2024-02-15 18:39:35.000000 py-memoize-1.1.4/py_memoize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-02-15 18:39:35.000000 py-memoize-1.1.4/py_memoize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 18:39:35.000000 py-memoize-1.1.4/py_memoize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-15 18:39:35.000000 py-memoize-1.1.4/py_memoize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-15 18:39:35.000000 py-memoize-1.1.4/py_memoize.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 18:39:35.404994 py-memoize-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-02-15 18:39:27.000000 py-memoize-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:42:30.045339 py-memoize-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-03 19:42:18.000000 py-memoize-1.1.5/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-03 19:42:18.000000 py-memoize-1.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18727 2024-05-03 19:42:30.045339 py-memoize-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17760 2024-05-03 19:42:18.000000 py-memoize-1.1.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:42:30.045339 py-memoize-1.1.5/memoize/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 19:42:18.000000 py-memoize-1.1.5/memoize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-03 19:42:18.000000 py-memoize-1.1.5/memoize/coerced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-05-03 19:42:18.000000 py-memoize-1.1.5/memoize/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-03 19:42:18.000000 py-memoize-1.1.5/memoize/entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-03 19:42:18.000000 py-memoize-1.1.5/memoize/entrybuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-03 19:42:18.000000 py-memoize-1.1.5/memoize/eviction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-03 19:42:18.000000 py-memoize-1.1.5/memoize/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-03 19:42:18.000000 py-memoize-1.1.5/memoize/invalidation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-03 19:42:18.000000 py-memoize-1.1.5/memoize/key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-03 19:42:18.000000 py-memoize-1.1.5/memoize/memoize_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-03 19:42:18.000000 py-memoize-1.1.5/memoize/serde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-03 19:42:18.000000 py-memoize-1.1.5/memoize/statuses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-03 19:42:18.000000 py-memoize-1.1.5/memoize/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-05-03 19:42:18.000000 py-memoize-1.1.5/memoize/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:42:30.045339 py-memoize-1.1.5/py_memoize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18727 2024-05-03 19:42:29.000000 py-memoize-1.1.5/py_memoize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-03 19:42:30.000000 py-memoize-1.1.5/py_memoize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:42:29.000000 py-memoize-1.1.5/py_memoize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-03 19:42:29.000000 py-memoize-1.1.5/py_memoize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 19:42:29.000000 py-memoize-1.1.5/py_memoize.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 19:42:30.045339 py-memoize-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-03 19:42:18.000000 py-memoize-1.1.5/setup.py
```

### Comparing `py-memoize-1.1.4/LICENCE` & `py-memoize-1.1.5/LICENCE`

 * *Files identical despite different names*

### Comparing `py-memoize-1.1.4/PKG-INFO` & `py-memoize-1.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-memoize
-Version: 1.1.4
+Version: 1.1.5
 Summary: Caching library for asynchronous Python applications (both based on asyncio and Tornado) that handles dogpiling properly and provides a configurable & extensible API.
 Home-page: https://github.com/DreamLab/memoize
 Author: Michal Zmuda
 Author-email: zmu.michal@gmail.com
 Maintainer: DreamLab
 License: Apache License 2.0
 Keywords: python cache tornado asyncio
@@ -448,7 +448,82 @@
         # expensive - computation - 73
         # expensive - computation - 73
         # Invalidation  # 2
         # expensive - computation - 59
 
     if __name__ == "__main__":
         asyncio.get_event_loop().run_until_complete(main())
+
+
+Openness to granular TTL
+------------------------
+
+Default configuration sets update and expiry based on fixed values, which are the same for all entries.
+If you need to set different TTLs for different entries, you can do so by providing
+a custom `memoize.entrybuilder.CacheEntryBuilder`.
+
+.. code-block:: python
+
+    import datetime
+    import asyncio
+    import random
+    from dataclasses import dataclass
+
+    from memoize.wrapper import memoize
+    from memoize.configuration import DefaultInMemoryCacheConfiguration, MutableCacheConfiguration
+    from memoize.entry import CacheKey, CacheEntry
+    from memoize.entrybuilder import CacheEntryBuilder
+    from memoize.storage import LocalInMemoryCacheStorage
+
+
+    @dataclass
+    class ValueWithTTL:
+        value: str
+        ttl_seconds: int  # for instance, it could be derived from Cache-Control response header
+
+
+    class TtlRespectingCacheEntryBuilder(CacheEntryBuilder):
+        def build(self, key: CacheKey, value: ValueWithTTL):
+            now = datetime.datetime.utcnow()
+            ttl_ends_at = now + datetime.timedelta(seconds=value.ttl_seconds)
+            return CacheEntry(
+                created=now,
+                update_after=ttl_ends_at,
+                # allowing stale data for 10% of TTL
+                expires_after=ttl_ends_at + datetime.timedelta(seconds=value.ttl_seconds // 10),
+                value=value
+            )
+
+
+    storage = LocalInMemoryCacheStorage()  # overridden & extracted for demonstration purposes only
+
+
+    @memoize(configuration=MutableCacheConfiguration
+             .initialized_with(DefaultInMemoryCacheConfiguration())
+             .set_entry_builder(TtlRespectingCacheEntryBuilder())
+             .set_storage(storage))
+    async def external_call(key: str):
+        return ValueWithTTL(
+            value=f'{key}-result-{random.randint(1, 100)}',
+            ttl_seconds=random.randint(60, 300)
+        )
+
+
+    async def main():
+        await external_call('a')
+        await external_call('b')
+        await external_call('b')
+
+        print("Entries persisted in the cache:")
+        for entry in storage._data.values():
+            print('Entry: ', entry.value)
+            print('Effective TTL: ', (entry.update_after - entry.created).total_seconds())
+
+        # Entries persisted in the cache:
+        # Entry: ValueWithTTL(value='a-result-79', ttl_seconds=148)
+        # Effective TTL: 148.0
+        # Entry: ValueWithTTL(value='b-result-27', ttl_seconds=192)
+        # Effective TTL: 192.0
+
+
+    if __name__ == "__main__":
+        asyncio.get_event_loop().run_until_complete(main())
```

### Comparing `py-memoize-1.1.4/README.rst` & `py-memoize-1.1.5/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -421,8 +421,83 @@
         # Invalidation  # 1
         # expensive - computation - 73
         # expensive - computation - 73
         # Invalidation  # 2
         # expensive - computation - 59
 
     if __name__ == "__main__":
+        asyncio.get_event_loop().run_until_complete(main())
+
+
+Openness to granular TTL
+------------------------
+
+Default configuration sets update and expiry based on fixed values, which are the same for all entries.
+If you need to set different TTLs for different entries, you can do so by providing
+a custom :class:`memoize.entrybuilder.CacheEntryBuilder`.
+
+.. code-block:: python
+
+    import datetime
+    import asyncio
+    import random
+    from dataclasses import dataclass
+
+    from memoize.wrapper import memoize
+    from memoize.configuration import DefaultInMemoryCacheConfiguration, MutableCacheConfiguration
+    from memoize.entry import CacheKey, CacheEntry
+    from memoize.entrybuilder import CacheEntryBuilder
+    from memoize.storage import LocalInMemoryCacheStorage
+
+
+    @dataclass
+    class ValueWithTTL:
+        value: str
+        ttl_seconds: int  # for instance, it could be derived from Cache-Control response header
+
+
+    class TtlRespectingCacheEntryBuilder(CacheEntryBuilder):
+        def build(self, key: CacheKey, value: ValueWithTTL):
+            now = datetime.datetime.utcnow()
+            ttl_ends_at = now + datetime.timedelta(seconds=value.ttl_seconds)
+            return CacheEntry(
+                created=now,
+                update_after=ttl_ends_at,
+                # allowing stale data for 10% of TTL
+                expires_after=ttl_ends_at + datetime.timedelta(seconds=value.ttl_seconds // 10),
+                value=value
+            )
+
+
+    storage = LocalInMemoryCacheStorage()  # overridden & extracted for demonstration purposes only
+
+
+    @memoize(configuration=MutableCacheConfiguration
+             .initialized_with(DefaultInMemoryCacheConfiguration())
+             .set_entry_builder(TtlRespectingCacheEntryBuilder())
+             .set_storage(storage))
+    async def external_call(key: str):
+        return ValueWithTTL(
+            value=f'{key}-result-{random.randint(1, 100)}',
+            ttl_seconds=random.randint(60, 300)
+        )
+
+
+    async def main():
+        await external_call('a')
+        await external_call('b')
+        await external_call('b')
+
+        print("Entries persisted in the cache:")
+        for entry in storage._data.values():
+            print('Entry: ', entry.value)
+            print('Effective TTL: ', (entry.update_after - entry.created).total_seconds())
+
+        # Entries persisted in the cache:
+        # Entry: ValueWithTTL(value='a-result-79', ttl_seconds=148)
+        # Effective TTL: 148.0
+        # Entry: ValueWithTTL(value='b-result-27', ttl_seconds=192)
+        # Effective TTL: 192.0
+
+
+    if __name__ == "__main__":
         asyncio.get_event_loop().run_until_complete(main())
```

### Comparing `py-memoize-1.1.4/memoize/coerced.py` & `py-memoize-1.1.5/memoize/coerced.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.1.4/memoize/configuration.py` & `py-memoize-1.1.5/memoize/configuration.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.1.4/memoize/entry.py` & `py-memoize-1.1.5/memoize/entry.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.1.4/memoize/entrybuilder.py` & `py-memoize-1.1.5/memoize/entrybuilder.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.1.4/memoize/eviction.py` & `py-memoize-1.1.5/memoize/eviction.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.1.4/memoize/invalidation.py` & `py-memoize-1.1.5/memoize/invalidation.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.1.4/memoize/key.py` & `py-memoize-1.1.5/memoize/key.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.1.4/memoize/serde.py` & `py-memoize-1.1.5/memoize/serde.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.1.4/memoize/statuses.py` & `py-memoize-1.1.5/memoize/statuses.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.1.4/memoize/storage.py` & `py-memoize-1.1.5/memoize/storage.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.1.4/memoize/wrapper.py` & `py-memoize-1.1.5/memoize/wrapper.py`

 * *Files identical despite different names*

### Comparing `py-memoize-1.1.4/py_memoize.egg-info/PKG-INFO` & `py-memoize-1.1.5/py_memoize.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-memoize
-Version: 1.1.4
+Version: 1.1.5
 Summary: Caching library for asynchronous Python applications (both based on asyncio and Tornado) that handles dogpiling properly and provides a configurable & extensible API.
 Home-page: https://github.com/DreamLab/memoize
 Author: Michal Zmuda
 Author-email: zmu.michal@gmail.com
 Maintainer: DreamLab
 License: Apache License 2.0
 Keywords: python cache tornado asyncio
@@ -448,7 +448,82 @@
         # expensive - computation - 73
         # expensive - computation - 73
         # Invalidation  # 2
         # expensive - computation - 59
 
     if __name__ == "__main__":
         asyncio.get_event_loop().run_until_complete(main())
+
+
+Openness to granular TTL
+------------------------
+
+Default configuration sets update and expiry based on fixed values, which are the same for all entries.
+If you need to set different TTLs for different entries, you can do so by providing
+a custom `memoize.entrybuilder.CacheEntryBuilder`.
+
+.. code-block:: python
+
+    import datetime
+    import asyncio
+    import random
+    from dataclasses import dataclass
+
+    from memoize.wrapper import memoize
+    from memoize.configuration import DefaultInMemoryCacheConfiguration, MutableCacheConfiguration
+    from memoize.entry import CacheKey, CacheEntry
+    from memoize.entrybuilder import CacheEntryBuilder
+    from memoize.storage import LocalInMemoryCacheStorage
+
+
+    @dataclass
+    class ValueWithTTL:
+        value: str
+        ttl_seconds: int  # for instance, it could be derived from Cache-Control response header
+
+
+    class TtlRespectingCacheEntryBuilder(CacheEntryBuilder):
+        def build(self, key: CacheKey, value: ValueWithTTL):
+            now = datetime.datetime.utcnow()
+            ttl_ends_at = now + datetime.timedelta(seconds=value.ttl_seconds)
+            return CacheEntry(
+                created=now,
+                update_after=ttl_ends_at,
+                # allowing stale data for 10% of TTL
+                expires_after=ttl_ends_at + datetime.timedelta(seconds=value.ttl_seconds // 10),
+                value=value
+            )
+
+
+    storage = LocalInMemoryCacheStorage()  # overridden & extracted for demonstration purposes only
+
+
+    @memoize(configuration=MutableCacheConfiguration
+             .initialized_with(DefaultInMemoryCacheConfiguration())
+             .set_entry_builder(TtlRespectingCacheEntryBuilder())
+             .set_storage(storage))
+    async def external_call(key: str):
+        return ValueWithTTL(
+            value=f'{key}-result-{random.randint(1, 100)}',
+            ttl_seconds=random.randint(60, 300)
+        )
+
+
+    async def main():
+        await external_call('a')
+        await external_call('b')
+        await external_call('b')
+
+        print("Entries persisted in the cache:")
+        for entry in storage._data.values():
+            print('Entry: ', entry.value)
+            print('Effective TTL: ', (entry.update_after - entry.created).total_seconds())
+
+        # Entries persisted in the cache:
+        # Entry: ValueWithTTL(value='a-result-79', ttl_seconds=148)
+        # Effective TTL: 148.0
+        # Entry: ValueWithTTL(value='b-result-27', ttl_seconds=192)
+        # Effective TTL: 192.0
+
+
+    if __name__ == "__main__":
+        asyncio.get_event_loop().run_until_complete(main())
```

### Comparing `py-memoize-1.1.4/setup.py` & `py-memoize-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     # but don't work at PyPi - therefore are removed
     description = description.replace(":class:", "")
     return description
 
 
 setup(
     name='py-memoize',
-    version='1.1.4',
+    version='1.1.5',
     author='Michal Zmuda',
     author_email='zmu.michal@gmail.com',
     url='https://github.com/DreamLab/memoize',
     maintainer='DreamLab',
     packages=['memoize'],
     test_suite='tests',
     license='Apache License 2.0',
```

