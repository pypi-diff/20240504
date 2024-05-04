# Comparing `tmp/pytrivialsql-0.1.2.tar.gz` & `tmp/pytrivialsql-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrivialsql-0.1.2.tar", last modified: Sat May  4 00:56:33 2024, max compression
+gzip compressed data, was "pytrivialsql-0.1.3.tar", last modified: Sat May  4 03:26:03 2024, max compression
```

## Comparing `pytrivialsql-0.1.2.tar` & `pytrivialsql-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:56:33.442072 pytrivialsql-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-04 00:56:13.000000 pytrivialsql-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-04 00:56:33.442072 pytrivialsql-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-04 00:56:13.000000 pytrivialsql-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-04 00:56:13.000000 pytrivialsql-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 00:56:33.442072 pytrivialsql-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:56:33.438072 pytrivialsql-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:56:33.442072 pytrivialsql-0.1.2/src/pytrivialsql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:56:13.000000 pytrivialsql-0.1.2/src/pytrivialsql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-05-04 00:56:13.000000 pytrivialsql-0.1.2/src/pytrivialsql/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-05-04 00:56:13.000000 pytrivialsql-0.1.2/src/pytrivialsql/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-04 00:56:13.000000 pytrivialsql-0.1.2/src/pytrivialsql/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:56:33.442072 pytrivialsql-0.1.2/src/pytrivialsql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-04 00:56:33.000000 pytrivialsql-0.1.2/src/pytrivialsql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-04 00:56:33.000000 pytrivialsql-0.1.2/src/pytrivialsql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 00:56:33.000000 pytrivialsql-0.1.2/src/pytrivialsql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-04 00:56:33.000000 pytrivialsql-0.1.2/src/pytrivialsql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-04 00:56:33.000000 pytrivialsql-0.1.2/src/pytrivialsql.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:56:33.442072 pytrivialsql-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-04 00:56:13.000000 pytrivialsql-0.1.2/tests/test_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     7369 2024-05-04 00:56:13.000000 pytrivialsql-0.1.2/tests/test_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-04 00:56:13.000000 pytrivialsql-0.1.2/tests/test_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:26:03.396720 pytrivialsql-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-04 03:25:47.000000 pytrivialsql-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-04 03:26:03.396720 pytrivialsql-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-04 03:25:47.000000 pytrivialsql-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-04 03:25:47.000000 pytrivialsql-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 03:26:03.396720 pytrivialsql-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:26:03.392720 pytrivialsql-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:26:03.392720 pytrivialsql-0.1.3/src/pytrivialsql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:25:47.000000 pytrivialsql-0.1.3/src/pytrivialsql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-05-04 03:25:47.000000 pytrivialsql-0.1.3/src/pytrivialsql/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-05-04 03:25:47.000000 pytrivialsql-0.1.3/src/pytrivialsql/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-05-04 03:25:47.000000 pytrivialsql-0.1.3/src/pytrivialsql/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:26:03.396720 pytrivialsql-0.1.3/src/pytrivialsql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-04 03:26:03.000000 pytrivialsql-0.1.3/src/pytrivialsql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-04 03:26:03.000000 pytrivialsql-0.1.3/src/pytrivialsql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 03:26:03.000000 pytrivialsql-0.1.3/src/pytrivialsql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-04 03:26:03.000000 pytrivialsql-0.1.3/src/pytrivialsql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-04 03:26:03.000000 pytrivialsql-0.1.3/src/pytrivialsql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:26:03.396720 pytrivialsql-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-04 03:25:47.000000 pytrivialsql-0.1.3/tests/test_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7369 2024-05-04 03:25:47.000000 pytrivialsql-0.1.3/tests/test_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-04 03:25:47.000000 pytrivialsql-0.1.3/tests/test_sqlite.py
```

### Comparing `pytrivialsql-0.1.2/LICENSE` & `pytrivialsql-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrivialsql-0.1.2/PKG-INFO` & `pytrivialsql-0.1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrivialsql
-Version: 0.1.2
+Version: 0.1.3
 Summary: A trivial set of QOL bindings for SQL in Python
 Author-email: inaimathi <leo.zovic@gmail.com>
 Project-URL: Homepage, https://github.com/inaimathi/pytrivialsql
 Project-URL: Issues, https://github.com/inaimathi/pytrivialsql/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pytrivialsql-0.1.2/pyproject.toml` & `pytrivialsql-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytrivialsql"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="inaimathi", email="leo.zovic@gmail.com" },
 ]
 description = "A trivial set of QOL bindings for SQL in Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pytrivialsql-0.1.2/src/pytrivialsql/postgres.py` & `pytrivialsql-0.1.3/src/pytrivialsql/postgres.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,14 +21,33 @@
     def _reconnect(self):
         self.close()
         self._connect()
 
     def close(self):
         self._conn.close()
 
+    def exec(self, query, args=None):
+        try:
+            with self._conn.cursor() as cur:
+                cur.execute(query, args)
+            self._commit()
+        except Exception as e:
+            self._reconnect()
+            raise e
+
+    def execs(self, query_args_pairs):
+        try:
+            with self._conn.cursor() as cur:
+                for q, qargs in query_args_pairs:
+                    cur.execute(q, qargs)
+            self._commit()
+        except Exception as e:
+            self._reconnect()
+            raise e
+
     def drop(self, *table_names):
         try:
             with self._conn.cursor() as cur:
                 for tbl in table_names:
                     cur.execute(sql.drop_q(tbl))
             self._commit()
         except Exception as e:
```

### Comparing `pytrivialsql-0.1.2/src/pytrivialsql/sql.py` & `pytrivialsql-0.1.3/src/pytrivialsql/sql.py`

 * *Files identical despite different names*

### Comparing `pytrivialsql-0.1.2/src/pytrivialsql/sqlite.py` & `pytrivialsql-0.1.3/src/pytrivialsql/sqlite.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,23 @@
 class Sqlite3:
     def __init__(self, db_path):
         self.path = db_path
         self._conn = sqlite3.connect(
             self.path, check_same_thread=not self.is_threadsafe()
         )
 
+    def exec(self, query, args=None):
+        with self._conn as cur:
+            cur.execute(query, args)
+
+    def execs(self, query_args_pairs):
+        with self._conn as cur:
+            for q, qargs in query_args_pairs:
+                cur.execute(q, qargs)
+
     def is_threadsafe(self):
         mem = sqlite3.connect("file::memory:?cache=shared")
         cur = mem.execute(
             "select * from pragma_compile_options where compile_options like 'THREADSAFE=%'"
         )
         res = cur.fetchall()
         cur.close()
```

### Comparing `pytrivialsql-0.1.2/src/pytrivialsql.egg-info/PKG-INFO` & `pytrivialsql-0.1.3/src/pytrivialsql.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrivialsql
-Version: 0.1.2
+Version: 0.1.3
 Summary: A trivial set of QOL bindings for SQL in Python
 Author-email: inaimathi <leo.zovic@gmail.com>
 Project-URL: Homepage, https://github.com/inaimathi/pytrivialsql
 Project-URL: Issues, https://github.com/inaimathi/pytrivialsql/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pytrivialsql-0.1.2/tests/test_postgres.py` & `pytrivialsql-0.1.3/tests/test_postgres.py`

 * *Files identical despite different names*

### Comparing `pytrivialsql-0.1.2/tests/test_sql.py` & `pytrivialsql-0.1.3/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `pytrivialsql-0.1.2/tests/test_sqlite.py` & `pytrivialsql-0.1.3/tests/test_sqlite.py`

 * *Files identical despite different names*

