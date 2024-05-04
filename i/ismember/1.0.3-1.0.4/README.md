# Comparing `tmp/ismember-1.0.3.tar.gz` & `tmp/ismember-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ismember-1.0.3.tar", last modified: Sun Apr 21 08:23:37 2024, max compression
+gzip compressed data, was "ismember-1.0.4.tar", last modified: Sat May  4 08:46:02 2024, max compression
```

## Comparing `ismember-1.0.3.tar` & `ismember-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 08:23:37.335730 ismember-1.0.3/
--rw-rw-rw-   0        0        0     1121 2021-05-24 09:24:10.000000 ismember-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     3391 2024-04-21 08:23:37.335730 ismember-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2808 2024-04-21 08:19:28.000000 ismember-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 08:23:37.304476 ismember-1.0.3/ismember/
--rw-rw-rw-   0        0        0     1228 2024-04-21 08:21:41.000000 ismember-1.0.3/ismember/__init__.py
--rw-rw-rw-   0        0        0     3161 2022-03-07 20:24:34.000000 ismember-1.0.3/ismember/example.py
--rw-rw-rw-   0        0        0     4871 2024-04-21 08:19:28.000000 ismember-1.0.3/ismember/ismember.py
-drwxrwxrwx   0        0        0        0 2024-04-21 08:23:37.335730 ismember-1.0.3/ismember/tests/
--rw-rw-rw-   0        0        0        0 2021-01-28 13:20:53.000000 ismember-1.0.3/ismember/tests/__init__.py
--rw-rw-rw-   0        0        0     3322 2024-04-21 08:19:28.000000 ismember-1.0.3/ismember/tests/test_ismember.py
-drwxrwxrwx   0        0        0        0 2024-04-21 08:23:37.335730 ismember-1.0.3/ismember.egg-info/
--rw-rw-rw-   0        0        0     3391 2024-04-21 08:23:37.000000 ismember-1.0.3/ismember.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2024-04-21 08:23:37.000000 ismember-1.0.3/ismember.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 08:23:37.000000 ismember-1.0.3/ismember.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-21 08:23:37.000000 ismember-1.0.3/ismember.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-21 08:23:37.000000 ismember-1.0.3/ismember.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 08:23:37.335730 ismember-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1340 2024-04-21 08:21:38.000000 ismember-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 08:46:02.083670 ismember-1.0.4/
+-rw-rw-rw-   0        0        0     1121 2021-05-24 09:24:10.000000 ismember-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     3391 2024-05-04 08:46:02.083670 ismember-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2808 2024-04-21 08:19:28.000000 ismember-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 08:46:02.049402 ismember-1.0.4/ismember/
+-rw-rw-rw-   0        0        0     1239 2024-05-04 08:45:15.000000 ismember-1.0.4/ismember/__init__.py
+-rw-rw-rw-   0        0        0     3161 2022-03-07 20:24:34.000000 ismember-1.0.4/ismember/example.py
+-rw-rw-rw-   0        0        0     4871 2024-04-21 08:19:28.000000 ismember-1.0.4/ismember/ismember.py
+drwxrwxrwx   0        0        0        0 2024-05-04 08:46:02.082897 ismember-1.0.4/ismember/tests/
+-rw-rw-rw-   0        0        0        0 2021-01-28 13:20:53.000000 ismember-1.0.4/ismember/tests/__init__.py
+-rw-rw-rw-   0        0        0     3322 2024-04-21 08:19:28.000000 ismember-1.0.4/ismember/tests/test_ismember.py
+drwxrwxrwx   0        0        0        0 2024-05-04 08:46:02.068557 ismember-1.0.4/ismember.egg-info/
+-rw-rw-rw-   0        0        0     3391 2024-05-04 08:46:01.000000 ismember-1.0.4/ismember.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2024-05-04 08:46:01.000000 ismember-1.0.4/ismember.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 08:46:01.000000 ismember-1.0.4/ismember.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-04 08:46:01.000000 ismember-1.0.4/ismember.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-04 08:46:01.000000 ismember-1.0.4/ismember.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 08:46:02.083670 ismember-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1340 2024-04-21 08:21:38.000000 ismember-1.0.4/setup.py
```

### Comparing `ismember-1.0.3/LICENSE` & `ismember-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ismember-1.0.3/PKG-INFO` & `ismember-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ismember
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python package ismember returns array elements that are members of set array.
 Home-page: https://erdogant.github.io/ismember
-Download-URL: https://github.com/erdogant/ismember/archive/1.0.3.tar.gz
+Download-URL: https://github.com/erdogant/ismember/archive/1.0.4.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: ismember Version: 1.0.3 Summary: Python package
+Metadata-Version: 2.1 Name: ismember Version: 1.0.4 Summary: Python package
 ismember returns array elements that are members of set array. Home-page:
 https://erdogant.github.io/ismember Download-URL: https://github.com/erdogant/
-ismember/archive/1.0.3.tar.gz Author: Erdogan Taskesen Author-email:
+ismember/archive/1.0.4.tar.gz Author: Erdogan Taskesen Author-email:
 erdogant@gmail.com Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: numpy # ismember [![Python](https://
 img.shields.io/pypi/pyversions/ismember)](https://img.shields.io/pypi/
 pyversions/ismember) [![PyPI Version](https://img.shields.io/pypi/v/ismember)]
 (https://pypi.org/project/ismember/) ![GitHub Repo stars](https://
```

### Comparing `ismember-1.0.3/README.md` & `ismember-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ismember-1.0.3/ismember/__init__.py` & `ismember-1.0.4/ismember/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from ismember.ismember import ismember
+from ismember.ismember import ismember, is_row_in
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '1.0.3'
+__version__ = '1.0.4'
 
 # module level doc-string
 __doc__ = """
 ismember
 =====================================================================
 
 Description
```

### Comparing `ismember-1.0.3/ismember/example.py` & `ismember-1.0.4/ismember/example.py`

 * *Files identical despite different names*

### Comparing `ismember-1.0.3/ismember/ismember.py` & `ismember-1.0.4/ismember/ismember.py`

 * *Files identical despite different names*

### Comparing `ismember-1.0.3/ismember/tests/test_ismember.py` & `ismember-1.0.4/ismember/tests/test_ismember.py`

 * *Files identical despite different names*

### Comparing `ismember-1.0.3/ismember.egg-info/PKG-INFO` & `ismember-1.0.4/ismember.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ismember
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python package ismember returns array elements that are members of set array.
 Home-page: https://erdogant.github.io/ismember
-Download-URL: https://github.com/erdogant/ismember/archive/1.0.3.tar.gz
+Download-URL: https://github.com/erdogant/ismember/archive/1.0.4.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: ismember Version: 1.0.3 Summary: Python package
+Metadata-Version: 2.1 Name: ismember Version: 1.0.4 Summary: Python package
 ismember returns array elements that are members of set array. Home-page:
 https://erdogant.github.io/ismember Download-URL: https://github.com/erdogant/
-ismember/archive/1.0.3.tar.gz Author: Erdogan Taskesen Author-email:
+ismember/archive/1.0.4.tar.gz Author: Erdogan Taskesen Author-email:
 erdogant@gmail.com Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: numpy # ismember [![Python](https://
 img.shields.io/pypi/pyversions/ismember)](https://img.shields.io/pypi/
 pyversions/ismember) [![PyPI Version](https://img.shields.io/pypi/v/ismember)]
 (https://pypi.org/project/ismember/) ![GitHub Repo stars](https://
```

### Comparing `ismember-1.0.3/setup.py` & `ismember-1.0.4/setup.py`

 * *Files identical despite different names*

