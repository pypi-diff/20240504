# Comparing `tmp/spotlight-sdk-0.0.8.tar.gz` & `tmp/spotlight-sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotlight-sdk-0.0.8.tar", last modified: Wed Feb  7 23:06:02 2024, max compression
+gzip compressed data, was "spotlight-sdk-0.0.9.tar", last modified: Mon Feb 12 17:02:44 2024, max compression
```

## Comparing `spotlight-sdk-0.0.8.tar` & `spotlight-sdk-0.0.9.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 23:06:02.013445 spotlight-sdk-0.0.8/
--rw-r--r--   0 root         (0) root         (0)     1264 2024-02-07 23:06:02.013445 spotlight-sdk-0.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      709 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-07 23:06:02.014445 spotlight-sdk-0.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 23:06:01.984442 spotlight-sdk-0.0.8/spotlight/
--rw-rw-rw-   0 root         (0) root         (0)       44 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 23:06:01.985442 spotlight-sdk-0.0.8/spotlight/admin/
--rw-rw-rw-   0 root         (0) root         (0)      955 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/admin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3114 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/admin/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     7658 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/admin/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     6877 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/admin/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 23:06:01.985442 spotlight-sdk-0.0.8/spotlight/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 23:06:01.986442 spotlight-sdk-0.0.8/spotlight/api/auth/
--rw-rw-rw-   0 root         (0) root         (0)      215 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1349 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/auth/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     2263 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/auth/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1727 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/auth/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 23:06:01.989442 spotlight-sdk-0.0.8/spotlight/api/data/
--rw-rw-rw-   0 root         (0) root         (0)      426 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/data/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     3081 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/data/asynchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 23:06:01.991443 spotlight-sdk-0.0.8/spotlight/api/data/barchart/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/data/barchart/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      318 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/data/barchart/__util.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/data/barchart/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      303 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/data/barchart/model.py
--rw-rw-rw-   0 root         (0) root         (0)      619 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/data/barchart/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1406 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/data/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2811 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/data/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 23:06:01.993443 spotlight-sdk-0.0.8/spotlight/api/dataset/
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      871 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/dataset/__util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 23:06:01.995443 spotlight-sdk-0.0.8/spotlight/api/dataset/abstract/
--rw-rw-rw-   0 root         (0) root         (0)      495 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/dataset/abstract/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1041 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/dataset/abstract/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     3141 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/dataset/abstract/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1002 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/dataset/abstract/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2805 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/dataset/abstract/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     2748 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/dataset/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1396 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/dataset/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2446 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/dataset/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 23:06:01.996443 spotlight-sdk-0.0.8/spotlight/api/dataset/view/
--rw-rw-rw-   0 root         (0) root         (0)      271 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/dataset/view/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      443 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/dataset/view/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1530 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/dataset/view/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/dataset/view/model.py
--rw-rw-rw-   0 root         (0) root         (0)     1370 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/dataset/view/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 23:06:01.999443 spotlight-sdk-0.0.8/spotlight/api/permission/
--rw-rw-rw-   0 root         (0) root         (0)      488 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/permission/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      897 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/permission/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     3008 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/permission/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/permission/enum.py
--rw-rw-rw-   0 root         (0) root         (0)      287 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/permission/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2656 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/api/permission/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 23:06:02.000444 spotlight-sdk-0.0.8/spotlight/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 23:06:02.003444 spotlight-sdk-0.0.8/spotlight/core/common/
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/core/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2650 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/core/common/base.py
--rw-rw-rw-   0 root         (0) root         (0)      231 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/core/common/base_enum.py
--rw-rw-rw-   0 root         (0) root         (0)     2978 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/core/common/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 23:06:02.004444 spotlight-sdk-0.0.8/spotlight/core/common/date/
--rw-rw-rw-   0 root         (0) root         (0)      206 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/core/common/date/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2417 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/core/common/date/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 23:06:02.004444 spotlight-sdk-0.0.8/spotlight/core/common/decorators/
--rw-rw-rw-   0 root         (0) root         (0)      345 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/core/common/decorators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 23:06:02.006444 spotlight-sdk-0.0.8/spotlight/core/common/decorators/authorization/
--rw-rw-rw-   0 root         (0) root         (0)      254 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/core/common/decorators/authorization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1154 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/core/common/decorators/authorization/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     3921 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/core/common/decorators/authorization/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     3899 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/core/common/decorators/authorization/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 23:06:02.008444 spotlight-sdk-0.0.8/spotlight/core/common/decorators/data/
--rw-rw-rw-   0 root         (0) root         (0)      191 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/core/common/decorators/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/core/common/decorators/data/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1381 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/core/common/decorators/data/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1400 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/core/common/decorators/data/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      686 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/core/common/decorators/timeit.py
--rw-rw-rw-   0 root         (0) root         (0)      692 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/core/common/enum.py
--rw-rw-rw-   0 root         (0) root         (0)      726 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/core/common/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     4795 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/core/common/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 23:06:02.010444 spotlight-sdk-0.0.8/spotlight/core/common/metaclass/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/core/common/metaclass/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/core/common/metaclass/singleton.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 23:06:02.010444 spotlight-sdk-0.0.8/spotlight/core/common/requests/
--rw-rw-rw-   0 root         (0) root         (0)      404 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/core/common/requests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4689 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/core/common/requests/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     3788 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/core/common/requests/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      242 2024-02-07 23:05:48.000000 spotlight-sdk-0.0.8/spotlight/core/common/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 23:06:02.013445 spotlight-sdk-0.0.8/spotlight_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1264 2024-02-07 23:06:01.000000 spotlight-sdk-0.0.8/spotlight_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2782 2024-02-07 23:06:01.000000 spotlight-sdk-0.0.8/spotlight_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-07 23:06:01.000000 spotlight-sdk-0.0.8/spotlight_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      176 2024-02-07 23:06:01.000000 spotlight-sdk-0.0.8/spotlight_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-02-07 23:06:01.000000 spotlight-sdk-0.0.8/spotlight_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.577653 spotlight-sdk-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)     1264 2024-02-12 17:02:44.576653 spotlight-sdk-0.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      709 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-02-12 17:02:44.577653 spotlight-sdk-0.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.560652 spotlight-sdk-0.0.9/spotlight/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.561652 spotlight-sdk-0.0.9/spotlight/admin/
+-rw-rw-rw-   0 root         (0) root         (0)      955 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/admin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3114 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/admin/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     7658 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/admin/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     6877 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/admin/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.561652 spotlight-sdk-0.0.9/spotlight/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.562652 spotlight-sdk-0.0.9/spotlight/api/auth/
+-rw-rw-rw-   0 root         (0) root         (0)      215 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1349 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/auth/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2263 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/auth/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/auth/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.563652 spotlight-sdk-0.0.9/spotlight/api/data/
+-rw-rw-rw-   0 root         (0) root         (0)      426 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/data/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3081 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/data/asynchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.564652 spotlight-sdk-0.0.9/spotlight/api/data/barchart/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/data/barchart/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      318 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/data/barchart/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/data/barchart/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      303 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/data/barchart/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      619 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/data/barchart/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/data/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2811 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/data/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.565652 spotlight-sdk-0.0.9/spotlight/api/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      871 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/dataset/__util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.567653 spotlight-sdk-0.0.9/spotlight/api/dataset/abstract/
+-rw-rw-rw-   0 root         (0) root         (0)      495 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/dataset/abstract/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/dataset/abstract/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3141 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/dataset/abstract/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/dataset/abstract/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2805 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/dataset/abstract/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     2748 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/dataset/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1396 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/dataset/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2446 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/dataset/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.568652 spotlight-sdk-0.0.9/spotlight/api/dataset/view/
+-rw-rw-rw-   0 root         (0) root         (0)      271 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/dataset/view/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      443 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/dataset/view/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1530 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/dataset/view/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/dataset/view/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1370 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/dataset/view/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.569653 spotlight-sdk-0.0.9/spotlight/api/permission/
+-rw-rw-rw-   0 root         (0) root         (0)      488 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/permission/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      897 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/permission/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3008 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/permission/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/permission/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)      287 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/permission/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2656 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/permission/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.569653 spotlight-sdk-0.0.9/spotlight/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.571653 spotlight-sdk-0.0.9/spotlight/core/common/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2650 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      231 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/base_enum.py
+-rw-rw-rw-   0 root         (0) root         (0)     2978 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.572653 spotlight-sdk-0.0.9/spotlight/core/common/date/
+-rw-rw-rw-   0 root         (0) root         (0)      206 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/date/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2417 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/date/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.572653 spotlight-sdk-0.0.9/spotlight/core/common/decorators/
+-rw-rw-rw-   0 root         (0) root         (0)      345 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/decorators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.573653 spotlight-sdk-0.0.9/spotlight/core/common/decorators/authorization/
+-rw-rw-rw-   0 root         (0) root         (0)      254 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/decorators/authorization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1266 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/decorators/authorization/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3921 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/decorators/authorization/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     3899 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/decorators/authorization/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.574653 spotlight-sdk-0.0.9/spotlight/core/common/decorators/data/
+-rw-rw-rw-   0 root         (0) root         (0)      191 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/decorators/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/decorators/data/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/decorators/data/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1400 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/decorators/data/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      686 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/decorators/timeit.py
+-rw-rw-rw-   0 root         (0) root         (0)      692 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)      726 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     4795 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.574653 spotlight-sdk-0.0.9/spotlight/core/common/metaclass/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/metaclass/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/metaclass/singleton.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.575653 spotlight-sdk-0.0.9/spotlight/core/common/requests/
+-rw-rw-rw-   0 root         (0) root         (0)      404 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/requests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4689 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/requests/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     3788 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/requests/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      242 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.576653 spotlight-sdk-0.0.9/spotlight_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1264 2024-02-12 17:02:44.000000 spotlight-sdk-0.0.9/spotlight_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2782 2024-02-12 17:02:44.000000 spotlight-sdk-0.0.9/spotlight_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-12 17:02:44.000000 spotlight-sdk-0.0.9/spotlight_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      176 2024-02-12 17:02:44.000000 spotlight-sdk-0.0.9/spotlight_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-02-12 17:02:44.000000 spotlight-sdk-0.0.9/spotlight_sdk.egg-info/top_level.txt
```

### Comparing `spotlight-sdk-0.0.8/PKG-INFO` & `spotlight-sdk-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotlight-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: Spotlight Python SDK
 Home-page: https://spotlight.dev
 Author: Spotlight
 Author-email: hello@spotlight.dev
 License: UNKNOWN
 Description: # Spotlight: The OTC Commodity Research Platform
