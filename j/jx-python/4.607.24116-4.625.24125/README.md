# Comparing `tmp/jx_python-4.607.24116.tar.gz` & `tmp/jx_python-4.625.24125.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jx_python-4.607.24116.tar", last modified: Thu Apr 25 00:55:36 2024, max compression
+gzip compressed data, was "jx_python-4.625.24125.tar", last modified: Sat May  4 20:35:50 2024, max compression
```

## Comparing `jx_python-4.607.24116.tar` & `jx_python-4.625.24125.tar`

### file list

```diff
@@ -1,286 +1,286 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 00:55:36.980508 jx_python-4.607.24116/
--rw-rw-rw-   0        0        0    16725 2019-09-12 20:44:42.000000 jx_python-4.607.24116/LICENSE
--rw-rw-rw-   0        0        0     1743 2024-04-25 00:55:36.980508 jx_python-4.607.24116/PKG-INFO
--rw-rw-rw-   0        0        0      501 2024-03-08 02:37:16.000000 jx_python-4.607.24116/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 00:55:36.675579 jx_python-4.607.24116/jx_base/
--rw-rw-rw-   0        0        0     1553 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_base/__init__.py
--rw-rw-rw-   0        0        0     8710 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/data_class.py
--rw-rw-rw-   0        0        0    25274 2024-02-06 05:15:22.000000 jx_python-4.607.24116/jx_base/domains.py
-drwxrwxrwx   0        0        0        0 2024-04-25 00:55:36.859450 jx_python-4.607.24116/jx_base/expressions/
--rw-rw-rw-   0        0        0    10593 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_base/expressions/__init__.py
--rw-rw-rw-   0        0        0     4925 2024-03-20 02:23:03.000000 jx_python-4.607.24116/jx_base/expressions/_utils.py
--rw-rw-rw-   0        0        0     1027 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/abs_op.py
--rw-rw-rw-   0        0        0      800 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/expressions/add_op.py
--rw-rw-rw-   0        0        0     2379 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/aggregate_op.py
--rw-rw-rw-   0        0        0     1277 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/expressions/all_op.py
--rw-rw-rw-   0        0        0     3312 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/and_op.py
--rw-rw-rw-   0        0        0     1394 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/any_op.py
--rw-rw-rw-   0        0        0      918 2023-06-17 11:25:18.000000 jx_python-4.607.24116/jx_base/expressions/array_of_op.py
--rw-rw-rw-   0        0        0      453 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/expressions/avg_op.py
--rw-rw-rw-   0        0        0     2183 2024-01-22 13:00:58.000000 jx_python-4.607.24116/jx_base/expressions/base_binary_op.py
--rw-rw-rw-   0        0        0      520 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/base_inequality_op.py
--rw-rw-rw-   0        0        0     2960 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/expressions/base_multi_op.py
--rw-rw-rw-   0        0        0     4496 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_base/expressions/between_op.py
--rw-rw-rw-   0        0        0     1544 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/call_op.py
--rw-rw-rw-   0        0        0      661 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/expressions/cardinality_op.py
--rw-rw-rw-   0        0        0     4044 2024-03-21 02:47:56.000000 jx_python-4.607.24116/jx_base/expressions/case_op.py
--rw-rw-rw-   0        0        0     2037 2024-02-27 03:13:49.000000 jx_python-4.607.24116/jx_base/expressions/coalesce_op.py
--rw-rw-rw-   0        0        0     1593 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/comment_op.py
--rw-rw-rw-   0        0        0     2890 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/concat_op.py
--rw-rw-rw-   0        0        0     1592 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/expressions/count_op.py
--rw-rw-rw-   0        0        0     1250 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/date_op.py
--rw-rw-rw-   0        0        0     2111 2024-02-27 03:13:49.000000 jx_python-4.607.24116/jx_base/expressions/default_op.py
--rw-rw-rw-   0        0        0     1179 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/expressions/div_op.py
--rw-rw-rw-   0        0        0     2757 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_base/expressions/eq_op.py
--rw-rw-rw-   0        0        0      418 2023-06-17 11:25:18.000000 jx_python-4.607.24116/jx_base/expressions/es_script.py
--rw-rw-rw-   0        0        0     1525 2024-01-28 16:03:01.000000 jx_python-4.607.24116/jx_base/expressions/es_select_op.py
--rw-rw-rw-   0        0        0     1270 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/exists_op.py
--rw-rw-rw-   0        0        0      373 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/expressions/exp_op.py
--rw-rw-rw-   0        0        0     6265 2024-01-22 13:00:58.000000 jx_python-4.607.24116/jx_base/expressions/expression.py
--rw-rw-rw-   0        0        0     1524 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/false_op.py
--rw-rw-rw-   0        0        0     1278 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/filter_op.py
--rw-rw-rw-   0        0        0     2242 2024-01-28 16:03:01.000000 jx_python-4.607.24116/jx_base/expressions/find_op.py
--rw-rw-rw-   0        0        0     2413 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/first_op.py
--rw-rw-rw-   0        0        0      657 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/floor_op.py
--rw-rw-rw-   0        0        0    10147 2024-02-06 05:15:22.000000 jx_python-4.607.24116/jx_base/expressions/format_op.py
--rw-rw-rw-   0        0        0     1577 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/from_op.py
--rw-rw-rw-   0        0        0      807 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/from_unix_op.py
--rw-rw-rw-   0        0        0     3022 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/get_op.py
--rw-rw-rw-   0        0        0     1082 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/group_op.py
--rw-rw-rw-   0        0        0      385 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/gt_op.py
--rw-rw-rw-   0        0        0      386 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/gte_op.py
--rw-rw-rw-   0        0        0     3648 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_base/expressions/in_op.py
--rw-rw-rw-   0        0        0     2505 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/inner_join_op.py
--rw-rw-rw-   0        0        0     1322 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/is_boolean_op.py
--rw-rw-rw-   0        0        0      969 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/is_integer_op.py
--rw-rw-rw-   0        0        0     1360 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/is_number_op.py
--rw-rw-rw-   0        0        0     1451 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/is_text_op.py
--rw-rw-rw-   0        0        0     1561 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/last_op.py
--rw-rw-rw-   0        0        0     1761 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/expressions/least_op.py
--rw-rw-rw-   0        0        0     1252 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/leaves_op.py
--rw-rw-rw-   0        0        0     2037 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_base/expressions/left_op.py
--rw-rw-rw-   0        0        0     1601 2024-02-27 03:13:49.000000 jx_python-4.607.24116/jx_base/expressions/length_op.py
--rw-rw-rw-   0        0        0     2593 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/limit_op.py
--rw-rw-rw-   0        0        0     3326 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/expressions/literal.py
--rw-rw-rw-   0        0        0      384 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/expressions/lt_op.py
--rw-rw-rw-   0        0        0      385 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/expressions/lte_op.py
--rw-rw-rw-   0        0        0      507 2023-06-17 11:25:18.000000 jx_python-4.607.24116/jx_base/expressions/map_op.py
--rw-rw-rw-   0        0        0     1418 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/max_op.py
--rw-rw-rw-   0        0        0     1442 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/min_op.py
--rw-rw-rw-   0        0        0     1861 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_base/expressions/missing_op.py
--rw-rw-rw-   0        0        0      373 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/expressions/mod_op.py
--rw-rw-rw-   0        0        0      845 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/expressions/most_op.py
--rw-rw-rw-   0        0        0      882 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/expressions/mul_op.py
--rw-rw-rw-   0        0        0     1170 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/name_op.py
--rw-rw-rw-   0        0        0     1647 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_base/expressions/ne_op.py
--rw-rw-rw-   0        0        0     4366 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_base/expressions/nested_op.py
--rw-rw-rw-   0        0        0     2061 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_base/expressions/not_left_op.py
--rw-rw-rw-   0        0        0     1612 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_base/expressions/not_op.py
--rw-rw-rw-   0        0        0     2150 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_base/expressions/not_right_op.py
--rw-rw-rw-   0        0        0     2442 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_base/expressions/null_op.py
--rw-rw-rw-   0        0        0     1059 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/offset_op.py
--rw-rw-rw-   0        0        0     2239 2024-03-02 22:12:26.000000 jx_python-4.607.24116/jx_base/expressions/or_op.py
--rw-rw-rw-   0        0        0     2503 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/outer_join_op.py
--rw-rw-rw-   0        0        0     1387 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/expressions/percentile_op.py
--rw-rw-rw-   0        0        0     3285 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_base/expressions/prefix_op.py
--rw-rw-rw-   0        0        0     1585 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/product_op.py
--rw-rw-rw-   0        0        0      460 2023-06-17 11:25:18.000000 jx_python-4.607.24116/jx_base/expressions/python_function.py
--rw-rw-rw-   0        0        0     1512 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/python_script.py
--rw-rw-rw-   0        0        0    24585 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_base/expressions/query_op.py
--rw-rw-rw-   0        0        0     1025 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/range_op.py
--rw-rw-rw-   0        0        0     1575 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/reg_exp_op.py
--rw-rw-rw-   0        0        0     2247 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_base/expressions/right_op.py
--rw-rw-rw-   0        0        0     1478 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/rows_op.py
--rw-rw-rw-   0        0        0     1247 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/script_op.py
--rw-rw-rw-   0        0        0    12251 2024-02-15 03:10:30.000000 jx_python-4.607.24116/jx_base/expressions/select_op.py
--rw-rw-rw-   0        0        0     1860 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/split_op.py
--rw-rw-rw-   0        0        0     1295 2024-02-15 03:10:30.000000 jx_python-4.607.24116/jx_base/expressions/sql_alias_op.py
--rw-rw-rw-   0        0        0     1027 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/expressions/sql_and_op.py
--rw-rw-rw-   0        0        0     1010 2024-02-27 03:13:49.000000 jx_python-4.607.24116/jx_base/expressions/sql_cast_op.py
--rw-rw-rw-   0        0        0     1361 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/expressions/sql_concat_op.py
--rw-rw-rw-   0        0        0     1490 2024-03-10 19:33:03.000000 jx_python-4.607.24116/jx_base/expressions/sql_eq_op.py
--rw-rw-rw-   0        0        0     1082 2023-06-17 11:25:18.000000 jx_python-4.607.24116/jx_base/expressions/sql_group_by_op.py
--rw-rw-rw-   0        0        0      423 2024-02-15 03:46:10.000000 jx_python-4.607.24116/jx_base/expressions/sql_gt_op.py
--rw-rw-rw-   0        0        0      424 2024-02-15 03:46:10.000000 jx_python-4.607.24116/jx_base/expressions/sql_gte_op.py
--rw-rw-rw-   0        0        0      343 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/expressions/sql_in_op.py
--rw-rw-rw-   0        0        0      428 2024-01-22 13:00:58.000000 jx_python-4.607.24116/jx_base/expressions/sql_inner_join_op.py
--rw-rw-rw-   0        0        0     1192 2024-02-27 03:13:49.000000 jx_python-4.607.24116/jx_base/expressions/sql_instr_op.py
--rw-rw-rw-   0        0        0      832 2024-03-10 19:33:03.000000 jx_python-4.607.24116/jx_base/expressions/sql_is_null_op.py
--rw-rw-rw-   0        0        0     3313 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/sql_left_joins_op.py
--rw-rw-rw-   0        0        0      499 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/expressions/sql_limit_op.py
--rw-rw-rw-   0        0        0      360 2024-02-15 03:10:30.000000 jx_python-4.607.24116/jx_base/expressions/sql_literal.py
--rw-rw-rw-   0        0        0      423 2024-02-15 03:46:10.000000 jx_python-4.607.24116/jx_base/expressions/sql_lt_op.py
--rw-rw-rw-   0        0        0      424 2024-02-15 03:46:10.000000 jx_python-4.607.24116/jx_base/expressions/sql_lte_op.py
--rw-rw-rw-   0        0        0     1449 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_base/expressions/sql_not_op.py
--rw-rw-rw-   0        0        0     2371 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/expressions/sql_or_op.py
--rw-rw-rw-   0        0        0      781 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/expressions/sql_order_by_op.py
--rw-rw-rw-   0        0        0     1057 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/sql_origins_op.py
--rw-rw-rw-   0        0        0      427 2023-06-17 11:25:18.000000 jx_python-4.607.24116/jx_base/expressions/sql_script.py
--rw-rw-rw-   0        0        0      958 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/sql_select_all_from_op.py
--rw-rw-rw-   0        0        0     2012 2024-02-15 03:10:30.000000 jx_python-4.607.24116/jx_base/expressions/sql_select_op.py
--rw-rw-rw-   0        0        0      911 2024-03-10 19:33:03.000000 jx_python-4.607.24116/jx_base/expressions/sql_substr_op.py
--rw-rw-rw-   0        0        0     1583 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/expressions/sql_variable.py
--rw-rw-rw-   0        0        0      396 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_base/expressions/strict_add_op.py
--rw-rw-rw-   0        0        0     1549 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_base/expressions/strict_boolean_op.py
--rw-rw-rw-   0        0        0     1112 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_base/expressions/strict_eq_op.py
--rw-rw-rw-   0        0        0     3378 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_base/expressions/strict_in_op.py
--rw-rw-rw-   0        0        0     1976 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_base/expressions/strict_index_of_op.py
--rw-rw-rw-   0        0        0      396 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_base/expressions/strict_mul_op.py
--rw-rw-rw-   0        0        0     1967 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_base/expressions/strict_multi_op.py
--rw-rw-rw-   0        0        0     1281 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_base/expressions/strict_not_op.py
--rw-rw-rw-   0        0        0     1671 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_base/expressions/strict_starts_with_op.py
--rw-rw-rw-   0        0        0     1335 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_base/expressions/strict_substring_op.py
--rw-rw-rw-   0        0        0      611 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/sub_op.py
--rw-rw-rw-   0        0        0     3011 2024-03-02 22:12:26.000000 jx_python-4.607.24116/jx_base/expressions/suffix_op.py
--rw-rw-rw-   0        0        0     1556 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/expressions/sum_op.py
--rw-rw-rw-   0        0        0      721 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/expressions/tally_op.py
--rw-rw-rw-   0        0        0     1594 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/to_array_op.py
--rw-rw-rw-   0        0        0     1304 2024-03-02 22:12:26.000000 jx_python-4.607.24116/jx_base/expressions/to_boolean_op.py
--rw-rw-rw-   0        0        0     2708 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/expressions/to_integer_op.py
--rw-rw-rw-   0        0        0     2874 2024-03-02 22:12:26.000000 jx_python-4.607.24116/jx_base/expressions/to_number_op.py
--rw-rw-rw-   0        0        0     2043 2024-03-10 19:33:03.000000 jx_python-4.607.24116/jx_base/expressions/to_text_op.py
--rw-rw-rw-   0        0        0     1170 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/to_value_op.py
--rw-rw-rw-   0        0        0     1626 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/true_op.py
--rw-rw-rw-   0        0        0     1678 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/tuple_op.py
--rw-rw-rw-   0        0        0     2000 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/union_op.py
--rw-rw-rw-   0        0        0      826 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/expressions/unix_op.py
--rw-rw-rw-   0        0        0     6148 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_base/expressions/variable.py
--rw-rw-rw-   0        0        0     3270 2024-03-21 02:47:56.000000 jx_python-4.607.24116/jx_base/expressions/when_op.py
--rw-rw-rw-   0        0        0    14489 2024-04-25 00:55:28.000000 jx_python-4.607.24116/jx_base/language.py
--rw-rw-rw-   0        0        0    15169 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_base/meta_columns.py
-drwxrwxrwx   0        0        0        0 2024-04-25 00:55:36.870195 jx_python-4.607.24116/jx_base/models/
--rw-rw-rw-   0        0        0        0 2022-11-12 15:14:28.000000 jx_python-4.607.24116/jx_base/models/__init__.py
--rw-rw-rw-   0        0        0     2369 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/models/container.py
--rw-rw-rw-   0        0        0    13016 2023-06-17 11:25:18.000000 jx_python-4.607.24116/jx_base/models/dimensions.py
--rw-rw-rw-   0        0        0      945 2023-06-17 11:25:18.000000 jx_python-4.607.24116/jx_base/models/facts.py
--rw-rw-rw-   0        0        0     1656 2023-06-17 11:25:18.000000 jx_python-4.607.24116/jx_base/models/namespace.py
--rw-rw-rw-   0        0        0      294 2023-06-17 11:25:18.000000 jx_python-4.607.24116/jx_base/models/nested_path.py
--rw-rw-rw-   0        0        0      408 2023-06-17 11:25:18.000000 jx_python-4.607.24116/jx_base/models/relation.py
--rw-rw-rw-   0        0        0     5523 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/models/schema.py
--rw-rw-rw-   0        0        0      833 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/models/snowflake.py
--rw-rw-rw-   0        0        0      687 2024-03-16 21:27:51.000000 jx_python-4.607.24116/jx_base/models/table.py
--rw-rw-rw-   0        0        0      791 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_base/queries.py
--rw-rw-rw-   0        0        0     2520 2024-02-15 03:10:30.000000 jx_python-4.607.24116/jx_base/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-25 00:55:36.880751 jx_python-4.607.24116/jx_python/
--rw-rw-rw-   0        0        0      614 2024-03-16 21:32:01.000000 jx_python-4.607.24116/jx_python/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 00:55:36.901107 jx_python-4.607.24116/jx_python/containers/
--rw-rw-rw-   0        0        0        0 2019-09-12 20:44:42.000000 jx_python-4.607.24116/jx_python/containers/__init__.py
--rw-rw-rw-   0        0        0    16625 2023-06-17 11:25:18.000000 jx_python-4.607.24116/jx_python/containers/cube.py
--rw-rw-rw-   0        0        0     9580 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_python/containers/list.py
--rw-rw-rw-   0        0        0     1836 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/convert.py
-drwxrwxrwx   0        0        0        0 2024-04-25 00:55:36.902117 jx_python-4.607.24116/jx_python/cubes/
--rw-rw-rw-   0        0        0        0 2020-01-29 00:24:56.000000 jx_python-4.607.24116/jx_python/cubes/__init__.py
--rw-rw-rw-   0        0        0     3647 2023-06-17 11:25:18.000000 jx_python-4.607.24116/jx_python/cubes/aggs.py
--rw-rw-rw-   0        0        0     1920 2024-03-16 21:32:01.000000 jx_python-4.607.24116/jx_python/expression_compiler.py
-drwxrwxrwx   0        0        0        0 2024-04-25 00:55:36.970402 jx_python-4.607.24116/jx_python/expressions/
--rw-rw-rw-   0        0        0     3964 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_python/expressions/__init__.py
--rw-rw-rw-   0        0        0     4651 2024-04-25 00:55:28.000000 jx_python-4.607.24116/jx_python/expressions/_utils.py
--rw-rw-rw-   0        0        0      440 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/add_op.py
--rw-rw-rw-   0        0        0      945 2024-02-27 03:13:49.000000 jx_python-4.607.24116/jx_python/expressions/and_op.py
--rw-rw-rw-   0        0        0      857 2024-03-16 21:32:01.000000 jx_python-4.607.24116/jx_python/expressions/array_of_op.py
--rw-rw-rw-   0        0        0      714 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/avg_op.py
--rw-rw-rw-   0        0        0      372 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/between_op.py
--rw-rw-rw-   0        0        0     1285 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/call_op.py
--rw-rw-rw-   0        0        0      673 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/cardinality_op.py
--rw-rw-rw-   0        0        0      716 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/case_op.py
--rw-rw-rw-   0        0        0      976 2024-01-21 21:27:17.000000 jx_python-4.607.24116/jx_python/expressions/coalesce_op.py
--rw-rw-rw-   0        0        0     1146 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/concat_op.py
--rw-rw-rw-   0        0        0      786 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/count_op.py
--rw-rw-rw-   0        0        0      554 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/date_op.py
--rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/div_op.py
--rw-rw-rw-   0        0        0     1608 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_python/expressions/eq_op.py
--rw-rw-rw-   0        0        0      750 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/exists_op.py
--rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/exp_op.py
--rw-rw-rw-   0        0        0      635 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/false_op.py
--rw-rw-rw-   0        0        0     1110 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/filter_op.py
--rw-rw-rw-   0        0        0     1692 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_python/expressions/find_op.py
--rw-rw-rw-   0        0        0      962 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/first_op.py
--rw-rw-rw-   0        0        0      647 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/floor_op.py
--rw-rw-rw-   0        0        0      368 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/format_op.py
--rw-rw-rw-   0        0        0     1823 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/get_op.py
--rw-rw-rw-   0        0        0     1718 2024-04-24 23:41:46.000000 jx_python-4.607.24116/jx_python/expressions/group_op.py
--rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/gt_op.py
--rw-rw-rw-   0        0        0      448 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/gte_op.py
--rw-rw-rw-   0        0        0      831 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/in_op.py
--rw-rw-rw-   0        0        0      787 2024-03-16 21:32:01.000000 jx_python-4.607.24116/jx_python/expressions/is_text_op.py
--rw-rw-rw-   0        0        0     1109 2024-03-16 21:32:01.000000 jx_python-4.607.24116/jx_python/expressions/last_op.py
--rw-rw-rw-   0        0        0     1026 2024-02-27 03:13:49.000000 jx_python-4.607.24116/jx_python/expressions/least_op.py
--rw-rw-rw-   0        0        0      559 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/leaves_op.py
--rw-rw-rw-   0        0        0      692 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/length_op.py
--rw-rw-rw-   0        0        0      953 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/limit_op.py
--rw-rw-rw-   0        0        0      618 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/literal.py
--rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/lt_op.py
--rw-rw-rw-   0        0        0      448 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/lte_op.py
--rw-rw-rw-   0        0        0      694 2024-03-16 21:32:01.000000 jx_python-4.607.24116/jx_python/expressions/max_op.py
--rw-rw-rw-   0        0        0      694 2024-03-16 21:32:01.000000 jx_python-4.607.24116/jx_python/expressions/min_op.py
--rw-rw-rw-   0        0        0     1045 2024-03-16 21:32:01.000000 jx_python-4.607.24116/jx_python/expressions/missing_op.py
--rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/mod_op.py
--rw-rw-rw-   0        0        0      981 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/most_op.py
--rw-rw-rw-   0        0        0      533 2024-03-16 21:32:01.000000 jx_python-4.607.24116/jx_python/expressions/mul_op.py
--rw-rw-rw-   0        0        0      992 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/name_op.py
--rw-rw-rw-   0        0        0      733 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/ne_op.py
--rw-rw-rw-   0        0        0      773 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/not_left_op.py
--rw-rw-rw-   0        0        0      680 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/not_op.py
--rw-rw-rw-   0        0        0      999 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/not_right_op.py
--rw-rw-rw-   0        0        0      556 2024-03-16 21:32:01.000000 jx_python-4.607.24116/jx_python/expressions/offset_op.py
--rw-rw-rw-   0        0        0      930 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/or_op.py
--rw-rw-rw-   0        0        0      468 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/percentile_op.py
--rw-rw-rw-   0        0        0      651 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/prefix_op.py
--rw-rw-rw-   0        0        0     1303 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/product_op.py
--rw-rw-rw-   0        0        0     1139 2024-03-16 21:32:01.000000 jx_python-4.607.24116/jx_python/expressions/python_function.py
--rw-rw-rw-   0        0        0     1443 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/python_script.py
--rw-rw-rw-   0        0        0      364 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/range_op.py
--rw-rw-rw-   0        0        0      946 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/reg_exp_op.py
--rw-rw-rw-   0        0        0      699 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/right_op.py
--rw-rw-rw-   0        0        0     1022 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/rows_op.py
--rw-rw-rw-   0        0        0      594 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/script_op.py
--rw-rw-rw-   0        0        0     2105 2024-03-16 21:32:01.000000 jx_python-4.607.24116/jx_python/expressions/select_op.py
--rw-rw-rw-   0        0        0      643 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/split_op.py
--rw-rw-rw-   0        0        0      888 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_python/expressions/strict_add_op.py
--rw-rw-rw-   0        0        0      850 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_python/expressions/strict_eq_op.py
--rw-rw-rw-   0        0        0      870 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_python/expressions/strict_index_of_op.py
--rw-rw-rw-   0        0        0      912 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_python/expressions/strict_starts_with_op.py
--rw-rw-rw-   0        0        0      998 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_python/expressions/strict_substring_op.py
--rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/sub_op.py
--rw-rw-rw-   0        0        0      742 2024-02-27 03:13:49.000000 jx_python-4.607.24116/jx_python/expressions/suffix_op.py
--rw-rw-rw-   0        0        0     1252 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/sum_op.py
--rw-rw-rw-   0        0        0     1056 2024-03-16 21:32:01.000000 jx_python-4.607.24116/jx_python/expressions/tally_op.py
--rw-rw-rw-   0        0        0      835 2024-03-16 21:32:01.000000 jx_python-4.607.24116/jx_python/expressions/to_array_op.py
--rw-rw-rw-   0        0        0      962 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/to_boolean_op.py
--rw-rw-rw-   0        0        0      606 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/to_integer_op.py
--rw-rw-rw-   0        0        0     1034 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/to_number_op.py
--rw-rw-rw-   0        0        0      800 2024-03-16 21:32:01.000000 jx_python-4.607.24116/jx_python/expressions/to_text_op.py
--rw-rw-rw-   0        0        0      957 2024-03-16 21:32:01.000000 jx_python-4.607.24116/jx_python/expressions/to_value_op.py
--rw-rw-rw-   0        0        0      628 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/true_op.py
--rw-rw-rw-   0        0        0      812 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/tuple_op.py
--rw-rw-rw-   0        0        0     1328 2024-03-16 21:32:01.000000 jx_python-4.607.24116/jx_python/expressions/variable.py
--rw-rw-rw-   0        0        0      968 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/expressions/when_op.py
--rw-rw-rw-   0        0        0     4434 2023-06-17 11:25:18.000000 jx_python-4.607.24116/jx_python/flat_list.py
--rw-rw-rw-   0        0        0     4439 2023-06-17 11:25:18.000000 jx_python-4.607.24116/jx_python/group_by.py
--rw-rw-rw-   0        0        0    34076 2024-01-25 04:46:12.000000 jx_python-4.607.24116/jx_python/jx.py
-drwxrwxrwx   0        0        0        0 2024-04-25 00:55:36.970402 jx_python-4.607.24116/jx_python/lists/
--rw-rw-rw-   0        0        0        0 2019-09-12 20:44:42.000000 jx_python-4.607.24116/jx_python/lists/__init__.py
--rw-rw-rw-   0        0        0     5009 2024-04-04 04:16:05.000000 jx_python-4.607.24116/jx_python/lists/aggs.py
-drwxrwxrwx   0        0        0        0 2024-04-25 00:55:36.976917 jx_python-4.607.24116/jx_python/namespace/
--rw-rw-rw-   0        0        0        0 2019-09-12 20:44:42.000000 jx_python-4.607.24116/jx_python/namespace/__init__.py
--rw-rw-rw-   0        0        0     8745 2024-01-20 18:36:41.000000 jx_python-4.607.24116/jx_python/namespace/normal.py
--rw-rw-rw-   0        0        0      768 2023-06-17 11:25:18.000000 jx_python-4.607.24116/jx_python/records.py
-drwxrwxrwx   0        0        0        0 2024-04-25 00:55:36.980508 jx_python-4.607.24116/jx_python/streams/
--rw-rw-rw-   0        0        0     4178 2024-03-16 21:32:01.000000 jx_python-4.607.24116/jx_python/streams/__init__.py
--rw-rw-rw-   0        0        0     1926 2023-06-17 11:25:18.000000 jx_python-4.607.24116/jx_python/streams/expression_compiler.py
--rw-rw-rw-   0        0        0     4531 2024-04-24 23:41:46.000000 jx_python-4.607.24116/jx_python/streams/expression_factory.py
--rw-rw-rw-   0        0        0      713 2023-06-17 11:25:18.000000 jx_python-4.607.24116/jx_python/streams/inspects.py
--rw-rw-rw-   0        0        0      807 2023-06-17 11:25:18.000000 jx_python-4.607.24116/jx_python/streams/type_parser.py
--rw-rw-rw-   0        0        0     5515 2023-06-17 11:25:18.000000 jx_python-4.607.24116/jx_python/streams/typers.py
--rw-rw-rw-   0        0        0     1622 2024-03-16 21:32:01.000000 jx_python-4.607.24116/jx_python/streams.py
--rw-rw-rw-   0        0        0      564 2023-06-17 11:25:18.000000 jx_python-4.607.24116/jx_python/table.py
--rw-rw-rw-   0        0        0     1431 2023-06-17 11:25:18.000000 jx_python-4.607.24116/jx_python/utils.py
--rw-rw-rw-   0        0        0     7410 2023-06-17 11:25:18.000000 jx_python-4.607.24116/jx_python/windows.py
-drwxrwxrwx   0        0        0        0 2024-04-25 00:55:36.980508 jx_python-4.607.24116/jx_python.egg-info/
--rw-rw-rw-   0        0        0     1743 2024-04-25 00:55:36.000000 jx_python-4.607.24116/jx_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8849 2024-04-25 00:55:36.000000 jx_python-4.607.24116/jx_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 00:55:36.000000 jx_python-4.607.24116/jx_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      265 2024-04-25 00:55:36.000000 jx_python-4.607.24116/jx_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-25 00:55:36.000000 jx_python-4.607.24116/jx_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 00:55:36.980508 jx_python-4.607.24116/setup.cfg
--rw-rw-rw-   0        0        0     1872 2024-04-25 00:55:31.000000 jx_python-4.607.24116/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:35:50.470042 jx_python-4.625.24125/
+-rw-rw-rw-   0        0        0    16725 2019-09-12 20:44:42.000000 jx_python-4.625.24125/LICENSE
+-rw-rw-rw-   0        0        0     1744 2024-05-04 20:35:50.468962 jx_python-4.625.24125/PKG-INFO
+-rw-rw-rw-   0        0        0      501 2024-03-08 02:37:16.000000 jx_python-4.625.24125/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 20:35:50.254062 jx_python-4.625.24125/jx_base/
+-rw-rw-rw-   0        0        0     1553 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_base/__init__.py
+-rw-rw-rw-   0        0        0     8710 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/data_class.py
+-rw-rw-rw-   0        0        0    25274 2024-02-06 05:15:22.000000 jx_python-4.625.24125/jx_base/domains.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:35:50.357627 jx_python-4.625.24125/jx_base/expressions/
+-rw-rw-rw-   0        0        0    10593 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_base/expressions/__init__.py
+-rw-rw-rw-   0        0        0     4925 2024-03-20 02:23:03.000000 jx_python-4.625.24125/jx_base/expressions/_utils.py
+-rw-rw-rw-   0        0        0     1027 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/abs_op.py
+-rw-rw-rw-   0        0        0      800 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/expressions/add_op.py
+-rw-rw-rw-   0        0        0     2379 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/aggregate_op.py
+-rw-rw-rw-   0        0        0     1277 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/expressions/all_op.py
+-rw-rw-rw-   0        0        0     3312 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/and_op.py
+-rw-rw-rw-   0        0        0     1394 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/any_op.py
+-rw-rw-rw-   0        0        0      918 2023-06-17 11:25:18.000000 jx_python-4.625.24125/jx_base/expressions/array_of_op.py
+-rw-rw-rw-   0        0        0      453 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/expressions/avg_op.py
+-rw-rw-rw-   0        0        0     2183 2024-01-22 13:00:58.000000 jx_python-4.625.24125/jx_base/expressions/base_binary_op.py
+-rw-rw-rw-   0        0        0      520 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/base_inequality_op.py
+-rw-rw-rw-   0        0        0     2960 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/expressions/base_multi_op.py
+-rw-rw-rw-   0        0        0     4496 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_base/expressions/between_op.py
+-rw-rw-rw-   0        0        0     1544 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/call_op.py
+-rw-rw-rw-   0        0        0      661 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/expressions/cardinality_op.py
+-rw-rw-rw-   0        0        0     4044 2024-03-21 02:47:56.000000 jx_python-4.625.24125/jx_base/expressions/case_op.py
+-rw-rw-rw-   0        0        0     2037 2024-02-27 03:13:49.000000 jx_python-4.625.24125/jx_base/expressions/coalesce_op.py
+-rw-rw-rw-   0        0        0     1593 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/comment_op.py
+-rw-rw-rw-   0        0        0     2890 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/concat_op.py
+-rw-rw-rw-   0        0        0     1592 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/expressions/count_op.py
+-rw-rw-rw-   0        0        0     1250 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/date_op.py
+-rw-rw-rw-   0        0        0     2111 2024-02-27 03:13:49.000000 jx_python-4.625.24125/jx_base/expressions/default_op.py
+-rw-rw-rw-   0        0        0     1179 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/expressions/div_op.py
+-rw-rw-rw-   0        0        0     2757 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_base/expressions/eq_op.py
+-rw-rw-rw-   0        0        0      418 2023-06-17 11:25:18.000000 jx_python-4.625.24125/jx_base/expressions/es_script.py
+-rw-rw-rw-   0        0        0     1525 2024-01-28 16:03:01.000000 jx_python-4.625.24125/jx_base/expressions/es_select_op.py
+-rw-rw-rw-   0        0        0     1270 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/exists_op.py
+-rw-rw-rw-   0        0        0      373 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/expressions/exp_op.py
+-rw-rw-rw-   0        0        0     6265 2024-01-22 13:00:58.000000 jx_python-4.625.24125/jx_base/expressions/expression.py
+-rw-rw-rw-   0        0        0     1524 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/false_op.py
+-rw-rw-rw-   0        0        0     1278 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/filter_op.py
+-rw-rw-rw-   0        0        0     2242 2024-01-28 16:03:01.000000 jx_python-4.625.24125/jx_base/expressions/find_op.py
+-rw-rw-rw-   0        0        0     2413 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/first_op.py
+-rw-rw-rw-   0        0        0      657 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/floor_op.py
+-rw-rw-rw-   0        0        0    10147 2024-02-06 05:15:22.000000 jx_python-4.625.24125/jx_base/expressions/format_op.py
+-rw-rw-rw-   0        0        0     1577 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/from_op.py
+-rw-rw-rw-   0        0        0      807 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/from_unix_op.py
+-rw-rw-rw-   0        0        0     3022 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/get_op.py
+-rw-rw-rw-   0        0        0     1082 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/group_op.py
+-rw-rw-rw-   0        0        0      385 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/gt_op.py
+-rw-rw-rw-   0        0        0      386 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/gte_op.py
+-rw-rw-rw-   0        0        0     3648 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_base/expressions/in_op.py
+-rw-rw-rw-   0        0        0     2505 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/inner_join_op.py
+-rw-rw-rw-   0        0        0     1322 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/is_boolean_op.py
+-rw-rw-rw-   0        0        0      969 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/is_integer_op.py
+-rw-rw-rw-   0        0        0     1360 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/is_number_op.py
+-rw-rw-rw-   0        0        0     1451 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/is_text_op.py
+-rw-rw-rw-   0        0        0     1561 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/last_op.py
+-rw-rw-rw-   0        0        0     1761 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/expressions/least_op.py
+-rw-rw-rw-   0        0        0     1252 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/leaves_op.py
+-rw-rw-rw-   0        0        0     2037 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_base/expressions/left_op.py
+-rw-rw-rw-   0        0        0     1601 2024-02-27 03:13:49.000000 jx_python-4.625.24125/jx_base/expressions/length_op.py
+-rw-rw-rw-   0        0        0     2593 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/limit_op.py
+-rw-rw-rw-   0        0        0     3326 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/expressions/literal.py
+-rw-rw-rw-   0        0        0      384 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/expressions/lt_op.py
+-rw-rw-rw-   0        0        0      385 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/expressions/lte_op.py
+-rw-rw-rw-   0        0        0      507 2023-06-17 11:25:18.000000 jx_python-4.625.24125/jx_base/expressions/map_op.py
+-rw-rw-rw-   0        0        0     1418 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/max_op.py
+-rw-rw-rw-   0        0        0     1442 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/min_op.py
+-rw-rw-rw-   0        0        0     1861 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_base/expressions/missing_op.py
+-rw-rw-rw-   0        0        0      373 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/expressions/mod_op.py
+-rw-rw-rw-   0        0        0      845 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/expressions/most_op.py
+-rw-rw-rw-   0        0        0      882 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/expressions/mul_op.py
+-rw-rw-rw-   0        0        0     1170 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/name_op.py
+-rw-rw-rw-   0        0        0     1647 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_base/expressions/ne_op.py
+-rw-rw-rw-   0        0        0     4366 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_base/expressions/nested_op.py
+-rw-rw-rw-   0        0        0     2061 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_base/expressions/not_left_op.py
+-rw-rw-rw-   0        0        0     1612 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_base/expressions/not_op.py
+-rw-rw-rw-   0        0        0     2150 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_base/expressions/not_right_op.py
+-rw-rw-rw-   0        0        0     2442 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_base/expressions/null_op.py
+-rw-rw-rw-   0        0        0     1059 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/offset_op.py
+-rw-rw-rw-   0        0        0     2239 2024-03-02 22:12:26.000000 jx_python-4.625.24125/jx_base/expressions/or_op.py
+-rw-rw-rw-   0        0        0     2503 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/outer_join_op.py
+-rw-rw-rw-   0        0        0     1387 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/expressions/percentile_op.py
+-rw-rw-rw-   0        0        0     3285 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_base/expressions/prefix_op.py
+-rw-rw-rw-   0        0        0     1585 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/product_op.py
+-rw-rw-rw-   0        0        0      460 2023-06-17 11:25:18.000000 jx_python-4.625.24125/jx_base/expressions/python_function.py
+-rw-rw-rw-   0        0        0     1512 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/python_script.py
+-rw-rw-rw-   0        0        0    24585 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_base/expressions/query_op.py
+-rw-rw-rw-   0        0        0     1025 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/range_op.py
+-rw-rw-rw-   0        0        0     1575 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/reg_exp_op.py
+-rw-rw-rw-   0        0        0     2247 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_base/expressions/right_op.py
+-rw-rw-rw-   0        0        0     1478 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/rows_op.py
+-rw-rw-rw-   0        0        0     1247 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/script_op.py
+-rw-rw-rw-   0        0        0    12251 2024-02-15 03:10:30.000000 jx_python-4.625.24125/jx_base/expressions/select_op.py
+-rw-rw-rw-   0        0        0     1860 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/split_op.py
+-rw-rw-rw-   0        0        0     1295 2024-02-15 03:10:30.000000 jx_python-4.625.24125/jx_base/expressions/sql_alias_op.py
+-rw-rw-rw-   0        0        0     1027 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/expressions/sql_and_op.py
+-rw-rw-rw-   0        0        0     1010 2024-02-27 03:13:49.000000 jx_python-4.625.24125/jx_base/expressions/sql_cast_op.py
+-rw-rw-rw-   0        0        0     1361 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/expressions/sql_concat_op.py
+-rw-rw-rw-   0        0        0     1490 2024-03-10 19:33:03.000000 jx_python-4.625.24125/jx_base/expressions/sql_eq_op.py
+-rw-rw-rw-   0        0        0     1082 2023-06-17 11:25:18.000000 jx_python-4.625.24125/jx_base/expressions/sql_group_by_op.py
+-rw-rw-rw-   0        0        0      423 2024-02-15 03:46:10.000000 jx_python-4.625.24125/jx_base/expressions/sql_gt_op.py
+-rw-rw-rw-   0        0        0      424 2024-02-15 03:46:10.000000 jx_python-4.625.24125/jx_base/expressions/sql_gte_op.py
+-rw-rw-rw-   0        0        0      343 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/expressions/sql_in_op.py
+-rw-rw-rw-   0        0        0      428 2024-01-22 13:00:58.000000 jx_python-4.625.24125/jx_base/expressions/sql_inner_join_op.py
+-rw-rw-rw-   0        0        0     1192 2024-02-27 03:13:49.000000 jx_python-4.625.24125/jx_base/expressions/sql_instr_op.py
+-rw-rw-rw-   0        0        0      832 2024-03-10 19:33:03.000000 jx_python-4.625.24125/jx_base/expressions/sql_is_null_op.py
+-rw-rw-rw-   0        0        0     3313 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/sql_left_joins_op.py
+-rw-rw-rw-   0        0        0      499 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/expressions/sql_limit_op.py
+-rw-rw-rw-   0        0        0      360 2024-02-15 03:10:30.000000 jx_python-4.625.24125/jx_base/expressions/sql_literal.py
+-rw-rw-rw-   0        0        0      423 2024-02-15 03:46:10.000000 jx_python-4.625.24125/jx_base/expressions/sql_lt_op.py
+-rw-rw-rw-   0        0        0      424 2024-02-15 03:46:10.000000 jx_python-4.625.24125/jx_base/expressions/sql_lte_op.py
+-rw-rw-rw-   0        0        0     1449 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_base/expressions/sql_not_op.py
+-rw-rw-rw-   0        0        0     2371 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/expressions/sql_or_op.py
+-rw-rw-rw-   0        0        0      781 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/expressions/sql_order_by_op.py
+-rw-rw-rw-   0        0        0     1057 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/sql_origins_op.py
+-rw-rw-rw-   0        0        0      427 2023-06-17 11:25:18.000000 jx_python-4.625.24125/jx_base/expressions/sql_script.py
+-rw-rw-rw-   0        0        0      958 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/sql_select_all_from_op.py
+-rw-rw-rw-   0        0        0     2012 2024-02-15 03:10:30.000000 jx_python-4.625.24125/jx_base/expressions/sql_select_op.py
+-rw-rw-rw-   0        0        0      911 2024-03-10 19:33:03.000000 jx_python-4.625.24125/jx_base/expressions/sql_substr_op.py
+-rw-rw-rw-   0        0        0     1583 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/expressions/sql_variable.py
+-rw-rw-rw-   0        0        0      396 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_base/expressions/strict_add_op.py
+-rw-rw-rw-   0        0        0     1549 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_base/expressions/strict_boolean_op.py
+-rw-rw-rw-   0        0        0     1112 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_base/expressions/strict_eq_op.py
+-rw-rw-rw-   0        0        0     3378 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_base/expressions/strict_in_op.py
+-rw-rw-rw-   0        0        0     1976 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_base/expressions/strict_index_of_op.py
+-rw-rw-rw-   0        0        0      396 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_base/expressions/strict_mul_op.py
+-rw-rw-rw-   0        0        0     1967 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_base/expressions/strict_multi_op.py
+-rw-rw-rw-   0        0        0     1281 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_base/expressions/strict_not_op.py
+-rw-rw-rw-   0        0        0     1671 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_base/expressions/strict_starts_with_op.py
+-rw-rw-rw-   0        0        0     1335 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_base/expressions/strict_substring_op.py
+-rw-rw-rw-   0        0        0      611 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/sub_op.py
+-rw-rw-rw-   0        0        0     3011 2024-03-02 22:12:26.000000 jx_python-4.625.24125/jx_base/expressions/suffix_op.py
+-rw-rw-rw-   0        0        0     1556 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/expressions/sum_op.py
+-rw-rw-rw-   0        0        0      721 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/expressions/tally_op.py
+-rw-rw-rw-   0        0        0     1594 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/to_array_op.py
+-rw-rw-rw-   0        0        0     1304 2024-03-02 22:12:26.000000 jx_python-4.625.24125/jx_base/expressions/to_boolean_op.py
+-rw-rw-rw-   0        0        0     2708 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/expressions/to_integer_op.py
+-rw-rw-rw-   0        0        0     2874 2024-03-02 22:12:26.000000 jx_python-4.625.24125/jx_base/expressions/to_number_op.py
+-rw-rw-rw-   0        0        0     2043 2024-03-10 19:33:03.000000 jx_python-4.625.24125/jx_base/expressions/to_text_op.py
+-rw-rw-rw-   0        0        0     1170 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/to_value_op.py
+-rw-rw-rw-   0        0        0     1626 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/true_op.py
+-rw-rw-rw-   0        0        0     1678 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/tuple_op.py
+-rw-rw-rw-   0        0        0     2000 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/union_op.py
+-rw-rw-rw-   0        0        0      826 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/expressions/unix_op.py
+-rw-rw-rw-   0        0        0     6148 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_base/expressions/variable.py
+-rw-rw-rw-   0        0        0     3270 2024-03-21 02:47:56.000000 jx_python-4.625.24125/jx_base/expressions/when_op.py
+-rw-rw-rw-   0        0        0    14427 2024-05-04 20:35:42.000000 jx_python-4.625.24125/jx_base/language.py
+-rw-rw-rw-   0        0        0    15169 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_base/meta_columns.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:35:50.364656 jx_python-4.625.24125/jx_base/models/
+-rw-rw-rw-   0        0        0        0 2022-11-12 15:14:28.000000 jx_python-4.625.24125/jx_base/models/__init__.py
+-rw-rw-rw-   0        0        0     2369 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/models/container.py
+-rw-rw-rw-   0        0        0    13016 2023-06-17 11:25:18.000000 jx_python-4.625.24125/jx_base/models/dimensions.py
+-rw-rw-rw-   0        0        0      945 2023-06-17 11:25:18.000000 jx_python-4.625.24125/jx_base/models/facts.py
+-rw-rw-rw-   0        0        0     1656 2023-06-17 11:25:18.000000 jx_python-4.625.24125/jx_base/models/namespace.py
+-rw-rw-rw-   0        0        0      294 2023-06-17 11:25:18.000000 jx_python-4.625.24125/jx_base/models/nested_path.py
+-rw-rw-rw-   0        0        0      408 2023-06-17 11:25:18.000000 jx_python-4.625.24125/jx_base/models/relation.py
+-rw-rw-rw-   0        0        0     5523 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/models/schema.py
+-rw-rw-rw-   0        0        0      833 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/models/snowflake.py
+-rw-rw-rw-   0        0        0      687 2024-03-16 21:27:51.000000 jx_python-4.625.24125/jx_base/models/table.py
+-rw-rw-rw-   0        0        0      791 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_base/queries.py
+-rw-rw-rw-   0        0        0     2520 2024-02-15 03:10:30.000000 jx_python-4.625.24125/jx_base/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:35:50.374262 jx_python-4.625.24125/jx_python/
+-rw-rw-rw-   0        0        0      614 2024-03-16 21:32:01.000000 jx_python-4.625.24125/jx_python/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:35:50.391639 jx_python-4.625.24125/jx_python/containers/
+-rw-rw-rw-   0        0        0        0 2019-09-12 20:44:42.000000 jx_python-4.625.24125/jx_python/containers/__init__.py
+-rw-rw-rw-   0        0        0    16625 2023-06-17 11:25:18.000000 jx_python-4.625.24125/jx_python/containers/cube.py
+-rw-rw-rw-   0        0        0     9580 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_python/containers/list.py
+-rw-rw-rw-   0        0        0     1836 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/convert.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:35:50.392639 jx_python-4.625.24125/jx_python/cubes/
+-rw-rw-rw-   0        0        0        0 2020-01-29 00:24:56.000000 jx_python-4.625.24125/jx_python/cubes/__init__.py
+-rw-rw-rw-   0        0        0     3647 2023-06-17 11:25:18.000000 jx_python-4.625.24125/jx_python/cubes/aggs.py
+-rw-rw-rw-   0        0        0     1920 2024-03-16 21:32:01.000000 jx_python-4.625.24125/jx_python/expression_compiler.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:35:50.459116 jx_python-4.625.24125/jx_python/expressions/
+-rw-rw-rw-   0        0        0     3964 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_python/expressions/__init__.py
+-rw-rw-rw-   0        0        0     4651 2024-04-25 00:55:28.000000 jx_python-4.625.24125/jx_python/expressions/_utils.py
+-rw-rw-rw-   0        0        0      440 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/add_op.py
+-rw-rw-rw-   0        0        0      945 2024-02-27 03:13:49.000000 jx_python-4.625.24125/jx_python/expressions/and_op.py
+-rw-rw-rw-   0        0        0      857 2024-03-16 21:32:01.000000 jx_python-4.625.24125/jx_python/expressions/array_of_op.py
+-rw-rw-rw-   0        0        0      714 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/avg_op.py
+-rw-rw-rw-   0        0        0      372 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/between_op.py
+-rw-rw-rw-   0        0        0     1285 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/call_op.py
+-rw-rw-rw-   0        0        0      673 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/cardinality_op.py
+-rw-rw-rw-   0        0        0      716 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/case_op.py
+-rw-rw-rw-   0        0        0      976 2024-01-21 21:27:17.000000 jx_python-4.625.24125/jx_python/expressions/coalesce_op.py
+-rw-rw-rw-   0        0        0     1146 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/concat_op.py
+-rw-rw-rw-   0        0        0      786 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/count_op.py
+-rw-rw-rw-   0        0        0      554 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/date_op.py
+-rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/div_op.py
+-rw-rw-rw-   0        0        0     1608 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_python/expressions/eq_op.py
+-rw-rw-rw-   0        0        0      750 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/exists_op.py
+-rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/exp_op.py
+-rw-rw-rw-   0        0        0      635 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/false_op.py
+-rw-rw-rw-   0        0        0     1110 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/filter_op.py
+-rw-rw-rw-   0        0        0     1692 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_python/expressions/find_op.py
+-rw-rw-rw-   0        0        0      962 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/first_op.py
+-rw-rw-rw-   0        0        0      647 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/floor_op.py
+-rw-rw-rw-   0        0        0      368 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/format_op.py
+-rw-rw-rw-   0        0        0     1823 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/get_op.py
+-rw-rw-rw-   0        0        0     1718 2024-04-24 23:41:46.000000 jx_python-4.625.24125/jx_python/expressions/group_op.py
+-rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/gt_op.py
+-rw-rw-rw-   0        0        0      448 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/gte_op.py
+-rw-rw-rw-   0        0        0      831 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/in_op.py
+-rw-rw-rw-   0        0        0      787 2024-03-16 21:32:01.000000 jx_python-4.625.24125/jx_python/expressions/is_text_op.py
+-rw-rw-rw-   0        0        0     1109 2024-03-16 21:32:01.000000 jx_python-4.625.24125/jx_python/expressions/last_op.py
+-rw-rw-rw-   0        0        0     1026 2024-02-27 03:13:49.000000 jx_python-4.625.24125/jx_python/expressions/least_op.py
+-rw-rw-rw-   0        0        0      559 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/leaves_op.py
+-rw-rw-rw-   0        0        0      692 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/length_op.py
+-rw-rw-rw-   0        0        0      953 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/limit_op.py
+-rw-rw-rw-   0        0        0      618 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/literal.py
+-rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/lt_op.py
+-rw-rw-rw-   0        0        0      448 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/lte_op.py
+-rw-rw-rw-   0        0        0      694 2024-03-16 21:32:01.000000 jx_python-4.625.24125/jx_python/expressions/max_op.py
+-rw-rw-rw-   0        0        0      694 2024-03-16 21:32:01.000000 jx_python-4.625.24125/jx_python/expressions/min_op.py
+-rw-rw-rw-   0        0        0     1045 2024-03-16 21:32:01.000000 jx_python-4.625.24125/jx_python/expressions/missing_op.py
+-rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/mod_op.py
+-rw-rw-rw-   0        0        0      981 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/most_op.py
+-rw-rw-rw-   0        0        0      533 2024-03-16 21:32:01.000000 jx_python-4.625.24125/jx_python/expressions/mul_op.py
+-rw-rw-rw-   0        0        0      992 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/name_op.py
+-rw-rw-rw-   0        0        0      733 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/ne_op.py
+-rw-rw-rw-   0        0        0      773 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/not_left_op.py
+-rw-rw-rw-   0        0        0      680 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/not_op.py
+-rw-rw-rw-   0        0        0      999 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/not_right_op.py
+-rw-rw-rw-   0        0        0      556 2024-03-16 21:32:01.000000 jx_python-4.625.24125/jx_python/expressions/offset_op.py
+-rw-rw-rw-   0        0        0      930 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/or_op.py
+-rw-rw-rw-   0        0        0      468 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/percentile_op.py
+-rw-rw-rw-   0        0        0      651 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/prefix_op.py
+-rw-rw-rw-   0        0        0     1303 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/product_op.py
+-rw-rw-rw-   0        0        0     1139 2024-03-16 21:32:01.000000 jx_python-4.625.24125/jx_python/expressions/python_function.py
+-rw-rw-rw-   0        0        0     1443 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/python_script.py
+-rw-rw-rw-   0        0        0      364 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/range_op.py
+-rw-rw-rw-   0        0        0      946 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/reg_exp_op.py
+-rw-rw-rw-   0        0        0      699 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/right_op.py
+-rw-rw-rw-   0        0        0     1022 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/rows_op.py
+-rw-rw-rw-   0        0        0      594 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/script_op.py
+-rw-rw-rw-   0        0        0     2105 2024-03-16 21:32:01.000000 jx_python-4.625.24125/jx_python/expressions/select_op.py
+-rw-rw-rw-   0        0        0      643 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/split_op.py
+-rw-rw-rw-   0        0        0      888 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_python/expressions/strict_add_op.py
+-rw-rw-rw-   0        0        0      850 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_python/expressions/strict_eq_op.py
+-rw-rw-rw-   0        0        0      870 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_python/expressions/strict_index_of_op.py
+-rw-rw-rw-   0        0        0      912 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_python/expressions/strict_starts_with_op.py
+-rw-rw-rw-   0        0        0      998 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_python/expressions/strict_substring_op.py
+-rw-rw-rw-   0        0        0      444 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/sub_op.py
+-rw-rw-rw-   0        0        0      742 2024-02-27 03:13:49.000000 jx_python-4.625.24125/jx_python/expressions/suffix_op.py
+-rw-rw-rw-   0        0        0     1252 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/sum_op.py
+-rw-rw-rw-   0        0        0     1056 2024-03-16 21:32:01.000000 jx_python-4.625.24125/jx_python/expressions/tally_op.py
+-rw-rw-rw-   0        0        0      835 2024-03-16 21:32:01.000000 jx_python-4.625.24125/jx_python/expressions/to_array_op.py
+-rw-rw-rw-   0        0        0      962 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/to_boolean_op.py
+-rw-rw-rw-   0        0        0      606 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/to_integer_op.py
+-rw-rw-rw-   0        0        0     1034 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/to_number_op.py
+-rw-rw-rw-   0        0        0      800 2024-03-16 21:32:01.000000 jx_python-4.625.24125/jx_python/expressions/to_text_op.py
+-rw-rw-rw-   0        0        0      957 2024-03-16 21:32:01.000000 jx_python-4.625.24125/jx_python/expressions/to_value_op.py
+-rw-rw-rw-   0        0        0      628 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/true_op.py
+-rw-rw-rw-   0        0        0      812 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/tuple_op.py
+-rw-rw-rw-   0        0        0     1328 2024-03-16 21:32:01.000000 jx_python-4.625.24125/jx_python/expressions/variable.py
+-rw-rw-rw-   0        0        0      968 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/expressions/when_op.py
+-rw-rw-rw-   0        0        0     4434 2023-06-17 11:25:18.000000 jx_python-4.625.24125/jx_python/flat_list.py
+-rw-rw-rw-   0        0        0     4408 2024-05-04 20:35:42.000000 jx_python-4.625.24125/jx_python/group_by.py
+-rw-rw-rw-   0        0        0    34076 2024-01-25 04:46:12.000000 jx_python-4.625.24125/jx_python/jx.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:35:50.460138 jx_python-4.625.24125/jx_python/lists/
+-rw-rw-rw-   0        0        0        0 2019-09-12 20:44:42.000000 jx_python-4.625.24125/jx_python/lists/__init__.py
+-rw-rw-rw-   0        0        0     5009 2024-04-04 04:16:05.000000 jx_python-4.625.24125/jx_python/lists/aggs.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:35:50.462179 jx_python-4.625.24125/jx_python/namespace/
+-rw-rw-rw-   0        0        0        0 2019-09-12 20:44:42.000000 jx_python-4.625.24125/jx_python/namespace/__init__.py
+-rw-rw-rw-   0        0        0     8745 2024-01-20 18:36:41.000000 jx_python-4.625.24125/jx_python/namespace/normal.py
+-rw-rw-rw-   0        0        0      768 2023-06-17 11:25:18.000000 jx_python-4.625.24125/jx_python/records.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:35:50.466723 jx_python-4.625.24125/jx_python/streams/
+-rw-rw-rw-   0        0        0     4178 2024-03-16 21:32:01.000000 jx_python-4.625.24125/jx_python/streams/__init__.py
+-rw-rw-rw-   0        0        0     1926 2023-06-17 11:25:18.000000 jx_python-4.625.24125/jx_python/streams/expression_compiler.py
+-rw-rw-rw-   0        0        0     4531 2024-04-24 23:41:46.000000 jx_python-4.625.24125/jx_python/streams/expression_factory.py
+-rw-rw-rw-   0        0        0      713 2023-06-17 11:25:18.000000 jx_python-4.625.24125/jx_python/streams/inspects.py
+-rw-rw-rw-   0        0        0      807 2023-06-17 11:25:18.000000 jx_python-4.625.24125/jx_python/streams/type_parser.py
+-rw-rw-rw-   0        0        0     5515 2023-06-17 11:25:18.000000 jx_python-4.625.24125/jx_python/streams/typers.py
+-rw-rw-rw-   0        0        0     1622 2024-03-16 21:32:01.000000 jx_python-4.625.24125/jx_python/streams.py
+-rw-rw-rw-   0        0        0      564 2023-06-17 11:25:18.000000 jx_python-4.625.24125/jx_python/table.py
+-rw-rw-rw-   0        0        0     1431 2023-06-17 11:25:18.000000 jx_python-4.625.24125/jx_python/utils.py
+-rw-rw-rw-   0        0        0     7410 2023-06-17 11:25:18.000000 jx_python-4.625.24125/jx_python/windows.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:35:50.467953 jx_python-4.625.24125/jx_python.egg-info/
+-rw-rw-rw-   0        0        0     1744 2024-05-04 20:35:50.000000 jx_python-4.625.24125/jx_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8849 2024-05-04 20:35:50.000000 jx_python-4.625.24125/jx_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 20:35:50.000000 jx_python-4.625.24125/jx_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      266 2024-05-04 20:35:50.000000 jx_python-4.625.24125/jx_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-04 20:35:50.000000 jx_python-4.625.24125/jx_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 20:35:50.470042 jx_python-4.625.24125/setup.cfg
+-rw-rw-rw-   0        0        0     1873 2024-05-04 20:35:45.000000 jx_python-4.625.24125/setup.py
```

### Comparing `jx_python-4.607.24116/LICENSE` & `jx_python-4.625.24125/LICENSE`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/PKG-INFO` & `jx_python-4.625.24125/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jx-python
-Version: 4.607.24116
+Version: 4.625.24125
 Summary: JSON query expressions using Python
 Home-page: https://github.com/klahnakoski/jx-python
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
@@ -12,24 +12,24 @@
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-collections==5.606.24115
-Requires-Dist: mo-dots==9.606.24115
+Requires-Dist: mo-collections==5.623.24125
+Requires-Dist: mo-dots==10.623.24125
 Requires-Dist: mo-future==7.584.24095
-Requires-Dist: mo-json==6.606.24115
-Requires-Dist: mo-json-config==4.606.24115
-Requires-Dist: mo-kwargs==7.606.24115
-Requires-Dist: mo-logs==8.606.24115
-Requires-Dist: mo-math==7.606.24115
-Requires-Dist: mo-threads==6.606.24115
-Requires-Dist: mo-times==5.606.24115
+Requires-Dist: mo-json==6.624.24125
+Requires-Dist: mo-json-config==4.624.24125
+Requires-Dist: mo-kwargs==7.623.24125
+Requires-Dist: mo-logs==8.623.24125
+Requires-Dist: mo-math==7.623.24125
+Requires-Dist: mo-threads==6.624.24125
+Requires-Dist: mo-times==5.623.24125
 Provides-Extra: tests
 Requires-Dist: mo-testing>=8.591.24112; extra == "tests"
 
 # jx-python
 
 Python library for JSON Expressions
```

