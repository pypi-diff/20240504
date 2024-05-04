# Comparing `tmp/mysqlx-2.1.4.tar.gz` & `tmp/mysqlx-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-2.1.4.tar", last modified: Mon Apr 22 01:17:31 2024, max compression
+gzip compressed data, was "dist\mysqlx-2.2.0.tar", last modified: Sat May  4 10:32:42 2024, max compression
```

## Comparing `mysqlx-2.1.4.tar` & `mysqlx-2.2.0.tar`

### file list

```diff
@@ -1,27 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 01:17:31.000000 mysqlx-2.1.4/
--rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-2.1.4/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-22 01:17:31.000000 mysqlx-2.1.4/mysqlx/
--rw-rw-rw-   0        0        0      163 2024-04-21 14:49:14.000000 mysqlx-2.1.4/mysqlx/constant.py
--rw-rw-rw-   0        0        0     5069 2024-04-21 15:19:48.000000 mysqlx-2.1.4/mysqlx/db.py
--rw-rw-rw-   0        0        0     5898 2024-04-21 15:53:48.000000 mysqlx-2.1.4/mysqlx/dbx.py
--rw-rw-rw-   0        0        0     7187 2024-03-27 02:51:39.000000 mysqlx-2.1.4/mysqlx/generator.py
--rw-rw-rw-   0        0        0     1802 2023-07-24 02:58:28.000000 mysqlx-2.1.4/mysqlx/generator.tpl
--rw-rw-rw-   0        0        0      871 2024-04-21 15:19:48.000000 mysqlx-2.1.4/mysqlx/log_support.py
--rw-rw-rw-   0        0        0     7278 2023-08-04 01:47:15.000000 mysqlx-2.1.4/mysqlx/sql_holder.py
--rw-rw-rw-   0        0        0      626 2024-04-22 01:06:31.000000 mysqlx-2.1.4/mysqlx/sql_id_exec.py
--rw-rw-rw-   0        0        0     4880 2024-04-21 15:26:32.000000 mysqlx-2.1.4/mysqlx/sql_mapper.py
--rw-rw-rw-   0        0        0      295 2024-03-26 05:59:56.000000 mysqlx-2.1.4/mysqlx/sql_page_exec.py
--rw-rw-rw-   0        0        0     1676 2024-04-21 15:19:48.000000 mysqlx-2.1.4/mysqlx/sql_support.py
--rw-rw-rw-   0        0        0      340 2024-03-26 05:16:39.000000 mysqlx-2.1.4/mysqlx/support.py
--rw-rw-rw-   0        0        0     1588 2024-04-21 15:35:44.000000 mysqlx-2.1.4/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 01:17:31.000000 mysqlx-2.1.4/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2024-04-22 01:17:31.000000 mysqlx-2.1.4/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-22 00:27:57.000000 mysqlx-2.1.4/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4984 2024-04-22 01:17:31.000000 mysqlx-2.1.4/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       31 2024-04-22 01:17:31.000000 mysqlx-2.1.4/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      461 2024-04-22 01:17:31.000000 mysqlx-2.1.4/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2024-04-22 01:17:31.000000 mysqlx-2.1.4/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4984 2024-04-22 01:17:31.000000 mysqlx-2.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4319 2024-04-22 00:20:10.000000 mysqlx-2.1.4/README.rst
--rw-rw-rw-   0        0        0       42 2024-04-22 01:17:31.000000 mysqlx-2.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1327 2024-04-22 00:30:05.000000 mysqlx-2.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 10:32:42.000000 mysqlx-2.2.0/
+drwxrwxrwx   0        0        0        0 2024-05-04 10:32:42.000000 mysqlx-2.2.0/mysqlx/
+-rw-rw-rw-   0        0        0      164 2024-05-04 10:10:36.000000 mysqlx-2.2.0/mysqlx/constant.py
+-rw-rw-rw-   0        0        0     5070 2024-05-04 10:10:36.000000 mysqlx-2.2.0/mysqlx/db.py
+-rw-rw-rw-   0        0        0     5898 2024-04-21 15:53:48.000000 mysqlx-2.2.0/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0      872 2024-05-04 10:10:36.000000 mysqlx-2.2.0/mysqlx/log_support.py
+-rw-rw-rw-   0        0        0     7278 2023-08-04 01:47:15.000000 mysqlx-2.2.0/mysqlx/sql_holder.py
+-rw-rw-rw-   0        0        0      628 2024-05-04 10:10:36.000000 mysqlx-2.2.0/mysqlx/sql_id_exec.py
+-rw-rw-rw-   0        0        0     4888 2024-05-04 10:24:20.000000 mysqlx-2.2.0/mysqlx/sql_mapper.py
+-rw-rw-rw-   0        0        0      297 2024-05-04 10:10:36.000000 mysqlx-2.2.0/mysqlx/sql_page_exec.py
+-rw-rw-rw-   0        0        0     1677 2024-05-04 10:10:36.000000 mysqlx-2.2.0/mysqlx/sql_support.py
+-rw-rw-rw-   0        0        0      344 2024-05-04 10:10:36.000000 mysqlx-2.2.0/mysqlx/support.py
+-rw-rw-rw-   0        0        0     1589 2024-05-04 10:10:36.000000 mysqlx-2.2.0/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 10:32:42.000000 mysqlx-2.2.0/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-05-04 10:32:42.000000 mysqlx-2.2.0/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-04 10:32:42.000000 mysqlx-2.2.0/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4955 2024-05-04 10:32:42.000000 mysqlx-2.2.0/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-04 10:32:42.000000 mysqlx-2.2.0/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      412 2024-05-04 10:32:42.000000 mysqlx-2.2.0/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2024-05-04 10:32:42.000000 mysqlx-2.2.0/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4955 2024-05-04 10:32:42.000000 mysqlx-2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4313 2024-05-04 10:32:25.000000 mysqlx-2.2.0/README.rst
+-rw-rw-rw-   0        0        0       42 2024-05-04 10:32:42.000000 mysqlx-2.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1326 2024-05-04 10:09:11.000000 mysqlx-2.2.0/setup.py
```

### Comparing `mysqlx-2.1.4/mysqlx/db.py` & `mysqlx-2.2.0/mysqlx/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from . import sql_support
 # Don't remove. Import for not repetitive implementation
