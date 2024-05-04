# Comparing `tmp/jx_sqlite-5.607.24116.tar.gz` & `tmp/jx_sqlite-5.626.24125.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jx_sqlite-5.607.24116.tar", last modified: Thu Apr 25 01:00:45 2024, max compression
+gzip compressed data, was "jx_sqlite-5.626.24125.tar", last modified: Sat May  4 21:08:42 2024, max compression
```

## Comparing `jx_sqlite-5.607.24116.tar` & `jx_sqlite-5.626.24125.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 01:00:45.737498 jx_sqlite-5.607.24116/
--rw-rw-rw-   0        0        0    16725 2017-02-23 13:51:40.000000 jx_sqlite-5.607.24116/LICENSE
--rw-rw-rw-   0        0        0     6234 2024-04-25 01:00:45.736461 jx_sqlite-5.607.24116/PKG-INFO
--rw-rw-rw-   0        0        0     4907 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 01:00:45.642420 jx_sqlite-5.607.24116/jx_sqlite/
--rw-rw-rw-   0        0        0      706 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/__init__.py
--rw-rw-rw-   0        0        0    30278 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/edges.py
-drwxrwxrwx   0        0        0        0 2024-04-25 01:00:45.728500 jx_sqlite-5.607.24116/jx_sqlite/expressions/
--rw-rw-rw-   0        0        0     3836 2024-04-04 13:10:35.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/__init__.py
--rw-rw-rw-   0        0        0     4654 2024-04-04 13:10:35.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/_utils.py
--rw-rw-rw-   0        0        0      855 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/abs_op.py
--rw-rw-rw-   0        0        0      440 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/add_op.py
--rw-rw-rw-   0        0        0       79 2024-02-02 03:46:38.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/aggregate_op.py
--rw-rw-rw-   0        0        0     1259 2024-04-04 13:10:35.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/and_op.py
--rw-rw-rw-   0        0        0      550 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/between_op.py
--rw-rw-rw-   0        0        0     1299 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/case_op.py
--rw-rw-rw-   0        0        0      762 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/coalesce_op.py
--rw-rw-rw-   0        0        0     2228 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/concat_op.py
--rw-rw-rw-   0        0        0      710 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/count_op.py
--rw-rw-rw-   0        0        0      658 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/date_op.py
--rw-rw-rw-   0        0        0      566 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/default_op.py
--rw-rw-rw-   0        0        0     1037 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/div_op.py
--rw-rw-rw-   0        0        0     2955 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/eq_op.py
--rw-rw-rw-   0        0        0      721 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/exists_op.py
--rw-rw-rw-   0        0        0      444 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/exp_op.py
--rw-rw-rw-   0        0        0      379 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/filter_op.py
--rw-rw-rw-   0        0        0     1783 2024-04-04 13:10:35.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/find_op.py
--rw-rw-rw-   0        0        0      993 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/first_op.py
--rw-rw-rw-   0        0        0     1446 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/floor_op.py
--rw-rw-rw-   0        0        0      490 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/format_op.py
--rw-rw-rw-   0        0        0      641 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/from_unix_op.py
--rw-rw-rw-   0        0        0     2424 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/get_op.py
--rw-rw-rw-   0        0        0      444 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/gt_op.py
--rw-rw-rw-   0        0        0      448 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/gte_op.py
--rw-rw-rw-   0        0        0     1795 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/in_op.py
--rw-rw-rw-   0        0        0      929 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/is_boolean_op.py
--rw-rw-rw-   0        0        0      649 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/is_integer_op.py
--rw-rw-rw-   0        0        0      643 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/is_number_op.py
--rw-rw-rw-   0        0        0     1376 2024-04-04 13:10:35.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/is_text_op.py
--rw-rw-rw-   0        0        0      369 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/last_op.py
--rw-rw-rw-   0        0        0      448 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/least_op.py
--rw-rw-rw-   0        0        0     1457 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/leaves_op.py
--rw-rw-rw-   0        0        0      922 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/left_op.py
--rw-rw-rw-   0        0        0     1254 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/length_op.py
--rw-rw-rw-   0        0        0      870 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/limit_op.py
--rw-rw-rw-   0        0        0      581 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/literal.py
--rw-rw-rw-   0        0        0      444 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/lt_op.py
--rw-rw-rw-   0        0        0      448 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/lte_op.py
--rw-rw-rw-   0        0        0      692 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/max_op.py
--rw-rw-rw-   0        0        0      672 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/min_op.py
--rw-rw-rw-   0        0        0     1373 2024-04-04 13:10:35.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/missing_op.py
--rw-rw-rw-   0        0        0      444 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/most_op.py
--rw-rw-rw-   0        0        0      440 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/mul_op.py
--rw-rw-rw-   0        0        0      666 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/ne_op.py
--rw-rw-rw-   0        0        0      868 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/nested_op.py
--rw-rw-rw-   0        0        0     1149 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/not_left_op.py
--rw-rw-rw-   0        0        0      864 2024-04-04 13:10:35.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/not_op.py
--rw-rw-rw-   0        0        0     1119 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/not_right_op.py
--rw-rw-rw-   0        0        0      377 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/offset_op.py
--rw-rw-rw-   0        0        0     1025 2024-03-21 02:53:47.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/or_op.py
--rw-rw-rw-   0        0        0     1061 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/prefix_op.py
--rw-rw-rw-   0        0        0      373 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/range_op.py
--rw-rw-rw-   0        0        0      998 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/reg_exp_op.py
--rw-rw-rw-   0        0        0     1021 2024-04-04 13:10:35.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/right_op.py
--rw-rw-rw-   0        0        0      369 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/rows_op.py
--rw-rw-rw-   0        0        0      377 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/script_op.py
--rw-rw-rw-   0        0        0     3123 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/select_op.py
--rw-rw-rw-   0        0        0     1550 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/sql_group_by_op.py
--rw-rw-rw-   0        0        0     1225 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/sql_left_joins_op.py
--rw-rw-rw-   0        0        0      654 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/sql_origins_op.py
--rw-rw-rw-   0        0        0     3755 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/sql_select_all_from_op.py
--rw-rw-rw-   0        0        0     1705 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/sql_select_op.py
--rw-rw-rw-   0        0        0      467 2024-04-04 13:10:35.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/strict_add_op.py
--rw-rw-rw-   0        0        0      574 2024-04-04 13:10:35.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/strict_boolean_op.py
--rw-rw-rw-   0        0        0     1437 2024-04-04 13:10:35.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/strict_eq_op.py
--rw-rw-rw-   0        0        0     1749 2024-04-04 13:10:35.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/strict_in_op.py
--rw-rw-rw-   0        0        0     2017 2024-04-04 13:10:35.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/strict_index_of_op.py
--rw-rw-rw-   0        0        0      478 2024-04-04 13:10:35.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/strict_mul_op.py
--rw-rw-rw-   0        0        0      782 2024-04-04 13:10:35.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/strict_not_op.py
--rw-rw-rw-   0        0        0     1505 2024-04-04 13:10:35.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/strict_starts_with_op.py
--rw-rw-rw-   0        0        0     1070 2024-04-04 13:10:35.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/strict_substring_op.py
--rw-rw-rw-   0        0        0     1186 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/sub_op.py
--rw-rw-rw-   0        0        0      905 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/suffix_op.py
--rw-rw-rw-   0        0        0      355 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/sum_op.py
--rw-rw-rw-   0        0        0      883 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/tally_op.py
--rw-rw-rw-   0        0        0      725 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/to_boolean_op.py
--rw-rw-rw-   0        0        0      831 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/to_integer_op.py
--rw-rw-rw-   0        0        0     1141 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/to_number_op.py
--rw-rw-rw-   0        0        0     2397 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/to_text_op.py
--rw-rw-rw-   0        0        0      794 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/tuple_op.py
--rw-rw-rw-   0        0        0      626 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/unix_op.py
--rw-rw-rw-   0        0        0     2710 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/variable.py
--rw-rw-rw-   0        0        0     1714 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/expressions/when_op.py
--rw-rw-rw-   0        0        0    10200 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/format.py
--rw-rw-rw-   0        0        0     6329 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/group.py
--rw-rw-rw-   0        0        0    17987 2024-03-21 02:53:47.000000 jx_sqlite-5.607.24116/jx_sqlite/insert.py
--rw-rw-rw-   0        0        0    18999 2024-04-19 03:26:09.000000 jx_sqlite-5.607.24116/jx_sqlite/meta_columns.py
-drwxrwxrwx   0        0        0        0 2024-04-25 01:00:45.734381 jx_sqlite-5.607.24116/jx_sqlite/models/
--rw-rw-rw-   0        0        0        0 2024-01-25 04:51:52.000000 jx_sqlite-5.607.24116/jx_sqlite/models/__init__.py
--rw-rw-rw-   0        0        0     7822 2024-04-04 13:10:35.000000 jx_sqlite-5.607.24116/jx_sqlite/models/container.py
--rw-rw-rw-   0        0        0      648 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/models/facts.py
--rw-rw-rw-   0        0        0     1917 2024-03-21 02:53:47.000000 jx_sqlite-5.607.24116/jx_sqlite/models/namespace.py
--rw-rw-rw-   0        0        0      285 2024-02-02 03:46:38.000000 jx_sqlite-5.607.24116/jx_sqlite/models/relation.py
--rw-rw-rw-   0        0        0     8222 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/models/schema.py
--rw-rw-rw-   0        0        0    12948 2024-03-21 02:53:47.000000 jx_sqlite-5.607.24116/jx_sqlite/models/snowflake.py
--rw-rw-rw-   0        0        0     1207 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/models/table.py
--rw-rw-rw-   0        0        0     5288 2024-04-04 13:10:35.000000 jx_sqlite-5.607.24116/jx_sqlite/query.py
--rw-rw-rw-   0        0        0    17005 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/setop.py
--rw-rw-rw-   0        0        0     7201 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/utils.py
--rw-rw-rw-   0        0        0     1446 2024-03-11 07:20:56.000000 jx_sqlite-5.607.24116/jx_sqlite/window.py
-drwxrwxrwx   0        0        0        0 2024-04-25 01:00:45.735448 jx_sqlite-5.607.24116/jx_sqlite.egg-info/
--rw-rw-rw-   0        0        0     6234 2024-04-25 01:00:45.000000 jx_sqlite-5.607.24116/jx_sqlite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3629 2024-04-25 01:00:45.000000 jx_sqlite-5.607.24116/jx_sqlite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 01:00:45.000000 jx_sqlite-5.607.24116/jx_sqlite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2024-04-25 01:00:45.000000 jx_sqlite-5.607.24116/jx_sqlite.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-25 01:00:45.000000 jx_sqlite-5.607.24116/jx_sqlite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 01:00:45.737498 jx_sqlite-5.607.24116/setup.cfg
--rw-rw-rw-   0        0        0     6281 2024-04-25 01:00:41.000000 jx_sqlite-5.607.24116/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 21:08:42.153817 jx_sqlite-5.626.24125/
+-rw-rw-rw-   0        0        0    16725 2017-02-23 13:51:40.000000 jx_sqlite-5.626.24125/LICENSE
+-rw-rw-rw-   0        0        0     6234 2024-05-04 21:08:42.152804 jx_sqlite-5.626.24125/PKG-INFO
+-rw-rw-rw-   0        0        0     4907 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 21:08:42.071021 jx_sqlite-5.626.24125/jx_sqlite/
+-rw-rw-rw-   0        0        0      706 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/__init__.py
+-rw-rw-rw-   0        0        0    30278 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/edges.py
+drwxrwxrwx   0        0        0        0 2024-05-04 21:08:42.144230 jx_sqlite-5.626.24125/jx_sqlite/expressions/
+-rw-rw-rw-   0        0        0     3836 2024-04-04 13:10:35.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/__init__.py
+-rw-rw-rw-   0        0        0     4654 2024-04-04 13:10:35.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/_utils.py
+-rw-rw-rw-   0        0        0      855 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/abs_op.py
+-rw-rw-rw-   0        0        0      440 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/add_op.py
+-rw-rw-rw-   0        0        0       79 2024-02-02 03:46:38.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/aggregate_op.py
+-rw-rw-rw-   0        0        0     1259 2024-04-04 13:10:35.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/and_op.py
+-rw-rw-rw-   0        0        0      550 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/between_op.py
+-rw-rw-rw-   0        0        0     1299 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/case_op.py
+-rw-rw-rw-   0        0        0      762 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/coalesce_op.py
+-rw-rw-rw-   0        0        0     2228 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/concat_op.py
+-rw-rw-rw-   0        0        0      710 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/count_op.py
+-rw-rw-rw-   0        0        0      658 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/date_op.py
+-rw-rw-rw-   0        0        0      566 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/default_op.py
+-rw-rw-rw-   0        0        0     1037 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/div_op.py
+-rw-rw-rw-   0        0        0     2955 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/eq_op.py
+-rw-rw-rw-   0        0        0      721 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/exists_op.py
+-rw-rw-rw-   0        0        0      444 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/exp_op.py
+-rw-rw-rw-   0        0        0      379 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/filter_op.py
+-rw-rw-rw-   0        0        0     1783 2024-04-04 13:10:35.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/find_op.py
+-rw-rw-rw-   0        0        0      993 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/first_op.py
+-rw-rw-rw-   0        0        0     1446 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/floor_op.py
+-rw-rw-rw-   0        0        0      490 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/format_op.py
+-rw-rw-rw-   0        0        0      641 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/from_unix_op.py
+-rw-rw-rw-   0        0        0     2424 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/get_op.py
+-rw-rw-rw-   0        0        0      444 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/gt_op.py
+-rw-rw-rw-   0        0        0      448 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/gte_op.py
+-rw-rw-rw-   0        0        0     1795 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/in_op.py
+-rw-rw-rw-   0        0        0      929 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/is_boolean_op.py
+-rw-rw-rw-   0        0        0      649 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/is_integer_op.py
+-rw-rw-rw-   0        0        0      643 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/is_number_op.py
+-rw-rw-rw-   0        0        0     1376 2024-04-04 13:10:35.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/is_text_op.py
+-rw-rw-rw-   0        0        0      369 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/last_op.py
+-rw-rw-rw-   0        0        0      448 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/least_op.py
+-rw-rw-rw-   0        0        0     1457 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/leaves_op.py
+-rw-rw-rw-   0        0        0      922 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/left_op.py
+-rw-rw-rw-   0        0        0     1254 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/length_op.py
+-rw-rw-rw-   0        0        0      870 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/limit_op.py
+-rw-rw-rw-   0        0        0      581 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/literal.py
+-rw-rw-rw-   0        0        0      444 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/lt_op.py
+-rw-rw-rw-   0        0        0      448 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/lte_op.py
+-rw-rw-rw-   0        0        0      692 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/max_op.py
+-rw-rw-rw-   0        0        0      672 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/min_op.py
+-rw-rw-rw-   0        0        0     1373 2024-04-04 13:10:35.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/missing_op.py
+-rw-rw-rw-   0        0        0      444 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/most_op.py
+-rw-rw-rw-   0        0        0      440 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/mul_op.py
+-rw-rw-rw-   0        0        0      666 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/ne_op.py
+-rw-rw-rw-   0        0        0      868 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/nested_op.py
+-rw-rw-rw-   0        0        0     1149 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/not_left_op.py
+-rw-rw-rw-   0        0        0      864 2024-04-04 13:10:35.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/not_op.py
+-rw-rw-rw-   0        0        0     1119 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/not_right_op.py
+-rw-rw-rw-   0        0        0      377 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/offset_op.py
+-rw-rw-rw-   0        0        0     1025 2024-03-21 02:53:47.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/or_op.py
+-rw-rw-rw-   0        0        0     1061 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/prefix_op.py
+-rw-rw-rw-   0        0        0      373 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/range_op.py
+-rw-rw-rw-   0        0        0      998 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/reg_exp_op.py
+-rw-rw-rw-   0        0        0     1021 2024-04-04 13:10:35.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/right_op.py
+-rw-rw-rw-   0        0        0      369 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/rows_op.py
+-rw-rw-rw-   0        0        0      377 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/script_op.py
+-rw-rw-rw-   0        0        0     3123 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/select_op.py
+-rw-rw-rw-   0        0        0     1550 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/sql_group_by_op.py
+-rw-rw-rw-   0        0        0     1225 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/sql_left_joins_op.py
+-rw-rw-rw-   0        0        0      654 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/sql_origins_op.py
+-rw-rw-rw-   0        0        0     3755 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/sql_select_all_from_op.py
+-rw-rw-rw-   0        0        0     1705 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/sql_select_op.py
+-rw-rw-rw-   0        0        0      467 2024-04-04 13:10:35.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/strict_add_op.py
+-rw-rw-rw-   0        0        0      574 2024-04-04 13:10:35.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/strict_boolean_op.py
+-rw-rw-rw-   0        0        0     1437 2024-04-04 13:10:35.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/strict_eq_op.py
+-rw-rw-rw-   0        0        0     1749 2024-04-04 13:10:35.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/strict_in_op.py
+-rw-rw-rw-   0        0        0     2017 2024-04-04 13:10:35.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/strict_index_of_op.py
+-rw-rw-rw-   0        0        0      478 2024-04-04 13:10:35.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/strict_mul_op.py
+-rw-rw-rw-   0        0        0      782 2024-04-04 13:10:35.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/strict_not_op.py
+-rw-rw-rw-   0        0        0     1505 2024-04-04 13:10:35.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/strict_starts_with_op.py
+-rw-rw-rw-   0        0        0     1070 2024-04-04 13:10:35.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/strict_substring_op.py
+-rw-rw-rw-   0        0        0     1186 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/sub_op.py
+-rw-rw-rw-   0        0        0      905 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/suffix_op.py
+-rw-rw-rw-   0        0        0      355 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/sum_op.py
+-rw-rw-rw-   0        0        0      883 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/tally_op.py
+-rw-rw-rw-   0        0        0      725 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/to_boolean_op.py
+-rw-rw-rw-   0        0        0      831 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/to_integer_op.py
+-rw-rw-rw-   0        0        0     1141 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/to_number_op.py
+-rw-rw-rw-   0        0        0     2397 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/to_text_op.py
+-rw-rw-rw-   0        0        0      794 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/tuple_op.py
+-rw-rw-rw-   0        0        0      626 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/unix_op.py
+-rw-rw-rw-   0        0        0     2710 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/variable.py
+-rw-rw-rw-   0        0        0     1714 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/expressions/when_op.py
+-rw-rw-rw-   0        0        0    10200 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/format.py
+-rw-rw-rw-   0        0        0     6329 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/group.py
+-rw-rw-rw-   0        0        0    17987 2024-03-21 02:53:47.000000 jx_sqlite-5.626.24125/jx_sqlite/insert.py
+-rw-rw-rw-   0        0        0    18999 2024-04-19 03:26:09.000000 jx_sqlite-5.626.24125/jx_sqlite/meta_columns.py
+drwxrwxrwx   0        0        0        0 2024-05-04 21:08:42.150604 jx_sqlite-5.626.24125/jx_sqlite/models/
+-rw-rw-rw-   0        0        0        0 2024-01-25 04:51:52.000000 jx_sqlite-5.626.24125/jx_sqlite/models/__init__.py
+-rw-rw-rw-   0        0        0     7822 2024-04-04 13:10:35.000000 jx_sqlite-5.626.24125/jx_sqlite/models/container.py
+-rw-rw-rw-   0        0        0      648 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/models/facts.py
+-rw-rw-rw-   0        0        0     1917 2024-03-21 02:53:47.000000 jx_sqlite-5.626.24125/jx_sqlite/models/namespace.py
+-rw-rw-rw-   0        0        0      285 2024-02-02 03:46:38.000000 jx_sqlite-5.626.24125/jx_sqlite/models/relation.py
+-rw-rw-rw-   0        0        0     8222 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/models/schema.py
+-rw-rw-rw-   0        0        0    12948 2024-03-21 02:53:47.000000 jx_sqlite-5.626.24125/jx_sqlite/models/snowflake.py
+-rw-rw-rw-   0        0        0     1207 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/models/table.py
+-rw-rw-rw-   0        0        0     5288 2024-04-04 13:10:35.000000 jx_sqlite-5.626.24125/jx_sqlite/query.py
+-rw-rw-rw-   0        0        0    17005 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/setop.py
+-rw-rw-rw-   0        0        0     7201 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/utils.py
+-rw-rw-rw-   0        0        0     1446 2024-03-11 07:20:56.000000 jx_sqlite-5.626.24125/jx_sqlite/window.py
+drwxrwxrwx   0        0        0        0 2024-05-04 21:08:42.151741 jx_sqlite-5.626.24125/jx_sqlite.egg-info/
+-rw-rw-rw-   0        0        0     6234 2024-05-04 21:08:42.000000 jx_sqlite-5.626.24125/jx_sqlite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3629 2024-05-04 21:08:42.000000 jx_sqlite-5.626.24125/jx_sqlite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 21:08:42.000000 jx_sqlite-5.626.24125/jx_sqlite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2024-05-04 21:08:42.000000 jx_sqlite-5.626.24125/jx_sqlite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-04 21:08:42.000000 jx_sqlite-5.626.24125/jx_sqlite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 21:08:42.153817 jx_sqlite-5.626.24125/setup.cfg
+-rw-rw-rw-   0        0        0     6281 2024-05-04 21:08:37.000000 jx_sqlite-5.626.24125/setup.py
```

### Comparing `jx_sqlite-5.607.24116/LICENSE` & `jx_sqlite-5.626.24125/LICENSE`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/PKG-INFO` & `jx_sqlite-5.626.24125/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jx-sqlite
-Version: 5.607.24116
+Version: 5.626.24125
 Summary: JSON query expressions using SQLite
 Home-page: https://github.com/klahnakoski/jx-sqlite
 Author: Rohit Kumar, Kyle Lahnakoski
 Author-email: rohitkumar.a255@gmail.com, kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development :: Libraries
@@ -17,20 +17,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hjson
-Requires-Dist: jx-python==4.607.24116
-Requires-Dist: mo-sql==4.606.24115
-Requires-Dist: mo-sqlite==2.607.24116
+Requires-Dist: jx-python==4.626.24125
+Requires-Dist: mo-sql==4.624.24125
+Requires-Dist: mo-sqlite==2.626.24125
 Requires-Dist: requests
 Provides-Extra: tests
-Requires-Dist: mo-testing>=7.587.24110; extra == "tests"
+Requires-Dist: mo-testing>=8.591.24112; extra == "tests"
 
 # jx-sqlite 
 
 JSON query expressions using SQLite
 
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/jx-sqlite.svg)](https://pypi.org/project/jx-sqlite/)
```

