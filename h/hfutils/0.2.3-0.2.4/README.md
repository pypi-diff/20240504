# Comparing `tmp/hfutils-0.2.3.tar.gz` & `tmp/hfutils-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hfutils-0.2.3.tar", last modified: Thu May  2 13:31:05 2024, max compression
+gzip compressed data, was "hfutils-0.2.4.tar", last modified: Sat May  4 18:52:47 2024, max compression
```

## Comparing `hfutils-0.2.3.tar` & `hfutils-0.2.4.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:31:05.633952 hfutils-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-02 13:30:45.000000 hfutils-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-02 13:30:45.000000 hfutils-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10149 2024-05-02 13:31:05.633952 hfutils-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-05-02 13:30:45.000000 hfutils-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:31:05.625952 hfutils-0.2.3/hfutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:31:05.625952 hfutils-0.2.3/hfutils/archive/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/archive/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/archive/rar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/archive/sevenz.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/archive/tar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/archive/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:31:05.625952 hfutils-0.2.3/hfutils/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:31:05.625952 hfutils-0.2.3/hfutils/entry/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/entry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/entry/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/entry/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/entry/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/entry/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/entry/ls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/entry/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/entry/whoami.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:31:05.625952 hfutils-0.2.3/hfutils/index/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/index/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/index/hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/index/make.py
--rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/index/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:31:05.629952 hfutils-0.2.3/hfutils/operate/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/operate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/operate/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/operate/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/operate/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/operate/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:31:05.629952 hfutils-0.2.3/hfutils/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/utils/binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/utils/temp.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/utils/tqdm_.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-02 13:30:45.000000 hfutils-0.2.3/hfutils/utils/walk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:31:05.629952 hfutils-0.2.3/hfutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10149 2024-05-02 13:31:05.000000 hfutils-0.2.3/hfutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-02 13:31:05.000000 hfutils-0.2.3/hfutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:31:05.000000 hfutils-0.2.3/hfutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-02 13:31:05.000000 hfutils-0.2.3/hfutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-02 13:31:05.000000 hfutils-0.2.3/hfutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 13:31:05.000000 hfutils-0.2.3/hfutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 13:30:45.000000 hfutils-0.2.3/requirements-7z.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-02 13:30:45.000000 hfutils-0.2.3/requirements-build.txt
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-02 13:30:45.000000 hfutils-0.2.3/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:30:45.000000 hfutils-0.2.3/requirements-rar.txt
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-02 13:30:45.000000 hfutils-0.2.3/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-02 13:30:45.000000 hfutils-0.2.3/requirements-transfer.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-02 13:30:45.000000 hfutils-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 13:31:05.633952 hfutils-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-02 13:30:45.000000 hfutils-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:47.085215 hfutils-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-04 18:52:24.000000 hfutils-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-04 18:52:24.000000 hfutils-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10149 2024-05-04 18:52:47.085215 hfutils-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-05-04 18:52:24.000000 hfutils-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:47.077216 hfutils-0.2.4/hfutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:47.077216 hfutils-0.2.4/hfutils/archive/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/archive/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/archive/rar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/archive/sevenz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/archive/tar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/archive/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:47.077216 hfutils-0.2.4/hfutils/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:47.081215 hfutils-0.2.4/hfutils/entry/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/entry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/entry/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/entry/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/entry/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/entry/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/entry/ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/entry/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/entry/whoami.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:47.081215 hfutils-0.2.4/hfutils/index/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/index/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/index/hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/index/make.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/index/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:47.081215 hfutils-0.2.4/hfutils/operate/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/operate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/operate/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/operate/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/operate/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/operate/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:47.081215 hfutils-0.2.4/hfutils/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/utils/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/utils/temp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/utils/tqdm_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-04 18:52:24.000000 hfutils-0.2.4/hfutils/utils/walk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:52:47.081215 hfutils-0.2.4/hfutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10149 2024-05-04 18:52:47.000000 hfutils-0.2.4/hfutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-04 18:52:47.000000 hfutils-0.2.4/hfutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 18:52:47.000000 hfutils-0.2.4/hfutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-04 18:52:47.000000 hfutils-0.2.4/hfutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-04 18:52:47.000000 hfutils-0.2.4/hfutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 18:52:47.000000 hfutils-0.2.4/hfutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-04 18:52:24.000000 hfutils-0.2.4/requirements-7z.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-04 18:52:24.000000 hfutils-0.2.4/requirements-build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-04 18:52:24.000000 hfutils-0.2.4/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-04 18:52:24.000000 hfutils-0.2.4/requirements-rar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-04 18:52:24.000000 hfutils-0.2.4/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 18:52:24.000000 hfutils-0.2.4/requirements-transfer.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-04 18:52:24.000000 hfutils-0.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 18:52:47.089216 hfutils-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-04 18:52:24.000000 hfutils-0.2.4/setup.py
```

### Comparing `hfutils-0.2.3/LICENSE` & `hfutils-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.3/PKG-INFO` & `hfutils-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfutils
-Version: 0.2.3
+Version: 0.2.4
 Summary: Useful utilities for huggingface
 Home-page: https://github.com/deepghs/hfutils
 Author: narugo1992
 Author-email: narugo992@gmail.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hfutils-0.2.3/README.md` & `hfutils-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.3/hfutils/archive/__init__.py` & `hfutils-0.2.4/hfutils/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.3/hfutils/archive/base.py` & `hfutils-0.2.4/hfutils/archive/base.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.3/hfutils/archive/rar.py` & `hfutils-0.2.4/hfutils/archive/rar.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.3/hfutils/archive/sevenz.py` & `hfutils-0.2.4/hfutils/archive/sevenz.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.3/hfutils/archive/tar.py` & `hfutils-0.2.4/hfutils/archive/tar.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.3/hfutils/archive/zip.py` & `hfutils-0.2.4/hfutils/archive/zip.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.3/hfutils/entry/base.py` & `hfutils-0.2.4/hfutils/entry/base.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.3/hfutils/entry/dispatch.py` & `hfutils-0.2.4/hfutils/entry/dispatch.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.3/hfutils/entry/download.py` & `hfutils-0.2.4/hfutils/entry/download.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.3/hfutils/entry/ls.py` & `hfutils-0.2.4/hfutils/entry/ls.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.3/hfutils/entry/upload.py` & `hfutils-0.2.4/hfutils/entry/upload.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.3/hfutils/entry/whoami.py` & `hfutils-0.2.4/hfutils/entry/whoami.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.3/hfutils/index/fetch.py` & `hfutils-0.2.4/hfutils/index/fetch.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.3/hfutils/index/hash.py` & `hfutils-0.2.4/hfutils/index/hash.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.3/hfutils/index/make.py` & `hfutils-0.2.4/hfutils/index/make.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.3/hfutils/index/validate.py` & `hfutils-0.2.4/hfutils/index/validate.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.3/hfutils/operate/base.py` & `hfutils-0.2.4/hfutils/operate/base.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.3/hfutils/operate/download.py` & `hfutils-0.2.4/hfutils/operate/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import List, Optional
 
 import requests.exceptions
 
 from .base import RepoTypeTyping, list_files_in_repository, _IGNORE_PATTERN_UNSET, get_hf_client
 from .validate import is_local_file_ready
 from ..archive import archive_unpack
