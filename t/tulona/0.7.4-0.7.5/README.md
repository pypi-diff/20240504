# Comparing `tmp/tulona-0.7.4.tar.gz` & `tmp/tulona-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tulona-0.7.4.tar", last modified: Mon Apr 29 11:49:14 2024, max compression
+gzip compressed data, was "tulona-0.7.5.tar", last modified: Sat May  4 04:39:33 2024, max compression
```

## Comparing `tulona-0.7.4.tar` & `tulona-0.7.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:49:14.979318 tulona-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-29 11:49:09.000000 tulona-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14575 2024-04-29 11:49:14.979318 tulona-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-04-29 11:49:09.000000 tulona-0.7.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:49:14.967317 tulona-0.7.4/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:49:14.971317 tulona-0.7.4/core/tulona/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-29 11:49:09.000000 tulona-0.7.4/core/tulona/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:49:14.971317 tulona-0.7.4/core/tulona/adapter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:49:14.971317 tulona-0.7.4/core/tulona/adapter/base/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-29 11:49:09.000000 tulona-0.7.4/core/tulona/adapter/base/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-29 11:49:09.000000 tulona-0.7.4/core/tulona/adapter/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-29 11:49:10.000000 tulona-0.7.4/core/tulona/adapter/mssql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-29 11:49:10.000000 tulona-0.7.4/core/tulona/adapter/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-29 11:49:10.000000 tulona-0.7.4/core/tulona/adapter/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-29 11:49:10.000000 tulona-0.7.4/core/tulona/adapter/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:49:14.975317 tulona-0.7.4/core/tulona/cli/
--rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-04-29 11:49:10.000000 tulona-0.7.4/core/tulona/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-29 11:49:10.000000 tulona-0.7.4/core/tulona/cli/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:49:14.975317 tulona-0.7.4/core/tulona/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:49:10.000000 tulona-0.7.4/core/tulona/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-29 11:49:10.000000 tulona-0.7.4/core/tulona/config/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-29 11:49:10.000000 tulona-0.7.4/core/tulona/config/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-29 11:49:10.000000 tulona-0.7.4/core/tulona/config/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-29 11:49:10.000000 tulona-0.7.4/core/tulona/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:49:14.975317 tulona-0.7.4/core/tulona/task/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-29 11:49:10.000000 tulona-0.7.4/core/tulona/task/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    22680 2024-04-29 11:49:10.000000 tulona-0.7.4/core/tulona/task/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-04-29 11:49:10.000000 tulona-0.7.4/core/tulona/task/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-29 11:49:10.000000 tulona-0.7.4/core/tulona/task/ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-29 11:49:10.000000 tulona-0.7.4/core/tulona/task/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    16757 2024-04-29 11:49:10.000000 tulona-0.7.4/core/tulona/task/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:49:14.975317 tulona-0.7.4/core/tulona/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:49:10.000000 tulona-0.7.4/core/tulona/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-29 11:49:10.000000 tulona-0.7.4/core/tulona/util/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-29 11:49:10.000000 tulona-0.7.4/core/tulona/util/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-29 11:49:10.000000 tulona-0.7.4/core/tulona/util/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-29 11:49:10.000000 tulona-0.7.4/core/tulona/util/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-29 11:49:10.000000 tulona-0.7.4/core/tulona/util/profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-04-29 11:49:10.000000 tulona-0.7.4/core/tulona/util/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-29 11:49:10.000000 tulona-0.7.4/core/tulona/util/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:49:14.975317 tulona-0.7.4/core/tulona.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14575 2024-04-29 11:49:14.000000 tulona-0.7.4/core/tulona.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-29 11:49:14.000000 tulona-0.7.4/core/tulona.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 11:49:14.000000 tulona-0.7.4/core/tulona.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-29 11:49:14.000000 tulona-0.7.4/core/tulona.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-29 11:49:14.000000 tulona-0.7.4/core/tulona.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 11:49:14.000000 tulona-0.7.4/core/tulona.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-04-29 11:49:10.000000 tulona-0.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 11:49:14.979318 tulona-0.7.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:39:33.949408 tulona-0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-04 04:39:27.000000 tulona-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14575 2024-05-04 04:39:33.949408 tulona-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-05-04 04:39:27.000000 tulona-0.7.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:39:33.937408 tulona-0.7.5/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:39:33.941408 tulona-0.7.5/core/tulona/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:39:33.941408 tulona-0.7.5/core/tulona/adapter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:39:33.941408 tulona-0.7.5/core/tulona/adapter/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/adapter/base/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/adapter/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/adapter/mssql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/adapter/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/adapter/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/adapter/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:39:33.945408 tulona-0.7.5/core/tulona/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/cli/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:39:33.945408 tulona-0.7.5/core/tulona/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/config/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/config/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:39:33.945408 tulona-0.7.5/core/tulona/task/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22826 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/task/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/task/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/task/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/task/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16757 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/task/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:39:33.945408 tulona-0.7.5/core/tulona/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/util/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/util/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/util/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/util/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/util/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/util/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-04 04:39:27.000000 tulona-0.7.5/core/tulona/util/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 04:39:33.945408 tulona-0.7.5/core/tulona.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14575 2024-05-04 04:39:33.000000 tulona-0.7.5/core/tulona.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-04 04:39:33.000000 tulona-0.7.5/core/tulona.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 04:39:33.000000 tulona-0.7.5/core/tulona.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-04 04:39:33.000000 tulona-0.7.5/core/tulona.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-04 04:39:33.000000 tulona-0.7.5/core/tulona.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-04 04:39:33.000000 tulona-0.7.5/core/tulona.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-04 04:39:27.000000 tulona-0.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 04:39:33.949408 tulona-0.7.5/setup.cfg
```

### Comparing `tulona-0.7.4/LICENSE` & `tulona-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tulona-0.7.4/PKG-INFO` & `tulona-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulona
-Version: 0.7.4
+Version: 0.7.5
 Summary: A tool to compare data from different sources.
 Author: Mrinal Kanti Sardar
 Project-URL: Homepage, https://github.com/mrinalsardar/tulona
 Project-URL: Documentation, https://github.com/mrinalsardar/tulona
 Project-URL: Repository, https://github.com/mrinalsardar/tulona.git
 Project-URL: Issues, https://github.com/mrinalsardar/tulona/issues
 Keywords: tulona,comparison,data comparison,database scan,database profile
