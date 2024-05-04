# Comparing `tmp/pywigxjpf-1.12.tar.gz` & `tmp/pywigxjpf-1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywigxjpf-1.12.tar", last modified: Sat Feb 17 13:32:45 2024, max compression
+gzip compressed data, was "pywigxjpf-1.13.tar", last modified: Sat May  4 10:18:04 2024, max compression
```

## Comparing `pywigxjpf-1.12.tar` & `pywigxjpf-1.13.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-02-17 13:32:45.076954 pywigxjpf-1.12/
--rw-r--r--   0 htj       (1001) f2b      (30425)     1902 2024-02-17 13:32:08.000000 pywigxjpf-1.12/CHANGELOG
--rw-r--r--   0 htj       (1001) f2b      (30425)    35147 2024-02-17 13:32:08.000000 pywigxjpf-1.12/COPYING
--rw-r--r--   0 htj       (1001) f2b      (30425)     7651 2024-02-17 13:32:08.000000 pywigxjpf-1.12/COPYING.LESSER
--rw-r--r--   0 htj       (1001) f2b      (30425)      124 2024-02-17 13:32:08.000000 pywigxjpf-1.12/MANIFEST.in
--rw-r--r--   0 htj       (1001) f2b      (30425)     1915 2024-02-17 13:32:45.072954 pywigxjpf-1.12/PKG-INFO
--rw-r--r--   0 htj       (1001) f2b      (30425)    10546 2024-02-17 13:32:08.000000 pywigxjpf-1.12/README
-drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-02-17 13:32:44.972952 pywigxjpf-1.12/cfg/
--rw-r--r--   0 htj       (1001) f2b      (30425)     3362 2024-02-17 13:32:08.000000 pywigxjpf-1.12/cfg/wigxjpf_config.h
-drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-02-17 13:32:45.008953 pywigxjpf-1.12/example/
--rw-r--r--   0 htj       (1001) f2b      (30425)     1015 2024-02-17 13:32:08.000000 pywigxjpf-1.12/example/ccsimple.cc
--rw-r--r--   0 htj       (1001) f2b      (30425)      202 2024-02-17 13:32:08.000000 pywigxjpf-1.12/example/ccsimple.good
--rw-r--r--   0 htj       (1001) f2b      (30425)     1417 2024-02-17 13:32:08.000000 pywigxjpf-1.12/example/cfail.c
--rw-r--r--   0 htj       (1001) f2b      (30425)     1328 2024-02-17 13:32:08.000000 pywigxjpf-1.12/example/cfail.expect
--rw-r--r--   0 htj       (1001) f2b      (30425)      761 2024-02-17 13:32:08.000000 pywigxjpf-1.12/example/csimple.c
--rw-r--r--   0 htj       (1001) f2b      (30425)      200 2024-02-17 13:32:08.000000 pywigxjpf-1.12/example/csimple.good
--rw-r--r--   0 htj       (1001) f2b      (30425)     1706 2024-02-17 13:32:08.000000 pywigxjpf-1.12/example/cthreadedsimple.c
--rw-r--r--   0 htj       (1001) f2b      (30425)       50 2024-02-17 13:32:08.000000 pywigxjpf-1.12/example/cthreadedsimple.good
--rw-r--r--   0 htj       (1001) f2b      (30425)      384 2024-02-17 13:32:08.000000 pywigxjpf-1.12/example/evaltable.huge.good
--rw-r--r--   0 htj       (1001) f2b      (30425)      644 2024-02-17 13:32:08.000000 pywigxjpf-1.12/example/evaltable.large.good
--rwxr-xr-x   0 htj       (1001) f2b      (30425)     4236 2024-02-17 13:32:08.000000 pywigxjpf-1.12/example/evaltable.sh
--rw-r--r--   0 htj       (1001) f2b      (30425)    11835 2024-02-17 13:32:08.000000 pywigxjpf-1.12/example/evaltable.small.good
--rw-r--r--   0 htj       (1001) f2b      (30425)     1941 2024-02-17 13:32:08.000000 pywigxjpf-1.12/example/fsimple.f
--rw-r--r--   0 htj       (1001) f2b      (30425)      227 2024-02-17 13:32:08.000000 pywigxjpf-1.12/example/fsimple.good
--rw-r--r--   0 htj       (1001) f2b      (30425)     3364 2024-02-17 13:32:08.000000 pywigxjpf-1.12/example/py_numba.py
--rw-r--r--   0 htj       (1001) f2b      (30425)     8320 2024-02-17 13:32:08.000000 pywigxjpf-1.12/example/pyfail.expect
--rw-r--r--   0 htj       (1001) f2b      (30425)     3128 2024-02-17 13:32:08.000000 pywigxjpf-1.12/example/pyfail.py
--rw-r--r--   0 htj       (1001) f2b      (30425)      340 2024-02-17 13:32:08.000000 pywigxjpf-1.12/example/pysimple.good
--rwxr-xr-x   0 htj       (1001) f2b      (30425)     1936 2024-02-17 13:32:08.000000 pywigxjpf-1.12/example/pysimple.py
--rw-r--r--   0 htj       (1001) f2b      (30425)     7768 2024-02-17 13:32:08.000000 pywigxjpf-1.12/example/wigxjpf.c
-drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-02-17 13:32:45.016953 pywigxjpf-1.12/inc/
--rw-r--r--   0 htj       (1001) f2b      (30425)     1755 2024-02-17 13:32:08.000000 pywigxjpf-1.12/inc/fpsimplexj.h
--rw-r--r--   0 htj       (1001) f2b      (30425)     4080 2024-02-17 13:32:08.000000 pywigxjpf-1.12/inc/wigxjpf.h
--rw-r--r--   0 htj       (1001) f2b      (30425)     2154 2024-02-17 13:32:08.000000 pywigxjpf-1.12/inc/wigxjpf_quadmath.h
-drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-02-17 13:32:45.020953 pywigxjpf-1.12/pywigxjpf/
--rw-r--r--   0 htj       (1001) f2b      (30425)      381 2024-02-17 13:32:08.000000 pywigxjpf-1.12/pywigxjpf/__init__.py
-drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-02-17 13:32:45.032953 pywigxjpf-1.12/pywigxjpf/pregen/
--rw-r--r--   0 htj       (1001) f2b      (30425)      168 2024-02-17 13:32:08.000000 pywigxjpf-1.12/pywigxjpf/pregen/wigxjpf_auto_config.h
--rw-r--r--   0 htj       (1001) f2b      (30425)     3970 2024-02-17 13:32:08.000000 pywigxjpf-1.12/pywigxjpf/pywigxjpf.py
--rw-r--r--   0 htj       (1001) f2b      (30425)     2379 2024-02-17 13:32:08.000000 pywigxjpf-1.12/pywigxjpf/pywigxjpf_ffi_builder.py
-drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-02-17 13:32:45.028953 pywigxjpf-1.12/pywigxjpf.egg-info/
--rw-r--r--   0 htj       (1001) f2b      (30425)     1915 2024-02-17 13:32:44.000000 pywigxjpf-1.12/pywigxjpf.egg-info/PKG-INFO
--rw-r--r--   0 htj       (1001) f2b      (30425)     1262 2024-02-17 13:32:44.000000 pywigxjpf-1.12/pywigxjpf.egg-info/SOURCES.txt
--rw-r--r--   0 htj       (1001) f2b      (30425)        1 2024-02-17 13:32:44.000000 pywigxjpf-1.12/pywigxjpf.egg-info/dependency_links.txt
--rw-r--r--   0 htj       (1001) f2b      (30425)       18 2024-02-17 13:32:44.000000 pywigxjpf-1.12/pywigxjpf.egg-info/requires.txt
--rw-r--r--   0 htj       (1001) f2b      (30425)       24 2024-02-17 13:32:44.000000 pywigxjpf-1.12/pywigxjpf.egg-info/top_level.txt
--rw-r--r--   0 htj       (1001) f2b      (30425)       38 2024-02-17 13:32:45.076954 pywigxjpf-1.12/setup.cfg
--rw-r--r--   0 htj       (1001) f2b      (30425)     2512 2024-02-17 13:32:08.000000 pywigxjpf-1.12/setup.py
-drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-02-17 13:32:45.072954 pywigxjpf-1.12/src/
--rw-r--r--   0 htj       (1001) f2b      (30425)     3871 2024-02-17 13:32:08.000000 pywigxjpf-1.12/src/c_wrap.c
--rw-r--r--   0 htj       (1001) f2b      (30425)     1037 2024-02-17 13:32:08.000000 pywigxjpf-1.12/src/c_wrap.h
--rw-r--r--   0 htj       (1001) f2b      (30425)     1586 2024-02-17 13:32:08.000000 pywigxjpf-1.12/src/c_wrap_float128.c
--rw-r--r--   0 htj       (1001) f2b      (30425)    21866 2024-02-17 13:32:08.000000 pywigxjpf-1.12/src/calc.c
--rw-r--r--   0 htj       (1001) f2b      (30425)     3483 2024-02-17 13:32:08.000000 pywigxjpf-1.12/src/calc.h
--rw-r--r--   0 htj       (1001) f2b      (30425)     4430 2024-02-17 13:32:08.000000 pywigxjpf-1.12/src/calc_dbl.h
--rw-r--r--   0 htj       (1001) f2b      (30425)     1070 2024-02-17 13:32:08.000000 pywigxjpf-1.12/src/calc_float128.c
--rw-r--r--   0 htj       (1001) f2b      (30425)     1301 2024-02-17 13:32:08.000000 pywigxjpf-1.12/src/calc_minmax.h
--rw-r--r--   0 htj       (1001) f2b      (30425)     2583 2024-02-17 13:32:08.000000 pywigxjpf-1.12/src/fortran_wrap.c
--rw-r--r--   0 htj       (1001) f2b      (30425)     8335 2024-02-17 13:32:08.000000 pywigxjpf-1.12/src/fpsimple.c
--rw-r--r--   0 htj       (1001) f2b      (30425)     7582 2024-02-17 13:32:08.000000 pywigxjpf-1.12/src/fpsimple_log.c
--rw-r--r--   0 htj       (1001) f2b      (30425)     1688 2024-02-17 13:32:08.000000 pywigxjpf-1.12/src/fpsimple_precalc.c
--rw-r--r--   0 htj       (1001) f2b      (30425)     1284 2024-02-17 13:32:08.000000 pywigxjpf-1.12/src/fwigxjpf.f
--rw-r--r--   0 htj       (1001) f2b      (30425)    10366 2024-02-17 13:32:08.000000 pywigxjpf-1.12/src/multi_word_int.h
--rw-r--r--   0 htj       (1001) f2b      (30425)     2039 2024-02-17 13:32:08.000000 pywigxjpf-1.12/src/multi_word_int_dbl.h
--rw-r--r--   0 htj       (1001) f2b      (30425)     1228 2024-02-17 13:32:08.000000 pywigxjpf-1.12/src/multi_word_int_float128.h
--rw-r--r--   0 htj       (1001) f2b      (30425)     8051 2024-02-17 13:32:08.000000 pywigxjpf-1.12/src/prime_factor.c
--rw-r--r--   0 htj       (1001) f2b      (30425)    17216 2024-02-17 13:32:08.000000 pywigxjpf-1.12/src/prime_factor.h
--rw-r--r--   0 htj       (1001) f2b      (30425)     1687 2024-02-17 13:32:08.000000 pywigxjpf-1.12/src/test_cc_dbl.c
--rw-r--r--   0 htj       (1001) f2b      (30425)     3393 2024-02-17 13:32:08.000000 pywigxjpf-1.12/src/trivial_zero.c
--rw-r--r--   0 htj       (1001) f2b      (30425)     1420 2024-02-17 13:32:08.000000 pywigxjpf-1.12/src/wigxjpf_error.c
--rw-r--r--   0 htj       (1001) f2b      (30425)     1970 2024-02-17 13:32:08.000000 pywigxjpf-1.12/src/wigxjpf_error.h
+drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-05-04 10:18:04.742176 pywigxjpf-1.13/
+-rw-r--r--   0 htj       (1001) f2b      (30425)     2017 2024-05-04 10:17:31.000000 pywigxjpf-1.13/CHANGELOG
+-rw-r--r--   0 htj       (1001) f2b      (30425)    35147 2024-05-04 10:17:31.000000 pywigxjpf-1.13/COPYING
+-rw-r--r--   0 htj       (1001) f2b      (30425)     7651 2024-05-04 10:17:31.000000 pywigxjpf-1.13/COPYING.LESSER
+-rw-r--r--   0 htj       (1001) f2b      (30425)      124 2024-05-04 10:17:32.000000 pywigxjpf-1.13/MANIFEST.in
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1915 2024-05-04 10:18:04.742176 pywigxjpf-1.13/PKG-INFO
+-rw-r--r--   0 htj       (1001) f2b      (30425)    10546 2024-05-04 10:17:31.000000 pywigxjpf-1.13/README
+drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-05-04 10:18:04.642174 pywigxjpf-1.13/cfg/
+-rw-r--r--   0 htj       (1001) f2b      (30425)     3939 2024-05-04 10:17:32.000000 pywigxjpf-1.13/cfg/wigxjpf_config.h
+drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-05-04 10:18:04.678175 pywigxjpf-1.13/example/
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1015 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/ccsimple.cc
+-rw-r--r--   0 htj       (1001) f2b      (30425)      202 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/ccsimple.good
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1417 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/cfail.c
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1328 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/cfail.expect
+-rw-r--r--   0 htj       (1001) f2b      (30425)      761 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/csimple.c
+-rw-r--r--   0 htj       (1001) f2b      (30425)      200 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/csimple.good
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1706 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/cthreadedsimple.c
+-rw-r--r--   0 htj       (1001) f2b      (30425)       50 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/cthreadedsimple.good
+-rw-r--r--   0 htj       (1001) f2b      (30425)      384 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/evaltable.huge.good
+-rw-r--r--   0 htj       (1001) f2b      (30425)      644 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/evaltable.large.good
+-rwxr-xr-x   0 htj       (1001) f2b      (30425)     4236 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/evaltable.sh
+-rw-r--r--   0 htj       (1001) f2b      (30425)    11835 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/evaltable.small.good
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1941 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/fsimple.f
+-rw-r--r--   0 htj       (1001) f2b      (30425)      227 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/fsimple.good
+-rw-r--r--   0 htj       (1001) f2b      (30425)     3364 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/py_numba.py
+-rw-r--r--   0 htj       (1001) f2b      (30425)     8320 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/pyfail.expect
+-rw-r--r--   0 htj       (1001) f2b      (30425)     3128 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/pyfail.py
+-rw-r--r--   0 htj       (1001) f2b      (30425)      340 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/pysimple.good
+-rwxr-xr-x   0 htj       (1001) f2b      (30425)     1936 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/pysimple.py
+-rw-r--r--   0 htj       (1001) f2b      (30425)     7768 2024-05-04 10:17:32.000000 pywigxjpf-1.13/example/wigxjpf.c
+drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-05-04 10:18:04.686175 pywigxjpf-1.13/inc/
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1755 2024-05-04 10:17:32.000000 pywigxjpf-1.13/inc/fpsimplexj.h
+-rw-r--r--   0 htj       (1001) f2b      (30425)     4080 2024-05-04 10:17:32.000000 pywigxjpf-1.13/inc/wigxjpf.h
+-rw-r--r--   0 htj       (1001) f2b      (30425)     2154 2024-05-04 10:17:32.000000 pywigxjpf-1.13/inc/wigxjpf_quadmath.h
+drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-05-04 10:18:04.690175 pywigxjpf-1.13/pywigxjpf/
+-rw-r--r--   0 htj       (1001) f2b      (30425)      381 2024-05-04 10:17:32.000000 pywigxjpf-1.13/pywigxjpf/__init__.py
+drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-05-04 10:18:04.702175 pywigxjpf-1.13/pywigxjpf/pregen/
+-rw-r--r--   0 htj       (1001) f2b      (30425)      168 2024-05-04 10:17:32.000000 pywigxjpf-1.13/pywigxjpf/pregen/wigxjpf_auto_config.h
+-rw-r--r--   0 htj       (1001) f2b      (30425)     3970 2024-05-04 10:17:32.000000 pywigxjpf-1.13/pywigxjpf/pywigxjpf.py
+-rw-r--r--   0 htj       (1001) f2b      (30425)     2379 2024-05-04 10:17:32.000000 pywigxjpf-1.13/pywigxjpf/pywigxjpf_ffi_builder.py
+drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-05-04 10:18:04.698175 pywigxjpf-1.13/pywigxjpf.egg-info/
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1915 2024-05-04 10:18:04.000000 pywigxjpf-1.13/pywigxjpf.egg-info/PKG-INFO
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1262 2024-05-04 10:18:04.000000 pywigxjpf-1.13/pywigxjpf.egg-info/SOURCES.txt
+-rw-r--r--   0 htj       (1001) f2b      (30425)        1 2024-05-04 10:18:04.000000 pywigxjpf-1.13/pywigxjpf.egg-info/dependency_links.txt
+-rw-r--r--   0 htj       (1001) f2b      (30425)       18 2024-05-04 10:18:04.000000 pywigxjpf-1.13/pywigxjpf.egg-info/requires.txt
+-rw-r--r--   0 htj       (1001) f2b      (30425)       24 2024-05-04 10:18:04.000000 pywigxjpf-1.13/pywigxjpf.egg-info/top_level.txt
+-rw-r--r--   0 htj       (1001) f2b      (30425)       38 2024-05-04 10:18:04.746176 pywigxjpf-1.13/setup.cfg
+-rw-r--r--   0 htj       (1001) f2b      (30425)     2512 2024-05-04 10:17:32.000000 pywigxjpf-1.13/setup.py
+drwxr-xr-x   0 htj       (1001) f2b      (30425)        0 2024-05-04 10:18:04.742176 pywigxjpf-1.13/src/
+-rw-r--r--   0 htj       (1001) f2b      (30425)     3871 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/c_wrap.c
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1037 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/c_wrap.h
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1586 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/c_wrap_float128.c
+-rw-r--r--   0 htj       (1001) f2b      (30425)    21866 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/calc.c
+-rw-r--r--   0 htj       (1001) f2b      (30425)     3483 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/calc.h
+-rw-r--r--   0 htj       (1001) f2b      (30425)     4430 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/calc_dbl.h
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1070 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/calc_float128.c
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1301 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/calc_minmax.h
+-rw-r--r--   0 htj       (1001) f2b      (30425)     2583 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/fortran_wrap.c
+-rw-r--r--   0 htj       (1001) f2b      (30425)     8335 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/fpsimple.c
+-rw-r--r--   0 htj       (1001) f2b      (30425)     7582 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/fpsimple_log.c
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1688 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/fpsimple_precalc.c
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1284 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/fwigxjpf.f
+-rw-r--r--   0 htj       (1001) f2b      (30425)    10366 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/multi_word_int.h
+-rw-r--r--   0 htj       (1001) f2b      (30425)     2039 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/multi_word_int_dbl.h
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1228 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/multi_word_int_float128.h
+-rw-r--r--   0 htj       (1001) f2b      (30425)     8051 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/prime_factor.c
+-rw-r--r--   0 htj       (1001) f2b      (30425)    15244 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/prime_factor.h
+-rw-r--r--   0 htj       (1001) f2b      (30425)     2359 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/test_cc_dbl.c
+-rw-r--r--   0 htj       (1001) f2b      (30425)     3393 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/trivial_zero.c
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1420 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/wigxjpf_error.c
+-rw-r--r--   0 htj       (1001) f2b      (30425)     1970 2024-05-04 10:17:32.000000 pywigxjpf-1.13/src/wigxjpf_error.h
```

### Comparing `pywigxjpf-1.12/CHANGELOG` & `pywigxjpf-1.13/CHANGELOG`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+1.13  2024-05-04
+
+	Bugfix for gcc 14:  (T. Djärv).
+	  Variable sized array at end of struct with [], [0] or [1].
+
 1.12  2024-02-17
 
 	Allow x for last m when calculating 3j from command line.
 	Handle compilation in other directory (VPATH).
 	Callback: wigxjpf_error_handler().  Use in python interface.
 	CMakeLists.txt file.  (Plain Makefile is and will remain standard.)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pywigxjpf-1.12/COPYING` & `pywigxjpf-1.13/COPYING`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/COPYING.LESSER` & `pywigxjpf-1.13/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/PKG-INFO` & `pywigxjpf-1.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywigxjpf
-Version: 1.12
+Version: 1.13
 Summary: Wigner Symbols
 Home-page: http://fy.chalmers.se/subatom/wigxjpf
 Author: C. Forssen and H. T. Johansson
 License: GPLv3
 Description: 
         WIGXJPF evaluates Wigner 3j, 6j and 9j symbols
         accurately using prime factorisation and multi-word integer arithmetic.
```

### Comparing `pywigxjpf-1.12/README` & `pywigxjpf-1.13/README`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 ====================================
 
 To compile from another directory (to not change in files in the
 source directory), VPATH can be used:
 
 mkdir wigxjpf-build
 cd wigxjpf-build
-make -f ../wigxjpf-1.12/Makefile VPATH=../wigxjpf-VERSION/ test
+make -f ../wigxjpf-1.13/Makefile VPATH=../wigxjpf-VERSION/ test
 
 Notes:
 
 It does not work if the code was already compiled in the source
 directory (use 'make clean').
 
 It does currently not work to compile the python interface with VPATH.
```

### Comparing `pywigxjpf-1.12/cfg/wigxjpf_config.h` & `pywigxjpf-1.13/cfg/wigxjpf_config.h`

 * *Files 14% similar despite different names*

```diff
@@ -37,25 +37,42 @@
 
 /* Generate code to include semi-factorials. */
 
 #ifndef WIGXJPF_IMPL_DOUBLE_FACTORIAL
 #define WIGXJPF_IMPL_DOUBLE_FACTORIAL  0
 #endif
 
+/* How to declare a variable sized array at end of structure. */
+
+#if   defined(TRAIL_ARRAY_EMPTY)
+#define WIGXJPF_STR_VAR_LEN_ARRAY_SIZE     /* Empty: []
+					      Since C11. */
+#elif defined(TRAIL_ARRAY_ZERO)
+#define WIGXJPF_STR_VAR_LEN_ARRAY_SIZE  0  /* Empty: [0]
+					      This is a compiler extension. */
+#elif defined(TRAIL_ARRAY_ONE)
+#define WIGXJPF_STR_VAR_LEN_ARRAY_SIZE  1  /* Empty: [1]
+					      This uses undefined behaviour. */
+#else
+#error No TRAIL_ARRAY_xxx -> no WIGXJPF_STR_VAR_LEN_ARRAY_SIZE implementation.
+#endif
+
 /* Size in bytes of each prime exponent.  2 or 4. */
 
 #define PRIME_LIST_SIZEOF_ITEM      4
 
 /* Use vector types / instructions, e.g. SSE / AVX, for the exponents. */
 
 /* Using vector instructions give ~0 (or at most single-digit %)
  * improvements for large symbols, and some 20 % for small symbols.
  */
 
-#define PRIME_LIST_USE_VECTOR       0
+/* Note: removed from code. */
+
+/* #define PRIME_LIST_USE_VECTOR       0 */
 
 /* Size in bytes of the vector instances.  SSE: 16, AVX:32 */
 
 /* Using vector_size(32), i.e. AVX instructions on x86-64 has been
  * tested, and gives ~0 difference.  We are memory/cache bandwidth
  * limited.
  */
```