-from sqlexec import insert, save, batch_insert, batch_execute, do_execute, do_save_sql, do_get, do_query,\
+from sqlexecx import insert, save, batch_insert, batch_execute, do_execute, do_save_sql, do_get, do_query,\
     do_query_one, do_select,do_select_one, do_select_page, do_query_page, do_select_page, do_query_page, load, do_load, insert_from_csv,\
     insert_from_df, insert_from_json, truncate_table, drop_table, table
 
 
 def execute(sql: str, *args, **kwargs):
     """
     Execute SQL.
```

### Comparing `mysqlx-2.1.4/mysqlx/dbx.py` & `mysqlx-2.2.0/mysqlx/dbx.py`

 * *Files identical despite different names*

### Comparing `mysqlx-2.1.4/mysqlx/log_support.py` & `mysqlx-2.2.0/mysqlx/log_support.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Don't remove. Import for not repetitive implementation
-from sqlexec.log_support import logger
+from sqlexecx.log_support import logger
 from .constant import MODULE
 
 
 def sql_id_log(function: str, sql_id: str, *args, **kwargs):
     logger.debug("Exec func '%s.dbx.%s', sql_id: %s, args: %s, kwargs: %s" % (MODULE, function, sql_id.strip(), args, kwargs))
```

### Comparing `mysqlx-2.1.4/mysqlx/sql_holder.py` & `mysqlx-2.2.0/mysqlx/sql_holder.py`

 * *Files identical despite different names*

### Comparing `mysqlx-2.1.4/mysqlx/sql_id_exec.py` & `mysqlx-2.2.0/mysqlx/sql_id_exec.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from . import dbx
-from sqlexec.sql_exec import SqlExec as _SqlExec
-from sqlexec.page_exec import PageExec
+from sqlexecx.sql_exec import SqlExec as _SqlExec
+from sqlexecx.page_exec import PageExec
 
 
 class SqlExec(_SqlExec):
 
     def save(self, *args, **kwargs):
         """
         Insert data into table, return primary key.
