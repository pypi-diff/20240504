# Comparing `tmp/Bottleneck-1.3.8rc5.tar.gz` & `tmp/bottleneck-1.4.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bottleneck-1.3.8rc5.tar", last modified: Sat Feb 24 01:52:54 2024, max compression
+gzip compressed data, was "bottleneck-1.4.0rc4.tar", last modified: Sat May  4 14:45:02 2024, max compression
```

## Comparing `Bottleneck-1.3.8rc5.tar` & `bottleneck-1.4.0rc4.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:52:54.720473 Bottleneck-1.3.8rc5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:52:54.720473 Bottleneck-1.3.8rc5/Bottleneck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-02-24 01:52:54.000000 Bottleneck-1.3.8rc5/Bottleneck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-02-24 01:52:54.000000 Bottleneck-1.3.8rc5/Bottleneck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-24 01:52:54.000000 Bottleneck-1.3.8rc5/Bottleneck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-24 01:52:54.000000 Bottleneck-1.3.8rc5/Bottleneck.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-24 01:52:54.000000 Bottleneck-1.3.8rc5/Bottleneck.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-24 01:52:54.000000 Bottleneck-1.3.8rc5/Bottleneck.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:52:54.708473 Bottleneck-1.3.8rc5/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/LICENSES/NUMPY_LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/LICENSES/PANDAS_LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/LICENSES/SCIPY_LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/LICENSES/SETUPTOOLS_LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-02-24 01:52:54.720473 Bottleneck-1.3.8rc5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)    18303 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/RELEASE.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:52:54.724473 Bottleneck-1.3.8rc5/bottleneck/
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/_pytesttester.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-02-24 01:52:54.724473 Bottleneck-1.3.8rc5/bottleneck/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:52:54.708473 Bottleneck-1.3.8rc5/bottleneck/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/benchmark/autotimeit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/benchmark/bench.py
--rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/benchmark/bench_detailed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:52:54.708473 Bottleneck-1.3.8rc5/bottleneck/slow/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/slow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7799 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/slow/move.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/slow/nonreduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/slow/nonreduce_axis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/slow/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:52:54.712473 Bottleneck-1.3.8rc5/bottleneck/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/src/bn_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/src/bn_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/src/bottleneck.h
--rw-r--r--   0 runner    (1001) docker     (127)    11899 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/src/iterators.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:52:54.712473 Bottleneck-1.3.8rc5/bottleneck/src/move_median/
--rw-r--r--   0 runner    (1001) docker     (127)    22210 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/src/move_median/move_median.c
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/src/move_median/move_median.h
--rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/src/move_median/move_median_debug.c
--rw-r--r--   0 runner    (1001) docker     (127)    44305 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/src/move_template.c
--rw-r--r--   0 runner    (1001) docker     (127)    29643 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/src/nonreduce_axis_template.c
--rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/src/nonreduce_template.c
--rw-r--r--   0 runner    (1001) docker     (127)    47002 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/src/reduce_template.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:52:54.712473 Bottleneck-1.3.8rc5/bottleneck/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/tests/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:52:54.700473 Bottleneck-1.3.8rc5/bottleneck/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:52:54.712473 Bottleneck-1.3.8rc5/bottleneck/tests/data/template_test/
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/tests/data/template_test/test_template.c
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/tests/data/template_test/truth.c
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/tests/input_modification_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/tests/list_input_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/tests/memory_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7644 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/tests/move_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7600 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/tests/nonreduce_axis_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/tests/nonreduce_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/tests/reduce_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/tests/scalar_input_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/tests/test_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/bottleneck/tests/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:52:54.712473 Bottleneck-1.3.8rc5/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/doc_howto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:52:54.716473 Bottleneck-1.3.8rc5/doc/image/
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/image/icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/image/icon.xcf
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/image/icon14.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:52:54.716473 Bottleneck-1.3.8rc5/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:52:54.716473 Bottleneck-1.3.8rc5/doc/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/bottleneck.benchmark.rst
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/bottleneck.move.rst
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/bottleneck.nonreduce.rst
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/bottleneck.nonreduce_axis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/bottleneck.reduce.rst
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/bottleneck.rst
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/bottleneck.slow.rst
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/bottleneck.src.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/bottleneck.tests.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7544 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/installing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/release.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:52:54.720473 Bottleneck-1.3.8rc5/doc/source/releases/
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/releases/RELEASE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/releases/v0.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/releases/v0.2.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/releases/v0.3.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/releases/v0.4.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/releases/v0.4.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/releases/v0.4.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/releases/v0.4.3.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/releases/v0.5.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/releases/v0.6.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/releases/v0.7.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/releases/v0.8.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/releases/v1.0.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/releases/v1.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/releases/v1.2.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/releases/v1.2.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/releases/v1.3.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/releases/v1.3.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/releases/v1.3.2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/source/releases/v1.4.0.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:52:54.720473 Bottleneck-1.3.8rc5/doc/sphinxext/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3912 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/sphinxext/announce.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/doc/sphinxext/contributors.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-02-24 01:52:54.720473 Bottleneck-1.3.8rc5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    81180 2024-02-24 01:52:45.000000 Bottleneck-1.3.8rc5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:45:02.643214 bottleneck-1.4.0rc4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:45:02.639214 bottleneck-1.4.0rc4/Bottleneck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-05-04 14:45:02.000000 bottleneck-1.4.0rc4/Bottleneck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-04 14:45:02.000000 bottleneck-1.4.0rc4/Bottleneck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 14:45:02.000000 bottleneck-1.4.0rc4/Bottleneck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 14:45:02.000000 bottleneck-1.4.0rc4/Bottleneck.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-04 14:45:02.000000 bottleneck-1.4.0rc4/Bottleneck.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 14:45:02.000000 bottleneck-1.4.0rc4/Bottleneck.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:45:02.627214 bottleneck-1.4.0rc4/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/LICENSES/NUMPY_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/LICENSES/PANDAS_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/LICENSES/SCIPY_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/LICENSES/SETUPTOOLS_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-05-04 14:45:02.643214 bottleneck-1.4.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    18303 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/RELEASE.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:45:02.643214 bottleneck-1.4.0rc4/bottleneck/
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/_pytesttester.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-04 14:45:02.643214 bottleneck-1.4.0rc4/bottleneck/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:45:02.627214 bottleneck-1.4.0rc4/bottleneck/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/benchmark/autotimeit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/benchmark/bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/benchmark/bench_detailed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:45:02.627214 bottleneck-1.4.0rc4/bottleneck/slow/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/slow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7799 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/slow/move.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/slow/nonreduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/slow/nonreduce_axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/slow/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:45:02.631214 bottleneck-1.4.0rc4/bottleneck/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/src/bn_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/src/bn_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/src/bottleneck.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11899 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/src/iterators.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:45:02.631214 bottleneck-1.4.0rc4/bottleneck/src/move_median/
+-rw-r--r--   0 runner    (1001) docker     (127)    22210 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/src/move_median/move_median.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/src/move_median/move_median.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/src/move_median/move_median_debug.c
+-rw-r--r--   0 runner    (1001) docker     (127)    44305 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/src/move_template.c
+-rw-r--r--   0 runner    (1001) docker     (127)    29643 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/src/nonreduce_axis_template.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/src/nonreduce_template.c
+-rw-r--r--   0 runner    (1001) docker     (127)    47002 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/src/reduce_template.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:45:02.635214 bottleneck-1.4.0rc4/bottleneck/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/tests/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:45:02.623214 bottleneck-1.4.0rc4/bottleneck/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:45:02.635214 bottleneck-1.4.0rc4/bottleneck/tests/data/template_test/
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/tests/data/template_test/test_template.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/tests/data/template_test/truth.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/tests/input_modification_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/tests/list_input_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/tests/memory_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7644 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/tests/move_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7600 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/tests/nonreduce_axis_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/tests/nonreduce_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/tests/reduce_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/tests/scalar_input_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/tests/test_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/bottleneck/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:45:02.635214 bottleneck-1.4.0rc4/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/doc_howto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:45:02.635214 bottleneck-1.4.0rc4/doc/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/image/icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/image/icon.xcf
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/image/icon14.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:45:02.635214 bottleneck-1.4.0rc4/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:45:02.635214 bottleneck-1.4.0rc4/doc/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/bottleneck.benchmark.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/bottleneck.move.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/bottleneck.nonreduce.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/bottleneck.nonreduce_axis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/bottleneck.reduce.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/bottleneck.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/bottleneck.slow.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/bottleneck.src.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/bottleneck.tests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7544 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/release.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:45:02.639214 bottleneck-1.4.0rc4/doc/source/releases/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/releases/RELEASE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/releases/v0.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/releases/v0.2.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/releases/v0.3.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/releases/v0.4.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/releases/v0.4.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/releases/v0.4.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/releases/v0.4.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/releases/v0.5.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/releases/v0.6.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/releases/v0.7.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/releases/v0.8.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/releases/v1.0.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/releases/v1.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/releases/v1.2.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/releases/v1.2.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/releases/v1.3.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/releases/v1.3.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/releases/v1.3.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/source/releases/v1.4.0.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:45:02.639214 bottleneck-1.4.0rc4/doc/sphinxext/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3912 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/sphinxext/announce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/doc/sphinxext/contributors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-04 14:45:02.643214 bottleneck-1.4.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6271 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81180 2024-05-04 14:44:56.000000 bottleneck-1.4.0rc4/versioneer.py
```

### Comparing `Bottleneck-1.3.8rc5/Bottleneck.egg-info/PKG-INFO` & `bottleneck-1.4.0rc4/Bottleneck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bottleneck
-Version: 1.3.8rc5
+Version: 1.4.0rc4
 Summary: Fast NumPy array functions written in C
 Home-page: https://github.com/pydata/bottleneck
 Download-URL: http://pypi.python.org/pypi/Bottleneck
 Maintainer: Christopher Whelan
 Maintainer-email: bottle-neck@googlegroups.com
 License: Simplified BSD
 Platform: OS Independent
