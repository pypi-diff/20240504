# Comparing `tmp/beat-2.0.0.tar.gz` & `tmp/beat-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beat-2.0.0.tar", last modified: Mon Mar 25 21:38:53 2024, max compression
+gzip compressed data, was "beat-2.0.1.tar", last modified: Sat May  4 17:39:41 2024, max compression
```

## Comparing `beat-2.0.0.tar` & `beat-2.0.1.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 21:38:53.961927 beat-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-25 21:38:48.000000 beat-2.0.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-03-25 21:38:53.961927 beat-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-03-25 21:38:48.000000 beat-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 21:38:53.953927 beat-2.0.0/beat/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-25 21:38:48.000000 beat-2.0.0/beat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 21:38:53.953927 beat-2.0.0/beat/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 21:38:48.000000 beat-2.0.0/beat/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    87968 2024-03-25 21:38:48.000000 beat-2.0.0/beat/apps/beat.py
--rw-r--r--   0 runner    (1001) docker     (127)    37501 2024-03-25 21:38:48.000000 beat-2.0.0/beat/apps/beatdown.py
--rw-r--r--   0 runner    (1001) docker     (127)    43106 2024-03-25 21:38:48.000000 beat-2.0.0/beat/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    13310 2024-03-25 21:38:48.000000 beat-2.0.0/beat/colormap.py
--rw-r--r--   0 runner    (1001) docker     (127)    77416 2024-03-25 21:38:48.000000 beat-2.0.0/beat/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    28183 2024-03-25 21:38:48.000000 beat-2.0.0/beat/covariance.py
--rw-r--r--   0 runner    (1001) docker     (127)    11005 2024-03-25 21:38:48.000000 beat-2.0.0/beat/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 21:38:53.953927 beat-2.0.0/beat/fast_sweeping/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 21:38:48.000000 beat-2.0.0/beat/fast_sweeping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11315 2024-03-25 21:38:48.000000 beat-2.0.0/beat/fast_sweeping/fast_sweep.py
--rw-r--r--   0 runner    (1001) docker     (127)     9223 2024-03-25 21:38:48.000000 beat-2.0.0/beat/fast_sweeping/fast_sweep_ext.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 21:38:53.953927 beat-2.0.0/beat/ffi/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-25 21:38:48.000000 beat-2.0.0/beat/ffi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38948 2024-03-25 21:38:48.000000 beat-2.0.0/beat/ffi/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    75819 2024-03-25 21:38:48.000000 beat-2.0.0/beat/ffi/fault.py
--rw-r--r--   0 runner    (1001) docker     (127)   145526 2024-03-25 21:38:48.000000 beat-2.0.0/beat/heart.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-25 21:38:53.000000 beat-2.0.0/beat/info.py
--rw-r--r--   0 runner    (1001) docker     (127)    13277 2024-03-25 21:38:48.000000 beat-2.0.0/beat/inputf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 21:38:53.957927 beat-2.0.0/beat/models/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-25 21:38:48.000000 beat-2.0.0/beat/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13399 2024-03-25 21:38:48.000000 beat-2.0.0/beat/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-03-25 21:38:48.000000 beat-2.0.0/beat/models/corrections.py
--rw-r--r--   0 runner    (1001) docker     (127)     9742 2024-03-25 21:38:48.000000 beat-2.0.0/beat/models/distributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    41870 2024-03-25 21:38:48.000000 beat-2.0.0/beat/models/geodetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     9110 2024-03-25 21:38:48.000000 beat-2.0.0/beat/models/laplacian.py
--rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-03-25 21:38:48.000000 beat-2.0.0/beat/models/polarity.py
--rw-r--r--   0 runner    (1001) docker     (127)    30370 2024-03-25 21:38:48.000000 beat-2.0.0/beat/models/problems.py
--rw-r--r--   0 runner    (1001) docker     (127)    53281 2024-03-25 21:38:48.000000 beat-2.0.0/beat/models/seismic.py
--rw-r--r--   0 runner    (1001) docker     (127)    13453 2024-03-25 21:38:48.000000 beat-2.0.0/beat/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 21:38:53.957927 beat-2.0.0/beat/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-03-25 21:38:48.000000 beat-2.0.0/beat/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-03-25 21:38:48.000000 beat-2.0.0/beat/plotting/bem.py
--rw-r--r--   0 runner    (1001) docker     (127)    28177 2024-03-25 21:38:48.000000 beat-2.0.0/beat/plotting/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    33419 2024-03-25 21:38:48.000000 beat-2.0.0/beat/plotting/ffi.py
--rw-r--r--   0 runner    (1001) docker     (127)    37639 2024-03-25 21:38:48.000000 beat-2.0.0/beat/plotting/geodetic.py
--rw-r--r--   0 runner    (1001) docker     (127)    33228 2024-03-25 21:38:48.000000 beat-2.0.0/beat/plotting/marginals.py
--rw-r--r--   0 runner    (1001) docker     (127)    89243 2024-03-25 21:38:48.000000 beat-2.0.0/beat/plotting/seismic.py
--rw-r--r--   0 runner    (1001) docker     (127)    19212 2024-03-25 21:38:48.000000 beat-2.0.0/beat/pytensorf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 21:38:53.957927 beat-2.0.0/beat/sampler/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-25 21:38:48.000000 beat-2.0.0/beat/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19567 2024-03-25 21:38:48.000000 beat-2.0.0/beat/sampler/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6655 2024-03-25 21:38:48.000000 beat-2.0.0/beat/sampler/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)    18897 2024-03-25 21:38:48.000000 beat-2.0.0/beat/sampler/metropolis.py
--rw-r--r--   0 runner    (1001) docker     (127)    30456 2024-03-25 21:38:48.000000 beat-2.0.0/beat/sampler/pt.py
--rw-r--r--   0 runner    (1001) docker     (127)    18460 2024-03-25 21:38:48.000000 beat-2.0.0/beat/sampler/smc.py
--rw-r--r--   0 runner    (1001) docker     (127)    20470 2024-03-25 21:38:48.000000 beat-2.0.0/beat/sources.py
--rw-r--r--   0 runner    (1001) docker     (127)     6108 2024-03-25 21:38:48.000000 beat-2.0.0/beat/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (127)    44757 2024-03-25 21:38:48.000000 beat-2.0.0/beat/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 21:38:53.957927 beat-2.0.0/beat/voronoi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 21:38:48.000000 beat-2.0.0/beat/voronoi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-03-25 21:38:48.000000 beat-2.0.0/beat/voronoi/voronoi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-03-25 21:38:48.000000 beat-2.0.0/beat/voronoi/voronoi_ext.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 21:38:53.961927 beat-2.0.0/beat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-03-25 21:38:53.000000 beat-2.0.0/beat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-03-25 21:38:53.000000 beat-2.0.0/beat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 21:38:53.000000 beat-2.0.0/beat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-25 21:38:53.000000 beat-2.0.0/beat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-25 21:38:53.000000 beat-2.0.0/beat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-25 21:38:53.000000 beat-2.0.0/beat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-03-25 21:38:48.000000 beat-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 21:38:53.961927 beat-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-03-25 21:38:48.000000 beat-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 21:38:53.961927 beat-2.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-03-25 21:38:48.000000 beat-2.0.0/test/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-03-25 21:38:48.000000 beat-2.0.0/test/test_bem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-03-25 21:38:48.000000 beat-2.0.0/test/test_composites.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-03-25 21:38:48.000000 beat-2.0.0/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-03-25 21:38:48.000000 beat-2.0.0/test/test_covariance.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-25 21:38:48.000000 beat-2.0.0/test/test_distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-03-25 21:38:48.000000 beat-2.0.0/test/test_fastsweep.py
--rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-03-25 21:38:48.000000 beat-2.0.0/test/test_ffi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-03-25 21:38:48.000000 beat-2.0.0/test/test_ffi_gfstacking.py
--rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-03-25 21:38:48.000000 beat-2.0.0/test/test_ffi_gfstacking_multifault.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-25 21:38:48.000000 beat-2.0.0/test/test_geodetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-03-25 21:38:48.000000 beat-2.0.0/test/test_heart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-03-25 21:38:48.000000 beat-2.0.0/test/test_laplacian.py
--rw-r--r--   0 runner    (1001) docker     (127)     8129 2024-03-25 21:38:48.000000 beat-2.0.0/test/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-03-25 21:38:48.000000 beat-2.0.0/test/test_paripool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-03-25 21:38:48.000000 beat-2.0.0/test/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-25 21:38:48.000000 beat-2.0.0/test/test_proposals.py
--rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-03-25 21:38:48.000000 beat-2.0.0/test/test_pt.py
--rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-03-25 21:38:48.000000 beat-2.0.0/test/test_resolution_subsampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-03-25 21:38:48.000000 beat-2.0.0/test/test_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-03-25 21:38:48.000000 beat-2.0.0/test/test_smc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-03-25 21:38:48.000000 beat-2.0.0/test/test_sources.py
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-03-25 21:38:48.000000 beat-2.0.0/test/test_utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-03-25 21:38:48.000000 beat-2.0.0/test/test_voronoi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:39:41.690363 beat-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-04 17:39:35.000000 beat-2.0.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-05-04 17:39:41.690363 beat-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-05-04 17:39:35.000000 beat-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:39:41.678363 beat-2.0.1/beat/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-04 17:39:35.000000 beat-2.0.1/beat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:39:41.678363 beat-2.0.1/beat/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:39:35.000000 beat-2.0.1/beat/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87983 2024-05-04 17:39:35.000000 beat-2.0.1/beat/apps/beat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37501 2024-05-04 17:39:35.000000 beat-2.0.1/beat/apps/beatdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43073 2024-05-04 17:39:35.000000 beat-2.0.1/beat/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13310 2024-05-04 17:39:35.000000 beat-2.0.1/beat/colormap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77424 2024-05-04 17:39:35.000000 beat-2.0.1/beat/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28179 2024-05-04 17:39:35.000000 beat-2.0.1/beat/covariance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10808 2024-05-04 17:39:35.000000 beat-2.0.1/beat/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:39:41.682363 beat-2.0.1/beat/fast_sweeping/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:39:35.000000 beat-2.0.1/beat/fast_sweeping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11315 2024-05-04 17:39:35.000000 beat-2.0.1/beat/fast_sweeping/fast_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9223 2024-05-04 17:39:35.000000 beat-2.0.1/beat/fast_sweeping/fast_sweep_ext.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:39:41.682363 beat-2.0.1/beat/ffi/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-04 17:39:35.000000 beat-2.0.1/beat/ffi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38948 2024-05-04 17:39:35.000000 beat-2.0.1/beat/ffi/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75819 2024-05-04 17:39:35.000000 beat-2.0.1/beat/ffi/fault.py
+-rw-r--r--   0 runner    (1001) docker     (127)   145921 2024-05-04 17:39:35.000000 beat-2.0.1/beat/heart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-04 17:39:41.000000 beat-2.0.1/beat/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13277 2024-05-04 17:39:35.000000 beat-2.0.1/beat/inputf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:39:41.682363 beat-2.0.1/beat/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-04 17:39:35.000000 beat-2.0.1/beat/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13399 2024-05-04 17:39:35.000000 beat-2.0.1/beat/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-05-04 17:39:35.000000 beat-2.0.1/beat/models/corrections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9742 2024-05-04 17:39:35.000000 beat-2.0.1/beat/models/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41363 2024-05-04 17:39:35.000000 beat-2.0.1/beat/models/geodetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9110 2024-05-04 17:39:35.000000 beat-2.0.1/beat/models/laplacian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-05-04 17:39:35.000000 beat-2.0.1/beat/models/polarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30370 2024-05-04 17:39:35.000000 beat-2.0.1/beat/models/problems.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53281 2024-05-04 17:39:35.000000 beat-2.0.1/beat/models/seismic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13453 2024-05-04 17:39:35.000000 beat-2.0.1/beat/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:39:41.682363 beat-2.0.1/beat/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-04 17:39:35.000000 beat-2.0.1/beat/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-05-04 17:39:35.000000 beat-2.0.1/beat/plotting/bem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28173 2024-05-04 17:39:35.000000 beat-2.0.1/beat/plotting/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33419 2024-05-04 17:39:35.000000 beat-2.0.1/beat/plotting/ffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38009 2024-05-04 17:39:35.000000 beat-2.0.1/beat/plotting/geodetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33228 2024-05-04 17:39:35.000000 beat-2.0.1/beat/plotting/marginals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89243 2024-05-04 17:39:35.000000 beat-2.0.1/beat/plotting/seismic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19221 2024-05-04 17:39:35.000000 beat-2.0.1/beat/pytensorf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:39:41.686363 beat-2.0.1/beat/sampler/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-04 17:39:35.000000 beat-2.0.1/beat/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19567 2024-05-04 17:39:35.000000 beat-2.0.1/beat/sampler/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6655 2024-05-04 17:39:35.000000 beat-2.0.1/beat/sampler/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18897 2024-05-04 17:39:35.000000 beat-2.0.1/beat/sampler/metropolis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30456 2024-05-04 17:39:35.000000 beat-2.0.1/beat/sampler/pt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18460 2024-05-04 17:39:35.000000 beat-2.0.1/beat/sampler/smc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20470 2024-05-04 17:39:35.000000 beat-2.0.1/beat/sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6108 2024-05-04 17:39:35.000000 beat-2.0.1/beat/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44757 2024-05-04 17:39:35.000000 beat-2.0.1/beat/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:39:41.686363 beat-2.0.1/beat/voronoi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:39:35.000000 beat-2.0.1/beat/voronoi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-04 17:39:35.000000 beat-2.0.1/beat/voronoi/voronoi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-05-04 17:39:35.000000 beat-2.0.1/beat/voronoi/voronoi_ext.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:39:41.690363 beat-2.0.1/beat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-05-04 17:39:41.000000 beat-2.0.1/beat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-04 17:39:41.000000 beat-2.0.1/beat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 17:39:41.000000 beat-2.0.1/beat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-04 17:39:41.000000 beat-2.0.1/beat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-04 17:39:41.000000 beat-2.0.1/beat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-04 17:39:41.000000 beat-2.0.1/beat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-04 17:39:36.000000 beat-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 17:39:41.690363 beat-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-04 17:39:36.000000 beat-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:39:41.690363 beat-2.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-05-04 17:39:36.000000 beat-2.0.1/test/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-05-04 17:39:36.000000 beat-2.0.1/test/test_bem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-05-04 17:39:36.000000 beat-2.0.1/test/test_composites.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-04 17:39:36.000000 beat-2.0.1/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-04 17:39:36.000000 beat-2.0.1/test/test_covariance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-04 17:39:36.000000 beat-2.0.1/test/test_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-05-04 17:39:36.000000 beat-2.0.1/test/test_fastsweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-05-04 17:39:36.000000 beat-2.0.1/test/test_ffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-05-04 17:39:36.000000 beat-2.0.1/test/test_ffi_gfstacking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-05-04 17:39:36.000000 beat-2.0.1/test/test_ffi_gfstacking_multifault.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-04 17:39:36.000000 beat-2.0.1/test/test_geodetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-05-04 17:39:36.000000 beat-2.0.1/test/test_heart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-04 17:39:36.000000 beat-2.0.1/test/test_laplacian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8129 2024-05-04 17:39:36.000000 beat-2.0.1/test/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-04 17:39:36.000000 beat-2.0.1/test/test_paripool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-04 17:39:36.000000 beat-2.0.1/test/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-04 17:39:36.000000 beat-2.0.1/test/test_proposals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-04 17:39:36.000000 beat-2.0.1/test/test_pt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-05-04 17:39:36.000000 beat-2.0.1/test/test_resolution_subsampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-04 17:39:36.000000 beat-2.0.1/test/test_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-04 17:39:36.000000 beat-2.0.1/test/test_smc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-04 17:39:36.000000 beat-2.0.1/test/test_sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-04 17:39:36.000000 beat-2.0.1/test/test_utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-04 17:39:36.000000 beat-2.0.1/test/test_voronoi.py
```

### Comparing `beat-2.0.0/PKG-INFO` & `beat-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beat
-Version: 2.0.0
+Version: 2.0.1
 Summary: 'Bayesian Earthquake Analysis Tool'
 Author-email: Hannes Vasyura-Bathke <vasbath@gfz-potsdam.de>
 Maintainer-email: Hannes Vasyura-Bathke <vasbath@gfz-potsdam.de>
 License: GPLv3
 Project-URL: Home, https://pyrocko.org/beat
 Project-URL: GitHub, https://github.com/hvasbath/beat
 Project-URL: Issues, https://github.com/hvasbath/beat/issues
