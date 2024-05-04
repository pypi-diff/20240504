# Comparing `tmp/rbfly-0.8.2.tar.gz` & `tmp/rbfly-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rbfly-0.8.2.tar", last modified: Tue Mar 19 20:51:50 2024, max compression
+gzip compressed data, was "rbfly-0.8.3.tar", last modified: Sat May  4 07:35:24 2024, max compression
```

## Comparing `rbfly-0.8.2.tar` & `rbfly-0.8.3.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-03-19 20:51:50.368421 rbfly-0.8.2/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    35147 2024-01-07 12:33:04.000000 rbfly-0.8.2/COPYING
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2594 2024-03-19 20:51:50.368421 rbfly-0.8.2/PKG-INFO
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1098 2024-01-07 12:33:04.000000 rbfly-0.8.2/README
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      588 2024-03-06 12:35:21.000000 rbfly-0.8.2/pyproject.toml
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-03-19 20:51:50.348421 rbfly-0.8.2/rbfly/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      922 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/__init__.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)   193841 2024-03-19 12:14:17.000000 rbfly-0.8.2/rbfly/_buffer.c
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1434 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/_buffer.pxd
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1898 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/_buffer.pyx
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)   184979 2024-03-19 12:14:17.000000 rbfly-0.8.2/rbfly/_codec.c
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1098 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/_codec.h
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1197 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/_codec.pxd
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2298 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/_codec.pyx
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-03-19 20:51:50.351754 rbfly-0.8.2/rbfly/amqp/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      956 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/amqp/__init__.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)   740829 2024-03-19 12:14:18.000000 rbfly-0.8.2/rbfly/amqp/_message.c
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1629 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/amqp/_message.pxd
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1560 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/amqp/_message.pyi
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    20670 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/amqp/_message.pyx
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     4250 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/cm.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1335 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/error.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)        0 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/py.typed
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3295 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/slotmap.py
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-03-19 20:51:50.358421 rbfly-0.8.2/rbfly/streams/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1649 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/streams/__init__.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)  1425384 2024-03-19 12:14:17.000000 rbfly-0.8.2/rbfly/streams/_client.c
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2248 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/streams/_client.pyi
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    19574 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/streams/_client.pyx
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)   737342 2024-03-19 12:14:19.000000 rbfly-0.8.2/rbfly/streams/_codec.c
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1555 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/streams/_codec.pyi
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    12519 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/streams/_codec.pyx
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)   515241 2024-03-19 12:14:19.000000 rbfly-0.8.2/rbfly/streams/_mqueue.c
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1065 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/streams/_mqueue.pxd
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1244 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/streams/_mqueue.pyi
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3893 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/streams/_mqueue.pyx
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    20127 2024-03-19 11:53:19.000000 rbfly-0.8.2/rbfly/streams/client.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     8770 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/streams/codec.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1894 2024-01-08 11:28:18.000000 rbfly-0.8.2/rbfly/streams/const.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1287 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/streams/error.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     5197 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/streams/offset.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    27513 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/streams/protocol.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2363 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/streams/types.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     4027 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/streams/util.py
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-03-19 20:51:50.358421 rbfly-0.8.2/rbfly/tests/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      790 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/tests/__init__.py
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-03-19 20:51:50.358421 rbfly-0.8.2/rbfly/tests/amqp/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      790 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/tests/amqp/__init__.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    10497 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/tests/amqp/test_message.py
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-03-19 20:51:50.361754 rbfly-0.8.2/rbfly/tests/streams/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      790 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/tests/streams/__init__.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    18605 2024-03-19 11:44:13.000000 rbfly-0.8.2/rbfly/tests/streams/test_client.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    16771 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/tests/streams/test_codec.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2267 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/tests/streams/test_mqueue.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1329 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/tests/streams/test_offset.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3393 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/tests/test_slotmap.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3228 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/tests/test_util.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2306 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/types.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2008 2024-01-07 12:33:04.000000 rbfly-0.8.2/rbfly/util.py
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-03-19 20:51:50.361754 rbfly-0.8.2/rbfly.egg-info/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2594 2024-03-19 20:51:50.000000 rbfly-0.8.2/rbfly.egg-info/PKG-INFO
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1306 2024-03-19 20:51:50.000000 rbfly-0.8.2/rbfly.egg-info/SOURCES.txt
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)        1 2024-03-19 20:51:50.000000 rbfly-0.8.2/rbfly.egg-info/dependency_links.txt
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      234 2024-03-19 20:51:50.000000 rbfly-0.8.2/rbfly.egg-info/requires.txt
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)        6 2024-03-19 20:51:50.000000 rbfly-0.8.2/rbfly.egg-info/top_level.txt
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1196 2024-03-19 20:51:50.368421 rbfly-0.8.2/setup.cfg
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1680 2024-01-07 12:33:04.000000 rbfly-0.8.2/setup.py
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-05-04 07:35:24.951259 rbfly-0.8.3/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    35147 2024-01-07 12:33:04.000000 rbfly-0.8.3/COPYING
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2663 2024-05-04 07:35:24.951259 rbfly-0.8.3/PKG-INFO
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1098 2024-01-07 12:33:04.000000 rbfly-0.8.3/README
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      589 2024-04-14 21:14:44.000000 rbfly-0.8.3/pyproject.toml
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-05-04 07:35:24.927926 rbfly-0.8.3/rbfly/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      922 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/__init__.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)   194660 2024-05-04 07:19:20.000000 rbfly-0.8.3/rbfly/_buffer.c
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1434 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/_buffer.pxd
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1898 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/_buffer.pyx
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)   185798 2024-05-04 07:19:20.000000 rbfly-0.8.3/rbfly/_codec.c
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1098 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/_codec.h
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1197 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/_codec.pxd
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2298 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/_codec.pyx
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-05-04 07:35:24.931259 rbfly-0.8.3/rbfly/amqp/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      956 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/amqp/__init__.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)   742026 2024-05-04 07:35:05.000000 rbfly-0.8.3/rbfly/amqp/_message.c
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1629 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/amqp/_message.pxd
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1560 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/amqp/_message.pyi
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    20670 2024-05-04 07:34:58.000000 rbfly-0.8.3/rbfly/amqp/_message.pyx
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     4250 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/cm.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1335 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/error.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)        0 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/py.typed
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3295 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/slotmap.py
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-05-04 07:35:24.934592 rbfly-0.8.3/rbfly/streams/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1649 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/streams/__init__.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)  1426495 2024-05-04 07:19:21.000000 rbfly-0.8.3/rbfly/streams/_client.c
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2248 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/streams/_client.pyi
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    19574 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/streams/_client.pyx
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)   738316 2024-05-04 07:19:21.000000 rbfly-0.8.3/rbfly/streams/_codec.c
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1555 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/streams/_codec.pyi
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    12519 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/streams/_codec.pyx
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)   516078 2024-05-04 07:19:21.000000 rbfly-0.8.3/rbfly/streams/_mqueue.c
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1065 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/streams/_mqueue.pxd
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1244 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/streams/_mqueue.pyi
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3893 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/streams/_mqueue.pyx
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    20151 2024-05-04 00:04:20.000000 rbfly-0.8.3/rbfly/streams/client.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     8770 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/streams/codec.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1894 2024-01-08 11:28:18.000000 rbfly-0.8.3/rbfly/streams/const.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1287 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/streams/error.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     5197 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/streams/offset.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    27513 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/streams/protocol.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2363 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/streams/types.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     4027 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/streams/util.py
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-05-04 07:35:24.934592 rbfly-0.8.3/rbfly/tests/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      790 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/tests/__init__.py
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-05-04 07:35:24.934592 rbfly-0.8.3/rbfly/tests/amqp/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      790 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/tests/amqp/__init__.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    10497 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/tests/amqp/test_message.py
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-05-04 07:35:24.934592 rbfly-0.8.3/rbfly/tests/streams/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      790 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/tests/streams/__init__.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    18746 2024-05-04 00:04:37.000000 rbfly-0.8.3/rbfly/tests/streams/test_client.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    16771 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/tests/streams/test_codec.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2267 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/tests/streams/test_mqueue.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1329 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/tests/streams/test_offset.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3393 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/tests/test_slotmap.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3228 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/tests/test_util.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2306 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/types.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2008 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/util.py
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-05-04 07:35:24.934592 rbfly-0.8.3/rbfly.egg-info/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2663 2024-05-04 07:35:24.000000 rbfly-0.8.3/rbfly.egg-info/PKG-INFO
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1306 2024-05-04 07:35:24.000000 rbfly-0.8.3/rbfly.egg-info/SOURCES.txt
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)        1 2024-05-04 07:35:24.000000 rbfly-0.8.3/rbfly.egg-info/dependency_links.txt
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      259 2024-05-04 07:35:24.000000 rbfly-0.8.3/rbfly.egg-info/requires.txt
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)        6 2024-05-04 07:35:24.000000 rbfly-0.8.3/rbfly.egg-info/top_level.txt
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1222 2024-05-04 07:35:24.954592 rbfly-0.8.3/setup.cfg
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1680 2024-01-07 12:33:04.000000 rbfly-0.8.3/setup.py
```

### Comparing `rbfly-0.8.2/COPYING` & `rbfly-0.8.3/COPYING`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/PKG-INFO` & `rbfly-0.8.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbfly
-Version: 0.8.2
+Version: 0.8.3
 Summary: RbFly - a library for RabbitMQ Streams using Python asyncio
 Home-page: https://wrobell.dcmod.org/rbfly/
 Author: Artur Wroblewski
 Author-email: wrobell@riseup.net
 License: GPLv3+
 Project-URL: Source Code, https://gitlab.com/wrobell/rbfly
 Project-URL: Bug tracker, https://gitlab.com/wrobell/rbfly/issues
@@ -14,29 +14,31 @@
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: COPYING
 Provides-Extra: tests
 Requires-Dist: bandit; extra == "tests"
 Requires-Dist: cython-lint; extra == "tests"
-Requires-Dist: mypy==1.9.0; extra == "tests"
+Requires-Dist: mypy==1.10.0; extra == "tests"
 Requires-Dist: pika; extra == "tests"
 Requires-Dist: pytest-asyncio; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: pytest-lazy-fixtures; extra == "tests"
 Requires-Dist: pytest-timeout; extra == "tests"
 Requires-Dist: ruff>=0.3.0; extra == "tests"
 Requires-Dist: toml; extra == "tests"
 Requires-Dist: uvloop>=0.19.0; extra == "tests"
 Provides-Extra: performance
 Requires-Dist: msgpack; extra == "performance"
 Requires-Dist: aiokafka==0.8.1; extra == "performance"
 Requires-Dist: rstream==0.13.0; extra == "performance"
 Requires-Dist: uamqp==1.6.5; extra == "performance"
 Requires-Dist: python-qpid-proton==0.39.0; extra == "performance"
+Provides-Extra: doc
+Requires-Dist: sphinx_rtd_theme; extra == "doc"
 
 RbFly is a library for RabbitMQ Streams using Python asyncio
 
 - https://www.rabbitmq.com/streams.html
 - https://docs.python.org/3/library/asyncio.html
 
 The library is designed and implemented with the following qualities in
```

