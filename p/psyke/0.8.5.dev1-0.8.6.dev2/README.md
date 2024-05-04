# Comparing `tmp/psyke-0.8.5.dev1.tar.gz` & `tmp/psyke-0.8.6.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psyke-0.8.5.dev1.tar", last modified: Thu May  2 15:23:21 2024, max compression
+gzip compressed data, was "psyke-0.8.6.dev2.tar", last modified: Sat May  4 00:09:03 2024, max compression
```

## Comparing `psyke-0.8.5.dev1.tar` & `psyke-0.8.6.dev2.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.614673 psyke-0.8.5.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-05-02 15:23:21.614673 psyke-0.8.5.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 15:23:21.000000 psyke-0.8.5.dev1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.602673 psyke-0.8.5.dev1/psyke/
--rw-r--r--   0 runner    (1001) docker     (127)    18545 2024-05-02 15:23:19.000000 psyke-0.8.5.dev1/psyke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.602673 psyke-0.8.5.dev1/psyke/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/clustering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.602673 psyke-0.8.5.dev1/psyke/clustering/cream/
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/clustering/cream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.602673 psyke-0.8.5.dev1/psyke/clustering/exact/
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/clustering/exact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/clustering/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.602673 psyke-0.8.5.dev1/psyke/extraction/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/extraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.602673 psyke-0.8.5.dev1/psyke/extraction/cart/
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/extraction/cart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/extraction/cart/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.606673 psyke-0.8.5.dev1/psyke/extraction/hypercubic/
--rw-r--r--   0 runner    (1001) docker     (127)    10620 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/extraction/hypercubic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.606673 psyke-0.8.5.dev1/psyke/extraction/hypercubic/cosmik/
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/extraction/hypercubic/cosmik/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.606673 psyke-0.8.5.dev1/psyke/extraction/hypercubic/creepy/
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/extraction/hypercubic/creepy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.606673 psyke-0.8.5.dev1/psyke/extraction/hypercubic/divine/
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/extraction/hypercubic/divine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.606673 psyke-0.8.5.dev1/psyke/extraction/hypercubic/gridex/
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/extraction/hypercubic/gridex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.606673 psyke-0.8.5.dev1/psyke/extraction/hypercubic/gridrex/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/extraction/hypercubic/gridrex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.606673 psyke-0.8.5.dev1/psyke/extraction/hypercubic/hex/
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/extraction/hypercubic/hex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25697 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/extraction/hypercubic/hypercube.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.606673 psyke-0.8.5.dev1/psyke/extraction/hypercubic/iter/
--rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/extraction/hypercubic/iter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/extraction/hypercubic/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/extraction/hypercubic/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.606673 psyke-0.8.5.dev1/psyke/extraction/real/
--rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/extraction/real/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/extraction/real/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.606673 psyke-0.8.5.dev1/psyke/extraction/trepan/
--rw-r--r--   0 runner    (1001) docker     (127)     6583 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/extraction/trepan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/extraction/trepan/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/hypercubepredictor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.606673 psyke-0.8.5.dev1/psyke/schema/
--rw-r--r--   0 runner    (1001) docker     (127)    17444 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.606673 psyke-0.8.5.dev1/psyke/tuning/
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/tuning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.606673 psyke-0.8.5.dev1/psyke/tuning/crash/
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/tuning/crash/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.606673 psyke-0.8.5.dev1/psyke/tuning/orchid/
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/tuning/orchid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.606673 psyke-0.8.5.dev1/psyke/tuning/pedro/
--rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/tuning/pedro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.610673 psyke-0.8.5.dev1/psyke/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/utils/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/utils/logic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/utils/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/psyke/utils/sorted.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.614673 psyke-0.8.5.dev1/psyke.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-05-02 15:23:21.000000 psyke-0.8.5.dev1/psyke.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-02 15:23:21.000000 psyke-0.8.5.dev1/psyke.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:23:21.000000 psyke-0.8.5.dev1/psyke.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:23:21.000000 psyke-0.8.5.dev1/psyke.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-02 15:23:21.000000 psyke-0.8.5.dev1/psyke.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-02 15:23:21.000000 psyke-0.8.5.dev1/psyke.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 15:23:21.614673 psyke-0.8.5.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.598673 psyke-0.8.5.dev1/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.610673 psyke-0.8.5.dev1/test/psyke/
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/test/psyke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.610673 psyke-0.8.5.dev1/test/psyke/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/test/psyke/clustering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.610673 psyke-0.8.5.dev1/test/psyke/extraction/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/test/psyke/extraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.610673 psyke-0.8.5.dev1/test/psyke/extraction/cart/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/test/psyke/extraction/cart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/test/psyke/extraction/cart/test_cart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/test/psyke/extraction/cart/test_simplified_cart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.610673 psyke-0.8.5.dev1/test/psyke/extraction/hypercubic/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/test/psyke/extraction/hypercubic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.610673 psyke-0.8.5.dev1/test/psyke/extraction/hypercubic/gridex/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/test/psyke/extraction/hypercubic/gridex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/test/psyke/extraction/hypercubic/gridex/test_gridex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.610673 psyke-0.8.5.dev1/test/psyke/extraction/hypercubic/iter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/test/psyke/extraction/hypercubic/iter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/test/psyke/extraction/hypercubic/iter/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14255 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/test/psyke/extraction/hypercubic/test_hypercube.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.614673 psyke-0.8.5.dev1/test/psyke/extraction/real/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/test/psyke/extraction/real/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/test/psyke/extraction/real/test_real.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/test/psyke/extraction/real/test_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.614673 psyke-0.8.5.dev1/test/psyke/extraction/trepan/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/test/psyke/extraction/trepan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/test/psyke/extraction/trepan/test_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/test/psyke/extraction/trepan/test_split.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/test/psyke/extraction/trepan/test_trepan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.614673 psyke-0.8.5.dev1/test/psyke/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/test/psyke/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/test/psyke/utils/test_prune.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/test/psyke/utils/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-02 15:22:11.000000 psyke-0.8.5.dev1/test/psyke/utils/test_simplify_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.614673 psyke-0.8.5.dev1/test/resources/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-02 15:22:13.000000 psyke-0.8.5.dev1/test/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.614673 psyke-0.8.5.dev1/test/resources/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-02 15:22:13.000000 psyke-0.8.5.dev1/test/resources/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.614673 psyke-0.8.5.dev1/test/resources/predictors/
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-02 15:22:13.000000 psyke-0.8.5.dev1/test/resources/predictors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:23:21.614673 psyke-0.8.5.dev1/test/resources/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-02 15:22:13.000000 psyke-0.8.5.dev1/test/resources/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.176646 psyke-0.8.6.dev2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-05-04 00:09:03.176646 psyke-0.8.6.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-04 00:09:03.000000 psyke-0.8.6.dev2/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.164646 psyke-0.8.6.dev2/psyke/
+-rw-r--r--   0 runner    (1001) docker     (127)    18545 2024-05-04 00:09:00.000000 psyke-0.8.6.dev2/psyke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.168646 psyke-0.8.6.dev2/psyke/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/clustering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.168646 psyke-0.8.6.dev2/psyke/clustering/cream/
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/clustering/cream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.168646 psyke-0.8.6.dev2/psyke/clustering/exact/
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/clustering/exact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/clustering/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.168646 psyke-0.8.6.dev2/psyke/extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.168646 psyke-0.8.6.dev2/psyke/extraction/cart/
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/cart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/cart/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.168646 psyke-0.8.6.dev2/psyke/extraction/hypercubic/
+-rw-r--r--   0 runner    (1001) docker     (127)    10620 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/hypercubic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.168646 psyke-0.8.6.dev2/psyke/extraction/hypercubic/cosmik/
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/hypercubic/cosmik/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.168646 psyke-0.8.6.dev2/psyke/extraction/hypercubic/creepy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/hypercubic/creepy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.168646 psyke-0.8.6.dev2/psyke/extraction/hypercubic/divine/
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/hypercubic/divine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.168646 psyke-0.8.6.dev2/psyke/extraction/hypercubic/gridex/
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/hypercubic/gridex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.168646 psyke-0.8.6.dev2/psyke/extraction/hypercubic/gridrex/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/hypercubic/gridrex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.168646 psyke-0.8.6.dev2/psyke/extraction/hypercubic/hex/
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/hypercubic/hex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25697 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/hypercubic/hypercube.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.168646 psyke-0.8.6.dev2/psyke/extraction/hypercubic/iter/
+-rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/hypercubic/iter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/hypercubic/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/hypercubic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.168646 psyke-0.8.6.dev2/psyke/extraction/real/
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/real/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/real/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.172646 psyke-0.8.6.dev2/psyke/extraction/trepan/
+-rw-r--r--   0 runner    (1001) docker     (127)     6583 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/trepan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/extraction/trepan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/hypercubepredictor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.172646 psyke-0.8.6.dev2/psyke/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)    17444 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.172646 psyke-0.8.6.dev2/psyke/tuning/
+-rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/tuning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.172646 psyke-0.8.6.dev2/psyke/tuning/crash/
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/tuning/crash/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.172646 psyke-0.8.6.dev2/psyke/tuning/orchid/
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/tuning/orchid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.172646 psyke-0.8.6.dev2/psyke/tuning/pedro/
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/tuning/pedro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.172646 psyke-0.8.6.dev2/psyke/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/utils/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/utils/logic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/psyke/utils/sorted.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.176646 psyke-0.8.6.dev2/psyke.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-05-04 00:09:03.000000 psyke-0.8.6.dev2/psyke.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-04 00:09:03.000000 psyke-0.8.6.dev2/psyke.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 00:09:03.000000 psyke-0.8.6.dev2/psyke.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 00:09:02.000000 psyke-0.8.6.dev2/psyke.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-04 00:09:03.000000 psyke-0.8.6.dev2/psyke.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 00:09:03.000000 psyke-0.8.6.dev2/psyke.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 00:09:03.176646 psyke-0.8.6.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.164646 psyke-0.8.6.dev2/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.172646 psyke-0.8.6.dev2/test/psyke/
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.172646 psyke-0.8.6.dev2/test/psyke/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/clustering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.172646 psyke-0.8.6.dev2/test/psyke/extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.172646 psyke-0.8.6.dev2/test/psyke/extraction/cart/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/cart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/cart/test_cart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/cart/test_simplified_cart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.172646 psyke-0.8.6.dev2/test/psyke/extraction/hypercubic/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/hypercubic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.172646 psyke-0.8.6.dev2/test/psyke/extraction/hypercubic/gridex/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/hypercubic/gridex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/hypercubic/gridex/test_gridex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.176646 psyke-0.8.6.dev2/test/psyke/extraction/hypercubic/iter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/hypercubic/iter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/hypercubic/iter/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14255 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/hypercubic/test_hypercube.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.176646 psyke-0.8.6.dev2/test/psyke/extraction/real/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/real/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/real/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/real/test_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.176646 psyke-0.8.6.dev2/test/psyke/extraction/trepan/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/trepan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/trepan/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/trepan/test_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/extraction/trepan/test_trepan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.176646 psyke-0.8.6.dev2/test/psyke/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/utils/test_prune.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/utils/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-04 00:07:21.000000 psyke-0.8.6.dev2/test/psyke/utils/test_simplify_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.176646 psyke-0.8.6.dev2/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-04 00:07:23.000000 psyke-0.8.6.dev2/test/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.176646 psyke-0.8.6.dev2/test/resources/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-04 00:07:23.000000 psyke-0.8.6.dev2/test/resources/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.176646 psyke-0.8.6.dev2/test/resources/predictors/
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-04 00:07:23.000000 psyke-0.8.6.dev2/test/resources/predictors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:09:03.176646 psyke-0.8.6.dev2/test/resources/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-04 00:07:23.000000 psyke-0.8.6.dev2/test/resources/tests/__init__.py
```

### Comparing `psyke-0.8.5.dev1/LICENSE` & `psyke-0.8.6.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/PKG-INFO` & `psyke-0.8.6.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyke
-Version: 0.8.5.dev1
+Version: 0.8.6.dev2
 Summary: Python-based implementation of PSyKE, i.e. a Platform for Symbolic Knowledge Extraction
 Home-page: https://github.com/psykei/psyke-python
 Author: Matteo Magnini
 Author-email: matteo.magnini@unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/psykei/psyke-python/issues
 Project-URL: Source, https://github.com/psykei/psyke-python
