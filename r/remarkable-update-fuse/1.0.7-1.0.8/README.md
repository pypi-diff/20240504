# Comparing `tmp/remarkable_update_fuse-1.0.7.tar.gz` & `tmp/remarkable_update_fuse-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remarkable_update_fuse-1.0.7.tar", last modified: Thu Apr 11 22:23:51 2024, max compression
+gzip compressed data, was "remarkable_update_fuse-1.0.8.tar", last modified: Sat May  4 09:09:37 2024, max compression
```

## Comparing `remarkable_update_fuse-1.0.7.tar` & `remarkable_update_fuse-1.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:23:51.607398 remarkable_update_fuse-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-11 22:23:33.000000 remarkable_update_fuse-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-11 22:23:51.607398 remarkable_update_fuse-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-11 22:23:33.000000 remarkable_update_fuse-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-11 22:23:33.000000 remarkable_update_fuse-1.0.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:23:51.603398 remarkable_update_fuse-1.0.7/remarkable_update_fuse/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-11 22:23:33.000000 remarkable_update_fuse-1.0.7/remarkable_update_fuse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-11 22:23:33.000000 remarkable_update_fuse-1.0.7/remarkable_update_fuse/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9712 2024-04-11 22:23:33.000000 remarkable_update_fuse-1.0.7/remarkable_update_fuse/fuse.py
--rw-r--r--   0 runner    (1001) docker     (127)     8972 2024-04-11 22:23:33.000000 remarkable_update_fuse-1.0.7/remarkable_update_fuse/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-11 22:23:33.000000 remarkable_update_fuse-1.0.7/remarkable_update_fuse/threads.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-11 22:23:45.000000 remarkable_update_fuse-1.0.7/remarkable_update_fuse/update_metadata_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:23:51.607398 remarkable_update_fuse-1.0.7/remarkable_update_fuse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-11 22:23:51.000000 remarkable_update_fuse-1.0.7/remarkable_update_fuse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-11 22:23:51.000000 remarkable_update_fuse-1.0.7/remarkable_update_fuse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:23:51.000000 remarkable_update_fuse-1.0.7/remarkable_update_fuse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 22:23:51.000000 remarkable_update_fuse-1.0.7/remarkable_update_fuse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 22:23:51.000000 remarkable_update_fuse-1.0.7/remarkable_update_fuse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-11 22:23:51.000000 remarkable_update_fuse-1.0.7/remarkable_update_fuse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 22:23:33.000000 remarkable_update_fuse-1.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 22:23:51.607398 remarkable_update_fuse-1.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:09:37.605716 remarkable_update_fuse-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-04 09:09:05.000000 remarkable_update_fuse-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-04 09:09:37.605716 remarkable_update_fuse-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-04 09:09:05.000000 remarkable_update_fuse-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-04 09:09:05.000000 remarkable_update_fuse-1.0.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:09:37.605716 remarkable_update_fuse-1.0.8/remarkable_update_fuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-04 09:09:05.000000 remarkable_update_fuse-1.0.8/remarkable_update_fuse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-04 09:09:05.000000 remarkable_update_fuse-1.0.8/remarkable_update_fuse/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9712 2024-05-04 09:09:05.000000 remarkable_update_fuse-1.0.8/remarkable_update_fuse/fuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-05-04 09:09:05.000000 remarkable_update_fuse-1.0.8/remarkable_update_fuse/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-04 09:09:05.000000 remarkable_update_fuse-1.0.8/remarkable_update_fuse/threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-04 09:09:26.000000 remarkable_update_fuse-1.0.8/remarkable_update_fuse/update_metadata_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:09:37.605716 remarkable_update_fuse-1.0.8/remarkable_update_fuse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-04 09:09:37.000000 remarkable_update_fuse-1.0.8/remarkable_update_fuse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-04 09:09:37.000000 remarkable_update_fuse-1.0.8/remarkable_update_fuse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 09:09:37.000000 remarkable_update_fuse-1.0.8/remarkable_update_fuse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-04 09:09:37.000000 remarkable_update_fuse-1.0.8/remarkable_update_fuse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-04 09:09:37.000000 remarkable_update_fuse-1.0.8/remarkable_update_fuse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-04 09:09:37.000000 remarkable_update_fuse-1.0.8/remarkable_update_fuse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-04 09:09:05.000000 remarkable_update_fuse-1.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 09:09:37.605716 remarkable_update_fuse-1.0.8/setup.cfg
```

### Comparing `remarkable_update_fuse-1.0.7/LICENSE` & `remarkable_update_fuse-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `remarkable_update_fuse-1.0.7/PKG-INFO` & `remarkable_update_fuse-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remarkable_update_fuse
-Version: 1.0.7
+Version: 1.0.8
 Summary: Userspace filesystem for remarkable update files
 Author-email: Eeems <eeems@eeems.email>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -58,14 +58,15 @@
 with open("version", "wb") as f:
     f.write(inode.open().read())
 ```
 
 ## Building
 Dependencies:
 - curl