```

### Comparing `tulona-0.7.4/README.rst` & `tulona-0.7.5/README.rst`

 * *Files identical despite different names*

### Comparing `tulona-0.7.4/core/tulona/adapter/connection.py` & `tulona-0.7.5/core/tulona/adapter/connection.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.4/core/tulona/adapter/mssql.py` & `tulona-0.7.5/core/tulona/adapter/mssql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.4/core/tulona/adapter/mysql.py` & `tulona-0.7.5/core/tulona/adapter/mysql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.4/core/tulona/adapter/postgres.py` & `tulona-0.7.5/core/tulona/adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.4/core/tulona/adapter/snowflake.py` & `tulona-0.7.5/core/tulona/adapter/snowflake.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.4/core/tulona/cli/base.py` & `tulona-0.7.5/core/tulona/cli/base.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.4/core/tulona/cli/params.py` & `tulona-0.7.5/core/tulona/cli/params.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.4/core/tulona/config/profile.py` & `tulona-0.7.5/core/tulona/config/profile.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.4/core/tulona/config/project.py` & `tulona-0.7.5/core/tulona/config/project.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.4/core/tulona/exceptions.py` & `tulona-0.7.5/core/tulona/exceptions.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.4/core/tulona/task/base.py` & `tulona-0.7.5/core/tulona/task/base.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.4/core/tulona/task/compare.py` & `tulona-0.7.5/core/tulona/task/compare.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,14 +237,15 @@
                     raise ValueError(f"Primary key {k} not present in {table_fqn1}")
 
             # Exclude columns
             if len(exclude_columns1) > 0:
                 log.debug(
                     f"Excluding columns from {econf_dict['ds_names'][0]}: {exclude_columns1}"
                 )
+                exclude_columns1 = [c.lower() for c in exclude_columns1]
                 df1 = apply_column_exclusion(
                     df1, primary_key, exclude_columns1, econf_dict["ds_names"][0]
                 )
             if "table_fqns" in econf_dict:
                 query2 = get_table_data_query(
                     dbtype2,
                     table_fqn2,
@@ -262,14 +263,15 @@
                     raise ValueError(f"Primary key {k} not present in {table_fqn2}")
 
             # Exclude columns
             if len(exclude_columns2) > 0:
                 log.debug(
                     f"Excluding columns from {econf_dict['ds_names'][1]}: {exclude_columns2}"
                 )
+                exclude_columns2 = [c.lower() for c in exclude_columns2]
                 df2 = apply_column_exclusion(
                     df2, primary_key, exclude_columns2, econf_dict["ds_names"][1]
                 )
 
             if df2.shape[0] > 0:
                 for k in primary_key:
                     df1 = df1[df1[k].isin(df2[k].tolist())]
```

### Comparing `tulona-0.7.4/core/tulona/task/helper.py` & `tulona-0.7.5/core/tulona/task/helper.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.4/core/tulona/task/ping.py` & `tulona-0.7.5/core/tulona/task/ping.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.4/core/tulona/task/profile.py` & `tulona-0.7.5/core/tulona/task/profile.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.4/core/tulona/task/scan.py` & `tulona-0.7.5/core/tulona/task/scan.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.4/core/tulona/util/database.py` & `tulona-0.7.5/core/tulona/util/database.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.4/core/tulona/util/dataframe.py` & `tulona-0.7.5/core/tulona/util/dataframe.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.4/core/tulona/util/excel.py` & `tulona-0.7.5/core/tulona/util/excel.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.4/core/tulona/util/filesystem.py` & `tulona-0.7.5/core/tulona/util/filesystem.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 def get_result_dir(dir_dict: dict, base: Union[str, Path], key: str) -> Path:
     p = Path(get_output_base_dir(base), dir_dict[key])
     return create_or_replace_dir(p)
 
 
 # TODO: Testable - pull current timestamp from caller
 def get_final_outdir(basedir: str, task_conf: str):
-    out_timestamp = datetime.now().strftime("%Y%m%d%H%M%S")
+    out_timestamp = datetime.now().strftime("%Y%m%d%H%M%S%f")
 
     task = task_conf["task"].replace("-", "")
     ds_list = [ds.split(":")[0].replace("_", "") for ds in task_conf["datasources"]]
     extra_params = []
     for p in task_conf:
         if p not in ["task", "datasources"]:
             if isinstance(task_conf[p], int):
```

### Comparing `tulona-0.7.4/core/tulona/util/profiles.py` & `tulona-0.7.5/core/tulona/util/profiles.py`

 * *Files identical despite different names*

### Comparing `tulona-0.7.4/core/tulona/util/sql.py` & `tulona-0.7.5/core/tulona/util/sql.py`

 * *Files 8% similar despite different names*

```diff
@@ -115,54 +115,55 @@
         "interval",
         "datetimeoffset",
         "smalldatetime",
         "datetime2",
         "timestamp_tz",
         "timestamp_ltz",
         "timestamp_ntz",
-        "timestamp with time zone",  # TODO probably incorrect representation
+        "timestamp with time zone",  # TODO: probably incorrect representation
         "timestamp without time zone",
     ]
 