### Comparing `pywigxjpf-1.12/example/ccsimple.cc` & `pywigxjpf-1.13/example/ccsimple.cc`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/example/cfail.c` & `pywigxjpf-1.13/example/cfail.c`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/example/cfail.expect` & `pywigxjpf-1.13/example/cfail.expect`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/example/csimple.c` & `pywigxjpf-1.13/example/csimple.c`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/example/cthreadedsimple.c` & `pywigxjpf-1.13/example/cthreadedsimple.c`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/example/evaltable.large.good` & `pywigxjpf-1.13/example/evaltable.large.good`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/example/evaltable.sh` & `pywigxjpf-1.13/example/evaltable.sh`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/example/evaltable.small.good` & `pywigxjpf-1.13/example/evaltable.small.good`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/example/fsimple.f` & `pywigxjpf-1.13/example/fsimple.f`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/example/py_numba.py` & `pywigxjpf-1.13/example/py_numba.py`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/example/pyfail.expect` & `pywigxjpf-1.13/example/pyfail.expect`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/example/pyfail.py` & `pywigxjpf-1.13/example/pyfail.py`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/example/pysimple.py` & `pywigxjpf-1.13/example/pysimple.py`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/example/wigxjpf.c` & `pywigxjpf-1.13/example/wigxjpf.c`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/inc/fpsimplexj.h` & `pywigxjpf-1.13/inc/fpsimplexj.h`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/inc/wigxjpf.h` & `pywigxjpf-1.13/inc/wigxjpf.h`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/inc/wigxjpf_quadmath.h` & `pywigxjpf-1.13/inc/wigxjpf_quadmath.h`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/pywigxjpf/pywigxjpf.py` & `pywigxjpf-1.13/pywigxjpf/pywigxjpf.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     (9)  wig6jj_array([jj1,jj2,jj3,
                        jj4,jj5,jj6])
     (10) wig9jj_array([jj1,jj2,jj3,
                        jj4,jj5,jj6,
                        jj7,jj8,jj9])
 """
 
-__version__ = '1.12'
+__version__ = '1.13'
 __author__ = 'C. Forssen and H.T. Johansson'
 __all__ = ['pywigxjpf']
 
 import numpy as np
 
 try:
     from pywigxjpf_ffi import ffi, lib
```

### Comparing `pywigxjpf-1.12/pywigxjpf/pywigxjpf_ffi_builder.py` & `pywigxjpf-1.13/pywigxjpf/pywigxjpf_ffi_builder.py`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/pywigxjpf.egg-info/PKG-INFO` & `pywigxjpf-1.13/pywigxjpf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywigxjpf
-Version: 1.12
+Version: 1.13
 Summary: Wigner Symbols
 Home-page: http://fy.chalmers.se/subatom/wigxjpf
 Author: C. Forssen and H. T. Johansson
 License: GPLv3
 Description: 
         WIGXJPF evaluates Wigner 3j, 6j and 9j symbols
         accurately using prime factorisation and multi-word integer arithmetic.
```

### Comparing `pywigxjpf-1.12/pywigxjpf.egg-info/SOURCES.txt` & `pywigxjpf-1.13/pywigxjpf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/setup.py` & `pywigxjpf-1.13/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
           '!                                            !\n'
           '##############################################\n\n'
           'For details, see '
           'https://github.com/pypa/setuptools/issues/391#issuecomment-202919511'
           '\n\n')
 
 setup(name='pywigxjpf',
-      version='1.12',
+      version='1.13',
       description='Wigner Symbols',
       long_description="""
 WIGXJPF evaluates Wigner 3j, 6j and 9j symbols
 accurately using prime factorisation and multi-word integer arithmetic.
 
 Known issue
 -----------
