# Comparing `tmp/pypomes_db-0.3.9.tar.gz` & `tmp/pypomes_db-0.4.0.tar.gz`

## Comparing `pypomes_db-0.3.9.tar` & `pypomes_db-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pypomes_db-0.3.9/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 pypomes_db-0.3.9/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    11374 2020-02-02 00:00:00.000000 pypomes_db-0.3.9/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 pypomes_db-0.3.9/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0     8848 2020-02-02 00:00:00.000000 pypomes_db-0.3.9/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0     8842 2020-02-02 00:00:00.000000 pypomes_db-0.3.9/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.3.9/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.3.9/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.3.9/README.md
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pypomes_db-0.3.9/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 pypomes_db-0.4.0/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 pypomes_db-0.4.0/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    16482 2020-02-02 00:00:00.000000 pypomes_db-0.4.0/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.0/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    12320 2020-02-02 00:00:00.000000 pypomes_db-0.4.0/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    10231 2020-02-02 00:00:00.000000 pypomes_db-0.4.0/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    10350 2020-02-02 00:00:00.000000 pypomes_db-0.4.0/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.4.0/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.0/README.md
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pypomes_db-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.4.0/PKG-INFO
```

### Comparing `pypomes_db-0.3.9/src/pypomes_db/db_pomes.py` & `pypomes_db-0.4.0/src/pypomes_db/oracle_pomes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,102 +1,53 @@
 from logging import Logger
-from typing import Any
+from oracledb import Connection, connect
 
-from .db_common import DB_ENGINE
+from .db_common import (
+    _assert_query_quota, _db_get_params, _db_log, _db_except_msg
+)
 
-match DB_ENGINE:
-    case "oracle":
-        from . import oracle_pomes
-    case "postgres":
-        from . import postgres_pomes
-    case "sqlserver":
-        from . import sqlserver_pomes
+# TODO: db_call_function, db_call_procedure
 
 
-def db_connect(errors: list[str] | None,
-               logger: Logger = None) -> Any:
+def db_connect(errors: list[str],
+               logger: Logger = None) -> Connection:
     """
-    Obtain and return a connection to the database, or *None* if the connection cannot be obtained.
+    Obtain and return a connection to the database, or *None* if the connection could not be obtained.
 
     :param errors: incidental error messages
     :param logger: optional logger
     :return: the connection to the database
     """
-    result: Any = None
-    match DB_ENGINE:
-        case "postgres":
-            result = postgres_pomes.db_connect(errors, logger)
-        case "sqlserver":
-            result = sqlserver_pomes.db_connect(errors, logger)
-
-    return result
+    # initialize the return variable
+    result: Connection | None = None
 
+    # retrieve the connection parameters
+    name, user, pwd, host, port = _db_get_params("oracle")
 
-def db_exists(errors: list[str],
-              table: str,
-              where_attrs: list[str],
-              where_vals: tuple,
-              logger: Logger = None) -> bool:
-    """
-    Determine whether the table *table* in the database contains at least one tuple.
-
-    For this determination, *where_attrs* are made equal to *where_values* in the query, respectively.
-    If more than one, the attributes are concatenated by the *AND* logical connector.
-
-    :param errors: incidental error messages
-    :param table: the table to be searched
-    :param where_attrs: the search attributes
-    :param where_vals: the values for the search attributes
-    :param logger: optional logger
-    :return: True if at least one tuple was found
-    """
-    # noinspection PyDataSource
-    sel_stmt: str = "SELECT * FROM " + table
-    if len(where_attrs) > 0:
-        sel_stmt += " WHERE " + "".join(f"{attr} = %s AND " for attr in where_attrs)[0:-5]
-    rec: tuple = db_select_one(errors=errors,
-                               sel_stmt=sel_stmt,
-                               where_vals=where_vals,
-                               require_nonempty=False,
-                               logger=logger)
-    result: bool = None if len(errors) > 0 else rec is not None
+    # obtain a connection to the database
+    err_msg: str | None = None
+    try:
+        result = connect(service_name=name,
+                         host=host,
+                         port=port,
+                         user=user,
+                         password=pwd)
+    except Exception as e:
+        err_msg = _db_except_msg(exception=e,
+                                 engine="oracle")
+
+    # log the results
+    _db_log(errors=errors,
+            err_msg=err_msg,
+            logger=logger,
+            query_stmt=f"Connected to '{name}' at '{host}'")
 
     return result
 
 