```

### Comparing `beat-2.0.0/README.md` & `beat-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/beat/apps/beat.py` & `beat-2.0.1/beat/apps/beat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1284,15 +1284,15 @@
                         reference.update(jpoint)
                         del jpoint, ldicts
 
                     derived = []
                     # BEAT sources calculate derived params
                     if options.calc_derived:
                         composite.point2sources(point)
-                        if options.mode == geometry_mode_str:
+                        if options.mode in [geometry_mode_str, ffi_mode_str]:
                             for source in sources:
                                 if hasattr(source, "get_derived_parameters"):
                                     deri = source.get_derived_parameters(
                                         point=reference,  # need to pass correction params
                                         store=store,
                                         target=target,
                                         event=problem.config.event,
@@ -1309,15 +1309,15 @@
                             if len(pc.source_types) > 1:
                                 derived = [hstack(derived)]
 
                         elif options.mode == bem_mode_str:
                             response = composite.engine.process(
                                 sources=composite.sources, targets=composite.targets
                             )
-                            derived = response.get_source_magnitudes(
+                            derived = response.get_derived_parameters(
                                 composite.engine.config.shear_modulus
                             )
 
                     lpoint = problem.model.lijection.d2l(point)
 
                     if derived:
                         lpoint.extend(
@@ -2180,15 +2180,15 @@
                 homepath = problem.config.geodetic_config.types["SAR"].datadir
                 scene_path = os.path.join(homepath, dataset.name)
                 logger.info("Loading full resolution kite scene: %s" % scene_path)
                 sandbox.loadReferenceScene(scene_path)
             except (UserIOWarning, KeyError):
                 raise ImportError("Full resolution data could not be loaded!")
         elif isinstance(dataset, heart.GNSSCompoundComponent):
-            logger.info("Found GNSS Compound %s, importing to kite..." % dataset.name)
+            logger.info("Found GNSS Compound %s, importing to kite..." % dataset.id)
             scene = dataset.to_kite_scene()
             # scene.spool()
             sandbox.setReferenceScene(scene)
         else:
             raise TypeError("Dataset type %s is not supported!" % dataset.__class__)
 
         from tempfile import mkdtemp
```

### Comparing `beat-2.0.0/beat/apps/beatdown.py` & `beat-2.0.1/beat/apps/beatdown.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/beat/backend.py` & `beat-2.0.1/beat/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,17 +80,16 @@
     return ["{}__{}".format(varname, "_".join(idxs)) for idxs in zip(*labels)]
 
 
 def _create_flat_names_summary(varname, shape):
     if not shape or sum(shape) == 1:
         return [varname]
 
-    labels = (num.ravel(xs).tolist() for xs in num.indices(shape))
-    labels = (map(str, [xs]) for xs in labels)
-    return ["{}{}".format(varname, "".join(idxs)) for idxs in zip(*labels)]
+    labels = num.indices(shape).ravel().tolist()
+    return ["{}[{}]".format(varname, idxs) for idxs in labels]
 
 
 def _create_shape(flat_names):
     """Determine shape from `_create_flat_names` output."""
     try:
         _, shape_str = flat_names[-1].rsplit("__", 1)
     except ValueError:
@@ -341,14 +340,15 @@
             )
 
         self.derived_mapping = {}
         for varname, shape in zip(varnames, shapes):
             if varname in self.varnames:
                 exist_idx = self.varnames.index(varname)
                 self.varnames.pop(exist_idx)
+                self.flat_names.pop(varname)
                 exist_shape = self.var_shapes[varname]
                 shape = tuple(map(sum, zip(exist_shape, shape)))
                 concat_idx = len(self.varnames)
                 self.derived_mapping[exist_idx] = concat_idx
 
             self.flat_names[varname] = _create_flat_names(varname, shape)
             self.var_shapes[varname] = shape
```

### Comparing `beat-2.0.0/beat/colormap.py` & `beat-2.0.1/beat/colormap.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/beat/config.py` & `beat-2.0.1/beat/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     "MTQTSource": mt_components + dc_components,
     "MTSource": dc_components,
     "RectangularSource": ["magnitude"],
     "RectangularSourcePole": ["magnitude", "coupling"],
 }
 
 derived_variables_mapping.update(
-    {source_name: ["magnitude"] for source_name in bem_source_catalog.keys()}
+    {source_name: ["magnitude", "slip"] for source_name in bem_source_catalog.keys()}
 )
 
 
 hyper_name_laplacian = "h_laplacian"
 
 response_file_name = "responses.pkl"
 geodetic_data_name = "geodetic_data.pkl"
```

### Comparing `beat-2.0.0/beat/covariance.py` & `beat-2.0.1/beat/covariance.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
         return NoiseStructureCatalog2d[self.config.structure](dataset.ncoords)
 
     def do_import(self, dataset):
         if dataset.covariance.data is not None:
             return dataset.covariance.data
         else:
             raise ValueError(
-                "Data covariance for dataset %s needs to be defined!" % dataset.name
+                "Data covariance for dataset %s needs to be defined!" % dataset.id
             )
 
     def do_non_toeplitz(self, dataset, result):
         if dataset.typ == "SAR":
             dataset.update_local_coords(self.events[0])
             coords = num.vstack([dataset.east_shifts, dataset.north_shifts]).T
 
@@ -200,15 +200,15 @@
             )
         else:
             scaling = dataset.covariance.data
 
         if num.isnan(scaling).any():
             raise ValueError(
                 "Estimated Non-Toeplitz covariance matrix for dataset %s contains Nan! "
-                "Please increase 'max_dist_perc'!" % dataset.name
+                "Please increase 'max_dist_perc'!" % dataset.id
             )
 
         return scaling
 
     def get_data_covariance(self, dataset, result=None):
         """
         Estimated data covariances of seismic traces
```

### Comparing `beat-2.0.0/beat/defaults.py` & `beat-2.0.1/beat/defaults.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 beat_dir_tmpl = os.environ.get("BEAT_DIR", os.path.expanduser("~/.beat"))
 
 
 class Bounds(Object):
     default_bounds = Tuple.T(2, Float.T(), default=(0, 1))
     physical_bounds = Tuple.T(2, Float.T(), default=(0, 1))
-    unit = String.T(default="$[m]$")
+    unit = String.T(default=r"[m]")
 
 
 class ParameterDefaults(Object):
     parameters = Dict.T(String.T(), Bounds.T())
 
     def __getitem__(self, k):
         if k not in self.parameters.keys():
@@ -34,261 +34,267 @@
         return self.parameters[k]
 
 
 sf_force = (0, 1e10)
 moffdiag = (-1.0, 1.0)
 mdiag = (-SQRT2, SQRT2)
 
+u_n = r"$[N]$"
+u_nm = r"$[Nm]$"
+u_km = r"$[km]$"
+u_km_s = r"$[km/s]$"
+u_deg = r"$[^\circ]$"
+u_deg_myr = r"$[^\circ/myr]$"
+u_m = r"$[m]$"
+u_v = r"$[m^3]$"
+u_s = r"$[s]$"
+u_rad = r"$[rad]$"
+u_hyp = r""
+u_percent = r"[$\%$]"
+u_nanostrain = r"[nstrain]"
+u_pa = r"$[MPa]$"
 
 # Bounds and Units for all parameters
 parameter_info = {
     "east_shift": Bounds(
-        physical_bounds=(-500.0, 500.0), default_bounds=(-10.0, 10.0), unit="$[km]$"
+        physical_bounds=(-500.0, 500.0), default_bounds=(-10.0, 10.0), unit=u_km
     ),
     "north_shift": Bounds(
-        physical_bounds=(-500.0, 500.0), default_bounds=(-10.0, 10.0), unit="$[km]$"
+        physical_bounds=(-500.0, 500.0), default_bounds=(-10.0, 10.0), unit=u_km
     ),
     "depth": Bounds(
-        physical_bounds=(0.0, 1000.0), default_bounds=(0.0, 5.0), unit="$[km]$"
+        physical_bounds=(0.0, 1000.0), default_bounds=(0.0, 5.0), unit=u_km
     ),
     "strike": Bounds(
-        physical_bounds=(-90.0, 420.0), default_bounds=(0, 180.0), unit=r"$[^\circ]$"
+        physical_bounds=(-90.0, 420.0), default_bounds=(0, 180.0), unit=u_deg
     ),
     "strike1": Bounds(
-        physical_bounds=(-90.0, 420.0), default_bounds=(0, 180.0), unit=r"$[^\circ]$"
+        physical_bounds=(-90.0, 420.0), default_bounds=(0, 180.0), unit=u_deg
     ),
     "strike2": Bounds(
-        physical_bounds=(-90.0, 420.0), default_bounds=(0, 180.0), unit=r"$[^\circ]$"
+        physical_bounds=(-90.0, 420.0), default_bounds=(0, 180.0), unit=u_deg
     ),
     "dip": Bounds(
-        physical_bounds=(-45.0, 135.0), default_bounds=(45.0, 90.0), unit=r"$[^\circ]$"
+        physical_bounds=(-45.0, 135.0), default_bounds=(45.0, 90.0), unit=u_deg
     ),
     "dip1": Bounds(
-        physical_bounds=(-45.0, 135.0), default_bounds=(45.0, 90.0), unit=r"$[^\circ]$"
+        physical_bounds=(-45.0, 135.0), default_bounds=(45.0, 90.0), unit=u_deg
     ),
     "dip2": Bounds(
-        physical_bounds=(-45.0, 135.0), default_bounds=(45.0, 90.0), unit=r"$[^\circ]$"
+        physical_bounds=(-45.0, 135.0), default_bounds=(45.0, 90.0), unit=u_deg
     ),
     "rake": Bounds(
         physical_bounds=(-180.0, 270.0),
         default_bounds=(-90.0, 90.0),
-        unit=r"$[^\circ]$",
+        unit=u_deg,
     ),
     "rake1": Bounds(
         physical_bounds=(-180.0, 270.0),
         default_bounds=(-90.0, 90.0),
-        unit=r"$[^\circ]$",
+        unit=u_deg,
     ),
     "rake2": Bounds(
         physical_bounds=(-180.0, 270.0),
         default_bounds=(-90.0, 90.0),
-        unit=r"$[^\circ]$",
+        unit=u_deg,
     ),
-    "mix": Bounds(physical_bounds=(0, 1), default_bounds=(0, 1), unit=""),
+    "mix": Bounds(physical_bounds=(0, 1), default_bounds=(0, 1), unit=u_hyp),
     "volume_change": Bounds(
-        physical_bounds=(-1e12, 1e12), default_bounds=(1e8, 1e10), unit="$[m^3]$"
+        physical_bounds=(-1e12, 1e12), default_bounds=(1e8, 1e10), unit=u_v
     ),
     "diameter": Bounds(
-        physical_bounds=(0.0, 100.0), default_bounds=(5.0, 10.0), unit="$[km]$"
-    ),
-    "slip": Bounds(
-        physical_bounds=(0.0, 150.0), default_bounds=(0.1, 8.0), unit="$[m]$"
+        physical_bounds=(0.0, 100.0), default_bounds=(5.0, 10.0), unit=u_km
     ),
+    "slip": Bounds(physical_bounds=(0.0, 150.0), default_bounds=(0.1, 8.0), unit=u_m),
     "opening_fraction": Bounds(
-        physical_bounds=moffdiag, default_bounds=(0.0, 0.0), unit=""
-    ),
-    "azimuth": Bounds(
-        physical_bounds=(0, 360), default_bounds=(0, 180), unit=r"$[^\circ]$"
+        physical_bounds=moffdiag, default_bounds=(0.0, 0.0), unit=u_hyp
     ),
+    "azimuth": Bounds(physical_bounds=(0, 360), default_bounds=(0, 180), unit=u_deg),
     "amplitude": Bounds(
-        physical_bounds=(1.0, 10e25), default_bounds=(1e10, 1e20), unit="$[Nm]$"
+        physical_bounds=(1.0, 10e25), default_bounds=(1e10, 1e20), unit=u_nm
     ),
     "locking_depth": Bounds(
-        physical_bounds=(0.1, 100.0), default_bounds=(1.0, 10.0), unit="$[km]$"
+        physical_bounds=(0.1, 100.0), default_bounds=(1.0, 10.0), unit=u_km
     ),
     "nucleation_dip": Bounds(
-        physical_bounds=(0.0, num.inf), default_bounds=(0.0, 7.0), unit="$[km]$"
+        physical_bounds=(0.0, num.inf), default_bounds=(0.0, 7.0), unit=u_km
     ),
     "nucleation_strike": Bounds(
-        physical_bounds=(0.0, num.inf), default_bounds=(0.0, 10.0), unit="$[km]$"
+        physical_bounds=(0.0, num.inf), default_bounds=(0.0, 10.0), unit=u_km
+    ),
+    "nucleation_x": Bounds(
+        physical_bounds=moffdiag, default_bounds=moffdiag, unit=u_hyp
+    ),
+    "nucleation_y": Bounds(
+        physical_bounds=moffdiag, default_bounds=moffdiag, unit=u_hyp
     ),
-    "nucleation_x": Bounds(physical_bounds=moffdiag, default_bounds=moffdiag, unit=""),
-    "nucleation_y": Bounds(physical_bounds=moffdiag, default_bounds=moffdiag, unit=""),
     "time_shift": Bounds(
-        physical_bounds=(-20.0, 20.0), default_bounds=(-5.0, 5.0), unit="$[s]$"
+        physical_bounds=(-20.0, 20.0), default_bounds=(-5.0, 5.0), unit=u_s
     ),
-    "coupling": Bounds(physical_bounds=(0, 100), default_bounds=(0, 1), unit="[$\%$]"),
+    "coupling": Bounds(physical_bounds=(0, 100), default_bounds=(0, 1), unit=u_percent),
     "uperp": Bounds(
-        physical_bounds=(-150.0, 150.0), default_bounds=(-0.3, 4.0), unit="$[m]$"
+        physical_bounds=(-150.0, 150.0), default_bounds=(-0.3, 4.0), unit=u_m
     ),
     "uparr": Bounds(
-        physical_bounds=(-1.0, 150.0), default_bounds=(-0.05, 6.0), unit="$[m]$"
+        physical_bounds=(-1.0, 150.0), default_bounds=(-0.05, 6.0), unit=u_m
     ),
     "utens": Bounds(
-        physical_bounds=(-150.0, 150.0), default_bounds=(0.0, 0.0), unit="$[m]$"
+        physical_bounds=(-150.0, 150.0), default_bounds=(0.0, 0.0), unit=u_m
     ),
     "durations": Bounds(
-        physical_bounds=(0.0, 600.0), default_bounds=(0.5, 29.5), unit="$[s]$"
+        physical_bounds=(0.0, 600.0), default_bounds=(0.5, 29.5), unit=u_s
     ),
     "velocities": Bounds(
-        physical_bounds=(0.0, 20.0), default_bounds=(0.5, 4.2), unit="$[km/s]$"
-    ),
-    "fn": Bounds(
-        physical_bounds=(-1e20, 1e20), default_bounds=(-1e20, 1e20), unit="$[N]$"
-    ),
-    "fe": Bounds(
-        physical_bounds=(-1e20, 1e20), default_bounds=(-1e20, 1e20), unit="$[N]$"
-    ),
-    "fd": Bounds(
-        physical_bounds=(-1e20, 1e20), default_bounds=(-1e20, 1e20), unit="$[N]$"
+        physical_bounds=(0.0, 20.0), default_bounds=(0.5, 4.2), unit=u_km_s
     ),
+    "fn": Bounds(physical_bounds=(-1e20, 1e20), default_bounds=(-1e20, 1e20), unit=u_n),
+    "fe": Bounds(physical_bounds=(-1e20, 1e20), default_bounds=(-1e20, 1e20), unit=u_n),
+    "fd": Bounds(physical_bounds=(-1e20, 1e20), default_bounds=(-1e20, 1e20), unit=u_n),
     "mnn": Bounds(
-        physical_bounds=(-SQRT2, SQRT2), default_bounds=(-SQRT2, SQRT2), unit="$[Nm]$"
+        physical_bounds=(-SQRT2, SQRT2), default_bounds=(-SQRT2, SQRT2), unit=u_nm
     ),
     "mee": Bounds(
-        physical_bounds=(-SQRT2, SQRT2), default_bounds=(-SQRT2, SQRT2), unit="$[Nm]$"
+        physical_bounds=(-SQRT2, SQRT2), default_bounds=(-SQRT2, SQRT2), unit=u_nm
     ),
     "mdd": Bounds(
-        physical_bounds=(-SQRT2, SQRT2), default_bounds=(-SQRT2, SQRT2), unit="$[Nm]$"
+        physical_bounds=(-SQRT2, SQRT2), default_bounds=(-SQRT2, SQRT2), unit=u_nm
     ),
-    "mne": Bounds(physical_bounds=moffdiag, default_bounds=moffdiag, unit="$[Nm]$"),
-    "mnd": Bounds(physical_bounds=moffdiag, default_bounds=moffdiag, unit="$[Nm]$"),
-    "med": Bounds(physical_bounds=moffdiag, default_bounds=moffdiag, unit="$[Nm]$"),
+    "mne": Bounds(physical_bounds=moffdiag, default_bounds=moffdiag, unit=u_nm),
+    "mnd": Bounds(physical_bounds=moffdiag, default_bounds=moffdiag, unit=u_nm),
+    "med": Bounds(physical_bounds=moffdiag, default_bounds=moffdiag, unit=u_nm),
     "magnitude": Bounds(
-        physical_bounds=(-5.0, 10.0), default_bounds=(4.0, 7.0), unit=""
+        physical_bounds=(-5.0, 10.0), default_bounds=(4.0, 7.0), unit=u_hyp
     ),
-    "eps_xx": Bounds(
-        physical_bounds=(-num.inf, num.inf), default_bounds=(0, 1), unit=""
+    "exx": Bounds(
+        physical_bounds=(-num.inf, num.inf),
+        default_bounds=(-200.0, 200.0),
+        unit=u_nanostrain,
     ),
-    "eps_yy": Bounds(
-        physical_bounds=(-num.inf, num.inf), default_bounds=(0, 1), unit=""
+    "eyy": Bounds(
+        physical_bounds=(-num.inf, num.inf),
+        default_bounds=(-200.0, 200.0),
+        unit=u_nanostrain,
     ),
-    "eps_xy": Bounds(
-        physical_bounds=(-num.inf, num.inf), default_bounds=(0, 1), unit=""
+    "exy": Bounds(
+        physical_bounds=(-num.inf, num.inf),
+        default_bounds=(-200.0, 200.0),
+        unit=u_nanostrain,
     ),
     "rotation": Bounds(
         physical_bounds=(-num.inf, num.inf),
         default_bounds=(-200.0, 200.0),
-        unit="$[rad]$",
+        unit=u_nanostrain,
     ),
-    "pole_lat": Bounds(
-        physical_bounds=(-90.0, 90.0), default_bounds=(0, 1), unit=r"$[^\circ]$"
+    "lat": Bounds(
+        physical_bounds=(-90.0, 90.0), default_bounds=(30.0, 30.5), unit=u_deg
     ),
-    "pole_lon": Bounds(
-        physical_bounds=(-180.0, 180.0), default_bounds=(0, 1), unit=r"$[^\circ]$"
+    "lon": Bounds(
+        physical_bounds=(-180.0, 180.0), default_bounds=(30.0, 30.5), unit=u_deg
     ),
     "omega": Bounds(
-        physical_bounds=(-10.0, 10.0), default_bounds=(0.5, 0.6), unit=r"$[^\circ/myr]$"
+        physical_bounds=(-10.0, 10.0), default_bounds=(0.5, 0.6), unit=u_deg_myr
     ),
     "w": Bounds(
         physical_bounds=(-3.0 / 8.0 * num.pi, 3.0 / 8.0 * num.pi),
         default_bounds=(-3.0 / 8.0 * num.pi, 3.0 / 8.0 * num.pi),
-        unit="$[rad]$",
+        unit=u_rad,
     ),
     "v": Bounds(
         physical_bounds=(-1.0 / 3, 1.0 / 3),
         default_bounds=(-1.0 / 3, 1.0 / 3),
-        unit="$[rad]$",
+        unit=u_rad,
     ),
     "kappa": Bounds(
         physical_bounds=(0.0, 2 * num.pi),
         default_bounds=(0.0, 2 * num.pi),
-        unit=r"$[^\circ]$",
+        unit=u_deg,
     ),
     "sigma": Bounds(
         physical_bounds=(-num.pi / 2.0, num.pi / 2.0),
         default_bounds=(-num.pi / 2.0, num.pi / 2.0),
-        unit=r"$[^\circ]$",
-    ),
-    "h": Bounds(
-        physical_bounds=(0.0, 1.0), default_bounds=(0.0, 1.0), unit=r"$[^\circ]$"
+        unit=u_deg,
     ),
+    "h": Bounds(physical_bounds=(0.0, 1.0), default_bounds=(0.0, 1.0), unit=u_deg),
     "length": Bounds(
-        physical_bounds=(0.0, 7000.0), default_bounds=(5.0, 30.0), unit="$[km]$"
+        physical_bounds=(0.0, 7000.0), default_bounds=(5.0, 30.0), unit=u_km
     ),
     "width": Bounds(
-        physical_bounds=(0.0, 500.0), default_bounds=(5.0, 20.0), unit="$[km]$"
+        physical_bounds=(0.0, 500.0), default_bounds=(5.0, 20.0), unit=u_km
     ),
     "time": Bounds(
-        physical_bounds=(-200.0, 200.0), default_bounds=(-5.0, 5.0), unit="$[s]$"
+        physical_bounds=(-200.0, 200.0), default_bounds=(-5.0, 5.0), unit=u_s
     ),
     "delta_time": Bounds(
-        physical_bounds=(0.0, 100.0), default_bounds=(0.0, 10.0), unit="$[s]$"
+        physical_bounds=(0.0, 100.0), default_bounds=(0.0, 10.0), unit=u_s
     ),
     "depth_bottom": Bounds(
-        physical_bounds=(0.0, 300.0), default_bounds=(0.0, 10.0), unit="$[km]$"
+        physical_bounds=(0.0, 300.0), default_bounds=(0.0, 10.0), unit=u_km
     ),
     "distance": Bounds(
-        physical_bounds=(0.0, 300.0), default_bounds=(0.0, 10.0), unit="$[km]$"
+        physical_bounds=(0.0, 300.0), default_bounds=(0.0, 10.0), unit=u_km
     ),
     "duration": Bounds(
-        physical_bounds=(0.0, 600.0), default_bounds=(1.0, 30.0), unit="$[s]$"
+        physical_bounds=(0.0, 600.0), default_bounds=(1.0, 30.0), unit=u_s
     ),
     "peak_ratio": Bounds(
-        physical_bounds=(0.0, 1.0), default_bounds=(0.0, 1.0), unit=""
+        physical_bounds=(0.0, 1.0), default_bounds=(0.0, 1.0), unit=u_hyp
+    ),
+    "hypers": Bounds(
+        physical_bounds=(-10.0, 10.0), default_bounds=(-2.0, 6.0), unit=u_hyp
     ),
-    "hypers": Bounds(physical_bounds=(-4.0, 10.0), default_bounds=(-2.0, 6.0), unit=""),
     "ramp": Bounds(
-        physical_bounds=(-0.005, 0.005), default_bounds=(-0.005, 0.005), unit="$[rad]$"
+        physical_bounds=(-0.005, 0.005), default_bounds=(-0.005, 0.005), unit=u_rad
     ),
     "offset": Bounds(
-        physical_bounds=(-0.05, 0.05), default_bounds=(-0.05, 0.05), unit="$[m]$"
-    ),
-    "lat": Bounds(
-        physical_bounds=(30.0, 30.5), default_bounds=(30.0, 30.5), unit=r"$[^\circ]$"
-    ),
-    "lon": Bounds(
-        physical_bounds=(30.0, 30.5), default_bounds=(30.0, 30.5), unit=r"$[^\circ]$"
-    ),
-    "traction": Bounds(
-        physical_bounds=(0, 1000), default_bounds=(0, 50), unit="$[MPa]$"
+        physical_bounds=(-0.05, 0.05), default_bounds=(-0.05, 0.05), unit=u_m
     ),
+    "traction": Bounds(physical_bounds=(0, 1000), default_bounds=(0, 50), unit=u_pa),
     "strike_traction": Bounds(
-        physical_bounds=(-15000, 15000), default_bounds=(-50, 50), unit="$[MPa]$"
+        physical_bounds=(-15000, 15000), default_bounds=(-50, 50), unit=u_pa
     ),
     "dip_traction": Bounds(
-        physical_bounds=(-15000, 15000), default_bounds=(-50, 50), unit="$[MPa]$"
+        physical_bounds=(-15000, 15000), default_bounds=(-50, 50), unit=u_pa
     ),
     "normal_traction": Bounds(
-        physical_bounds=(-15000, 15000), default_bounds=(-50, 50), unit="$[MPa]$"
+        physical_bounds=(-15000, 15000), default_bounds=(-50, 50), unit=u_pa
     ),
     "a_half_axis": Bounds(
-        physical_bounds=(0.01, 100), default_bounds=(0.01, 10), unit="$[km]$"
+        physical_bounds=(0.01, 100), default_bounds=(0.01, 10), unit=u_km
     ),
     "b_half_axis": Bounds(
-        physical_bounds=(0.01, 100), default_bounds=(0.01, 10), unit="$[km]$"
+        physical_bounds=(0.01, 100), default_bounds=(0.01, 10), unit=u_km
     ),
     "a_half_axis_bottom": Bounds(
-        physical_bounds=(0.01, 100), default_bounds=(0.01, 10), unit="$[km]$"
+        physical_bounds=(0.01, 100), default_bounds=(0.01, 10), unit=u_km
     ),
     "b_half_axis_bottom": Bounds(
-        physical_bounds=(0.01, 100), default_bounds=(0.01, 10), unit="$[km]$"
-    ),
-    "plunge": Bounds(
-        physical_bounds=(0, 90), default_bounds=(0, 20), unit=r"$[^\circ]$"
+        physical_bounds=(0.01, 100), default_bounds=(0.01, 10), unit=u_km
     ),
+    "plunge": Bounds(physical_bounds=(0, 90), default_bounds=(0, 20), unit=u_deg),
     "delta_east_shift_bottom": Bounds(
-        physical_bounds=(-500, 500), default_bounds=(-10, 10), unit="$[km]$"
+        physical_bounds=(-500, 500), default_bounds=(-10, 10), unit=u_km
     ),
     "delta_north_shift_bottom": Bounds(
-        physical_bounds=(-500, 500), default_bounds=(-10, 10), unit="$[km]$"
+        physical_bounds=(-500, 500), default_bounds=(-10, 10), unit=u_km
     ),
     "curv_amplitude_bottom": Bounds(
-        physical_bounds=moffdiag, default_bounds=moffdiag, unit=""
+        physical_bounds=moffdiag, default_bounds=moffdiag, unit=u_hyp
     ),
     "curv_location_bottom": Bounds(
-        physical_bounds=(0.0, 1.0), default_bounds=(0.0, 1.0), unit=""
+        physical_bounds=(0.0, 1.0), default_bounds=(0.0, 1.0), unit=u_hyp
     ),
     "bend_location": Bounds(
-        physical_bounds=(0.0, 1.0), default_bounds=(0.0, 1.0), unit=""
+        physical_bounds=(0.0, 1.0), default_bounds=(0.0, 1.0), unit=u_hyp
     ),
     "bend_amplitude": Bounds(
-        physical_bounds=moffdiag, default_bounds=moffdiag, unit=""
+        physical_bounds=moffdiag, default_bounds=moffdiag, unit=u_hyp
+    ),
+    "like": Bounds(
+        physical_bounds=(-num.inf, num.inf), default_bounds=(0, 1), unit=u_hyp
     ),
-    "like": Bounds(physical_bounds=(-num.inf, num.inf), default_bounds=(0, 1), unit=""),
 }
 
 
 def hypername(varname):
     return varname if varname in parameter_info.keys() else "hypers"
```

### Comparing `beat-2.0.0/beat/fast_sweeping/fast_sweep.py` & `beat-2.0.1/beat/fast_sweeping/fast_sweep.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/beat/fast_sweeping/fast_sweep_ext.c` & `beat-2.0.1/beat/fast_sweeping/fast_sweep_ext.c`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/beat/ffi/base.py` & `beat-2.0.1/beat/ffi/base.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/beat/ffi/fault.py` & `beat-2.0.1/beat/ffi/fault.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/beat/heart.py` & `beat-2.0.1/beat/heart.py`

 * *Files 1% similar despite different names*

```diff
@@ -1070,14 +1070,18 @@
     )
 
     def __init__(self, **kwargs):
         self.has_correction = False
         self.corrections = None
         super(GeodeticDataset, self).__init__(**kwargs)
 
+    @property
+    def id(self):
+        return self.name
+
     def get_corrections(self, hierarchicals, point=None):
         """
         Needs to be specified on inherited dataset classes.
         """
         raise NotImplementedError("Needs implementation in subclass")
 
     def setup_corrections(self, event, correction_configs):
@@ -1095,14 +1099,17 @@
                 locx_name, locy_name = corr.get_required_coordinate_names()
 
                 locx = getattr(self, locx_name)
                 locy = getattr(self, locy_name)
 
                 data_mask = self.get_data_mask(corr_conf)
 
+                if self.los_vector is None:
+                    self.update_los_vector()
+
                 corr.setup_correction(
                     locy=locy,
                     locx=locx,
                     los_vector=self.los_vector,
                     data_mask=data_mask,
                     dataset_name=self.name,
                     number=number,
@@ -1170,14 +1177,18 @@
         optional=True,
     )
 
     def __init__(self, **kwargs):
         self._station2index = None
         super(GNSSCompoundComponent, self).__init__(**kwargs)
 
+    @property
+    def id(self):
+        return "%s_%s" % (self.name, self.component)
+
     def update_los_vector(self):
         if self.component == "east":
             c = num.array([0, 1, 0])
         elif self.component == "north":
             c = num.array([1, 0, 0])
         elif self.component == "up":
             c = num.array([0, 0, 1])
@@ -1232,16 +1243,18 @@
         scene = Scene(
             theta=theta_bin, phi=phi_bin, displacement=bin_disp, config=config
         )
 
         return scene
 
     def get_data_mask(self, corr_config):
+        """
+        Return dataset mask, i.e. boolean numpy array, 0/1 indicating false/true masking,
+        """
         s2idx = self.station_name_index_mapping()
-
         if (
             len(corr_config.station_whitelist) > 0
             and len(corr_config.station_blacklist) > 0
         ):
             raise ValueError("Either White or Blacklist can be defined!")
 
         station_blacklist_idxs = []
@@ -1259,16 +1272,17 @@
                 if station_name not in corr_config.station_whitelist:
                     station_blacklist_idxs.append(s2idx[station_name])
 
         logger.info(
             "Stations with idxs %s got blacklisted!"
             % utility.list2string(station_blacklist_idxs)
         )
-        mask = num.ones_like(self.lats, dtype=num.bool_)
-        mask[num.array(station_blacklist_idxs)] = False
+        mask = num.zeros_like(self.lats, dtype=num.bool_)
+        if len(station_blacklist_idxs) > 0:
+            mask[num.array(station_blacklist_idxs)] = True
         return mask
 
     def station_name_index_mapping(self):
         if self._station2index is None:
             self._station2index = dict(
                 (station.code, i) for (i, station) in enumerate(self.stations)
             )
```

### Comparing `beat-2.0.0/beat/inputf.py` & `beat-2.0.1/beat/inputf.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/beat/models/base.py` & `beat-2.0.1/beat/models/base.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/beat/models/corrections.py` & `beat-2.0.1/beat/models/corrections.py`

 * *Files 8% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                         "No hierarchical parameters initialized,"
                         "but requested! Please check init!"
                     )
 
                 kwargs = self.get_point_rvs(hierarchicals)
 
             vels = velocities_from_pole(self.lats, self.lons, **kwargs)
-            if self.data_mask.size > 0:
+            if self.data_mask.any():
                 vels[self.data_mask] = 0.0
             return (vels * self.los_vector).sum(axis=1)
 
 
 class StrainRateCorrection(Correction):
     def get_required_coordinate_names(self):
         return ["lons", "lats"]
@@ -158,22 +158,23 @@
         self.strain_rate_tensor = StrainRateTensor(self.lats, self.lons, data_mask)
 
         self.slos_vector = shared(
             self.los_vector.astype(tconfig.floatX), name="los", borrow=True
         )
 
     def get_station_coordinates(self, mask=None):
+        """Return masked coordinates of stations"""
         if mask is None:
             mask = self.data_mask
 
-        return array(self.lats)[mask], array(self.lons)[mask]
+        return array(self.lats)[~mask], array(self.lons)[~mask]
 
     def get_displacements(self, hierarchicals, point=None):
         """
