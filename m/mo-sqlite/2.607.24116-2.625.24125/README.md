# Comparing `tmp/mo_sqlite-2.607.24116.tar.gz` & `tmp/mo_sqlite-2.625.24125.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo_sqlite-2.607.24116.tar", last modified: Thu Apr 25 00:57:47 2024, max compression
+gzip compressed data, was "mo_sqlite-2.625.24125.tar", last modified: Sat May  4 20:37:57 2024, max compression
```

## Comparing `mo_sqlite-2.607.24116.tar` & `mo_sqlite-2.625.24125.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 00:57:47.146583 mo_sqlite-2.607.24116/
--rw-rw-rw-   0        0        0    16725 2019-11-12 20:20:36.000000 mo_sqlite-2.607.24116/LICENSE
--rw-rw-rw-   0        0        0     3462 2024-04-25 00:57:47.146583 mo_sqlite-2.607.24116/PKG-INFO
--rw-rw-rw-   0        0        0     1913 2024-03-10 19:35:09.000000 mo_sqlite-2.607.24116/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 00:57:47.107086 mo_sqlite-2.607.24116/mo_sqlite/
--rw-rw-rw-   0        0        0      507 2024-02-27 03:34:35.000000 mo_sqlite-2.607.24116/mo_sqlite/__init__.py
--rw-rw-rw-   0        0        0    16964 2024-04-04 04:18:21.000000 mo_sqlite-2.607.24116/mo_sqlite/database.py
-drwxrwxrwx   0        0        0        0 2024-04-25 00:57:47.139038 mo_sqlite-2.607.24116/mo_sqlite/expressions/
--rw-rw-rw-   0        0        0     1580 2024-03-10 20:49:59.000000 mo_sqlite-2.607.24116/mo_sqlite/expressions/__init__.py
--rw-rw-rw-   0        0        0     1343 2024-03-11 06:29:29.000000 mo_sqlite-2.607.24116/mo_sqlite/expressions/_utils.py
--rw-rw-rw-   0        0        0      585 2024-03-11 06:29:29.000000 mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_add_op.py
--rw-rw-rw-   0        0        0      691 2024-03-11 06:29:29.000000 mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_alias_op.py
--rw-rw-rw-   0        0        0     2991 2024-03-11 06:29:29.000000 mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_and_op.py
--rw-rw-rw-   0        0        0     3244 2024-03-21 02:50:25.000000 mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_case_op.py
--rw-rw-rw-   0        0        0      672 2024-03-10 20:49:59.000000 mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_cast_op.py
--rw-rw-rw-   0        0        0     1034 2024-03-11 06:29:29.000000 mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_coalesce_op.py
--rw-rw-rw-   0        0        0      575 2024-03-10 19:35:09.000000 mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_concat_op.py
--rw-rw-rw-   0        0        0      497 2024-03-10 20:49:59.000000 mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_eq_op.py
--rw-rw-rw-   0        0        0      446 2024-03-10 20:49:59.000000 mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_group_by_op.py
--rw-rw-rw-   0        0        0      497 2024-02-15 03:48:30.000000 mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_gt_op.py
--rw-rw-rw-   0        0        0      501 2024-02-15 03:48:30.000000 mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_gte_op.py
--rw-rw-rw-   0        0        0      502 2024-03-10 20:49:59.000000 mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_in_op.py
--rw-rw-rw-   0        0        0      681 2024-03-11 06:29:29.000000 mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_inner_join_op.py
--rw-rw-rw-   0        0        0     1183 2024-03-11 06:29:29.000000 mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_instr_op.py
--rw-rw-rw-   0        0        0      552 2024-03-11 06:29:29.000000 mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_is_null_op.py
--rw-rw-rw-   0        0        0      378 2024-03-10 20:49:59.000000 mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_limit_op.py
--rw-rw-rw-   0        0        0      725 2024-03-11 06:29:29.000000 mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_literal.py
--rw-rw-rw-   0        0        0      617 2024-02-15 03:48:30.000000 mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_lt_op.py
--rw-rw-rw-   0        0        0      501 2024-02-15 03:48:30.000000 mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_lte_op.py
--rw-rw-rw-   0        0        0      570 2024-03-11 06:29:29.000000 mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_not_op.py
--rw-rw-rw-   0        0        0     1713 2024-03-11 06:29:29.000000 mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_or_op.py
--rw-rw-rw-   0        0        0      991 2024-03-10 20:49:59.000000 mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_order_by_op.py
--rw-rw-rw-   0        0        0     4839 2024-03-21 02:50:25.000000 mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_script.py
--rw-rw-rw-   0        0        0     2585 2024-03-11 06:29:29.000000 mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_select_op.py
--rw-rw-rw-   0        0        0     1160 2024-03-11 06:29:29.000000 mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_substr_op.py
--rw-rw-rw-   0        0        0      769 2024-03-11 06:29:29.000000 mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_variable.py
--rw-rw-rw-   0        0        0     6684 2024-02-15 03:48:30.000000 mo_sqlite-2.607.24116/mo_sqlite/sql_script.py
--rw-rw-rw-   0        0        0     6210 2024-03-18 02:53:29.000000 mo_sqlite-2.607.24116/mo_sqlite/transacfion.py
--rw-rw-rw-   0        0        0     1543 2024-01-28 17:16:21.000000 mo_sqlite-2.607.24116/mo_sqlite/types.py
--rw-rw-rw-   0        0        0     5687 2024-03-20 02:25:01.000000 mo_sqlite-2.607.24116/mo_sqlite/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-25 00:57:47.139038 mo_sqlite-2.607.24116/mo_sqlite.egg-info/
--rw-rw-rw-   0        0        0     3462 2024-04-25 00:57:47.000000 mo_sqlite-2.607.24116/mo_sqlite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1364 2024-04-25 00:57:47.000000 mo_sqlite-2.607.24116/mo_sqlite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 00:57:47.000000 mo_sqlite-2.607.24116/mo_sqlite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      341 2024-04-25 00:57:47.000000 mo_sqlite-2.607.24116/mo_sqlite.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-25 00:57:47.000000 mo_sqlite-2.607.24116/mo_sqlite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 00:57:47.146583 mo_sqlite-2.607.24116/setup.cfg
--rw-rw-rw-   0        0        0     3333 2024-04-25 00:57:42.000000 mo_sqlite-2.607.24116/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:37:57.438780 mo_sqlite-2.625.24125/
+-rw-rw-rw-   0        0        0    16725 2019-11-12 20:20:36.000000 mo_sqlite-2.625.24125/LICENSE
+-rw-rw-rw-   0        0        0     3463 2024-05-04 20:37:57.438780 mo_sqlite-2.625.24125/PKG-INFO
+-rw-rw-rw-   0        0        0     1913 2024-03-10 19:35:09.000000 mo_sqlite-2.625.24125/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 20:37:57.410921 mo_sqlite-2.625.24125/mo_sqlite/
+-rw-rw-rw-   0        0        0      507 2024-02-27 03:34:35.000000 mo_sqlite-2.625.24125/mo_sqlite/__init__.py
+-rw-rw-rw-   0        0        0    16971 2024-05-04 20:37:50.000000 mo_sqlite-2.625.24125/mo_sqlite/database.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:37:57.436725 mo_sqlite-2.625.24125/mo_sqlite/expressions/
+-rw-rw-rw-   0        0        0     1580 2024-03-10 20:49:59.000000 mo_sqlite-2.625.24125/mo_sqlite/expressions/__init__.py
+-rw-rw-rw-   0        0        0     1343 2024-03-11 06:29:29.000000 mo_sqlite-2.625.24125/mo_sqlite/expressions/_utils.py
+-rw-rw-rw-   0        0        0      585 2024-03-11 06:29:29.000000 mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_add_op.py
+-rw-rw-rw-   0        0        0      691 2024-03-11 06:29:29.000000 mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_alias_op.py
+-rw-rw-rw-   0        0        0     2991 2024-03-11 06:29:29.000000 mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_and_op.py
+-rw-rw-rw-   0        0        0     3244 2024-03-21 02:50:25.000000 mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_case_op.py
+-rw-rw-rw-   0        0        0      672 2024-03-10 20:49:59.000000 mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_cast_op.py
+-rw-rw-rw-   0        0        0     1034 2024-03-11 06:29:29.000000 mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_coalesce_op.py
+-rw-rw-rw-   0        0        0      575 2024-03-10 19:35:09.000000 mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_concat_op.py
+-rw-rw-rw-   0        0        0      497 2024-03-10 20:49:59.000000 mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_eq_op.py
+-rw-rw-rw-   0        0        0      446 2024-03-10 20:49:59.000000 mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_group_by_op.py
+-rw-rw-rw-   0        0        0      497 2024-02-15 03:48:30.000000 mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_gt_op.py
+-rw-rw-rw-   0        0        0      501 2024-02-15 03:48:30.000000 mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_gte_op.py
+-rw-rw-rw-   0        0        0      502 2024-03-10 20:49:59.000000 mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_in_op.py
+-rw-rw-rw-   0        0        0      681 2024-03-11 06:29:29.000000 mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_inner_join_op.py
+-rw-rw-rw-   0        0        0     1183 2024-03-11 06:29:29.000000 mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_instr_op.py
+-rw-rw-rw-   0        0        0      552 2024-03-11 06:29:29.000000 mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_is_null_op.py
+-rw-rw-rw-   0        0        0      378 2024-03-10 20:49:59.000000 mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_limit_op.py
+-rw-rw-rw-   0        0        0      725 2024-03-11 06:29:29.000000 mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_literal.py
+-rw-rw-rw-   0        0        0      617 2024-02-15 03:48:30.000000 mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_lt_op.py
+-rw-rw-rw-   0        0        0      501 2024-02-15 03:48:30.000000 mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_lte_op.py
+-rw-rw-rw-   0        0        0      570 2024-03-11 06:29:29.000000 mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_not_op.py
+-rw-rw-rw-   0        0        0     1713 2024-03-11 06:29:29.000000 mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_or_op.py
+-rw-rw-rw-   0        0        0      991 2024-03-10 20:49:59.000000 mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_order_by_op.py
+-rw-rw-rw-   0        0        0     4839 2024-03-21 02:50:25.000000 mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_script.py
+-rw-rw-rw-   0        0        0     2585 2024-03-11 06:29:29.000000 mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_select_op.py
+-rw-rw-rw-   0        0        0     1160 2024-03-11 06:29:29.000000 mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_substr_op.py
+-rw-rw-rw-   0        0        0      769 2024-03-11 06:29:29.000000 mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_variable.py
+-rw-rw-rw-   0        0        0     6684 2024-02-15 03:48:30.000000 mo_sqlite-2.625.24125/mo_sqlite/sql_script.py
+-rw-rw-rw-   0        0        0     6210 2024-03-18 02:53:29.000000 mo_sqlite-2.625.24125/mo_sqlite/transacfion.py
+-rw-rw-rw-   0        0        0     1543 2024-01-28 17:16:21.000000 mo_sqlite-2.625.24125/mo_sqlite/types.py
+-rw-rw-rw-   0        0        0     5687 2024-03-20 02:25:01.000000 mo_sqlite-2.625.24125/mo_sqlite/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:37:57.437736 mo_sqlite-2.625.24125/mo_sqlite.egg-info/
+-rw-rw-rw-   0        0        0     3463 2024-05-04 20:37:57.000000 mo_sqlite-2.625.24125/mo_sqlite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1364 2024-05-04 20:37:57.000000 mo_sqlite-2.625.24125/mo_sqlite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 20:37:57.000000 mo_sqlite-2.625.24125/mo_sqlite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      342 2024-05-04 20:37:57.000000 mo_sqlite-2.625.24125/mo_sqlite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-04 20:37:57.000000 mo_sqlite-2.625.24125/mo_sqlite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 20:37:57.438780 mo_sqlite-2.625.24125/setup.cfg
+-rw-rw-rw-   0        0        0     3334 2024-05-04 20:37:53.000000 mo_sqlite-2.625.24125/setup.py
```

### Comparing `mo_sqlite-2.607.24116/LICENSE` & `mo_sqlite-2.625.24125/LICENSE`

 * *Files identical despite different names*

### Comparing `mo_sqlite-2.607.24116/PKG-INFO` & `mo_sqlite-2.625.24125/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-sqlite
-Version: 2.607.24116
+Version: 2.625.24125
 Summary: Multithreading for Sqlite, plus expression composition
 Home-page: https://github.com/klahnakoski/mo-sqlite
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
@@ -15,27 +15,27 @@
 Classifier: Programming Language :: SQL
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: jx-python==4.607.24116
-Requires-Dist: mo-dots==9.606.24115
-Requires-Dist: mo-files==6.606.24115
+Requires-Dist: jx-python==4.625.24125
+Requires-Dist: mo-dots==10.623.24125
+Requires-Dist: mo-files==6.624.24125
 Requires-Dist: mo-future==7.584.24095
 Requires-Dist: mo-imports==7.584.24095
