# Comparing `tmp/sqlexecutorx-0.0.2.tar.gz` & `tmp/sqlexecutorx-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlexecutorx-0.0.2.tar", last modified: Sat May  4 03:23:58 2024, max compression
+gzip compressed data, was "sqlexecutorx-0.0.3.tar", last modified: Sat May  4 04:09:50 2024, max compression
```

## Comparing `sqlexecutorx-0.0.2.tar` & `sqlexecutorx-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-04 03:23:57.992891 sqlexecutorx-0.0.2/
--rw-rw-r--   0 summy      (501) staff       (20)    11357 2024-03-14 05:16:15.000000 sqlexecutorx-0.0.2/LICENSE
--rw-r--r--   0 summy      (501) staff       (20)     2031 2024-05-04 03:23:57.990235 sqlexecutorx-0.0.2/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)     1577 2024-05-04 03:23:13.000000 sqlexecutorx-0.0.2/README.rst
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-04 03:23:57.993170 sqlexecutorx-0.0.2/setup.cfg
--rw-rw-r--   0 summy      (501) staff       (20)     1172 2024-05-04 03:23:54.000000 sqlexecutorx-0.0.2/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-04 03:23:57.978938 sqlexecutorx-0.0.2/sqlexecutorx/
--rw-rw-r--   0 summy      (501) staff       (20)      347 2024-03-28 02:27:57.000000 sqlexecutorx-0.0.2/sqlexecutorx/__init__.py
--rw-rw-r--   0 summy      (501) staff       (20)      209 2024-05-04 03:22:15.000000 sqlexecutorx-0.0.2/sqlexecutorx/constant.py
--rw-rw-r--   0 summy      (501) staff       (20)     8655 2024-05-04 03:22:15.000000 sqlexecutorx-0.0.2/sqlexecutorx/core.py
--rw-r--r--   0 summy      (501) staff       (20)      901 2024-03-23 15:57:10.000000 sqlexecutorx-0.0.2/sqlexecutorx/engine.py
--rw-rw-r--   0 summy      (501) staff       (20)     2042 2024-03-23 16:12:52.000000 sqlexecutorx-0.0.2/sqlexecutorx/init_import.py
--rw-rw-r--   0 summy      (501) staff       (20)      740 2024-03-25 03:02:59.000000 sqlexecutorx-0.0.2/sqlexecutorx/log_support.py
--rw-rw-r--   0 summy      (501) staff       (20)     1031 2024-05-04 03:22:15.000000 sqlexecutorx-0.0.2/sqlexecutorx/pooling.py
--rw-r--r--   0 summy      (501) staff       (20)      422 2024-03-29 05:50:43.000000 sqlexecutorx-0.0.2/sqlexecutorx/sql_support.py
--rw-rw-r--   0 summy      (501) staff       (20)     3892 2024-03-25 02:25:33.000000 sqlexecutorx-0.0.2/sqlexecutorx/support.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-04 03:23:57.989071 sqlexecutorx-0.0.2/sqlexecutorx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)     2031 2024-05-04 03:23:57.000000 sqlexecutorx-0.0.2/sqlexecutorx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      432 2024-05-04 03:23:57.000000 sqlexecutorx-0.0.2/sqlexecutorx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-04 03:23:57.000000 sqlexecutorx-0.0.2/sqlexecutorx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-04 03:23:57.000000 sqlexecutorx-0.0.2/sqlexecutorx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)       13 2024-05-04 03:23:57.000000 sqlexecutorx-0.0.2/sqlexecutorx.egg-info/top_level.txt
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-04 04:09:50.159429 sqlexecutorx-0.0.3/
+-rw-rw-r--   0 summy      (501) staff       (20)    11357 2024-03-14 05:16:15.000000 sqlexecutorx-0.0.3/LICENSE
+-rw-r--r--   0 summy      (501) staff       (20)     2031 2024-05-04 04:09:50.157095 sqlexecutorx-0.0.3/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)     1577 2024-05-04 03:23:13.000000 sqlexecutorx-0.0.3/README.rst
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-04 04:09:50.160225 sqlexecutorx-0.0.3/setup.cfg
+-rw-rw-r--   0 summy      (501) staff       (20)     1172 2024-05-04 04:09:43.000000 sqlexecutorx-0.0.3/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-04 04:09:50.145826 sqlexecutorx-0.0.3/sqlexecutorx/
+-rw-rw-r--   0 summy      (501) staff       (20)      903 2024-05-04 04:09:24.000000 sqlexecutorx-0.0.3/sqlexecutorx/__init__.py
+-rw-rw-r--   0 summy      (501) staff       (20)      209 2024-05-04 03:22:15.000000 sqlexecutorx-0.0.3/sqlexecutorx/constant.py
+-rw-rw-r--   0 summy      (501) staff       (20)    11253 2024-05-04 04:09:24.000000 sqlexecutorx-0.0.3/sqlexecutorx/core.py
+-rw-r--r--   0 summy      (501) staff       (20)      901 2024-03-23 15:57:10.000000 sqlexecutorx-0.0.3/sqlexecutorx/engine.py
+-rw-rw-r--   0 summy      (501) staff       (20)     2042 2024-03-23 16:12:52.000000 sqlexecutorx-0.0.3/sqlexecutorx/init_import.py
+-rw-rw-r--   0 summy      (501) staff       (20)      740 2024-03-25 03:02:59.000000 sqlexecutorx-0.0.3/sqlexecutorx/log_support.py
+-rw-rw-r--   0 summy      (501) staff       (20)     1031 2024-05-04 03:22:15.000000 sqlexecutorx-0.0.3/sqlexecutorx/pooling.py
+-rw-r--r--   0 summy      (501) staff       (20)      422 2024-03-29 05:50:43.000000 sqlexecutorx-0.0.3/sqlexecutorx/sql_support.py
+-rw-rw-r--   0 summy      (501) staff       (20)     3892 2024-03-25 02:25:33.000000 sqlexecutorx-0.0.3/sqlexecutorx/support.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-04 04:09:50.154914 sqlexecutorx-0.0.3/sqlexecutorx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)     2031 2024-05-04 04:09:50.000000 sqlexecutorx-0.0.3/sqlexecutorx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      432 2024-05-04 04:09:50.000000 sqlexecutorx-0.0.3/sqlexecutorx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-04 04:09:50.000000 sqlexecutorx-0.0.3/sqlexecutorx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-04 03:23:57.000000 sqlexecutorx-0.0.3/sqlexecutorx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)       13 2024-05-04 04:09:50.000000 sqlexecutorx-0.0.3/sqlexecutorx.egg-info/top_level.txt
```

### Comparing `sqlexecutorx-0.0.2/LICENSE` & `sqlexecutorx-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.0.2/PKG-INFO` & `sqlexecutorx-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: sqlexecutorx
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple thread safe sql sqlexecutorx for Python with connection pool. Support MySQL, PostgreSQL, SQLite etc.
-Home-page: https://gitee.com/summry/sql-executor
+Home-page: https://gitee.com/summry/sqlexecutorx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Database,Python,RDB
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `sqlexecutorx-0.0.2/README.rst` & `sqlexecutorx-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.0.2/setup.py` & `sqlexecutorx-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 setup(
     name='sqlexecutorx',
     packages=['sqlexecutorx'],
     description="A simple thread safe sql sqlexecutorx for Python with connection pool. Support MySQL, PostgreSQL, SQLite etc.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.0.2',
-    url='https://gitee.com/summry/sql-executor',
+    version='0.0.3',
+    url='https://gitee.com/summry/sqlexecutorx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Database', 'Python', 'RDB'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
     },
```

### Comparing `sqlexecutorx-0.0.2/sqlexecutorx/engine.py` & `sqlexecutorx-0.0.3/sqlexecutorx/engine.py`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.0.2/sqlexecutorx/init_import.py` & `sqlexecutorx-0.0.3/sqlexecutorx/init_import.py`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.0.2/sqlexecutorx/log_support.py` & `sqlexecutorx-0.0.3/sqlexecutorx/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.0.2/sqlexecutorx/pooling.py` & `sqlexecutorx-0.0.3/sqlexecutorx/pooling.py`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.0.2/sqlexecutorx/support.py` & `sqlexecutorx-0.0.3/sqlexecutorx/support.py`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.0.2/sqlexecutorx.egg-info/PKG-INFO` & `sqlexecutorx-0.0.3/sqlexecutorx.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: sqlexecutorx
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple thread safe sql sqlexecutorx for Python with connection pool. Support MySQL, PostgreSQL, SQLite etc.
-Home-page: https://gitee.com/summry/sql-executor
+Home-page: https://gitee.com/summry/sqlexecutorx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Database,Python,RDB
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