```

### Comparing `psyke-0.8.5.dev1/README.md` & `psyke-0.8.6.dev2/README.md`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/__init__.py` & `psyke-0.8.6.dev2/psyke/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/clustering/__init__.py` & `psyke-0.8.6.dev2/psyke/clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/clustering/cream/__init__.py` & `psyke-0.8.6.dev2/psyke/clustering/cream/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/clustering/exact/__init__.py` & `psyke-0.8.6.dev2/psyke/clustering/exact/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/clustering/utils.py` & `psyke-0.8.6.dev2/psyke/clustering/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/extraction/__init__.py` & `psyke-0.8.6.dev2/psyke/extraction/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/extraction/cart/__init__.py` & `psyke-0.8.6.dev2/psyke/extraction/cart/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         return simplified
 
     def _create_theory(self, data: pd.DataFrame) -> Theory:
         new_theory = mutable_theory()
         nodes = [node for node in self._cart_predictor]
         nodes = Cart._simplify_nodes(nodes) if self._simplify else nodes
         for (constraints, prediction) in nodes:
-            if self.normalization is not None:
+            if self.normalization is not None and data.columns[-1] in self.normalization:
                 m, s = self.normalization[data.columns[-1]]
                 prediction = prediction * s + m
             variables = create_variable_list(self.discretization, data)
             new_theory.assertZ(
                 clause(
                     create_head(data.columns[-1], list(variables.values()), prediction),
                     self._create_body(variables, constraints)
```