```

### Comparing `pywigxjpf-1.12/src/c_wrap.c` & `pywigxjpf-1.13/src/c_wrap.c`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/src/c_wrap.h` & `pywigxjpf-1.13/src/c_wrap.h`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/src/c_wrap_float128.c` & `pywigxjpf-1.13/src/c_wrap_float128.c`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/src/calc.c` & `pywigxjpf-1.13/src/calc.c`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/src/calc.h` & `pywigxjpf-1.13/src/calc.h`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/src/calc_dbl.h` & `pywigxjpf-1.13/src/calc_dbl.h`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/src/calc_float128.c` & `pywigxjpf-1.13/src/calc_float128.c`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/src/calc_minmax.h` & `pywigxjpf-1.13/src/calc_minmax.h`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/src/fortran_wrap.c` & `pywigxjpf-1.13/src/fortran_wrap.c`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/src/fpsimple.c` & `pywigxjpf-1.13/src/fpsimple.c`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/src/fpsimple_log.c` & `pywigxjpf-1.13/src/fpsimple_log.c`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/src/fpsimple_precalc.c` & `pywigxjpf-1.13/src/fpsimple_precalc.c`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/src/fwigxjpf.f` & `pywigxjpf-1.13/src/fwigxjpf.f`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/src/multi_word_int.h` & `pywigxjpf-1.13/src/multi_word_int.h`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/src/multi_word_int_dbl.h` & `pywigxjpf-1.13/src/multi_word_int_dbl.h`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/src/multi_word_int_float128.h` & `pywigxjpf-1.13/src/multi_word_int_float128.h`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/src/prime_factor.c` & `pywigxjpf-1.13/src/prime_factor.c`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 	continue;
 
       for (mark = p*p; mark <= max_factorial; mark += p)
 	isprime[mark] = 0;
     }
 
   /* We can now count the number of prime numbers, i.e. the size of
-   * out basis.
+   * our basis.
    */
 
   int num_primes = 0;
 
   for (i = 2; i <= max_factorial; i++)
     num_primes += isprime[i];
```