-Requires-Dist: mo-json==6.606.24115
-Requires-Dist: mo-kwargs==7.606.24115
-Requires-Dist: mo-logs==8.606.24115
-Requires-Dist: mo-math==7.606.24115
-Requires-Dist: mo-sql==4.606.24115
-Requires-Dist: mo-sql==4.606.24115
-Requires-Dist: mo-threads==6.606.24115
-Requires-Dist: mo-times==5.606.24115
+Requires-Dist: mo-json==6.624.24125
+Requires-Dist: mo-kwargs==7.623.24125
+Requires-Dist: mo-logs==8.623.24125
+Requires-Dist: mo-math==7.623.24125
+Requires-Dist: mo-sql==4.624.24125
+Requires-Dist: mo-sql==4.624.24125
+Requires-Dist: mo-threads==6.624.24125
+Requires-Dist: mo-times==5.623.24125
 Provides-Extra: tests
 Requires-Dist: mo-testing>=8.591.24112; extra == "tests"
 Requires-Dist: beautifulsoup4>=4.12.3; extra == "tests"
 
 # More SQLite!
 
 Multithreading for Sqlite, plus expression composition
```

### Comparing `mo_sqlite-2.607.24116/README.md` & `mo_sqlite-2.625.24125/README.md`

 * *Files identical despite different names*

### Comparing `mo_sqlite-2.607.24116/mo_sqlite/database.py` & `mo_sqlite-2.625.24125/mo_sqlite/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,15 @@
     def add_child(self, child):
         pass
 
     def close(self):
         logger.error("Use stop()")
 
     def __enter__(self):
