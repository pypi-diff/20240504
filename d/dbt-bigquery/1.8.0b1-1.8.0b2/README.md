# Comparing `tmp/dbt-bigquery-1.8.0b1.tar.gz` & `tmp/dbt-bigquery-1.8.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-bigquery-1.8.0b1.tar", last modified: Fri Mar  1 23:17:59 2024, max compression
+gzip compressed data, was "dbt-bigquery-1.8.0b2.tar", last modified: Wed Apr  3 20:04:37 2024, max compression
```

## Comparing `dbt-bigquery-1.8.0b1.tar` & `dbt-bigquery-1.8.0b2.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:17:59.407912 dbt-bigquery-1.8.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-03-01 23:17:59.407912 dbt-bigquery-1.8.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:17:59.387911 dbt-bigquery-1.8.0b1/dbt/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:17:59.383911 dbt-bigquery-1.8.0b1/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:17:59.391912 dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11429 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/column.py
--rw-r--r--   0 runner    (1001) docker     (127)    29045 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/connections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:17:59.391912 dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/dataproc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/dataproc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/dataproc/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/gcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    37964 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     7538 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/python_submissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6358 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:17:59.391912 dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/relation_configs/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/relation_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/relation_configs/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/relation_configs/_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/relation_configs/_materialized_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/relation_configs/_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/relation_configs/_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/relation_configs/_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:17:59.383911 dbt-bigquery-1.8.0b1/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:17:59.391912 dbt-bigquery-1.8.0b1/dbt/include/bigquery/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:17:59.391912 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:17:59.391912 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/adapters.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:17:59.391912 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/catalog/by_relation.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/catalog/by_schema.sql
--rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/catalog/catalog.sql
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/etc.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:17:59.391912 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/materializations/clone.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/materializations/copy.sql
--rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/materializations/incremental.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:17:59.395912 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/materializations/incremental_strategy/
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/materializations/incremental_strategy/common.sql
--rw-r--r--   0 runner    (1001) docker     (127)     7382 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/materializations/incremental_strategy/insert_overwrite.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/materializations/incremental_strategy/merge.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/materializations/incremental_strategy/time_ingestion_tables.sql
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:17:59.395912 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/python_model/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/python_model/python.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:17:59.395912 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/relations/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/relations/cluster.sql
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/relations/drop.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:17:59.395912 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/relations/materialized_view/
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/relations/materialized_view/alter.sql
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/relations/materialized_view/create.sql
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/relations/materialized_view/drop.sql
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/relations/materialized_view/refresh.sql
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/relations/materialized_view/replace.sql
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/relations/options.sql
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/relations/partition.sql
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/relations/rename.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:17:59.399911 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/relations/table/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/relations/table/drop.sql
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/relations/table/options.sql
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/relations/table/rename.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:17:59.399911 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/relations/view/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/relations/view/drop.sql
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/relations/view/options.sql
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/relations/view/rename.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/relations/view/replace.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:17:59.403912 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/utils/except.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/utils/get_columns_spec_ddl.sql
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/utils/intersect.sql
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/utils/position.sql
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/dbt/include/bigquery/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 23:17:59.407912 dbt-bigquery-1.8.0b1/dbt_bigquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-03-01 23:17:59.000000 dbt-bigquery-1.8.0b1/dbt_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-03-01 23:17:59.000000 dbt-bigquery-1.8.0b1/dbt_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 23:17:59.000000 dbt-bigquery-1.8.0b1/dbt_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 23:17:59.000000 dbt-bigquery-1.8.0b1/dbt_bigquery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-01 23:17:59.000000 dbt-bigquery-1.8.0b1/dbt_bigquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-01 23:17:59.000000 dbt-bigquery-1.8.0b1/dbt_bigquery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 23:17:59.407912 dbt-bigquery-1.8.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-03-01 23:17:49.000000 dbt-bigquery-1.8.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.557318 dbt-bigquery-1.8.0b2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-03 20:04:37.557318 dbt-bigquery-1.8.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.541318 dbt-bigquery-1.8.0b2/dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.541318 dbt-bigquery-1.8.0b2/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.545318 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11429 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29022 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/connections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.545318 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/dataproc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/dataproc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/dataproc/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/gcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37964 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7538 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/python_submissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.545318 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation_configs/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation_configs/_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation_configs/_materialized_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation_configs/_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation_configs/_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation_configs/_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.541318 dbt-bigquery-1.8.0b2/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.545318 dbt-bigquery-1.8.0b2/dbt/include/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.545318 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.545318 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/adapters.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.549318 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/catalog/by_relation.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/catalog/by_schema.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/catalog/catalog.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/etc.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.549318 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/clone.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/copy.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/incremental.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.549318 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/incremental_strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/incremental_strategy/common.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     7382 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/incremental_strategy/insert_overwrite.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/incremental_strategy/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/incremental_strategy/time_ingestion_tables.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.549318 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/python_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/python_model/python.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.549318 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/cluster.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/drop.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.549318 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/materialized_view/
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/materialized_view/alter.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/materialized_view/create.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/materialized_view/drop.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/materialized_view/refresh.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/materialized_view/replace.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/options.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/partition.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/rename.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.553318 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/table/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/table/drop.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/table/options.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/table/rename.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.553318 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/view/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/view/drop.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/view/options.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/view/rename.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/view/replace.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.557318 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/except.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/get_columns_spec_ddl.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/intersect.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/position.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.557318 dbt-bigquery-1.8.0b2/dbt_bigquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-03 20:04:37.000000 dbt-bigquery-1.8.0b2/dbt_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-04-03 20:04:37.000000 dbt-bigquery-1.8.0b2/dbt_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:04:37.000000 dbt-bigquery-1.8.0b2/dbt_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:04:37.000000 dbt-bigquery-1.8.0b2/dbt_bigquery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-03 20:04:37.000000 dbt-bigquery-1.8.0b2/dbt_bigquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-03 20:04:37.000000 dbt-bigquery-1.8.0b2/dbt_bigquery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 20:04:37.557318 dbt-bigquery-1.8.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/setup.py
```

### Comparing `dbt-bigquery-1.8.0b1/LICENSE.md` & `dbt-bigquery-1.8.0b2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/PKG-INFO` & `dbt-bigquery-1.8.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-bigquery
-Version: 1.8.0b1
+Version: 1.8.0b2
 Summary: The Bigquery adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-bigquery
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -15,18 +15,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: dbt-common<2.0,>=0.1.0a1
 Requires-Dist: dbt-adapters<2.0,>=0.1.0a1
