# Comparing `tmp/dbt-bigquery-1.8.0b2.tar.gz` & `tmp/dbt_bigquery-1.8.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-bigquery-1.8.0b2.tar", last modified: Wed Apr  3 20:04:37 2024, max compression
+gzip compressed data, was "dbt_bigquery-1.8.0rc1.tar", last modified: Fri May  3 22:51:44 2024, max compression
```

## Comparing `dbt-bigquery-1.8.0b2.tar` & `dbt_bigquery-1.8.0rc1.tar`

### file list

```diff
@@ -1,109 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.557318 dbt-bigquery-1.8.0b2/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-03 20:04:37.557318 dbt-bigquery-1.8.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.541318 dbt-bigquery-1.8.0b2/dbt/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.541318 dbt-bigquery-1.8.0b2/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.545318 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11429 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/column.py
--rw-r--r--   0 runner    (1001) docker     (127)    29022 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/connections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.545318 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/dataproc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/dataproc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/dataproc/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/gcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    37964 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     7538 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/python_submissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.545318 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation_configs/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation_configs/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation_configs/_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation_configs/_materialized_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation_configs/_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation_configs/_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation_configs/_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.541318 dbt-bigquery-1.8.0b2/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.545318 dbt-bigquery-1.8.0b2/dbt/include/bigquery/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.545318 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.545318 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/adapters.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.549318 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/catalog/by_relation.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/catalog/by_schema.sql
--rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/catalog/catalog.sql
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/etc.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.549318 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/clone.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/copy.sql
--rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/incremental.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.549318 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/incremental_strategy/
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/incremental_strategy/common.sql
--rw-r--r--   0 runner    (1001) docker     (127)     7382 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/incremental_strategy/insert_overwrite.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/incremental_strategy/merge.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/incremental_strategy/time_ingestion_tables.sql
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.549318 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/python_model/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/python_model/python.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.549318 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/cluster.sql
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/drop.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.549318 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/materialized_view/
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/materialized_view/alter.sql
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/materialized_view/create.sql
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/materialized_view/drop.sql
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/materialized_view/refresh.sql
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/materialized_view/replace.sql
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/options.sql
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/partition.sql
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/rename.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.553318 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/table/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/table/drop.sql
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/table/options.sql
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/table/rename.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.553318 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/view/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/view/drop.sql
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/view/options.sql
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/view/rename.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/view/replace.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.557318 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/except.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/get_columns_spec_ddl.sql
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/intersect.sql
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/position.sql
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/dbt/include/bigquery/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:04:37.557318 dbt-bigquery-1.8.0b2/dbt_bigquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-03 20:04:37.000000 dbt-bigquery-1.8.0b2/dbt_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-04-03 20:04:37.000000 dbt-bigquery-1.8.0b2/dbt_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:04:37.000000 dbt-bigquery-1.8.0b2/dbt_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:04:37.000000 dbt-bigquery-1.8.0b2/dbt_bigquery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-03 20:04:37.000000 dbt-bigquery-1.8.0b2/dbt_bigquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-03 20:04:37.000000 dbt-bigquery-1.8.0b2/dbt_bigquery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 20:04:37.557318 dbt-bigquery-1.8.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-03 20:04:21.000000 dbt-bigquery-1.8.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:51:44.921049 dbt_bigquery-1.8.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-03 22:51:44.921049 dbt_bigquery-1.8.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:51:44.905049 dbt_bigquery-1.8.0rc1/dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:51:44.901049 dbt_bigquery-1.8.0rc1/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:51:44.905049 dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11429 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29265 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/connections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:51:44.905049 dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/dataproc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/dataproc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/dataproc/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/gcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37964 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7538 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/python_submissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:51:44.909049 dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/relation_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/relation_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/relation_configs/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/relation_configs/_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/relation_configs/_materialized_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/relation_configs/_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/relation_configs/_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/relation_configs/_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:51:44.901049 dbt_bigquery-1.8.0rc1/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:51:44.909049 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:51:44.909049 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:51:44.909049 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/adapters.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:51:44.909049 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/catalog/by_relation.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/catalog/by_schema.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/catalog/catalog.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/etc.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:51:44.913049 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/materializations/clone.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/materializations/copy.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/materializations/incremental.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:51:44.913049 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/common.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     7382 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/insert_overwrite.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/time_ingestion_tables.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:51:44.913049 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/python_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/python_model/python.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:51:44.913049 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/relations/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/relations/cluster.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/relations/drop.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:51:44.913049 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/relations/materialized_view/
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/relations/materialized_view/alter.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/relations/materialized_view/create.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/relations/materialized_view/drop.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/relations/materialized_view/refresh.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/relations/materialized_view/replace.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/relations/options.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/relations/partition.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/relations/rename.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:51:44.913049 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/relations/table/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/relations/table/drop.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/relations/table/options.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/relations/table/rename.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:51:44.917049 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/relations/view/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/relations/view/drop.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/relations/view/options.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/relations/view/rename.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/relations/view/replace.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:51:44.917049 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/utils/except.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/utils/get_columns_spec_ddl.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/utils/intersect.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/utils/position.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/utils/string_literal.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/dbt/include/bigquery/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:51:44.921049 dbt_bigquery-1.8.0rc1/dbt_bigquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-03 22:51:44.000000 dbt_bigquery-1.8.0rc1/dbt_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-03 22:51:44.000000 dbt_bigquery-1.8.0rc1/dbt_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 22:51:44.000000 dbt_bigquery-1.8.0rc1/dbt_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 22:51:44.000000 dbt_bigquery-1.8.0rc1/dbt_bigquery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-03 22:51:44.000000 dbt_bigquery-1.8.0rc1/dbt_bigquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-03 22:51:44.000000 dbt_bigquery-1.8.0rc1/dbt_bigquery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 22:51:44.921049 dbt_bigquery-1.8.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-03 22:51:32.000000 dbt_bigquery-1.8.0rc1/setup.py
```

### Comparing `dbt-bigquery-1.8.0b2/LICENSE.md` & `dbt_bigquery-1.8.0rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/PKG-INFO` & `dbt_bigquery-1.8.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-bigquery
-Version: 1.8.0b2
+Version: 1.8.0rc1
 Summary: The Bigquery adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-bigquery
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
-Metadata-Version: 2.1 Name: dbt-bigquery Version: 1.8.0b2 Summary: The Bigquery
-adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-bigquery
-Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
-:: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
-License Classifier: Operating System :: Microsoft :: Windows Classifier:
-Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
-Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE.md Requires-Dist:
-dbt-common<2.0,>=0.1.0a1 Requires-Dist: dbt-adapters<2.0,>=0.1.0a1 Requires-
-Dist: google-cloud-bigquery[pandas]<4.0,>=3.0 Requires-Dist: google-cloud-
-storage~=2.4 Requires-Dist: google-cloud-dataproc~=5.0 Requires-Dist: google-
-api-core>=2.11.0 Requires-Dist: dbt-core>=1.8.0a1
+Metadata-Version: 2.1 Name: dbt-bigquery Version: 1.8.0rc1 Summary: The
+Bigquery adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
+bigquery Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+:: Apache Software License Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
+:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Python: >=3.8 Description-Content-Type: text/markdown License-File: LICENSE.md
+Requires-Dist: dbt-common<2.0,>=0.1.0a1 Requires-Dist: dbt-
+adapters<2.0,>=0.1.0a1 Requires-Dist: google-cloud-bigquery[pandas]<4.0,>=3.0
+Requires-Dist: google-cloud-storage~=2.4 Requires-Dist: google-cloud-
+dataproc~=5.0 Requires-Dist: google-api-core>=2.11.0 Requires-Dist: dbt-
+core>=1.8.0a1
                                   [dbt logo]
                   _[_U_n_i_t_ _T_e_s_t_s_ _B_a_d_g_e_]_[_I_n_t_e_g_r_a_t_i_o_n_ _T_e_s_t_s_ _B_a_d_g_e_]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-bigquery The `dbt-bigquery` package contains all of
