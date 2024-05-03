# Comparing `tmp/dbt_redshift-1.8.0b3.tar.gz` & `tmp/dbt_redshift-1.8.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_redshift-1.8.0b3.tar", last modified: Fri Apr 19 00:18:32 2024, max compression
+gzip compressed data, was "dbt_redshift-1.8.0rc1.tar", last modified: Fri May  3 23:29:24 2024, max compression
```

## Comparing `dbt_redshift-1.8.0b3.tar` & `dbt_redshift-1.8.0rc1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:18:32.454103 dbt_redshift-1.8.0b3/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-19 00:18:32.454103 dbt_redshift-1.8.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:18:32.442103 dbt_redshift-1.8.0b3/dbt/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:18:32.438103 dbt_redshift-1.8.0b3/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:18:32.442103 dbt_redshift-1.8.0b3/dbt/adapters/redshift/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/adapters/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/adapters/redshift/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13442 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/adapters/redshift/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/adapters/redshift/impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/adapters/redshift/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:18:32.446103 dbt_redshift-1.8.0b3/dbt/adapters/redshift/relation_configs/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/adapters/redshift/relation_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/adapters/redshift/relation_configs/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/adapters/redshift/relation_configs/dist.py
--rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/adapters/redshift/relation_configs/materialized_view.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/adapters/redshift/relation_configs/policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/adapters/redshift/relation_configs/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/adapters/redshift/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:18:32.442103 dbt_redshift-1.8.0b3/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:18:32.446103 dbt_redshift-1.8.0b3/dbt/include/redshift/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:18:32.446103 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:18:32.446103 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (127)     9030 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/adapters.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:18:32.446103 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/catalog/by_relation.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/catalog/by_schema.sql
--rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/catalog/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:18:32.446103 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/materializations/incremental_merge.sql
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/materializations/materialized_view.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:18:32.446103 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/materializations/seeds/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/materializations/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:18:32.446103 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/metadata/relation_last_modified.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:18:32.442103 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/relations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:18:32.450103 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/relations/materialized_view/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/relations/materialized_view/alter.sql
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/relations/materialized_view/create.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/relations/materialized_view/describe.sql
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/relations/materialized_view/drop.sql
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/relations/materialized_view/refresh.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:18:32.450103 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/relations/table/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/relations/table/drop.sql
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/relations/table/rename.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:18:32.450103 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/relations/view/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/relations/view/drop.sql
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/relations/view/rename.sql
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/relations/view/replace.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/relations.sql
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:18:32.450103 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/utils/length.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/dbt/include/redshift/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:18:32.454103 dbt_redshift-1.8.0b3/dbt_redshift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-19 00:18:32.000000 dbt_redshift-1.8.0b3/dbt_redshift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-19 00:18:32.000000 dbt_redshift-1.8.0b3/dbt_redshift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 00:18:32.000000 dbt_redshift-1.8.0b3/dbt_redshift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 00:18:32.000000 dbt_redshift-1.8.0b3/dbt_redshift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-19 00:18:32.000000 dbt_redshift-1.8.0b3/dbt_redshift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-19 00:18:32.000000 dbt_redshift-1.8.0b3/dbt_redshift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 00:18:32.454103 dbt_redshift-1.8.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-19 00:18:21.000000 dbt_redshift-1.8.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:29:24.443709 dbt_redshift-1.8.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-03 23:29:24.443709 dbt_redshift-1.8.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:29:24.435709 dbt_redshift-1.8.0rc1/dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:29:24.431709 dbt_redshift-1.8.0rc1/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:29:24.435709 dbt_redshift-1.8.0rc1/dbt/adapters/redshift/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/adapters/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/adapters/redshift/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13460 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/adapters/redshift/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/adapters/redshift/impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/adapters/redshift/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:29:24.435709 dbt_redshift-1.8.0rc1/dbt/adapters/redshift/relation_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/adapters/redshift/relation_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/adapters/redshift/relation_configs/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/adapters/redshift/relation_configs/dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10744 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/adapters/redshift/relation_configs/materialized_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/adapters/redshift/relation_configs/policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/adapters/redshift/relation_configs/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/adapters/redshift/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:29:24.431709 dbt_redshift-1.8.0rc1/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:29:24.435709 dbt_redshift-1.8.0rc1/dbt/include/redshift/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:29:24.439710 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:29:24.439710 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     9030 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/adapters.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:29:24.439710 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/catalog/by_relation.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/catalog/by_schema.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/catalog/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:29:24.439710 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/materializations/incremental_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/materializations/materialized_view.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:29:24.439710 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/materializations/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:29:24.439710 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/metadata/relation_last_modified.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:29:24.431709 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/relations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:29:24.439710 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/relations/materialized_view/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/relations/materialized_view/alter.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/relations/materialized_view/create.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/relations/materialized_view/describe.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/relations/materialized_view/drop.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/relations/materialized_view/refresh.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:29:24.439710 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/relations/table/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/relations/table/drop.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/relations/table/rename.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:29:24.443709 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/relations/view/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/relations/view/drop.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/relations/view/rename.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/relations/view/replace.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/relations.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:29:24.443709 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/dbt/include/redshift/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:29:24.443709 dbt_redshift-1.8.0rc1/dbt_redshift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-03 23:29:24.000000 dbt_redshift-1.8.0rc1/dbt_redshift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-03 23:29:24.000000 dbt_redshift-1.8.0rc1/dbt_redshift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 23:29:24.000000 dbt_redshift-1.8.0rc1/dbt_redshift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 23:29:24.000000 dbt_redshift-1.8.0rc1/dbt_redshift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-03 23:29:24.000000 dbt_redshift-1.8.0rc1/dbt_redshift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-03 23:29:24.000000 dbt_redshift-1.8.0rc1/dbt_redshift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 23:29:24.443709 dbt_redshift-1.8.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-03 23:29:14.000000 dbt_redshift-1.8.0rc1/setup.py
```

### Comparing `dbt_redshift-1.8.0b3/LICENSE.md` & `dbt_redshift-1.8.0rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt_redshift-1.8.0b3/PKG-INFO` & `dbt_redshift-1.8.0rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-redshift
-Version: 1.8.0b3
+Version: 1.8.0rc1
 Summary: The Redshift adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-redshift
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: dbt-common<2.0,>=0.1.0a1
 Requires-Dist: dbt-adapters<2.0,>=0.1.0a1
