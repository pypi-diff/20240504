# Comparing `tmp/haskellian-0.3.8.tar.gz` & `tmp/haskellian-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haskellian-0.3.8.tar", last modified: Tue Apr 23 05:10:25 2024, max compression
+gzip compressed data, was "haskellian-0.3.9.tar", last modified: Thu Apr 25 06:09:34 2024, max compression
```

## Comparing `haskellian-0.3.8.tar` & `haskellian-0.3.9.tar`

### file list

```diff
@@ -1,68 +1,72 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 05:10:25.489484 haskellian-0.3.8/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1539 2024-04-23 05:10:25.489484 haskellian-0.3.8/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1154 2024-04-22 10:09:42.000000 haskellian-0.3.8/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      514 2024-04-23 05:10:22.000000 haskellian-0.3.8/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-23 05:10:25.489484 haskellian-0.3.8/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 05:10:25.469484 haskellian-0.3.8/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 05:10:25.469484 haskellian-0.3.8/src/haskellian/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      156 2024-04-21 08:31:50.000000 haskellian-0.3.8/src/haskellian/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      494 2024-04-22 10:03:32.000000 haskellian-0.3.8/src/haskellian/__init__.pyi
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 05:10:25.479484 haskellian-0.3.8/src/haskellian/asyn_iter/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 14:25:49.000000 haskellian-0.3.8/src/haskellian/asyn_iter/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      455 2024-04-23 05:08:08.000000 haskellian-0.3.8/src/haskellian/asyn_iter/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2319 2024-04-23 05:07:58.000000 haskellian-0.3.8/src/haskellian/asyn_iter/funcs.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2189 2024-04-23 05:08:49.000000 haskellian-0.3.8/src/haskellian/asyn_iter/iter.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      490 2024-04-21 14:38:54.000000 haskellian-0.3.8/src/haskellian/asyn_iter/lifting.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      886 2024-04-21 14:38:19.000000 haskellian-0.3.8/src/haskellian/asyn_iter/managed.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      650 2024-04-21 14:40:28.000000 haskellian-0.3.8/src/haskellian/asyn_iter/prefetching.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 05:10:25.479484 haskellian-0.3.8/src/haskellian/classes/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 09:04:50.000000 haskellian-0.3.8/src/haskellian/classes/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      137 2024-04-21 09:04:51.000000 haskellian-0.3.8/src/haskellian/classes/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      578 2024-04-21 10:23:51.000000 haskellian-0.3.8/src/haskellian/classes/applicative.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      413 2024-04-21 10:23:57.000000 haskellian-0.3.8/src/haskellian/classes/functor.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      832 2024-04-21 14:05:41.000000 haskellian-0.3.8/src/haskellian/classes/monad.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       21 2024-04-21 15:09:01.000000 haskellian-0.3.8/src/haskellian/config.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 05:10:25.479484 haskellian-0.3.8/src/haskellian/either/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 10:31:26.000000 haskellian-0.3.8/src/haskellian/either/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      405 2024-04-21 10:39:57.000000 haskellian-0.3.8/src/haskellian/either/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2644 2024-04-21 14:05:41.000000 haskellian-0.3.8/src/haskellian/either/either.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1285 2024-04-21 10:38:12.000000 haskellian-0.3.8/src/haskellian/either/funcs.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      381 2024-04-21 10:36:36.000000 haskellian-0.3.8/src/haskellian/either/narrowing.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      464 2024-04-21 10:39:34.000000 haskellian-0.3.8/src/haskellian/either/pydantic.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 05:10:25.479484 haskellian-0.3.8/src/haskellian/funcs/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-22 09:49:11.000000 haskellian-0.3.8/src/haskellian/funcs/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      167 2024-04-22 10:08:12.000000 haskellian-0.3.8/src/haskellian/funcs/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1477 2024-04-22 09:57:25.000000 haskellian-0.3.8/src/haskellian/funcs/_flow.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1512 2024-04-22 10:00:34.000000 haskellian-0.3.8/src/haskellian/funcs/_pipe.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      996 2024-04-22 10:07:57.000000 haskellian-0.3.8/src/haskellian/funcs/curried.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 05:10:25.479484 haskellian-0.3.8/src/haskellian/iter/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 13:06:20.000000 haskellian-0.3.8/src/haskellian/iter/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      697 2024-04-23 04:56:41.000000 haskellian-0.3.8/src/haskellian/iter/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1023 2024-04-23 04:56:28.000000 haskellian-0.3.8/src/haskellian/iter/basics.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      680 2024-04-21 13:53:19.000000 haskellian-0.3.8/src/haskellian/iter/batching.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      485 2024-04-21 13:53:13.000000 haskellian-0.3.8/src/haskellian/iter/indexing.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3357 2024-04-23 05:09:57.000000 haskellian-0.3.8/src/haskellian/iter/iter.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      473 2024-04-21 13:52:51.000000 haskellian-0.3.8/src/haskellian/iter/lifting.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4144 2024-04-21 13:58:56.000000 haskellian-0.3.8/src/haskellian/iter/nested.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1140 2024-04-21 13:59:18.000000 haskellian-0.3.8/src/haskellian/iter/slicing.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      869 2024-04-21 19:17:41.000000 haskellian-0.3.8/src/haskellian/iter/transposing.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1003 2024-04-21 13:59:47.000000 haskellian-0.3.8/src/haskellian/iter/zipping.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 05:10:25.479484 haskellian-0.3.8/src/haskellian/pipe/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       22 2024-04-21 10:07:57.000000 haskellian-0.3.8/src/haskellian/pipe/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      767 2024-04-21 14:05:41.000000 haskellian-0.3.8/src/haskellian/pipe/pipe.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 05:10:25.479484 haskellian-0.3.8/src/haskellian/promise/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 14:06:21.000000 haskellian-0.3.8/src/haskellian/promise/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      259 2024-04-21 17:53:58.000000 haskellian-0.3.8/src/haskellian/promise/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1173 2024-04-22 07:58:14.000000 haskellian-0.3.8/src/haskellian/promise/funcs.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      480 2024-04-21 14:17:11.000000 haskellian-0.3.8/src/haskellian/promise/lifting.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      600 2024-04-21 14:35:57.000000 haskellian-0.3.8/src/haskellian/promise/managed.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1053 2024-04-21 14:21:51.000000 haskellian-0.3.8/src/haskellian/promise/promise.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 05:10:25.479484 haskellian-0.3.8/src/haskellian/thunk/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       24 2024-04-21 10:06:39.000000 haskellian-0.3.8/src/haskellian/thunk/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      933 2024-04-21 14:05:41.000000 haskellian-0.3.8/src/haskellian/thunk/thunk.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 05:10:25.479484 haskellian-0.3.8/src/haskellian.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1539 2024-04-23 05:10:25.000000 haskellian-0.3.8/src/haskellian.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1755 2024-04-23 05:10:25.000000 haskellian-0.3.8/src/haskellian.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-23 05:10:25.000000 haskellian-0.3.8/src/haskellian.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       33 2024-04-23 05:10:25.000000 haskellian-0.3.8/src/haskellian.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-23 05:10:25.000000 haskellian-0.3.8/src/haskellian.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:09:34.164238 haskellian-0.3.9/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1539 2024-04-25 06:09:34.164238 haskellian-0.3.9/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1154 2024-04-23 05:10:28.000000 haskellian-0.3.9/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      514 2024-04-25 06:09:31.000000 haskellian-0.3.9/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-25 06:09:34.164238 haskellian-0.3.9/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:09:34.144238 haskellian-0.3.9/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:09:34.144238 haskellian-0.3.9/src/haskellian/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      156 2024-04-21 08:31:50.000000 haskellian-0.3.9/src/haskellian/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      494 2024-04-22 10:03:32.000000 haskellian-0.3.9/src/haskellian/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:09:34.154238 haskellian-0.3.9/src/haskellian/asyn_iter/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 14:25:49.000000 haskellian-0.3.9/src/haskellian/asyn_iter/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      455 2024-04-23 05:08:08.000000 haskellian-0.3.9/src/haskellian/asyn_iter/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2319 2024-04-23 05:07:58.000000 haskellian-0.3.9/src/haskellian/asyn_iter/funcs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2514 2024-04-23 06:44:54.000000 haskellian-0.3.9/src/haskellian/asyn_iter/iter.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      490 2024-04-21 14:38:54.000000 haskellian-0.3.9/src/haskellian/asyn_iter/lifting.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      886 2024-04-21 14:38:19.000000 haskellian-0.3.9/src/haskellian/asyn_iter/managed.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      650 2024-04-21 14:40:28.000000 haskellian-0.3.9/src/haskellian/asyn_iter/prefetching.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:09:34.154238 haskellian-0.3.9/src/haskellian/classes/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 09:04:50.000000 haskellian-0.3.9/src/haskellian/classes/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      137 2024-04-21 09:04:51.000000 haskellian-0.3.9/src/haskellian/classes/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      578 2024-04-21 10:23:51.000000 haskellian-0.3.9/src/haskellian/classes/applicative.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      413 2024-04-21 10:23:57.000000 haskellian-0.3.9/src/haskellian/classes/functor.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      832 2024-04-21 14:05:41.000000 haskellian-0.3.9/src/haskellian/classes/monad.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       21 2024-04-21 15:09:01.000000 haskellian-0.3.9/src/haskellian/config.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:09:34.154238 haskellian-0.3.9/src/haskellian/either/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 10:31:26.000000 haskellian-0.3.9/src/haskellian/either/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      405 2024-04-21 10:39:57.000000 haskellian-0.3.9/src/haskellian/either/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2644 2024-04-21 14:05:41.000000 haskellian-0.3.9/src/haskellian/either/either.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1285 2024-04-21 10:38:12.000000 haskellian-0.3.9/src/haskellian/either/funcs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      381 2024-04-21 10:36:36.000000 haskellian-0.3.9/src/haskellian/either/narrowing.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      464 2024-04-21 10:39:34.000000 haskellian-0.3.9/src/haskellian/either/pydantic.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:09:34.154238 haskellian-0.3.9/src/haskellian/funcs/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-22 09:49:11.000000 haskellian-0.3.9/src/haskellian/funcs/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       76 2024-04-23 07:36:11.000000 haskellian-0.3.9/src/haskellian/funcs/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1477 2024-04-22 09:57:25.000000 haskellian-0.3.9/src/haskellian/funcs/_flow.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1512 2024-04-22 10:00:34.000000 haskellian-0.3.9/src/haskellian/funcs/_pipe.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:09:34.154238 haskellian-0.3.9/src/haskellian/iter/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 13:06:20.000000 haskellian-0.3.9/src/haskellian/iter/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      792 2024-04-23 07:36:19.000000 haskellian-0.3.9/src/haskellian/iter/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1023 2024-04-23 04:56:28.000000 haskellian-0.3.9/src/haskellian/iter/basics.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      680 2024-04-21 13:53:19.000000 haskellian-0.3.9/src/haskellian/iter/batching.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      996 2024-04-23 07:35:56.000000 haskellian-0.3.9/src/haskellian/iter/curried.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      485 2024-04-21 13:53:13.000000 haskellian-0.3.9/src/haskellian/iter/indexing.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3705 2024-04-23 08:13:56.000000 haskellian-0.3.9/src/haskellian/iter/iter.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      473 2024-04-21 13:52:51.000000 haskellian-0.3.9/src/haskellian/iter/lifting.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4144 2024-04-21 13:58:56.000000 haskellian-0.3.9/src/haskellian/iter/nested.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1140 2024-04-21 13:59:18.000000 haskellian-0.3.9/src/haskellian/iter/slicing.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      869 2024-04-21 19:17:41.000000 haskellian-0.3.9/src/haskellian/iter/transposing.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1003 2024-04-21 13:59:47.000000 haskellian-0.3.9/src/haskellian/iter/zipping.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:09:34.154238 haskellian-0.3.9/src/haskellian/kwargs/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      130 2024-04-23 05:32:43.000000 haskellian-0.3.9/src/haskellian/kwargs/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       46 2024-04-23 05:33:07.000000 haskellian-0.3.9/src/haskellian/kwargs/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      637 2024-04-23 05:42:38.000000 haskellian-0.3.9/src/haskellian/kwargs/kwargs.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:09:34.154238 haskellian-0.3.9/src/haskellian/pipe/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       22 2024-04-21 10:07:57.000000 haskellian-0.3.9/src/haskellian/pipe/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      767 2024-04-21 14:05:41.000000 haskellian-0.3.9/src/haskellian/pipe/pipe.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:09:34.164238 haskellian-0.3.9/src/haskellian/promise/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 14:06:21.000000 haskellian-0.3.9/src/haskellian/promise/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      259 2024-04-21 17:53:58.000000 haskellian-0.3.9/src/haskellian/promise/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1173 2024-04-22 07:58:14.000000 haskellian-0.3.9/src/haskellian/promise/funcs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      480 2024-04-21 14:17:11.000000 haskellian-0.3.9/src/haskellian/promise/lifting.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      600 2024-04-21 14:35:57.000000 haskellian-0.3.9/src/haskellian/promise/managed.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1053 2024-04-21 14:21:51.000000 haskellian-0.3.9/src/haskellian/promise/promise.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:09:34.164238 haskellian-0.3.9/src/haskellian/thunk/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       24 2024-04-21 10:06:39.000000 haskellian-0.3.9/src/haskellian/thunk/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      933 2024-04-21 14:05:41.000000 haskellian-0.3.9/src/haskellian/thunk/thunk.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 06:09:34.164238 haskellian-0.3.9/src/haskellian.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1539 2024-04-25 06:09:34.000000 haskellian-0.3.9/src/haskellian.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1855 2024-04-25 06:09:34.000000 haskellian-0.3.9/src/haskellian.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-25 06:09:34.000000 haskellian-0.3.9/src/haskellian.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       33 2024-04-25 06:09:34.000000 haskellian-0.3.9/src/haskellian.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-25 06:09:34.000000 haskellian-0.3.9/src/haskellian.egg-info/top_level.txt
```

### Comparing `haskellian-0.3.8/PKG-INFO` & `haskellian-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haskellian
-Version: 0.3.8
+Version: 0.3.9
 Summary: The functional programming library you need
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/haskellian.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: lazy-loader
 Provides-Extra: pydantic