-Requires-Dist: google-cloud-bigquery~=3.0
+Requires-Dist: google-cloud-bigquery[pandas]<4.0,>=3.0
 Requires-Dist: google-cloud-storage~=2.4
 Requires-Dist: google-cloud-dataproc~=5.0
 Requires-Dist: google-api-core>=2.11.0
+Requires-Dist: dbt-core>=1.8.0a1
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="500"/>
 </p>
 <p align="center">
   <a href="https://github.com/dbt-labs/dbt-bigquery/actions/workflows/main.yml">
     <img src="https://github.com/dbt-labs/dbt-bigquery/actions/workflows/main.yml/badge.svg?event=push" alt="Unit Tests Badge"/>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: dbt-bigquery Version: 1.8.0b1 Summary: The Bigquery
+Metadata-Version: 2.1 Name: dbt-bigquery Version: 1.8.0b2 Summary: The Bigquery
 adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-bigquery
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE.md Requires-Dist:
 dbt-common<2.0,>=0.1.0a1 Requires-Dist: dbt-adapters<2.0,>=0.1.0a1 Requires-
-Dist: google-cloud-bigquery~=3.0 Requires-Dist: google-cloud-storage~=2.4
-Requires-Dist: google-cloud-dataproc~=5.0 Requires-Dist: google-api-
-core>=2.11.0
+Dist: google-cloud-bigquery[pandas]<4.0,>=3.0 Requires-Dist: google-cloud-
+storage~=2.4 Requires-Dist: google-cloud-dataproc~=5.0 Requires-Dist: google-
+api-core>=2.11.0 Requires-Dist: dbt-core>=1.8.0a1
                                   [dbt logo]
                   _[_U_n_i_t_ _T_e_s_t_s_ _B_a_d_g_e_]_[_I_n_t_e_g_r_a_t_i_o_n_ _T_e_s_t_s_ _B_a_d_g_e_]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-bigquery The `dbt-bigquery` package contains all of
