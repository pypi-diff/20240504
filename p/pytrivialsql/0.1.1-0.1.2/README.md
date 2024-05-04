# Comparing `tmp/pytrivialsql-0.1.1.tar.gz` & `tmp/pytrivialsql-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrivialsql-0.1.1.tar", last modified: Fri May  3 20:46:16 2024, max compression
+gzip compressed data, was "pytrivialsql-0.1.2.tar", last modified: Sat May  4 00:56:33 2024, max compression
```

## Comparing `pytrivialsql-0.1.1.tar` & `pytrivialsql-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:46:16.315246 pytrivialsql-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-03 20:46:11.000000 pytrivialsql-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-03 20:46:16.315246 pytrivialsql-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-03 20:46:11.000000 pytrivialsql-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-03 20:46:11.000000 pytrivialsql-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 20:46:16.315246 pytrivialsql-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:46:16.311246 pytrivialsql-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:46:16.315246 pytrivialsql-0.1.1/src/pytrivialsql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 20:46:11.000000 pytrivialsql-0.1.1/src/pytrivialsql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-03 20:46:11.000000 pytrivialsql-0.1.1/src/pytrivialsql/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-05-03 20:46:11.000000 pytrivialsql-0.1.1/src/pytrivialsql/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-05-03 20:46:11.000000 pytrivialsql-0.1.1/src/pytrivialsql/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:46:16.315246 pytrivialsql-0.1.1/src/pytrivialsql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-03 20:46:16.000000 pytrivialsql-0.1.1/src/pytrivialsql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-03 20:46:16.000000 pytrivialsql-0.1.1/src/pytrivialsql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:46:16.000000 pytrivialsql-0.1.1/src/pytrivialsql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-03 20:46:16.000000 pytrivialsql-0.1.1/src/pytrivialsql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 20:46:16.000000 pytrivialsql-0.1.1/src/pytrivialsql.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:46:16.315246 pytrivialsql-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7369 2024-05-03 20:46:11.000000 pytrivialsql-0.1.1/tests/test_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-03 20:46:11.000000 pytrivialsql-0.1.1/tests/test_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:56:33.442072 pytrivialsql-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-04 00:56:13.000000 pytrivialsql-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-04 00:56:33.442072 pytrivialsql-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-04 00:56:13.000000 pytrivialsql-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-04 00:56:13.000000 pytrivialsql-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 00:56:33.442072 pytrivialsql-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:56:33.438072 pytrivialsql-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:56:33.442072 pytrivialsql-0.1.2/src/pytrivialsql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:56:13.000000 pytrivialsql-0.1.2/src/pytrivialsql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-05-04 00:56:13.000000 pytrivialsql-0.1.2/src/pytrivialsql/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-05-04 00:56:13.000000 pytrivialsql-0.1.2/src/pytrivialsql/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-04 00:56:13.000000 pytrivialsql-0.1.2/src/pytrivialsql/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:56:33.442072 pytrivialsql-0.1.2/src/pytrivialsql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-04 00:56:33.000000 pytrivialsql-0.1.2/src/pytrivialsql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-04 00:56:33.000000 pytrivialsql-0.1.2/src/pytrivialsql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 00:56:33.000000 pytrivialsql-0.1.2/src/pytrivialsql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-04 00:56:33.000000 pytrivialsql-0.1.2/src/pytrivialsql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-04 00:56:33.000000 pytrivialsql-0.1.2/src/pytrivialsql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:56:33.442072 pytrivialsql-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-04 00:56:13.000000 pytrivialsql-0.1.2/tests/test_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7369 2024-05-04 00:56:13.000000 pytrivialsql-0.1.2/tests/test_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-04 00:56:13.000000 pytrivialsql-0.1.2/tests/test_sqlite.py
```

### Comparing `pytrivialsql-0.1.1/LICENSE` & `pytrivialsql-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrivialsql-0.1.1/PKG-INFO` & `pytrivialsql-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrivialsql
-Version: 0.1.1
+Version: 0.1.2
 Summary: A trivial set of QOL bindings for SQL in Python
 Author-email: inaimathi <leo.zovic@gmail.com>
 Project-URL: Homepage, https://github.com/inaimathi/pytrivialsql
 Project-URL: Issues, https://github.com/inaimathi/pytrivialsql/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pytrivialsql-0.1.1/pyproject.toml` & `pytrivialsql-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytrivialsql"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="inaimathi", email="leo.zovic@gmail.com" },
 ]
 description = "A trivial set of QOL bindings for SQL in Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pytrivialsql-0.1.1/src/pytrivialsql/postgres.py` & `pytrivialsql-0.1.2/src/pytrivialsql/postgres.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,49 @@
+import json
+
 import psycopg
 
 from . import sql
 