```

### Comparing `mysqlx-2.1.4/mysqlx/sql_mapper.py` & `mysqlx-2.2.0/mysqlx/sql_mapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-import sqlexec
+import sqlexecx
 import functools
 from .log_support import logger
 from .support import SqlAction, DBError
 from .sql_support import simple_sql, get_named_sql_args
 from .sql_holder import get_sql_model, do_get_sql, build_sql_id
 
 _UPDATE_ACTIONS = (SqlAction.INSERT.value, SqlAction.UPDATE.value, SqlAction.DELETE.value, SqlAction.CALL.value)
@@ -75,34 +75,34 @@
     return _decorator
 
 
 def get_exec_func(func, action, batch):
     if action == SqlAction.SELECT.value:
         return get_select_func(func)
     elif batch:
-        return sqlexec.batch_execute
+        return sqlexecx.batch_execute
     else:
-        return sqlexec.do_execute
+        return sqlexecx.do_execute
 
 
 def get_select_func(func):
     names = func.__code__.co_names
     is_list = 'list' in names or 'List' in names
     if 'Mapping' in names and is_list:
-        return sqlexec.do_query
+        return sqlexecx.do_query
     elif 'Mapping' in names:
         return sqlexec.do_query_one
     elif len(names) == 1 and names[0] in ('int', 'float', 'Decimal', 'str', 'AnyStr', 'date', 'time', 'datetime'):
-        return sqlexec.do_get
+        return sqlexecx.do_get
     elif len(names) == 1 and names[0] in ('tuple', 'Tuple'):
-        return sqlexec.do_select_one
+        return sqlexecx.do_select_one
     elif is_list:
-        return sqlexec.do_select
+        return sqlexecx.do_select
     else:
-        return sqlexec.do_query
+        return sqlexecx.do_query
 
 
 def before(func, namespace, _id, *args, **kwargs):
     file_name = os.path.basename(func.__code__.co_filename)[:-3]
     _namespace = namespace if namespace else file_name
     _id = _id if _id else func.__name__
     sql_id = build_sql_id(_namespace, _id)
```

### Comparing `mysqlx-2.1.4/mysqlx/sql_support.py` & `mysqlx-2.2.0/mysqlx/sql_support.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from jinja2 import Template
 from functools import lru_cache
 from .log_support import page_log
 from .constant import LIMIT_1, DYNAMIC_REGEX, CACHE_SIZE
 
 # Don't remove. Import for not repetitive implementation
-from sqlexec.sql_support import get_batch_args, get_named_sql_args, is_mapping, get_mapping_sql_args, require_limit, try_mapping, get_table_select_sql
+from sqlexecx.sql_support import get_batch_args, get_named_sql_args, is_mapping, get_mapping_sql_args, require_limit, try_mapping, get_table_select_sql
 
 
 def simple_sql(sql: str, *args, **kwargs):
     return get_named_sql_args(sql, **kwargs) if kwargs else (sql, args)
 
 
 def dynamic_sql(sql: str, **kwargs):