```

### Comparing `Bottleneck-1.3.8rc5/Bottleneck.egg-info/SOURCES.txt` & `bottleneck-1.4.0rc4/Bottleneck.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/LICENSE` & `bottleneck-1.4.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/LICENSES/NUMPY_LICENSE` & `bottleneck-1.4.0rc4/LICENSES/NUMPY_LICENSE`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/LICENSES/PANDAS_LICENSE` & `bottleneck-1.4.0rc4/LICENSES/PANDAS_LICENSE`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/LICENSES/SCIPY_LICENSE` & `bottleneck-1.4.0rc4/LICENSES/SCIPY_LICENSE`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/LICENSES/SETUPTOOLS_LICENSE` & `bottleneck-1.4.0rc4/LICENSES/SETUPTOOLS_LICENSE`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/Makefile` & `bottleneck-1.4.0rc4/Makefile`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/PKG-INFO` & `bottleneck-1.4.0rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bottleneck
-Version: 1.3.8rc5
+Version: 1.4.0rc4
 Summary: Fast NumPy array functions written in C
 Home-page: https://github.com/pydata/bottleneck
 Download-URL: http://pypi.python.org/pypi/Bottleneck
 Maintainer: Christopher Whelan
 Maintainer-email: bottle-neck@googlegroups.com
 License: Simplified BSD
 Platform: OS Independent
```