-        pass
+        return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.stop()
 
     def create_new_functions(self):
         def regexp(pattern, item):
             return re.search(pattern, item) is not None
```

### Comparing `mo_sqlite-2.607.24116/mo_sqlite/expressions/__init__.py` & `mo_sqlite-2.625.24125/mo_sqlite/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `mo_sqlite-2.607.24116/mo_sqlite/expressions/_utils.py` & `mo_sqlite-2.625.24125/mo_sqlite/expressions/_utils.py`

 * *Files identical despite different names*

### Comparing `mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_add_op.py` & `mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_add_op.py`

 * *Files identical despite different names*

### Comparing `mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_alias_op.py` & `mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_alias_op.py`

 * *Files identical despite different names*

### Comparing `mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_and_op.py` & `mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_and_op.py`

 * *Files identical despite different names*

### Comparing `mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_case_op.py` & `mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_case_op.py`

 * *Files identical despite different names*

### Comparing `mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_cast_op.py` & `mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_cast_op.py`

 * *Files identical despite different names*

### Comparing `mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_coalesce_op.py` & `mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_coalesce_op.py`

 * *Files identical despite different names*

### Comparing `mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_concat_op.py` & `mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_concat_op.py`

 * *Files identical despite different names*

### Comparing `mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_inner_join_op.py` & `mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_inner_join_op.py`

 * *Files identical despite different names*

