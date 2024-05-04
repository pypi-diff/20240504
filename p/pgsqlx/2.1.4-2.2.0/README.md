# Comparing `tmp/pgsqlx-2.1.4.tar.gz` & `tmp/pgsqlx-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pgsqlx-2.1.4.tar", last modified: Mon Apr 22 03:34:32 2024, max compression
+gzip compressed data, was "dist\pgsqlx-2.2.0.tar", last modified: Sat May  4 10:37:12 2024, max compression
```

## Comparing `pgsqlx-2.1.4.tar` & `pgsqlx-2.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 03:34:32.000000 pgsqlx-2.1.4/
-drwxrwxrwx   0        0        0        0 2024-04-22 03:34:32.000000 pgsqlx-2.1.4/pgsqlx/
--rw-rw-rw-   0        0        0       47 2024-04-22 01:34:52.000000 pgsqlx-2.1.4/pgsqlx/constant.py
--rw-rw-rw-   0        0        0     1253 2024-04-22 01:30:19.000000 pgsqlx-2.1.4/pgsqlx/db.py
--rw-rw-rw-   0        0        0     1246 2024-04-22 01:31:03.000000 pgsqlx-2.1.4/pgsqlx/dbx.py
--rw-rw-rw-   0        0        0      956 2023-07-28 02:25:02.000000 pgsqlx-2.1.4/pgsqlx/log_support.py
--rw-rw-rw-   0        0        0     3302 2024-04-22 01:29:23.000000 pgsqlx-2.1.4/pgsqlx/sql_mapper.py
--rw-rw-rw-   0        0        0     1348 2024-04-22 01:26:50.000000 pgsqlx-2.1.4/pgsqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 03:34:32.000000 pgsqlx-2.1.4/pgsqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2024-04-22 03:34:32.000000 pgsqlx-2.1.4/pgsqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-22 03:34:32.000000 pgsqlx-2.1.4/pgsqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     5812 2024-04-22 03:34:32.000000 pgsqlx-2.1.4/pgsqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       18 2024-04-22 03:34:32.000000 pgsqlx-2.1.4/pgsqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      305 2024-04-22 03:34:32.000000 pgsqlx-2.1.4/pgsqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2024-04-22 03:34:32.000000 pgsqlx-2.1.4/pgsqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5812 2024-04-22 03:34:32.000000 pgsqlx-2.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     5136 2024-04-22 01:22:30.000000 pgsqlx-2.1.4/README.rst
--rw-rw-rw-   0        0        0       42 2024-04-22 03:34:32.000000 pgsqlx-2.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1312 2024-04-22 01:12:18.000000 pgsqlx-2.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 10:37:12.000000 pgsqlx-2.2.0/
+drwxrwxrwx   0        0        0        0 2024-05-04 10:37:12.000000 pgsqlx-2.2.0/pgsqlx/
+-rw-rw-rw-   0        0        0       47 2024-04-22 01:34:52.000000 pgsqlx-2.2.0/pgsqlx/constant.py
+-rw-rw-rw-   0        0        0     1251 2024-05-04 10:35:55.000000 pgsqlx-2.2.0/pgsqlx/db.py
+-rw-rw-rw-   0        0        0     1244 2024-05-04 10:35:55.000000 pgsqlx-2.2.0/pgsqlx/dbx.py
+-rw-rw-rw-   0        0        0      954 2024-05-04 10:35:55.000000 pgsqlx-2.2.0/pgsqlx/log_support.py
+-rw-rw-rw-   0        0        0     3307 2024-05-04 10:36:15.000000 pgsqlx-2.2.0/pgsqlx/sql_mapper.py
+-rw-rw-rw-   0        0        0     1347 2024-05-04 10:36:15.000000 pgsqlx-2.2.0/pgsqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 10:37:12.000000 pgsqlx-2.2.0/pgsqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-05-04 10:37:12.000000 pgsqlx-2.2.0/pgsqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-04 10:37:12.000000 pgsqlx-2.2.0/pgsqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     5812 2024-05-04 10:37:12.000000 pgsqlx-2.2.0/pgsqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2024-05-04 10:37:12.000000 pgsqlx-2.2.0/pgsqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      305 2024-05-04 10:37:12.000000 pgsqlx-2.2.0/pgsqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2024-05-04 10:37:12.000000 pgsqlx-2.2.0/pgsqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5812 2024-05-04 10:37:12.000000 pgsqlx-2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5136 2024-04-22 01:22:30.000000 pgsqlx-2.2.0/README.rst
+-rw-rw-rw-   0        0        0       42 2024-05-04 10:37:12.000000 pgsqlx-2.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1308 2024-05-04 10:35:55.000000 pgsqlx-2.2.0/setup.py
```

### Comparing `pgsqlx-2.1.4/pgsqlx/db.py` & `pgsqlx-2.2.0/pgsqlx/db.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from . import Dialect
 from .log_support import save_log, save_key_seq_log
 
 # Don't remove. Import for not repetitive implementation
