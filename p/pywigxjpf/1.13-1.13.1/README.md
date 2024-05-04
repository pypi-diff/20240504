# Comparing `tmp/pywigxjpf-1.13.tar.gz` & `tmp/pywigxjpf-1.13.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywigxjpf-1.13.tar", last modified: Sat May  4 10:18:04 2024, max compression
+gzip compressed data, was "pywigxjpf-1.13.1.tar", last modified: Sat May  4 10:37:44 2024, max compression
```

## Comparing `pywigxjpf-1.13.tar` & `pywigxjpf-1.13.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-05-04 10:18:04.742176 pywigxjpf-1.13/
--rw-r--r--   0 htj       (1001) f2b      (30425)     2017 2024-05-04 10:17:31.000000 pywigxjpf-1.13/CHANGELOG
--rw-r--r--   0 htj       (1001) f2b      (30425)    35147 2024-05-04 10:17:31.000000 pywigxjpf-1.13/COPYING
--rw-r--r--   0 htj       (1001) f2b      (30425)     7651 2024-05-04 10:17:31.000000 pywigxjpf-1.13/COPYING.LESSER
--rw-r--r--   0 htj       (1001) f2b      (30425)      124 2024-05-04 10:17:32.000000 pywigxjpf-1.13/MANIFEST.in
--rw-r--r--   0 htj       (1001) f2b      (30425)     1915 2024-05-04 10:18:04.742176 pywigxjpf-1.13/PKG-INFO
--rw-r--r--   0 htj       (1001) f2b      (30425)    10546 2024-05-04 10:17:31.000000 pywigxjpf-1.13/README
-drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-05-04 10:18:04.642174 pywigxjpf-1.13/cfg/
--rw-r--r--   0 htj       (1001) f2b      (30425)     3939 2024-05-04 10:17:32.000000 pywigxjpf-1.13/cfg/wigxjpf_config.h
-drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-05-04 10:18:04.678175 pywigxjpf-1.13/example/
--rw-r--r--   0 htj       (1001) f2b      (30425)     1015 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/ccsimple.cc
--rw-r--r--   0 htj       (1001) f2b      (30425)      202 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/ccsimple.good
--rw-r--r--   0 htj       (1001) f2b      (30425)     1417 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/cfail.c
--rw-r--r--   0 htj       (1001) f2b      (30425)     1328 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/cfail.expect
--rw-r--r--   0 htj       (1001) f2b      (30425)      761 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/csimple.c
--rw-r--r--   0 htj       (1001) f2b      (30425)      200 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/csimple.good
--rw-r--r--   0 htj       (1001) f2b      (30425)     1706 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/cthreadedsimple.c
--rw-r--r--   0 htj       (1001) f2b      (30425)       50 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/cthreadedsimple.good
--rw-r--r--   0 htj       (1001) f2b      (30425)      384 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/evaltable.huge.good
--rw-r--r--   0 htj       (1001) f2b      (30425)      644 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/evaltable.large.good
--rwxr-xr-x   0 htj       (1001) f2b      (30425)     4236 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/evaltable.sh
--rw-r--r--   0 htj       (1001) f2b      (30425)    11835 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/evaltable.small.good
--rw-r--r--   0 htj       (1001) f2b      (30425)     1941 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/fsimple.f
--rw-r--r--   0 htj       (1001) f2b      (30425)      227 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/fsimple.good
--rw-r--r--   0 htj       (1001) f2b      (30425)     3364 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/py_numba.py
--rw-r--r--   0 htj       (1001) f2b      (30425)     8320 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/pyfail.expect
--rw-r--r--   0 htj       (1001) f2b      (30425)     3128 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/pyfail.py
--rw-r--r--   0 htj       (1001) f2b      (30425)      340 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/pysimple.good
--rwxr-xr-x   0 htj       (1001) f2b      (30425)     1936 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/pysimple.py
--rw-r--r--   0 htj       (1001) f2b      (30425)     7768 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/wigxjpf.c
-drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-05-04 10:18:04.686175 pywigxjpf-1.13/inc/
--rw-r--r--   0 htj       (1001) f2b      (30425)     1755 2024-05-04 10:17:32.000000 pywigxjpf-1.13/inc/fpsimplexj.h
--rw-r--r--   0 htj       (1001) f2b      (30425)     4080 2024-05-04 10:17:32.000000 pywigxjpf-1.13/inc/wigxjpf.h
--rw-r--r--   0 htj       (1001) f2b      (30425)     2154 2024-05-04 10:17:32.000000 pywigxjpf-1.13/inc/wigxjpf_quadmath.h
-drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-05-04 10:18:04.690175 pywigxjpf-1.13/pywigxjpf/
--rw-r--r--   0 htj       (1001) f2b      (30425)      381 2024-05-04 10:17:32.000000 pywigxjpf-1.13/pywigxjpf/__init__.py
-drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-05-04 10:18:04.702175 pywigxjpf-1.13/pywigxjpf/pregen/
--rw-r--r--   0 htj       (1001) f2b      (30425)      168 2024-05-04 10:17:32.000000 pywigxjpf-1.13/pywigxjpf/pregen/wigxjpf_auto_config.h
--rw-r--r--   0 htj       (1001) f2b      (30425)     3970 2024-05-04 10:17:32.000000 pywigxjpf-1.13/pywigxjpf/pywigxjpf.py
--rw-r--r--   0 htj       (1001) f2b      (30425)     2379 2024-05-04 10:17:32.000000 pywigxjpf-1.13/pywigxjpf/pywigxjpf_ffi_builder.py
-drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-05-04 10:18:04.698175 pywigxjpf-1.13/pywigxjpf.egg-info/
--rw-r--r--   0 htj       (1001) f2b      (30425)     1915 2024-05-04 10:18:04.000000 pywigxjpf-1.13/pywigxjpf.egg-info/PKG-INFO
--rw-r--r--   0 htj       (1001) f2b      (30425)     1262 2024-05-04 10:18:04.000000 pywigxjpf-1.13/pywigxjpf.egg-info/SOURCES.txt
--rw-r--r--   0 htj       (1001) f2b      (30425)        1 2024-05-04 10:18:04.000000 pywigxjpf-1.13/pywigxjpf.egg-info/dependency_links.txt
--rw-r--r--   0 htj       (1001) f2b      (30425)       18 2024-05-04 10:18:04.000000 pywigxjpf-1.13/pywigxjpf.egg-info/requires.txt
--rw-r--r--   0 htj       (1001) f2b      (30425)       24 2024-05-04 10:18:04.000000 pywigxjpf-1.13/pywigxjpf.egg-info/top_level.txt
--rw-r--r--   0 htj       (1001) f2b      (30425)       38 2024-05-04 10:18:04.746176 pywigxjpf-1.13/setup.cfg
--rw-r--r--   0 htj       (1001) f2b      (30425)     2512 2024-05-04 10:17:32.000000 pywigxjpf-1.13/setup.py
-drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-05-04 10:18:04.742176 pywigxjpf-1.13/src/
--rw-r--r--   0 htj       (1001) f2b      (30425)     3871 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/c_wrap.c
--rw-r--r--   0 htj       (1001) f2b      (30425)     1037 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/c_wrap.h
--rw-r--r--   0 htj       (1001) f2b      (30425)     1586 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/c_wrap_float128.c
--rw-r--r--   0 htj       (1001) f2b      (30425)    21866 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/calc.c
--rw-r--r--   0 htj       (1001) f2b      (30425)     3483 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/calc.h
--rw-r--r--   0 htj       (1001) f2b      (30425)     4430 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/calc_dbl.h
--rw-r--r--   0 htj       (1001) f2b      (30425)     1070 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/calc_float128.c
--rw-r--r--   0 htj       (1001) f2b      (30425)     1301 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/calc_minmax.h
--rw-r--r--   0 htj       (1001) f2b      (30425)     2583 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/fortran_wrap.c
--rw-r--r--   0 htj       (1001) f2b      (30425)     8335 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/fpsimple.c
--rw-r--r--   0 htj       (1001) f2b      (30425)     7582 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/fpsimple_log.c
--rw-r--r--   0 htj       (1001) f2b      (30425)     1688 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/fpsimple_precalc.c
--rw-r--r--   0 htj       (1001) f2b      (30425)     1284 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/fwigxjpf.f
--rw-r--r--   0 htj       (1001) f2b      (30425)    10366 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/multi_word_int.h
--rw-r--r--   0 htj       (1001) f2b      (30425)     2039 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/multi_word_int_dbl.h
--rw-r--r--   0 htj       (1001) f2b      (30425)     1228 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/multi_word_int_float128.h
--rw-r--r--   0 htj       (1001) f2b      (30425)     8051 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/prime_factor.c
--rw-r--r--   0 htj       (1001) f2b      (30425)    15244 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/prime_factor.h
--rw-r--r--   0 htj       (1001) f2b      (30425)     2359 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/test_cc_dbl.c
--rw-r--r--   0 htj       (1001) f2b      (30425)     3393 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/trivial_zero.c
--rw-r--r--   0 htj       (1001) f2b      (30425)     1420 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/wigxjpf_error.c
--rw-r--r--   0 htj       (1001) f2b      (30425)     1970 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/wigxjpf_error.h
+drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-05-04 10:37:44.780609 pywigxjpf-1.13.1/
+-rw-r--r--   0 htj       (1001) f2b      (30425)     2017 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/CHANGELOG
+-rw-r--r--   0 htj       (1001) f2b      (30425)    35147 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/COPYING
+-rw-r--r--   0 htj       (1001) f2b      (30425)     7651 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/COPYING.LESSER
+-rw-r--r--   0 htj       (1001) f2b      (30425)      124 2024-05-04 10:34:00.000000 pywigxjpf-1.13.1/MANIFEST.in
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1917 2024-05-04 10:37:44.776609 pywigxjpf-1.13.1/PKG-INFO
+-rw-r--r--   0 htj       (1001) f2b      (30425)    10546 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/README
+drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-05-04 10:37:44.676607 pywigxjpf-1.13.1/cfg/
+-rw-r--r--   0 htj       (1001) f2b      (30425)     3939 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/cfg/wigxjpf_config.h
+drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-05-04 10:37:44.712608 pywigxjpf-1.13.1/example/
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1015 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/example/ccsimple.cc
+-rw-r--r--   0 htj       (1001) f2b      (30425)      202 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/example/ccsimple.good
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1417 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/example/cfail.c
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1328 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/example/cfail.expect
+-rw-r--r--   0 htj       (1001) f2b      (30425)      761 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/example/csimple.c
+-rw-r--r--   0 htj       (1001) f2b      (30425)      200 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/example/csimple.good
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1706 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/example/cthreadedsimple.c
+-rw-r--r--   0 htj       (1001) f2b      (30425)       50 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/example/cthreadedsimple.good
+-rw-r--r--   0 htj       (1001) f2b      (30425)      384 2024-05-04 10:34:00.000000 pywigxjpf-1.13.1/example/evaltable.huge.good
+-rw-r--r--   0 htj       (1001) f2b      (30425)      644 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/example/evaltable.large.good
+-rwxr-xr-x   0 htj       (1001) f2b      (30425)     4236 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/example/evaltable.sh
+-rw-r--r--   0 htj       (1001) f2b      (30425)    11835 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/example/evaltable.small.good
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1941 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/example/fsimple.f
+-rw-r--r--   0 htj       (1001) f2b      (30425)      227 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/example/fsimple.good
+-rw-r--r--   0 htj       (1001) f2b      (30425)     3364 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/example/py_numba.py
+-rw-r--r--   0 htj       (1001) f2b      (30425)     8320 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/example/pyfail.expect
+-rw-r--r--   0 htj       (1001) f2b      (30425)     3128 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/example/pyfail.py
+-rw-r--r--   0 htj       (1001) f2b      (30425)      340 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/example/pysimple.good
+-rwxr-xr-x   0 htj       (1001) f2b      (30425)     1936 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/example/pysimple.py
+-rw-r--r--   0 htj       (1001) f2b      (30425)     7768 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/example/wigxjpf.c
+drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-05-04 10:37:44.716608 pywigxjpf-1.13.1/inc/
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1755 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/inc/fpsimplexj.h
+-rw-r--r--   0 htj       (1001) f2b      (30425)     4080 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/inc/wigxjpf.h
+-rw-r--r--   0 htj       (1001) f2b      (30425)     2154 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/inc/wigxjpf_quadmath.h
+drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-05-04 10:37:44.724608 pywigxjpf-1.13.1/pywigxjpf/
+-rw-r--r--   0 htj       (1001) f2b      (30425)      381 2024-05-04 10:34:00.000000 pywigxjpf-1.13.1/pywigxjpf/__init__.py
+drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-05-04 10:37:44.732608 pywigxjpf-1.13.1/pywigxjpf/pregen/
+-rw-r--r--   0 htj       (1001) f2b      (30425)      168 2024-05-04 10:34:00.000000 pywigxjpf-1.13.1/pywigxjpf/pregen/wigxjpf_auto_config.h
+-rw-r--r--   0 htj       (1001) f2b      (30425)     3974 2024-05-04 10:34:00.000000 pywigxjpf-1.13.1/pywigxjpf/pywigxjpf.py
+-rw-r--r--   0 htj       (1001) f2b      (30425)     2379 2024-05-04 10:34:00.000000 pywigxjpf-1.13.1/pywigxjpf/pywigxjpf_ffi_builder.py
+drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-05-04 10:37:44.732608 pywigxjpf-1.13.1/pywigxjpf.egg-info/
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1917 2024-05-04 10:37:44.000000 pywigxjpf-1.13.1/pywigxjpf.egg-info/PKG-INFO
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1262 2024-05-04 10:37:44.000000 pywigxjpf-1.13.1/pywigxjpf.egg-info/SOURCES.txt
+-rw-r--r--   0 htj       (1001) f2b      (30425)        1 2024-05-04 10:37:44.000000 pywigxjpf-1.13.1/pywigxjpf.egg-info/dependency_links.txt
+-rw-r--r--   0 htj       (1001) f2b      (30425)       18 2024-05-04 10:37:44.000000 pywigxjpf-1.13.1/pywigxjpf.egg-info/requires.txt
+-rw-r--r--   0 htj       (1001) f2b      (30425)       24 2024-05-04 10:37:44.000000 pywigxjpf-1.13.1/pywigxjpf.egg-info/top_level.txt
+-rw-r--r--   0 htj       (1001) f2b      (30425)       38 2024-05-04 10:37:44.780609 pywigxjpf-1.13.1/setup.cfg
+-rw-r--r--   0 htj       (1001) f2b      (30425)     2516 2024-05-04 10:34:00.000000 pywigxjpf-1.13.1/setup.py
+drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-05-04 10:37:44.776609 pywigxjpf-1.13.1/src/
+-rw-r--r--   0 htj       (1001) f2b      (30425)     3871 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/src/c_wrap.c
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1037 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/src/c_wrap.h
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1586 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/src/c_wrap_float128.c
+-rw-r--r--   0 htj       (1001) f2b      (30425)    21866 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/src/calc.c
+-rw-r--r--   0 htj       (1001) f2b      (30425)     3483 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/src/calc.h
+-rw-r--r--   0 htj       (1001) f2b      (30425)     4430 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/src/calc_dbl.h
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1070 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/src/calc_float128.c
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1301 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/src/calc_minmax.h
+-rw-r--r--   0 htj       (1001) f2b      (30425)     2583 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/src/fortran_wrap.c
+-rw-r--r--   0 htj       (1001) f2b      (30425)     8335 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/src/fpsimple.c
+-rw-r--r--   0 htj       (1001) f2b      (30425)     7582 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/src/fpsimple_log.c
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1688 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/src/fpsimple_precalc.c
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1284 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/src/fwigxjpf.f
+-rw-r--r--   0 htj       (1001) f2b      (30425)    10366 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/src/multi_word_int.h
+-rw-r--r--   0 htj       (1001) f2b      (30425)     2039 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/src/multi_word_int_dbl.h
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1228 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/src/multi_word_int_float128.h
+-rw-r--r--   0 htj       (1001) f2b      (30425)     8051 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/src/prime_factor.c
+-rw-r--r--   0 htj       (1001) f2b      (30425)    15244 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/src/prime_factor.h
+-rw-r--r--   0 htj       (1001) f2b      (30425)     2368 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/src/test_cc_dbl.c
+-rw-r--r--   0 htj       (1001) f2b      (30425)     3393 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/src/trivial_zero.c
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1420 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/src/wigxjpf_error.c
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1970 2024-05-04 10:33:59.000000 pywigxjpf-1.13.1/src/wigxjpf_error.h
```

### Comparing `pywigxjpf-1.13/CHANGELOG` & `pywigxjpf-1.13.1/CHANGELOG`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/COPYING` & `pywigxjpf-1.13.1/COPYING`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/COPYING.LESSER` & `pywigxjpf-1.13.1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/PKG-INFO` & `pywigxjpf-1.13.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywigxjpf
-Version: 1.13
+Version: 1.13.1
 Summary: Wigner Symbols
 Home-page: http://fy.chalmers.se/subatom/wigxjpf
 Author: C. Forssen and H. T. Johansson
 License: GPLv3
 Description: 
         WIGXJPF evaluates Wigner 3j, 6j and 9j symbols
         accurately using prime factorisation and multi-word integer arithmetic.
