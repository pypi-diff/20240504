# Comparing `tmp/sqlclasses-1.0.tar.gz` & `tmp/sqlclasses-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlclasses-1.0.tar", last modified: Sun Apr 28 20:39:48 2024, max compression
+gzip compressed data, was "sqlclasses-1.1.tar", last modified: Sat May  4 16:35:14 2024, max compression
```

## Comparing `sqlclasses-1.0.tar` & `sqlclasses-1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 diedrich  (1001) staff       (20)        0 2024-04-28 20:39:48.215792 sqlclasses-1.0/
--rw-r--r--   0 diedrich  (1001) staff       (20)    35149 2024-04-28 20:14:39.000000 sqlclasses-1.0/LICENSE
--rw-r--r--   0 diedrich  (1001) staff       (20)     1175 2024-04-28 20:39:48.215454 sqlclasses-1.0/PKG-INFO
--rw-r--r--   0 diedrich  (1001) staff       (20)      690 2024-04-28 20:38:42.000000 sqlclasses-1.0/README.md
--rw-r--r--   0 diedrich  (1001) staff       (20)       38 2024-04-28 20:39:48.215860 sqlclasses-1.0/setup.cfg
--rwxr-xr-x   0 diedrich  (1001) staff       (20)      758 2024-04-28 20:38:06.000000 sqlclasses-1.0/setup.py
-drwxr-xr-x   0 diedrich  (1001) staff       (20)        0 2024-04-28 20:39:48.213174 sqlclasses-1.0/sqlclasses/
--rw-r--r--   0 diedrich  (1001) staff       (20)        7 2024-04-28 20:28:07.000000 sqlclasses-1.0/sqlclasses/__init__.py
--rw-r--r--   0 diedrich  (1001) staff       (20)    21684 2024-04-28 20:20:37.000000 sqlclasses-1.0/sqlclasses/sql.py
-drwxr-xr-x   0 diedrich  (1001) staff       (20)        0 2024-04-28 20:39:48.215135 sqlclasses-1.0/sqlclasses.egg-info/
--rw-r--r--   0 diedrich  (1001) staff       (20)     1175 2024-04-28 20:39:48.000000 sqlclasses-1.0/sqlclasses.egg-info/PKG-INFO
--rw-r--r--   0 diedrich  (1001) staff       (20)      203 2024-04-28 20:39:48.000000 sqlclasses-1.0/sqlclasses.egg-info/SOURCES.txt
--rw-r--r--   0 diedrich  (1001) staff       (20)        1 2024-04-28 20:39:48.000000 sqlclasses-1.0/sqlclasses.egg-info/dependency_links.txt
--rw-r--r--   0 diedrich  (1001) staff       (20)       11 2024-04-28 20:39:48.000000 sqlclasses-1.0/sqlclasses.egg-info/top_level.txt
+drwxr-xr-x   0 diedrich  (1001) staff       (20)        0 2024-05-04 16:35:14.660620 sqlclasses-1.1/
+-rw-r--r--   0 diedrich  (1001) staff       (20)    35149 2024-04-28 20:14:39.000000 sqlclasses-1.1/LICENSE
+-rw-r--r--   0 diedrich  (1001) staff       (20)     1175 2024-05-04 16:35:14.660239 sqlclasses-1.1/PKG-INFO
+-rw-r--r--   0 diedrich  (1001) staff       (20)      690 2024-04-28 20:38:42.000000 sqlclasses-1.1/README.md
+-rw-r--r--   0 diedrich  (1001) staff       (20)       38 2024-05-04 16:35:14.660697 sqlclasses-1.1/setup.cfg
+-rwxr-xr-x   0 diedrich  (1001) staff       (20)      758 2024-05-04 16:34:21.000000 sqlclasses-1.1/setup.py
+drwxr-xr-x   0 diedrich  (1001) staff       (20)        0 2024-05-04 16:35:14.658572 sqlclasses-1.1/sqlclasses/
+-rw-r--r--   0 diedrich  (1001) staff       (20)        7 2024-04-28 20:28:07.000000 sqlclasses-1.1/sqlclasses/__init__.py
+-rw-r--r--   0 diedrich  (1001) staff       (20)    22000 2024-05-02 17:30:44.000000 sqlclasses-1.1/sqlclasses/sql.py
+drwxr-xr-x   0 diedrich  (1001) staff       (20)        0 2024-05-04 16:35:14.659922 sqlclasses-1.1/sqlclasses.egg-info/
+-rw-r--r--   0 diedrich  (1001) staff       (20)     1175 2024-05-04 16:35:14.000000 sqlclasses-1.1/sqlclasses.egg-info/PKG-INFO
+-rw-r--r--   0 diedrich  (1001) staff       (20)      203 2024-05-04 16:35:14.000000 sqlclasses-1.1/sqlclasses.egg-info/SOURCES.txt
+-rw-r--r--   0 diedrich  (1001) staff       (20)        1 2024-05-04 16:35:14.000000 sqlclasses-1.1/sqlclasses.egg-info/dependency_links.txt
+-rw-r--r--   0 diedrich  (1001) staff       (20)       11 2024-05-04 16:35:14.000000 sqlclasses-1.1/sqlclasses.egg-info/top_level.txt
```

### Comparing `sqlclasses-1.0/LICENSE` & `sqlclasses-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlclasses-1.0/PKG-INFO` & `sqlclasses-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlclasses
-Version: 1.0
+Version: 1.1
 Summary: Construct SQL commands and queries using Python classes.
 Home-page: https://github.com/dvorberg/sqlclasses
 Author: Diedrich Vorberg
 Author-email: diedrich@tux4web.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `sqlclasses-1.0/README.md` & `sqlclasses-1.1/README.md`

 * *Files identical despite different names*

### Comparing `sqlclasses-1.0/setup.py` & `sqlclasses-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sqlclasses",
-    version="1.0",
+    version="1.1",
     author="Diedrich Vorberg",
     author_email="diedrich@tux4web.de",
     description="Construct SQL commands and queries using Python classes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dvorberg/sqlclasses",
```

### Comparing `sqlclasses-1.0/sqlclasses/sql.py` & `sqlclasses-1.1/sqlclasses/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -766,14 +766,23 @@
         self._relation = relation
         self._columns = columns
         self._values = values
 
         if len(values) == 0:
             raise ValueError("You must supply values to an insert statement")
 
+    @classmethod
+    def from_dict(insert, relation, *dicts):
+        """
+        Construct an INSERT command using the (first) dicts’ keys
+        as column names and expecting the following dicts to provide
+        data for each column.
+        """
+        return insert(relation, list(dicts[0].keys()), dicts)
+
     def sql(self):
         relation = self._relation
 
         ret = ["INSERT INTO ", self._relation,]
 
         if self._columns:
             ret += [ "(", comma_separated(self._columns), ")", ]
```

### Comparing `sqlclasses-1.0/sqlclasses.egg-info/PKG-INFO` & `sqlclasses-1.1/sqlclasses.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlclasses
-Version: 1.0
+Version: 1.1
 Summary: Construct SQL commands and queries using Python classes.
 Home-page: https://github.com/dvorberg/sqlclasses
 Author: Diedrich Vorberg
 Author-email: diedrich@tux4web.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

