# Comparing `tmp/dragonfly-schema-1.9.8.tar.gz` & `tmp/dragonfly-schema-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dragonfly-schema-1.9.8.tar", last modified: Wed Jan  3 20:48:56 2024, max compression
+gzip compressed data, was "dist/dragonfly-schema-1.9.9.tar", last modified: Fri Jan 26 03:49:08 2024, max compression
```

## Comparing `dragonfly-schema-1.9.8.tar` & `dragonfly-schema-1.9.9.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:48:56.000000 dragonfly-schema-1.9.8/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:48:56.000000 dragonfly-schema-1.9.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:48:56.000000 dragonfly-schema-1.9.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/.github/workflows/dependency-release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-01-03 20:48:56.000000 dragonfly-schema-1.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:48:56.000000 dragonfly-schema-1.9.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/docs/model.html
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/docs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:48:56.000000 dragonfly-schema-1.9.8/dragonfly_schema/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/dragonfly_schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:48:56.000000 dragonfly-schema-1.9.8/dragonfly_schema/energy/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/dragonfly_schema/energy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/dragonfly_schema/energy/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    13445 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/dragonfly_schema/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:48:56.000000 dragonfly-schema-1.9.8/dragonfly_schema/radiance/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/dragonfly_schema/radiance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/dragonfly_schema/radiance/gridpar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/dragonfly_schema/radiance/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/dragonfly_schema/roof.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/dragonfly_schema/shading_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/dragonfly_schema/skylight_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9649 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/dragonfly_schema/window_parameter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:48:56.000000 dragonfly-schema-1.9.8/dragonfly_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-01-03 20:48:56.000000 dragonfly-schema-1.9.8/dragonfly_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-01-03 20:48:56.000000 dragonfly-schema-1.9.8/dragonfly_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-03 20:48:56.000000 dragonfly-schema-1.9.8/dragonfly_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-03 20:48:56.000000 dragonfly-schema-1.9.8/dragonfly_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-03 20:48:56.000000 dragonfly-schema-1.9.8/dragonfly_schema.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:48:56.000000 dragonfly-schema-1.9.8/samples/
--rw-r--r--   0 runner    (1001) docker     (127)    22598 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/samples/building_simple.json
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/samples/context_shade_two_tree_canopy.json
--rw-r--r--   0 runner    (1001) docker     (127)    90404 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/samples/model_complete_simple.dfjson
--rw-r--r--   0 runner    (1001) docker     (127)   112149 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/samples/model_with_doors_skylights.dfjson
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/samples/room2d_simple.json
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/samples/shading_par_extruded_border.json
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/samples/shading_par_louvers_by_count.json
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/samples/shading_par_louvers_by_distance.json
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/samples/shading_par_overhang.json
--rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/samples/story_air_boundary.json
--rw-r--r--   0 runner    (1001) docker     (127)     9468 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/samples/story_simple.json
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/samples/window_par_detailed_rectangular_windows.json
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/samples/window_par_detailed_windows.json
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/samples/window_par_repeating_window_ratio.json
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/samples/window_par_repeating_window_width_height.json
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/samples/window_par_simple_window_ratio.json
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/samples/window_par_single_window.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:48:56.000000 dragonfly-schema-1.9.8/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/scripts/export_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     9703 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/scripts/sample_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/scripts/sample_shading_par.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/scripts/sample_window_par.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-03 20:48:56.000000 dragonfly-schema-1.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:48:56.000000 dragonfly-schema-1.9.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/tests/test_openapi_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/tests/test_shading_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-01-03 20:47:43.000000 dragonfly-schema-1.9.8/tests/test_window_parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 03:49:08.000000 dragonfly-schema-1.9.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 03:49:07.000000 dragonfly-schema-1.9.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 03:49:07.000000 dragonfly-schema-1.9.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/.github/workflows/dependency-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-01-26 03:49:08.000000 dragonfly-schema-1.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 03:49:07.000000 dragonfly-schema-1.9.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/docs/model.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/docs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 03:49:07.000000 dragonfly-schema-1.9.9/dragonfly_schema/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/dragonfly_schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 03:49:07.000000 dragonfly-schema-1.9.9/dragonfly_schema/energy/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/dragonfly_schema/energy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/dragonfly_schema/energy/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13445 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/dragonfly_schema/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 03:49:07.000000 dragonfly-schema-1.9.9/dragonfly_schema/radiance/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/dragonfly_schema/radiance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/dragonfly_schema/radiance/gridpar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/dragonfly_schema/radiance/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/dragonfly_schema/roof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/dragonfly_schema/shading_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/dragonfly_schema/skylight_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9649 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/dragonfly_schema/window_parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 03:49:07.000000 dragonfly-schema-1.9.9/dragonfly_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-01-26 03:49:07.000000 dragonfly-schema-1.9.9/dragonfly_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-01-26 03:49:07.000000 dragonfly-schema-1.9.9/dragonfly_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 03:49:07.000000 dragonfly-schema-1.9.9/dragonfly_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-26 03:49:07.000000 dragonfly-schema-1.9.9/dragonfly_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-26 03:49:07.000000 dragonfly-schema-1.9.9/dragonfly_schema.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 03:49:08.000000 dragonfly-schema-1.9.9/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)    22598 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/samples/building_simple.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/samples/context_shade_two_tree_canopy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    90404 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/samples/model_complete_simple.dfjson
+-rw-r--r--   0 runner    (1001) docker     (127)  1460160 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/samples/model_multiple_buildings.dfjson
+-rw-r--r--   0 runner    (1001) docker     (127)   112149 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/samples/model_with_doors_skylights.dfjson
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/samples/room2d_simple.json
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/samples/shading_par_extruded_border.json
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/samples/shading_par_louvers_by_count.json
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/samples/shading_par_louvers_by_distance.json
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/samples/shading_par_overhang.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/samples/story_air_boundary.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9468 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/samples/story_simple.json
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/samples/window_par_detailed_rectangular_windows.json
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/samples/window_par_detailed_windows.json
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/samples/window_par_repeating_window_ratio.json
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/samples/window_par_repeating_window_width_height.json
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/samples/window_par_simple_window_ratio.json
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/samples/window_par_single_window.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 03:49:08.000000 dragonfly-schema-1.9.9/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/scripts/export_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9703 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/scripts/sample_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/scripts/sample_shading_par.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/scripts/sample_window_par.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-26 03:49:08.000000 dragonfly-schema-1.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 03:49:08.000000 dragonfly-schema-1.9.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/tests/test_openapi_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/tests/test_shading_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-01-26 03:47:51.000000 dragonfly-schema-1.9.9/tests/test_window_parameter.py
```

### Comparing `dragonfly-schema-1.9.8/.github/workflows/ci.yaml` & `dragonfly-schema-1.9.9/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/.github/workflows/dependency-release.yaml` & `dragonfly-schema-1.9.9/.github/workflows/dependency-release.yaml`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/.releaserc.json` & `dragonfly-schema-1.9.9/.releaserc.json`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/LICENSE` & `dragonfly-schema-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/PKG-INFO` & `dragonfly-schema-1.9.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonfly-schema
-Version: 1.9.8
+Version: 1.9.9
 Summary: Dragonfly Data-Model Objects
 Home-page: https://github.com/ladybug-tools/dragonfly-schema
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
```

### Comparing `dragonfly-schema-1.9.8/README.md` & `dragonfly-schema-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/docs/index.html` & `dragonfly-schema-1.9.9/docs/index.html`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/docs/model.html` & `dragonfly-schema-1.9.9/docs/model.html`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/docs.py` & `dragonfly-schema-1.9.9/docs.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/dragonfly_schema/energy/properties.py` & `dragonfly-schema-1.9.9/dragonfly_schema/energy/properties.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/dragonfly_schema/model.py` & `dragonfly-schema-1.9.9/dragonfly_schema/model.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/dragonfly_schema/radiance/gridpar.py` & `dragonfly-schema-1.9.9/dragonfly_schema/radiance/gridpar.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/dragonfly_schema/radiance/properties.py` & `dragonfly-schema-1.9.9/dragonfly_schema/radiance/properties.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/dragonfly_schema/roof.py` & `dragonfly-schema-1.9.9/dragonfly_schema/roof.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/dragonfly_schema/shading_parameter.py` & `dragonfly-schema-1.9.9/dragonfly_schema/shading_parameter.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/dragonfly_schema/skylight_parameter.py` & `dragonfly-schema-1.9.9/dragonfly_schema/skylight_parameter.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/dragonfly_schema/window_parameter.py` & `dragonfly-schema-1.9.9/dragonfly_schema/window_parameter.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/dragonfly_schema.egg-info/PKG-INFO` & `dragonfly-schema-1.9.9/dragonfly_schema.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonfly-schema
-Version: 1.9.8
+Version: 1.9.9
 Summary: Dragonfly Data-Model Objects
 Home-page: https://github.com/ladybug-tools/dragonfly-schema
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
```

### Comparing `dragonfly-schema-1.9.8/dragonfly_schema.egg-info/SOURCES.txt` & `dragonfly-schema-1.9.9/dragonfly_schema.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 dragonfly_schema/energy/properties.py
 dragonfly_schema/radiance/__init__.py
 dragonfly_schema/radiance/gridpar.py
 dragonfly_schema/radiance/properties.py
 samples/building_simple.json
 samples/context_shade_two_tree_canopy.json
 samples/model_complete_simple.dfjson