-Requires-Dist: dbt-postgres~=1.8.0b3
+Requires-Dist: dbt-postgres~=1.8.0rc1
 Requires-Dist: redshift-connector!=2.0.914,<2.0.918,>=2.0.913
 Requires-Dist: dbt-core>=1.8.0b3
 Requires-Dist: sqlparse<0.6.0,>=0.5.0
 Requires-Dist: agate
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="500"/>
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: dbt-redshift Version: 1.8.0b3 Summary: The Redshift
-adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-redshift
-Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
-:: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
-License Classifier: Operating System :: Microsoft :: Windows Classifier:
-Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
-Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE.md Requires-Dist:
-dbt-common<2.0,>=0.1.0a1 Requires-Dist: dbt-adapters<2.0,>=0.1.0a1 Requires-
-Dist: dbt-postgres~=1.8.0b3 Requires-Dist: redshift-
-connector!=2.0.914,<2.0.918,>=2.0.913 Requires-Dist: dbt-core>=1.8.0b3
+Metadata-Version: 2.1 Name: dbt-redshift Version: 1.8.0rc1 Summary: The
+Redshift adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
+redshift Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+:: Apache Software License Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
+:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Python: >=3.8 Description-Content-Type: text/markdown License-File: LICENSE.md
+Requires-Dist: dbt-common<2.0,>=0.1.0a1 Requires-Dist: dbt-
+adapters<2.0,>=0.1.0a1 Requires-Dist: dbt-postgres~=1.8.0rc1 Requires-Dist:
+redshift-connector!=2.0.914,<2.0.918,>=2.0.913 Requires-Dist: dbt-core>=1.8.0b3
 Requires-Dist: sqlparse<0.6.0,>=0.5.0 Requires-Dist: agate
                                   [dbt logo]
                   _[_U_n_i_t_ _T_e_s_t_s_ _B_a_d_g_e_]_[_I_n_t_e_g_r_a_t_i_o_n_ _T_e_s_t_s_ _B_a_d_g_e_]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