-        Get synthetic correction velocity due to Euler pole rotation.
+        Get synthetic correction velocity due to Strain Rate Tensor.
         """
         if not self.correction_names:
             raise ValueError("Requested correction, but is not setup or configured!")
 
         if not point:  # pytensor instance for get_formula
             inputs = OrderedDict()
             for corr_name in self.correction_names:
@@ -194,11 +195,11 @@
 
                 kwargs = self.get_point_rvs(hierarchicals)
 
         v_xyz = velocities_from_strain_rate_tensor(
             array(self.lats), array(self.lons), **kwargs
         )
 
-        if self.data_mask.size > 0:
+        if self.data_mask.any():
             v_xyz[self.data_mask, :] = 0.0
 
         return (v_xyz * self.los_vector).sum(axis=1)
```

### Comparing `beat-2.0.0/beat/models/distributions.py` & `beat-2.0.1/beat/models/distributions.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/beat/models/geodetic.py` & `beat-2.0.1/beat/models/geodetic.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,32 +127,19 @@
             self.weights.append(shared(choli, name="geo_weight_%i" % i, borrow=True))
             data.covariance.update_slog_pdet()
 
     @property
     def n_t(self):
         return len(self.datasets)
 
-    def get_all_dataset_names(self, hp_name):
+    def get_all_dataset_ids(self, hp_name):
         """
         Return unique GNSS stations and radar acquisitions.
         """
-        names = []
-        for dataset in self.datasets:
-            if dataset.typ == hp_name.split("_")[1]:
-                if isinstance(dataset, heart.DiffIFG):
-                    names.append(dataset.name)
-                elif isinstance(dataset, heart.GNSSCompoundComponent):
-                    names.append(dataset.component)
-                else:
-                    TypeError(
-                        'Geodetic Dataset of class "%s" not '
-                        "supported" % dataset.__class__.__name__
-                    )
-
-        return names
+        return [dataset.id for dataset in self.datasets]
 
     def analyse_noise(self, tpoint=None):
         """
         Analyse geodetic noise in datasets and set
         data-covariance matrixes accordingly.
         """
         if self.config.noise_estimator.structure == "non-toeplitz":
@@ -162,15 +149,15 @@
 
         if len(self.datasets) != len(results):
             raise ValueError("Number of datasets and results need to be equal!")
 
         for dataset, result in zip(self.datasets, results):
             logger.info(
                 'Retrieving geodetic data-covariances with structure "%s" '
-                "for %s ..." % (self.config.noise_estimator.structure, dataset.name)
+                "for %s ..." % (self.config.noise_estimator.structure, dataset.id)
             )
 
             cov_d_geodetic = self.noise_analyser.get_data_covariance(
                 dataset, result=result
             )
 
             if dataset.covariance is None:
@@ -192,15 +179,15 @@
         hp_name: str
             of hyperparameter name
 
         Returns
         -------
         int
         """