```

### Comparing `mysqlx-2.1.4/mysqlx/__init__.py` & `mysqlx-2.2.0/mysqlx/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sqlexec import (
+from sqlexecx import (
     connection,
     transaction,
     with_connection,
     with_transaction,
     get_connection,
     close,
     Driver,
```

### Comparing `mysqlx-2.1.4/mysqlx.egg-info/PKG-INFO` & `mysqlx-2.2.0/mysqlx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 2.1.4
+Version: 2.2.0
 Summary: A thread safe sql executor for MySQL like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 Mapper file
 '''''''''''
 
 Create a mapper file in 'mapper' folder, you can named
 'user_mapper.xml', like follow:
 
@@ -145,16 +144,16 @@
 
 
        def test_transaction2():
            with transaction():
                insert_func(....)
                update_func(....)
 
-You can generate model class with mysqlx-generator: https://pypi.org/project/sqlx-orm
+You can generate model class with mysqlx-generator: https://pypi.org/project/sqlormx
 
 If you want to operate PostgreSQL database, may be you need PgSqlx: https://pypi.org/project/pgsqlx
 
-If you just wanted a simple sql executor, may be you need sqlx-exec: https://pypi.org/project/sqlx-exec
+If you just wanted a simple sql executor, may be you need sqlx-exec: https://pypi.org/project/sqlexecx
 
-If you wanted simultaneously support MySQL and PostgreSQL, may be you need sqlx-batis: https://pypi.org/project/sqlx-batis
+If you wanted simultaneously support MySQL and PostgreSQL, may be you need sqlx-batis: https://pypi.org/project/batisx
```

### Comparing `mysqlx-2.1.4/PKG-INFO` & `mysqlx-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 2.1.4
+Version: 2.2.0
 Summary: A thread safe sql executor for MySQL like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 Mapper file
 '''''''''''
 
 Create a mapper file in 'mapper' folder, you can named
 'user_mapper.xml', like follow:
 
@@ -145,16 +144,16 @@
 
 
        def test_transaction2():
            with transaction():
                insert_func(....)
                update_func(....)
 
-You can generate model class with mysqlx-generator: https://pypi.org/project/sqlx-orm
+You can generate model class with mysqlx-generator: https://pypi.org/project/sqlormx
 
 If you want to operate PostgreSQL database, may be you need PgSqlx: https://pypi.org/project/pgsqlx
 
-If you just wanted a simple sql executor, may be you need sqlx-exec: https://pypi.org/project/sqlx-exec
+If you just wanted a simple sql executor, may be you need sqlx-exec: https://pypi.org/project/sqlexecx
 
-If you wanted simultaneously support MySQL and PostgreSQL, may be you need sqlx-batis: https://pypi.org/project/sqlx-batis
+If you wanted simultaneously support MySQL and PostgreSQL, may be you need sqlx-batis: https://pypi.org/project/batisx
```

### Comparing `mysqlx-2.1.4/README.rst` & `mysqlx-2.2.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,14 @@
 
 
        def test_transaction2():
            with transaction():
                insert_func(....)
                update_func(....)
 
-You can generate model class with mysqlx-generator: https://pypi.org/project/sqlx-orm
+You can generate model class with mysqlx-generator: https://pypi.org/project/sqlormx
 
 If you want to operate PostgreSQL database, may be you need PgSqlx: https://pypi.org/project/pgsqlx
 
-If you just wanted a simple sql executor, may be you need sqlx-exec: https://pypi.org/project/sqlx-exec
+If you just wanted a simple sql executor, may be you need sqlx-exec: https://pypi.org/project/sqlexecx
 
-If you wanted simultaneously support MySQL and PostgreSQL, may be you need sqlx-batis: https://pypi.org/project/sqlx-batis
+If you wanted simultaneously support MySQL and PostgreSQL, may be you need sqlx-batis: https://pypi.org/project/batisx
```

### Comparing `mysqlx-2.1.4/setup.py` & `mysqlx-2.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     name='mysqlx',
     packages=['mysqlx'],
     description="A thread safe sql executor for MySQL like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
-        'sqlx-exec>=2.3.6',
+        'sqlexecx>=0.0.2',
     ],
-    version='2.1.4',
+    version='2.2.0',
     url='https://gitee.com/summry/mysqlx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