```

### Comparing `dbt_redshift-1.8.0b3/README.md` & `dbt_redshift-1.8.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt_redshift-1.8.0b3/dbt/adapters/redshift/__init__.py` & `dbt_redshift-1.8.0rc1/dbt/adapters/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_redshift-1.8.0b3/dbt/adapters/redshift/connections.py` & `dbt_redshift-1.8.0rc1/dbt/adapters/redshift/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,29 +46,29 @@
     require = "require"
     verify_ca = "verify-ca"
     verify_full = "verify-full"
 
     @classmethod
     def default(cls) -> "UserSSLMode":
         # default for `psycopg2`, which aligns with dbt-redshift 1.4 and provides backwards compatibility
-        return cls.prefer
+        return cls("prefer")
 
 
 class RedshiftSSLMode(StrEnum):
     verify_ca = "verify-ca"
     verify_full = "verify-full"
 
 
 SSL_MODE_TRANSLATION = {
     UserSSLMode.disable: None,
-    UserSSLMode.allow: RedshiftSSLMode.verify_ca,
-    UserSSLMode.prefer: RedshiftSSLMode.verify_ca,
-    UserSSLMode.require: RedshiftSSLMode.verify_ca,
-    UserSSLMode.verify_ca: RedshiftSSLMode.verify_ca,
-    UserSSLMode.verify_full: RedshiftSSLMode.verify_full,
+    UserSSLMode.allow: RedshiftSSLMode("verify-ca"),
+    UserSSLMode.prefer: RedshiftSSLMode("verify-ca"),
+    UserSSLMode.require: RedshiftSSLMode("verify-ca"),
+    UserSSLMode.verify_ca: RedshiftSSLMode("verify-ca"),
+    UserSSLMode.verify_full: RedshiftSSLMode("verify-full"),
 }
 
 
 @dataclass
 class RedshiftSSLConfig(dbtClassMixin, Replaceable):  # type: ignore
     ssl: bool = True
     sslmode: Optional[RedshiftSSLMode] = SSL_MODE_TRANSLATION[UserSSLMode.default()]
```

### Comparing `dbt_redshift-1.8.0b3/dbt/adapters/redshift/impl.py` & `dbt_redshift-1.8.0rc1/dbt/adapters/redshift/impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         ConstraintType.foreign_key: ConstraintSupport.NOT_ENFORCED,
     }
 
     _capabilities = CapabilityDict(
         {
             Capability.SchemaMetadataByRelations: CapabilitySupport(support=Support.Full),
             Capability.TableLastModifiedMetadata: CapabilitySupport(support=Support.Full),
+            Capability.TableLastModifiedMetadataBatch: CapabilitySupport(support=Support.Full),
         }
     )
 
     @classmethod
     def date_function(cls):
         return "getdate()"
```

### Comparing `dbt_redshift-1.8.0b3/dbt/adapters/redshift/relation.py` & `dbt_redshift-1.8.0rc1/dbt/adapters/redshift/relation.py`

 * *Files identical despite different names*

### Comparing `dbt_redshift-1.8.0b3/dbt/adapters/redshift/relation_configs/__init__.py` & `dbt_redshift-1.8.0rc1/dbt/adapters/redshift/relation_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_redshift-1.8.0b3/dbt/adapters/redshift/relation_configs/base.py` & `dbt_redshift-1.8.0rc1/dbt/adapters/redshift/relation_configs/base.py`

 * *Files identical despite different names*

### Comparing `dbt_redshift-1.8.0b3/dbt/adapters/redshift/relation_configs/dist.py` & `dbt_redshift-1.8.0rc1/dbt/adapters/redshift/relation_configs/dist.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     auto = "auto"
     even = "even"
     all = "all"
     key = "key"
 
     @classmethod
     def default(cls) -> "RedshiftDistStyle":