### Comparing `psyke-0.8.5.dev1/psyke/extraction/cart/predictor.py` & `psyke-0.8.6.dev2/psyke/extraction/cart/predictor.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/extraction/hypercubic/__init__.py` & `psyke-0.8.6.dev2/psyke/extraction/hypercubic/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/extraction/hypercubic/cosmik/__init__.py` & `psyke-0.8.6.dev2/psyke/extraction/hypercubic/cosmik/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/extraction/hypercubic/creepy/__init__.py` & `psyke-0.8.6.dev2/psyke/extraction/hypercubic/creepy/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/extraction/hypercubic/divine/__init__.py` & `psyke-0.8.6.dev2/psyke/extraction/hypercubic/divine/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/extraction/hypercubic/gridex/__init__.py` & `psyke-0.8.6.dev2/psyke/extraction/hypercubic/gridex/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/extraction/hypercubic/gridrex/__init__.py` & `psyke-0.8.6.dev2/psyke/extraction/hypercubic/gridrex/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/extraction/hypercubic/hex/__init__.py` & `psyke-0.8.6.dev2/psyke/extraction/hypercubic/hex/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/extraction/hypercubic/hypercube.py` & `psyke-0.8.6.dev2/psyke/extraction/hypercubic/hypercube.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/extraction/hypercubic/iter/__init__.py` & `psyke-0.8.6.dev2/psyke/extraction/hypercubic/iter/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/extraction/hypercubic/strategy.py` & `psyke-0.8.6.dev2/psyke/extraction/hypercubic/strategy.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/extraction/hypercubic/utils.py` & `psyke-0.8.6.dev2/psyke/extraction/hypercubic/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/extraction/real/__init__.py` & `psyke-0.8.6.dev2/psyke/extraction/real/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/extraction/real/utils.py` & `psyke-0.8.6.dev2/psyke/extraction/real/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/extraction/trepan/__init__.py` & `psyke-0.8.6.dev2/psyke/extraction/trepan/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/extraction/trepan/utils.py` & `psyke-0.8.6.dev2/psyke/extraction/trepan/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/hypercubepredictor.py` & `psyke-0.8.6.dev2/psyke/hypercubepredictor.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/schema/__init__.py` & `psyke-0.8.6.dev2/psyke/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/tuning/__init__.py` & `psyke-0.8.6.dev2/psyke/tuning/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,8 +80,10 @@
                 (1 - other[0] / best[0]) ** self.readability_tradeoff *
                 np.ceil(other[1] / self.readability_tradeoff) / np.ceil(best[1] / self.readability_tradeoff)
         )
 
     def _check_iteration_improvement(self, best, current):
         improvement = \
             self._iteration_improvement([best[0], best[1]], [current[0], current[1]]) if best is not None else np.inf