### Comparing `jx_sqlite-5.607.24116/README.md` & `jx_sqlite-5.626.24125/README.md`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/__init__.py` & `jx_sqlite-5.626.24125/jx_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/edges.py` & `jx_sqlite-5.626.24125/jx_sqlite/edges.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/__init__.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/_utils.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/_utils.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/abs_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/abs_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/and_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/and_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/between_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/between_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/case_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/case_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/coalesce_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/coalesce_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/concat_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/concat_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/count_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/count_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/date_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/date_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/default_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/default_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/div_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/div_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/eq_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/eq_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/exists_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/exists_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/find_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/find_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/first_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/first_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/floor_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/floor_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/from_unix_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/from_unix_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/get_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/get_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/in_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/in_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/is_boolean_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/is_boolean_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/is_integer_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/is_integer_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/is_number_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/is_number_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/is_text_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/is_text_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/leaves_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/leaves_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/left_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/left_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/length_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/length_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/limit_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/limit_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/literal.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/literal.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/max_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/max_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/min_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/min_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/missing_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/missing_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/ne_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/ne_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/nested_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/nested_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/not_left_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/not_left_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/not_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/not_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/not_right_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/not_right_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/or_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/or_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/prefix_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/prefix_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/reg_exp_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/reg_exp_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/right_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/right_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/select_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/select_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/sql_group_by_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/sql_group_by_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/sql_left_joins_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/sql_left_joins_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/sql_origins_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/sql_origins_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/sql_select_all_from_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/sql_select_all_from_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/sql_select_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/sql_select_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/strict_boolean_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/strict_boolean_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/strict_eq_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/strict_eq_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/strict_in_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/strict_in_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/strict_index_of_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/strict_index_of_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/strict_not_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/strict_not_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/strict_starts_with_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/strict_starts_with_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/strict_substring_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/strict_substring_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/sub_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/sub_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/suffix_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/suffix_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/tally_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/tally_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/to_boolean_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/to_boolean_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/to_integer_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/to_integer_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/to_number_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/to_number_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/to_text_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/to_text_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/tuple_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/tuple_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/unix_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/unix_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/variable.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/variable.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/expressions/when_op.py` & `jx_sqlite-5.626.24125/jx_sqlite/expressions/when_op.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/format.py` & `jx_sqlite-5.626.24125/jx_sqlite/format.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/group.py` & `jx_sqlite-5.626.24125/jx_sqlite/group.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/insert.py` & `jx_sqlite-5.626.24125/jx_sqlite/insert.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/meta_columns.py` & `jx_sqlite-5.626.24125/jx_sqlite/meta_columns.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/models/container.py` & `jx_sqlite-5.626.24125/jx_sqlite/models/container.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/models/facts.py` & `jx_sqlite-5.626.24125/jx_sqlite/models/facts.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/models/namespace.py` & `jx_sqlite-5.626.24125/jx_sqlite/models/namespace.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/models/schema.py` & `jx_sqlite-5.626.24125/jx_sqlite/models/schema.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/models/snowflake.py` & `jx_sqlite-5.626.24125/jx_sqlite/models/snowflake.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/models/table.py` & `jx_sqlite-5.626.24125/jx_sqlite/models/table.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/query.py` & `jx_sqlite-5.626.24125/jx_sqlite/query.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/setop.py` & `jx_sqlite-5.626.24125/jx_sqlite/setop.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/utils.py` & `jx_sqlite-5.626.24125/jx_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite/window.py` & `jx_sqlite-5.626.24125/jx_sqlite/window.py`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/jx_sqlite.egg-info/PKG-INFO` & `jx_sqlite-5.626.24125/jx_sqlite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jx-sqlite
-Version: 5.607.24116
+Version: 5.626.24125
 Summary: JSON query expressions using SQLite
 Home-page: https://github.com/klahnakoski/jx-sqlite
 Author: Rohit Kumar, Kyle Lahnakoski
 Author-email: rohitkumar.a255@gmail.com, kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development :: Libraries