-        return cls.auto
+        return cls("auto")
 
 
 @dataclass(frozen=True, eq=True, unsafe_hash=True)
 class RedshiftDistConfig(RedshiftRelationConfigBase, RelationConfigValidationMixin):
     """
     This config fallows the specs found here:
     https://docs.aws.amazon.com/redshift/latest/dg/r_CREATE_TABLE_NEW.html
@@ -99,15 +99,15 @@
             RedshiftDistStyle.auto,
             RedshiftDistStyle.even,
             RedshiftDistStyle.all,
         ):
             config = {"diststyle": diststyle}
 
         else:
-            config = {"diststyle": RedshiftDistStyle.key.value, "distkey": dist}
+            config = {"diststyle": RedshiftDistStyle.key.value, "distkey": dist}  # type: ignore
 
         return config
 
     @classmethod
     def parse_relation_results(cls, relation_results_entry: agate.Row) -> Dict:
         """
         Translate agate objects from the database into a standard dictionary.
```

### Comparing `dbt_redshift-1.8.0b3/dbt/adapters/redshift/relation_configs/materialized_view.py` & `dbt_redshift-1.8.0rc1/dbt/adapters/redshift/relation_configs/materialized_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     """
 
     mv_name: str
     schema_name: str
     database_name: str
     query: str
     backup: bool = field(default=True, compare=False, hash=False)
-    dist: RedshiftDistConfig = RedshiftDistConfig(diststyle=RedshiftDistStyle.even)
+    dist: RedshiftDistConfig = RedshiftDistConfig(diststyle=RedshiftDistStyle("even"))
     sort: RedshiftSortConfig = RedshiftSortConfig()
     autorefresh: bool = False
 
     @property
     def path(self) -> str:
         return ".".join(
             part
```

### Comparing `dbt_redshift-1.8.0b3/dbt/adapters/redshift/relation_configs/sort.py` & `dbt_redshift-1.8.0rc1/dbt/adapters/redshift/relation_configs/sort.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 class RedshiftSortStyle(StrEnum):
     auto = "auto"
     compound = "compound"
     interleaved = "interleaved"
 
     @classmethod
     def default(cls) -> "RedshiftSortStyle":
-        return cls.auto
+        return cls("auto")
 
     @classmethod
     def default_with_columns(cls) -> "RedshiftSortStyle":
-        return cls.compound
+        return cls("compound")
 
 
 @dataclass(frozen=True, eq=True, unsafe_hash=True)
 class RedshiftSortConfig(RedshiftRelationConfigBase, RelationConfigValidationMixin):
     """
     This config fallows the specs found here:
     https://docs.aws.amazon.com/redshift/latest/dg/r_CREATE_TABLE_NEW.html