-def db_select_one(errors: list[str] | None,
-                  sel_stmt: str,
-                  where_vals: tuple,
-                  require_nonempty: bool = False,
-                  logger: Logger = None) -> tuple:
-    """
-    Search the database and return the first tuple that satisfies the *sel_stmt* search command.
-
-    The command can optionally contain search criteria, with respective values given
-    in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
-    in a specific tuple. In case of error, or if the search is empty, *None* is returned.
-
-    :param errors: incidental error messages
-    :param sel_stmt: SELECT command for the search
-    :param where_vals: values to be associated with the search criteria
-    :param require_nonempty: defines whether an empty search should be considered an error
-    :param logger: optional logger
-    :return: tuple containing the search result, or None if there was an error, or if the search was empty
-    """
-    require_min: int = 1 if require_nonempty else None
-    reply: list[tuple] = db_select_all(errors=errors,
-                                       sel_stmt=sel_stmt,
-                                       where_vals=where_vals,
-                                       require_min=require_min,
-                                       require_max=1,
-                                       logger=logger)
-
-    return reply[0] if reply else None
-
-
 def db_select_all(errors: list[str] | None,
                   sel_stmt: str,
                   where_vals: tuple = None,
                   require_min: int = None,
                   require_max: int = None,
                   logger: Logger = None) -> list[tuple]:
     """
@@ -111,105 +62,64 @@
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
     :param require_min: optionally defines the minimum number of tuples to be returned
     :param require_max: optionally defines the maximum number of tuples to be returned
     :param logger: optional logger
     :return: list of tuples containing the search result, or [] if the search is empty
     """
-    result: list[tuple] | None = None
-    match DB_ENGINE:
-        case "oracle":
-            result = oracle_pomes.db_select_all(errors, sel_stmt, where_vals, require_min, require_max,  logger)
-        case "postgres":
-            result = postgres_pomes.db_select_all(errors, sel_stmt, where_vals, require_min, require_max,  logger)
-        case "sqlserver":
-            result = sqlserver_pomes.db_select_all(errors, sel_stmt, where_vals, require_min, require_max, logger)
-
-    return result
-
-
-def db_insert(errors: list[str] | None,
-              insert_stmt: str,
-              insert_vals: tuple,
-              logger: Logger = None) -> int:
-    """
-    Insert a tuple, with values defined in *insert_vals*, into the database.
-
-    :param errors: incidental error messages
-    :param insert_stmt: the INSERT command
-    :param insert_vals: the values to be inserted
-    :param logger: optional logger
-    :return: the number of inserted tuples (0 ou 1), or None if an error occurred
-    """
-    result: int | None = None
-    match DB_ENGINE:
-        case "oracle":
-            result = oracle_pomes.db_modify(errors, insert_stmt, insert_vals, logger)
-        case "postgres":
-            result = postgres_pomes.db_modify(errors, insert_stmt, insert_vals, logger)
-        case "sqlserver":
-            result = sqlserver_pomes.db_modify(errors, insert_stmt, insert_vals, logger)
-
-    return result
-
-
-def db_update(errors: list[str] | None,
-              update_stmt: str,
-              update_vals: tuple,
-              where_vals: tuple,
-              logger: Logger = None) -> int:
-    """
-    Update one or more tuples in the database, as defined by the command *update_stmt*.
-
-    The values for this update are in *update_vals*.
-    The values for selecting the tuples to be updated are in *where_vals*.
-
-    :param errors: incidental error messages
-    :param update_stmt: the UPDATE command
-    :param update_vals: the values for the update operation
-    :param where_vals: the values to be associated with the search criteria
-    :param logger: optional logger
-    :return: the number of updated tuples, or None if an error occurred
-    """
-    result: int | None = None
-    values: tuple = update_vals + where_vals
-    match DB_ENGINE:
-        case "oracle":
-            result = oracle_pomes.db_modify(errors, update_stmt, values, logger)
-        case "postgres":
-            result = postgres_pomes.db_modify(errors, update_stmt, values, logger)
-        case "sqlserver":
-            result = sqlserver_pomes.db_modify(errors, update_stmt, values, logger)
-
-    return result
+    # initialize the return variable
+    result: list[tuple] = []
 
+    # retrieve the connection parameters
+    name, user, pwd, host, port = _db_get_params("oracle")
 