-        n_datasets = len(self.get_all_dataset_names(hp_name))
+        n_datasets = len(self.get_all_dataset_ids(hp_name))
         if n_datasets == 0:
             raise ConfigInconsistentError(
                 'Found no data for hyperparameter "%s". Please either load'
                 " the data or remove it from types dictionary!" % hp_name,
                 params="hypers",
             )
         elif self.config.dataset_specific_residual_noise_estimation:
@@ -246,15 +233,14 @@
         point,
         results_path,
         stage_number,
         fix_output=False,
         force=False,
         update=False,
     ):
-        from kite.scene import Scene, UserIOWarning
         from pyrocko.guts import dump
 
         from beat.plotting import map_displacement_grid
 
         def save_covs(datasets, cov_mat="pred_v"):
             """
             Save covariance matrixes of given attribute
@@ -273,15 +259,15 @@
 
         results = self.assemble_results(point)
 
         def get_filename(attr, ending="csv"):
             return os.path.join(
                 results_path,
                 "{}_{}_{}.{}".format(
-                    os.path.splitext(dataset.name)[0], attr, stage_number, ending
+                    os.path.splitext(dataset.id)[0], attr, stage_number, ending
                 ),
             )
 
         # export for gnss
         for typ, config in gc.types.items():
             if "GNSS" == typ:
                 from pyrocko.model import gnss
@@ -309,14 +295,16 @@
                     outname = os.path.join(
                         results_path, "gnss_synths_%i.yaml" % stage_number
                     )
 
                     dump(model_camp, filename=outname)
 
             elif "SAR" == typ:
+                from kite.scene import Scene, UserIOWarning
+
                 logger.info("Exporting SAR data ...")
                 for dataset, result in zip(self.datasets, results):
                     if dataset.typ == "SAR":
                         try:
                             scene_path = os.path.join(config.datadir, dataset.name)
                             logger.info(
                                 f"Loading full resolution kite scene: {scene_path}"
@@ -501,25 +489,25 @@
 
             nom = residual.T.dot(icov).dot(residual)
             denom = data.T.dot(icov).dot(data)
 
             logger.debug("nom %f, denom %f" % (float(nom), float(denom)))
             var_red = 1 - (nom / denom)
 
-            logger.debug("Variance reduction for %s is %f" % (dataset.name, var_red))
+            logger.debug("Variance reduction for %s is %f" % (dataset.id, var_red))
 
             if 0:
                 from matplotlib import pyplot as plt
 
                 fig, ax = plt.subplots(1, 1)
                 im = ax.imshow(dataset.covariance.data)
                 plt.colorbar(im)
                 plt.show()
 
-            var_reds[dataset.name] = var_red
+            var_reds[dataset.id] = var_red
 
         return var_reds
 
     def get_standardized_residuals(self, point, results=None, weights=None):
         """
         Parameters
         ----------
