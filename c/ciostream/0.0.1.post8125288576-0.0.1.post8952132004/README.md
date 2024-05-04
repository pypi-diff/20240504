# Comparing `tmp/ciostream-0.0.1.post8125288576.tar.gz` & `tmp/ciostream-0.0.1.post8952132004.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciostream-0.0.1.post8125288576.tar", last modified: Sat Mar  2 20:37:30 2024, max compression
+gzip compressed data, was "ciostream-0.0.1.post8952132004.tar", last modified: Sat May  4 17:24:21 2024, max compression
```

## Comparing `ciostream-0.0.1.post8125288576.tar` & `ciostream-0.0.1.post8952132004.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 20:37:30.495489 ciostream-0.0.1.post8125288576/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-02 20:37:19.000000 ciostream-0.0.1.post8125288576/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-02 20:37:30.495489 ciostream-0.0.1.post8125288576/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-03-02 20:37:19.000000 ciostream-0.0.1.post8125288576/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-02 20:37:30.495489 ciostream-0.0.1.post8125288576/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-02 20:37:19.000000 ciostream-0.0.1.post8125288576/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 20:37:30.491489 ciostream-0.0.1.post8125288576/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 20:37:30.495489 ciostream-0.0.1.post8125288576/src/ciostream/
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-03-02 20:37:19.000000 ciostream-0.0.1.post8125288576/src/ciostream/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-02 20:37:19.000000 ciostream-0.0.1.post8125288576/src/ciostream/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-03-02 20:37:19.000000 ciostream-0.0.1.post8125288576/src/ciostream/__init__.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-03-02 20:37:19.000000 ciostream-0.0.1.post8125288576/src/ciostream/ciostream_native.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-03-02 20:37:19.000000 ciostream-0.0.1.post8125288576/src/ciostream/ciostream_native.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 20:37:30.495489 ciostream-0.0.1.post8125288576/src/ciostream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-02 20:37:30.000000 ciostream-0.0.1.post8125288576/src/ciostream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-02 20:37:30.000000 ciostream-0.0.1.post8125288576/src/ciostream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 20:37:30.000000 ciostream-0.0.1.post8125288576/src/ciostream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 20:37:30.000000 ciostream-0.0.1.post8125288576/src/ciostream.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-02 20:37:30.000000 ciostream-0.0.1.post8125288576/src/ciostream.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 20:37:30.495489 ciostream-0.0.1.post8125288576/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-03-02 20:37:19.000000 ciostream-0.0.1.post8125288576/tests/test_smoke.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:24:21.758458 ciostream-0.0.1.post8952132004/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-04 17:24:13.000000 ciostream-0.0.1.post8952132004/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-04 17:24:21.758458 ciostream-0.0.1.post8952132004/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-04 17:24:13.000000 ciostream-0.0.1.post8952132004/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 17:24:21.758458 ciostream-0.0.1.post8952132004/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-04 17:24:13.000000 ciostream-0.0.1.post8952132004/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:24:21.754458 ciostream-0.0.1.post8952132004/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:24:21.758458 ciostream-0.0.1.post8952132004/src/ciostream/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-04 17:24:13.000000 ciostream-0.0.1.post8952132004/src/ciostream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-04 17:24:13.000000 ciostream-0.0.1.post8952132004/src/ciostream/ciostream_native.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-04 17:24:13.000000 ciostream-0.0.1.post8952132004/src/ciostream/ciostream_native.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-04 17:24:13.000000 ciostream-0.0.1.post8952132004/src/ciostream/core.pxd
+-rwxr-xr-x   0 runner    (1001) docker     (127)   375336 2024-05-04 17:24:13.000000 ciostream-0.0.1.post8952132004/src/ciostream/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-04 17:24:13.000000 ciostream-0.0.1.post8952132004/src/ciostream/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-04 17:24:13.000000 ciostream-0.0.1.post8952132004/src/ciostream/core.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:24:21.758458 ciostream-0.0.1.post8952132004/src/ciostream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-04 17:24:21.000000 ciostream-0.0.1.post8952132004/src/ciostream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-04 17:24:21.000000 ciostream-0.0.1.post8952132004/src/ciostream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 17:24:21.000000 ciostream-0.0.1.post8952132004/src/ciostream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 17:24:21.000000 ciostream-0.0.1.post8952132004/src/ciostream.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-04 17:24:21.000000 ciostream-0.0.1.post8952132004/src/ciostream.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:24:21.758458 ciostream-0.0.1.post8952132004/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-04 17:24:13.000000 ciostream-0.0.1.post8952132004/tests/test_smoke.py
```

### Comparing `ciostream-0.0.1.post8125288576/LICENSE` & `ciostream-0.0.1.post8952132004/LICENSE`

 * *Files identical despite different names*

### Comparing `ciostream-0.0.1.post8125288576/README.md` & `ciostream-0.0.1.post8952132004/README.md`

 * *Files identical despite different names*

### Comparing `ciostream-0.0.1.post8125288576/setup.py` & `ciostream-0.0.1.post8952132004/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 version="0.0.1"
 
 if "GITHUB_RUN_ID" in os.environ:
     version += "-"
     version += os.environ["GITHUB_RUN_ID"]
 
 ext = Extension(
-    "ciostream",
+    "ciostream.core",
     sources=[
-        "src/ciostream/__init__.pyx",
+        "src/ciostream/core.pyx",
         "src/ciostream/ciostream_native.cpp"],
     language="c++")
 
 setup(
     name="ciostream",
     version=version,
     author="Matthew Ballance",
```

### Comparing `ciostream-0.0.1.post8125288576/src/ciostream/__init__.pxd` & `ciostream-0.0.1.post8952132004/src/ciostream/core.pxd`

 * *Files identical despite different names*

### Comparing `ciostream-0.0.1.post8125288576/src/ciostream/__init__.pyx` & `ciostream-0.0.1.post8952132004/src/ciostream/core.pyx`

 * *Files identical despite different names*

### Comparing `ciostream-0.0.1.post8125288576/src/ciostream/ciostream_native.cpp` & `ciostream-0.0.1.post8952132004/src/ciostream/ciostream_native.cpp`

 * *Files identical despite different names*

### Comparing `ciostream-0.0.1.post8125288576/src/ciostream/ciostream_native.h` & `ciostream-0.0.1.post8952132004/src/ciostream/ciostream_native.h`

 * *Files identical despite different names*

### Comparing `ciostream-0.0.1.post8125288576/tests/test_smoke.py` & `ciostream-0.0.1.post8952132004/tests/test_smoke.py`

 * *Files identical despite different names*