```

### Comparing `haskellian-0.3.8/README.md` & `haskellian-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.8/pyproject.toml` & `haskellian-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "haskellian"
-version = "0.3.8"
+version = "0.3.9"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "The functional programming library you need"
 dependencies = [
   "lazy-loader"
 ]
```

### Comparing `haskellian-0.3.8/src/haskellian/asyn_iter/funcs.py` & `haskellian-0.3.9/src/haskellian/asyn_iter/funcs.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.8/src/haskellian/asyn_iter/iter.py` & `haskellian-0.3.9/src/haskellian/asyn_iter/iter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from haskellian import DEBUG_IMPORTS, asyn_iter as AI, Monad
+from haskellian import DEBUG_IMPORTS, asyn_iter as AI, Monad, Pipe
 if DEBUG_IMPORTS:
   print('Import:', __name__)
 from typing import Callable, Generic, TypeVar, Awaitable, AsyncIterator, AsyncIterable, TypeGuard, overload, TypeVarTuple
 
 A = TypeVar('A', covariant=True)
 B = TypeVar('B')
 As = TypeVarTuple('As')
@@ -69,8 +69,17 @@
     return AI.enumerate(self)
   
   async def split(self, n: int) -> tuple[list[A], 'AsyncIter[A]']:
     head, xs = await AI.split(n, self)
     return head, AsyncIter(xs)
   
   def prefetch(self, n: int) -> 'AsyncIter[A]':