### Comparing `pywigxjpf-1.12/src/prime_factor.h` & `pywigxjpf-1.13/src/prime_factor.h`

 * *Files 4% similar despite different names*

```diff
@@ -33,51 +33,27 @@
 #elif PRIME_LIST_SIZEOF_ITEM == 4
 typedef int32_t       prime_exp_t;
 typedef uint32_t    u_prime_exp_t;
 #else
 # error PRIME_LIST_SIZEOF_ITEM must be 2 or 4.
 #endif
 
-#if PRIME_LIST_USE_VECTOR
-typedef prime_exp_t v_prime_exp_t
-__attribute__ ((vector_size (PRIME_LIST_VECT_SIZE)));
-# define V_PRIME_EXP_T  v_prime_exp_t
-# define V_EXPO         v_expo
-# define PRIME_LIST_VECT_BLOCK_ITEMS \
-  (PRIME_LIST_VECT_SIZE / PRIME_LIST_SIZEOF_ITEM)
-# if PRIME_LIST_VECT_BLOCK_ITEMS == 2
-#  define V_ITEM_INIT(x)   { x, x }
-# elif PRIME_LIST_VECT_BLOCK_ITEMS == 4
-#  define V_ITEM_INIT(x)   { x, x, x, x }
-# elif PRIME_LIST_VECT_BLOCK_ITEMS == 8
-#  define V_ITEM_INIT(x)   { x, x, x, x, x, x, x, x }
-# elif PRIME_LIST_VECT_BLOCK_ITEMS == 16
-#  define V_ITEM_INIT(x)   { x, x, x, x, x, x, x, x, x, x, x, x, x, x, x, x }
-# endif
-#else
 # define V_PRIME_EXP_T    prime_exp_t
 # define V_EXPO           expo
 # define PRIME_LIST_VECT_BLOCK_ITEMS 1
 # define V_ITEM_INIT(x)   x
-#endif
 
 struct prime_exponents
 {
   int num_blocks; /* how many items (in units of vector blocks). */
-  union
-  {
-    /* Note: the size of the arrays below are not included in memory
-     * allocations.  They are dynamic and use the offset of expo in
-     * the structure.
-     */
-    prime_exp_t      expo[PRIME_LIST_VECT_BLOCK_ITEMS * 4];
-#if PRIME_LIST_USE_VECTOR
-    v_prime_exp_t  v_expo[4];
-#endif
-  };
+  /* Note: the size of the arrays below are not included in memory
+   * allocations.  They are dynamic and use the offset of expo in
+   * the structure.
+   */
+  prime_exp_t      expo[WIGXJPF_STR_VAR_LEN_ARRAY_SIZE /* Variable size! */];
 };
 
 extern uint32_t *wigxjpf_prime_list;
 
 extern size_t wigxjpf_prime_fact_stride;
 extern int    wigxjpf_max_prime_decomp;
 extern void *wigxjpf_prime_factors_base;
@@ -167,85 +143,39 @@
 static inline void pexpo_keep_min(struct prime_exponents *keep_fpf,
 				  const struct prime_exponents *in_fpf)
 {
   int i;
 
   assert(keep_fpf->num_blocks == in_fpf->num_blocks);
 
-#if !PRIME_LIST_USE_VECTOR
   for (i = 0; i < keep_fpf->num_blocks; i++)
     {
       keep_fpf->expo[i] =
 	(in_fpf->expo[i] < keep_fpf->expo[i]) ?
 	in_fpf->expo[i] : keep_fpf->expo[i];
     }
-#else
-  for (i = 0; i < keep_fpf->num_blocks; i++)
-    {
-      v_prime_exp_t in_smaller_sign_bit =
-	in_fpf->v_expo[i] - keep_fpf->v_expo[i];
-
-      v_prime_exp_t shift_sign =
-	V_ITEM_INIT(sizeof (prime_exp_t) * 8 - 1);
-
-      v_prime_exp_t in_smaller_all_bits   =
-	in_smaller_sign_bit >> shift_sign;
-      v_prime_exp_t keep_smaller_all_bits = ~in_smaller_all_bits;
-
-      v_prime_exp_t smallest =
-	(in_fpf->v_expo[i] & in_smaller_all_bits) |
-	(keep_fpf->v_expo[i] & keep_smaller_all_bits);
-
-      keep_fpf->v_expo[i] = smallest;
-    }
-#endif
 }
 
 static inline void pexpo_keep_min_in_as_diff(struct prime_exponents *keep_fpf,
 					     struct prime_exponents *in_fpf)
 {
   int i;
 
   assert(keep_fpf->num_blocks == in_fpf->num_blocks);
 
-#if !PRIME_LIST_USE_VECTOR
   for (i = 0; i < keep_fpf->num_blocks; i++)
     {
       prime_exp_t tmp = in_fpf->expo[i] - keep_fpf->expo[i];
 
       keep_fpf->expo[i] =
 	(in_fpf->expo[i] < keep_fpf->expo[i]) ?
 	in_fpf->expo[i] : keep_fpf->expo[i];
 
       in_fpf->expo[i] = tmp;
     }
-#else
-  for (i = 0; i < keep_fpf->num_blocks; i++)
-    {
-      v_prime_exp_t tmp = in_fpf->v_expo[i] - keep_fpf->v_expo[i];
-
-      v_prime_exp_t in_smaller_sign_bit =
-	in_fpf->v_expo[i] - keep_fpf->v_expo[i];
-
-      v_prime_exp_t shift_sign =
-	V_ITEM_INIT(sizeof (prime_exp_t) * 8 - 1);
-
-      v_prime_exp_t in_smaller_all_bits   =
-	in_smaller_sign_bit >> shift_sign;
-      v_prime_exp_t keep_smaller_all_bits = ~in_smaller_all_bits;
-
-      v_prime_exp_t smallest =
-	(in_fpf->v_expo[i] & in_smaller_all_bits) |
-	(keep_fpf->v_expo[i] & keep_smaller_all_bits);
-
-      keep_fpf->v_expo[i] = smallest;
-
-      in_fpf->v_expo[i] = tmp;
-    }
-#endif
 }
 
 struct pexpo_eval_temp
 {
   struct multi_word_int prod_pos[2];
   struct multi_word_int prod_neg[2];
   struct multi_word_int factor[2];
```