### Comparing `mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_instr_op.py` & `mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_instr_op.py`

 * *Files identical despite different names*

### Comparing `mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_is_null_op.py` & `mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_is_null_op.py`

 * *Files identical despite different names*

### Comparing `mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_literal.py` & `mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_literal.py`

 * *Files identical despite different names*

### Comparing `mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_lt_op.py` & `mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_lt_op.py`

 * *Files identical despite different names*

### Comparing `mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_not_op.py` & `mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_not_op.py`

 * *Files identical despite different names*

### Comparing `mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_or_op.py` & `mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_or_op.py`

 * *Files identical despite different names*

### Comparing `mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_order_by_op.py` & `mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_order_by_op.py`

 * *Files identical despite different names*

### Comparing `mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_script.py` & `mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_script.py`

 * *Files identical despite different names*

### Comparing `mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_select_op.py` & `mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_select_op.py`

 * *Files identical despite different names*

### Comparing `mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_substr_op.py` & `mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_substr_op.py`

 * *Files identical despite different names*

### Comparing `mo_sqlite-2.607.24116/mo_sqlite/expressions/sql_variable.py` & `mo_sqlite-2.625.24125/mo_sqlite/expressions/sql_variable.py`

 * *Files identical despite different names*

### Comparing `mo_sqlite-2.607.24116/mo_sqlite/sql_script.py` & `mo_sqlite-2.625.24125/mo_sqlite/sql_script.py`

 * *Files identical despite different names*