-    return AI.prefetched(n, self)
+    return AI.prefetched(n, self) if n > 0 else self
+
+
+  def i(self, f: Callable[['AsyncIter[A]'], AsyncIterable[B]]) -> 'AsyncIter[B]':
+    """Apply an arbitrary iterable function"""
+    return AsyncIter(f(self))
+  
+  def f(self, f: Callable[['AsyncIter[A]'], B]) -> Pipe[B]:
+    """Apply an arbitrary function into a `Pipe`"""
+    return Pipe(f(self))
```

### Comparing `haskellian-0.3.8/src/haskellian/asyn_iter/managed.py` & `haskellian-0.3.9/src/haskellian/asyn_iter/managed.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.8/src/haskellian/asyn_iter/prefetching.py` & `haskellian-0.3.9/src/haskellian/asyn_iter/prefetching.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.8/src/haskellian/classes/applicative.py` & `haskellian-0.3.9/src/haskellian/classes/applicative.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.8/src/haskellian/classes/monad.py` & `haskellian-0.3.9/src/haskellian/classes/monad.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.8/src/haskellian/either/either.py` & `haskellian-0.3.9/src/haskellian/either/either.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.8/src/haskellian/either/funcs.py` & `haskellian-0.3.9/src/haskellian/either/funcs.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.8/src/haskellian/funcs/_flow.py` & `haskellian-0.3.9/src/haskellian/funcs/_flow.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.8/src/haskellian/funcs/_pipe.py` & `haskellian-0.3.9/src/haskellian/funcs/_pipe.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.8/src/haskellian/funcs/curried.py` & `haskellian-0.3.9/src/haskellian/iter/curried.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.8/src/haskellian/iter/__init__.pyi` & `haskellian-0.3.9/src/haskellian/iter/__init__.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 from .basics import isiterable, flatmap, flatten, range
 from .zipping import unzip, uncons, pairwise
 from .slicing import fst, snd, head, tail, last, skip, take, take_while
 from .indexing import at, pick
 from .batching import batch, split
 from .nested import ndmap, ndrange, ndenumerate, ndflat
 from .transposing import transpose, transpose_ragged