### Comparing `pywigxjpf-1.12/src/test_cc_dbl.c` & `pywigxjpf-1.13/src/wigxjpf_error.c`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-/* Copyright 2015 Haakan T. Johansson */
+/* Copyright 2019 Haakan T. Johansson */
 
 /*  This file is part of WIGXJPF.
  *
  *  WIGXJPF is free software: you can redistribute it and/or modify it
  *  under the terms of the GNU Lesser General Public License as
  *  published by the Free Software Foundation, either version 3 of the
  *  License, or (at your option) any later version.
@@ -14,61 +14,45 @@
  *  Lesser General Public License for more details.
  *
  *  You should have received a copy of the GNU Lesser General Public
  *  License along with WIGXJPF.  If not, see
  *  <http://www.gnu.org/licenses/>.
  */
 
-/* This small program is for compile-time test of availability of long
- * double and __float128, threading support,
- */
+#include "wigxjpf_error.h"
 
+#include <stdlib.h>
 #include <stdio.h>
 
-#if TEST_LONG_DOUBLE
-#include <math.h>
-#endif
-#if TEST_FLOAT128
-#include "quadmath.h"
-#endif
-#if TEST_THREAD
-__thread int global = 0;
-#endif
+#if PYWIGXJPF_ERROR_HANDLING
+
+__thread jmp_buf pywigxjpf_jmp_env;
 
