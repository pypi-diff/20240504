# Comparing `tmp/sfconn-0.3.0.tar.gz` & `tmp/sfconn-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sfconn-0.3.0.tar", last modified: Fri Feb  9 21:57:43 2024, max compression
+gzip compressed data, was "sfconn-0.3.1.tar", last modified: Sat May  4 21:19:20 2024, max compression
```

## Comparing `sfconn-0.3.0.tar` & `sfconn-0.3.1.tar`

### file list

```diff
@@ -1,30 +1,25 @@
-drwxr-xr-x   0 padhia    (1000) users      (100)        0 2024-02-09 21:57:43.382663 sfconn-0.3.0/
--rw-r--r--   0 padhia    (1000) users      (100)      107 2024-02-09 21:28:34.000000 sfconn-0.3.0/.editorconfig
-drwxr-xr-x   0 padhia    (1000) users      (100)        0 2024-02-09 21:57:43.380663 sfconn-0.3.0/.github/
-drwxr-xr-x   0 padhia    (1000) users      (100)        0 2024-02-09 21:57:43.380663 sfconn-0.3.0/.github/workflows/
--rw-r--r--   0 padhia    (1000) users      (100)      682 2024-02-09 21:28:34.000000 sfconn-0.3.0/.github/workflows/release.yaml
--rw-r--r--   0 padhia    (1000) users      (100)       20 2024-02-09 21:29:35.000000 sfconn-0.3.0/.gitignore
--rw-r--r--   0 padhia    (1000) users      (100)     7013 2024-02-09 21:57:43.381663 sfconn-0.3.0/PKG-INFO
--rw-r--r--   0 padhia    (1000) users      (100)     6515 2024-02-09 21:44:54.000000 sfconn-0.3.0/README.md
--rw-r--r--   0 padhia    (1000) users      (100)      765 2024-02-09 21:44:54.000000 sfconn-0.3.0/pyproject.toml
--rw-r--r--   0 padhia    (1000) users      (100)       38 2024-02-09 21:57:43.382663 sfconn-0.3.0/setup.cfg
-drwxr-xr-x   0 padhia    (1000) users      (100)        0 2024-02-09 21:57:43.380663 sfconn-0.3.0/sfconn/
--rw-r--r--   0 padhia    (1000) users      (100)      654 2024-02-09 21:44:54.000000 sfconn-0.3.0/sfconn/__init__.py
--rw-r--r--   0 padhia    (1000) users      (100)     3873 2024-02-09 21:44:54.000000 sfconn-0.3.0/sfconn/conn.py
--rw-r--r--   0 padhia    (1000) users      (100)     5208 2024-02-09 21:29:35.000000 sfconn-0.3.0/sfconn/cursor.py
--rw-r--r--   0 padhia    (1000) users      (100)     2219 2024-02-09 21:44:54.000000 sfconn-0.3.0/sfconn/jwt.py
--rw-r--r--   0 padhia    (1000) users      (100)     1561 2024-02-09 21:28:34.000000 sfconn-0.3.0/sfconn/privkey.py
--rw-r--r--   0 padhia    (1000) users      (100)        0 2024-02-09 21:28:34.000000 sfconn-0.3.0/sfconn/py.typed
--rw-r--r--   0 padhia    (1000) users      (100)     4453 2024-02-09 21:44:54.000000 sfconn-0.3.0/sfconn/utils.py
-drwxr-xr-x   0 padhia    (1000) users      (100)        0 2024-02-09 21:57:43.381663 sfconn-0.3.0/sfconn.egg-info/
--rw-r--r--   0 padhia    (1000) users      (100)     7013 2024-02-09 21:57:43.000000 sfconn-0.3.0/sfconn.egg-info/PKG-INFO
--rw-r--r--   0 padhia    (1000) users      (100)      438 2024-02-09 21:57:43.000000 sfconn-0.3.0/sfconn.egg-info/SOURCES.txt
--rw-r--r--   0 padhia    (1000) users      (100)        1 2024-02-09 21:57:43.000000 sfconn-0.3.0/sfconn.egg-info/dependency_links.txt
--rw-r--r--   0 padhia    (1000) users      (100)       82 2024-02-09 21:57:43.000000 sfconn-0.3.0/sfconn.egg-info/requires.txt
--rw-r--r--   0 padhia    (1000) users      (100)        7 2024-02-09 21:57:43.000000 sfconn-0.3.0/sfconn.egg-info/top_level.txt
--rw-r--r--   0 padhia    (1000) users      (100)      490 2024-02-09 21:44:54.000000 sfconn-0.3.0/sfconn.nix
-drwxr-xr-x   0 padhia    (1000) users      (100)        0 2024-02-09 21:57:43.381663 sfconn-0.3.0/tests/
--rw-r--r--   0 padhia    (1000) users      (100)      341 2024-02-09 21:44:54.000000 sfconn-0.3.0/tests/test_conn.py
--rw-r--r--   0 padhia    (1000) users      (100)     2220 2024-02-09 21:29:35.000000 sfconn-0.3.0/tests/test_cursor.py
--rw-r--r--   0 padhia    (1000) users      (100)      728 2024-02-09 21:29:35.000000 sfconn-0.3.0/tests/test_decorators.py
--rw-r--r--   0 padhia    (1000) users      (100)      310 2024-02-09 21:44:54.000000 sfconn-0.3.0/tests/test_jwt.py
+drwxr-xr-x   0 padhia     (501) staff       (20)        0 2024-05-04 21:19:20.307125 sfconn-0.3.1/
+-rw-r--r--   0 padhia     (501) staff       (20)     7362 2024-05-04 21:19:20.306873 sfconn-0.3.1/PKG-INFO
+-rw-r--r--   0 padhia     (501) staff       (20)     6826 2024-05-04 21:08:28.000000 sfconn-0.3.1/README.md
+-rw-r--r--   0 padhia     (501) staff       (20)      830 2024-05-04 21:08:28.000000 sfconn-0.3.1/pyproject.toml
+-rw-r--r--   0 padhia     (501) staff       (20)       38 2024-05-04 21:19:20.307175 sfconn-0.3.1/setup.cfg
+drwxr-xr-x   0 padhia     (501) staff       (20)        0 2024-05-04 21:19:20.303217 sfconn-0.3.1/sfconn/
+-rw-r--r--   0 padhia     (501) staff       (20)      745 2024-05-04 21:08:28.000000 sfconn-0.3.1/sfconn/__init__.py
+-rw-r--r--   0 padhia     (501) staff       (20)     5245 2024-05-04 21:08:28.000000 sfconn-0.3.1/sfconn/conn.py
+-rw-r--r--   0 padhia     (501) staff       (20)     7029 2024-05-04 21:08:28.000000 sfconn-0.3.1/sfconn/cursor.py
+-rw-r--r--   0 padhia     (501) staff       (20)     2236 2024-05-04 21:08:28.000000 sfconn-0.3.1/sfconn/jwt.py
+-rw-r--r--   0 padhia     (501) staff       (20)     1562 2024-05-04 21:08:28.000000 sfconn-0.3.1/sfconn/privkey.py
+-rw-r--r--   0 padhia     (501) staff       (20)        0 2024-04-13 17:14:28.000000 sfconn-0.3.1/sfconn/py.typed
+-rw-r--r--   0 padhia     (501) staff       (20)     7665 2024-05-04 21:08:28.000000 sfconn-0.3.1/sfconn/utils.py
+drwxr-xr-x   0 padhia     (501) staff       (20)        0 2024-05-04 21:19:20.306307 sfconn-0.3.1/sfconn.egg-info/
+-rw-r--r--   0 padhia     (501) staff       (20)     7362 2024-05-04 21:19:20.000000 sfconn-0.3.1/sfconn.egg-info/PKG-INFO
+-rw-r--r--   0 padhia     (501) staff       (20)      392 2024-05-04 21:19:20.000000 sfconn-0.3.1/sfconn.egg-info/SOURCES.txt
+-rw-r--r--   0 padhia     (501) staff       (20)        1 2024-05-04 21:19:20.000000 sfconn-0.3.1/sfconn.egg-info/dependency_links.txt
+-rw-r--r--   0 padhia     (501) staff       (20)       93 2024-05-04 21:19:20.000000 sfconn-0.3.1/sfconn.egg-info/requires.txt
+-rw-r--r--   0 padhia     (501) staff       (20)        7 2024-05-04 21:19:20.000000 sfconn-0.3.1/sfconn.egg-info/top_level.txt
+drwxr-xr-x   0 padhia     (501) staff       (20)        0 2024-05-04 21:19:20.305805 sfconn-0.3.1/tests/
+-rw-r--r--   0 padhia     (501) staff       (20)      330 2024-05-04 21:08:28.000000 sfconn-0.3.1/tests/test_conn.py
+-rw-r--r--   0 padhia     (501) staff       (20)     2529 2024-05-04 21:08:28.000000 sfconn-0.3.1/tests/test_cursor.py
+-rw-r--r--   0 padhia     (501) staff       (20)      729 2024-05-04 21:08:28.000000 sfconn-0.3.1/tests/test_decorators.py
+-rw-r--r--   0 padhia     (501) staff       (20)      311 2024-05-04 21:08:28.000000 sfconn-0.3.1/tests/test_jwt.py
+-rw-r--r--   0 padhia     (501) staff       (20)     1885 2024-05-04 21:08:28.000000 sfconn-0.3.1/tests/test_pytype.py
```

### Comparing `sfconn-0.3.0/PKG-INFO` & `sfconn-0.3.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,80 @@
 Metadata-Version: 2.1
 Name: sfconn
