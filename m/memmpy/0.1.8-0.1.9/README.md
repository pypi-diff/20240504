# Comparing `tmp/memmpy-0.1.8.tar.gz` & `tmp/memmpy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memmpy-0.1.8.tar", last modified: Sat Jan 27 21:34:22 2024, max compression
+gzip compressed data, was "memmpy-0.1.9.tar", last modified: Sat Jan 27 21:47:32 2024, max compression
```

## Comparing `memmpy-0.1.8.tar` & `memmpy-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2024-01-27 21:34:22.652885 memmpy-0.1.8/
--rw-r--r--   0 anton     (1000) anton     (1000)     4875 2024-01-27 21:34:22.652885 memmpy-0.1.8/PKG-INFO
--rw-r--r--   0 anton     (1000) anton     (1000)     4615 2024-01-23 20:59:53.000000 memmpy-0.1.8/README.md
-drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2024-01-27 21:34:22.652885 memmpy-0.1.8/memmpy/
--rw-r--r--   0 anton     (1000) anton     (1000)      551 2024-01-27 21:34:03.000000 memmpy-0.1.8/memmpy/__init__.py
--rw-r--r--   0 anton     (1000) anton     (1000)    19672 2024-01-05 21:18:36.000000 memmpy-0.1.8/memmpy/_jagged.py
--rw-r--r--   0 anton     (1000) anton     (1000)     3126 2024-01-04 21:14:07.000000 memmpy-0.1.8/memmpy/_labels.py
--rw-r--r--   0 anton     (1000) anton     (1000)    14781 2024-01-09 13:53:57.000000 memmpy-0.1.8/memmpy/_loader.py
--rw-r--r--   0 anton     (1000) anton     (1000)     2800 2024-01-09 13:50:40.000000 memmpy-0.1.8/memmpy/_subset.py
--rw-r--r--   0 anton     (1000) anton     (1000)    12688 2024-01-27 21:14:43.000000 memmpy-0.1.8/memmpy/_vector.py
--rw-r--r--   0 anton     (1000) anton     (1000)     5795 2024-01-07 16:18:21.000000 memmpy-0.1.8/memmpy/reroot.py
-drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2024-01-27 21:34:22.652885 memmpy-0.1.8/memmpy.egg-info/
--rw-r--r--   0 anton     (1000) anton     (1000)     4875 2024-01-27 21:34:22.000000 memmpy-0.1.8/memmpy.egg-info/PKG-INFO
--rw-r--r--   0 anton     (1000) anton     (1000)      293 2024-01-27 21:34:22.000000 memmpy-0.1.8/memmpy.egg-info/SOURCES.txt
--rw-r--r--   0 anton     (1000) anton     (1000)        1 2024-01-27 21:34:22.000000 memmpy-0.1.8/memmpy.egg-info/dependency_links.txt
--rw-r--r--   0 anton     (1000) anton     (1000)       21 2024-01-27 21:34:22.000000 memmpy-0.1.8/memmpy.egg-info/requires.txt
--rw-r--r--   0 anton     (1000) anton     (1000)        7 2024-01-27 21:34:22.000000 memmpy-0.1.8/memmpy.egg-info/top_level.txt
--rw-r--r--   0 anton     (1000) anton     (1000)       38 2024-01-27 21:34:22.652885 memmpy-0.1.8/setup.cfg
--rw-r--r--   0 anton     (1000) anton     (1000)      637 2024-01-06 23:20:31.000000 memmpy-0.1.8/setup.py
+drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2024-01-27 21:47:32.310666 memmpy-0.1.9/
+-rw-r--r--   0 anton     (1000) anton     (1000)     4875 2024-01-27 21:47:32.310666 memmpy-0.1.9/PKG-INFO
+-rw-r--r--   0 anton     (1000) anton     (1000)     4615 2024-01-23 20:59:53.000000 memmpy-0.1.9/README.md
+drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2024-01-27 21:47:32.310666 memmpy-0.1.9/memmpy/
+-rw-r--r--   0 anton     (1000) anton     (1000)      551 2024-01-27 21:47:08.000000 memmpy-0.1.9/memmpy/__init__.py
+-rw-r--r--   0 anton     (1000) anton     (1000)    19672 2024-01-05 21:18:36.000000 memmpy-0.1.9/memmpy/_jagged.py
+-rw-r--r--   0 anton     (1000) anton     (1000)     3126 2024-01-04 21:14:07.000000 memmpy-0.1.9/memmpy/_labels.py
+-rw-r--r--   0 anton     (1000) anton     (1000)    14781 2024-01-09 13:53:57.000000 memmpy-0.1.9/memmpy/_loader.py
+-rw-r--r--   0 anton     (1000) anton     (1000)     2800 2024-01-09 13:50:40.000000 memmpy-0.1.9/memmpy/_subset.py
+-rw-r--r--   0 anton     (1000) anton     (1000)    12644 2024-01-27 21:45:19.000000 memmpy-0.1.9/memmpy/_vector.py
+-rw-r--r--   0 anton     (1000) anton     (1000)     5795 2024-01-07 16:18:21.000000 memmpy-0.1.9/memmpy/reroot.py
+drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2024-01-27 21:47:32.310666 memmpy-0.1.9/memmpy.egg-info/
+-rw-r--r--   0 anton     (1000) anton     (1000)     4875 2024-01-27 21:47:32.000000 memmpy-0.1.9/memmpy.egg-info/PKG-INFO
+-rw-r--r--   0 anton     (1000) anton     (1000)      293 2024-01-27 21:47:32.000000 memmpy-0.1.9/memmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 anton     (1000) anton     (1000)        1 2024-01-27 21:47:32.000000 memmpy-0.1.9/memmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 anton     (1000) anton     (1000)       21 2024-01-27 21:47:32.000000 memmpy-0.1.9/memmpy.egg-info/requires.txt
+-rw-r--r--   0 anton     (1000) anton     (1000)        7 2024-01-27 21:47:32.000000 memmpy-0.1.9/memmpy.egg-info/top_level.txt
+-rw-r--r--   0 anton     (1000) anton     (1000)       38 2024-01-27 21:47:32.310666 memmpy-0.1.9/setup.cfg
+-rw-r--r--   0 anton     (1000) anton     (1000)      637 2024-01-06 23:20:31.000000 memmpy-0.1.9/setup.py
```

### Comparing `memmpy-0.1.8/PKG-INFO` & `memmpy-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memmpy
-Version: 0.1.8
+Version: 0.1.9
 Summary: Memory mapped of datasets
 Home-page: https://github.com/pwolle/memmpy
 Author: Paul Wollenhaupt
 Author-email: paul.wollenhaupt@gmail.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `memmpy-0.1.8/README.md` & `memmpy-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `memmpy-0.1.8/memmpy/__init__.py` & `memmpy-0.1.9/memmpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,8 +24,8 @@
     "compute_cut_batched",
     "WriteVector",
     "WriteVectorDict",
     "read_vector",
     "read_vectors",
 ]
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
```

### Comparing `memmpy-0.1.8/memmpy/_jagged.py` & `memmpy-0.1.9/memmpy/_jagged.py`

 * *Files identical despite different names*

### Comparing `memmpy-0.1.8/memmpy/_labels.py` & `memmpy-0.1.9/memmpy/_labels.py`

 * *Files identical despite different names*

### Comparing `memmpy-0.1.8/memmpy/_loader.py` & `memmpy-0.1.9/memmpy/_loader.py`

 * *Files identical despite different names*

### Comparing `memmpy-0.1.8/memmpy/_subset.py` & `memmpy-0.1.9/memmpy/_subset.py`

 * *Files identical despite different names*

### Comparing `memmpy-0.1.8/memmpy/_vector.py` & `memmpy-0.1.9/memmpy/_vector.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,14 @@
             error = f"Got shape {value.shape[1:]} != {self._mmap.shape[1:]}."
             raise ValueError(error)
 
         length = self._index + value.shape[0]
 
         if length > self._mmap.shape[0]:
             length = 2 ** math.ceil(math.log2(length))
-            print(f"Resizing to {length}.")
 
             self._file = tempfile.NamedTemporaryFile()
             mmap = np.memmap(
                 self._file,
                 self.dtype,
                 "w+",
                 shape=(length, *self._mmap.shape[1:]),
```

### Comparing `memmpy-0.1.8/memmpy/reroot.py` & `memmpy-0.1.9/memmpy/reroot.py`

 * *Files identical despite different names*

### Comparing `memmpy-0.1.8/memmpy.egg-info/PKG-INFO` & `memmpy-0.1.9/memmpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memmpy
-Version: 0.1.8
+Version: 0.1.9
 Summary: Memory mapped of datasets
 Home-page: https://github.com/pwolle/memmpy
 Author: Paul Wollenhaupt
 Author-email: paul.wollenhaupt@gmail.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `memmpy-0.1.8/setup.py` & `memmpy-0.1.9/setup.py`

 * *Files identical despite different names*