+samples/model_multiple_buildings.dfjson
 samples/model_with_doors_skylights.dfjson
 samples/room2d_simple.json
 samples/shading_par_extruded_border.json
 samples/shading_par_louvers_by_count.json
 samples/shading_par_louvers_by_distance.json
 samples/shading_par_overhang.json
 samples/story_air_boundary.json
```

### Comparing `dragonfly-schema-1.9.8/samples/building_simple.json` & `dragonfly-schema-1.9.9/samples/building_simple.json`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/samples/context_shade_two_tree_canopy.json` & `dragonfly-schema-1.9.9/samples/context_shade_two_tree_canopy.json`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/samples/model_complete_simple.dfjson` & `dragonfly-schema-1.9.9/samples/model_complete_simple.dfjson`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/samples/model_with_doors_skylights.dfjson` & `dragonfly-schema-1.9.9/samples/model_with_doors_skylights.dfjson`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/samples/room2d_simple.json` & `dragonfly-schema-1.9.9/samples/room2d_simple.json`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/samples/story_air_boundary.json` & `dragonfly-schema-1.9.9/samples/story_air_boundary.json`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/samples/story_simple.json` & `dragonfly-schema-1.9.9/samples/story_simple.json`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/samples/window_par_detailed_windows.json` & `dragonfly-schema-1.9.9/samples/window_par_detailed_windows.json`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/scripts/export_samples.py` & `dragonfly-schema-1.9.9/scripts/export_samples.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/scripts/sample_model.py` & `dragonfly-schema-1.9.9/scripts/sample_model.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/scripts/sample_shading_par.py` & `dragonfly-schema-1.9.9/scripts/sample_shading_par.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/scripts/sample_window_par.py` & `dragonfly-schema-1.9.9/scripts/sample_window_par.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/setup.py` & `dragonfly-schema-1.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/tests/test_model.py` & `dragonfly-schema-1.9.9/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/tests/test_shading_parameter.py` & `dragonfly-schema-1.9.9/tests/test_shading_parameter.py`

 * *Files identical despite different names*

### Comparing `dragonfly-schema-1.9.8/tests/test_window_parameter.py` & `dragonfly-schema-1.9.9/tests/test_window_parameter.py`

 * *Files identical despite different names*