### Comparing `Bottleneck-1.3.8rc5/README.rst` & `bottleneck-1.4.0rc4/README.rst`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/RELEASE.rst` & `bottleneck-1.4.0rc4/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/__init__.py` & `bottleneck-1.4.0rc4/bottleneck/__init__.py`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/_pytesttester.py` & `bottleneck-1.4.0rc4/bottleneck/_pytesttester.py`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/benchmark/bench.py` & `bottleneck-1.4.0rc4/bottleneck/benchmark/bench.py`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/benchmark/bench_detailed.py` & `bottleneck-1.4.0rc4/bottleneck/benchmark/bench_detailed.py`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/slow/move.py` & `bottleneck-1.4.0rc4/bottleneck/slow/move.py`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/slow/nonreduce.py` & `bottleneck-1.4.0rc4/bottleneck/slow/nonreduce.py`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/slow/nonreduce_axis.py` & `bottleneck-1.4.0rc4/bottleneck/slow/nonreduce_axis.py`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/slow/reduce.py` & `bottleneck-1.4.0rc4/bottleneck/slow/reduce.py`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/src/bn_config.py` & `bottleneck-1.4.0rc4/bottleneck/src/bn_config.py`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/src/bn_template.py` & `bottleneck-1.4.0rc4/bottleneck/src/bn_template.py`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/src/bottleneck.h` & `bottleneck-1.4.0rc4/bottleneck/src/bottleneck.h`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/src/iterators.h` & `bottleneck-1.4.0rc4/bottleneck/src/iterators.h`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/src/move_median/move_median.c` & `bottleneck-1.4.0rc4/bottleneck/src/move_median/move_median.c`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/src/move_median/move_median.h` & `bottleneck-1.4.0rc4/bottleneck/src/move_median/move_median.h`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/src/move_median/move_median_debug.c` & `bottleneck-1.4.0rc4/bottleneck/src/move_median/move_median_debug.c`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/src/move_template.c` & `bottleneck-1.4.0rc4/bottleneck/src/move_template.c`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/src/nonreduce_axis_template.c` & `bottleneck-1.4.0rc4/bottleneck/src/nonreduce_axis_template.c`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/src/nonreduce_template.c` & `bottleneck-1.4.0rc4/bottleneck/src/nonreduce_template.c`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/src/reduce_template.c` & `bottleneck-1.4.0rc4/bottleneck/src/reduce_template.c`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/tests/data/template_test/test_template.c` & `bottleneck-1.4.0rc4/bottleneck/tests/data/template_test/test_template.c`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/tests/data/template_test/truth.c` & `bottleneck-1.4.0rc4/bottleneck/tests/data/template_test/truth.c`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/tests/input_modification_test.py` & `bottleneck-1.4.0rc4/bottleneck/tests/input_modification_test.py`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/tests/list_input_test.py` & `bottleneck-1.4.0rc4/bottleneck/tests/list_input_test.py`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/tests/memory_test.py` & `bottleneck-1.4.0rc4/bottleneck/tests/memory_test.py`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/tests/move_test.py` & `bottleneck-1.4.0rc4/bottleneck/tests/move_test.py`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/tests/nonreduce_axis_test.py` & `bottleneck-1.4.0rc4/bottleneck/tests/nonreduce_axis_test.py`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/tests/nonreduce_test.py` & `bottleneck-1.4.0rc4/bottleneck/tests/nonreduce_test.py`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/tests/reduce_test.py` & `bottleneck-1.4.0rc4/bottleneck/tests/reduce_test.py`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/tests/scalar_input_test.py` & `bottleneck-1.4.0rc4/bottleneck/tests/scalar_input_test.py`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/tests/test_template.py` & `bottleneck-1.4.0rc4/bottleneck/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/bottleneck/tests/util.py` & `bottleneck-1.4.0rc4/bottleneck/tests/util.py`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/doc/image/icon.png` & `bottleneck-1.4.0rc4/doc/image/icon.png`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/doc/image/icon.xcf` & `bottleneck-1.4.0rc4/doc/image/icon.xcf`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/doc/image/icon14.png` & `bottleneck-1.4.0rc4/doc/image/icon14.png`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/doc/source/bottleneck.benchmark.rst` & `bottleneck-1.4.0rc4/doc/source/bottleneck.benchmark.rst`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/doc/source/bottleneck.slow.rst` & `bottleneck-1.4.0rc4/doc/source/bottleneck.slow.rst`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/doc/source/bottleneck.tests.rst` & `bottleneck-1.4.0rc4/doc/source/bottleneck.tests.rst`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/doc/source/conf.py` & `bottleneck-1.4.0rc4/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/doc/source/installing.rst` & `bottleneck-1.4.0rc4/doc/source/installing.rst`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/doc/source/license.rst` & `bottleneck-1.4.0rc4/doc/source/license.rst`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/doc/source/reference.rst` & `bottleneck-1.4.0rc4/doc/source/reference.rst`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/doc/source/releases/RELEASE.rst` & `bottleneck-1.4.0rc4/doc/source/releases/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/doc/source/releases/v0.2.0.rst` & `bottleneck-1.4.0rc4/doc/source/releases/v0.2.0.rst`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/doc/source/releases/v0.3.0.rst` & `bottleneck-1.4.0rc4/doc/source/releases/v0.3.0.rst`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/doc/source/releases/v0.4.0.rst` & `bottleneck-1.4.0rc4/doc/source/releases/v0.4.0.rst`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/doc/source/releases/v0.5.0.rst` & `bottleneck-1.4.0rc4/doc/source/releases/v0.5.0.rst`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/doc/source/releases/v0.6.0.rst` & `bottleneck-1.4.0rc4/doc/source/releases/v0.6.0.rst`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/doc/source/releases/v0.7.0.rst` & `bottleneck-1.4.0rc4/doc/source/releases/v0.7.0.rst`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/doc/source/releases/v1.0.0.rst` & `bottleneck-1.4.0rc4/doc/source/releases/v1.0.0.rst`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/doc/source/releases/v1.1.0.rst` & `bottleneck-1.4.0rc4/doc/source/releases/v1.1.0.rst`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/doc/source/releases/v1.2.0.rst` & `bottleneck-1.4.0rc4/doc/source/releases/v1.2.0.rst`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/doc/source/releases/v1.2.1.rst` & `bottleneck-1.4.0rc4/doc/source/releases/v1.2.1.rst`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/doc/source/releases/v1.3.0.rst` & `bottleneck-1.4.0rc4/doc/source/releases/v1.3.0.rst`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/doc/sphinxext/announce.py` & `bottleneck-1.4.0rc4/doc/sphinxext/announce.py`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/doc/sphinxext/contributors.py` & `bottleneck-1.4.0rc4/doc/sphinxext/contributors.py`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/setup.cfg` & `bottleneck-1.4.0rc4/setup.cfg`

 * *Files identical despite different names*

### Comparing `Bottleneck-1.3.8rc5/setup.py` & `bottleneck-1.4.0rc4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,14 +192,17 @@
         "bottleneck": ["LICENSE"],
         "bottleneck.tests": ["data/*/*"],
     },
     requires=["numpy"],
     install_requires=["numpy"],
     extras_require={"doc": ["numpydoc", "sphinx", "gitpython"]},
     cmdclass=cmdclass,
-    setup_requires=["numpy"],
+    setup_requires=[
+        "oldest-supported-numpy ; python_version < '3.9'",
+        "numpy>=2.0.0rc1 ; python_version >= '3.9'"
+    ],
     ext_modules=prepare_modules(),
     zip_safe=False,
 )
 
 
 setup(**metadata)
```

### Comparing `Bottleneck-1.3.8rc5/versioneer.py` & `bottleneck-1.4.0rc4/versioneer.py`

 * *Files identical despite different names*