```

### Comparing `spotlight-sdk-0.0.8/README.md` & `spotlight-sdk-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/setup.py` & `spotlight-sdk-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/admin/__init__.py` & `spotlight-sdk-0.0.9/spotlight/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/admin/__util.py` & `spotlight-sdk-0.0.9/spotlight/admin/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/admin/asynchronous.py` & `spotlight-sdk-0.0.9/spotlight/admin/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/admin/synchronous.py` & `spotlight-sdk-0.0.9/spotlight/admin/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/api/auth/__util.py` & `spotlight-sdk-0.0.9/spotlight/api/auth/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/api/auth/asynchronous.py` & `spotlight-sdk-0.0.9/spotlight/api/auth/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/api/auth/synchronous.py` & `spotlight-sdk-0.0.9/spotlight/api/auth/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/api/data/__util.py` & `spotlight-sdk-0.0.9/spotlight/api/data/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/api/data/asynchronous.py` & `spotlight-sdk-0.0.9/spotlight/api/data/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/api/data/barchart/asynchronous.py` & `spotlight-sdk-0.0.9/spotlight/api/data/barchart/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/api/data/barchart/synchronous.py` & `spotlight-sdk-0.0.9/spotlight/api/data/barchart/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/api/data/model.py` & `spotlight-sdk-0.0.9/spotlight/api/data/model.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/api/data/synchronous.py` & `spotlight-sdk-0.0.9/spotlight/api/data/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/api/dataset/__util.py` & `spotlight-sdk-0.0.9/spotlight/api/dataset/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/api/dataset/abstract/__util.py` & `spotlight-sdk-0.0.9/spotlight/api/dataset/abstract/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/api/dataset/abstract/asynchronous.py` & `spotlight-sdk-0.0.9/spotlight/api/dataset/abstract/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/api/dataset/abstract/model.py` & `spotlight-sdk-0.0.9/spotlight/api/dataset/abstract/model.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/api/dataset/abstract/synchronous.py` & `spotlight-sdk-0.0.9/spotlight/api/dataset/abstract/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/api/dataset/asynchronous.py` & `spotlight-sdk-0.0.9/spotlight/api/dataset/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/api/dataset/model.py` & `spotlight-sdk-0.0.9/spotlight/api/dataset/model.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/api/dataset/synchronous.py` & `spotlight-sdk-0.0.9/spotlight/api/dataset/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/api/dataset/view/asynchronous.py` & `spotlight-sdk-0.0.9/spotlight/api/dataset/view/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/api/dataset/view/model.py` & `spotlight-sdk-0.0.9/spotlight/api/dataset/view/model.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/api/dataset/view/synchronous.py` & `spotlight-sdk-0.0.9/spotlight/api/dataset/view/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/api/permission/__util.py` & `spotlight-sdk-0.0.9/spotlight/api/permission/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/api/permission/asynchronous.py` & `spotlight-sdk-0.0.9/spotlight/api/permission/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/api/permission/synchronous.py` & `spotlight-sdk-0.0.9/spotlight/api/permission/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/core/common/base.py` & `spotlight-sdk-0.0.9/spotlight/core/common/base.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/core/common/config.py` & `spotlight-sdk-0.0.9/spotlight/core/common/config.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/core/common/date/function.py` & `spotlight-sdk-0.0.9/spotlight/core/common/date/function.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/core/common/decorators/authorization/__util.py` & `spotlight-sdk-0.0.9/spotlight/core/common/decorators/authorization/__util.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 
 
 def _handle_auth_response(auth_response: Response, error_msg: str) -> dict:
     if auth_response.status_code == 200:
         bearer_token = auth_response.json()["access_token"]
         return {"Authorization": f"Bearer {bearer_token}"}
     else:
