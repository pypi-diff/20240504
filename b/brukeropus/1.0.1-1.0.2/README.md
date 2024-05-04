# Comparing `tmp/brukeropus-1.0.1.tar.gz` & `tmp/brukeropus-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brukeropus-1.0.1.tar", last modified: Fri May  3 17:08:30 2024, max compression
+gzip compressed data, was "brukeropus-1.0.2.tar", last modified: Sat May  4 18:07:30 2024, max compression
```

## Comparing `brukeropus-1.0.1.tar` & `brukeropus-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 17:08:30.255411 brukeropus-1.0.1/
--rw-rw-rw-   0        0        0     1087 2024-02-29 18:02:08.000000 brukeropus-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     5274 2024-05-03 17:08:30.255411 brukeropus-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4523 2024-05-03 14:26:32.000000 brukeropus-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 17:08:30.205406 brukeropus-1.0.1/brukeropus/
--rw-rw-rw-   0        0        0     2581 2024-05-03 13:47:15.000000 brukeropus-1.0.1/brukeropus/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 17:08:30.237688 brukeropus-1.0.1/brukeropus/control/
--rw-rw-rw-   0        0        0     1746 2024-04-24 01:13:04.000000 brukeropus-1.0.1/brukeropus/control/__init__.py
--rw-rw-rw-   0        0        0     9678 2024-04-23 16:48:27.000000 brukeropus-1.0.1/brukeropus/control/dde.py
--rw-rw-rw-   0        0        0    11639 2024-04-24 00:59:48.000000 brukeropus-1.0.1/brukeropus/control/opus.py
-drwxrwxrwx   0        0        0        0 2024-05-03 17:08:30.238895 brukeropus-1.0.1/brukeropus/file/
--rw-rw-rw-   0        0        0    17333 2024-04-23 18:20:14.000000 brukeropus-1.0.1/brukeropus/file/__init__.py
--rw-rw-rw-   0        0        0     9467 2024-03-05 15:18:18.000000 brukeropus-1.0.1/brukeropus/file/constants.py
--rw-rw-rw-   0        0        0    25809 2024-04-23 01:26:07.000000 brukeropus-1.0.1/brukeropus/file/file.py
--rw-rw-rw-   0        0        0    13119 2024-02-29 18:02:08.000000 brukeropus-1.0.1/brukeropus/file/parser.py
--rw-rw-rw-   0        0        0     9949 2024-02-29 18:02:08.000000 brukeropus-1.0.1/brukeropus/file/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-03 17:08:30.255411 brukeropus-1.0.1/brukeropus.egg-info/
--rw-rw-rw-   0        0        0     5274 2024-05-03 17:08:30.000000 brukeropus-1.0.1/brukeropus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      440 2024-05-03 17:08:30.000000 brukeropus-1.0.1/brukeropus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 17:08:30.000000 brukeropus-1.0.1/brukeropus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-03 17:08:30.000000 brukeropus-1.0.1/brukeropus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-03 17:08:30.000000 brukeropus-1.0.1/brukeropus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      816 2024-05-03 16:59:29.000000 brukeropus-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-03 17:08:30.255411 brukeropus-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-04 18:07:30.440015 brukeropus-1.0.2/
+-rw-rw-rw-   0        0        0     1087 2024-02-29 18:02:08.000000 brukeropus-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     5274 2024-05-04 18:07:30.440015 brukeropus-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4523 2024-05-03 14:26:32.000000 brukeropus-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 18:07:30.405367 brukeropus-1.0.2/brukeropus/
+-rw-rw-rw-   0        0        0     2581 2024-05-03 13:47:15.000000 brukeropus-1.0.2/brukeropus/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 18:07:30.424361 brukeropus-1.0.2/brukeropus/control/
+-rw-rw-rw-   0        0        0     1746 2024-04-24 01:13:04.000000 brukeropus-1.0.2/brukeropus/control/__init__.py
+-rw-rw-rw-   0        0        0     9678 2024-04-23 16:48:27.000000 brukeropus-1.0.2/brukeropus/control/dde.py
+-rw-rw-rw-   0        0        0    11639 2024-04-24 00:59:48.000000 brukeropus-1.0.2/brukeropus/control/opus.py
+drwxrwxrwx   0        0        0        0 2024-05-04 18:07:30.424361 brukeropus-1.0.2/brukeropus/file/
+-rw-rw-rw-   0        0        0    17333 2024-04-23 18:20:14.000000 brukeropus-1.0.2/brukeropus/file/__init__.py
+-rw-rw-rw-   0        0        0     9467 2024-03-05 15:18:18.000000 brukeropus-1.0.2/brukeropus/file/constants.py
+-rw-rw-rw-   0        0        0    25809 2024-04-23 01:26:07.000000 brukeropus-1.0.2/brukeropus/file/file.py
+-rw-rw-rw-   0        0        0    13119 2024-02-29 18:02:08.000000 brukeropus-1.0.2/brukeropus/file/parser.py
+-rw-rw-rw-   0        0        0     9949 2024-02-29 18:02:08.000000 brukeropus-1.0.2/brukeropus/file/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-04 18:07:30.440015 brukeropus-1.0.2/brukeropus.egg-info/
+-rw-rw-rw-   0        0        0     5274 2024-05-04 18:07:30.000000 brukeropus-1.0.2/brukeropus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2024-05-04 18:07:30.000000 brukeropus-1.0.2/brukeropus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 18:07:30.000000 brukeropus-1.0.2/brukeropus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-04 18:07:30.000000 brukeropus-1.0.2/brukeropus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-04 18:07:30.000000 brukeropus-1.0.2/brukeropus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      816 2024-05-04 18:02:25.000000 brukeropus-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-04 18:07:30.440015 brukeropus-1.0.2/setup.cfg
```

### Comparing `brukeropus-1.0.1/LICENSE` & `brukeropus-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.1/PKG-INFO` & `brukeropus-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brukeropus
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python package for communicating with Bruker OPUS spectroscopy software and reading its binary file format.
 Author-email: Josh Duran <josh.m.duran@gmail.com>
 Project-URL: Homepage, https://github.com/joshduran/brukeropus
 Project-URL: Issues, https://github.com/joshduran/brukeropus/issues
 Project-URL: Documentation, https://joshduran.github.io/brukeropus/brukeropus.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `brukeropus-1.0.1/README.md` & `brukeropus-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.1/brukeropus/__init__.py` & `brukeropus-1.0.2/brukeropus/__init__.py`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.1/brukeropus/control/__init__.py` & `brukeropus-1.0.2/brukeropus/control/__init__.py`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.1/brukeropus/control/dde.py` & `brukeropus-1.0.2/brukeropus/control/dde.py`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.1/brukeropus/control/opus.py` & `brukeropus-1.0.2/brukeropus/control/opus.py`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.1/brukeropus/file/__init__.py` & `brukeropus-1.0.2/brukeropus/file/__init__.py`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.1/brukeropus/file/constants.py` & `brukeropus-1.0.2/brukeropus/file/constants.py`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.1/brukeropus/file/file.py` & `brukeropus-1.0.2/brukeropus/file/file.py`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.1/brukeropus/file/parser.py` & `brukeropus-1.0.2/brukeropus/file/parser.py`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.1/brukeropus/file/utils.py` & `brukeropus-1.0.2/brukeropus/file/utils.py`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.1/brukeropus.egg-info/PKG-INFO` & `brukeropus-1.0.2/brukeropus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brukeropus
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python package for communicating with Bruker OPUS spectroscopy software and reading its binary file format.
 Author-email: Josh Duran <josh.m.duran@gmail.com>
 Project-URL: Homepage, https://github.com/joshduran/brukeropus
 Project-URL: Issues, https://github.com/joshduran/brukeropus/issues
 Project-URL: Documentation, https://joshduran.github.io/brukeropus/brukeropus.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `brukeropus-1.0.1/pyproject.toml` & `brukeropus-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "brukeropus"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Josh Duran", email="josh.m.duran@gmail.com" },
 ]
 description = "A python package for communicating with Bruker OPUS spectroscopy software and reading its binary file format."
 readme = "README.md"
 dependencies = ["numpy"]
 requires-python = ">=3.6"
```