+from .curried import map, filter, max, min, sorted
 from .iter import Iter
 
 __all__ = [
   'isiterable', 'flatmap', 'flatten', 'range',
   'unzip', 'uncons', 'pairwise',
   'fst', 'snd', 'head', 'tail', 'last', 'skip', 'take', 'take_while',
   'at', 'pick',
   'batch', 'split',
   'ndmap', 'ndrange', 'ndenumerate', 'ndflat',
   'transpose', 'transpose_ragged',
-  'Iter', 'lift'
+  'map', 'filter', 'max', 'min', 'sorted',
+  'Iter', 'lift',
 ]
```

### Comparing `haskellian-0.3.8/src/haskellian/iter/basics.py` & `haskellian-0.3.9/src/haskellian/iter/basics.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.8/src/haskellian/iter/batching.py` & `haskellian-0.3.9/src/haskellian/iter/batching.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.8/src/haskellian/iter/iter.py` & `haskellian-0.3.9/src/haskellian/iter/iter.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,15 +33,16 @@
   @classmethod
   def of(cls, value: B) -> 'Iter[B]':
     return Iter([value])
   
   def bind(self, f: Callable[[A], Iterable[B]]) -> 'Iter[B]':
     return I.flatmap(f, self)
   
-  def flatmap(self, f: Callable[[A], Iterable[B]]) -> 'Iter[B]':
+  def flatmap(self, f: Callable[[A], Iterable[B]] = lambda x: x) -> 'Iter[B]': # type: ignore
+    """Acts like `flatten` by default (`f` defaults to the identity)"""
     return self.bind(f)
   
   def iflatmap(self, f: Callable[[int, A], Iterable[B]]) -> 'Iter[B]':
     """`flatmap` with indices"""
     return self.enumerate().flatmap(lambda xs: f(*xs))
   
   def map(self, f: Callable[[A], B]) -> 'Iter[B]':