@@ -543,15 +531,15 @@
 
         stdz_residuals = OrderedDict()
         for dataset, result in zip(self.datasets, results):
             hp = get_hypervalue_from_point(
                 point, dataset, counter, hp_specific=hp_specific
             )
             choli = num.linalg.inv(dataset.covariance.chol(num.exp(hp * 2.0)))
-            stdz_residuals[dataset.name] = choli.dot(result.processed_res)
+            stdz_residuals[dataset.id] = choli.dot(result.processed_res)
 
         return stdz_residuals
 
 
 class GeodeticSourceComposite(GeodeticComposite):
     """
     Comprises how to solve the non-linear geodetic forward model.
```

### Comparing `beat-2.0.0/beat/models/laplacian.py` & `beat-2.0.1/beat/models/laplacian.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/beat/models/polarity.py` & `beat-2.0.1/beat/models/polarity.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/beat/models/problems.py` & `beat-2.0.1/beat/models/problems.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/beat/models/seismic.py` & `beat-2.0.1/beat/models/seismic.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/beat/parallel.py` & `beat-2.0.1/beat/parallel.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/beat/plotting/__init__.py` & `beat-2.0.1/beat/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/beat/plotting/bem.py` & `beat-2.0.1/beat/plotting/bem.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/beat/plotting/common.py` & `beat-2.0.1/beat/plotting/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -877,30 +877,30 @@
                 xticker = MaxNLocator(nbins=2)
                 yticker = MaxNLocator(nbins=2)
                 ax.xaxis.set_major_locator(xticker)
                 ax.yaxis.set_major_locator(yticker)
                 if i_l == 0:
                     ax.set_ylabel("Sample idx")
                     ax.set_xlabel("Sample idx")
-                    ax.set_title(dataset.name)
+                    ax.set_title(dataset.id)
 
                     cbaxes = fig.add_axes([cbl, cbb, cbw, cbh])
                     cblabel = "Covariance [m²]"
                     cbs = plt.colorbar(
                         im,
                         ax=ax,
                         ticks=(vmin, vmax),
                         format=lambda x, _: f"{x:.2e}",
                         cax=cbaxes,
                         orientation="horizontal",
                     )
                     cbs.set_label(cblabel, fontsize=fontsize)
             else:
                 logger.info(
-                    'Did not find "%s" covariance component for %s', attr, dataset.name
+                    'Did not find "%s" covariance component for %s', attr, dataset.id
                 )
                 fig.delaxes(ax)
 
     return figures, axes
 
 
 def set_axes_equal_3d(ax, axes="xyz"):
```

### Comparing `beat-2.0.0/beat/plotting/ffi.py` & `beat-2.0.1/beat/plotting/ffi.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/beat/plotting/geodetic.py` & `beat-2.0.1/beat/plotting/geodetic.py`

 * *Files 4% similar despite different names*

```diff
@@ -214,19 +214,19 @@
                 )
             )
 
         all_var_reductions = {}
         bvar_reductions_comp = {}
         for dataset in dataset_to_result.keys():
             target_var_reds = []
-            target_bvar_red = bvar_reductions[dataset.name]
+            target_bvar_red = bvar_reductions[dataset.id]
             target_var_reds.append(target_bvar_red)
             bvar_reductions_comp[dataset.component] = target_bvar_red * 100.0
             for var_reds in ens_var_reductions:
-                target_var_reds.append(var_reds[dataset.name])
+                target_var_reds.append(var_reds[dataset.id])
 
             all_var_reductions[dataset.component] = num.array(target_var_reds) * 100.0
 
     radius = otd.distance_accurate50m_numpy(
         lat[num.newaxis], lon[num.newaxis], coords[:, 0], coords[:, 1]
     ).max()
 
@@ -369,27 +369,41 @@
                 var_reductions_ens = num.mean(var_reductions_tmp, axis=0)
 
             # draw white background box for histogram
             m.gmt.psbasemap(D="n0.722/0.716+w4c/4c", F="+gwhite+p0.25p", *m.jxyr)
 
             # get resulting bounds no plotting
             vmin, vmax = var_reductions_ens.min(), var_reductions_ens.max()
+            vspread = num.abs(vmax - vmin)
+            if vspread < 1e-4:
+                logger.warning(
+                    "Spread in Variance Reduction is too small: %f, "
+                    "skipping histogram plot!" % vspread
+                )
+                figs.append(m)
+                continue
+            # axis bounds
             imin, imax, sinc = get_nice_plot_bounds(vmin, vmax)
-            nbins = 50
+            # hist bins
             Z = 0
+            W = (imax - imin) / 30
+            # T = "%s/%s/%s+i" % (imin, imax, 0.1) this is buggy
 
             out_filename = "/tmp/histbounds.txt"
+            in_rows = num.atleast_2d(var_reductions_ens).T
+
             m.gmt.pshistogram(
-                in_rows=num.atleast_2d(all_var_reductions[dataset.component]),
-                W=(imax - imin) / nbins,
+                in_rows=in_rows,
+                # T=T,
+                W=W,
                 out_filename=out_filename,
                 Z=Z,
                 I="o",
             )
-            bin_bounds = num.loadtxt(out_filename).max(0)
+            bin_bounds = num.atleast_2d(num.loadtxt(out_filename)).max(0)
             bmin, bmax, binc = get_nice_plot_bounds(0, bin_bounds[1])
 
             # set data region
             jxyr = [
                 "-JX4c/4c",
                 "-Xf13.5c",
                 "-Yf13.4c",
@@ -399,28 +413,29 @@
             hist_args = [
                 "-Bxa%ff%f+lVR [%s]" % (sinc, sinc, "%"),
                 "-Bya%i" % binc,
                 "-BwSne",
             ] + jxyr
 
             m.gmt.pshistogram(
-                in_rows=num.atleast_2d(all_var_reductions[dataset.component]),
-                W=(imax - imin) / nbins,
+                in_rows=in_rows,
+                W=W,
+                # T=T,
                 G="lightorange",
                 Z=Z,
                 F=True,
                 L="0.5p,orange",
                 *hist_args,
             )
 
             # plot vertical line on hist with best solution
             m.gmt.psxy(
                 in_rows=(
-                    [bvar_reductions_comp[dataset.component], 0],
-                    [bvar_reductions_comp[dataset.component], po.nensemble],
+                    [var_reductions_ens[0], 0],
+                    [var_reductions_ens[0], po.nensemble],
                 ),
                 W="1.5p,red",
                 *jxyr,
             )
 
         figs.append(m)
 
@@ -528,15 +543,15 @@
     # to display standardized residuals
     stdz_residuals = composite.get_standardized_residuals(
         bpoint, results=bresults_tmp, weights=composite.weights
     )
 
     if po.plot_projection == "individual":
         for result, dataset in zip(bresults_tmp, composite.datasets):
-            result.processed_res = stdz_residuals[dataset.name]
+            result.processed_res = stdz_residuals[dataset.id]
 
     bvar_reductions = composite.get_variance_reductions(
         bpoint, weights=composite.weights, results=bresults_tmp
     )
 
     dataset_to_result = {}
     for dataset, bresult in zip(composite.datasets, bresults_tmp):
@@ -584,19 +599,19 @@
                     point, weights=composite.weights, results=e_results
                 )
             )
 
         all_var_reductions = {}
         for dataset in dataset_to_result.keys():
             target_var_reds = []
-            target_var_reds.append(bvar_reductions[dataset.name])
+            target_var_reds.append(bvar_reductions[dataset.id])
             for var_reds in ens_var_reductions:
-                target_var_reds.append(var_reds[dataset.name])
+                target_var_reds.append(var_reds[dataset.id])
 
-            all_var_reductions[dataset.name] = num.array(target_var_reds) * 100.0
+            all_var_reductions[dataset.id] = num.array(target_var_reds) * 100.0
 
     figures = []
     axes = []
     for f in factors:
         figsize = list(mpl_papersize("a4", "portrait"))
         figsize[1] *= f
 
@@ -877,15 +892,15 @@
             logger.info("Plotting %s" % data_str)
             datavec = getattr(result, "processed_%s" % data_str)
 
             if data_str == "res" and po.plot_projection in ["local", "individual"]:
                 vmin = -dcolims[tidx]
                 vmax = dcolims[tidx]
                 logger.debug(
-                    "Variance of residual for %s is: %f", dataset.name, datavec.var()
+                    "Variance of residual for %s is: %f", dataset.id, datavec.var()
                 )
             else:
                 vmin = -colims[tidx]
                 vmax = colims[tidx]
 
             data = map_displacement_grid(datavec, scene)
 
@@ -941,16 +956,16 @@
                 in_ax_res, remove=["right", "bottom"], visible=True, linewidth=0.75
             )
             in_ax_res.set_xlabel(r"std. res. [$\sigma$]", fontsize=fontsize - 3)
 
         if po.nensemble > 1:
             in_ax = plot_inset_hist(
                 axs[2],
-                data=num.atleast_2d(all_var_reductions[dataset.name]),
-                best_data=bvar_reductions[dataset.name] * 100.0,
+                data=num.atleast_2d(all_var_reductions[dataset.id]),
+                best_data=bvar_reductions[dataset.id] * 100.0,
                 linewidth=1.0,
                 bbox_to_anchor=(0.75, 0.775, 0.25, 0.225),
                 labelsize=6,
             )
 
             format_axes(in_ax, remove=["left", "bottom"], visible=True, linewidth=0.75)
             in_ax.set_xlabel("VR [%]", fontsize=fontsize - 3)
```

### Comparing `beat-2.0.0/beat/plotting/marginals.py` & `beat-2.0.1/beat/plotting/marginals.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/beat/plotting/seismic.py` & `beat-2.0.1/beat/plotting/seismic.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/beat/pytensorf.py` & `beat-2.0.1/beat/pytensorf.py`

 * *Files 0% similar despite different names*

```diff
@@ -543,15 +543,15 @@
         pole_lon = point["lon"]
         omega = point["omega"]
 
         velocities = heart.velocities_from_pole(
             num.array(self.lats), num.array(self.lons), pole_lat, pole_lon, omega
         )
 
-        if self.data_mask:
+        if len(self.data_mask) > 0:
             velocities[num.array(self.data_mask), :] = 0.0
 
         z[0] = velocities
 
     def infer_shape(self, fgraph=None, node=None, input_shapes=None):
         return [(len(self.lats), 3)]
```

### Comparing `beat-2.0.0/beat/sampler/base.py` & `beat-2.0.1/beat/sampler/base.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/beat/sampler/distributed.py` & `beat-2.0.1/beat/sampler/distributed.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/beat/sampler/metropolis.py` & `beat-2.0.1/beat/sampler/metropolis.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/beat/sampler/pt.py` & `beat-2.0.1/beat/sampler/pt.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/beat/sampler/smc.py` & `beat-2.0.1/beat/sampler/smc.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/beat/sources.py` & `beat-2.0.1/beat/sources.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/beat/upgrade.py` & `beat-2.0.1/beat/upgrade.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/beat/utility.py` & `beat-2.0.1/beat/utility.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/beat/voronoi/voronoi.py` & `beat-2.0.1/beat/voronoi/voronoi.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/beat/voronoi/voronoi_ext.c` & `beat-2.0.1/beat/voronoi/voronoi_ext.c`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/beat.egg-info/PKG-INFO` & `beat-2.0.1/beat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beat
-Version: 2.0.0
+Version: 2.0.1
 Summary: 'Bayesian Earthquake Analysis Tool'
 Author-email: Hannes Vasyura-Bathke <vasbath@gfz-potsdam.de>
 Maintainer-email: Hannes Vasyura-Bathke <vasbath@gfz-potsdam.de>
 License: GPLv3
 Project-URL: Home, https://pyrocko.org/beat
 Project-URL: GitHub, https://github.com/hvasbath/beat
 Project-URL: Issues, https://github.com/hvasbath/beat/issues
```

### Comparing `beat-2.0.0/beat.egg-info/SOURCES.txt` & `beat-2.0.1/beat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/pyproject.toml` & `beat-2.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0.0", "oldest-supported-numpy"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "beat"
-version = "2.0.0"
+version = "2.0.1"
 requires-python = ">=3.9"
 license = {text = "GPLv3"}
 description = "'Bayesian Earthquake Analysis Tool'"
 readme = "README.md"
 authors = [
   {name = "Hannes Vasyura-Bathke", email = "vasbath@gfz-potsdam.de"}
 ]
```

### Comparing `beat-2.0.0/setup.py` & `beat-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from distutils.sysconfig import get_python_inc
 
 from setuptools import Extension, setup
 
 op = os.path
 
 packname = "beat"
-version = "2.0.0"
+version = "2.0.1"
 
 
 try:
     import numpy
 except ImportError:
 
     class numpy:
```

### Comparing `beat-2.0.0/test/test_backend.py` & `beat-2.0.1/test/test_backend.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/test/test_bem.py` & `beat-2.0.1/test/test_bem.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/test/test_composites.py` & `beat-2.0.1/test/test_composites.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/test/test_config.py` & `beat-2.0.1/test/test_config.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/test/test_covariance.py` & `beat-2.0.1/test/test_covariance.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/test/test_distributed.py` & `beat-2.0.1/test/test_distributed.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/test/test_fastsweep.py` & `beat-2.0.1/test/test_fastsweep.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/test/test_ffi.py` & `beat-2.0.1/test/test_ffi.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/test/test_ffi_gfstacking.py` & `beat-2.0.1/test/test_ffi_gfstacking.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/test/test_ffi_gfstacking_multifault.py` & `beat-2.0.1/test/test_ffi_gfstacking_multifault.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/test/test_geodetic.py` & `beat-2.0.1/test/test_geodetic.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/test/test_heart.py` & `beat-2.0.1/test/test_heart.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/test/test_laplacian.py` & `beat-2.0.1/test/test_laplacian.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/test/test_models.py` & `beat-2.0.1/test/test_models.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/test/test_paripool.py` & `beat-2.0.1/test/test_paripool.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/test/test_plotting.py` & `beat-2.0.1/test/test_plotting.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/test/test_proposals.py` & `beat-2.0.1/test/test_proposals.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/test/test_pt.py` & `beat-2.0.1/test/test_pt.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/test/test_resolution_subsampling.py` & `beat-2.0.1/test/test_resolution_subsampling.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/test/test_sampler.py` & `beat-2.0.1/test/test_sampler.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/test/test_smc.py` & `beat-2.0.1/test/test_smc.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/test/test_sources.py` & `beat-2.0.1/test/test_sources.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/test/test_utility.py` & `beat-2.0.1/test/test_utility.py`

 * *Files identical despite different names*

### Comparing `beat-2.0.0/test/test_voronoi.py` & `beat-2.0.1/test/test_voronoi.py`

 * *Files identical despite different names*