```

### Comparing `pywigxjpf-1.13/README` & `pywigxjpf-1.13.1/README`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/cfg/wigxjpf_config.h` & `pywigxjpf-1.13.1/cfg/wigxjpf_config.h`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/example/ccsimple.cc` & `pywigxjpf-1.13.1/example/ccsimple.cc`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/example/cfail.c` & `pywigxjpf-1.13.1/example/cfail.c`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/example/cfail.expect` & `pywigxjpf-1.13.1/example/cfail.expect`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/example/csimple.c` & `pywigxjpf-1.13.1/example/csimple.c`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/example/cthreadedsimple.c` & `pywigxjpf-1.13.1/example/cthreadedsimple.c`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/example/evaltable.large.good` & `pywigxjpf-1.13.1/example/evaltable.large.good`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/example/evaltable.sh` & `pywigxjpf-1.13.1/example/evaltable.sh`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/example/evaltable.small.good` & `pywigxjpf-1.13.1/example/evaltable.small.good`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/example/fsimple.f` & `pywigxjpf-1.13.1/example/fsimple.f`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/example/py_numba.py` & `pywigxjpf-1.13.1/example/py_numba.py`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/example/pyfail.expect` & `pywigxjpf-1.13.1/example/pyfail.expect`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/example/pyfail.py` & `pywigxjpf-1.13.1/example/pyfail.py`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/example/pysimple.py` & `pywigxjpf-1.13.1/example/pysimple.py`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/example/wigxjpf.c` & `pywigxjpf-1.13.1/example/wigxjpf.c`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/inc/fpsimplexj.h` & `pywigxjpf-1.13.1/inc/fpsimplexj.h`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/inc/wigxjpf.h` & `pywigxjpf-1.13.1/inc/wigxjpf.h`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/inc/wigxjpf_quadmath.h` & `pywigxjpf-1.13.1/inc/wigxjpf_quadmath.h`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/pywigxjpf/pywigxjpf.py` & `pywigxjpf-1.13.1/pywigxjpf/pywigxjpf.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     (9)  wig6jj_array([jj1,jj2,jj3,
                        jj4,jj5,jj6])
     (10) wig9jj_array([jj1,jj2,jj3,
                        jj4,jj5,jj6,
                        jj7,jj8,jj9])
 """
 
-__version__ = '1.13'
+__version__ = '1.13.1  '
 __author__ = 'C. Forssen and H.T. Johansson'
 __all__ = ['pywigxjpf']
 
 import numpy as np
 
 try:
     from pywigxjpf_ffi import ffi, lib
```