-int main()
+void pywigxjpf_error_handler(void)
 {
-#if TEST_LONG_DOUBLE
-  long double a;
-  long double b = 1.14, c = 2.00159;
-  long double d;
-
-  a = b + c;
-  d = ldexpl(c, 5);
-
-  printf ("%Lf\n", a);
-  printf ("#define WIGXJPF_IMPL_LONG_DOUBLE 1\n");
-#endif
-#if TEST_FLOAT128
-  __float128 a;
-  __float128 b = 1.14, c = 2.00159;
-  char s[64];
-
-  a = b + c;
-
-  quadmath_snprintf(s, sizeof(s), "%Qf", a);
-
-  printf ("%s\n", s);
-  printf ("#define WIGXJPF_IMPL_FLOAT128 1\n");
-#endif
-#if TEST_THREAD
-  global = 2;
-  printf ("#define WIGXJPF_HAVE_THREAD 1\n");
-#endif
-#if TEST_UINT128
-  __int128    a;
-  __uint128_t b;
-  printf ("#define MULTI_WORD_INT_SIZEOF_ITEM 8\n");
-#endif
+  /* Allow reuse of the (thread-local) temp array. */
+  wigxjpf_drop_temp();
+
+  fprintf(stderr,
+	  "\n"
+	  "pywigxjpf: Error detected! "
+	  "** Library misuse?  See documentation. **\n"
+	  "\n");
+
+  longjmp(pywigxjpf_jmp_env, 1);
+}
+
+#endif/*PYWIGXJPF_ERROR_HANDLING*/
 