+        if isinstance(improvement, complex):
+            improvement = 1.0
         return current, improvement < 1.2
```

### Comparing `psyke-0.8.5.dev1/psyke/tuning/crash/__init__.py` & `psyke-0.8.6.dev2/psyke/tuning/crash/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/tuning/orchid/__init__.py` & `psyke-0.8.6.dev2/psyke/tuning/orchid/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/tuning/pedro/__init__.py` & `psyke-0.8.6.dev2/psyke/tuning/pedro/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,42 +94,46 @@
     def __contains(self, strategies, strategy):
         for s in strategies:
             if strategy.equals(s, self.dataframe.columns[:-1]):
                 return True
         return False
 
     def search(self):
-        base_strategy = FixedStrategy(2)
-        strategies = [base_strategy, FixedStrategy(3)]
-
-        base_partitions = base_strategy.partition_number(self.dataframe.columns[:-1])
+        base_partitions = FixedStrategy(2).partition_number(self.dataframe.columns[:-1]) * 3
+        if base_partitions <= 50:
+            strategies = [FixedStrategy(2)]
+            if FixedStrategy(3).partition_number(self.dataframe.columns[:-1]) <= base_partitions:
+                strategies.append(FixedStrategy(3))
+        else:
+            strategies = []
+            base_partitions = 50
 
         for n in [2, 3, 5, 10]:
             for th in [0.99, 0.75, 0.67, 0.5, 0.3]:
                 strategy = AdaptiveStrategy(self.ranked, [(th, n)])
