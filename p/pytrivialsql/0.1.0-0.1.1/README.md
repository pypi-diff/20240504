# Comparing `tmp/pytrivialsql-0.1.0.tar.gz` & `tmp/pytrivialsql-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrivialsql-0.1.0.tar", last modified: Fri May  3 19:49:59 2024, max compression
+gzip compressed data, was "pytrivialsql-0.1.1.tar", last modified: Fri May  3 20:46:16 2024, max compression
```

## Comparing `pytrivialsql-0.1.0.tar` & `pytrivialsql-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:49:59.367769 pytrivialsql-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-03 19:49:55.000000 pytrivialsql-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-03 19:49:59.367769 pytrivialsql-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-03 19:49:55.000000 pytrivialsql-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-03 19:49:55.000000 pytrivialsql-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 19:49:59.367769 pytrivialsql-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:49:59.363769 pytrivialsql-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:49:59.367769 pytrivialsql-0.1.0/src/pytrivialsql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:49:55.000000 pytrivialsql-0.1.0/src/pytrivialsql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-03 19:49:55.000000 pytrivialsql-0.1.0/src/pytrivialsql/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-05-03 19:49:55.000000 pytrivialsql-0.1.0/src/pytrivialsql/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-05-03 19:49:55.000000 pytrivialsql-0.1.0/src/pytrivialsql/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:49:59.367769 pytrivialsql-0.1.0/src/pytrivialsql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-03 19:49:59.000000 pytrivialsql-0.1.0/src/pytrivialsql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-03 19:49:59.000000 pytrivialsql-0.1.0/src/pytrivialsql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:49:59.000000 pytrivialsql-0.1.0/src/pytrivialsql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-03 19:49:59.000000 pytrivialsql-0.1.0/src/pytrivialsql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 19:49:59.000000 pytrivialsql-0.1.0/src/pytrivialsql.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:49:59.367769 pytrivialsql-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7369 2024-05-03 19:49:55.000000 pytrivialsql-0.1.0/tests/test_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-03 19:49:55.000000 pytrivialsql-0.1.0/tests/test_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:46:16.315246 pytrivialsql-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-03 20:46:11.000000 pytrivialsql-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-03 20:46:16.315246 pytrivialsql-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-03 20:46:11.000000 pytrivialsql-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-03 20:46:11.000000 pytrivialsql-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 20:46:16.315246 pytrivialsql-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:46:16.311246 pytrivialsql-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:46:16.315246 pytrivialsql-0.1.1/src/pytrivialsql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 20:46:11.000000 pytrivialsql-0.1.1/src/pytrivialsql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-03 20:46:11.000000 pytrivialsql-0.1.1/src/pytrivialsql/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-05-03 20:46:11.000000 pytrivialsql-0.1.1/src/pytrivialsql/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-05-03 20:46:11.000000 pytrivialsql-0.1.1/src/pytrivialsql/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:46:16.315246 pytrivialsql-0.1.1/src/pytrivialsql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-03 20:46:16.000000 pytrivialsql-0.1.1/src/pytrivialsql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-03 20:46:16.000000 pytrivialsql-0.1.1/src/pytrivialsql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:46:16.000000 pytrivialsql-0.1.1/src/pytrivialsql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-03 20:46:16.000000 pytrivialsql-0.1.1/src/pytrivialsql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 20:46:16.000000 pytrivialsql-0.1.1/src/pytrivialsql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:46:16.315246 pytrivialsql-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7369 2024-05-03 20:46:11.000000 pytrivialsql-0.1.1/tests/test_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-03 20:46:11.000000 pytrivialsql-0.1.1/tests/test_sqlite.py
```

### Comparing `pytrivialsql-0.1.0/LICENSE` & `pytrivialsql-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrivialsql-0.1.0/PKG-INFO` & `pytrivialsql-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrivialsql
-Version: 0.1.0
+Version: 0.1.1
 Summary: A trivial set of QOL bindings for SQL in Python
 Author-email: inaimathi <leo.zovic@gmail.com>
 Project-URL: Homepage, https://github.com/inaimathi/pytrivialsql
 Project-URL: Issues, https://github.com/inaimathi/pytrivialsql/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pytrivialsql-0.1.0/pyproject.toml` & `pytrivialsql-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytrivialsql"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="inaimathi", email="leo.zovic@gmail.com" },
 ]
 description = "A trivial set of QOL bindings for SQL in Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pytrivialsql-0.1.0/src/pytrivialsql/postgres.py` & `pytrivialsql-0.1.1/src/pytrivialsql/postgres.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,19 @@
         try:
             with self._conn.cursor() as cur:
                 if columns is None:
                     columns = "*"
                 if isinstance(columns, str):
                     columns = [columns]
                 query, args = sql.select_q(
-                    table_name, columns, where=where, order_by=order_by
+                    table_name,
+                    columns,
+                    where=where,
+                    order_by=order_by,
+                    placeholder="%s",
                 )
                 cur.execute(query, args)
                 cols = [col.name for col in cur.description]
                 res = (dict(zip(cols, vals)) for vals in cur.fetchall())
                 if transform is not None:
                     return [transform(el) for el in res]
                 return list(res)
```

### Comparing `pytrivialsql-0.1.0/src/pytrivialsql/sql.py` & `pytrivialsql-0.1.1/src/pytrivialsql/sql.py`

 * *Files identical despite different names*

### Comparing `pytrivialsql-0.1.0/src/pytrivialsql/sqlite.py` & `pytrivialsql-0.1.1/src/pytrivialsql/sqlite.py`

 * *Files identical despite different names*

### Comparing `pytrivialsql-0.1.0/src/pytrivialsql.egg-info/PKG-INFO` & `pytrivialsql-0.1.1/src/pytrivialsql.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrivialsql
-Version: 0.1.0
+Version: 0.1.1
 Summary: A trivial set of QOL bindings for SQL in Python
 Author-email: inaimathi <leo.zovic@gmail.com>
 Project-URL: Homepage, https://github.com/inaimathi/pytrivialsql
 Project-URL: Issues, https://github.com/inaimathi/pytrivialsql/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pytrivialsql-0.1.0/tests/test_sql.py` & `pytrivialsql-0.1.1/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `pytrivialsql-0.1.0/tests/test_sqlite.py` & `pytrivialsql-0.1.1/tests/test_sqlite.py`

 * *Files identical despite different names*