-from sqlbatis.db import insert, save, save_select_key, execute, batch_insert, batch_execute, get, query, query_one, select, select_one, save_sql, \
+from batisx.db import insert, save, save_select_key, execute, batch_insert, batch_execute, get, query, query_one, select, select_one, save_sql, \
     save_sql_select_key, do_execute, do_get, do_query, do_query_one, do_select, do_select_one, do_select_page, do_query_page, select_page, query_page,\
     do_save_sql, do_save_sql_select_key, drop_table, drop_table, sql, table, page
 
 
 def save_key_seq(key_seq: str, table_name: str, **kwargs):
     """
     Insert data into table, return primary key.
```

### Comparing `pgsqlx-2.1.4/pgsqlx/dbx.py` & `pgsqlx-2.2.0/pgsqlx/dbx.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from . import Dialect, db
 from mysqlx import sql_holder as holder
 from .log_support import sql_id_log, sql_id_key_seq_log
-from sqlbatis.dbx import save_select_key, batch_execute, execute, get, query, query_one, select, select_one, select_page, query_page, sql, page
+from batisx.dbx import save_select_key, batch_execute, execute, get, query, query_one, select, select_one, select_page, query_page, sql, page
 
 
 def save(sql_id: str, *args, **kwargs):
     """
     Execute insert SQL, return primary key.
     :return: Primary key
     """
```

### Comparing `pgsqlx-2.1.4/pgsqlx/log_support.py` & `pgsqlx-2.2.0/pgsqlx/log_support.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sqlbatis.log_support import logger
+from batisx.log_support import logger
 
 
 def save_log(table, **kwargs):
     logger.debug("Exec func 'pgsqlx.db.save' \n\t Table: '%s', kwargs: %s" % (table, kwargs))
 
 
 def sql_id_log(function: str, sql_id: str, *args, **kwargs):
```

### Comparing `pgsqlx-2.1.4/pgsqlx/sql_mapper.py` & `pgsqlx-2.2.0/pgsqlx/sql_mapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import sqlexec
+import sqlexecx
 import functools
 from .log_support import logger
 from mysqlx.support import SqlAction
 from mysqlx.sql_support import simple_sql, get_named_sql_args
 from mysqlx.sql_holder import get_sql_model, do_get_sql
-from sqlbatis.sql_mapper import get_exec_func, before, get_select_func
+from batisx.sql_mapper import get_exec_func, before, get_select_func
 
 _UPDATE_ACTIONS = (SqlAction.INSERT.value, SqlAction.UPDATE.value, SqlAction.DELETE.value, SqlAction.CALL.value)
 
 
 def mapper(namespace: str = None, sql_id: str = None, batch=False, return_key=False, key_seq=None):
     def _decorator(func):
         @functools.wraps(func)
@@ -18,16 +18,16 @@
             sql_model = get_sql_model(full_sql_id)
             exec_func = get_exec_func(func, sql_model.action, batch)
             if return_key:
                 use_key_seq = key_seq
                 use_sql, args = do_get_sql(sql_model, batch, param_names, *args, **kwargs)
                 if use_key_seq is None:
                     use_key_seq = sql_model.key_seq
-                select_key = sqlexec.Dialect.get_select_key(key_seq=use_key_seq, sql=use_sql)
-                return sqlexec.do_save_sql_select_key(select_key, use_sql, *args)
+                select_key = sqlexecx.Dialect.get_select_key(key_seq=use_key_seq, sql=use_sql)
+                return sqlexecx.do_save_sql_select_key(select_key, use_sql, *args)
             if batch:
                 if kwargs:
                     logger.warning("Batch exec sql better use like '{}(args)' or '{}(*args)' then '{}(args=args)'".format(func_name, func_name, func_name))
                     args = list(kwargs.values())[0]
                 use_sql, _ = do_get_sql(sql_model, batch, param_names, *args)
             else:
                 use_sql, args = do_get_sql(sql_model, batch, param_names, *args, **kwargs)
@@ -43,25 +43,25 @@
         def _wrapper(*args, **kwargs):
             use_sql = value
             low_sql = value.lower()
             if any([action in low_sql for action in _UPDATE_ACTIONS]):
                 if batch:
                     if kwargs:
                         args = list(kwargs.values())[0]
-                    return sqlexec.batch_execute(use_sql, *args)
+                    return sqlexecx.batch_execute(use_sql, *args)
                 if return_key:
                     assert SqlAction.INSERT.value in low_sql, 'Only insert sql can return primary key.'
                     if kwargs:
                         use_sql, args = get_named_sql_args(use_sql, **kwargs)
-                    select_key = sqlexec.Dialect.get_select_key(key_seq=key_seq, sql=use_sql)
-                    return sqlexec.do_save_sql_select_key(select_key, use_sql, *args)
+                    select_key = sqlexecx.Dialect.get_select_key(key_seq=key_seq, sql=use_sql)
+                    return sqlexecx.do_save_sql_select_key(select_key, use_sql, *args)
 
                 if kwargs:
                     use_sql, args = get_named_sql_args(use_sql, **kwargs)
-                return sqlexec.execute(use_sql, *args)
+                return sqlexecx.execute(use_sql, *args)
             elif SqlAction.SELECT.value in low_sql:
                 select_func = get_select_func(func)
                 use_sql, args = simple_sql(use_sql, *args, **kwargs)
                 return select_func(use_sql, *args)
             else:
                 return ValueError("Invalid sql: {}.".format(sql))
```

### Comparing `pgsqlx-2.1.4/pgsqlx/__init__.py` & `pgsqlx-2.2.0/pgsqlx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from sqlbatis import (
+from batisx import (
     connection,
     transaction,
     with_connection,
     with_transaction,
     get_connection,
     close,
     Driver,
     sql,
     mapper,
     init_db as _init_db
 )
 
 from .sql_mapper import sql, mapper
-from sqlexec import Dialect, Engine
+from sqlexecx import Dialect, Engine
 
 def init_db(*args, **kwargs):
     """
     Compliant with the Python DB API 2.0 (PEP-249).
 
     from pgsqlx import init_db
     init_db('test.db', driver='sqlite3', show_sql=True, debug=True)
```

### Comparing `pgsqlx-2.1.4/pgsqlx.egg-info/PKG-INFO` & `pgsqlx-2.2.0/pgsqlx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 2.1.4
+Version: 2.2.0
 Summary: A thread safe sql executor for PostgreSQL like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `pgsqlx-2.1.4/PKG-INFO` & `pgsqlx-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 2.1.4
+Version: 2.2.0
 Summary: A thread safe sql executor for PostgreSQL like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `pgsqlx-2.1.4/README.rst` & `pgsqlx-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `pgsqlx-2.1.4/setup.py` & `pgsqlx-2.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 setup(
     name='pgsqlx',
     packages=['pgsqlx'],
     description="A thread safe sql executor for PostgreSQL like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
-        'sqlx-batis>=2.1.4',
+        'batisx>=2.2.1',
     ],
-    version='2.1.4',
+    version='2.2.0',
     url='https://gitee.com/summry/pgsqlx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