```

### Comparing `dbt_redshift-1.8.0b3/dbt/adapters/redshift/utility.py` & `dbt_redshift-1.8.0rc1/dbt/adapters/redshift/utility.py`

 * *Files identical despite different names*

### Comparing `dbt_redshift-1.8.0b3/dbt/include/redshift/macros/adapters/apply_grants.sql` & `dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt_redshift-1.8.0b3/dbt/include/redshift/macros/adapters.sql` & `dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt_redshift-1.8.0b3/dbt/include/redshift/macros/catalog/by_relation.sql` & `dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/catalog/by_relation.sql`

 * *Files identical despite different names*

### Comparing `dbt_redshift-1.8.0b3/dbt/include/redshift/macros/catalog/by_schema.sql` & `dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/catalog/by_schema.sql`

 * *Files identical despite different names*

### Comparing `dbt_redshift-1.8.0b3/dbt/include/redshift/macros/catalog/catalog.sql` & `dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/catalog/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt_redshift-1.8.0b3/dbt/include/redshift/macros/materializations/incremental_merge.sql` & `dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/materializations/incremental_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt_redshift-1.8.0b3/dbt/include/redshift/macros/materializations/seeds/helpers.sql` & `dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_redshift-1.8.0b3/dbt/include/redshift/macros/materializations/table.sql` & `dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt_redshift-1.8.0b3/dbt/include/redshift/macros/materializations/view.sql` & `dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt_redshift-1.8.0b3/dbt/include/redshift/macros/metadata/relation_last_modified.sql` & `dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/metadata/relation_last_modified.sql`

 * *Files identical despite different names*

### Comparing `dbt_redshift-1.8.0b3/dbt/include/redshift/macros/relations/materialized_view/alter.sql` & `dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/relations/materialized_view/alter.sql`

 * *Files identical despite different names*

### Comparing `dbt_redshift-1.8.0b3/dbt/include/redshift/macros/relations/materialized_view/create.sql` & `dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/relations/materialized_view/create.sql`

 * *Files identical despite different names*

### Comparing `dbt_redshift-1.8.0b3/dbt/include/redshift/macros/relations/materialized_view/describe.sql` & `dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/relations/materialized_view/describe.sql`

 * *Files identical despite different names*

### Comparing `dbt_redshift-1.8.0b3/dbt/include/redshift/macros/relations/view/replace.sql` & `dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/relations/view/replace.sql`

 * *Files identical despite different names*

### Comparing `dbt_redshift-1.8.0b3/dbt/include/redshift/macros/relations.sql` & `dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/relations.sql`

 * *Files identical despite different names*

### Comparing `dbt_redshift-1.8.0b3/dbt/include/redshift/macros/utils/listagg.sql` & `dbt_redshift-1.8.0rc1/dbt/include/redshift/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt_redshift-1.8.0b3/dbt/include/redshift/profile_template.yml` & `dbt_redshift-1.8.0rc1/dbt/include/redshift/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt_redshift-1.8.0b3/dbt_redshift.egg-info/PKG-INFO` & `dbt_redshift-1.8.0rc1/dbt_redshift.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-redshift
-Version: 1.8.0b3
+Version: 1.8.0rc1
 Summary: The Redshift adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-redshift
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: dbt-common<2.0,>=0.1.0a1
 Requires-Dist: dbt-adapters<2.0,>=0.1.0a1
-Requires-Dist: dbt-postgres~=1.8.0b3
+Requires-Dist: dbt-postgres~=1.8.0rc1
 Requires-Dist: redshift-connector!=2.0.914,<2.0.918,>=2.0.913
 Requires-Dist: dbt-core>=1.8.0b3
 Requires-Dist: sqlparse<0.6.0,>=0.5.0
 Requires-Dist: agate
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="500"/>
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: dbt-redshift Version: 1.8.0b3 Summary: The Redshift
-adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-redshift
-Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
-:: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
-License Classifier: Operating System :: Microsoft :: Windows Classifier:
-Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
-Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE.md Requires-Dist:
-dbt-common<2.0,>=0.1.0a1 Requires-Dist: dbt-adapters<2.0,>=0.1.0a1 Requires-
-Dist: dbt-postgres~=1.8.0b3 Requires-Dist: redshift-
-connector!=2.0.914,<2.0.918,>=2.0.913 Requires-Dist: dbt-core>=1.8.0b3
+Metadata-Version: 2.1 Name: dbt-redshift Version: 1.8.0rc1 Summary: The
+Redshift adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
+redshift Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+:: Apache Software License Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
+:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Python: >=3.8 Description-Content-Type: text/markdown License-File: LICENSE.md
+Requires-Dist: dbt-common<2.0,>=0.1.0a1 Requires-Dist: dbt-
+adapters<2.0,>=0.1.0a1 Requires-Dist: dbt-postgres~=1.8.0rc1 Requires-Dist:
+redshift-connector!=2.0.914,<2.0.918,>=2.0.913 Requires-Dist: dbt-core>=1.8.0b3
 Requires-Dist: sqlparse<0.6.0,>=0.5.0 Requires-Dist: agate
                                   [dbt logo]
                   _[_U_n_i_t_ _T_e_s_t_s_ _B_a_d_g_e_]_[_I_n_t_e_g_r_a_t_i_o_n_ _T_e_s_t_s_ _B_a_d_g_e_]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
```

### Comparing `dbt_redshift-1.8.0b3/dbt_redshift.egg-info/SOURCES.txt` & `dbt_redshift-1.8.0rc1/dbt_redshift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt_redshift-1.8.0b3/setup.py` & `dbt_redshift-1.8.0rc1/setup.py`

 * *Files identical despite different names*