### Comparing `mo_sqlite-2.607.24116/mo_sqlite/transacfion.py` & `mo_sqlite-2.625.24125/mo_sqlite/transacfion.py`

 * *Files identical despite different names*

### Comparing `mo_sqlite-2.607.24116/mo_sqlite/types.py` & `mo_sqlite-2.625.24125/mo_sqlite/types.py`

 * *Files identical despite different names*

### Comparing `mo_sqlite-2.607.24116/mo_sqlite/utils.py` & `mo_sqlite-2.625.24125/mo_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `mo_sqlite-2.607.24116/mo_sqlite.egg-info/PKG-INFO` & `mo_sqlite-2.625.24125/mo_sqlite.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-sqlite
-Version: 2.607.24116
+Version: 2.625.24125
 Summary: Multithreading for Sqlite, plus expression composition
 Home-page: https://github.com/klahnakoski/mo-sqlite
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
@@ -15,27 +15,27 @@
 Classifier: Programming Language :: SQL
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: jx-python==4.607.24116
-Requires-Dist: mo-dots==9.606.24115
-Requires-Dist: mo-files==6.606.24115
+Requires-Dist: jx-python==4.625.24125
+Requires-Dist: mo-dots==10.623.24125
+Requires-Dist: mo-files==6.624.24125
 Requires-Dist: mo-future==7.584.24095
 Requires-Dist: mo-imports==7.584.24095
-Requires-Dist: mo-json==6.606.24115
-Requires-Dist: mo-kwargs==7.606.24115
-Requires-Dist: mo-logs==8.606.24115
-Requires-Dist: mo-math==7.606.24115
-Requires-Dist: mo-sql==4.606.24115
-Requires-Dist: mo-sql==4.606.24115
-Requires-Dist: mo-threads==6.606.24115
-Requires-Dist: mo-times==5.606.24115
+Requires-Dist: mo-json==6.624.24125
+Requires-Dist: mo-kwargs==7.623.24125
+Requires-Dist: mo-logs==8.623.24125
+Requires-Dist: mo-math==7.623.24125
+Requires-Dist: mo-sql==4.624.24125
+Requires-Dist: mo-sql==4.624.24125
+Requires-Dist: mo-threads==6.624.24125
+Requires-Dist: mo-times==5.623.24125
 Provides-Extra: tests
 Requires-Dist: mo-testing>=8.591.24112; extra == "tests"
 Requires-Dist: beautifulsoup4>=4.12.3; extra == "tests"
 
 # More SQLite!
 
 Multithreading for Sqlite, plus expression composition