-from ..utils import tqdm, TemporaryDirectory
+from ..utils import tqdm, TemporaryDirectory, hf_normpath
 
 
 def download_file_to_file(local_file: str, repo_id: str, file_in_repo: str,
                           repo_type: RepoTypeTyping = 'dataset', revision: str = 'main',
                           resume_download: bool = True, hf_token: Optional[str] = None):
     """
     Download a file from a Hugging Face repository and save it to a local file.
@@ -37,15 +37,15 @@
     relative_filename = os.path.join(*file_in_repo.split("/"))
     with TemporaryDirectory() as td:
         temp_path = os.path.join(td, relative_filename)
         try:
             hf_client.hf_hub_download(
                 repo_id=repo_id,
                 repo_type=repo_type,
-                filename=file_in_repo,
+                filename=hf_normpath(file_in_repo),
                 revision=revision,
                 local_dir=td,
                 force_download=True,
                 local_dir_use_symlinks=False,
                 resume_download=resume_download,
             )
         finally:
@@ -116,31 +116,32 @@
     files = list_files_in_repository(repo_id, repo_type, dir_in_repo, revision, ignore_patterns, hf_token=hf_token)
     progress = tqdm(files, silent=silent, desc=f'Downloading {dir_in_repo!r} ...')
 
     def _download_one_file(rel_file):
         current_resume_download = resume_download
         try:
             dst_file = os.path.join(local_directory, rel_file)
+            file_in_repo = hf_normpath(f'{dir_in_repo}/{rel_file}')
             if os.path.exists(dst_file) and is_local_file_ready(
                     repo_id=repo_id,
                     repo_type=repo_type,
                     local_file=dst_file,
-                    file_in_repo=f'{dir_in_repo}/{rel_file}',
+                    file_in_repo=file_in_repo,
                     revision=revision,
                     hf_token=hf_token,
             ):
                 logging.info(f'Local file {rel_file} is ready, download skipped.')
             else:
                 tries = 0
                 while True:
                     try:
                         download_file_to_file(
                             local_file=dst_file,
                             repo_id=repo_id,
-                            file_in_repo=f'{dir_in_repo}/{rel_file}',
+                            file_in_repo=file_in_repo,
                             repo_type=repo_type,
                             revision=revision,
                             resume_download=current_resume_download,
                             hf_token=hf_token,
                         )
                     except requests.exceptions.RequestException as err:
                         if tries < max_retries:
```

### Comparing `hfutils-0.2.3/hfutils/operate/upload.py` & `hfutils-0.2.4/hfutils/operate/upload.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.3/hfutils/operate/validate.py` & `hfutils-0.2.4/hfutils/operate/validate.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.3/hfutils/utils/binary.py` & `hfutils-0.2.4/hfutils/utils/binary.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.3/hfutils/utils/download.py` & `hfutils-0.2.4/hfutils/utils/download.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.3/hfutils/utils/temp.py` & `hfutils-0.2.4/hfutils/utils/temp.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.3/hfutils/utils/tqdm_.py` & `hfutils-0.2.4/hfutils/utils/tqdm_.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.3/hfutils/utils/walk.py` & `hfutils-0.2.4/hfutils/utils/walk.py`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.3/hfutils.egg-info/PKG-INFO` & `hfutils-0.2.4/hfutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfutils
-Version: 0.2.3
+Version: 0.2.4
 Summary: Useful utilities for huggingface
 Home-page: https://github.com/deepghs/hfutils
 Author: narugo1992
 Author-email: narugo992@gmail.com
 License: Apache License, Version 2.0
 Keywords: Utilities of images.
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hfutils-0.2.3/hfutils.egg-info/SOURCES.txt` & `hfutils-0.2.4/hfutils.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -41,10 +41,11 @@
 hfutils/operate/base.py
 hfutils/operate/download.py
 hfutils/operate/upload.py
 hfutils/operate/validate.py
 hfutils/utils/__init__.py
 hfutils/utils/binary.py
 hfutils/utils/download.py
+hfutils/utils/path.py
 hfutils/utils/temp.py
 hfutils/utils/tqdm_.py
 hfutils/utils/walk.py
```

### Comparing `hfutils-0.2.3/hfutils.egg-info/requires.txt` & `hfutils-0.2.4/hfutils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hfutils-0.2.3/setup.py` & `hfutils-0.2.4/setup.py`

 * *Files identical despite different names*