-def db_delete(errors: list[str] | None,
-              delete_stmt: str,
-              where_vals: tuple,
-              logger: Logger = None) -> int:
-    """
-    Delete one or more tuples in the database, as defined by the *delete_stmt* command.
-
-    The values for selecting the tuples to be deleted are in *where_vals*.
+    if isinstance(require_max, int) and require_max > 0:
+        sel_stmt: str = f"{sel_stmt} FETCH NEXT {require_max} ROWS ONLY"
 
-    :param errors: incidental error messages
-    :param delete_stmt: the DELETE command
-    :param where_vals: the values to be associated with the search criteria
-    :param logger: optional logger
-    :return: the number of deleted tuples, or None if an error occurred
-    """
-    result: int | None = None
-    match DB_ENGINE:
-        case "oracle":
-            result = oracle_pomes.db_modify(errors, delete_stmt, where_vals, logger)
-        case "postgres":
-            result = postgres_pomes.db_modify(errors, delete_stmt, where_vals, logger)
-        case "sqlserver":
-            result = sqlserver_pomes.db_modify(errors, delete_stmt, where_vals, logger)
+    err_msg: str | None = None
+    try:
+        # obtain the connection
+        with  connect(service_name=name,
+                      host=host,
+                      port=port,
+                      user=user,
+                      password=pwd) as conn:
+            # make sure the connection is not in autocommit mode
+            conn.autocommit = False
+
+            # obtain a cursor and perform the operation
+            with conn.cursor() as cursor:
+                # execute the query
+                cursor.execute(statement=sel_stmt,
+                               parameters=where_vals)
+                # obtain the number of tuples returned
+                count: int = cursor.rowcount
+
+                # has the query quota been satisfied ?
+                if _assert_query_quota(errors=errors,
+                                       query=sel_stmt,
+                                       where_vals=where_vals,
+                                       count=count,
+                                       require_min=require_min,
+                                       require_max=require_max):
+                    # yes, retrieve the returned tuples
+                    rows: list = cursor.fetchall()
+                    result = [tuple(row) for row in rows]
+            # commit the transaction
+            conn.commit()
+    except Exception as e:
+        err_msg = _db_except_msg(exception=e,
+                                 engine="oracle")
+
+    # log the results
+    _db_log(errors=errors,
+            err_msg=err_msg,
+            logger=logger,
+            query_stmt=sel_stmt,
+            bind_vals=where_vals)
 
     return result
 
 
 def db_bulk_insert(errors: list[str] | None,
                    insert_stmt: str,
                    insert_vals: list[tuple],
@@ -219,65 +129,209 @@
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the list of values to be inserted
     :param logger: optional logger
     :return: the number of inserted tuples, or None if an error occurred
     """
+    # initialize the return variable
     result: int | None = None
-    match DB_ENGINE:
-        case "postgres":
-            result = postgres_pomes.db_bulk_insert(errors, insert_stmt, insert_vals, logger)
-        case "sqlserver":
-            result = sqlserver_pomes.db_bulk_insert(errors, insert_stmt, insert_vals, logger)
+
+    # retrieve the connection parameters
+    name, user, pwd, host, port = _db_get_params("oracle")
+
+    err_msg: str | None = None
+    try:
+        # obtain the connection
+        with  connect(service_name=name,
+                      host=host,
+                      port=port,
+                      user=user,
+                      password=pwd) as conn:
+            # make sure the connection is not in autocommit mode
+            conn.autocommit = False
+
+            # obtain a cursor and perform the operation
+            with conn.cursor() as cursor:
+                try:
+                    cursor.executemany(statement=insert_stmt,
+                                       parameters=insert_vals)
+                    result = len(insert_vals)
+                except Exception:
+                    conn.rollback()
+                    raise
+            conn.commit()
+    except Exception as e:
+        err_msg = _db_except_msg(exception=e,
+                                 engine="oracle")
+
+    # log the results
+    _db_log(errors=errors,
+            err_msg=err_msg,
+            logger=logger,
+            query_stmt=insert_stmt,
+            bind_vals=insert_vals[0])
 
     return result
 
 
+# TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
 def db_call_function(errors: list[str] | None,
                      func_name: str,
                      func_vals: tuple,
                      logger: Logger = None) -> list[tuple]:
     """
     Execute the stored function *func_name* in the database, with the parameters given in *func_vals*.
 
     :param errors: incidental error messages
     :param func_name: name of the stored function
     :param func_vals: parameters for the stored function
     :param logger: optional logger
     :return: the data returned by the function
     """
-    result: Any = None
-    match DB_ENGINE:
-        case "oracle":
-            result = oracle_pomes.db_call_function(errors, func_name, func_vals, logger)
-        case "postgres":
-            result = postgres_pomes.db_call_procedure(errors, func_name, func_vals, logger)
-        case "sqlserver":
-            result = sqlserver_pomes.db_call_procedure(errors, func_name, func_vals, logger)
+    # initialize the return variable
+    # noinspection DuplicatedCode
+    result: list[tuple] = []
+
+    # retrieve the connection parameters
+    name, user, pwd, host, port = _db_get_params("oracle")
+
+    # execute the stored procedure
+    err_msg: str | None = None
+    try:
+        # obtain a connection
+        with  connect(service_name=name,
+                      host=host,
+                      port=port,
+                      user=user,
+                      password=pwd) as conn:
+            # make sure the connection is not in autocommit mode
+            conn.autocommit = False
+            # obtain a cursor and perform the operation
+            with conn.cursor() as cursor:
+                cursor.callproc(name=func_name,
+                                parameters=func_vals)
+                # yes, retrieve the returned tuples
+                result = list(cursor)
+            # commit the transaction
+            conn.commit()
+    except Exception as e:
+        err_msg = _db_except_msg(exception=e,
+                                 engine="oracle")
+
+    # log the results
+    _db_log(errors, err_msg, logger, func_name, func_vals)
+    _db_log(errors=errors,
+            err_msg=err_msg,
+            logger=logger,
+            query_stmt=func_name,
+            bind_vals=func_vals)
 
     return result
 
 
+# TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
 def db_call_procedure(errors: list[str] | None,
                       proc_name: str,
                       proc_vals: tuple,
                       logger: Logger = None) -> list[tuple]:
     """
     Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
 
     :param errors: incidental error messages
     :param proc_name: name of the stored procedure
     :param proc_vals: parameters for the stored procedure
     :param logger: optional logger
     :return: the data returned by the procedure
     """
-    result: Any = None
-    match DB_ENGINE:
-        case "oracle":
-            result = oracle_pomes.db_call_procedure(errors, proc_name, proc_vals, logger)
-        case "postgres":
-            result = postgres_pomes.db_call_procedure(errors, proc_name, proc_vals, logger)
-        case "sqlserver":
-            result = sqlserver_pomes.db_call_procedure(errors, proc_name, proc_vals, logger)
+    # initialize the return variable
+    # noinspection DuplicatedCode
+    result: list[tuple] = []
+
+    # retrieve the connection parameters
+    name, user, pwd, host, port = _db_get_params("oracle")
+
+    # execute the stored procedure
+    err_msg: str | None = None
+    try:
+        # obtain a connection
+        with  connect(service_name=name,
+                      host=host,
+                      port=port,
+                      user=user,
+                      password=pwd) as conn:
+            # make sure the connection is not in autocommit mode
+            conn.autocommit = False
+            # obtain a cursor and perform the operation
+            with conn.cursor() as cursor:
+                cursor.callproc(name=proc_name,
+                                parameters=proc_vals)
+
+                # retrieve the returned tuples
+                result = list(cursor)
+            # commit the transaction
+            conn.commit()
+    except Exception as e:
+        err_msg = _db_except_msg(exception=e,
+                                 engine="oracle")
+
+    # log the results
+    _db_log(errors=errors,
+            err_msg=err_msg,
+            logger=logger,
+            query_stmt=proc_name,
+            bind_vals=proc_vals)
+
+    return result
+
+
+def db_modify(errors: list[str] | None,
+              modify_stmt: str,
+              bind_vals: tuple | list[tuple],
+              logger: Logger) -> int:
+    """
+    Modify the database, inserting, updating or deleting tuples, according to the *modify_stmt* command definitions.
+
+    The values for this modification, followed by the values for selecting tuples are in *bind_vals*.
+
+    :param errors: incidental error messages
+    :param modify_stmt: INSERT, UPDATE, or DELETE command
+    :param bind_vals: values for database modification, and for tuples selection
+    :param logger: optional logger
+    :return: the number of inserted, modified, or deleted tuples, ou None if an error occurred
+    """
+    # initialize the return variable
+    result: int | None = None
+
+    # retrieve the connection parameters
+    name, user, pwd, host, port = _db_get_params("oracle")
+
+    err_msg: str | None = None
+    try:
+        # obtain a connection
+        with  connect(service_name=name,
+                      host=host,
+                      port=port,
+                      user=user,
+                      password=pwd) as conn:
+            # make sure the connection is not in autocommit mode
+            conn.autocommit = False
+            # obtain the cursor and execute the operation
+            with conn.cursor() as cursor:
+                cursor.execute(statement=modify_stmt,
+                               parameters=bind_vals)
+                result = cursor.rowcount
+            # commit the transaction
+            conn.commit()
+    except Exception as e:
+        err_msg = _db_except_msg(exception=e,
+                                 engine="oracle")
+
+    # log the results
+    _db_log(errors, err_msg, logger, modify_stmt, bind_vals)
+    _db_log(errors=errors,
+            err_msg=err_msg,
+            logger=logger,
+            query_stmt=modify_stmt,
+            bind_vals=bind_vals)
 
     return result
```

### Comparing `pypomes_db-0.3.9/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.4.0/src/pypomes_db/sqlserver_pomes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 from logging import Logger
-from oracledb import Connection, connect
+from pyodbc import connect, Connection, Row
 
 from .db_common import (
-    DB_NAME, DB_HOST, DB_PORT, DB_PWD, DB_USER,
-    _assert_query_quota, _db_log, _db_except_msg
+    _assert_query_quota, _db_get_params, _db_log, _db_except_msg
 )
 
-# TODO: db_bulk_insert, db_call_function, db_call_procedure
 
-
-def db_connect(errors: list[str], logger: Logger = None) -> Connection:
+def db_connect(errors: list[str] | None,
+               logger: Logger = None) -> Connection:
     """
-    Obtain and return a connection to the database, or *None* if the connection cannot be obtained.
+    Obtain and return a connection to the database, or *None* if the connection could not be obtained.
 
     :param errors: incidental error messages
     :param logger: optional logger
     :return: the connection to the database
     """
-    # initialize the return variable
+    # initialize the return valiable
     result: Connection | None = None
 
-    # obtain a connection to the database
+    # obtain the connection string
+    connection_kwargs: str = _get_connection_kwargs()
+
+    # Obtain a connection to the database
     err_msg: str | None = None
     try:
-        result = connect(
-            host=DB_HOST,
-            port=DB_PORT,
-            user=DB_USER,
-            password=DB_PWD
-        )
+        result = connect(connection_kwargs)
     except Exception as e:
-        err_msg = _db_except_msg(e)
+        err_msg = _db_except_msg(exception=e,
+                                 engine="sqlserver")
 
     # log the results
-    _db_log(errors, err_msg, logger, f"Connected to '{DB_NAME}'")
+    name, _user, _pwd, host, _port = _db_get_params("sqlserver")
+    _db_log(errors=errors,
+            err_msg=err_msg,
+            logger=logger,
+            query_stmt=f"Connected to '{name}' at '{host}'")
 
     return result
 
 
 def db_select_all(errors: list[str] | None,
                   sel_stmt: str,
                   where_vals: tuple = None,
@@ -59,47 +60,55 @@
     :param require_max: optionally defines the maximum number of tuples to be returned
     :param logger: optional logger
     :return: list of tuples containing the search result, or [] if the search is empty
     """
     # initialize the return variable
     result: list[tuple] = []
 
-    if isinstance(require_max, int) and require_max > 0:
-        sel_stmt: str = f"{sel_stmt} FETCH NEXT {require_max} ROWS ONLY"
+    # obtain the connection string
+    connection_kwargs: str = _get_connection_kwargs()
 
     err_msg: str | None = None
+    if isinstance(require_max, int) and require_max > 0:
+        sel_stmt: str = sel_stmt.replace("SELECT", f"SELECT TOP {require_max}", 1)
+
     try:
-        # obtain the connection
-        with connect(host=DB_HOST,
-                     port=DB_PORT,
-                     user=DB_USER,
-                     password=DB_PWD) as conn:
+        # obtain a connection
+        with connect(connection_kwargs) as conn:
             # make sure the connection is not in autocommit mode
             conn.autocommit = False
 
-            # obtain a cursor and perform the operation
+            # obtain a cursor and execute the operation
             with conn.cursor() as cursor:
-                # execute the query
-                cursor.execute(statement=sel_stmt,
-                               parameters=where_vals)
+                cursor.execute(sel_stmt, where_vals)
                 # obtain the number of tuples returned
                 count: int = cursor.rowcount
 
                 # has the query quota been satisfied ?
-                if _assert_query_quota(errors, sel_stmt, where_vals, count, require_min, require_max):
+                if _assert_query_quota(errors=errors,
+                                       query=sel_stmt,
+                                       where_vals=where_vals,
+                                       count=count,
+                                       require_min=require_min,
+                                       require_max=require_max):
                     # yes, retrieve the returned tuples
-                    rows: list = cursor.fetchall()
+                    rows: list[Row] = cursor.fetchall()
                     result = [tuple(row) for row in rows]
             # commit the transaction
             conn.commit()
     except Exception as e:
-        err_msg = _db_except_msg(e)
+        err_msg = _db_except_msg(exception=e,
+                                 engine="sqlserver")
 
     # log the results
-    _db_log(errors, err_msg, logger, sel_stmt, where_vals)
+    _db_log(errors=errors,
+            err_msg=err_msg,
+            logger=logger,
+            query_stmt=sel_stmt,
+            bind_vals=where_vals)
 
     return result
 
 
 def db_bulk_insert(errors: list[str] | None,
                    insert_stmt: str,
                    insert_vals: list[tuple],
@@ -112,128 +121,106 @@
     :param insert_vals: the list of values to be inserted
     :param logger: optional logger
     :return: the number of inserted tuples, or None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
+    # obtain the connection string
+    connection_kwargs: str = _get_connection_kwargs()
+
     err_msg: str | None = None
     try:
-        # obtain the connection
-        with connect(host=DB_HOST,
-                     port=DB_PORT,
-                     user=DB_USER,
-                     password=DB_PWD) as conn:
+        # obtain a connection
+        with connect(connection_kwargs) as conn:
             # make sure the connection is not in autocommit mode
             conn.autocommit = False
 
-            # obtain a cursor and perform the operation
+            # obtain the cursor and perform the operation
             with conn.cursor() as cursor:
+                cursor.fast_executemany = True
                 try:
-                    cursor.executemany(statement=insert_stmt,
-                                       parameters=insert_vals)
+                    cursor.executemany(insert_stmt, insert_vals)
                     result = len(insert_vals)
                 except Exception:
                     conn.rollback()
                     raise
             conn.commit()
     except Exception as e:
-        err_msg = _db_except_msg(e)
-
-    # log the results
-    _db_log(errors, err_msg, logger, insert_stmt, insert_vals[0])
-
-    return result
-
-
-# TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
-def db_call_function(errors: list[str] | None,
-                     func_name: str,
-                     func_vals: tuple,
-                     logger: Logger = None) -> list[tuple]:
-    """
-    Execute the stored function *func_name* in the database, with the parameters given in *func_vals*.
-
-    :param errors: incidental error messages
-    :param func_name: name of the stored function
-    :param func_vals: parameters for the stored function
-    :param logger: optional logger
-    :return: the data returned by the function
-    """
-    # initialize the return variable
-    result: list[tuple] = []
-
-    # execute the stored procedure
-    err_msg: str | None = None
-    try:
-        # obtain a connection
-        with connect(host=DB_HOST,
-                     port=DB_PORT,
-                     user=DB_USER,
-                     password=DB_PWD) as conn:
-            # make sure the connection is not in autocommit mode
-            conn.autocommit = False
-            # obtain a cursor and perform the operation
-            with conn.cursor() as cursor:
-                cursor.callproc(name=func_name,
-                                parameters=func_vals)
-                # yes, retrieve the returned tuples
-                result = list(cursor)
-            # commit the transaction
-            conn.commit()
-    except Exception as e:
-        err_msg = _db_except_msg(e)
+        err_msg = _db_except_msg(exception=e,
+                                 engine="sqlserver")
 
     # log the results
-    _db_log(errors, err_msg, logger, func_name, func_vals)
+    _db_log(errors=errors,
+            err_msg=err_msg,
+            logger=logger,
+            query_stmt=insert_stmt,
+            bind_vals=insert_vals[0])
 
     return result
 
 
-# TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
 def db_call_procedure(errors: list[str] | None,
                       proc_name: str,
                       proc_vals: tuple,
+                      require_min: int = None,
+                      require_max: int = None,
                       logger: Logger = None) -> list[tuple]:
     """
     Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
 
     :param errors: incidental error messages
     :param proc_name: name of the stored procedure
     :param proc_vals: parameters for the stored procedure
+    :param require_min: optionally defines the minimum number of tuples to be returned
+    :param require_max: optionally defines the maximum number of tuples to be returned
     :param logger: optional logger
     :return: the data returned by the procedure
     """
     # initialize the return variable
-    result: list[tuple] = []
+    result: list[tuple] | None = None
+
+    # obtain the connection string
+    connection_kwargs: str = _get_connection_kwargs()
+
+    # build the command
+    proc_stmt: str | None = None
 
     # execute the stored procedure
     err_msg: str | None = None
     try:
         # obtain a connection
-        with connect(host=DB_HOST,
-                     port=DB_PORT,
-                     user=DB_USER,
-                     password=DB_PWD) as conn:
+        with connect(connection_kwargs) as conn:
             # make sure the connection is not in autocommit mode
             conn.autocommit = False
-            # obtain a cursor and perform the operation
+            # obtain the cursor and execute the operation
             with conn.cursor() as cursor:
-                cursor.callproc(name=proc_name,
-                                parameters=proc_vals)
+                proc_stmt = f"SET NOCOUNT ON; EXEC {proc_name} {','.join(('?',) * len(proc_vals))}"
+                cursor.execute(proc_stmt, proc_vals)
+                # obtain the number of tuples returned
+                count: int = cursor.rowcount
 
-                # retrieve the returned tuples
-                result = list(cursor)
+                # has the query quota been satisfied ?
+                # noinspection PyTypeChecker
+                if _assert_query_quota(errors, proc_name, None, count, require_min, require_max):
+                    # yes, retrieve the returned tuples
+                    rows: list[Row] = cursor.fetchall()
+                    result = [tuple(row) for row in rows]
             # commit the transaction
             conn.commit()
     except Exception as e:
-        err_msg = _db_except_msg(e)
+        err_msg = _db_except_msg(exception=e,
+                                 engine="sqlserver")
 
     # log the results
-    _db_log(errors, err_msg, logger, proc_name, proc_vals)
+    _db_log(errors=errors,
+            err_msg=err_msg,
+            logger=logger,
+            query_stmt=proc_stmt,
+            bind_vals=proc_vals)
 
     return result
 
 
 def db_modify(errors: list[str] | None,
               modify_stmt: str,
               bind_vals: tuple | list[tuple],
@@ -248,30 +235,44 @@
     :param bind_vals: values for database modification, and for tuples selection
     :param logger: optional logger
     :return: the number of inserted, modified, or deleted tuples, ou None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
+    # obtain the connection string
+    connection_kwargs: str = _get_connection_kwargs()
+
     err_msg: str | None = None
     try:
         # obtain a connection
-        with connect(host=DB_HOST,
-                     port=DB_PORT,
-                     user=DB_USER,
-                     password=DB_PWD) as conn:
+        with connect(connection_kwargs) as conn:
             # make sure the connection is not in autocommit mode
             conn.autocommit = False
             # obtain the cursor and execute the operation
             with conn.cursor() as cursor:
-                cursor.execute(statement=modify_stmt,
-                               parameters=bind_vals)
+                cursor.execute(modify_stmt, bind_vals)
                 result = cursor.rowcount
             # commit the transaction
             conn.commit()
     except Exception as e:
-        err_msg = _db_except_msg(e)
+        err_msg = _db_except_msg(exception=e,
+                                 engine="sqlserver")
 
     # log the results
-    _db_log(errors, err_msg, logger, modify_stmt, bind_vals)
+    _db_log(errors=errors,
+            err_msg=err_msg,
+            logger=logger,
+            query_stmt=modify_stmt,
+            bind_vals=bind_vals)
 
     return result
+
+
+def _get_connection_kwargs() -> str:
+
+    # retrieve the connection parameters
+    name, user, pwd, host, port, driver = _db_get_params("sqlserver")
+    return (
+        f"DRIVER={{{driver}}};SERVER={host},{port};"
+        f"DATABASE={name};UID={user};PWD={pwd};TrustServerCertificate=yes;"
+    )
```

### Comparing `pypomes_db-0.3.9/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.4.0/src/pypomes_db/postgres_pomes.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,49 @@
 from logging import Logger
 from psycopg2 import connect
 from psycopg2.extras import execute_values
 # noinspection PyProtectedMember
 from psycopg2._psycopg import connection
 
 from .db_common import (
-    DB_NAME, DB_HOST, DB_PORT, DB_PWD, DB_USER,
-    _assert_query_quota, _db_log, _db_except_msg
+    _assert_query_quota, _db_get_params, _db_log, _db_except_msg
 )
 
 
 def db_connect(errors: list[str] | None,
                logger: Logger = None) -> connection:
     """
-    Obtain and return a connection to the database, or *None* if the connection cannot be obtained.
+    Obtain and return a connection to the database, or *None* if the connection could not be obtained.
 
     :param errors: incidental error messages
     :param logger: optional logger
     :return: the connection to the database
     """
     # initialize the return variable
     result: connection | None = None
 
+    # retrieve the connection parameters
+    name, user, pwd, host, port = _db_get_params("postgres")
+
     # Obtain a connection to the database
     err_msg: str | None = None
     try:
-        result = connect(host=DB_HOST,
-                         port=DB_PORT,
-                         database=DB_NAME,
-                         user=DB_USER,
-                         password=DB_PWD)
+        result = connect(host=host,
+                         port=port,
+                         database=name,
+                         user=user,
+                         password=pwd)
     except Exception as e:
-        err_msg = _db_except_msg(e)
+        err_msg = _db_except_msg(e, "postgres")
 
     # log the results
-    _db_log(errors, err_msg, logger, f"Connected to '{DB_NAME}'")
+    _db_log(errors=errors,
+            err_msg=err_msg,
+            logger=logger,
+            query_stmt=f"Connected to '{name}' at '{host}'")
 
     return result
 
 
 def db_select_all(errors: list[str] | None,
                   sel_stmt: str,
                   where_vals: tuple = None,
@@ -59,95 +64,116 @@
     :param require_min: optionally defines the minimum number of tuples to be returned
     :param require_max: optionally defines the maximum number of tuples to be returned
     :param logger: optional logger
     :return: list of tuples containing the search result, or [] if the search is empty
     """
     # initialize the return variable
     result: list[tuple] = []
+
+    # retrieve the connection parameters
+    name, user, pwd, host, port = _db_get_params("postgres")
+
     if isinstance(require_max, int) and require_max >= 0:
         sel_stmt += f" LIMIT {require_max}"
 
     err_msg: str | None = None
     try:
         # obtain a connection
-        with connect(host=DB_HOST,
-                     port=DB_PORT,
-                     database=DB_NAME,
-                     user=DB_USER,
-                     password=DB_PWD) as conn:
+        with connect(host=host,
+                     port=port,
+                     database=name,
+                     user=user,
+                     password=pwd) as conn:
             # make sure the connection is not in autocommit mode
             conn.autocommit = False
 
             # obtain a cursor and execute the operation
             with conn.cursor() as cursor:
                 cursor.execute(query=f"{sel_stmt};",
                                vars=where_vals)
                 # obtain the number of tuples returned
                 count: int = cursor.rowcount
 
                 # has the query quota been satisfied ?
-                if _assert_query_quota(errors, sel_stmt, where_vals, count, require_min, require_max):
+                if _assert_query_quota(errors=errors,
+                                       query=sel_stmt,
+                                       where_vals=where_vals,
+                                       count=count,
+                                       require_min=require_min,
+                                       require_max=require_max):
                     # yes, retrieve the returned tuples
                     result = list(cursor)
 
             # commit the transaction
             conn.commit()
     except Exception as e:
-        err_msg = _db_except_msg(e)
+        err_msg = _db_except_msg(exception=e,
+                                 engine="postgres")
 
     # log the results
-    _db_log(errors, err_msg, logger, sel_stmt, where_vals)
+    _db_log(errors=errors,
+            err_msg=err_msg,
+            logger=logger,
+            query_stmt=sel_stmt,
+            bind_vals=where_vals)
 
     return result
 
 
 def db_bulk_insert(errors: list[str] | None,
                    insert_stmt: str,
                    insert_vals: list[tuple],
                    logger: Logger = None) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
-    The 'VALUES' clause in *insert_stmt' must be simply 'VALUES %s'.
-    Note that, after the execution of 'execute_values', the 'cursor.rowcount' property
+    The *VALUES* clause in *insert_stmt* must be simply *VALUES %s*.
+    Note that, after the execution of *execute_values*, the *cursor.rowcount* property
     will not contain a total result, and thus the value 1 (one) is returned on success.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the list of values to be inserted
     :param logger: optional logger
     :return: the number of inserted tuples, or None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
+    # retrieve the connection parameters
+    name, user, pwd, host, port = _db_get_params("postgres")
+
     # execute the bulk insert
     err_msg: str | None = None
     try:
         # obtain a connection
-        with connect(host=DB_HOST,
-                     port=DB_PORT,
-                     database=DB_NAME,
-                     user=DB_USER,
-                     password=DB_PWD) as conn:
+        with connect(host=host,
+                     port=port,
+                     database=name,
+                     user=user,
+                     password=pwd) as conn:
             # make sure the connection is not in autocommit mode
             conn.autocommit = False
             # obtain a cursor and perform the operation
             with conn.cursor() as cursor:
                 execute_values(cur=cursor,
                                sql=insert_stmt,
                                argslist=insert_vals)
                 result = len(insert_vals)
             # commit the transaction
             conn.commit()
     except Exception as e:
-        err_msg = _db_except_msg(e)
+        err_msg = _db_except_msg(exception=e,
+                                 engine="postgres")
 
     # log the results
-    _db_log(errors, err_msg, logger, insert_stmt)
+    _db_log(errors=errors,
+            err_msg=err_msg,
+            logger=logger,
+            query_stmt=insert_stmt)
 
     return result
 
 
 def db_call_procedure(errors: list[str] | None,
                       proc_name: str,
                       proc_vals: tuple,
@@ -160,42 +186,50 @@
     :param proc_vals: the arguments to be passed
     :param logger: optional logger
     :return: the data returned by the procedure
     """
     # initialize the return variable
     result: list[tuple] = [()]
 
+    # retrieve the connection parameters
+    name, user, pwd, host, port = _db_get_params("postgres")
+
     # build the command
     proc_stmt: str = f"{proc_name}(" + "%s, " * (len(proc_vals) - 1) + "%s)"
 
     # execute the stored procedure
     err_msg: str | None = None
     try:
         # obtain a connection
-        with connect(host=DB_HOST,
-                     port=DB_PORT,
-                     database=DB_NAME,
-                     user=DB_USER,
-                     password=DB_PWD) as conn:
+        with connect(host=host,
+                     port=port,
+                     database=name,
+                     user=user,
+                     password=pwd) as conn:
             # make sure the connection is not in autocommit mode
             conn.autocommit = False
 
             # obtain a cursor and perform the operation
             with conn.cursor() as cursor:
                 cursor.execute(query=proc_stmt,
                                argslist=proc_vals)
                 # retrieve the returned tuples
                 result = list(cursor)
             # commit the transaction
             conn.commit()
     except Exception as e:
-        err_msg = _db_except_msg(e)
+        err_msg = _db_except_msg(exception=e,
+                                 engine="postgres")
 
     # log the results
-    _db_log(errors, err_msg, logger, proc_stmt, proc_vals)
+    _db_log(errors=errors,
+            err_msg=err_msg,
+            logger=logger,
+            query_stmt=proc_stmt,
+            bind_vals=proc_vals)
 
     return result
 
 
 def db_modify(errors: list[str] | None,
               modify_stmt: str,
               bind_vals: tuple | list[tuple],
@@ -210,31 +244,39 @@
     :param bind_vals: values for database modification, and for tuples selection
     :param logger: optional logger
     :return: the number of inserted, modified, or deleted tuples, ou None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
+    # retrieve the connection parameters
+    name, user, pwd, host, port = _db_get_params("postgres")
+
     err_msg: str | None = None
     try:
         # obtain a connection
-        with connect(host=DB_HOST,
-                     port=DB_PORT,
-                     database=DB_NAME,
-                     user=DB_USER,
-                     password=DB_PWD) as conn:
+        with connect(host=host,
+                     port=port,
+                     database=name,
+                     user=user,
+                     password=pwd) as conn:
             # make sure the connection is not in autocommit mode
             conn.autocommit = False
             # obtain the cursor and execute the operation
             with conn.cursor() as cursor:
                 cursor.execute(query=f"{modify_stmt};",
                                vars=bind_vals)
                 result = cursor.rowcount
             # commit the transaction
             conn.commit()
     except Exception as e:
-        err_msg = _db_except_msg(e)
+        err_msg = _db_except_msg(exception=e,
+                                 engine="postgres")
 
     # log the results
-    _db_log(errors, err_msg, logger, modify_stmt, bind_vals)
+    _db_log(errors=errors,
+            err_msg=err_msg,
+            logger=logger,
+            query_stmt=modify_stmt,
+            bind_vals=bind_vals)
 
     return result
```

### Comparing `pypomes_db-0.3.9/LICENSE` & `pypomes_db-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.3.9/pyproject.toml` & `pypomes_db-0.4.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.3.9"
+version = "0.4.0"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "pip>=24.0",
-#   "oracledb>=2.1.1",
+#   "oracledb>=2.1.2",
 #   "psycopg2-binary>=2.9.9",
 #   "pyodbc>=5.1.0",
-    "pypomes_core>=0.8.7",
+    "pypomes_core>=0.9.6",
     "setuptools>=68.0.0",
     "wheel>=0.42.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-DB"
 "Bug Tracker" = "https://github.com/TheWiseCoder/PyPomes-DB/issues"
```

### Comparing `pypomes_db-0.3.9/PKG-INFO` & `pypomes_db-0.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.3.9
+Version: 0.4.0
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: pip>=24.0
-Requires-Dist: pypomes-core>=0.8.7
+Requires-Dist: pypomes-core>=0.9.6
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.42.0
```