@@ -17,20 +17,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hjson
-Requires-Dist: jx-python==4.607.24116
-Requires-Dist: mo-sql==4.606.24115
-Requires-Dist: mo-sqlite==2.607.24116
+Requires-Dist: jx-python==4.626.24125
+Requires-Dist: mo-sql==4.624.24125
+Requires-Dist: mo-sqlite==2.626.24125
 Requires-Dist: requests
 Provides-Extra: tests
-Requires-Dist: mo-testing>=7.587.24110; extra == "tests"
+Requires-Dist: mo-testing>=8.591.24112; extra == "tests"
 
 # jx-sqlite 
 
 JSON query expressions using SQLite
 
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/jx-sqlite.svg)](https://pypi.org/project/jx-sqlite/)
```

### Comparing `jx_sqlite-5.607.24116/jx_sqlite.egg-info/SOURCES.txt` & `jx_sqlite-5.626.24125/jx_sqlite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jx_sqlite-5.607.24116/setup.py` & `jx_sqlite-5.626.24125/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 # THIS FILE IS AUTOGENERATED!
 from setuptools import setup
 setup(
     author='Rohit Kumar, Kyle Lahnakoski',
     author_email='rohitkumar.a255@gmail.com, kyle@lahnakoski.com',
     classifiers=["Development Status :: 3 - Alpha","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules","License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)","Topic :: Database","Topic :: Utilities","Programming Language :: SQL","Programming Language :: Python :: 3.8","Programming Language :: Python :: 3.9","Programming Language :: Python :: 3.10","Programming Language :: Python :: 3.11","Programming Language :: Python :: 3.12"],
     description='JSON query expressions using SQLite',
-    extras_require={"tests":["mo-testing>=7.587.24110"]},
+    extras_require={"tests":["mo-testing>=8.591.24112"]},
     include_package_data=True,
-    install_requires=["hjson","jx-python==4.607.24116","mo-sql==4.606.24115","mo-sqlite==2.607.24116","requests"],
+    install_requires=["hjson","jx-python==4.626.24125","mo-sql==4.624.24125","mo-sqlite==2.626.24125","requests"],
     license='MPL 2.0',
     long_description='# jx-sqlite \n\nJSON query expressions using SQLite\n\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/jx-sqlite.svg)](https://pypi.org/project/jx-sqlite/)\n[![Build Status](https://app.travis-ci.com/klahnakoski/jx-sqlite.svg?branch=master)](https://travis-ci.com/github/klahnakoski/jx-sqlite)\n[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/jx-sqlite/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/jx-sqlite?branch=dev)\n\n## Summary\n\nThis library will manage your database schema to store JSON documents. You get all the speed of a well-formed database schema without the schema migration headaches. \n\n\n## Status\n\nSignificant updates to the supporting libraries has broken this code.  It still works for the simple cases that require it\n\n**Jan 2024** - 118 of 334 tests ignored\n\n\n## Installation\n\n    pip install jx-sqlite\n\n## Code Example\n\nThe smoke test, found in the `tests` is a simple example of how to use this library.\n\n```python\nimport jx_sqlite\n\ntable = (\n    jx_sqlite\n    .Container(filename="my.db")\n    .get_or_create_facts("my_table")\n    .insert([{"os": "linux", "value": 42}])\n    .query({\n        "select": "os",\n        "where": {"gt": {"value": 0}}\n    })\n)\n```\n\n## More\n\nThis project is an attempt to store JSON documents in SQLite so that they are accessible via SQL. The hope is this will serve a basis for a general document-relational map (DRM), and leverage the database\'s query optimizer.\n`jx-sqlite` is responsible for expanding the schema dynamically as new JSON documents are encountered.  It also strives to ensure old queries against the new schema have the same meaning; the same results.\n\nThe most interesting, and most important feature is that we query nested object arrays as if they were just another table.  This is important for two reasons:\n\n1. Inner objects `{"a": {"b": 0}}` are a shortcut for nested arrays `{"a": [{"b": 0}]}`, plus\n2. Schemas can be expanded from one-to-one  to one-to-many `{"a": [{"b": 0}, {"b": 1}]}`.\n\n\n## Motivation\n\nJSON is a nice format to store data, and it has become quite prevalent. Unfortunately, databases do not handle it well, often a human is required to declare a schema that can hold the JSON before it can be queried. If we are not overwhelmed by the diversity of JSON now, we soon will be. There will be more JSON, of more different shapes, as the number of connected devices( and the information they generate) continues to increase.\n\n## Contributing\n\nContributions are always welcome! The best thing to do is find a failing test, and try to fix it.\n\nThese instructions will get you a copy of the project up and running on your local machine for development and testing purposes.\n\n    $ git clone https://github.com/klahnakoski/jx-sqlite\n    $ cd jx-sqlite\n\n### Running tests\n\nThere are over 300 tests used to confirm the expected behaviour: They test a variety of JSON forms, and the queries that can be performed on them. Most tests are further split into three different output formats ( list, table and cube).\n\nThe `requirements.lock` file is the last successful combination that passed all tests, despite the version conflicts.\n\n    python.exe -m pip install --no-deps -r tests\\requirements.lock\n\n\nLinux\n\n    export PYTHONPATH=.:vendor\n    python -m unittest discover -v -s tests\n\nWindows\n\n    set PYTHONPATH=.;vendor\n    python -m unittest discover -v -s tests\n\n\n### Technical Docs\n\n* [Json Query Expression](https://github.com/klahnakoski/ActiveData/blob/dev/docs/jx.md)\n* [Nomenclature](https://github.com/mozilla/jx-sqlite/blob/master/docs/Nomenclature.md)\n* [Snowflake](https://github.com/mozilla/jx-sqlite/blob/master/docs/Perspective.md)\n* [JSON in Database](https://github.com/mozilla/jx-sqlite/blob/master/docs/JSON%20in%20Database.md)\n* [The Future](https://github.com/mozilla/jx-sqlite/blob/master/docs/The%20Future.md)\n\n## License\n\nThis project is licensed under Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed with this file, You can obtain one at http://mozilla.org/MPL/2.0/.\n\n\n## History\n\n*Jan 2024* - Attempt to resurrect this project (118 of 334 tests ignored)\n\n*Sep 2018* - Upgrade libs, start refactoring to work with other libs\n\n*Dec 2017* - A number of tests were added, but they do not pass.\n\n*Sep 2017* - GSoC work completed, all but a few tests pass.\n \n\n## GSOC\n\nGood work by Rohit Kumar.  You may see the end result on [gsoc branch](https://github.com/klahnakoski/jx-sqlite/tree/gsoc).  Installation requires python2.7,  and will require some version fixing to get running.\n\nSee [the demonstration video](https://www.youtube.com/watch?v=0_YLzb7BegI&list=PLSE8ODhjZXja7K1hjZ01UTVDnGQdx5v5U&index=26&t=260s)\n\n\nWork done up to the deadline of GSoC\'17:\n\n* [Pull Requests](https://github.com/mozilla/jx-sqlite/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Arohit-rk)\n* [Commits](https://github.com/mozilla/jx-sqlite/commits?author=rohit-rk)\n\n\n\n',
     long_description_content_type='text/markdown',
     name='jx-sqlite',
     package_dir={},
     packages=["jx_sqlite","jx_sqlite.models","jx_sqlite.expressions"],
     url='https://github.com/klahnakoski/jx-sqlite',
-    version='5.607.24116'
+    version='5.626.24125'
 )
```