+_JSON_TYPES = {list, dict}
+
 
 class Postgres:
     def __init__(self, db_url):
         self._url = db_url
         self._connect()
 
     def _commit(self):
         self._conn.commit()
 
     def _connect(self):
         self._conn = psycopg.connect(self._url)
 
     def _reconnect(self):
-        self._close()
+        self.close()
         self._connect()
 
-    def _close(self):
+    def close(self):
         self._conn.close()
 
     def drop(self, *table_names):
         try:
             with self._conn.cursor() as cur:
                 for tbl in table_names:
-                    cur.execute(f'DROP TABLE "{tbl}"')
+                    cur.execute(sql.drop_q(tbl))
             self._commit()
         except Exception as e:
             self._reconnect()
             raise e
 
     def create(self, table_name, props):
-        try:
-            with self._conn.cursor() as cur:
-                cur.execute(sql.create_q(table_name, props))
+        with self._conn.cursor() as cur:
+            cur.execute(sql.create_q(table_name, props))
             self._commit()
             return True
-        except Exception:
-            return False
 
     def select(self, table_name, columns, where=None, order_by=None, transform=None):
         try:
             with self._conn.cursor() as cur:
                 if columns is None:
                     columns = "*"
                 if isinstance(columns, str):
@@ -61,17 +62,24 @@
                     return [transform(el) for el in res]
                 return list(res)
         except Exception as e:
             self._reconnect()
             raise e
 
     def insert(self, table_name, **args):
+        global _JSON_TYPES
         returning = args.get("returning", args.get("RETURNING", None))
         try:
             with self._conn.cursor() as cur:
+                for k, v in args.items():
+                    if k in {"returning", "RETURNING"}:
+                        if type(v) is str:
+                            args[k] = [v]
+                    if type(v) in _JSON_TYPES:
+                        args[k] = json.dumps(v)
                 args["placeholder"] = "%s"
                 q, qargs = sql.insert_q(table_name, **args)
                 cur.execute(q, qargs)
                 if returning is None:
                     res = None
                 else:
                     res = cur.fetchone()
@@ -83,18 +91,22 @@
             self._commit()
             return res
         except Exception as e:
             self._reconnect()
             raise e
 
     def update(self, table_name, bindings, where):
+        global _JSON_TYPES
+        binds = {"placeholder": "%s", **bindings}
         try:
             with self._conn.cursor() as cur:
-                bindings["placeholder"] = "%s"
-                q, args = sql.update_q(table_name, where=where, **bindings)
+                for k, v in binds.items():
+                    if type(v) in _JSON_TYPES:
+                        binds[k] = json.dumps(v)
+                q, args = sql.update_q(table_name, where=where, **binds)
                 cur.execute(q, args)
             self._commit()
         except Exception as e:
             self._reconnect()
             raise e
 
     def delete(self, table_name, where):
```

### Comparing `pytrivialsql-0.1.1/src/pytrivialsql/sql.py` & `pytrivialsql-0.1.2/src/pytrivialsql/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,18 @@
     res = _where_to_string(where, placeholder)
     if res is not None:
         qstr, qvars = res
         return f" WHERE {qstr}", qvars
     return None
 
 
+def drop_q(table_name):
+    return f"DROP TABLE IF EXISTS {table_name}"
+
+
 def create_q(table_name, cols):
     return f"CREATE TABLE IF NOT EXISTS {table_name}({', '.join(cols)})"
 
 
 def insert_q(table_name, **args):
     placeholder = args.get("placeholder", "?")
     returning = args.get("RETURNING", args.get("returning", None))
```

### Comparing `pytrivialsql-0.1.1/src/pytrivialsql/sqlite.py` & `pytrivialsql-0.1.2/src/pytrivialsql/sqlite.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             return res[0][0].split("=")[1] == "1"
         except Exception:
             False
 
     def drop(self, *table_names):
         with self._conn as cur:
             for tbl in table_names:
-                cur.execute(f"DROP TABLE {tbl}")
+                cur.execute(sql.drop_q(tbl))
 
     def create(self, table_name, props):
         try:
             with self._conn as cur:
                 cur.execute(sql.create_q(table_name, props))
                 return True
         except Exception:
```

### Comparing `pytrivialsql-0.1.1/src/pytrivialsql.egg-info/PKG-INFO` & `pytrivialsql-0.1.2/src/pytrivialsql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrivialsql
-Version: 0.1.1
+Version: 0.1.2
 Summary: A trivial set of QOL bindings for SQL in Python
 Author-email: inaimathi <leo.zovic@gmail.com>
 Project-URL: Homepage, https://github.com/inaimathi/pytrivialsql
 Project-URL: Issues, https://github.com/inaimathi/pytrivialsql/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pytrivialsql-0.1.1/tests/test_sql.py` & `pytrivialsql-0.1.2/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `pytrivialsql-0.1.1/tests/test_sqlite.py` & `pytrivialsql-0.1.2/tests/test_sqlite.py`

 * *Files identical despite different names*