```

### Comparing `dbt-bigquery-1.8.0b2/README.md` & `dbt_bigquery-1.8.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/__init__.py` & `dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/column.py` & `dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/column.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/connections.py` & `dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/connections.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from concurrent.futures import TimeoutError
 import json
 import re
 from contextlib import contextmanager
 from dataclasses import dataclass, field
 
 from dbt_common.invocation import get_invocation_id
 
@@ -732,17 +733,20 @@
             query_job.location is not None
             and query_job.job_id is not None
             and query_job.project is not None
         ):
             logger.debug(
                 self._bq_job_link(query_job.location, query_job.project, query_job.job_id)
             )
-
-        iterator = query_job.result(max_results=limit, timeout=job_execution_timeout)
-        return query_job, iterator
+        try:
+            iterator = query_job.result(max_results=limit, timeout=job_execution_timeout)
+            return query_job, iterator
+        except TimeoutError:
+            exc = f"Operation did not complete within the designated timeout of {job_execution_timeout} seconds."
+            raise TimeoutError(exc)
 
     def _retry_and_handle(self, msg, conn, fn):
         """retry a function call within the context of exception_handler."""
 
         def reopen_conn_on_error(error):
             if isinstance(error, REOPENABLE_ERRORS):
                 logger.warning("Reopening connection after {!r}".format(error))