### Comparing `pywigxjpf-1.13/pywigxjpf/pywigxjpf_ffi_builder.py` & `pywigxjpf-1.13.1/pywigxjpf/pywigxjpf_ffi_builder.py`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/pywigxjpf.egg-info/PKG-INFO` & `pywigxjpf-1.13.1/pywigxjpf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywigxjpf
-Version: 1.13
+Version: 1.13.1
 Summary: Wigner Symbols
 Home-page: http://fy.chalmers.se/subatom/wigxjpf
 Author: C. Forssen and H. T. Johansson
 License: GPLv3
 Description: 
         WIGXJPF evaluates Wigner 3j, 6j and 9j symbols
         accurately using prime factorisation and multi-word integer arithmetic.
```

### Comparing `pywigxjpf-1.13/pywigxjpf.egg-info/SOURCES.txt` & `pywigxjpf-1.13.1/pywigxjpf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/setup.py` & `pywigxjpf-1.13.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
           '!                                            !\n'
           '##############################################\n\n'
           'For details, see '
           'https://github.com/pypa/setuptools/issues/391#issuecomment-202919511'
           '\n\n')
 
 setup(name='pywigxjpf',
-      version='1.13',
+      version='1.13.1  ',
       description='Wigner Symbols',
       long_description="""
 WIGXJPF evaluates Wigner 3j, 6j and 9j symbols
 accurately using prime factorisation and multi-word integer arithmetic.
 
 Known issue
 -----------
```

### Comparing `pywigxjpf-1.13/src/c_wrap.c` & `pywigxjpf-1.13.1/src/c_wrap.c`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/src/c_wrap.h` & `pywigxjpf-1.13.1/src/c_wrap.h`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/src/c_wrap_float128.c` & `pywigxjpf-1.13.1/src/c_wrap_float128.c`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/src/calc.c` & `pywigxjpf-1.13.1/src/calc.c`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/src/calc.h` & `pywigxjpf-1.13.1/src/calc.h`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/src/calc_dbl.h` & `pywigxjpf-1.13.1/src/calc_dbl.h`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/src/calc_float128.c` & `pywigxjpf-1.13.1/src/calc_float128.c`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/src/calc_minmax.h` & `pywigxjpf-1.13.1/src/calc_minmax.h`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/src/fortran_wrap.c` & `pywigxjpf-1.13.1/src/fortran_wrap.c`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/src/fpsimple.c` & `pywigxjpf-1.13.1/src/fpsimple.c`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/src/fpsimple_log.c` & `pywigxjpf-1.13.1/src/fpsimple_log.c`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/src/fpsimple_precalc.c` & `pywigxjpf-1.13.1/src/fpsimple_precalc.c`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/src/fwigxjpf.f` & `pywigxjpf-1.13.1/src/fwigxjpf.f`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/src/multi_word_int.h` & `pywigxjpf-1.13.1/src/multi_word_int.h`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/src/multi_word_int_dbl.h` & `pywigxjpf-1.13.1/src/multi_word_int_dbl.h`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/src/multi_word_int_float128.h` & `pywigxjpf-1.13.1/src/multi_word_int_float128.h`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/src/prime_factor.c` & `pywigxjpf-1.13.1/src/prime_factor.c`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/src/prime_factor.h` & `pywigxjpf-1.13.1/src/prime_factor.h`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/src/test_cc_dbl.c` & `pywigxjpf-1.13.1/src/test_cc_dbl.c`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 __thread int global = 0;
 #endif
 #if defined(TEST_TRAIL_ARRAY_EMPTY) || \
   defined(TEST_TRAIL_ARRAY_ZERO) || \
   defined(TEST_TRAIL_ARRAY_ONE)
 struct trail_struct
 {
+  int a;
 # if TEST_TRAIL_ARRAY_EMPTY
   int trail[];
 # endif
 # if TEST_TRAIL_ARRAY_ZERO
   int trail[0];
 # endif
 # if TEST_TRAIL_ARRAY_ONE
```

### Comparing `pywigxjpf-1.13/src/trivial_zero.c` & `pywigxjpf-1.13.1/src/trivial_zero.c`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/src/wigxjpf_error.c` & `pywigxjpf-1.13.1/src/wigxjpf_error.c`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.13/src/wigxjpf_error.h` & `pywigxjpf-1.13.1/src/wigxjpf_error.h`

 * *Files identical despite different names*