@@ -92,25 +93,32 @@
   def pairwise(self) -> 'Iter[tuple[A, A]]':
     return I.pairwise(self)
   
   def enumerate(self) -> 'Iter[tuple[int, A]]':
     return Iter(enumerate(self))
   
   def sort(self, key: Callable[[A], Any] | None = None, reverse: bool = False) -> 'Iter[A]':
+    """Like `sorted`, but returns an `Iter`"""
     return Iter(sorted(self, key=key, reverse=reverse)) # type: ignore
   
+  def sorted(self, key: Callable[[A], Any] | None = None, reverse: bool = False) -> list[A]:
+    return sorted(self, key=key, reverse=reverse)
+  
   def min(self, key: Callable[[A], Any] | None = None) -> A | None:
     return min(self, key=key, default=None) # type: ignore
   
   def max(self, key: Callable[[A], Any] | None = None) -> A | None:
     return max(self, key=key, default=None) # type: ignore
   
   def sync(self) -> list[A]:
     return list(self.xs)
   
+  def len(self) -> int:
+    return len(list(self))
+  
   def i(self, f: Callable[['Iter[A]'], Iterable[B]]) -> 'Iter[B]':
     """Apply an arbitrary iterable function"""
     return Iter(f(self))
   
   def f(self, f: Callable[['Iter[A]'], B]) -> Pipe[B]:
     """Apply an arbitrary function into a `Pipe`"""
     return Pipe(f(self))