### Comparing `jx_python-4.607.24116/jx_base/__init__.py` & `jx_python-4.625.24125/jx_base/__init__.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/data_class.py` & `jx_python-4.625.24125/jx_base/data_class.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/domains.py` & `jx_python-4.625.24125/jx_base/domains.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/__init__.py` & `jx_python-4.625.24125/jx_base/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/_utils.py` & `jx_python-4.625.24125/jx_base/expressions/_utils.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/abs_op.py` & `jx_python-4.625.24125/jx_base/expressions/abs_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/add_op.py` & `jx_python-4.625.24125/jx_base/expressions/add_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/aggregate_op.py` & `jx_python-4.625.24125/jx_base/expressions/aggregate_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/all_op.py` & `jx_python-4.625.24125/jx_base/expressions/all_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/and_op.py` & `jx_python-4.625.24125/jx_base/expressions/and_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/any_op.py` & `jx_python-4.625.24125/jx_base/expressions/any_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/array_of_op.py` & `jx_python-4.625.24125/jx_base/expressions/array_of_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/base_binary_op.py` & `jx_python-4.625.24125/jx_base/expressions/base_binary_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/base_inequality_op.py` & `jx_python-4.625.24125/jx_base/expressions/base_inequality_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/base_multi_op.py` & `jx_python-4.625.24125/jx_base/expressions/base_multi_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/between_op.py` & `jx_python-4.625.24125/jx_base/expressions/between_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/call_op.py` & `jx_python-4.625.24125/jx_base/expressions/call_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/cardinality_op.py` & `jx_python-4.625.24125/jx_base/expressions/cardinality_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/case_op.py` & `jx_python-4.625.24125/jx_base/expressions/case_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/coalesce_op.py` & `jx_python-4.625.24125/jx_base/expressions/coalesce_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/comment_op.py` & `jx_python-4.625.24125/jx_base/expressions/comment_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/concat_op.py` & `jx_python-4.625.24125/jx_base/expressions/concat_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/count_op.py` & `jx_python-4.625.24125/jx_base/expressions/count_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/date_op.py` & `jx_python-4.625.24125/jx_base/expressions/date_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/default_op.py` & `jx_python-4.625.24125/jx_base/expressions/default_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/div_op.py` & `jx_python-4.625.24125/jx_base/expressions/div_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/eq_op.py` & `jx_python-4.625.24125/jx_base/expressions/eq_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/es_select_op.py` & `jx_python-4.625.24125/jx_base/expressions/es_select_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/exists_op.py` & `jx_python-4.625.24125/jx_base/expressions/exists_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/expression.py` & `jx_python-4.625.24125/jx_base/expressions/expression.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/false_op.py` & `jx_python-4.625.24125/jx_base/expressions/false_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/filter_op.py` & `jx_python-4.625.24125/jx_base/expressions/filter_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/find_op.py` & `jx_python-4.625.24125/jx_base/expressions/find_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/first_op.py` & `jx_python-4.625.24125/jx_base/expressions/first_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/floor_op.py` & `jx_python-4.625.24125/jx_base/expressions/floor_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/format_op.py` & `jx_python-4.625.24125/jx_base/expressions/format_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/from_op.py` & `jx_python-4.625.24125/jx_base/expressions/from_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/from_unix_op.py` & `jx_python-4.625.24125/jx_base/expressions/from_unix_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/get_op.py` & `jx_python-4.625.24125/jx_base/expressions/get_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/group_op.py` & `jx_python-4.625.24125/jx_base/expressions/group_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/in_op.py` & `jx_python-4.625.24125/jx_base/expressions/in_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/inner_join_op.py` & `jx_python-4.625.24125/jx_base/expressions/inner_join_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/is_boolean_op.py` & `jx_python-4.625.24125/jx_base/expressions/is_boolean_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/is_integer_op.py` & `jx_python-4.625.24125/jx_base/expressions/is_integer_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/is_number_op.py` & `jx_python-4.625.24125/jx_base/expressions/is_number_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/is_text_op.py` & `jx_python-4.625.24125/jx_base/expressions/is_text_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/last_op.py` & `jx_python-4.625.24125/jx_base/expressions/last_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/least_op.py` & `jx_python-4.625.24125/jx_base/expressions/least_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/leaves_op.py` & `jx_python-4.625.24125/jx_base/expressions/leaves_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/left_op.py` & `jx_python-4.625.24125/jx_base/expressions/left_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/length_op.py` & `jx_python-4.625.24125/jx_base/expressions/length_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/limit_op.py` & `jx_python-4.625.24125/jx_base/expressions/limit_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/literal.py` & `jx_python-4.625.24125/jx_base/expressions/literal.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/max_op.py` & `jx_python-4.625.24125/jx_base/expressions/max_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/min_op.py` & `jx_python-4.625.24125/jx_base/expressions/min_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/missing_op.py` & `jx_python-4.625.24125/jx_base/expressions/missing_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/most_op.py` & `jx_python-4.625.24125/jx_base/expressions/most_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/mul_op.py` & `jx_python-4.625.24125/jx_base/expressions/mul_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/name_op.py` & `jx_python-4.625.24125/jx_base/expressions/name_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/ne_op.py` & `jx_python-4.625.24125/jx_base/expressions/ne_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/nested_op.py` & `jx_python-4.625.24125/jx_base/expressions/nested_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/not_left_op.py` & `jx_python-4.625.24125/jx_base/expressions/not_left_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/not_op.py` & `jx_python-4.625.24125/jx_base/expressions/not_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/not_right_op.py` & `jx_python-4.625.24125/jx_base/expressions/not_right_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/null_op.py` & `jx_python-4.625.24125/jx_base/expressions/null_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/offset_op.py` & `jx_python-4.625.24125/jx_base/expressions/offset_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/or_op.py` & `jx_python-4.625.24125/jx_base/expressions/or_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/outer_join_op.py` & `jx_python-4.625.24125/jx_base/expressions/outer_join_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/percentile_op.py` & `jx_python-4.625.24125/jx_base/expressions/percentile_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/prefix_op.py` & `jx_python-4.625.24125/jx_base/expressions/prefix_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/product_op.py` & `jx_python-4.625.24125/jx_base/expressions/product_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/python_script.py` & `jx_python-4.625.24125/jx_base/expressions/python_script.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/query_op.py` & `jx_python-4.625.24125/jx_base/expressions/query_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/range_op.py` & `jx_python-4.625.24125/jx_base/expressions/range_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/reg_exp_op.py` & `jx_python-4.625.24125/jx_base/expressions/reg_exp_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/right_op.py` & `jx_python-4.625.24125/jx_base/expressions/right_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/rows_op.py` & `jx_python-4.625.24125/jx_base/expressions/rows_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/script_op.py` & `jx_python-4.625.24125/jx_base/expressions/script_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/select_op.py` & `jx_python-4.625.24125/jx_base/expressions/select_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/split_op.py` & `jx_python-4.625.24125/jx_base/expressions/split_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/sql_alias_op.py` & `jx_python-4.625.24125/jx_base/expressions/sql_alias_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/sql_and_op.py` & `jx_python-4.625.24125/jx_base/expressions/sql_and_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/sql_cast_op.py` & `jx_python-4.625.24125/jx_base/expressions/sql_cast_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/sql_concat_op.py` & `jx_python-4.625.24125/jx_base/expressions/sql_concat_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/sql_eq_op.py` & `jx_python-4.625.24125/jx_base/expressions/sql_eq_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/sql_group_by_op.py` & `jx_python-4.625.24125/jx_base/expressions/sql_group_by_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/sql_instr_op.py` & `jx_python-4.625.24125/jx_base/expressions/sql_instr_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/sql_is_null_op.py` & `jx_python-4.625.24125/jx_base/expressions/sql_is_null_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/sql_left_joins_op.py` & `jx_python-4.625.24125/jx_base/expressions/sql_left_joins_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/sql_not_op.py` & `jx_python-4.625.24125/jx_base/expressions/sql_not_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/sql_or_op.py` & `jx_python-4.625.24125/jx_base/expressions/sql_or_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/sql_order_by_op.py` & `jx_python-4.625.24125/jx_base/expressions/sql_order_by_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/sql_origins_op.py` & `jx_python-4.625.24125/jx_base/expressions/sql_origins_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/sql_select_all_from_op.py` & `jx_python-4.625.24125/jx_base/expressions/sql_select_all_from_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/sql_select_op.py` & `jx_python-4.625.24125/jx_base/expressions/sql_select_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/sql_substr_op.py` & `jx_python-4.625.24125/jx_base/expressions/sql_substr_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/sql_variable.py` & `jx_python-4.625.24125/jx_base/expressions/sql_variable.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/strict_boolean_op.py` & `jx_python-4.625.24125/jx_base/expressions/strict_boolean_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/strict_eq_op.py` & `jx_python-4.625.24125/jx_base/expressions/strict_eq_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/strict_in_op.py` & `jx_python-4.625.24125/jx_base/expressions/strict_in_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/strict_index_of_op.py` & `jx_python-4.625.24125/jx_base/expressions/strict_index_of_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/strict_multi_op.py` & `jx_python-4.625.24125/jx_base/expressions/strict_multi_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/strict_not_op.py` & `jx_python-4.625.24125/jx_base/expressions/strict_not_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/strict_starts_with_op.py` & `jx_python-4.625.24125/jx_base/expressions/strict_starts_with_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/strict_substring_op.py` & `jx_python-4.625.24125/jx_base/expressions/strict_substring_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/sub_op.py` & `jx_python-4.625.24125/jx_base/expressions/sub_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/suffix_op.py` & `jx_python-4.625.24125/jx_base/expressions/suffix_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/sum_op.py` & `jx_python-4.625.24125/jx_base/expressions/sum_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/tally_op.py` & `jx_python-4.625.24125/jx_base/expressions/tally_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/to_array_op.py` & `jx_python-4.625.24125/jx_base/expressions/to_array_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/to_boolean_op.py` & `jx_python-4.625.24125/jx_base/expressions/to_boolean_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/to_integer_op.py` & `jx_python-4.625.24125/jx_base/expressions/to_integer_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/to_number_op.py` & `jx_python-4.625.24125/jx_base/expressions/to_number_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/to_text_op.py` & `jx_python-4.625.24125/jx_base/expressions/to_text_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/to_value_op.py` & `jx_python-4.625.24125/jx_base/expressions/to_value_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/true_op.py` & `jx_python-4.625.24125/jx_base/expressions/true_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/tuple_op.py` & `jx_python-4.625.24125/jx_base/expressions/tuple_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/union_op.py` & `jx_python-4.625.24125/jx_base/expressions/union_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/unix_op.py` & `jx_python-4.625.24125/jx_base/expressions/unix_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/variable.py` & `jx_python-4.625.24125/jx_base/expressions/variable.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/expressions/when_op.py` & `jx_python-4.625.24125/jx_base/expressions/when_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/language.py` & `jx_python-4.625.24125/jx_base/language.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 
 from collections import deque
 from copy import copy
 from datetime import datetime
 from decimal import Decimal
 from math import isnan
 