### Comparing `rbfly-0.8.2/README` & `rbfly-0.8.3/README`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/pyproject.toml` & `rbfly-0.8.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = [
     "build",
     "setuptools",
     "wheel",
-    "cython==3.0.9",
+    "cython==3.0.10",
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.mypy]
 strict = true
 
 [tool.bandit]
```

### Comparing `rbfly-0.8.2/rbfly/__init__.py` & `rbfly-0.8.3/rbfly/__init__.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/_buffer.c` & `rbfly-0.8.3/rbfly/_buffer.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "rbfly._buffer",
         "sources": [
@@ -33,18 +33,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -128,14 +128,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -189,14 +191,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -250,60 +254,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -386,14 +413,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
```

### Comparing `rbfly-0.8.2/rbfly/_buffer.pxd` & `rbfly-0.8.3/rbfly/_buffer.pxd`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/_buffer.pyx` & `rbfly-0.8.3/rbfly/_buffer.pyx`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/_codec.c` & `rbfly-0.8.3/rbfly/_codec.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "rbfly/_codec.h"
         ],
@@ -38,18 +38,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -133,14 +133,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -194,14 +196,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -255,60 +259,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -391,14 +418,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
```

### Comparing `rbfly-0.8.2/rbfly/_codec.h` & `rbfly-0.8.3/rbfly/_codec.h`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/_codec.pxd` & `rbfly-0.8.3/rbfly/_codec.pxd`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/_codec.pyx` & `rbfly-0.8.3/rbfly/_codec.pyx`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/amqp/__init__.py` & `rbfly-0.8.3/rbfly/amqp/__init__.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/amqp/_message.c` & `rbfly-0.8.3/rbfly/amqp/_message.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "rbfly.amqp._message",
         "sources": [
@@ -50,18 +50,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -145,14 +145,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -206,14 +208,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -267,60 +271,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -403,14 +430,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -1470,19 +1500,19 @@
 static const char *__pyx_filename;
 
 /* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
   "<stringsource>",
   "rbfly/amqp/_message.pyx",
-  "contextvars.pxd",
+  ".venv-3.12.3/lib/python3.12/site-packages/Cython/Includes/cpython/contextvars.pxd",
   "rbfly/amqp/_message.pxd",
-  "type.pxd",
-  "bool.pxd",
-  "complex.pxd",
+  ".venv-3.12.3/lib/python3.12/site-packages/Cython/Includes/cpython/type.pxd",
+  ".venv-3.12.3/lib/python3.12/site-packages/Cython/Includes/cpython/bool.pxd",
+  ".venv-3.12.3/lib/python3.12/site-packages/Cython/Includes/cpython/complex.pxd",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
@@ -2048,30 +2078,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_9
-#define __PYX_HAVE_RT_ImportType_proto_3_0_9
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_9 {
-   __Pyx_ImportType_CheckSize_Error_3_0_9 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_9 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_9 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportDottedModule.proto */
 static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
@@ -2345,15 +2375,15 @@
 static unsigned long __Pyx_get_runtime_version(void);
 static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer);
 
 /* FunctionExport.proto */
 static int __Pyx_ExportFunction(const char *name, void (*f)(void), const char *sig);
 
 /* FunctionImport.proto */
-static int __Pyx_ImportFunction_3_0_9(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
+static int __Pyx_ImportFunction_3_0_10(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 /* #### Code section: module_declarations ### */
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4real_real(PyComplexObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4imag_imag(PyComplexObject *__pyx_v_self); /* proto*/
@@ -3429,70 +3459,70 @@
 #define __pyx_codeobj__17 __pyx_mstate_global->__pyx_codeobj__17
 #define __pyx_codeobj__18 __pyx_mstate_global->__pyx_codeobj__18
 /* #### Code section: module_code ### */
 
 /* "cpython/complex.pxd":19
  * 
  *         @property
- *         cdef inline double real(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double real(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.real
  * 
  */
 
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4real_real(PyComplexObject *__pyx_v_self) {
   double __pyx_r;
 
   /* "cpython/complex.pxd":20
  *         @property
- *         cdef inline double real(self):
+ *         cdef inline double real(self) noexcept:
  *             return self.cval.real             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = __pyx_v_self->cval.real;
   goto __pyx_L0;
 
   /* "cpython/complex.pxd":19
  * 
  *         @property
- *         cdef inline double real(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double real(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.real
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
 /* "cpython/complex.pxd":23
  * 
  *         @property
- *         cdef inline double imag(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double imag(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.imag
  * 
  */
 
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4imag_imag(PyComplexObject *__pyx_v_self) {
   double __pyx_r;
 
   /* "cpython/complex.pxd":24
  *         @property
- *         cdef inline double imag(self):
+ *         cdef inline double imag(self) noexcept:
  *             return self.cval.imag             # <<<<<<<<<<<<<<
  * 
  *     # PyTypeObject PyComplex_Type
  */
   __pyx_r = __pyx_v_self->cval.imag;
   goto __pyx_L0;
 
   /* "cpython/complex.pxd":23
  * 
  *         @property
- *         cdef inline double imag(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double imag(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.imag
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
@@ -10138,25 +10168,27 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *__pyx_freelist_5rbfly_4amqp_8_message_MessageCtx[1000];
 static int __pyx_freecount_5rbfly_4amqp_8_message_MessageCtx = 0;
+#endif
 
 static PyObject *__pyx_tp_new_5rbfly_4amqp_8_message_MessageCtx(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *p;
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_5rbfly_4amqp_8_message_MessageCtx > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx)))) {
     o = (PyObject*)__pyx_freelist_5rbfly_4amqp_8_message_MessageCtx[--__pyx_freecount_5rbfly_4amqp_8_message_MessageCtx];
     memset(o, 0, sizeof(struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -10178,15 +10210,15 @@
 
 static void __pyx_tp_dealloc_5rbfly_4amqp_8_message_MessageCtx(PyObject *o) {
   struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *p = (struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *)o;
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->body);
   Py_CLEAR(p->annotations);
   Py_CLEAR(p->app_properties);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_5rbfly_4amqp_8_message_MessageCtx < 1000) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx)))) {
     __pyx_freelist_5rbfly_4amqp_8_message_MessageCtx[__pyx_freecount_5rbfly_4amqp_8_message_MessageCtx++] = ((struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -10787,31 +10819,31 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_9(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_9(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_9(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -10831,28 +10863,28 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __pyx_t_1 = PyImport_ImportModule("rbfly._buffer"); if (!__pyx_t_1) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction_3_0_9(__pyx_t_1, "buffer_claim", (void (**)(void))&__pyx_f_5rbfly_7_buffer_buffer_claim, "char *(struct __pyx_t_5rbfly_7_buffer_Buffer *, Py_ssize_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction_3_0_9(__pyx_t_1, "buffer_get_uint8", (void (**)(void))&__pyx_f_5rbfly_7_buffer_buffer_get_uint8, "uint8_t (struct __pyx_t_5rbfly_7_buffer_Buffer *)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction_3_0_9(__pyx_t_1, "buffer_check_size", (void (**)(void))&__pyx_f_5rbfly_7_buffer_buffer_check_size, "char (struct __pyx_t_5rbfly_7_buffer_Buffer *, uint32_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_3_0_10(__pyx_t_1, "buffer_claim", (void (**)(void))&__pyx_f_5rbfly_7_buffer_buffer_claim, "char *(struct __pyx_t_5rbfly_7_buffer_Buffer *, Py_ssize_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_3_0_10(__pyx_t_1, "buffer_get_uint8", (void (**)(void))&__pyx_f_5rbfly_7_buffer_buffer_get_uint8, "uint8_t (struct __pyx_t_5rbfly_7_buffer_Buffer *)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_3_0_10(__pyx_t_1, "buffer_check_size", (void (**)(void))&__pyx_f_5rbfly_7_buffer_buffer_check_size, "char (struct __pyx_t_5rbfly_7_buffer_Buffer *, uint32_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("rbfly._codec"); if (!__pyx_t_1) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction_3_0_9(__pyx_t_1, "unpack_uint16", (void (**)(void))&__pyx_f_5rbfly_6_codec_unpack_uint16, "uint16_t (char const *)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction_3_0_9(__pyx_t_1, "unpack_uint32", (void (**)(void))&__pyx_f_5rbfly_6_codec_unpack_uint32, "uint32_t (char const *)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction_3_0_9(__pyx_t_1, "unpack_uint64", (void (**)(void))&__pyx_f_5rbfly_6_codec_unpack_uint64, "uint64_t (char const *)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction_3_0_9(__pyx_t_1, "unpack_float", (void (**)(void))&__pyx_f_5rbfly_6_codec_unpack_float, "float (char const *)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction_3_0_9(__pyx_t_1, "unpack_double", (void (**)(void))&__pyx_f_5rbfly_6_codec_unpack_double, "double (char const *)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction_3_0_9(__pyx_t_1, "pack_uint32", (void (**)(void))&__pyx_f_5rbfly_6_codec_pack_uint32, "void (char *, uint32_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction_3_0_9(__pyx_t_1, "pack_uint64", (void (**)(void))&__pyx_f_5rbfly_6_codec_pack_uint64, "void (char *, uint64_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction_3_0_9(__pyx_t_1, "pack_double", (void (**)(void))&__pyx_f_5rbfly_6_codec_pack_double, "void (char *, double)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_3_0_10(__pyx_t_1, "unpack_uint16", (void (**)(void))&__pyx_f_5rbfly_6_codec_unpack_uint16, "uint16_t (char const *)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_3_0_10(__pyx_t_1, "unpack_uint32", (void (**)(void))&__pyx_f_5rbfly_6_codec_unpack_uint32, "uint32_t (char const *)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_3_0_10(__pyx_t_1, "unpack_uint64", (void (**)(void))&__pyx_f_5rbfly_6_codec_unpack_uint64, "uint64_t (char const *)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_3_0_10(__pyx_t_1, "unpack_float", (void (**)(void))&__pyx_f_5rbfly_6_codec_unpack_float, "float (char const *)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_3_0_10(__pyx_t_1, "unpack_double", (void (**)(void))&__pyx_f_5rbfly_6_codec_unpack_double, "double (char const *)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_3_0_10(__pyx_t_1, "pack_uint32", (void (**)(void))&__pyx_f_5rbfly_6_codec_pack_uint32, "void (char *, uint32_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_3_0_10(__pyx_t_1, "pack_uint64", (void (**)(void))&__pyx_f_5rbfly_6_codec_pack_uint64, "void (char *, uint64_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_3_0_10(__pyx_t_1, "pack_double", (void (**)(void))&__pyx_f_5rbfly_6_codec_pack_double, "void (char *, double)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -13709,18 +13741,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_9
-#define __PYX_HAVE_RT_ImportType_3_0_9
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -13766,23 +13798,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_9 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_9 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -17984,17 +18016,17 @@
 bad:
     Py_XDECREF(cobj);
     Py_XDECREF(d);
     return -1;
 }
 
 /* FunctionImport */
-#ifndef __PYX_HAVE_RT_ImportFunction_3_0_9
-#define __PYX_HAVE_RT_ImportFunction_3_0_9
-static int __Pyx_ImportFunction_3_0_9(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
+#ifndef __PYX_HAVE_RT_ImportFunction_3_0_10
+#define __PYX_HAVE_RT_ImportFunction_3_0_10
+static int __Pyx_ImportFunction_3_0_10(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
     PyObject *d = 0;
     PyObject *cobj = 0;
     union {
         void (*fp)(void);
         void *p;
     } tmp;
     d = PyObject_GetAttrString(module, (char *)"__pyx_capi__");
```