-Version: 0.3.0
+Version: 0.3.1
 Summary: Snowflake connection helper functions
 Author-email: Paresh Adhia <padhia+github@gmail.com>
+Project-URL: Homepage, https://github.com/padhia/sfconn
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: snowflake-connector-python>=3.7.0
-Provides-Extra: keyring
-Requires-Dist: keyring; extra == "keyring"
-Provides-Extra: jwt
-Requires-Dist: pyjwt; extra == "jwt"
-Provides-Extra: tests
-Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pyjwt
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Provides-Extra: snowpark
+Requires-Dist: snowflake-snowpark-python; extra == "snowpark"
+
+# sfconn
 
 [![PyPi](https://img.shields.io/pypi/v/sfconn.svg)](https://pypi.python.org/pypi/sfconn) [![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT) ![Python3.11+](https://img.shields.io/badge/dynamic/json?query=info.requires_python&label=python&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fsfconn%2Fjson)
 
 Snowflake connection helper functions
 
 A Python library to simplify connecting to Snowflake databases
 
 **Notes**
-1. This is a major version upgrade and breaks compatibility with the previous versions (< `0.3.0`). `sfconn` now relies on `snowflake-python-connector` for accessing named connections (e.g. `connections.toml`). If you still need the ability use named connections from `~/.snowflake/config`, please continue using older version (`0.2.x`).
-1. `sfconn` modifies the way `private_key_file` connection option is evaluated in the following ways:
-    - with `--keyfile-anchor` option (default `$SFCONN_KEYFILE_ANCHOR`): uses the supplied value to anchor any relative paths (v/s anchoring paths relative to current working directory of the running process)
-    - with `--keyfile-strip-pfx` option (default `$SFCONN_KEYFILE_STRIP_PFX` ): strips the specified prefix from the path values (so `--keyfile-anchor` option can be used)
+1. This is a major version upgrade and breaks compatibility with the previous versions (< `0.3.0`). `sfconn` now relies on `snowflake-python-connector` for accessing named connections ([`connections.toml`](https://docs.snowflake.com/en/developer-guide/python-connector/python-connector-connect#connecting-using-the-connections-toml-file)).
+1. `sfconn` optionally modifies the way `private_key_file` connection option is evaluated. When `--keyfile-pfx-map` option is specified, or if `$SFCONN_KEYFILE_PFX_MAP` is set, (option value must be a pair of source and target paths separated by `:`). `private_key_file` option, if present and begins with the source path, it is temporarily modified as if it begins with the target path. Primary use-case is to be able to maintain one copy of `connections.toml` file across different execution environments, such as within containers.
 
-# Installation
+## Installation
 
 Use Python's standard `pip` utility for installation:
 
 ```sh
 pip install --upgrade sfconn
 ```
 
-# Usage
+## Usage
+
+### `getconn()` and `getsess()`
 
-## `getconn()`
+`getconn` and `getsess` are wrapper functions over native Snowflake functions with added functionality (mainly mapping `private_key_file` value as described above).
+
+**Note:** `getsess` is meant to work with *Snowpark* applications. As such, it will raise a `NotImplementedError` exception if `snowflake-snowpark-python` package is not available.
 
 **Usage:**
 ```python
-def getconn(connection_name: str | None, **overrides: dict[str, Any]) -> Connection
+def getconn(connection_name: str | None, **overrides: dict[str, Any]) -> Connection:
+def getsess(connection_name: str | None, **overrides: dict[str, Any]) -> Session:
 ```
 
-`getconn` accepts a connection name and returns a connection object with modified behavior as noted above.
-
-**Example:**
+`getconn` and `getsess` accept a connection name and return a connection or session object respectively with modified behavior as noted above.
 
+**Examples:**
 ```python
 from sfconn import getconn
 
-# assuming 'dev' is a connection defined in ~/.snowflake/config
+# assuming 'dev' is a named connection defined in connections.toml
 with getconn('dev', schema='PUBLIC') as cnx:
     with cnx.cursor() as csr:
         csr.execute('SELECT CURRENT_USER()')
         print("Hello " + csr.fetchone()[0])
 ```
 
-## `conn_opts()`
-
-**Usage:**
-```python
-def conn_opts(name: str | None , **overrides: dict[str, Any]) -> dict[str, Any]
-```
-
-`conn_opts`, returns a Python `dict` object populated with options and values. This can be useful passing as an argument to `snowflake.snowpark.Session.builder.configs()` method.
-
-**Example:**
-
 ```python
-from sfconn import conn_opts
-from snowflake.snowpark import Session
+from sfconn import getsess
 
-# assuming 'dev' is a connection defined in ~/.snowflake/config
-session = Session.builder.configs(conn_opts('dev')).create()
+# assuming 'dev' is a named connection defined in connections.toml
+with getsess('dev', schema='PUBLIC') as session:
+    df = sess.sql("select current_user() as curr_user, current_role() as curr_role")
+    print(df.collect())
 ```
 
-## `run_query*()`
+### `run_query*()`
 
 Cursor objects add a family of few convenience methods that return an `Iterable` of values instead of generic `tuple` or `dict`.
 
 1. `<cursor>.run_query(<callable>|<class>, <sql> [,<params>])`: Returns an Iterable of values.
     - `<callable>` is a mapping function that shall accept all column values of a row as individual arguments, in order, and returns a value that will be used for `Iterable`.
     - `<class>` is any Python class whose attribute names, after upper-casing, are treated as column names from the result set. `<class>` can include only a subset of a all available column from the query result as attributes and in a different order than the query.
 1. `<cursor>.run_query1(<callable>|<class>, <sql> [,<params>])`: Similar to `run_query`, except returns a single value. Note, if at least one value is not available, raises `ProgrammingError` exception.
@@ -113,63 +107,63 @@
 with getconn() as cnx, cnx.cursor() as csr:
     result = csr.run_query1(
         Result,
         "select current_user() as user, current_date() as date, current_warehouse() as wh_name"
     )
 ```
 
-## Decorator functions
+### Decorator Functions
 
-Python scripts that accept command-line parameters and use `argparse` library, can use decorator functions to further reduce boilerplate code needed for setting up common Snowflake connection options as command-line arguments
+Python command-line scripts that use `argparse` library, can use decorator functions to further reduce boilerplate code needed for setting up a Snowflake connection and error checking
 
 ```python
 def with_connection_args(doc: str | None) -> Callable[[argparse.ArgumentParser], None]:
 def with_connection(logger = None) -> Callable[[Connection, ...], None]:
-def with_connection_option(logger = None) => Callable([dict[str, Any, ...]])
+def with_session(logger = None) -> Callable[[Session, ...], None]:
 ```
 
 `with_connection_args()` decorator function:
 1. builds an `ArgumentParser` object
-1. adds common Snowflake connection options as arguments that allow overriding values specified in `~/.snowsql/config`
+1. adds common Snowflake connection options as arguments including overriding role, database, schema and warehouse
 1. calls the decorated function with the parser object to allow adding any script specific options
 
 `with_connection()` decorator function:
-1. consumes standard Snowflake connection options (specified with `args()`)
+1. consumes standard Snowflake connection options (specified with `with_connection_args()`)
 1. creates a connection object
 1. calls the decorated function with a connection object as first parameter and any other script specific options that were specified on command line
 
-`with_connection_option()` decorator function:
-- Similar to `entry()` but passes a `dict` of options as the first parameter. This is useful for passing options to the `snowflake.snowpark.Session.builder.configs()` method
+`with_session()` decorator function:
+1. Similar to `with_connection()` but creates a `snowflake.snowpark.Session` object instead of a connection object
+1. **Note:** this decorator will raise an `NotImplementedError` exception if `snowflake-snowpark-python` package is not available.
 
 **Example:**
 
 ```python
-from sfconn import args, entry
+from sfconn import with_connection_args, with_connection
 
-@entry
+@with_connection
 def main(con, show_account: bool):
     with con.cursor() as csr:
         csr.execute('SELECT CURRENT_USER()')
         print("Hello " + csr.fetchone()[0])
         if show_account:
             csr.execute("SELECT CURRENT_ACCOUNT()")
             print("You are connected to account: " + csr.fetchone()[0])
 
-@args("Sample application that greets the current Snowflake user")
+@with_connection_args("Sample application that greets the current Snowflake user")
 def getargs(parser):
     parser.add_argument("-a", "--show-account", action='store_true', help="show snowflake account name")
 
 if __name__ == '__main__':
     main(**vars(getargs()))
 ```
 
-## `get_token()`
+### `get_token()`
 
 Function `sfconn.get_token()` returns a JWT token for connections that use `private_key_path` option. An optional lifetime value can be specified (default 54 minutes)
 
 **Example:**
 
 ```python
 from sfconn import get_token
-
-# assuming 'dev' is a connection defined in ~/.snowflake/config and uses key-pair authentication
-jwt_token = get_token('dev', 120)  # get a token valid for 120 minutes
+jwt_token = get_token(None, 120)  # get token using default (None) connection, and valid for 120 minutes
+```
```

### Comparing `sfconn-0.3.0/README.md` & `sfconn-0.3.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,64 @@
+# sfconn
+
 [![PyPi](https://img.shields.io/pypi/v/sfconn.svg)](https://pypi.python.org/pypi/sfconn) [![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT) ![Python3.11+](https://img.shields.io/badge/dynamic/json?query=info.requires_python&label=python&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fsfconn%2Fjson)
 
 Snowflake connection helper functions
 
 A Python library to simplify connecting to Snowflake databases
 
 **Notes**
-1. This is a major version upgrade and breaks compatibility with the previous versions (< `0.3.0`). `sfconn` now relies on `snowflake-python-connector` for accessing named connections (e.g. `connections.toml`). If you still need the ability use named connections from `~/.snowflake/config`, please continue using older version (`0.2.x`).
-1. `sfconn` modifies the way `private_key_file` connection option is evaluated in the following ways:
-    - with `--keyfile-anchor` option (default `$SFCONN_KEYFILE_ANCHOR`): uses the supplied value to anchor any relative paths (v/s anchoring paths relative to current working directory of the running process)
-    - with `--keyfile-strip-pfx` option (default `$SFCONN_KEYFILE_STRIP_PFX` ): strips the specified prefix from the path values (so `--keyfile-anchor` option can be used)
+1. This is a major version upgrade and breaks compatibility with the previous versions (< `0.3.0`). `sfconn` now relies on `snowflake-python-connector` for accessing named connections ([`connections.toml`](https://docs.snowflake.com/en/developer-guide/python-connector/python-connector-connect#connecting-using-the-connections-toml-file)).
+1. `sfconn` optionally modifies the way `private_key_file` connection option is evaluated. When `--keyfile-pfx-map` option is specified, or if `$SFCONN_KEYFILE_PFX_MAP` is set, (option value must be a pair of source and target paths separated by `:`). `private_key_file` option, if present and begins with the source path, it is temporarily modified as if it begins with the target path. Primary use-case is to be able to maintain one copy of `connections.toml` file across different execution environments, such as within containers.
 
-# Installation
+## Installation
 
 Use Python's standard `pip` utility for installation:
 
 ```sh
 pip install --upgrade sfconn
 ```
 
-# Usage
+## Usage
+
+### `getconn()` and `getsess()`
 
-## `getconn()`
+`getconn` and `getsess` are wrapper functions over native Snowflake functions with added functionality (mainly mapping `private_key_file` value as described above).
+
+**Note:** `getsess` is meant to work with *Snowpark* applications. As such, it will raise a `NotImplementedError` exception if `snowflake-snowpark-python` package is not available.
 
 **Usage:**
 ```python
-def getconn(connection_name: str | None, **overrides: dict[str, Any]) -> Connection
+def getconn(connection_name: str | None, **overrides: dict[str, Any]) -> Connection:
+def getsess(connection_name: str | None, **overrides: dict[str, Any]) -> Session:
 ```
 
-`getconn` accepts a connection name and returns a connection object with modified behavior as noted above.
-
-**Example:**
+`getconn` and `getsess` accept a connection name and return a connection or session object respectively with modified behavior as noted above.
 
+**Examples:**
 ```python
 from sfconn import getconn
 
-# assuming 'dev' is a connection defined in ~/.snowflake/config
+# assuming 'dev' is a named connection defined in connections.toml
 with getconn('dev', schema='PUBLIC') as cnx:
     with cnx.cursor() as csr:
         csr.execute('SELECT CURRENT_USER()')
         print("Hello " + csr.fetchone()[0])
 ```
 
-## `conn_opts()`
-
-**Usage:**
-```python
-def conn_opts(name: str | None , **overrides: dict[str, Any]) -> dict[str, Any]
-```
-
-`conn_opts`, returns a Python `dict` object populated with options and values. This can be useful passing as an argument to `snowflake.snowpark.Session.builder.configs()` method.
-
-**Example:**
-
 ```python
-from sfconn import conn_opts
-from snowflake.snowpark import Session
+from sfconn import getsess
 
-# assuming 'dev' is a connection defined in ~/.snowflake/config
-session = Session.builder.configs(conn_opts('dev')).create()
+# assuming 'dev' is a named connection defined in connections.toml
+with getsess('dev', schema='PUBLIC') as session:
+    df = sess.sql("select current_user() as curr_user, current_role() as curr_role")
+    print(df.collect())
 ```
 
-## `run_query*()`
+### `run_query*()`
 
 Cursor objects add a family of few convenience methods that return an `Iterable` of values instead of generic `tuple` or `dict`.
 
 1. `<cursor>.run_query(<callable>|<class>, <sql> [,<params>])`: Returns an Iterable of values.
     - `<callable>` is a mapping function that shall accept all column values of a row as individual arguments, in order, and returns a value that will be used for `Iterable`.
     - `<class>` is any Python class whose attribute names, after upper-casing, are treated as column names from the result set. `<class>` can include only a subset of a all available column from the query result as attributes and in a different order than the query.
 1. `<cursor>.run_query1(<callable>|<class>, <sql> [,<params>])`: Similar to `run_query`, except returns a single value. Note, if at least one value is not available, raises `ProgrammingError` exception.
@@ -97,63 +91,63 @@
 with getconn() as cnx, cnx.cursor() as csr:
     result = csr.run_query1(
         Result,
         "select current_user() as user, current_date() as date, current_warehouse() as wh_name"
     )
 ```
 
-## Decorator functions
+### Decorator Functions
 
-Python scripts that accept command-line parameters and use `argparse` library, can use decorator functions to further reduce boilerplate code needed for setting up common Snowflake connection options as command-line arguments
+Python command-line scripts that use `argparse` library, can use decorator functions to further reduce boilerplate code needed for setting up a Snowflake connection and error checking
 
 ```python
 def with_connection_args(doc: str | None) -> Callable[[argparse.ArgumentParser], None]:
 def with_connection(logger = None) -> Callable[[Connection, ...], None]:
-def with_connection_option(logger = None) => Callable([dict[str, Any, ...]])
+def with_session(logger = None) -> Callable[[Session, ...], None]:
 ```
 
 `with_connection_args()` decorator function:
 1. builds an `ArgumentParser` object
-1. adds common Snowflake connection options as arguments that allow overriding values specified in `~/.snowsql/config`
+1. adds common Snowflake connection options as arguments including overriding role, database, schema and warehouse
 1. calls the decorated function with the parser object to allow adding any script specific options
 
 `with_connection()` decorator function:
-1. consumes standard Snowflake connection options (specified with `args()`)
+1. consumes standard Snowflake connection options (specified with `with_connection_args()`)
 1. creates a connection object
 1. calls the decorated function with a connection object as first parameter and any other script specific options that were specified on command line
 
-`with_connection_option()` decorator function:
-- Similar to `entry()` but passes a `dict` of options as the first parameter. This is useful for passing options to the `snowflake.snowpark.Session.builder.configs()` method
+`with_session()` decorator function:
+1. Similar to `with_connection()` but creates a `snowflake.snowpark.Session` object instead of a connection object
+1. **Note:** this decorator will raise an `NotImplementedError` exception if `snowflake-snowpark-python` package is not available.
 
 **Example:**
 
 ```python
-from sfconn import args, entry
+from sfconn import with_connection_args, with_connection
 
-@entry
+@with_connection
 def main(con, show_account: bool):
     with con.cursor() as csr:
         csr.execute('SELECT CURRENT_USER()')
         print("Hello " + csr.fetchone()[0])
         if show_account:
             csr.execute("SELECT CURRENT_ACCOUNT()")
             print("You are connected to account: " + csr.fetchone()[0])
 
-@args("Sample application that greets the current Snowflake user")
+@with_connection_args("Sample application that greets the current Snowflake user")
 def getargs(parser):
     parser.add_argument("-a", "--show-account", action='store_true', help="show snowflake account name")
 
 if __name__ == '__main__':
     main(**vars(getargs()))
 ```
 
-## `get_token()`
+### `get_token()`
 
 Function `sfconn.get_token()` returns a JWT token for connections that use `private_key_path` option. An optional lifetime value can be specified (default 54 minutes)
 
 **Example:**
 
 ```python
 from sfconn import get_token
-
-# assuming 'dev' is a connection defined in ~/.snowflake/config and uses key-pair authentication
-jwt_token = get_token('dev', 120)  # get a token valid for 120 minutes
+jwt_token = get_token(None, 120)  # get token using default (None) connection, and valid for 120 minutes
+```
```

### Comparing `sfconn-0.3.0/pyproject.toml` & `sfconn-0.3.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -6,33 +6,34 @@
 name = "sfconn"
 authors = [
     {name = "Paresh Adhia", email = "padhia+github@gmail.com"},
 ]
 description = "Snowflake connection helper functions"
 readme = "README.md"
 requires-python = ">=3.11"
-classifiers = [
-    "Programming Language :: Python :: 3",
-]
+classifiers = ["Programming Language :: Python :: 3"]
 dependencies = [
     "snowflake-connector-python>=3.7.0",
+    "pyjwt",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
-keyring = ["keyring"]
-jwt = ["pyjwt"]
-tests = ["pytest"]
+test = ["pytest"]
+snowpark = ["snowflake-snowpark-python"]
+
+[project.urls]
+Homepage = "https://github.com/padhia/sfconn"
+
+[tool.setuptools]
+packages = ["sfconn"]
 
 [tool.setuptools.dynamic]
 version = {attr = "sfconn.__version__"}
 
-[tool.setuptools.package-data]
-"*" = ["py.typed"]
-
 [tool.ruff]
 line-length = 130
 target-version = "py311"
-extend-select = ["I"]
+lint.extend-select = ["I"]
 
 [tool.pytest.ini_options]
 pythonpath = [ "." ]
```

### Comparing `sfconn-0.3.0/sfconn/__init__.py` & `sfconn-0.3.1/sfconn/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 "connection package"
-__version__ = "0.3.0"
 
-from snowflake.connector import DatabaseError, InterfaceError, ProgrammingError
+__version__ = "0.3.1"
+
+from snowflake.connector import DatabaseError, DataError, InterfaceError, ProgrammingError
 from snowflake.connector.cursor import ResultMetadata
 
-from .conn import Connection, Cursor, conn_opts, connection_names, getconn
+from .conn import Connection, Cursor, available_connections, default_connection_name, getconn, getsess
 from .jwt import get_token
-from .utils import with_connection, with_connection_args, with_connection_options
+from .utils import pytype, with_connection, with_connection_args, with_session
 
 __all__ = [
-    "conn_opts",
-    "getconn",
-    "connection_names",
-    "get_token",
-    "Connection",
-    "ResultMetadata",
-    "Cursor",
     "DatabaseError",
-    "ProgrammingError",
+    "DataError",
     "InterfaceError",
-    "with_connection_args",
+    "ProgrammingError",
+    "ResultMetadata",
+    "Connection",
+    "Cursor",
+    "available_connections",
+    "default_connection_name",
+    "getconn",
+    "getsess",
+    "get_token",
+    "pytype",
     "with_connection",
-    "with_connection_options",
+    "with_connection_args",
+    "with_session",
 ]
```

### Comparing `sfconn-0.3.0/sfconn/conn.py` & `sfconn-0.3.1/sfconn/conn.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 "get a snowflake connection using connections.toml configuration with added convenience methods"
+
 from __future__ import annotations
 
 import logging
 import os
 from pathlib import Path
 from typing import Any, Self, cast
 
 from snowflake.connector.config_manager import CONFIG_MANAGER
-from snowflake.connector.connection import SnowflakeConnection, SnowflakeCursor
+from snowflake.connector.connection import SnowflakeConnection
+from snowflake.connector.cursor import SnowflakeCursor
 from snowflake.connector.errors import Error
 
 from .cursor import Cursor
 
 logger = logging.getLogger(__name__)
 
 
@@ -40,33 +42,42 @@
     def __exit__(self, *args: Any, **kwargs: Any):
         return super().__exit__(*args, **kwargs)
 
     def cursor(self, cursor_class: type[SnowflakeCursor] = Cursor) -> Cursor:
         return cast(Cursor, super().cursor(cursor_class))
 
 
-def connection_names() -> list[str]:
-    """returns names of available connections
+def available_connections() -> dict[str, dict[str, int | str]]:
+    """returns available connections
+    Returns:
+        dict of connection name and connection options
+    """
+    return cast(dict[str, dict[str, int | str]], CONFIG_MANAGER["connections"])
+
+
+def default_connection_name() -> str:
+    """returns name of the default connection
     Returns:
-        list of connection names
+        connection name
     """
-    return list(cast(dict[str, dict[str, Any]], CONFIG_MANAGER["connections"]).keys())
+    return cast(str, CONFIG_MANAGER["default_connection_name"])
 
 
 def conn_opts(
-    connection_name: str | None = None,
+    *,
     keyfile_pfx_map: tuple[Path, Path] | None = None,
+    connection_name: str | None = None,
     **overrides: Any,
 ) -> dict[str, Any]:
     """returns connection options with overrides applied, if suplied
 
     Args:
-        name: A connection name to be looked up from the config_file; value can be None
-        keyfile_pfx_map: if specified must be a a pair of Path values specified as <from-path>:<to-path>,
-           which will be used to change private_key_file path value if it starts with <from-pahd> prefix
+        connection_name: A connection name to be looked up from the config_file; value can be None
+        keyfile_pfx_map: if specified must be a a pair of Path values specified as <from-path>:<to-path>, which will
+                         be used to temporarily change private_key_file path value if it starts with <from-pahd> prefix
         **overrides: A valid Snowflake python connector parameter; when not-None, will override value read from config_file
 
     Returns:
         dictionary containing option name and it's value
 
     Raises:
         *: any exceptions raised by snowflake.connector are passed through
@@ -75,32 +86,55 @@
         keyfile_pfx_map = _default_keyfile_pfx_map
 
     def fix_keyfile_path(path: str) -> str:
         if keyfile_pfx_map is not None and (p := Path(path)).is_relative_to(keyfile_pfx_map[0]):
             return str(keyfile_pfx_map[1] / p.relative_to(keyfile_pfx_map[0]))
         return path
 
-    connections = cast(dict[str, dict[str, Any]], CONFIG_MANAGER["connections"])
+    connections = available_connections()
     if connection_name is None:
-        connection_name = cast(str, CONFIG_MANAGER["default_connection_name"])
+        connection_name = default_connection_name()
 
     if connection_name not in connections:
         raise Error(f"Invalid connection name '{connection_name}', select from [{', '.join(connections.keys())}]")
 
     opts = {**connections[connection_name], **{k: v for k, v in overrides.items() if v is not None}}
     if "private_key_file" in opts:
         opts["private_key_file"] = fix_keyfile_path(cast(str, opts["private_key_file"]))
 
     return opts
 
 
-def getconn(connection_name: str | None = None, **overrides: Any) -> Connection:
+def getconn(*, keyfile_pfx_map: tuple[Path, Path] | None = None, **kwargs: Any) -> Connection:
     """connect to Snowflake database using named configuration
 
-    Args
-        name: A connection name to be looked up from the config_file, optional defaults to None for default connection
-        **overrides: Any parameter that is valid for conn_opts() method; see conn_opts() documentation
+    Args:
+        keyfile_pfx_map: if specified must be a a pair of Path values specified as <from-path>:<to-path>, which will
+                         be used to temporarily change private_key_file path value if it starts with <from-pahd> prefix
+        **kwargs: Any parameter that is valid for snowflake.connector.connect() method
 
     Returns:
         Connection object returned by Snowflake python connector
     """
-    return Connection(**conn_opts(connection_name, **overrides))  # type: ignore
+    return Connection(**conn_opts(keyfile_pfx_map=keyfile_pfx_map, **kwargs))  # type: ignore
+
+
+try:
+    from snowflake.snowpark import Session
+
+    def getsess(*, keyfile_pfx_map: tuple[Path, Path] | None = None, **kwargs: Any) -> Session:
+        """create a Session object using named configuration
+
+        Args:
+            keyfile_pfx_map: if specified must be a a pair of Path values specified as <from-path>:<to-path>, which will
+                             be used to temporarily change private_key_file path value if it starts with <from-pahd> prefix
+            **kwargs: Any parameter that is valid for snowflake.connector.connect() method
+
+        Returns:
+            Session object returned by Snowflake python connector
+        """
+        return Session.builder.configs(conn_opts(keyfile_pfx_map=keyfile_pfx_map, **kwargs)).create()
+
+except ImportError:
+
+    def getsess(*, keyfile_pfx_map: tuple[Path, Path] | None = None, **kwargs: Any) -> Session:
+        raise NotImplementedError("Unable to import snowflake.snowpark.Session; is snowflake-snowpark-python installed?")
```

### Comparing `sfconn-0.3.0/sfconn/cursor.py` & `sfconn-0.3.1/sfconn/cursor.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 "Snowflake cursor class"
+
 from inspect import currentframe, getframeinfo
 from logging import DEBUG, getLogger
 from typing import Any, Callable, Iterable, Self, Sequence, TypeAlias, TypeVar, cast
 
 from snowflake.connector.cursor import SnowflakeCursor
-from snowflake.connector.errors import ProgrammingError
+from snowflake.connector.errors import DataError, ProgrammingError
 
 logger = getLogger(__name__)
 T = TypeVar("T")
 Params: TypeAlias = Sequence[Any] | dict[Any, Any] | None
 
 
 class Cursor(SnowflakeCursor):
@@ -38,33 +39,38 @@
                 fi.lineno,
                 fi.function,
                 sql.replace("\t", "    "),
             )
         self.execute(sql, params=params)
         return self
 
-    def run_query(self, rec: Callable[..., T] | type[T], sql: str, params: Params = None) -> Iterable[T]:
+    def run_query(
+        self, rec: Callable[..., T] | type[T], sql: str, params: Params = None, *, select: list[str] | None = None
+    ) -> Iterable[T]:
         """execute a SELECT statement, map rows to produce instances of type T
 
         Args:
             rec: must be either
-                 - a Callable that accepts each column of a as a parameter in the same order and returns instance of T
-                 - a class T, whose __init__ method argument names must match some column names when upper-cased.
-                   Only the matching column names are passed to T.__init__() in the argument order
+                 - a Callable that accepts columns from the result-set as arguments. column names and the order are described in 'select'
+                 - a class T, whose __init__ method accepts columns from result-set as arguments. column names and the order are described in 'select'
             sql: SELECT SQL query text
             params: optional parameters as a Sequence or a dict
+            select: an optional, keyword only, argument that explicitly specifies the list of result-set columns to use.
+                    When omitted, default list of columns is picked based on 'rec' as follows:
+                    - for Callable, all columns from the result-set in result-set order
+                    - for class T, upper-cased argument names of T.__init__ method in the argument order
 
         Returns:
-            Iterable over instance of the type T
-        """
+            Iterable over instance of the type T or a tuple of values of only the selected columns
 
-        def mk_class(fn: Callable[..., T]) -> Iterable[T]:
-            return (fn(*r) for r in cast(Iterable[tuple[Any, ...]], self.execute_debug(sql, params)))
+        Raises:
+            ProgrammingError if argument or attribute name needed to instantiate T is not a column from the result-set
+        """
 
-        def get_elems() -> list[str]:
+        def get_init_args(rec: type[Any]) -> list[str]:
             try:
                 elems = [c.upper() for c in cast(dict[str, type], rec.__init__.__annotations__) if c != "return"]
                 if len(elems) == 0:
                     raise TypeError(f"'{rec}.__init__()' takes no arguments")
                 return elems
             except AttributeError:
                 raise TypeError(f"'{rec}.__init__()' takes no arguments")
@@ -72,56 +78,73 @@
         def get_col_pos(elems: list[str]) -> list[int]:
             try:
                 cols = {d.name: e for e, d in enumerate(self.description)}
                 return [cols[a] for a in elems]
             except KeyError as err:
                 raise ProgrammingError(f"Column access error: {err} in SQL: {sql}")
 
-        if isinstance(rec, type):
-            elems = get_elems()
-            self.execute_debug(sql)
-            pos = get_col_pos(elems)
-            return mk_class(lambda *r: rec(*(r[e] for e in pos)))  # type: ignore
+        self.execute_debug(sql)
 
-        if callable(rec):
-            return mk_class(rec)
-
-        raise TypeError(f"'{rec}' must be either ")
-
-    def run_query1_opt(self, rec: Callable[..., T] | type[T], sql: str, params: Params = None) -> T | None:
+        if select:
+            col_pos = get_col_pos(select)
+        else:
+            if isinstance(rec, type):
+                col_pos = get_col_pos(get_init_args(rec))
+            elif callable(rec):
+                col_pos = list(range(len(self.description)))
+            else:
+                raise TypeError(f"'{rec}' must be either ")
+
+        return (rec(*(row[e] for e in col_pos)) for row in self)  # type: ignore
+
+    def run_query1_opt(
+        self, rec: Callable[..., T] | type[T], sql: str, params: Params = None, *, select: list[str] | None = None
+    ) -> T | None:
         """execute a SELECT statement, return the first row mapped using the provided function
 
         Args:
             rec: must be either
-                 - a Callable that accepts each column of a as a parameter in the same order and returns instance of T
-                 - a class T, whose __init__ method argument names must match some column names when upper-cased.
-                   Only the matching column names are passed to T.__init__() in the argument order
+                 - a Callable that accepts columns from the result-set as arguments. column names and the order are described in 'select'
+                 - a class T, whose __init__ method accepts columns from result-set as arguments. column names and the order are described in 'select'
             sql: SELECT SQL query text
             params: optional parameters as a Sequence or a dict
+            select: an optional, keyword only, argument that explicitly specifies the list of result-set columns to use.
+                    When omitted, default list of columns is picked based on 'rec' as follows:
+                    - for Callable, all columns from the result-set in result-set order
+                    - for class T, upper-cased argument names of T.__init__ method in the argument order
 
         Returns:
-            Iterable over instance of the type T
+            Iterable over instance of the type T or a tuple of values of only the selected columns
+
+        Raises:
+            ProgrammingError if argument or attribute name needed to instantiate T is not a column from the result-set
         """
-        return next(iter(self.run_query(rec, sql, params)), None)
+        return next(iter(self.run_query(rec, sql, params, select=select)), None)
 
-    def run_query1(self, rec: Callable[..., T] | type[T], sql: str, params: Params = None) -> T:
+    def run_query1(
+        self, rec: Callable[..., T] | type[T], sql: str, params: Params = None, *, select: list[str] | None = None
+    ) -> T:
         """execute a SELECT statement, return the first row mapped using the provided function
 
         Args:
             rec: must be either
-                 - a Callable that accepts each column of a as a parameter in the same order and returns instance of T
-                 - a class T, whose __init__ method argument names must match some column names when upper-cased.
-                   Only the matching column names are passed to T.__init__() in the argument order
+                 - a Callable that accepts columns from the result-set as arguments. column names and the order are described in 'select'
+                 - a class T, whose __init__ method accepts columns from result-set as arguments. column names and the order are described in 'select'
             sql: SELECT SQL query text
             params: optional parameters as a Sequence or a dict
+            select: an optional, keyword only, argument that explicitly specifies the list of result-set columns to use.
+                    When omitted, default list of columns is picked based on 'rec' as follows:
+                    - for Callable, all columns from the result-set in result-set order
+                    - for class T, upper-cased argument names of T.__init__ method in the argument order
 
         Returns:
-            Iterable over instance of the type T
+            Iterable over instance of the type T or a tuple of values of only the selected columns
 
         Raises:
-            ProgrammingError if a row is not available
+            ProgrammingError if argument or attribute name needed to instantiate T is not a column from the result-set
+            DataError if at least one is not available in the result-set
         """
-        row = self.run_query1_opt(rec, sql, params)
+        row = self.run_query1_opt(rec, sql, params, select=select)
         if row is None:
-            raise ProgrammingError("no data available")
+            raise DataError("no data available")
 
         return row
```

### Comparing `sfconn-0.3.0/sfconn/jwt.py` & `sfconn-0.3.1/sfconn/jwt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 "get a JWT token"
+
 import base64
 import datetime as dt
 import hashlib
 from pathlib import Path
 from typing import cast
 
 import jwt
@@ -44,15 +45,15 @@
         a JWT
 
     Exceptions:
         ValueError: if `conn` doesn't support key-pair authentication
         *: Any exceptions raised by either conn_opts() or class PrivateKey
     """
 
-    opts = conn_opts(connection_name)
+    opts = conn_opts(connection_name=connection_name)
     keyf = cast(str | None, opts.get("private_key_file"))
     if keyf is None:
         raise ValueError(f"'{connection_name}' does not use key-pair authentication to support creating a JWT")
 
     qual_user = f"{_clean_account_name(opts['account']).upper()}.{opts['user'].upper()}"
 
     key = PrivateKey(Path(keyf))
```

### Comparing `sfconn-0.3.0/sfconn/privkey.py` & `sfconn-0.3.1/sfconn/privkey.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 "Private key"
+
 import os
 from functools import cached_property
 from pathlib import Path
 
 import cryptography.hazmat.primitives.serialization as Serde
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives.asymmetric.rsa import RSAPrivateKey
```

### Comparing `sfconn-0.3.0/sfconn.egg-info/PKG-INFO` & `sfconn-0.3.1/sfconn.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,80 @@
 Metadata-Version: 2.1
 Name: sfconn
-Version: 0.3.0
+Version: 0.3.1
 Summary: Snowflake connection helper functions
 Author-email: Paresh Adhia <padhia+github@gmail.com>
+Project-URL: Homepage, https://github.com/padhia/sfconn
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: snowflake-connector-python>=3.7.0
-Provides-Extra: keyring
-Requires-Dist: keyring; extra == "keyring"
-Provides-Extra: jwt
-Requires-Dist: pyjwt; extra == "jwt"
-Provides-Extra: tests
-Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pyjwt
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Provides-Extra: snowpark
+Requires-Dist: snowflake-snowpark-python; extra == "snowpark"
+
+# sfconn
 
 [![PyPi](https://img.shields.io/pypi/v/sfconn.svg)](https://pypi.python.org/pypi/sfconn) [![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT) ![Python3.11+](https://img.shields.io/badge/dynamic/json?query=info.requires_python&label=python&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fsfconn%2Fjson)
 
 Snowflake connection helper functions
 
 A Python library to simplify connecting to Snowflake databases
 
 **Notes**
-1. This is a major version upgrade and breaks compatibility with the previous versions (< `0.3.0`). `sfconn` now relies on `snowflake-python-connector` for accessing named connections (e.g. `connections.toml`). If you still need the ability use named connections from `~/.snowflake/config`, please continue using older version (`0.2.x`).
-1. `sfconn` modifies the way `private_key_file` connection option is evaluated in the following ways:
-    - with `--keyfile-anchor` option (default `$SFCONN_KEYFILE_ANCHOR`): uses the supplied value to anchor any relative paths (v/s anchoring paths relative to current working directory of the running process)
-    - with `--keyfile-strip-pfx` option (default `$SFCONN_KEYFILE_STRIP_PFX` ): strips the specified prefix from the path values (so `--keyfile-anchor` option can be used)
+1. This is a major version upgrade and breaks compatibility with the previous versions (< `0.3.0`). `sfconn` now relies on `snowflake-python-connector` for accessing named connections ([`connections.toml`](https://docs.snowflake.com/en/developer-guide/python-connector/python-connector-connect#connecting-using-the-connections-toml-file)).
+1. `sfconn` optionally modifies the way `private_key_file` connection option is evaluated. When `--keyfile-pfx-map` option is specified, or if `$SFCONN_KEYFILE_PFX_MAP` is set, (option value must be a pair of source and target paths separated by `:`). `private_key_file` option, if present and begins with the source path, it is temporarily modified as if it begins with the target path. Primary use-case is to be able to maintain one copy of `connections.toml` file across different execution environments, such as within containers.
 
-# Installation
+## Installation
 
 Use Python's standard `pip` utility for installation:
 
 ```sh
 pip install --upgrade sfconn
 ```
 
-# Usage
+## Usage
+
+### `getconn()` and `getsess()`
 
-## `getconn()`
+`getconn` and `getsess` are wrapper functions over native Snowflake functions with added functionality (mainly mapping `private_key_file` value as described above).
+
+**Note:** `getsess` is meant to work with *Snowpark* applications. As such, it will raise a `NotImplementedError` exception if `snowflake-snowpark-python` package is not available.
 
 **Usage:**
 ```python
-def getconn(connection_name: str | None, **overrides: dict[str, Any]) -> Connection
+def getconn(connection_name: str | None, **overrides: dict[str, Any]) -> Connection:
+def getsess(connection_name: str | None, **overrides: dict[str, Any]) -> Session:
 ```
 
-`getconn` accepts a connection name and returns a connection object with modified behavior as noted above.
-
-**Example:**
+`getconn` and `getsess` accept a connection name and return a connection or session object respectively with modified behavior as noted above.
 
+**Examples:**
 ```python
 from sfconn import getconn
 
-# assuming 'dev' is a connection defined in ~/.snowflake/config
+# assuming 'dev' is a named connection defined in connections.toml
 with getconn('dev', schema='PUBLIC') as cnx:
     with cnx.cursor() as csr:
         csr.execute('SELECT CURRENT_USER()')
         print("Hello " + csr.fetchone()[0])
 ```
 
-## `conn_opts()`
-
-**Usage:**
-```python
-def conn_opts(name: str | None , **overrides: dict[str, Any]) -> dict[str, Any]
-```
-
-`conn_opts`, returns a Python `dict` object populated with options and values. This can be useful passing as an argument to `snowflake.snowpark.Session.builder.configs()` method.
-
-**Example:**
-
 ```python
-from sfconn import conn_opts
-from snowflake.snowpark import Session
+from sfconn import getsess
 
-# assuming 'dev' is a connection defined in ~/.snowflake/config
-session = Session.builder.configs(conn_opts('dev')).create()
+# assuming 'dev' is a named connection defined in connections.toml
+with getsess('dev', schema='PUBLIC') as session:
+    df = sess.sql("select current_user() as curr_user, current_role() as curr_role")
+    print(df.collect())
 ```
 
-## `run_query*()`
+### `run_query*()`
 
 Cursor objects add a family of few convenience methods that return an `Iterable` of values instead of generic `tuple` or `dict`.
 
 1. `<cursor>.run_query(<callable>|<class>, <sql> [,<params>])`: Returns an Iterable of values.
     - `<callable>` is a mapping function that shall accept all column values of a row as individual arguments, in order, and returns a value that will be used for `Iterable`.
     - `<class>` is any Python class whose attribute names, after upper-casing, are treated as column names from the result set. `<class>` can include only a subset of a all available column from the query result as attributes and in a different order than the query.
 1. `<cursor>.run_query1(<callable>|<class>, <sql> [,<params>])`: Similar to `run_query`, except returns a single value. Note, if at least one value is not available, raises `ProgrammingError` exception.
@@ -113,63 +107,63 @@
 with getconn() as cnx, cnx.cursor() as csr:
     result = csr.run_query1(
         Result,
         "select current_user() as user, current_date() as date, current_warehouse() as wh_name"
     )
 ```
 
-## Decorator functions
+### Decorator Functions
 
-Python scripts that accept command-line parameters and use `argparse` library, can use decorator functions to further reduce boilerplate code needed for setting up common Snowflake connection options as command-line arguments
+Python command-line scripts that use `argparse` library, can use decorator functions to further reduce boilerplate code needed for setting up a Snowflake connection and error checking
 
 ```python
 def with_connection_args(doc: str | None) -> Callable[[argparse.ArgumentParser], None]:
 def with_connection(logger = None) -> Callable[[Connection, ...], None]:
-def with_connection_option(logger = None) => Callable([dict[str, Any, ...]])
+def with_session(logger = None) -> Callable[[Session, ...], None]:
 ```
 
 `with_connection_args()` decorator function:
 1. builds an `ArgumentParser` object
-1. adds common Snowflake connection options as arguments that allow overriding values specified in `~/.snowsql/config`
+1. adds common Snowflake connection options as arguments including overriding role, database, schema and warehouse
 1. calls the decorated function with the parser object to allow adding any script specific options
 
 `with_connection()` decorator function:
-1. consumes standard Snowflake connection options (specified with `args()`)
+1. consumes standard Snowflake connection options (specified with `with_connection_args()`)
 1. creates a connection object
 1. calls the decorated function with a connection object as first parameter and any other script specific options that were specified on command line
 
-`with_connection_option()` decorator function:
-- Similar to `entry()` but passes a `dict` of options as the first parameter. This is useful for passing options to the `snowflake.snowpark.Session.builder.configs()` method
+`with_session()` decorator function:
+1. Similar to `with_connection()` but creates a `snowflake.snowpark.Session` object instead of a connection object
+1. **Note:** this decorator will raise an `NotImplementedError` exception if `snowflake-snowpark-python` package is not available.
 
 **Example:**
 
 ```python
-from sfconn import args, entry
+from sfconn import with_connection_args, with_connection
 
-@entry
+@with_connection
 def main(con, show_account: bool):
     with con.cursor() as csr:
         csr.execute('SELECT CURRENT_USER()')
         print("Hello " + csr.fetchone()[0])
         if show_account:
             csr.execute("SELECT CURRENT_ACCOUNT()")
             print("You are connected to account: " + csr.fetchone()[0])
 
-@args("Sample application that greets the current Snowflake user")
+@with_connection_args("Sample application that greets the current Snowflake user")
 def getargs(parser):
     parser.add_argument("-a", "--show-account", action='store_true', help="show snowflake account name")
 
 if __name__ == '__main__':
     main(**vars(getargs()))
 ```
 
-## `get_token()`
+### `get_token()`
 
 Function `sfconn.get_token()` returns a JWT token for connections that use `private_key_path` option. An optional lifetime value can be specified (default 54 minutes)
 
 **Example:**
 
 ```python
 from sfconn import get_token
-
-# assuming 'dev' is a connection defined in ~/.snowflake/config and uses key-pair authentication
-jwt_token = get_token('dev', 120)  # get a token valid for 120 minutes
+jwt_token = get_token(None, 120)  # get token using default (None) connection, and valid for 120 minutes
+```
```

### Comparing `sfconn-0.3.0/tests/test_cursor.py` & `sfconn-0.3.1/tests/test_cursor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,85 +1,97 @@
 "test Cursor class"
+
 import datetime as dt
 from collections import namedtuple
 from dataclasses import dataclass
 
 import pytest
 
-from sfconn import ProgrammingError, getconn
+from sfconn import Connection, DataError, ProgrammingError
 
 SQL = "select current_user() as user, current_date() as date"
 
 
-def test_run_query_func() -> None:
+def test_run_query_func(cnx: Connection) -> None:
     Result = namedtuple("Result", ["user", "date"])  # type: ignore
 
     def mkResult(x: str, y: dt.date) -> Result:
         return Result(x, y)
 
-    with getconn() as cnx, cnx.cursor() as csr:
-        csr.run_query1(mkResult, SQL)
+    with cnx.cursor() as csr:
+        assert isinstance(csr.run_query1(mkResult, SQL), Result)
 
 
-def test_run_query_class() -> None:
+def test_run_query_columns(cnx: Connection) -> None:
+    @dataclass
+    class Result:
+        one: int
+        three: int
+
+    with cnx.cursor() as csr:
+        r = csr.run_query1(Result, 'select 1 as "one", 2 as "two", 3 as "three"', select=["one", "three"])
+        assert r == Result(1, 3)
+
+
+def test_run_query_class(cnx: Connection) -> None:
     @dataclass
     class Result:
         user: str
         date: dt.date
 
-    with getconn() as cnx, cnx.cursor() as csr:
+    with cnx.cursor() as csr:
         assert isinstance(csr.run_query1(Result, SQL), Result)
 
 
-def test_run_query_class_elem_order() -> None:
+def test_run_query_class_elem_order(cnx: Connection) -> None:
     "class with elements defined in different order than SELECT"
 
     @dataclass
     class Result:
         date: dt.date
         user: str
 
-    with getconn() as cnx, cnx.cursor() as csr:
+    with cnx.cursor() as csr:
         assert isinstance(csr.run_query1(Result, SQL), Result)
 
 
-def test_run_query_class_fewer_elems() -> None:
+def test_run_query_class_fewer_elems(cnx: Connection) -> None:
     "class with elements defined with fewer elements than SELECT"
 
     @dataclass
     class Result:
         date: dt.date
 
-    with getconn() as cnx, cnx.cursor() as csr:
+    with cnx.cursor() as csr:
         assert isinstance(csr.run_query1(Result, SQL), Result)
 
 
-def test_run_query_class_noinit() -> None:
+def test_run_query_class_noinit(cnx: Connection) -> None:
     class Result:
         user: str
         date: dt.date
 
     with pytest.raises(TypeError):
-        with getconn() as cnx, cnx.cursor() as csr:
+        with cnx.cursor() as csr:
             csr.run_query1(Result, SQL)
 
 
-def test_run_query_bad_columns() -> None:
+def test_run_query_bad_columns(cnx: Connection) -> None:
     "when __init__ has arguments whose names do not match any columns"
 
     class Result:
         user: str
         date: dt.date
 
         def __init__(self, x: str, y: str) -> None:
             self.user, self.role = x, y
 
     with pytest.raises(ProgrammingError):
-        with getconn() as cnx, cnx.cursor() as csr:
+        with cnx.cursor() as csr:
             csr.run_query1(Result, SQL)
 
 
-def test_select1_norows() -> None:
+def test_select1_norows(cnx: Connection) -> None:
     "test an exception is thrown when no rows are returned for run_query1() call"
-    with pytest.raises(ProgrammingError):
-        with getconn() as cnx, cnx.cursor() as csr:
+    with pytest.raises(DataError):
+        with cnx.cursor() as csr:
             csr.run_query1(lambda *x: x, SQL + " where 1 = 0")
```

### Comparing `sfconn-0.3.0/tests/test_decorators.py` & `sfconn-0.3.1/tests/test_decorators.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 "test decorators"
+
 from argparse import ArgumentParser
 from dataclasses import dataclass
 from typing import Any
 
 from sfconn import Connection, with_connection, with_connection_args
```