-    numeric_funcs = [
-        "min",
-        "max",
-        "average",
-        "avg",
-    ]
-    timestamp_funcs = [
-        "min",
-        "max",
-    ]
-    generic_funcs = [
-        "count",
-        "distinct_count",
-    ]
-
-    function_map = {
-        "min": "min({}) as {}_min",
-        "max": "max({}) as {}_max",
-        "avg": "avg({}) as {}_avg",
-        "average": "avg({}) as {}_average",
+    generic_function_map = {
         "count": "count({}) as {}_count",
         "distinct_count": "count(distinct({})) as {}_distinct_count",
     }
+    numeric_function_map = {
+        "min": "min(cast({} as decimal)) as {}_min",
+        "max": "max(cast({} as decimal)) as {}_max",
+        "avg": "avg(cast({} as decimal)) as {}_avg",
+        "average": "avg(cast({} as decimal)) as {}_avg",
+    }
+    timestamp_function_map = {
+        "min": "min({}) as {}_min",
+        "max": "max({}) as {}_max",
+    }
 
     call_funcs = []
     for col, dtype in columns_dtype.items():
         dtype = dtype.lower()
         qp = []
         for m in metrics:
-            if (
-                (m in numeric_funcs and dtype in numeric_types)
-                or (m in timestamp_funcs and dtype in timestamp_types)
-                or (m in generic_funcs)
-            ):
+            if m in generic_function_map:
+                qp.append(
+                    generic_function_map[m.lower()].format(
+                        f'"{col}"' if quoted else col, col
+                    )
+                )
+            elif m in numeric_function_map and dtype in numeric_types:
+                qp.append(
+                    numeric_function_map[m.lower()].format(
+                        f'"{col}"' if quoted else col, col
+                    )
+                )
+            elif m in timestamp_function_map and dtype in timestamp_types:
                 qp.append(
-                    function_map[m.lower()].format(f'"{col}"' if quoted else col, col)
+                    timestamp_function_map[m.lower()].format(
+                        f'"{col}"' if quoted else col, col
+                    )
                 )
             else:
                 qp.append(f"'NA' as {col}_{m.lower()}")
         call_funcs.extend(qp)
 
     query = f"""
     select
```

### Comparing `tulona-0.7.4/core/tulona.egg-info/PKG-INFO` & `tulona-0.7.5/core/tulona.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulona
-Version: 0.7.4
+Version: 0.7.5
 Summary: A tool to compare data from different sources.
 Author: Mrinal Kanti Sardar
 Project-URL: Homepage, https://github.com/mrinalsardar/tulona
 Project-URL: Documentation, https://github.com/mrinalsardar/tulona
 Project-URL: Repository, https://github.com/mrinalsardar/tulona.git
 Project-URL: Issues, https://github.com/mrinalsardar/tulona/issues
 Keywords: tulona,comparison,data comparison,database scan,database profile
```

### Comparing `tulona-0.7.4/core/tulona.egg-info/SOURCES.txt` & `tulona-0.7.5/core/tulona.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tulona-0.7.4/pyproject.toml` & `tulona-0.7.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tulona"
-version = "0.7.4"
+version = "0.7.5"
 description = "A tool to compare data from different sources."
 dependencies = [
   "click~=8.1",
   "ruamel.yaml~=0.18",
   "psycopg2-binary~=2.9",
   "pymysql~=1.1",
   "cryptography~=42.0",
@@ -111,15 +111,15 @@
 
 [tool.isort]
 profile = "black"
 line_length = 90
 skip = [".gitignore"]
 
 [tool.bumpversion]
-current_version = "0.7.4"
+current_version = "0.7.5"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = false
 tag = false
```