```

### Comparing `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/dataproc/batch.py` & `dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/dataproc/batch.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/dataset.py` & `dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/dataset.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/gcloud.py` & `dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/gcloud.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/impl.py` & `dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/python_submissions.py` & `dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/python_submissions.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation.py` & `dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/relation.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 Self = TypeVar("Self", bound="BigQueryRelation")
 
 
 @dataclass(frozen=True, eq=False, repr=False)
 class BigQueryRelation(BaseRelation):
     quote_character: str = "`"
     location: Optional[str] = None
+    require_alias: bool = False
 
     renameable_relations: FrozenSet[RelationType] = field(
         default_factory=lambda: frozenset(
             {
                 RelationType.Table,
             }
         )
```

### Comparing `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation_configs/__init__.py` & `dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/relation_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation_configs/_base.py` & `dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/relation_configs/_base.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation_configs/_cluster.py` & `dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/relation_configs/_cluster.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation_configs/_materialized_view.py` & `dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/relation_configs/_materialized_view.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation_configs/_options.py` & `dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/relation_configs/_options.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/relation_configs/_partition.py` & `dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/relation_configs/_partition.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/adapters/bigquery/utility.py` & `dbt_bigquery-1.8.0rc1/dbt/adapters/bigquery/utility.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/adapters/apply_grants.sql` & `dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/adapters.sql` & `dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/catalog/by_relation.sql` & `dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/catalog/by_relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/catalog/by_schema.sql` & `dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/catalog/by_schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/catalog/catalog.sql` & `dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/catalog/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/copy.sql` & `dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/materializations/copy.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/incremental.sql` & `dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/incremental_strategy/common.sql` & `dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/common.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/incremental_strategy/insert_overwrite.sql` & `dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/insert_overwrite.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/incremental_strategy/merge.sql` & `dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/incremental_strategy/time_ingestion_tables.sql` & `dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/materializations/incremental_strategy/time_ingestion_tables.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/seed.sql` & `dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/table.sql` & `dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/materializations/view.sql` & `dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/materialized_view/alter.sql` & `dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/relations/materialized_view/alter.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/materialized_view/create.sql` & `dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/relations/materialized_view/create.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/materialized_view/replace.sql` & `dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/relations/materialized_view/replace.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/partition.sql` & `dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/relations/partition.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/relations/view/replace.sql` & `dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/relations/view/replace.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/get_columns_spec_ddl.sql` & `dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/utils/get_columns_spec_ddl.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/safe_cast.sql` & `dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/utils/safe_cast.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/include/bigquery/macros/utils/split_part.sql` & `dbt_bigquery-1.8.0rc1/dbt/include/bigquery/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt/include/bigquery/profile_template.yml` & `dbt_bigquery-1.8.0rc1/dbt/include/bigquery/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.8.0b2/dbt_bigquery.egg-info/PKG-INFO` & `dbt_bigquery-1.8.0rc1/dbt_bigquery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-bigquery
-Version: 1.8.0b2
+Version: 1.8.0rc1
 Summary: The Bigquery adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-bigquery
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
-Metadata-Version: 2.1 Name: dbt-bigquery Version: 1.8.0b2 Summary: The Bigquery
-adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-bigquery
-Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
-:: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
-License Classifier: Operating System :: Microsoft :: Windows Classifier:
-Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
-Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE.md Requires-Dist:
-dbt-common<2.0,>=0.1.0a1 Requires-Dist: dbt-adapters<2.0,>=0.1.0a1 Requires-
-Dist: google-cloud-bigquery[pandas]<4.0,>=3.0 Requires-Dist: google-cloud-
-storage~=2.4 Requires-Dist: google-cloud-dataproc~=5.0 Requires-Dist: google-
-api-core>=2.11.0 Requires-Dist: dbt-core>=1.8.0a1
+Metadata-Version: 2.1 Name: dbt-bigquery Version: 1.8.0rc1 Summary: The
+Bigquery adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
+bigquery Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+:: Apache Software License Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
+:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Python: >=3.8 Description-Content-Type: text/markdown License-File: LICENSE.md
+Requires-Dist: dbt-common<2.0,>=0.1.0a1 Requires-Dist: dbt-
+adapters<2.0,>=0.1.0a1 Requires-Dist: google-cloud-bigquery[pandas]<4.0,>=3.0
+Requires-Dist: google-cloud-storage~=2.4 Requires-Dist: google-cloud-
+dataproc~=5.0 Requires-Dist: google-api-core>=2.11.0 Requires-Dist: dbt-
+core>=1.8.0a1
                                   [dbt logo]
                   _[_U_n_i_t_ _T_e_s_t_s_ _B_a_d_g_e_]_[_I_n_t_e_g_r_a_t_i_o_n_ _T_e_s_t_s_ _B_a_d_g_e_]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-bigquery The `dbt-bigquery` package contains all of
```

### Comparing `dbt-bigquery-1.8.0b2/dbt_bigquery.egg-info/SOURCES.txt` & `dbt_bigquery-1.8.0rc1/dbt_bigquery.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 dbt/include/bigquery/macros/utils/hash.sql
 dbt/include/bigquery/macros/utils/intersect.sql
 dbt/include/bigquery/macros/utils/listagg.sql
 dbt/include/bigquery/macros/utils/position.sql
 dbt/include/bigquery/macros/utils/right.sql
 dbt/include/bigquery/macros/utils/safe_cast.sql
 dbt/include/bigquery/macros/utils/split_part.sql
+dbt/include/bigquery/macros/utils/string_literal.sql
 dbt/include/bigquery/macros/utils/timestamps.sql
 dbt_bigquery.egg-info/PKG-INFO
 dbt_bigquery.egg-info/SOURCES.txt
 dbt_bigquery.egg-info/dependency_links.txt
 dbt_bigquery.egg-info/not-zip-safe
 dbt_bigquery.egg-info/requires.txt
 dbt_bigquery.egg-info/top_level.txt
```

### Comparing `dbt-bigquery-1.8.0b2/setup.py` & `dbt_bigquery-1.8.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     """
     attributes = {}
     exec(VERSION.read_text(), attributes)
     return attributes["version"]
 
 
 package_name = "dbt-bigquery"
-package_version = "1.8.0b2"
+package_version = "1.8.0rc1"
 description = """The BigQuery adapter plugin for dbt"""
 
 setup(
     name="dbt-bigquery",
     version=_dbt_bigquery_version(),
     description="The Bigquery adapter plugin for dbt",
     long_description=README.read_text(),
```