-                if strategy.partition_number(self.dataframe.columns[:-1]) < base_partitions * 3 and \
+                if strategy.partition_number(self.dataframe.columns[:-1]) < base_partitions and \
                         not self.__contains(strategies, strategy):
                     strategies.append(strategy)
 
         for (a, b) in [(0.33, 0.67), (0.25, 0.75), (0.1, 0.9)]:
             strategy = AdaptiveStrategy(self.ranked, [(a, 2), (b, 3)])
-            if strategy.partition_number(self.dataframe.columns[:-1]) < base_partitions * 3 and \
+            if strategy.partition_number(self.dataframe.columns[:-1]) < base_partitions and \
                     not self.__contains(strategies, strategy):
                 strategies.append(strategy)
 
         avg = 0.
         for strategy in strategies:
             avg += strategy.partition_number(self.dataframe.columns[:-1])
         avg /= len(strategies)
 
         params = []
         for strategy in strategies:
             params += self._search_depth(strategy,
                                          strategy.partition_number(self.dataframe.columns[:-1]) > avg,
-                                         base_partitions * 3)
+                                         base_partitions)
         self.params = params
 
     def _print_params(self, name, params):
         print("**********************")
         print(f"Best {name}")
         print("**********************")
         print(f"Error = {params[0]:.2f}, {params[1]} rules")
```

### Comparing `psyke-0.8.5.dev1/psyke/utils/__init__.py` & `psyke-0.8.6.dev2/psyke/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/utils/dataframe.py` & `psyke-0.8.6.dev2/psyke/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/utils/logic.py` & `psyke-0.8.6.dev2/psyke/utils/logic.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/utils/metrics.py` & `psyke-0.8.6.dev2/psyke/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/utils/plot.py` & `psyke-0.8.6.dev2/psyke/utils/plot.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke/utils/sorted.py` & `psyke-0.8.6.dev2/psyke/utils/sorted.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/psyke.egg-info/PKG-INFO` & `psyke-0.8.6.dev2/psyke.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyke
-Version: 0.8.5.dev1
+Version: 0.8.6.dev2
 Summary: Python-based implementation of PSyKE, i.e. a Platform for Symbolic Knowledge Extraction
 Home-page: https://github.com/psykei/psyke-python
 Author: Matteo Magnini
 Author-email: matteo.magnini@unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/psykei/psyke-python/issues
 Project-URL: Source, https://github.com/psykei/psyke-python
```

### Comparing `psyke-0.8.5.dev1/psyke.egg-info/SOURCES.txt` & `psyke-0.8.6.dev2/psyke.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/setup.py` & `psyke-0.8.6.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/test/psyke/__init__.py` & `psyke-0.8.6.dev2/test/psyke/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/test/psyke/extraction/cart/test_cart.py` & `psyke-0.8.6.dev2/test/psyke/extraction/cart/test_cart.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/test/psyke/extraction/cart/test_simplified_cart.py` & `psyke-0.8.6.dev2/test/psyke/extraction/cart/test_simplified_cart.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/test/psyke/extraction/hypercubic/gridex/test_gridex.py` & `psyke-0.8.6.dev2/test/psyke/extraction/hypercubic/gridex/test_gridex.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/test/psyke/extraction/hypercubic/iter/test_iter.py` & `psyke-0.8.6.dev2/test/psyke/extraction/hypercubic/iter/test_iter.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/test/psyke/extraction/hypercubic/test_hypercube.py` & `psyke-0.8.6.dev2/test/psyke/extraction/hypercubic/test_hypercube.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/test/psyke/extraction/real/test_real.py` & `psyke-0.8.6.dev2/test/psyke/extraction/real/test_real.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/test/psyke/extraction/real/test_rule.py` & `psyke-0.8.6.dev2/test/psyke/extraction/real/test_rule.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/test/psyke/extraction/trepan/test_node.py` & `psyke-0.8.6.dev2/test/psyke/extraction/trepan/test_node.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/test/psyke/extraction/trepan/test_split.py` & `psyke-0.8.6.dev2/test/psyke/extraction/trepan/test_split.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/test/psyke/extraction/trepan/test_trepan.py` & `psyke-0.8.6.dev2/test/psyke/extraction/trepan/test_trepan.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/test/psyke/utils/test_prune.py` & `psyke-0.8.6.dev2/test/psyke/utils/test_prune.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/test/psyke/utils/test_simplify.py` & `psyke-0.8.6.dev2/test/psyke/utils/test_simplify.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/test/psyke/utils/test_simplify_formatter.py` & `psyke-0.8.6.dev2/test/psyke/utils/test_simplify_formatter.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.5.dev1/test/resources/tests/__init__.py` & `psyke-0.8.6.dev2/test/resources/tests/__init__.py`

 * *Files identical despite different names*