```

### Comparing `haskellian-0.3.8/src/haskellian/iter/nested.py` & `haskellian-0.3.9/src/haskellian/iter/nested.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.8/src/haskellian/iter/slicing.py` & `haskellian-0.3.9/src/haskellian/iter/slicing.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.8/src/haskellian/iter/transposing.py` & `haskellian-0.3.9/src/haskellian/iter/transposing.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.8/src/haskellian/iter/zipping.py` & `haskellian-0.3.9/src/haskellian/iter/zipping.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.8/src/haskellian/pipe/pipe.py` & `haskellian-0.3.9/src/haskellian/pipe/pipe.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.8/src/haskellian/promise/funcs.py` & `haskellian-0.3.9/src/haskellian/promise/funcs.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.8/src/haskellian/promise/managed.py` & `haskellian-0.3.9/src/haskellian/promise/managed.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.8/src/haskellian/promise/promise.py` & `haskellian-0.3.9/src/haskellian/promise/promise.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.8/src/haskellian/thunk/thunk.py` & `haskellian-0.3.9/src/haskellian/thunk/thunk.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.8/src/haskellian.egg-info/PKG-INFO` & `haskellian-0.3.9/src/haskellian.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haskellian
-Version: 0.3.8
+Version: 0.3.9
 Summary: The functional programming library you need
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/haskellian.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: lazy-loader
 Provides-Extra: pydantic
```

### Comparing `haskellian-0.3.8/src/haskellian.egg-info/SOURCES.txt` & `haskellian-0.3.9/src/haskellian.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -26,26 +26,29 @@
 src/haskellian/either/funcs.py
 src/haskellian/either/narrowing.py
 src/haskellian/either/pydantic.py
 src/haskellian/funcs/__init__.py
 src/haskellian/funcs/__init__.pyi
 src/haskellian/funcs/_flow.py
 src/haskellian/funcs/_pipe.py
-src/haskellian/funcs/curried.py
 src/haskellian/iter/__init__.py
 src/haskellian/iter/__init__.pyi
 src/haskellian/iter/basics.py
 src/haskellian/iter/batching.py
+src/haskellian/iter/curried.py
 src/haskellian/iter/indexing.py
 src/haskellian/iter/iter.py
 src/haskellian/iter/lifting.py
 src/haskellian/iter/nested.py
 src/haskellian/iter/slicing.py
 src/haskellian/iter/transposing.py
 src/haskellian/iter/zipping.py
+src/haskellian/kwargs/__init__.py
+src/haskellian/kwargs/__init__.pyi
+src/haskellian/kwargs/kwargs.py
 src/haskellian/pipe/__init__.py
 src/haskellian/pipe/pipe.py
 src/haskellian/promise/__init__.py
 src/haskellian/promise/__init__.pyi
 src/haskellian/promise/funcs.py
 src/haskellian/promise/lifting.py
 src/haskellian/promise/managed.py
```