```

### Comparing `mo_sqlite-2.607.24116/mo_sqlite.egg-info/SOURCES.txt` & `mo_sqlite-2.625.24125/mo_sqlite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mo_sqlite-2.607.24116/setup.py` & `mo_sqlite-2.625.24125/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 setup(
     author='Kyle Lahnakoski',
     author_email='kyle@lahnakoski.com',
     classifiers=["Development Status :: 4 - Beta","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules","License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)","Topic :: Database","Topic :: Utilities","Programming Language :: SQL","Programming Language :: Python :: 3.8","Programming Language :: Python :: 3.9","Programming Language :: Python :: 3.11","Programming Language :: Python :: 3.12"],
     description='Multithreading for Sqlite, plus expression composition',
     extras_require={"tests":["mo-testing>=8.591.24112","beautifulsoup4>=4.12.3"]},
     include_package_data=True,
-    install_requires=["jx-python==4.607.24116","mo-dots==9.606.24115","mo-files==6.606.24115","mo-future==7.584.24095","mo-imports==7.584.24095","mo-json==6.606.24115","mo-kwargs==7.606.24115","mo-logs==8.606.24115","mo-math==7.606.24115","mo-sql==4.606.24115","mo-sql==4.606.24115","mo-threads==6.606.24115","mo-times==5.606.24115"],
+    install_requires=["jx-python==4.625.24125","mo-dots==10.623.24125","mo-files==6.624.24125","mo-future==7.584.24095","mo-imports==7.584.24095","mo-json==6.624.24125","mo-kwargs==7.623.24125","mo-logs==8.623.24125","mo-math==7.623.24125","mo-sql==4.624.24125","mo-sql==4.624.24125","mo-threads==6.624.24125","mo-times==5.623.24125"],
     license='MPL 2.0',
     long_description='# More SQLite!\n\nMultithreading for Sqlite, plus expression composition\n\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-sqlite.svg)](https://pypi.org/project/mo-sqlite/)\n[![Build Status](https://github.com/klahnakoski/mo-sqlite/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-sqlite/actions/workflows/build.yml)\n[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-sqlite/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-sqlite?branch=dev)\n[![Downloads](https://pepy.tech/badge/mo-sqlite/month)](https://pepy.tech/project/mo-sqlite)\n\n\n## Multi-threaded Sqlite\n\nThis module wraps the `sqlite3.connection` with thread-safe traffic manager.  Here is typical usage: \n\n    from mo_sqlite import Sqlite\n    db = Sqlite("mydb.sqlite")\n    with db.transaction() as t:\n        t.command("insert into mytable values (1, 2, 3)")\n\nWhile you may have each thread own a `sqlite3.connection` to the same file, you will still get exceptions when another thread has the file locked.\n\n## Pull JSON out of database\n\nThis module includes a minimum experimental structure that can describe pulling deeply nested JSON documents out of a normalized database.  The tactic is to shape a single query who\'s resultset can be easily converted to the desired JSON by Python. Read more on [pulling json from a database](docs/JSON%20in%20Database.md)\n\nThere are multiple normal forms, including domain key normal form, and columnar form;  these have a multitude one-to-one relations, all represent the same logical schema, but differ in their access patterns to optimize for particular use cases.  This module intends to hide the particular database schema from the caller; exposing just the logical schema. \n\n\n\nThis experiment compliments the [mo-columns](https://github.com/klahnakoski/mo-columns) experiment, which is about pushing JSON into a database. \n   ',
     long_description_content_type='text/markdown',
     name='mo-sqlite',
     packages=["mo_sqlite","mo_sqlite.expressions"],
     url='https://github.com/klahnakoski/mo-sqlite',
-    version='2.607.24116'
+    version='2.625.24125'
 )
```