### Comparing `rbfly-0.8.2/rbfly/amqp/_message.pxd` & `rbfly-0.8.3/rbfly/amqp/_message.pxd`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/amqp/_message.pyi` & `rbfly-0.8.3/rbfly/amqp/_message.pyi`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/amqp/_message.pyx` & `rbfly-0.8.3/rbfly/amqp/_message.pyx`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/cm.py` & `rbfly-0.8.3/rbfly/cm.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/error.py` & `rbfly-0.8.3/rbfly/error.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/slotmap.py` & `rbfly-0.8.3/rbfly/slotmap.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/streams/__init__.py` & `rbfly-0.8.3/rbfly/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/streams/_client.c` & `rbfly-0.8.3/rbfly/streams/_client.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "rbfly.streams._client",
         "sources": [
@@ -33,18 +33,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -128,14 +128,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -189,14 +191,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -250,60 +254,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -386,14 +413,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -2913,30 +2943,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_9
-#define __PYX_HAVE_RT_ImportType_proto_3_0_9
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_9 {
-   __Pyx_ImportType_CheckSize_Error_3_0_9 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_9 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_9 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportDottedModule.proto */
 static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
@@ -18512,24 +18542,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct__close *__pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct__close[8];
 static int __pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct__close = 0;
+#endif
 
 static PyObject *__pyx_tp_new_5rbfly_7streams_7_client___pyx_scope_struct__close(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct__close > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct__close)))) {
     o = (PyObject*)__pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct__close[--__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct__close];
     memset(o, 0, sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct__close));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -18548,15 +18580,15 @@
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_5rbfly_7streams_7_client___pyx_scope_struct__close) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_self);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct__close < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct__close)))) {
     __pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct__close[__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct__close++] = ((struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct__close *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -18671,24 +18703,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_1__publish *__pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_1__publish[8];
 static int __pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_1__publish = 0;
+#endif
 
 static PyObject *__pyx_tp_new_5rbfly_7streams_7_client___pyx_scope_struct_1__publish(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_1__publish > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_1__publish)))) {
     o = (PyObject*)__pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_1__publish[--__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_1__publish];
     memset(o, 0, sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_1__publish));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -18723,15 +18757,15 @@
   Py_CLEAR(p->__pyx_t_4);
   Py_CLEAR(p->__pyx_t_5);
   Py_CLEAR(p->__pyx_t_6);
   Py_CLEAR(p->__pyx_t_7);
   Py_CLEAR(p->__pyx_t_8);
   Py_CLEAR(p->__pyx_t_9);
   Py_CLEAR(p->__pyx_t_10);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_1__publish < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_1__publish)))) {
     __pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_1__publish[__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_1__publish++] = ((struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_1__publish *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -18894,24 +18928,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_2_close *__pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_2_close[8];
 static int __pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_2_close = 0;
+#endif
 
 static PyObject *__pyx_tp_new_5rbfly_7streams_7_client___pyx_scope_struct_2_close(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_2_close > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_2_close)))) {
     o = (PyObject*)__pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_2_close[--__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_2_close];
     memset(o, 0, sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_2_close));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -18930,15 +18966,15 @@
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_5rbfly_7streams_7_client___pyx_scope_struct_2_close) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_self);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_2_close < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_2_close)))) {
     __pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_2_close[__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_2_close++] = ((struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_2_close *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -19053,24 +19089,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_3_send *__pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_3_send[8];
 static int __pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_3_send = 0;
+#endif
 
 static PyObject *__pyx_tp_new_5rbfly_7streams_7_client___pyx_scope_struct_3_send(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_3_send > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_3_send)))) {
     o = (PyObject*)__pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_3_send[--__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_3_send];
     memset(o, 0, sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_3_send));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -19091,15 +19129,15 @@
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_ctx);
   Py_CLEAR(p->__pyx_v_message);
   Py_CLEAR(p->__pyx_v_self);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_3_send < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_3_send)))) {
     __pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_3_send[__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_3_send++] = ((struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_3_send *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -19220,24 +19258,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_4_flush *__pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_4_flush[8];
 static int __pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_4_flush = 0;
+#endif
 
 static PyObject *__pyx_tp_new_5rbfly_7streams_7_client___pyx_scope_struct_4_flush(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_4_flush > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_4_flush)))) {
     o = (PyObject*)__pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_4_flush[--__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_4_flush];
     memset(o, 0, sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_4_flush));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -19256,15 +19296,15 @@
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_5rbfly_7streams_7_client___pyx_scope_struct_4_flush) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_self);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_4_flush < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_4_flush)))) {
     __pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_4_flush[__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_4_flush++] = ((struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_4_flush *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -19379,24 +19419,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_5_close *__pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_5_close[8];
 static int __pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_5_close = 0;
+#endif
 
 static PyObject *__pyx_tp_new_5rbfly_7streams_7_client___pyx_scope_struct_5_close(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_5_close > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_5_close)))) {
     o = (PyObject*)__pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_5_close[--__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_5_close];
     memset(o, 0, sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_5_close));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -19415,15 +19457,15 @@
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_5rbfly_7streams_7_client___pyx_scope_struct_5_close) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_self);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_5_close < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_5_close)))) {
     __pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_5_close[__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_5_close++] = ((struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_5_close *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -19538,24 +19580,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_6_batch *__pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_6_batch[8];
 static int __pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_6_batch = 0;
+#endif
 
 static PyObject *__pyx_tp_new_5rbfly_7streams_7_client___pyx_scope_struct_6_batch(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_6_batch > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_6_batch)))) {
     o = (PyObject*)__pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_6_batch[--__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_6_batch];
     memset(o, 0, sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_6_batch));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -19585,15 +19629,15 @@
   Py_CLEAR(p->__pyx_t_1);
   Py_CLEAR(p->__pyx_t_2);
   Py_CLEAR(p->__pyx_t_3);
   Py_CLEAR(p->__pyx_t_4);
   Py_CLEAR(p->__pyx_t_5);
   Py_CLEAR(p->__pyx_t_6);
   Py_CLEAR(p->__pyx_t_7);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_6_batch < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_6_batch)))) {
     __pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_6_batch[__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_6_batch++] = ((struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_6_batch *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -19738,24 +19782,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_7__flush *__pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_7__flush[8];
 static int __pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_7__flush = 0;
+#endif
 
 static PyObject *__pyx_tp_new_5rbfly_7streams_7_client___pyx_scope_struct_7__flush(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_7__flush > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_7__flush)))) {
     o = (PyObject*)__pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_7__flush[--__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_7__flush];
     memset(o, 0, sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_7__flush));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -19785,15 +19831,15 @@
   Py_CLEAR(p->__pyx_t_1);
   Py_CLEAR(p->__pyx_t_2);
   Py_CLEAR(p->__pyx_t_3);
   Py_CLEAR(p->__pyx_t_4);
   Py_CLEAR(p->__pyx_t_5);
   Py_CLEAR(p->__pyx_t_6);
   Py_CLEAR(p->__pyx_t_7);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_7__flush < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_7__flush)))) {
     __pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_7__flush[__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_7__flush++] = ((struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_7__flush *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -19941,24 +19987,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_8_flush *__pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_8_flush[8];
 static int __pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_8_flush = 0;
+#endif
 
 static PyObject *__pyx_tp_new_5rbfly_7streams_7_client___pyx_scope_struct_8_flush(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_8_flush > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_8_flush)))) {
     o = (PyObject*)__pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_8_flush[--__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_8_flush];
     memset(o, 0, sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_8_flush));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -19977,15 +20025,15 @@
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_5rbfly_7streams_7_client___pyx_scope_struct_8_flush) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_self);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_8_flush < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_8_flush)))) {
     __pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_8_flush[__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_8_flush++] = ((struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_8_flush *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -20100,24 +20148,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_9_close *__pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_9_close[8];
 static int __pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_9_close = 0;
+#endif
 
 static PyObject *__pyx_tp_new_5rbfly_7streams_7_client___pyx_scope_struct_9_close(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_9_close > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_9_close)))) {
     o = (PyObject*)__pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_9_close[--__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_9_close];
     memset(o, 0, sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_9_close));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -20136,15 +20186,15 @@
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_5rbfly_7streams_7_client___pyx_scope_struct_9_close) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_self);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_9_close < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_9_close)))) {
     __pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_9_close[__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_9_close++] = ((struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_9_close *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -20259,24 +20309,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_10_send *__pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_10_send[8];
 static int __pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_10_send = 0;
+#endif
 
 static PyObject *__pyx_tp_new_5rbfly_7streams_7_client___pyx_scope_struct_10_send(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_10_send > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_10_send)))) {
     o = (PyObject*)__pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_10_send[--__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_10_send];
     memset(o, 0, sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_10_send));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -20297,15 +20349,15 @@
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_ctx);
   Py_CLEAR(p->__pyx_v_message);
   Py_CLEAR(p->__pyx_v_self);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_10_send < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_10_send)))) {
     __pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_10_send[__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_10_send++] = ((struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_10_send *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -20423,24 +20475,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_11_flush *__pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_11_flush[8];
 static int __pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_11_flush = 0;
+#endif
 
 static PyObject *__pyx_tp_new_5rbfly_7streams_7_client___pyx_scope_struct_11_flush(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_11_flush > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_11_flush)))) {
     o = (PyObject*)__pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_11_flush[--__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_11_flush];
     memset(o, 0, sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_11_flush));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -20459,15 +20513,15 @@
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_5rbfly_7streams_7_client___pyx_scope_struct_11_flush) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_self);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_11_flush < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_11_flush)))) {
     __pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_11_flush[__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_11_flush++] = ((struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_11_flush *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -20582,24 +20636,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_12_close *__pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_12_close[8];
 static int __pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_12_close = 0;
+#endif
 
 static PyObject *__pyx_tp_new_5rbfly_7streams_7_client___pyx_scope_struct_12_close(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_12_close > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_12_close)))) {
     o = (PyObject*)__pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_12_close[--__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_12_close];
     memset(o, 0, sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_12_close));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -20618,15 +20674,15 @@
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_5rbfly_7streams_7_client___pyx_scope_struct_12_close) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_self);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_12_close < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_12_close)))) {
     __pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_12_close[__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_12_close++] = ((struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_12_close *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -20741,24 +20797,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_13___aiter__ *__pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_13___aiter__[8];
 static int __pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_13___aiter__ = 0;
+#endif
 
 static PyObject *__pyx_tp_new_5rbfly_7streams_7_client___pyx_scope_struct_13___aiter__(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_13___aiter__ > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_13___aiter__)))) {
     o = (PyObject*)__pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_13___aiter__[--__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_13___aiter__];
     memset(o, 0, sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_13___aiter__));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -20787,15 +20845,15 @@
   Py_CLEAR(p->__pyx_v_protocol);
   Py_CLEAR(p->__pyx_v_queue);
   Py_CLEAR(p->__pyx_v_self);
   Py_CLEAR(p->__pyx_v_task);
   Py_CLEAR(p->__pyx_t_0);
   Py_CLEAR(p->__pyx_t_1);
   Py_CLEAR(p->__pyx_t_2);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_13___aiter__ < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_13___aiter__)))) {
     __pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_13___aiter__[__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_13___aiter__++] = ((struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_13___aiter__ *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -20940,24 +20998,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_14__flush_messages *__pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_14__flush_messages[8];
 static int __pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_14__flush_messages = 0;
+#endif
 
 static PyObject *__pyx_tp_new_5rbfly_7streams_7_client___pyx_scope_struct_14__flush_messages(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_14__flush_messages > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_14__flush_messages)))) {
     o = (PyObject*)__pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_14__flush_messages[--__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_14__flush_messages];
     memset(o, 0, sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_14__flush_messages));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -20979,15 +21039,15 @@
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_amqp);
   Py_CLEAR(p->__pyx_v_data);
   Py_CLEAR(p->__pyx_v_publisher);
   Py_CLEAR(p->__pyx_v_wait_connected);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_14__flush_messages < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_14__flush_messages)))) {
     __pyx_freelist_5rbfly_7streams_7_client___pyx_scope_struct_14__flush_messages[__pyx_freecount_5rbfly_7streams_7_client___pyx_scope_struct_14__flush_messages++] = ((struct __pyx_obj_5rbfly_7streams_7_client___pyx_scope_struct_14__flush_messages *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -22469,19 +22529,19 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("rbfly.amqp._message"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5rbfly_4amqp_8_message_MessageCtx = __Pyx_ImportType_3_0_9(__pyx_t_1, "rbfly.amqp._message", "MessageCtx", sizeof(struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5rbfly_4amqp_8_message_MessageCtx) __PYX_ERR(2, 24, __pyx_L1_error)
+  __pyx_ptype_5rbfly_4amqp_8_message_MessageCtx = __Pyx_ImportType_3_0_10(__pyx_t_1, "rbfly.amqp._message", "MessageCtx", sizeof(struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5rbfly_4amqp_8_message_MessageCtx) __PYX_ERR(2, 24, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("rbfly.streams._mqueue"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5rbfly_7streams_7_mqueue_MessageQueue = __Pyx_ImportType_3_0_9(__pyx_t_1, "rbfly.streams._mqueue", "MessageQueue", sizeof(struct __pyx_obj_5rbfly_7streams_7_mqueue_MessageQueue), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_5rbfly_7streams_7_mqueue_MessageQueue),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5rbfly_7streams_7_mqueue_MessageQueue) __PYX_ERR(3, 22, __pyx_L1_error)
+  __pyx_ptype_5rbfly_7streams_7_mqueue_MessageQueue = __Pyx_ImportType_3_0_10(__pyx_t_1, "rbfly.streams._mqueue", "MessageQueue", sizeof(struct __pyx_obj_5rbfly_7streams_7_mqueue_MessageQueue), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_5rbfly_7streams_7_mqueue_MessageQueue),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5rbfly_7streams_7_mqueue_MessageQueue) __PYX_ERR(3, 22, __pyx_L1_error)
   __pyx_vtabptr_5rbfly_7streams_7_mqueue_MessageQueue = (struct __pyx_vtabstruct_5rbfly_7streams_7_mqueue_MessageQueue*)__Pyx_GetVtable(__pyx_ptype_5rbfly_7streams_7_mqueue_MessageQueue); if (unlikely(!__pyx_vtabptr_5rbfly_7streams_7_mqueue_MessageQueue)) __PYX_ERR(3, 22, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -29071,18 +29131,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_3_0_9
-#define __PYX_HAVE_RT_ImportType_3_0_9
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -29128,23 +29188,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_9 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_9 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `rbfly-0.8.2/rbfly/streams/_client.pyi` & `rbfly-0.8.3/rbfly/streams/_client.pyi`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/streams/_client.pyx` & `rbfly-0.8.3/rbfly/streams/_client.pyx`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/streams/_codec.c` & `rbfly-0.8.3/rbfly/streams/_codec.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "rbfly.streams._codec",
         "sources": [
@@ -50,18 +50,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -145,14 +145,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -206,14 +208,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -267,60 +271,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -403,14 +430,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -2086,30 +2116,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_9
-#define __PYX_HAVE_RT_ImportType_proto_3_0_9
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_9 {
-   __Pyx_ImportType_CheckSize_Error_3_0_9 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_9 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_9 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportDottedModule.proto */
 static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
@@ -2543,15 +2573,15 @@
 static int __pyx_Generator_init(PyObject *module);
 
 /* CheckBinaryVersion.proto */
 static unsigned long __Pyx_get_runtime_version(void);
 static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer);
 
 /* FunctionImport.proto */
-static int __Pyx_ImportFunction_3_0_9(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
+static int __Pyx_ImportFunction_3_0_10(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 /* #### Code section: module_declarations ### */
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4real_real(PyComplexObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4imag_imag(PyComplexObject *__pyx_v_self); /* proto*/
@@ -3843,70 +3873,70 @@
 #define __pyx_codeobj__19 __pyx_mstate_global->__pyx_codeobj__19
 #define __pyx_codeobj__21 __pyx_mstate_global->__pyx_codeobj__21
 /* #### Code section: module_code ### */
 
 /* "cpython/complex.pxd":19
  * 
  *         @property
- *         cdef inline double real(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double real(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.real
  * 
  */
 
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4real_real(PyComplexObject *__pyx_v_self) {
   double __pyx_r;
 
   /* "cpython/complex.pxd":20
  *         @property
- *         cdef inline double real(self):
+ *         cdef inline double real(self) noexcept:
  *             return self.cval.real             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = __pyx_v_self->cval.real;
   goto __pyx_L0;
 
   /* "cpython/complex.pxd":19
  * 
  *         @property
- *         cdef inline double real(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double real(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.real
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
 /* "cpython/complex.pxd":23
  * 
  *         @property
- *         cdef inline double imag(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double imag(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.imag
  * 
  */
 
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4imag_imag(PyComplexObject *__pyx_v_self) {
   double __pyx_r;
 
   /* "cpython/complex.pxd":24
  *         @property
- *         cdef inline double imag(self):
+ *         cdef inline double imag(self) noexcept:
  *             return self.cval.imag             # <<<<<<<<<<<<<<
  * 
  *     # PyTypeObject PyComplex_Type
  */
   __pyx_r = __pyx_v_self->cval.imag;
   goto __pyx_L0;
 
   /* "cpython/complex.pxd":23
  * 
  *         @property
- *         cdef inline double imag(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double imag(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.imag
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
@@ -4724,15 +4754,15 @@
   }
 
   /* "array.pxd":170
  *     if self.ob_descr.typecode != other.ob_descr.typecode:
  *         PyErr_BadArgument()
  *     return extend_buffer(self, other.data.as_chars, Py_SIZE(other))             # <<<<<<<<<<<<<<
  * 
- * cdef inline void zero(array self):
+ * cdef inline void zero(array self) noexcept:
  */
   __pyx_t_2 = __pyx_f_7cpython_5array_extend_buffer(__pyx_v_self, __pyx_v_other->data.as_chars, Py_SIZE(((PyObject *)__pyx_v_other))); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(3, 170, __pyx_L1_error)
   __pyx_r = __pyx_t_2;
   goto __pyx_L0;
 
   /* "array.pxd":166
  *     return 0
@@ -4749,32 +4779,32 @@
   __pyx_L0:;
   return __pyx_r;
 }
 
 /* "array.pxd":172
  *     return extend_buffer(self, other.data.as_chars, Py_SIZE(other))
  * 
- * cdef inline void zero(array self):             # <<<<<<<<<<<<<<
+ * cdef inline void zero(array self) noexcept:             # <<<<<<<<<<<<<<
  *     """ set all elements of array to zero. """
  *     memset(self.data.as_chars, 0, Py_SIZE(self) * self.ob_descr.itemsize)
  */
 
 static CYTHON_INLINE void __pyx_f_7cpython_5array_zero(arrayobject *__pyx_v_self) {
 
   /* "array.pxd":174
- * cdef inline void zero(array self):
+ * cdef inline void zero(array self) noexcept:
  *     """ set all elements of array to zero. """
  *     memset(self.data.as_chars, 0, Py_SIZE(self) * self.ob_descr.itemsize)             # <<<<<<<<<<<<<<
  */
   (void)(memset(__pyx_v_self->data.as_chars, 0, (Py_SIZE(((PyObject *)__pyx_v_self)) * __pyx_v_self->ob_descr->itemsize)));
 
   /* "array.pxd":172
  *     return extend_buffer(self, other.data.as_chars, Py_SIZE(other))
  * 
- * cdef inline void zero(array self):             # <<<<<<<<<<<<<<
+ * cdef inline void zero(array self) noexcept:             # <<<<<<<<<<<<<<
  *     """ set all elements of array to zero. """
  *     memset(self.data.as_chars, 0, Py_SIZE(self) * self.ob_descr.itemsize)
  */
 
   /* function exit code */
 }
 
@@ -9353,24 +9383,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_5rbfly_7streams_6_codec___pyx_scope_struct__commands *__pyx_freelist_5rbfly_7streams_6_codec___pyx_scope_struct__commands[8];
 static int __pyx_freecount_5rbfly_7streams_6_codec___pyx_scope_struct__commands = 0;
+#endif
 
 static PyObject *__pyx_tp_new_5rbfly_7streams_6_codec___pyx_scope_struct__commands(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_5rbfly_7streams_6_codec___pyx_scope_struct__commands > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_6_codec___pyx_scope_struct__commands)))) {
     o = (PyObject*)__pyx_freelist_5rbfly_7streams_6_codec___pyx_scope_struct__commands[--__pyx_freecount_5rbfly_7streams_6_codec___pyx_scope_struct__commands];
     memset(o, 0, sizeof(struct __pyx_obj_5rbfly_7streams_6_codec___pyx_scope_struct__commands));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -9390,15 +9422,15 @@
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_chunk);
   Py_CLEAR(p->__pyx_v_self);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_5rbfly_7streams_6_codec___pyx_scope_struct__commands < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_6_codec___pyx_scope_struct__commands)))) {
     __pyx_freelist_5rbfly_7streams_6_codec___pyx_scope_struct__commands[__pyx_freecount_5rbfly_7streams_6_codec___pyx_scope_struct__commands++] = ((struct __pyx_obj_5rbfly_7streams_6_codec___pyx_scope_struct__commands *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -9950,39 +9982,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_9(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_9(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_9(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("array"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_5array_array = __Pyx_ImportType_3_0_9(__pyx_t_1, "array", "array", sizeof(arrayobject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(arrayobject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_5array_array) __PYX_ERR(3, 69, __pyx_L1_error)
+  __pyx_ptype_7cpython_5array_array = __Pyx_ImportType_3_0_10(__pyx_t_1, "array", "array", sizeof(arrayobject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(arrayobject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_5array_array) __PYX_ERR(3, 69, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("rbfly.amqp._message"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5rbfly_4amqp_8_message_MessageCtx = __Pyx_ImportType_3_0_9(__pyx_t_1, "rbfly.amqp._message", "MessageCtx", sizeof(struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5rbfly_4amqp_8_message_MessageCtx) __PYX_ERR(7, 24, __pyx_L1_error)
+  __pyx_ptype_5rbfly_4amqp_8_message_MessageCtx = __Pyx_ImportType_3_0_10(__pyx_t_1, "rbfly.amqp._message", "MessageCtx", sizeof(struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5rbfly_4amqp_8_message_MessageCtx) __PYX_ERR(7, 24, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -10002,30 +10034,30 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __pyx_t_1 = PyImport_ImportModule("rbfly._buffer"); if (!__pyx_t_1) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction_3_0_9(__pyx_t_1, "buffer_claim", (void (**)(void))&__pyx_f_5rbfly_7_buffer_buffer_claim, "char *(struct __pyx_t_5rbfly_7_buffer_Buffer *, Py_ssize_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction_3_0_9(__pyx_t_1, "buffer_check_size", (void (**)(void))&__pyx_f_5rbfly_7_buffer_buffer_check_size, "char (struct __pyx_t_5rbfly_7_buffer_Buffer *, uint32_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_3_0_10(__pyx_t_1, "buffer_claim", (void (**)(void))&__pyx_f_5rbfly_7_buffer_buffer_claim, "char *(struct __pyx_t_5rbfly_7_buffer_Buffer *, Py_ssize_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_3_0_10(__pyx_t_1, "buffer_check_size", (void (**)(void))&__pyx_f_5rbfly_7_buffer_buffer_check_size, "char (struct __pyx_t_5rbfly_7_buffer_Buffer *, uint32_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("rbfly.amqp._message"); if (!__pyx_t_1) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction_3_0_9(__pyx_t_1, "c_encode_amqp", (void (**)(void))&__pyx_f_5rbfly_4amqp_8_message_c_encode_amqp, "Py_ssize_t (struct __pyx_t_5rbfly_7_buffer_Buffer *, PyObject *)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction_3_0_9(__pyx_t_1, "c_decode_amqp", (void (**)(void))&__pyx_f_5rbfly_4amqp_8_message_c_decode_amqp, "struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *(struct __pyx_t_5rbfly_7_buffer_Buffer *, Py_ssize_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_3_0_10(__pyx_t_1, "c_encode_amqp", (void (**)(void))&__pyx_f_5rbfly_4amqp_8_message_c_encode_amqp, "Py_ssize_t (struct __pyx_t_5rbfly_7_buffer_Buffer *, PyObject *)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_3_0_10(__pyx_t_1, "c_decode_amqp", (void (**)(void))&__pyx_f_5rbfly_4amqp_8_message_c_decode_amqp, "struct __pyx_obj_5rbfly_4amqp_8_message_MessageCtx *(struct __pyx_t_5rbfly_7_buffer_Buffer *, Py_ssize_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("rbfly._codec"); if (!__pyx_t_1) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_ImportFunction_3_0_9(__pyx_t_1, "unpack_uint16", (void (**)(void))&__pyx_f_5rbfly_6_codec_unpack_uint16, "uint16_t (char const *)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction_3_0_9(__pyx_t_1, "unpack_uint32", (void (**)(void))&__pyx_f_5rbfly_6_codec_unpack_uint32, "uint32_t (char const *)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction_3_0_9(__pyx_t_1, "unpack_uint64", (void (**)(void))&__pyx_f_5rbfly_6_codec_unpack_uint64, "uint64_t (char const *)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction_3_0_9(__pyx_t_1, "pack_uint16", (void (**)(void))&__pyx_f_5rbfly_6_codec_pack_uint16, "void (char *, uint16_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction_3_0_9(__pyx_t_1, "pack_uint32", (void (**)(void))&__pyx_f_5rbfly_6_codec_pack_uint32, "void (char *, uint32_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ImportFunction_3_0_9(__pyx_t_1, "pack_uint64", (void (**)(void))&__pyx_f_5rbfly_6_codec_pack_uint64, "void (char *, uint64_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_3_0_10(__pyx_t_1, "unpack_uint16", (void (**)(void))&__pyx_f_5rbfly_6_codec_unpack_uint16, "uint16_t (char const *)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_3_0_10(__pyx_t_1, "unpack_uint32", (void (**)(void))&__pyx_f_5rbfly_6_codec_unpack_uint32, "uint32_t (char const *)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_3_0_10(__pyx_t_1, "unpack_uint64", (void (**)(void))&__pyx_f_5rbfly_6_codec_unpack_uint64, "uint64_t (char const *)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_3_0_10(__pyx_t_1, "pack_uint16", (void (**)(void))&__pyx_f_5rbfly_6_codec_pack_uint16, "void (char *, uint16_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_3_0_10(__pyx_t_1, "pack_uint32", (void (**)(void))&__pyx_f_5rbfly_6_codec_pack_uint32, "void (char *, uint32_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction_3_0_10(__pyx_t_1, "pack_uint64", (void (**)(void))&__pyx_f_5rbfly_6_codec_pack_uint64, "void (char *, uint64_t)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -12800,18 +12832,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_9
-#define __PYX_HAVE_RT_ImportType_3_0_9
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -12857,23 +12889,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_9 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_9 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -17888,17 +17920,17 @@
                        (int) (rt_version >> 24), (int) ((rt_version >> 16) & 0xFF)
        );
         return PyErr_WarnEx(NULL, message, 1);
     }
 }
 
 /* FunctionImport */
-#ifndef __PYX_HAVE_RT_ImportFunction_3_0_9
-#define __PYX_HAVE_RT_ImportFunction_3_0_9
-static int __Pyx_ImportFunction_3_0_9(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
+#ifndef __PYX_HAVE_RT_ImportFunction_3_0_10
+#define __PYX_HAVE_RT_ImportFunction_3_0_10
+static int __Pyx_ImportFunction_3_0_10(PyObject *module, const char *funcname, void (**f)(void), const char *sig) {
     PyObject *d = 0;
     PyObject *cobj = 0;
     union {
         void (*fp)(void);
         void *p;
     } tmp;
     d = PyObject_GetAttrString(module, (char *)"__pyx_capi__");
```

### Comparing `rbfly-0.8.2/rbfly/streams/_codec.pyi` & `rbfly-0.8.3/rbfly/streams/_codec.pyi`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/streams/_codec.pyx` & `rbfly-0.8.3/rbfly/streams/_codec.pyx`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/streams/_mqueue.c` & `rbfly-0.8.3/rbfly/streams/_mqueue.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "rbfly.streams._mqueue",
         "sources": [
@@ -33,18 +33,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -128,14 +128,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -189,14 +191,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -250,60 +254,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -386,14 +413,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -4932,24 +4962,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_5rbfly_7streams_7_mqueue___pyx_scope_struct__wait *__pyx_freelist_5rbfly_7streams_7_mqueue___pyx_scope_struct__wait[8];
 static int __pyx_freecount_5rbfly_7streams_7_mqueue___pyx_scope_struct__wait = 0;
+#endif
 
 static PyObject *__pyx_tp_new_5rbfly_7streams_7_mqueue___pyx_scope_struct__wait(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_5rbfly_7streams_7_mqueue___pyx_scope_struct__wait > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_mqueue___pyx_scope_struct__wait)))) {
     o = (PyObject*)__pyx_freelist_5rbfly_7streams_7_mqueue___pyx_scope_struct__wait[--__pyx_freecount_5rbfly_7streams_7_mqueue___pyx_scope_struct__wait];
     memset(o, 0, sizeof(struct __pyx_obj_5rbfly_7streams_7_mqueue___pyx_scope_struct__wait));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -4969,15 +5001,15 @@
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_self);
   Py_CLEAR(p->__pyx_v_task);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_5rbfly_7streams_7_mqueue___pyx_scope_struct__wait < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_5rbfly_7streams_7_mqueue___pyx_scope_struct__wait)))) {
     __pyx_freelist_5rbfly_7streams_7_mqueue___pyx_scope_struct__wait[__pyx_freecount_5rbfly_7streams_7_mqueue___pyx_scope_struct__wait++] = ((struct __pyx_obj_5rbfly_7streams_7_mqueue___pyx_scope_struct__wait *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
```

### Comparing `rbfly-0.8.2/rbfly/streams/_mqueue.pxd` & `rbfly-0.8.3/rbfly/streams/_mqueue.pxd`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/streams/_mqueue.pyi` & `rbfly-0.8.3/rbfly/streams/_mqueue.pyi`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/streams/_mqueue.pyx` & `rbfly-0.8.3/rbfly/streams/_mqueue.pyx`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/streams/client.py` & `rbfly-0.8.3/rbfly/streams/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -528,23 +528,24 @@
 def connection(coro: CallAsyncAny[Trc, P, T]) -> CallAsyncAny[Trc, P, T]:
     """
     Decorator to manage RabbitMQ Streams client connection.
 
     Streams client implements connection manager abstract class.
 
     Streams client has to be the first parameter of coroutine `coro`.
+
     Streams client is disconnected on exit of the coroutine using
     connection manager API.
 
     :param coro: Coroutine using RabbitMQ Streams client.
     """
     async def wrapper(client: RabbitMQClient, *args: P.args, **kw: P.kwargs) -> T:
-        assert isinstance(coro, Coroutine)
+        f_coro = tp.cast(CallAsync[RabbitMQClient, P, T], coro)
         async with connection_tracker(CLIENT_REFERENCES, client):
-            result = await coro(client, *args, **kw)
+            result = await f_coro(client, *args, **kw)
         return result
 
     async def wrapper_gen(client: RabbitMQClient, *args: P.args, **kw: P.kwargs) -> AsyncIterator[T]:
         f_gen = tp.cast(CallAsyncIter[RabbitMQClient, P, T], coro)
         async with connection_tracker(CLIENT_REFERENCES, client):
             async for v in f_gen(client, *args, **kw):
                 yield v
```

### Comparing `rbfly-0.8.2/rbfly/streams/codec.py` & `rbfly-0.8.3/rbfly/streams/codec.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/streams/const.py` & `rbfly-0.8.3/rbfly/streams/const.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/streams/error.py` & `rbfly-0.8.3/rbfly/streams/error.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/streams/offset.py` & `rbfly-0.8.3/rbfly/streams/offset.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/streams/protocol.py` & `rbfly-0.8.3/rbfly/streams/protocol.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/streams/types.py` & `rbfly-0.8.3/rbfly/streams/types.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/streams/util.py` & `rbfly-0.8.3/rbfly/streams/util.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/tests/__init__.py` & `rbfly-0.8.3/rbfly/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/tests/amqp/__init__.py` & `rbfly-0.8.3/rbfly/tests/amqp/__init__.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/tests/amqp/test_message.py` & `rbfly-0.8.3/rbfly/tests/amqp/test_message.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/tests/streams/__init__.py` & `rbfly-0.8.3/rbfly/tests/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/tests/streams/test_client.py` & `rbfly-0.8.3/rbfly/tests/streams/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -493,24 +493,30 @@
     ]
     assert call_recorder == expected
 
     # last message id is increased by 2
     assert publisher.message_id == 13
     assert publisher._data == []
 
-def test_connection_coroutine() -> None:
+@pytest.mark.asyncio
+async def test_connection_coroutine() -> None:
     """
     Test if connection decorator returns coroutine function.
     """
-    async def f(client: StreamsClient) -> None:
-        pass
+    async def f(client: StreamsClient) -> int:
+        return 1
 
     assert inspect.iscoroutinefunction(connection(f))
     assert inspect.iscoroutinefunction(connection(partial(f)))
 
+    client = mock.AsyncMock()
+    coro = connection(f)(client)
+    result = await coro
+    assert result == 1
+
 @pytest.mark.asyncio
 async def test_connection_async_iterator() -> None:
     """
     Test if connection decorator returns asynchronous iterator function.
     """
     async def fx(client: StreamsClient) -> AsyncIterator[int]:
         for i in range(10):
```

### Comparing `rbfly-0.8.2/rbfly/tests/streams/test_codec.py` & `rbfly-0.8.3/rbfly/tests/streams/test_codec.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/tests/streams/test_mqueue.py` & `rbfly-0.8.3/rbfly/tests/streams/test_mqueue.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/tests/streams/test_offset.py` & `rbfly-0.8.3/rbfly/tests/streams/test_offset.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/tests/test_slotmap.py` & `rbfly-0.8.3/rbfly/tests/test_slotmap.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/tests/test_util.py` & `rbfly-0.8.3/rbfly/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/types.py` & `rbfly-0.8.3/rbfly/types.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly/util.py` & `rbfly-0.8.3/rbfly/util.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/rbfly.egg-info/PKG-INFO` & `rbfly-0.8.3/rbfly.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbfly
-Version: 0.8.2
+Version: 0.8.3
 Summary: RbFly - a library for RabbitMQ Streams using Python asyncio
 Home-page: https://wrobell.dcmod.org/rbfly/
 Author: Artur Wroblewski
 Author-email: wrobell@riseup.net
 License: GPLv3+
 Project-URL: Source Code, https://gitlab.com/wrobell/rbfly
 Project-URL: Bug tracker, https://gitlab.com/wrobell/rbfly/issues
@@ -14,29 +14,31 @@
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: COPYING
 Provides-Extra: tests
 Requires-Dist: bandit; extra == "tests"
 Requires-Dist: cython-lint; extra == "tests"
-Requires-Dist: mypy==1.9.0; extra == "tests"
+Requires-Dist: mypy==1.10.0; extra == "tests"
 Requires-Dist: pika; extra == "tests"
 Requires-Dist: pytest-asyncio; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: pytest-lazy-fixtures; extra == "tests"
 Requires-Dist: pytest-timeout; extra == "tests"
 Requires-Dist: ruff>=0.3.0; extra == "tests"
 Requires-Dist: toml; extra == "tests"
 Requires-Dist: uvloop>=0.19.0; extra == "tests"
 Provides-Extra: performance
 Requires-Dist: msgpack; extra == "performance"
 Requires-Dist: aiokafka==0.8.1; extra == "performance"
 Requires-Dist: rstream==0.13.0; extra == "performance"
 Requires-Dist: uamqp==1.6.5; extra == "performance"
 Requires-Dist: python-qpid-proton==0.39.0; extra == "performance"
+Provides-Extra: doc
+Requires-Dist: sphinx_rtd_theme; extra == "doc"
 
 RbFly is a library for RabbitMQ Streams using Python asyncio
 
 - https://www.rabbitmq.com/streams.html
 - https://docs.python.org/3/library/asyncio.html
 
 The library is designed and implemented with the following qualities in
```

### Comparing `rbfly-0.8.2/rbfly.egg-info/SOURCES.txt` & `rbfly-0.8.3/rbfly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.2/setup.cfg` & `rbfly-0.8.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rbfly
-version = 0.8.2
+version = 0.8.3
 author = Artur Wroblewski
 author_email = wrobell@riseup.net
 license = GPLv3+
 description = RbFly - a library for RabbitMQ Streams using Python asyncio
 long_description = file: README
 long_description_content_type = text/x-rst
 url = https://wrobell.dcmod.org/rbfly/
@@ -30,27 +30,29 @@
 	*.pxd
 	*.h
 
 [options.extras_require]
 tests = 
 	bandit
 	cython-lint
-	mypy == 1.9.0
+	mypy == 1.10.0
 	pika  # required for integration tests
 	pytest-asyncio
 	pytest-cov
 	pytest-lazy-fixtures
 	pytest-timeout
 	ruff >= 0.3.0
 	toml  # required by bandit, not needed when using Python 3.11?
 	uvloop >= 0.19.0
 performance = 
 	msgpack
 	aiokafka == 0.8.1
 	rstream == 0.13.0
 	uamqp == 1.6.5
 	python-qpid-proton == 0.39.0
+doc = 
+	sphinx_rtd_theme
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `rbfly-0.8.2/setup.py` & `rbfly-0.8.3/setup.py`

 * *Files identical despite different names*