+wigxjpf_error_handler_func_t wigxjpf_error_handler = NULL;
+
+void wigxjpf_error(void)
+{
+  if (wigxjpf_error_handler)
+    {
+      wigxjpf_error_handler();
+      return;
+    }
 
-  return 0;
+  fprintf (stderr, "wigxjpf: Abort.\n");
+  exit(1);
 }
```

### Comparing `pywigxjpf-1.12/src/trivial_zero.c` & `pywigxjpf-1.13/src/trivial_zero.c`

 * *Files identical despite different names*

### Comparing `pywigxjpf-1.12/src/wigxjpf_error.c` & `pywigxjpf-1.13/src/wigxjpf_error.h`

 * *Files 22% similar despite different names*

```diff
@@ -14,45 +14,51 @@
  *  Lesser General Public License for more details.
  *
  *  You should have received a copy of the GNU Lesser General Public
  *  License along with WIGXJPF.  If not, see
  *  <http://www.gnu.org/licenses/>.
  */
 
-#include "wigxjpf_error.h"
+#ifndef __WIGXJPF_ERROR_H__
+#define __WIGXJPF_ERROR_H__
 
-#include <stdlib.h>
-#include <stdio.h>
+#include "wigxjpf_config.h"
+
+typedef void (*wigxjpf_error_handler_func_t)(void);
+
+extern wigxjpf_error_handler_func_t wigxjpf_error_handler;
+
+void wigxjpf_error(void);
 
 #if PYWIGXJPF_ERROR_HANDLING
 
-__thread jmp_buf pywigxjpf_jmp_env;
+#include <setjmp.h>
+
+void pywigxjpf_error_handler(void);
+
+extern __thread jmp_buf pywigxjpf_jmp_env;
+
+/* This is called before every evaluation in the python code, in order
+ * to deal gracefully with invalid user input.
+ *
+ * It is not recommended to do something similar in other code - rather
+ * fix the code to initialise the temporary arrays large enough for all
+ * used symbols!
+ *
+ * Note: wigxjpf_error_handler is a not thread local global, which
+ * does not matter since it will be set to the same every time.
+ */
+# define PYWIGXJPF_ERROR_SETUP(x) do {			\
+    wigxjpf_error_handler = pywigxjpf_error_handler;	\
+    if (setjmp(pywigxjpf_jmp_env))			\
+      return x;						\
+  } while (0)
+#else
+# define PYWIGXJPF_ERROR_SETUP(x) do { } while (0)
+#endif
+
+# define PYWIGXJPF_ERROR_SETUP_void  PYWIGXJPF_ERROR_SETUP()
+# define PYWIGXJPF_ERROR_SETUP_NaN   PYWIGXJPF_ERROR_SETUP(strtof("NAN",NULL))
+
+void wigxjpf_drop_temp(void);
 
-void pywigxjpf_error_handler(void)
-{
-  /* Allow reuse of the (thread-local) temp array. */
-  wigxjpf_drop_temp();
-
-  fprintf(stderr,
-	  "\n"
-	  "pywigxjpf: Error detected! "
-	  "** Library misuse?  See documentation. **\n"
-	  "\n");
-
-  longjmp(pywigxjpf_jmp_env, 1);
-}
-
-#endif/*PYWIGXJPF_ERROR_HANDLING*/
-
-wigxjpf_error_handler_func_t wigxjpf_error_handler = NULL;
-
-void wigxjpf_error(void)
-{
-  if (wigxjpf_error_handler)
-    {
-      wigxjpf_error_handler();
-      return;
-    }
-
-  fprintf (stderr, "wigxjpf: Abort.\n");
-  exit(1);
-}
+#endif/*__WIGXJPF_ERROR_H__*/
```