-import mo_dots
-from mo_dots import Data, startswith_field, null_types, is_data, datas
-from mo_dots.lists import list_types, is_many
+from mo_dots import Data, startswith_field, null_types, datas, is_many, is_list
 from mo_times import Date
 
 from jx_base.utils import enlist
 from mo_future import (
     boolean_type,
     long,
     none_type,
@@ -325,15 +323,15 @@
     if left is right:
         return 0
 
     try:
         ltype = left.__class__
         rtype = right.__class__
 
-        if ltype in list_types or rtype in list_types:
+        if is_list(ltype) or is_list(rtype):
             if left == None:
                 return ordering
             elif right == None:
                 return -ordering
 
             left = enlist(left)
             right = enlist(right)
```

### Comparing `jx_python-4.607.24116/jx_base/meta_columns.py` & `jx_python-4.625.24125/jx_base/meta_columns.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/models/container.py` & `jx_python-4.625.24125/jx_base/models/container.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/models/dimensions.py` & `jx_python-4.625.24125/jx_base/models/dimensions.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/models/facts.py` & `jx_python-4.625.24125/jx_base/models/facts.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/models/namespace.py` & `jx_python-4.625.24125/jx_base/models/namespace.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/models/schema.py` & `jx_python-4.625.24125/jx_base/models/schema.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/models/snowflake.py` & `jx_python-4.625.24125/jx_base/models/snowflake.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/models/table.py` & `jx_python-4.625.24125/jx_base/models/table.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/queries.py` & `jx_python-4.625.24125/jx_base/queries.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_base/utils.py` & `jx_python-4.625.24125/jx_base/utils.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/__init__.py` & `jx_python-4.625.24125/jx_python/__init__.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/containers/cube.py` & `jx_python-4.625.24125/jx_python/containers/cube.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/containers/list.py` & `jx_python-4.625.24125/jx_python/containers/list.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/convert.py` & `jx_python-4.625.24125/jx_python/convert.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/cubes/aggs.py` & `jx_python-4.625.24125/jx_python/cubes/aggs.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expression_compiler.py` & `jx_python-4.625.24125/jx_python/expression_compiler.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/__init__.py` & `jx_python-4.625.24125/jx_python/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/_utils.py` & `jx_python-4.625.24125/jx_python/expressions/_utils.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/and_op.py` & `jx_python-4.625.24125/jx_python/expressions/and_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/array_of_op.py` & `jx_python-4.625.24125/jx_python/expressions/array_of_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/avg_op.py` & `jx_python-4.625.24125/jx_python/expressions/avg_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/call_op.py` & `jx_python-4.625.24125/jx_python/expressions/call_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/cardinality_op.py` & `jx_python-4.625.24125/jx_python/expressions/cardinality_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/case_op.py` & `jx_python-4.625.24125/jx_python/expressions/case_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/coalesce_op.py` & `jx_python-4.625.24125/jx_python/expressions/coalesce_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/concat_op.py` & `jx_python-4.625.24125/jx_python/expressions/concat_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/count_op.py` & `jx_python-4.625.24125/jx_python/expressions/count_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/date_op.py` & `jx_python-4.625.24125/jx_python/expressions/date_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/eq_op.py` & `jx_python-4.625.24125/jx_python/expressions/eq_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/exists_op.py` & `jx_python-4.625.24125/jx_python/expressions/exists_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/false_op.py` & `jx_python-4.625.24125/jx_python/expressions/false_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/filter_op.py` & `jx_python-4.625.24125/jx_python/expressions/filter_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/find_op.py` & `jx_python-4.625.24125/jx_python/expressions/find_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/first_op.py` & `jx_python-4.625.24125/jx_python/expressions/first_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/floor_op.py` & `jx_python-4.625.24125/jx_python/expressions/floor_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/get_op.py` & `jx_python-4.625.24125/jx_python/expressions/get_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/group_op.py` & `jx_python-4.625.24125/jx_python/expressions/group_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/in_op.py` & `jx_python-4.625.24125/jx_python/expressions/in_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/is_text_op.py` & `jx_python-4.625.24125/jx_python/expressions/is_text_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/last_op.py` & `jx_python-4.625.24125/jx_python/expressions/last_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/least_op.py` & `jx_python-4.625.24125/jx_python/expressions/least_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/leaves_op.py` & `jx_python-4.625.24125/jx_python/expressions/leaves_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/length_op.py` & `jx_python-4.625.24125/jx_python/expressions/length_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/limit_op.py` & `jx_python-4.625.24125/jx_python/expressions/limit_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/literal.py` & `jx_python-4.625.24125/jx_python/expressions/literal.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/max_op.py` & `jx_python-4.625.24125/jx_python/expressions/max_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/min_op.py` & `jx_python-4.625.24125/jx_python/expressions/min_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/missing_op.py` & `jx_python-4.625.24125/jx_python/expressions/missing_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/most_op.py` & `jx_python-4.625.24125/jx_python/expressions/most_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/mul_op.py` & `jx_python-4.625.24125/jx_python/expressions/mul_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/name_op.py` & `jx_python-4.625.24125/jx_python/expressions/name_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/ne_op.py` & `jx_python-4.625.24125/jx_python/expressions/ne_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/not_left_op.py` & `jx_python-4.625.24125/jx_python/expressions/not_left_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/not_op.py` & `jx_python-4.625.24125/jx_python/expressions/not_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/not_right_op.py` & `jx_python-4.625.24125/jx_python/expressions/not_right_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/offset_op.py` & `jx_python-4.625.24125/jx_python/expressions/offset_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/or_op.py` & `jx_python-4.625.24125/jx_python/expressions/or_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/prefix_op.py` & `jx_python-4.625.24125/jx_python/expressions/prefix_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/product_op.py` & `jx_python-4.625.24125/jx_python/expressions/product_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/python_function.py` & `jx_python-4.625.24125/jx_python/expressions/python_function.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/python_script.py` & `jx_python-4.625.24125/jx_python/expressions/python_script.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/reg_exp_op.py` & `jx_python-4.625.24125/jx_python/expressions/reg_exp_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/right_op.py` & `jx_python-4.625.24125/jx_python/expressions/right_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/rows_op.py` & `jx_python-4.625.24125/jx_python/expressions/rows_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/script_op.py` & `jx_python-4.625.24125/jx_python/expressions/script_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/select_op.py` & `jx_python-4.625.24125/jx_python/expressions/select_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/split_op.py` & `jx_python-4.625.24125/jx_python/expressions/split_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/strict_add_op.py` & `jx_python-4.625.24125/jx_python/expressions/strict_add_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/strict_eq_op.py` & `jx_python-4.625.24125/jx_python/expressions/strict_eq_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/strict_index_of_op.py` & `jx_python-4.625.24125/jx_python/expressions/strict_index_of_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/strict_starts_with_op.py` & `jx_python-4.625.24125/jx_python/expressions/strict_starts_with_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/strict_substring_op.py` & `jx_python-4.625.24125/jx_python/expressions/strict_substring_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/suffix_op.py` & `jx_python-4.625.24125/jx_python/expressions/suffix_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/sum_op.py` & `jx_python-4.625.24125/jx_python/expressions/sum_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/tally_op.py` & `jx_python-4.625.24125/jx_python/expressions/tally_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/to_array_op.py` & `jx_python-4.625.24125/jx_python/expressions/to_array_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/to_boolean_op.py` & `jx_python-4.625.24125/jx_python/expressions/to_boolean_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/to_integer_op.py` & `jx_python-4.625.24125/jx_python/expressions/to_integer_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/to_number_op.py` & `jx_python-4.625.24125/jx_python/expressions/to_number_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/to_text_op.py` & `jx_python-4.625.24125/jx_python/expressions/to_text_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/to_value_op.py` & `jx_python-4.625.24125/jx_python/expressions/to_value_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/true_op.py` & `jx_python-4.625.24125/jx_python/expressions/true_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/tuple_op.py` & `jx_python-4.625.24125/jx_python/expressions/tuple_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/variable.py` & `jx_python-4.625.24125/jx_python/expressions/variable.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/expressions/when_op.py` & `jx_python-4.625.24125/jx_python/expressions/when_op.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/flat_list.py` & `jx_python-4.625.24125/jx_python/flat_list.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/group_by.py` & `jx_python-4.625.24125/jx_python/group_by.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 
 
 import math
 
-from mo_dots import FlatList, Null, dict_to_data
-from mo_dots.lists import list_types
+from mo_dots import FlatList, Null, dict_to_data, is_list
 from mo_future import binary_type, text
 from mo_logs import Log
 from mo_logs.exceptions import Except
 
 from jx_base.expressions import jx_expression
 from jx_base.language import is_expression
 from jx_base.models.container import Container
@@ -114,15 +113,15 @@
         yield (i, g)
 
 
 def chunk(data, size=0):
     if not size:
         return [data]
 
-    if data.__class__ in list_types + (tuple, bytearray, text, binary_type):
+    if is_list(data) or isinstance(data, (bytearray, text, binary_type)):
         # USE SLICING
         def _iter():
             num = int(math.ceil(len(data) / size))
             for i in range(num):
                 output = (i, data[i * size : i * size + size :])
                 yield output
```

### Comparing `jx_python-4.607.24116/jx_python/jx.py` & `jx_python-4.625.24125/jx_python/jx.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/lists/aggs.py` & `jx_python-4.625.24125/jx_python/lists/aggs.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/namespace/normal.py` & `jx_python-4.625.24125/jx_python/namespace/normal.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/records.py` & `jx_python-4.625.24125/jx_python/records.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/streams/__init__.py` & `jx_python-4.625.24125/jx_python/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/streams/expression_compiler.py` & `jx_python-4.625.24125/jx_python/streams/expression_compiler.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/streams/expression_factory.py` & `jx_python-4.625.24125/jx_python/streams/expression_factory.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/streams/inspects.py` & `jx_python-4.625.24125/jx_python/streams/inspects.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/streams/type_parser.py` & `jx_python-4.625.24125/jx_python/streams/type_parser.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/streams/typers.py` & `jx_python-4.625.24125/jx_python/streams/typers.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/streams.py` & `jx_python-4.625.24125/jx_python/streams.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/table.py` & `jx_python-4.625.24125/jx_python/table.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/utils.py` & `jx_python-4.625.24125/jx_python/utils.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python/windows.py` & `jx_python-4.625.24125/jx_python/windows.py`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/jx_python.egg-info/PKG-INFO` & `jx_python-4.625.24125/jx_python.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jx-python
-Version: 4.607.24116
+Version: 4.625.24125
 Summary: JSON query expressions using Python
 Home-page: https://github.com/klahnakoski/jx-python
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
@@ -12,24 +12,24 @@
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-collections==5.606.24115
-Requires-Dist: mo-dots==9.606.24115
+Requires-Dist: mo-collections==5.623.24125
+Requires-Dist: mo-dots==10.623.24125
 Requires-Dist: mo-future==7.584.24095
-Requires-Dist: mo-json==6.606.24115
-Requires-Dist: mo-json-config==4.606.24115
-Requires-Dist: mo-kwargs==7.606.24115
-Requires-Dist: mo-logs==8.606.24115
-Requires-Dist: mo-math==7.606.24115
-Requires-Dist: mo-threads==6.606.24115
-Requires-Dist: mo-times==5.606.24115
+Requires-Dist: mo-json==6.624.24125
+Requires-Dist: mo-json-config==4.624.24125
+Requires-Dist: mo-kwargs==7.623.24125
+Requires-Dist: mo-logs==8.623.24125
+Requires-Dist: mo-math==7.623.24125
+Requires-Dist: mo-threads==6.624.24125
+Requires-Dist: mo-times==5.623.24125
 Provides-Extra: tests
 Requires-Dist: mo-testing>=8.591.24112; extra == "tests"
 
 # jx-python
 
 Python library for JSON Expressions
```

### Comparing `jx_python-4.607.24116/jx_python.egg-info/SOURCES.txt` & `jx_python-4.625.24125/jx_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jx_python-4.607.24116/setup.py` & `jx_python-4.625.24125/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 setup(
     author='Kyle Lahnakoski',
     author_email='kyle@lahnakoski.com',
     classifiers=["Development Status :: 4 - Beta","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules","License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)","Programming Language :: Python :: 3.8","Programming Language :: Python :: 3.9","Programming Language :: Python :: 3.11","Programming Language :: Python :: 3.12"],
     description='JSON query expressions using Python',
     extras_require={"tests":["mo-testing>=8.591.24112"]},
     include_package_data=True,
-    install_requires=["mo-collections==5.606.24115","mo-dots==9.606.24115","mo-future==7.584.24095","mo-json==6.606.24115","mo-json-config==4.606.24115","mo-kwargs==7.606.24115","mo-logs==8.606.24115","mo-math==7.606.24115","mo-threads==6.606.24115","mo-times==5.606.24115"],
+    install_requires=["mo-collections==5.623.24125","mo-dots==10.623.24125","mo-future==7.584.24095","mo-json==6.624.24125","mo-json-config==4.624.24125","mo-kwargs==7.623.24125","mo-logs==8.623.24125","mo-math==7.623.24125","mo-threads==6.624.24125","mo-times==5.623.24125"],
     license='MPL 2.0',
     long_description='# jx-python\n\nPython library for JSON Expressions \n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/jx-python.svg)](https://pypi.org/project/jx-python/)\n[![Build Status](https://github.com/klahnakoski/jx-python/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/jx-python/actions/workflows/build.yml)\n[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/jx-python/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/jx-python?branch=dev)\n',
     long_description_content_type='text/markdown',
     name='jx-python',
     packages=["jx_base","jx_base.expressions","jx_base.models","jx_python.expressions","jx_python.containers","jx_python.cubes","jx_python.lists","jx_python.namespace","jx_python","jx_python.streams"],
     url='https://github.com/klahnakoski/jx-python',
-    version='4.607.24116'
+    version='4.625.24125'
 )
```