```

### Comparing `dbt-bigquery-1.8.0b1/README.md` & `dbt-bigquery-1.8.0b2/README.md`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/__init__.py` & `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/column.py` & `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/column.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/connections.py` & `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/connections.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,14 @@
             "priority",
             "maximum_bytes_billed",
             "impersonate_service_account",
             "job_retry_deadline_seconds",
             "job_retries",
             "job_creation_timeout_seconds",
             "job_execution_timeout_seconds",
-            "keyfile",
             "timeout_seconds",
             "client_id",
             "token_uri",
             "dataproc_region",
             "dataproc_cluster_name",
             "gcs_bucket",
             "dataproc_batch",
```

### Comparing `dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/dataproc/batch.py` & `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/dataproc/batch.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/dataset.py` & `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/dataset.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/gcloud.py` & `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/gcloud.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/impl.py` & `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/python_submissions.py` & `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/python_submissions.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/relation.py` & `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import FrozenSet, Optional, TypeVar
 
 from itertools import chain, islice
 from dbt.adapters.base.relation import BaseRelation, ComponentName, InformationSchema
 from dbt.adapters.relation_configs import RelationConfigChangeAction
 from dbt.adapters.bigquery.relation_configs import (
     BigQueryClusterConfigChange,
@@ -19,17 +19,30 @@
 Self = TypeVar("Self", bound="BigQueryRelation")
 
 
 @dataclass(frozen=True, eq=False, repr=False)
 class BigQueryRelation(BaseRelation):
     quote_character: str = "`"
     location: Optional[str] = None
-    renameable_relations: FrozenSet[RelationType] = frozenset({RelationType.Table})
-    replaceable_relations: FrozenSet[RelationType] = frozenset(
-        {RelationType.Table, RelationType.View}
+
+    renameable_relations: FrozenSet[RelationType] = field(
+        default_factory=lambda: frozenset(
+            {
+                RelationType.Table,
+            }
+        )
+    )
+
+    replaceable_relations: FrozenSet[RelationType] = field(
+        default_factory=lambda: frozenset(
+            {
+                RelationType.View,
+                RelationType.Table,
+            }
+        )
     )
 
     def matches(
         self,
         database: Optional[str] = None,
         schema: Optional[str] = None,
         identifier: Optional[str] = None,
```

### Comparing `dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/relation_configs/__init__.py` & `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/relation_configs/_base.py` & `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation_configs/_base.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/relation_configs/_cluster.py` & `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation_configs/_cluster.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/relation_configs/_materialized_view.py` & `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation_configs/_materialized_view.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/relation_configs/_options.py` & `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation_configs/_options.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/relation_configs/_partition.py` & `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation_configs/_partition.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/adapters/bigquery/utility.py` & `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/utility.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/adapters/apply_grants.sql` & `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/adapters.sql` & `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/catalog/by_relation.sql` & `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/catalog/by_relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/catalog/by_schema.sql` & `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/catalog/by_schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/catalog/catalog.sql` & `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/catalog/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/materializations/copy.sql` & `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/copy.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/materializations/incremental.sql` & `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/materializations/incremental_strategy/common.sql` & `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/incremental_strategy/common.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/materializations/incremental_strategy/insert_overwrite.sql` & `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/incremental_strategy/insert_overwrite.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/materializations/incremental_strategy/merge.sql` & `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/incremental_strategy/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/materializations/incremental_strategy/time_ingestion_tables.sql` & `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/incremental_strategy/time_ingestion_tables.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/materializations/seed.sql` & `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/materializations/table.sql` & `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/materializations/view.sql` & `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/relations/materialized_view/alter.sql` & `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/materialized_view/alter.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/relations/materialized_view/create.sql` & `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/materialized_view/create.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/relations/materialized_view/replace.sql` & `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/materialized_view/replace.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/relations/partition.sql` & `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/partition.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/relations/view/replace.sql` & `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/view/replace.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/utils/get_columns_spec_ddl.sql` & `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/get_columns_spec_ddl.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/utils/safe_cast.sql` & `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/safe_cast.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/include/bigquery/macros/utils/split_part.sql` & `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt/include/bigquery/profile_template.yml` & `dbt-bigquery-1.8.0b2/dbt/include/bigquery/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/dbt_bigquery.egg-info/PKG-INFO` & `dbt-bigquery-1.8.0b2/dbt_bigquery.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-bigquery
-Version: 1.8.0b1
+Version: 1.8.0b2
 Summary: The Bigquery adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-bigquery
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -15,18 +15,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: dbt-common<2.0,>=0.1.0a1
 Requires-Dist: dbt-adapters<2.0,>=0.1.0a1
-Requires-Dist: google-cloud-bigquery~=3.0
+Requires-Dist: google-cloud-bigquery[pandas]<4.0,>=3.0
 Requires-Dist: google-cloud-storage~=2.4
 Requires-Dist: google-cloud-dataproc~=5.0
 Requires-Dist: google-api-core>=2.11.0
+Requires-Dist: dbt-core>=1.8.0a1
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="500"/>
 </p>
 <p align="center">
   <a href="https://github.com/dbt-labs/dbt-bigquery/actions/workflows/main.yml">
     <img src="https://github.com/dbt-labs/dbt-bigquery/actions/workflows/main.yml/badge.svg?event=push" alt="Unit Tests Badge"/>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: dbt-bigquery Version: 1.8.0b1 Summary: The Bigquery
+Metadata-Version: 2.1 Name: dbt-bigquery Version: 1.8.0b2 Summary: The Bigquery
 adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-bigquery
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE.md Requires-Dist:
 dbt-common<2.0,>=0.1.0a1 Requires-Dist: dbt-adapters<2.0,>=0.1.0a1 Requires-
-Dist: google-cloud-bigquery~=3.0 Requires-Dist: google-cloud-storage~=2.4
-Requires-Dist: google-cloud-dataproc~=5.0 Requires-Dist: google-api-
-core>=2.11.0
+Dist: google-cloud-bigquery[pandas]<4.0,>=3.0 Requires-Dist: google-cloud-
+storage~=2.4 Requires-Dist: google-cloud-dataproc~=5.0 Requires-Dist: google-
+api-core>=2.11.0 Requires-Dist: dbt-core>=1.8.0a1
                                   [dbt logo]
                   _[_U_n_i_t_ _T_e_s_t_s_ _B_a_d_g_e_]_[_I_n_t_e_g_r_a_t_i_o_n_ _T_e_s_t_s_ _B_a_d_g_e_]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-bigquery The `dbt-bigquery` package contains all of
```

### Comparing `dbt-bigquery-1.8.0b1/dbt_bigquery.egg-info/SOURCES.txt` & `dbt-bigquery-1.8.0b2/dbt_bigquery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b1/setup.py` & `dbt-bigquery-1.8.0b2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     """
     attributes = {}
     exec(VERSION.read_text(), attributes)
     return attributes["version"]
 
 
 package_name = "dbt-bigquery"
-package_version = "1.8.0b1"
+package_version = "1.8.0b2"
 description = """The BigQuery adapter plugin for dbt"""
 
 setup(
     name="dbt-bigquery",
     version=_dbt_bigquery_version(),
     description="The Bigquery adapter plugin for dbt",
     long_description=README.read_text(),
@@ -49,20 +49,23 @@
     author_email="info@dbtlabs.com",
     url="https://github.com/dbt-labs/dbt-bigquery",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
         "dbt-common>=0.1.0a1,<2.0",
         "dbt-adapters>=0.1.0a1,<2.0",
-        "google-cloud-bigquery~=3.0",
+        # 3.20 introduced pyarrow>=3.0 under the `pandas` extra
+        "google-cloud-bigquery[pandas]>=3.0,<4.0",
         "google-cloud-storage~=2.4",
         "google-cloud-dataproc~=5.0",
         # ----
         # Expect compatibility with all new versions of these packages, so lower bounds only.
         "google-api-core>=2.11.0",
+        # add dbt-core to ensure backwards compatibility of installation, this is not a functional dependency
+        "dbt-core>=1.8.0a1",
     ],
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
```