-        error = AuthenticationError(error_msg)
+        error = AuthenticationError(
+            f"Status Code: {auth_response.status_code}\nResponse content: {auth_response.content}\n{error_msg}"
+        )
         logger.error(error)
         raise error
 
 
 def _access_token(access_token: str) -> dict:
     return json.loads(access_token)
```

### Comparing `spotlight-sdk-0.0.8/spotlight/core/common/decorators/authorization/asynchronous.py` & `spotlight-sdk-0.0.9/spotlight/core/common/decorators/authorization/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/core/common/decorators/authorization/synchronous.py` & `spotlight-sdk-0.0.9/spotlight/core/common/decorators/authorization/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/core/common/decorators/data/__util.py` & `spotlight-sdk-0.0.9/spotlight/core/common/decorators/data/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/core/common/decorators/data/asynchronous.py` & `spotlight-sdk-0.0.9/spotlight/core/common/decorators/data/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/core/common/decorators/data/synchronous.py` & `spotlight-sdk-0.0.9/spotlight/core/common/decorators/data/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/core/common/decorators/timeit.py` & `spotlight-sdk-0.0.9/spotlight/core/common/decorators/timeit.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/core/common/enum.py` & `spotlight-sdk-0.0.9/spotlight/core/common/enum.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/core/common/errors.py` & `spotlight-sdk-0.0.9/spotlight/core/common/errors.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/core/common/function.py` & `spotlight-sdk-0.0.9/spotlight/core/common/function.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/core/common/metaclass/singleton.py` & `spotlight-sdk-0.0.9/spotlight/core/common/metaclass/singleton.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/core/common/requests/asynchronous.py` & `spotlight-sdk-0.0.9/spotlight/core/common/requests/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight/core/common/requests/synchronous.py` & `spotlight-sdk-0.0.9/spotlight/core/common/requests/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.8/spotlight_sdk.egg-info/PKG-INFO` & `spotlight-sdk-0.0.9/spotlight_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotlight-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: Spotlight Python SDK
 Home-page: https://spotlight.dev
 Author: Spotlight
 Author-email: hello@spotlight.dev
 License: UNKNOWN
 Description: # Spotlight: The OTC Commodity Research Platform
```

### Comparing `spotlight-sdk-0.0.8/spotlight_sdk.egg-info/SOURCES.txt` & `spotlight-sdk-0.0.9/spotlight_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