+- protoc
 - python
 - python-build
 - python-pip
 - python-pipx
 - python-venv
 - python-wheel
```

### Comparing `remarkable_update_fuse-1.0.7/README.md` & `remarkable_update_fuse-1.0.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 with open("version", "wb") as f:
     f.write(inode.open().read())
 ```
 
 ## Building
 Dependencies:
 - curl
+- protoc
 - python
 - python-build
 - python-pip
 - python-pipx
 - python-venv
 - python-wheel
```

### Comparing `remarkable_update_fuse-1.0.7/pyproject.toml` & `remarkable_update_fuse-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "remarkable_update_fuse"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
   { name="Eeems", email="eeems@eeems.email" },
 ]
 description = "Userspace filesystem for remarkable update files"
 requires-python = ">=3.11"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `remarkable_update_fuse-1.0.7/remarkable_update_fuse/fuse.py` & `remarkable_update_fuse-1.0.8/remarkable_update_fuse/fuse.py`

 * *Files identical despite different names*

### Comparing `remarkable_update_fuse-1.0.7/remarkable_update_fuse/image.py` & `remarkable_update_fuse-1.0.8/remarkable_update_fuse/image.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,18 @@
     for unit in ("", "Ki", "Mi", "Gi", "Ti", "Pi", "Ei", "Zi"):
         if abs(num) < 1024.0:
             return f"{num:3.1f}{unit}{suffix}"
         num /= 1024.0
     return f"{num:.1f}Yi{suffix}"
 
 
+def range_contains(range1, range2):
+    return range1.start < range2.stop and range2.start < range1.stop
+
+
 class BlockCache(TTLCache):
     def __init__(self, maxsize, ttl, timer=time.monotonic, getsizeof=sys.getsizeof):
         super().__init__(maxsize, ttl, timer, getsizeof)
 
     @property
     def usage_str(self):
         return f"{self.curr_size_str}/{self.max_size_str}"
@@ -219,17 +223,21 @@
             return b""
 
         if size <= 0 or offset + size > self._size:
             size = self._size - offset
 
         res = bytearray(size)
         for blob, blob_offset, blob_length, f in self._blobs:
-            if offset < blob_offset:
-                continue
-            if offset >= blob_offset + blob_length:
+            if not range_contains(
+                range(offset, offset + size),
+                range(blob_offset, blob_offset + blob_length),
+            ):
+                if size >= self._size:
+                    print(f"Skipping blob {blob_offset} to {blob_length}, {offset}")
+
                 continue
 
             blob_data = self._read_blob(blob, blob_offset, blob_length, f)
             blob_start_offset = max(offset - blob_offset, 0)
             blob_end_offset = min(offset - blob_offset + size, blob_length)
             data = blob_data[blob_start_offset:blob_end_offset]
```

### Comparing `remarkable_update_fuse-1.0.7/remarkable_update_fuse/threads.py` & `remarkable_update_fuse-1.0.8/remarkable_update_fuse/threads.py`

 * *Files identical despite different names*

### Comparing `remarkable_update_fuse-1.0.7/remarkable_update_fuse/update_metadata_pb2.py` & `remarkable_update_fuse-1.0.8/remarkable_update_fuse/update_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `remarkable_update_fuse-1.0.7/remarkable_update_fuse.egg-info/PKG-INFO` & `remarkable_update_fuse-1.0.8/remarkable_update_fuse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remarkable_update_fuse
-Version: 1.0.7
+Version: 1.0.8
 Summary: Userspace filesystem for remarkable update files
 Author-email: Eeems <eeems@eeems.email>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -58,14 +58,15 @@
 with open("version", "wb") as f:
     f.write(inode.open().read())
 ```
 
 ## Building
 Dependencies:
 - curl
+- protoc
 - python
 - python-build
 - python-pip
 - python-pipx
 - python-venv
 - python-wheel
```

### Comparing `remarkable_update_fuse-1.0.7/remarkable_update_fuse.egg-info/SOURCES.txt` & `remarkable_update_fuse-1.0.8/remarkable_update_fuse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

