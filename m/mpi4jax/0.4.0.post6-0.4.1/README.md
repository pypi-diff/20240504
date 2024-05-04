# Comparing `tmp/mpi4jax-0.4.0.post6.tar.gz` & `tmp/mpi4jax-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpi4jax-0.4.0.post6.tar", last modified: Fri Apr  5 16:03:31 2024, max compression
+gzip compressed data, was "mpi4jax-0.4.1.tar", last modified: Sat May  4 08:54:19 2024, max compression
```

## Comparing `mpi4jax-0.4.0.post6.tar` & `mpi4jax-0.4.1.tar`

### file list

```diff
@@ -1,93 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:03:31.379869 mpi4jax-0.4.0.post6/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-05 16:01:39.000000 mpi4jax-0.4.0.post6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-05 16:01:39.000000 mpi4jax-0.4.0.post6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-04-05 16:03:31.379869 mpi4jax-0.4.0.post6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-05 16:01:39.000000 mpi4jax-0.4.0.post6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:03:31.363869 mpi4jax-0.4.0.post6/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    16700 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/examples/shallow_water.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:03:31.379869 mpi4jax-0.4.0.post6/mpi4jax/
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:03:31.367869 mpi4jax-0.4.0.post6/mpi4jax/_src/
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/_latest_jax_version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:03:31.371868 mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/allgather.py
--rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/allreduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/alltoall.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/barrier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/bcast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/gather.py
--rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/recv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/send.py
--rw-r--r--   0 runner    (1001) docker     (127)    11028 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/sendrecv.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/comm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/flush.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/jax_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:03:31.371868 mpi4jax-0.4.0.post6/mpi4jax/_src/xla_bridge/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/xla_bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/xla_bridge/cuda_runtime_api.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/xla_bridge/mpi_xla_bridge_cpu.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    28146 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/_src/xla_bridge/mpi_xla_bridge_gpu.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-05 16:03:31.379869 mpi4jax-0.4.0.post6/mpi4jax/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:03:31.371868 mpi4jax-0.4.0.post6/mpi4jax/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:03:31.371868 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:03:31.375868 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/allgather.py
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/allreduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/alltoall.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/barrier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/bcast.py
--rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/gather.py
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/recv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/send.py
--rw-r--r--   0 runner    (1001) docker     (127)    10529 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/sendrecv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:03:31.375868 mpi4jax-0.4.0.post6/mpi4jax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-04-05 16:03:31.000000 mpi4jax-0.4.0.post6/mpi4jax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-05 16:03:31.000000 mpi4jax-0.4.0.post6/mpi4jax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:03:31.000000 mpi4jax-0.4.0.post6/mpi4jax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:03:31.000000 mpi4jax-0.4.0.post6/mpi4jax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-05 16:03:31.000000 mpi4jax-0.4.0.post6/mpi4jax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 16:03:31.000000 mpi4jax-0.4.0.post6/mpi4jax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-05 16:03:31.379869 mpi4jax-0.4.0.post6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:03:31.375868 mpi4jax-0.4.0.post6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:03:31.375868 mpi4jax-0.4.0.post6/tests/collective_ops/
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/collective_ops/test_allgather.py
--rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/collective_ops/test_allreduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/collective_ops/test_allreduce_matvec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/collective_ops/test_alltoall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/collective_ops/test_barrier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/collective_ops/test_bcast.py
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/collective_ops/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/collective_ops/test_gather.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/collective_ops/test_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/collective_ops/test_scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/collective_ops/test_scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/collective_ops/test_send_and_recv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/collective_ops/test_sendrecv.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:03:31.375868 mpi4jax-0.4.0.post6/tests/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)     9676 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/experimental/test_notoken.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/test_flush.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/test_has_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/test_jax_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    81295 2024-04-05 16:01:40.000000 mpi4jax-0.4.0.post6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:54:19.756313 mpi4jax-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-05-04 08:54:19.756313 mpi4jax-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:54:19.740313 mpi4jax-0.4.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    16700 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/examples/shallow_water.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:54:19.756313 mpi4jax-0.4.1/mpi4jax/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:54:19.744313 mpi4jax-0.4.1/mpi4jax/_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/_latest_jax_version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:54:19.748313 mpi4jax-0.4.1/mpi4jax/_src/collective_ops/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/collective_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/collective_ops/allgather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/collective_ops/allreduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/collective_ops/alltoall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/collective_ops/barrier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/collective_ops/bcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/collective_ops/gather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/collective_ops/recv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/collective_ops/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/collective_ops/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/collective_ops/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/collective_ops/send.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11988 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/collective_ops/sendrecv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/comm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/flush.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/jax_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:54:19.748313 mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/cuda_runtime_api.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/device_descriptors.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/device_descriptors.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/mpi_xla_bridge_cpu.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    22934 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/mpi_xla_bridge_gpu.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    21542 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/mpi_xla_bridge_xpu.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/sycl_runtime_api.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-04 08:54:19.756313 mpi4jax-0.4.1/mpi4jax/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:54:19.748313 mpi4jax-0.4.1/mpi4jax/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:54:19.748313 mpi4jax-0.4.1/mpi4jax/experimental/notoken/
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/experimental/notoken/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:54:19.752313 mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/allgather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/allreduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/alltoall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/barrier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/bcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/gather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/recv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/send.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11490 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/sendrecv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:54:19.756313 mpi4jax-0.4.1/mpi4jax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-05-04 08:54:19.000000 mpi4jax-0.4.1/mpi4jax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-04 08:54:19.000000 mpi4jax-0.4.1/mpi4jax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 08:54:19.000000 mpi4jax-0.4.1/mpi4jax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 08:54:19.000000 mpi4jax-0.4.1/mpi4jax.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-04 08:54:19.000000 mpi4jax-0.4.1/mpi4jax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 08:54:19.000000 mpi4jax-0.4.1/mpi4jax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-04 08:54:19.756313 mpi4jax-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:54:19.752313 mpi4jax-0.4.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:54:19.756313 mpi4jax-0.4.1/tests/collective_ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/collective_ops/test_allgather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/collective_ops/test_allreduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/collective_ops/test_allreduce_matvec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/collective_ops/test_alltoall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/collective_ops/test_barrier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/collective_ops/test_bcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/collective_ops/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/collective_ops/test_gather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/collective_ops/test_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/collective_ops/test_scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/collective_ops/test_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/collective_ops/test_send_and_recv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/collective_ops/test_sendrecv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:54:19.756313 mpi4jax-0.4.1/tests/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)     9676 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/experimental/test_notoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/test_flush.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/test_has_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/test_has_sycl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/test_jax_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81295 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/versioneer.py
```

### Comparing `mpi4jax-0.4.0.post6/LICENSE.md` & `mpi4jax-0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post6/PKG-INFO` & `mpi4jax-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpi4jax
-Version: 0.4.0.post6
+Version: 0.4.1
 Summary: Zero-copy MPI communication of JAX arrays, for turbo-charged HPC applications in Python ⚡
 Home-page: https://github.com/mpi4jax/mpi4jax
 Author: Filippo Vicentini
 Author-email: filippovicentini@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Cython
```

### Comparing `mpi4jax-0.4.0.post6/README.rst` & `mpi4jax-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post6/examples/shallow_water.py` & `mpi4jax-0.4.1/examples/shallow_water.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/_src/__init__.py` & `mpi4jax-0.4.1/mpi4jax/_src/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,11 +26,11 @@
 from .collective_ops.recv import recv  # noqa: F401, E402
 from .collective_ops.reduce import reduce  # noqa: F401, E402
 from .collective_ops.scan import scan  # noqa: F401, E402
 from .collective_ops.scatter import scatter  # noqa: F401, E402
 from .collective_ops.send import send  # noqa: F401, E402
 from .collective_ops.sendrecv import sendrecv  # noqa: F401, E402
 
-from .utils import has_cuda_support  # noqa: F401, E402
+from .utils import has_cuda_support, has_sycl_support  # noqa: F401, E402
 
 # sanitize namespace
 del jax_compat, xla_bridge, MPI, atexit, flush
```

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/allgather.py` & `mpi4jax-0.4.1/mpi4jax/_src/collective_ops/allgather.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,18 +17,24 @@
     wrap_as_hashable,
     as_mhlo_constant,
     get_default_layouts,
     effect,
     prefer_notoken,
 )
 from ..jax_compat import custom_call, token_type, ShapedArray
-from ..decorators import translation_rule_cpu, translation_rule_gpu
+from ..decorators import (
+    translation_rule_cpu,
+    translation_rule_gpu,
+    translation_rule_xpu,
+)
 from ..validation import enforce_types
 from ..comm import get_default_comm
 
+from ..xla_bridge.device_descriptors import build_allgather_descriptor
+
 # The Jax primitive
 mpi_allgather_p = Primitive("allgather_mpi")  # Create the primitive
 mpi_allgather_impl = default_primitive_impl(mpi_allgather_p)
 
 
 # This function applies the primitive to an AST
 @enforce_types(
@@ -124,18 +130,15 @@
         # layout matters here, because the first axis is special
         operand_layouts=get_default_layouts(operands, order="c"),
         result_layouts=get_default_layouts(out_types, order="c"),
         has_side_effect=True,
     ).results
 
 
-@translation_rule_gpu
-def mpi_allgather_xla_encode_gpu(ctx, sendbuf, token, comm):
-    from ..xla_bridge.mpi_xla_bridge_gpu import build_allgather_descriptor
-
+def mpi_allgather_xla_encode_device(ctx, sendbuf, token, comm):
     comm = unpack_hashable(comm)
 
     sendbuf_aval, *_ = ctx.avals_in
     send_nptype = sendbuf_aval.dtype
 
     send_type = ir.RankedTensorType(sendbuf.type)
     send_dtype = send_type.element_type
@@ -173,14 +176,18 @@
         operand_layouts=get_default_layouts(operands, order="c"),
         result_layouts=get_default_layouts(out_types, order="c"),
         backend_config=descriptor,
         has_side_effect=True,
     ).results
 
 
+mpi_allgather_xla_encode_xpu = translation_rule_xpu(mpi_allgather_xla_encode_device)
+mpi_allgather_xla_encode_gpu = translation_rule_gpu(mpi_allgather_xla_encode_device)
+
+
 # This function evaluates only the shapes during AST construction
 def mpi_allgather_abstract_eval(x, token, comm):
     comm = unpack_hashable(comm)
     size = comm.Get_size()
     out_shape = (size, *x.shape)
     return (
         ShapedArray(out_shape, x.dtype),
@@ -190,7 +197,8 @@
 
 mpi_allgather_p.multiple_results = True
 mpi_allgather_p.def_impl(mpi_allgather_impl)
 mpi_allgather_p.def_effectful_abstract_eval(mpi_allgather_abstract_eval)
 
 mlir.register_lowering(mpi_allgather_p, mpi_allgather_xla_encode_cpu, platform="cpu")
 mlir.register_lowering(mpi_allgather_p, mpi_allgather_xla_encode_gpu, platform="cuda")
+mlir.register_lowering(mpi_allgather_p, mpi_allgather_xla_encode_xpu, platform="xpu")
```

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/allreduce.py` & `mpi4jax-0.4.1/mpi4jax/_src/collective_ops/allreduce.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,18 +18,23 @@
     wrap_as_hashable,
     as_mhlo_constant,
     get_default_layouts,
     effect,
     prefer_notoken,
 )
 from ..jax_compat import custom_call, token_type, ShapedArray
-from ..decorators import translation_rule_cpu, translation_rule_gpu
+from ..decorators import (
+    translation_rule_cpu,
+    translation_rule_gpu,
+    translation_rule_xpu,
+)
 from ..validation import enforce_types
 from ..comm import get_default_comm
 
+from ..xla_bridge.device_descriptors import build_allreduce_descriptor
 
 # The Jax primitive
 mpi_allreduce_p = Primitive("allreduce_mpi")  # Create the primitive
 mpi_allreduce_impl = default_primitive_impl(mpi_allreduce_p)
 
 
 # This function applies the primitive to an AST
@@ -118,18 +123,15 @@
         operands=operands,
         operand_layouts=get_default_layouts(operands),
         result_layouts=get_default_layouts(out_types),
         has_side_effect=True,
     ).results
 
 
-@translation_rule_gpu
-def mpi_allreduce_xla_encode_gpu(ctx, x, token, op, comm, transpose):
-    from ..xla_bridge.mpi_xla_bridge_gpu import build_allreduce_descriptor
-
+def mpi_allreduce_xla_encode_device(ctx, x, token, op, comm, transpose):
     op = unpack_hashable(op)
     comm = unpack_hashable(comm)
 
     if transpose:
         assert op == _MPI.SUM
         return [x, token]
 
@@ -167,14 +169,18 @@
         operand_layouts=get_default_layouts(operands),
         result_layouts=get_default_layouts(out_types),
         has_side_effect=True,
         backend_config=descriptor,
     ).results
 
 
+mpi_allreduce_xla_encode_gpu = translation_rule_gpu(mpi_allreduce_xla_encode_device)
+mpi_allreduce_xla_encode_xpu = translation_rule_xpu(mpi_allreduce_xla_encode_device)
+
+
 # This function evaluates only the shapes during AST construction
 def mpi_allreduce_abstract_eval(xs, token, op, comm, transpose):
     return (
         ShapedArray(xs.shape, xs.dtype),
         core.abstract_token,
     ), {effect}
 
@@ -226,7 +232,8 @@
 
 ad.primitive_jvps[mpi_allreduce_p] = mpi_allreduce_value_and_jvp
 ad.primitive_transposes[mpi_allreduce_p] = mpi_allreduce_transpose_rule
 
 # assign to the primitive the correct encoder
 mlir.register_lowering(mpi_allreduce_p, mpi_allreduce_xla_encode_cpu, platform="cpu")
 mlir.register_lowering(mpi_allreduce_p, mpi_allreduce_xla_encode_gpu, platform="cuda")
+mlir.register_lowering(mpi_allreduce_p, mpi_allreduce_xla_encode_xpu, platform="xpu")
```

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/alltoall.py` & `mpi4jax-0.4.1/mpi4jax/_src/collective_ops/alltoall.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,18 +17,22 @@
     wrap_as_hashable,
     as_mhlo_constant,
     get_default_layouts,
     effect,
     prefer_notoken,
 )
 from ..jax_compat import custom_call, token_type, ShapedArray
-from ..decorators import translation_rule_cpu, translation_rule_gpu
+from ..decorators import (
+    translation_rule_cpu,
+    translation_rule_gpu,
+    translation_rule_xpu,
+)
 from ..validation import enforce_types
 from ..comm import get_default_comm
-
+from ..xla_bridge.device_descriptors import build_alltoall_descriptor
 
 # The Jax primitive
 mpi_alltoall_p = Primitive("alltoall_mpi")  # Create the primitive
 mpi_alltoall_impl = default_primitive_impl(mpi_alltoall_p)
 
 
 # This function applies the primitive to an AST
@@ -125,18 +129,15 @@
         # force c order because first axis is special
         operand_layouts=get_default_layouts(operands, order="c"),
         result_layouts=get_default_layouts(out_types, order="c"),
         has_side_effect=True,
     ).results
 
 
-@translation_rule_gpu
-def mpi_alltoall_xla_encode_gpu(ctx, x, token, comm):
-    from ..xla_bridge.mpi_xla_bridge_gpu import build_alltoall_descriptor
-
+def mpi_alltoall_xla_encode_device(ctx, x, token, comm):
     comm = unpack_hashable(comm)
 
     x_aval, *_ = ctx.avals_in
     x_nptype = x_aval.dtype
 
     x_type = ir.RankedTensorType(x.type)
     dtype = x_type.element_type
@@ -176,14 +177,18 @@
         operand_layouts=get_default_layouts(operands, order="c"),
         result_layouts=get_default_layouts(out_types, order="c"),
         has_side_effect=True,
         backend_config=descriptor,
     ).results
 
 
+mpi_alltoall_xla_encode_xpu = translation_rule_xpu(mpi_alltoall_xla_encode_device)
+mpi_alltoall_xla_encode_gpu = translation_rule_gpu(mpi_alltoall_xla_encode_device)
+
+
 # This function evaluates only the shapes during AST construction
 def mpi_alltoall_abstract_eval(xs, token, comm):
     return (
         ShapedArray(xs.shape, xs.dtype),
         core.abstract_token,
     ), {effect}
 
@@ -191,7 +196,8 @@
 mpi_alltoall_p.multiple_results = True
 mpi_alltoall_p.def_impl(mpi_alltoall_impl)
 mpi_alltoall_p.def_effectful_abstract_eval(mpi_alltoall_abstract_eval)
 
 # assign to the primitive the correct encoder
 mlir.register_lowering(mpi_alltoall_p, mpi_alltoall_xla_encode_cpu, platform="cpu")
 mlir.register_lowering(mpi_alltoall_p, mpi_alltoall_xla_encode_gpu, platform="cuda")
+mlir.register_lowering(mpi_alltoall_p, mpi_alltoall_xla_encode_xpu, platform="xpu")
```

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/barrier.py` & `mpi4jax-0.4.1/mpi4jax/_src/collective_ops/barrier.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,17 +16,22 @@
     wrap_as_hashable,
     as_mhlo_constant,
     get_default_layouts,
     effect,
     prefer_notoken,
 )
 from ..jax_compat import custom_call, token_type
-from ..decorators import translation_rule_cpu, translation_rule_gpu
+from ..decorators import (
+    translation_rule_cpu,
+    translation_rule_gpu,
+    translation_rule_xpu,
+)
 from ..validation import enforce_types
 from ..comm import get_default_comm
+from ..xla_bridge.device_descriptors import build_barrier_descriptor
 
 
 # The Jax primitive
 mpi_barrier_p = Primitive("barrier_mpi")  # Create the primitive
 mpi_barrier_impl = default_primitive_impl(mpi_barrier_p)
 
 
@@ -85,18 +90,15 @@
         operands=operands,
         operand_layouts=get_default_layouts(operands),
         result_layouts=get_default_layouts(out_types),
         has_side_effect=True,
     ).results
 
 
-@translation_rule_gpu
-def mpi_barrier_xla_encode_gpu(ctx, token, comm):
-    from ..xla_bridge.mpi_xla_bridge_gpu import build_barrier_descriptor
-
+def mpi_barrier_xla_encode_device(ctx, token, comm):
     comm = unpack_hashable(comm)
 
     out_types = token_type()
 
     operands = (token,)
 
     descriptor = build_barrier_descriptor(to_mpi_handle(comm))
@@ -108,14 +110,18 @@
         operand_layouts=get_default_layouts(operands),
         result_layouts=get_default_layouts(out_types),
         has_side_effect=True,
         backend_config=descriptor,
     ).results
 
 
+mpi_barrier_xla_encode_xpu = translation_rule_xpu(mpi_barrier_xla_encode_device)
+mpi_barrier_xla_encode_gpu = translation_rule_gpu(mpi_barrier_xla_encode_device)
+
+
 # This function evaluates only the shapes during AST construction
 def mpi_barrier_abstract_eval(token, comm):
     return core.abstract_token, {effect}
 
 
 def mpi_barrier_batch_eval(in_args, batch_axes, comm):
     token = in_args[0]
@@ -127,7 +133,8 @@
 mpi_barrier_p.def_effectful_abstract_eval(mpi_barrier_abstract_eval)
 
 batching.primitive_batchers[mpi_barrier_p] = mpi_barrier_batch_eval
 
 # assign to the primitive the correct encoder
 mlir.register_lowering(mpi_barrier_p, mpi_barrier_xla_encode_cpu, platform="cpu")
 mlir.register_lowering(mpi_barrier_p, mpi_barrier_xla_encode_gpu, platform="cuda")
+mlir.register_lowering(mpi_barrier_p, mpi_barrier_xla_encode_xpu, platform="xpu")
```

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/bcast.py` & `mpi4jax-0.4.1/mpi4jax/_src/collective_ops/bcast.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,17 +17,22 @@
     wrap_as_hashable,
     as_mhlo_constant,
     get_default_layouts,
     effect,
     prefer_notoken,
 )
 from ..jax_compat import custom_call, token_type, ShapedArray
-from ..decorators import translation_rule_cpu, translation_rule_gpu
+from ..decorators import (
+    translation_rule_cpu,
+    translation_rule_gpu,
+    translation_rule_xpu,
+)
 from ..validation import enforce_types
 from ..comm import get_default_comm
+from ..xla_bridge.device_descriptors import build_bcast_descriptor
 
 
 # The Jax primitive
 mpi_bcast_p = Primitive("bcast_mpi")  # Create the primitive
 mpi_bcast_impl = default_primitive_impl(mpi_bcast_p)
 
 
@@ -122,18 +127,15 @@
         operands=operands,
         operand_layouts=get_default_layouts(operands),
         result_layouts=get_default_layouts(out_types),
         has_side_effect=True,
     ).results
 
 
-@translation_rule_gpu
-def mpi_bcast_xla_encode_gpu(ctx, x, token, root, comm):
-    from ..xla_bridge.mpi_xla_bridge_gpu import build_bcast_descriptor
-
+def mpi_bcast_xla_encode_device(ctx, x, token, root, comm):
     comm = unpack_hashable(comm)
 
     x_aval, *_ = ctx.avals_in
     x_nptype = x_aval.dtype
 
     x_type = ir.RankedTensorType(x.type)
     dtype = x_type.element_type
@@ -172,14 +174,18 @@
         operand_layouts=get_default_layouts(operands),
         result_layouts=get_default_layouts(out_types),
         has_side_effect=True,
         backend_config=descriptor,
     ).results
 
 
+mpi_bcast_xla_encode_xpu = translation_rule_xpu(mpi_bcast_xla_encode_device)
+mpi_bcast_xla_encode_gpu = translation_rule_gpu(mpi_bcast_xla_encode_device)
+
+
 # This function evaluates only the shapes during AST construction
 def mpi_bcast_abstract_eval(xs, token, root, comm):
     comm = unpack_hashable(comm)
     rank = comm.Get_rank()
 
     if rank == root:
         dims = (0,)
@@ -195,7 +201,8 @@
 mpi_bcast_p.multiple_results = True
 mpi_bcast_p.def_impl(mpi_bcast_impl)
 mpi_bcast_p.def_effectful_abstract_eval(mpi_bcast_abstract_eval)
 
 # assign to the primitive the correct encoder
 mlir.register_lowering(mpi_bcast_p, mpi_bcast_xla_encode_cpu, platform="cpu")
 mlir.register_lowering(mpi_bcast_p, mpi_bcast_xla_encode_gpu, platform="cuda")
+mlir.register_lowering(mpi_bcast_p, mpi_bcast_xla_encode_xpu, platform="xpu")
```

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/gather.py` & `mpi4jax-0.4.1/mpi4jax/_src/collective_ops/gather.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,17 +17,22 @@
     wrap_as_hashable,
     as_mhlo_constant,
     get_default_layouts,
     effect,
     prefer_notoken,
 )
 from ..jax_compat import custom_call, token_type, ShapedArray
-from ..decorators import translation_rule_cpu, translation_rule_gpu
+from ..decorators import (
+    translation_rule_cpu,
+    translation_rule_gpu,
+    translation_rule_xpu,
+)
 from ..validation import enforce_types
 from ..comm import get_default_comm
+from ..xla_bridge.device_descriptors import build_gather_descriptor
 
 
 # The Jax primitive
 mpi_gather_p = Primitive("gather_mpi")  # Create the primitive
 mpi_gather_impl = default_primitive_impl(mpi_gather_p)
 
 
@@ -146,18 +151,15 @@
         # enforce c order because the first axis is special
         operand_layouts=get_default_layouts(operands, order="c"),
         result_layouts=get_default_layouts(out_types, order="c"),
         has_side_effect=True,
     ).results
 
 
-@translation_rule_gpu
-def mpi_gather_xla_encode_gpu(ctx, x, token, root, comm):
-    from ..xla_bridge.mpi_xla_bridge_gpu import build_gather_descriptor
-
+def mpi_gather_xla_encode_device(ctx, x, token, root, comm):
     comm = unpack_hashable(comm)
 
     x_aval, *_ = ctx.avals_in
     x_nptype = x_aval.dtype
 
     x_type = ir.RankedTensorType(x.type)
     dtype = x_type.element_type
@@ -205,14 +207,18 @@
         operand_layouts=get_default_layouts(operands, order="c"),
         result_layouts=get_default_layouts(out_types, order="c"),
         has_side_effect=True,
         backend_config=descriptor,
     ).results
 
 
+mpi_gather_xla_encode_xpu = translation_rule_xpu(mpi_gather_xla_encode_device)
+mpi_gather_xla_encode_gpu = translation_rule_gpu(mpi_gather_xla_encode_device)
+
+
 # This function evaluates only the shapes during AST construction
 def mpi_gather_abstract_eval(x, token, root, comm):
     comm = unpack_hashable(comm)
     rank = comm.Get_rank()
     size = comm.Get_size()
 
     if rank == root:
@@ -229,7 +235,8 @@
 mpi_gather_p.multiple_results = True
 mpi_gather_p.def_impl(mpi_gather_impl)
 mpi_gather_p.def_effectful_abstract_eval(mpi_gather_abstract_eval)
 
 # assign to the primitive the correct encoder
 mlir.register_lowering(mpi_gather_p, mpi_gather_xla_encode_cpu, platform="cpu")
 mlir.register_lowering(mpi_gather_p, mpi_gather_xla_encode_gpu, platform="cuda")
+mlir.register_lowering(mpi_gather_p, mpi_gather_xla_encode_xpu, platform="xpu")
```

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/recv.py` & `mpi4jax-0.4.1/mpi4jax/_src/collective_ops/recv.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,18 +18,23 @@
     wrap_as_hashable,
     as_mhlo_constant,
     get_default_layouts,
     effect,
     prefer_notoken,
 )
 from ..jax_compat import custom_call, token_type, ShapedArray
-from ..decorators import translation_rule_cpu, translation_rule_gpu
+from ..decorators import (
+    translation_rule_cpu,
+    translation_rule_gpu,
+    translation_rule_xpu,
+)
 from ..validation import enforce_types
 from ..comm import get_default_comm
 
+from ..xla_bridge.device_descriptors import build_recv_descriptor
 
 # The Jax primitive
 mpi_recv_p = Primitive("recv_mpi")  # Create the primitive
 mpi_recv_impl = default_primitive_impl(mpi_recv_p)
 
 
 # This function applies the primitive to an AST
@@ -138,18 +143,16 @@
         operands=operands,
         operand_layouts=get_default_layouts(operands),
         result_layouts=get_default_layouts(out_types),
         has_side_effect=True,
     ).results
 
 
-@translation_rule_gpu
-def mpi_recv_xla_encode_gpu(ctx, x, token, source, tag, comm, status):
+def mpi_recv_xla_encode_device(ctx, x, token, source, tag, comm, status):
     from ..xla_bridge.mpi_xla_bridge import MPI_STATUS_IGNORE_ADDR
-    from ..xla_bridge.mpi_xla_bridge_gpu import build_recv_descriptor
 
     comm = unpack_hashable(comm)
     status = unpack_hashable(status)
 
     x_aval, *_ = ctx.avals_in
     x_nptype = x_aval.dtype
 
@@ -189,14 +192,18 @@
         operand_layouts=get_default_layouts(operands),
         result_layouts=get_default_layouts(out_types),
         has_side_effect=True,
         backend_config=descriptor,
     ).results
 
 
+mpi_recv_xla_encode_xpu = translation_rule_xpu(mpi_recv_xla_encode_device)
+mpi_recv_xla_encode_gpu = translation_rule_gpu(mpi_recv_xla_encode_device)
+
+
 # This function evaluates only the shapes during AST construction
 def mpi_recv_abstract_eval(xs, token, source, tag, comm, status):
     return (
         ShapedArray(xs.shape, xs.dtype),
         core.abstract_token,
     ), {effect}
 
@@ -204,7 +211,8 @@
 mpi_recv_p.multiple_results = True
 mpi_recv_p.def_impl(mpi_recv_impl)
 mpi_recv_p.def_effectful_abstract_eval(mpi_recv_abstract_eval)
 
 # assign to the primitive the correct encoder
 mlir.register_lowering(mpi_recv_p, mpi_recv_xla_encode_cpu, platform="cpu")
 mlir.register_lowering(mpi_recv_p, mpi_recv_xla_encode_gpu, platform="cuda")
+mlir.register_lowering(mpi_recv_p, mpi_recv_xla_encode_xpu, platform="xpu")
```

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/reduce.py` & `mpi4jax-0.4.1/mpi4jax/_src/collective_ops/reduce.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,17 +17,22 @@
     wrap_as_hashable,
     as_mhlo_constant,
     get_default_layouts,
     effect,
     prefer_notoken,
 )
 from ..jax_compat import custom_call, token_type, ShapedArray
-from ..decorators import translation_rule_cpu, translation_rule_gpu
+from ..decorators import (
+    translation_rule_cpu,
+    translation_rule_gpu,
+    translation_rule_xpu,
+)
 from ..validation import enforce_types
 from ..comm import get_default_comm
+from ..xla_bridge.device_descriptors import build_reduce_descriptor
 
 
 # The Jax primitive
 mpi_reduce_p = Primitive("reduce_mpi")  # Create the primitive
 mpi_reduce_impl = default_primitive_impl(mpi_reduce_p)
 
 
@@ -125,18 +130,15 @@
         operands=operands,
         operand_layouts=get_default_layouts(operands),
         result_layouts=get_default_layouts(out_types),
         has_side_effect=True,
     ).results
 
 
-@translation_rule_gpu
-def mpi_reduce_xla_encode_gpu(ctx, x, token, op, root, comm):
-    from ..xla_bridge.mpi_xla_bridge_gpu import build_reduce_descriptor
-
+def mpi_reduce_xla_encode_device(ctx, x, token, op, root, comm):
     op = unpack_hashable(op)
     comm = unpack_hashable(comm)
 
     x_aval, *_ = ctx.avals_in
     x_nptype = x_aval.dtype
 
     x_type = ir.RankedTensorType(x.type)
@@ -179,14 +181,18 @@
         operand_layouts=get_default_layouts(operands),
         result_layouts=get_default_layouts(out_types),
         has_side_effect=True,
         backend_config=descriptor,
     ).results
 
 
+mpi_reduce_xla_encode_xpu = translation_rule_xpu(mpi_reduce_xla_encode_device)
+mpi_reduce_xla_encode_gpu = translation_rule_gpu(mpi_reduce_xla_encode_device)
+
+
 # This function evaluates only the shapes during AST construction
 def mpi_reduce_abstract_eval(xs, token, op, root, comm):
     comm = unpack_hashable(comm)
     rank = comm.Get_rank()
 
     if rank != root:
         dims = (0,)
@@ -202,7 +208,8 @@
 mpi_reduce_p.multiple_results = True
 mpi_reduce_p.def_impl(mpi_reduce_impl)
 mpi_reduce_p.def_effectful_abstract_eval(mpi_reduce_abstract_eval)
 
 # assign to the primitive the correct encoder
 mlir.register_lowering(mpi_reduce_p, mpi_reduce_xla_encode_cpu, platform="cpu")
 mlir.register_lowering(mpi_reduce_p, mpi_reduce_xla_encode_gpu, platform="cuda")
+mlir.register_lowering(mpi_reduce_p, mpi_reduce_xla_encode_xpu, platform="xpu")
```

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/scan.py` & `mpi4jax-0.4.1/mpi4jax/_src/collective_ops/scan.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,17 +17,22 @@
     wrap_as_hashable,
     as_mhlo_constant,
     get_default_layouts,
     effect,
     prefer_notoken,
 )
 from ..jax_compat import custom_call, token_type, ShapedArray
-from ..decorators import translation_rule_cpu, translation_rule_gpu
+from ..decorators import (
+    translation_rule_cpu,
+    translation_rule_gpu,
+    translation_rule_xpu,
+)
 from ..validation import enforce_types
 from ..comm import get_default_comm
+from ..xla_bridge.device_descriptors import build_scan_descriptor
 
 
 # The Jax primitive
 mpi_scan_p = Primitive("scan_mpi")  # Create the primitive
 mpi_scan_impl = default_primitive_impl(mpi_scan_p)
 
 
@@ -108,18 +113,15 @@
         operands=operands,
         operand_layouts=get_default_layouts(operands),
         result_layouts=get_default_layouts(out_types),
         has_side_effect=True,
     ).results
 
 
-@translation_rule_gpu
-def mpi_scan_xla_encode_gpu(ctx, x, token, op, comm):
-    from ..xla_bridge.mpi_xla_bridge_gpu import build_scan_descriptor
-
+def mpi_scan_xla_encode_device(ctx, x, token, op, comm):
     op = unpack_hashable(op)
     comm = unpack_hashable(comm)
 
     x_aval, *_ = ctx.avals_in
     x_nptype = x_aval.dtype
 
     x_type = ir.RankedTensorType(x.type)
@@ -155,14 +157,18 @@
         operand_layouts=get_default_layouts(operands),
         result_layouts=get_default_layouts(out_types),
         has_side_effect=True,
         backend_config=descriptor,
     ).results
 
 
+mpi_scan_xla_encode_xpu = translation_rule_xpu(mpi_scan_xla_encode_device)
+mpi_scan_xla_encode_gpu = translation_rule_gpu(mpi_scan_xla_encode_device)
+
+
 # This function evaluates only the shapes during AST construction
 def mpi_scan_abstract_eval(xs, token, op, comm):
     return (
         ShapedArray(xs.shape, xs.dtype),
         core.abstract_token,
     ), {effect}
 
@@ -170,7 +176,8 @@
 mpi_scan_p.multiple_results = True
 mpi_scan_p.def_impl(mpi_scan_impl)
 mpi_scan_p.def_effectful_abstract_eval(mpi_scan_abstract_eval)
 
 # assign to the primitive the correct encoder
 mlir.register_lowering(mpi_scan_p, mpi_scan_xla_encode_cpu, platform="cpu")
 mlir.register_lowering(mpi_scan_p, mpi_scan_xla_encode_gpu, platform="cuda")
+mlir.register_lowering(mpi_scan_p, mpi_scan_xla_encode_xpu, platform="xpu")
```

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/scatter.py` & `mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/scatter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 import numpy as _np
 from mpi4py import MPI as _MPI
 
-from jax import core
-from jax.core import Primitive, Tracer, Token
-from jax.lax import create_token
+from jax.core import Primitive
 
 from jax.interpreters import mlir
 import jaxlib.mlir.ir as ir
 
-from ..utils import (
+from mpi4jax._src.utils import (
     HashableMPIType,
     default_primitive_impl,
     to_dtype_handle,
     to_mpi_handle,
     unpack_hashable,
     wrap_as_hashable,
     as_mhlo_constant,
     get_default_layouts,
-    effect,
-    prefer_notoken,
+    ordered_effect,
 )
-from ..jax_compat import custom_call, token_type, ShapedArray
-from ..decorators import translation_rule_cpu, translation_rule_gpu
-from ..validation import enforce_types
-from ..comm import get_default_comm
+from mpi4jax._src.jax_compat import custom_call, token_type, ShapedArray
+from mpi4jax._src.decorators import (
+    translation_rule_cpu,
+    translation_rule_gpu,
+    translation_rule_xpu,
+)
+from mpi4jax._src.validation import enforce_types
+from mpi4jax._src.comm import get_default_comm
+
+from mpi4jax._src.xla_bridge.device_descriptors import build_scatter_descriptor
 
 
 # The Jax primitive
 mpi_scatter_p = Primitive("scatter_mpi")  # Create the primitive
 mpi_scatter_impl = default_primitive_impl(mpi_scatter_p)
 
 
 # This function applies the primitive to an AST
 @enforce_types(
     root=(_np.integer),
     comm=(type(None), _MPI.Intracomm, HashableMPIType),
-    token=(type(None), Token, Tracer),
 )
 def scatter(
     x,
     root,
     *,
     comm=None,
-    token=None,
 ):
     """Perform a scatter operation.
 
     .. warning::
 
         Unlike mpi4py's scatter, this returns a *new* array with the received data.
 
@@ -59,55 +60,40 @@
         x: Array or scalar input with the correct shape and dtype. On the root process,
            this contains the data to send, and its first axis must have size ``nproc``.
            On non-root processes, this may contain arbitrary data and will not be
            overwritten.
         root (int): Rank of the root MPI process.
         comm (mpi4py.MPI.Comm): The MPI communicator to use (defaults to
             a clone of :obj:`COMM_WORLD`).
-        token (Token): XLA token to use to ensure correct execution order.
-            If not given, a new token is generated.
 
     Returns:
-        Tuple[DeviceArray, Token]:
-            - Received data.
-            - A new, modified token, that depends on this operation.
+        DeviceArray: Received data.
 
     """
-    if token is None:
-        token = create_token(x)
-
-    if prefer_notoken():
-        from mpi4jax.experimental.notoken import scatter
-
-        return scatter(x, root, comm=comm), token
-
     if comm is None:
         comm = get_default_comm()
 
     rank = comm.Get_rank()
     if rank == root:
         size = comm.Get_size()
         if x.shape[0] != size:
             raise ValueError("Scatter input must have shape (nproc, ...)")
 
     comm = wrap_as_hashable(comm)
 
-    return tuple(
-        mpi_scatter_p.bind(
-            x,
-            token,
-            root=root,
-            comm=comm,
-        )
+    return mpi_scatter_p.bind(
+        x,
+        root=root,
+        comm=comm,
     )
 
 
 # This function compiles the operation
 @translation_rule_cpu
-def mpi_scatter_xla_encode_cpu(ctx, x, token, root, comm):
+def mpi_scatter_xla_encode_cpu(ctx, x, root, comm):
     comm = unpack_hashable(comm)
 
     x_aval, *_ = ctx.avals_in
     x_nptype = x_aval.dtype
 
     x_type = ir.RankedTensorType(x.type)
     dtype = x_type.element_type
@@ -122,41 +108,46 @@
     dtype_handle = to_dtype_handle(x_nptype)
 
     out_types = [
         ir.RankedTensorType.get(dims, dtype),
         *token_type(),
     ]
 
+    token = ctx.tokens_in.get(ordered_effect)[0]
+
     operands = (
         as_mhlo_constant(nitems, _np.intc),
         x,
         as_mhlo_constant(dtype_handle, _np.uintp),
         # we only support matching input and output arrays
         as_mhlo_constant(nitems, _np.intc),
         as_mhlo_constant(dtype_handle, _np.uintp),
         #
         as_mhlo_constant(root, _np.intc),
         as_mhlo_constant(to_mpi_handle(comm), _np.uintp),
         token,
     )
 
-    return custom_call(
+    result_obj = custom_call(
         b"mpi_scatter",
         result_types=out_types,
         operands=operands,
         operand_layouts=get_default_layouts(operands),
         result_layouts=get_default_layouts(out_types),
         has_side_effect=True,
-    ).results
+    )
 
+    results = list(result_obj.results)
+    token = results.pop(-1)
+    ctx.set_tokens_out(mlir.TokenSet({ordered_effect: (token,)}))
 
-@translation_rule_gpu
-def mpi_scatter_xla_encode_gpu(ctx, x, token, root, comm):
-    from ..xla_bridge.mpi_xla_bridge_gpu import build_scatter_descriptor
+    return results
 
+
+def mpi_scatter_xla_encode_device(ctx, x, root, comm):
     comm = unpack_hashable(comm)
 
     x_aval, *_ = ctx.avals_in
     x_nptype = x_aval.dtype
 
     x_type = ir.RankedTensorType(x.type)
     dtype = x_type.element_type
@@ -171,14 +162,16 @@
     dtype_handle = to_dtype_handle(x_nptype)
 
     out_types = [
         ir.RankedTensorType.get(dims, dtype),
         *token_type(),
     ]
 
+    token = ctx.tokens_in.get(ordered_effect)[0]
+
     operands = (
         x,
         token,
     )
 
     descriptor = build_scatter_descriptor(
         nitems,
@@ -187,40 +180,47 @@
         nitems,
         dtype_handle,
         #
         root,
         to_mpi_handle(comm),
     )
 
-    return custom_call(
+    result_obj = custom_call(
         b"mpi_scatter",
         result_types=out_types,
         operands=operands,
         operand_layouts=get_default_layouts(operands),
         result_layouts=get_default_layouts(out_types),
         has_side_effect=True,
         backend_config=descriptor,
-    ).results
+    )
+
+    results = list(result_obj.results)
+    token = results.pop(-1)
+    ctx.set_tokens_out(mlir.TokenSet({ordered_effect: (token,)}))
+
+    return results
+
+
+mpi_scatter_xla_encode_xpu = translation_rule_xpu(mpi_scatter_xla_encode_device)
+mpi_scatter_xla_encode_gpu = translation_rule_gpu(mpi_scatter_xla_encode_device)
 
 
 # This function evaluates only the shapes during AST construction
-def mpi_scatter_abstract_eval(x, token, root, comm):
+def mpi_scatter_abstract_eval(x, root, comm):
     comm = unpack_hashable(comm)
     rank = comm.Get_rank()
     if rank == root:
         out_shape = x.shape[1:]
     else:
         out_shape = x.shape
 
-    return (
-        ShapedArray(out_shape, x.dtype),
-        core.abstract_token,
-    ), {effect}
+    return ShapedArray(out_shape, x.dtype), {ordered_effect}
 
 
-mpi_scatter_p.multiple_results = True
 mpi_scatter_p.def_impl(mpi_scatter_impl)
 mpi_scatter_p.def_effectful_abstract_eval(mpi_scatter_abstract_eval)
 
 # assign to the primitive the correct encoder
 mlir.register_lowering(mpi_scatter_p, mpi_scatter_xla_encode_cpu, platform="cpu")
 mlir.register_lowering(mpi_scatter_p, mpi_scatter_xla_encode_gpu, platform="cuda")
+mlir.register_lowering(mpi_scatter_p, mpi_scatter_xla_encode_xpu, platform="xpu")
```

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/send.py` & `mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/send.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,162 +1,174 @@
 import numpy as _np
 from mpi4py import MPI as _MPI
 
-from jax import core
-from jax.core import Primitive, Tracer, Token
-from jax.lax import create_token
+from jax.core import Primitive
 
 from jax.interpreters import mlir
 import jaxlib.mlir.ir as ir
 
-from ..utils import (
+from mpi4jax._src.utils import (
     HashableMPIType,
     default_primitive_impl,
     to_dtype_handle,
     to_mpi_handle,
     unpack_hashable,
     wrap_as_hashable,
     as_mhlo_constant,
     get_default_layouts,
-    effect,
-    prefer_notoken,
+    ordered_effect,
 )
-from ..jax_compat import custom_call, token_type
-from ..decorators import translation_rule_cpu, translation_rule_gpu
-from ..validation import enforce_types
-from ..comm import get_default_comm
+from mpi4jax._src.jax_compat import custom_call, token_type
+from mpi4jax._src.decorators import (
+    translation_rule_cpu,
+    translation_rule_gpu,
+    translation_rule_xpu,
+)
+from mpi4jax._src.validation import enforce_types
+from mpi4jax._src.comm import get_default_comm
 
+from mpi4jax._src.xla_bridge.device_descriptors import build_send_descriptor
 
 # The Jax primitive
 mpi_send_p = Primitive("send_mpi")  # Create the primitive
 mpi_send_impl = default_primitive_impl(mpi_send_p)
 
 
 # This function applies the primitive to an AST
 @enforce_types(
     dest=_np.integer,
     tag=_np.integer,
     comm=(type(None), _MPI.Intracomm, HashableMPIType),
-    token=(type(None), Token, Tracer),
 )
-def send(x, dest, *, tag=0, comm=None, token=None):
+def send(
+    x,
+    dest,
+    *,
+    tag=0,
+    comm=None,
+):
     """Perform a send operation.
 
     Arguments:
         x: Array or scalar input to send.
         dest (int): Rank of the destination MPI process.
         tag (int): Tag of this message.
         comm (mpi4py.MPI.Comm): The MPI communicator to use (defaults to
             a clone of :obj:`COMM_WORLD`).
-        token (Token): XLA token to use to ensure correct execution order.
-            If not given, a new token is generated.
-
-    Returns:
-        Token: A new, modified token, that depends on this operation.
 
     """
-    if token is None:
-        token = create_token(x)
-
-    if prefer_notoken():
-        from mpi4jax.experimental.notoken import send
-
-        send(x, dest, tag=tag, comm=comm)
-        return token
-
     if comm is None:
         comm = get_default_comm()
 
     comm = wrap_as_hashable(comm)
-    return mpi_send_p.bind(x, token, dest=dest, tag=tag, comm=comm)
+    return mpi_send_p.bind(x, dest=dest, tag=tag, comm=comm)
 
 
 # This function compiles the operation
 @translation_rule_cpu
-def mpi_send_xla_encode_cpu(ctx, x, token, dest, tag, comm):
+def mpi_send_xla_encode_cpu(ctx, x, dest, tag, comm):
     comm = unpack_hashable(comm)
 
     x_aval, *_ = ctx.avals_in
     x_nptype = x_aval.dtype
 
     x_type = ir.RankedTensorType(x.type)
     dims = x_type.shape
 
     # compute total number of elements in array
     nitems = _np.prod(dims, dtype=int)
     dtype_handle = to_dtype_handle(x_nptype)
 
     out_types = token_type()
 
+    token = ctx.tokens_in.get(ordered_effect)[0]
+
     operands = (
         as_mhlo_constant(nitems, _np.intc),
         x,
         as_mhlo_constant(dest, _np.intc),
         as_mhlo_constant(tag, _np.intc),
         as_mhlo_constant(to_mpi_handle(comm), _np.uintp),
         as_mhlo_constant(dtype_handle, _np.uintp),
         token,
     )
 
-    return custom_call(
+    result_obj = custom_call(
         b"mpi_send",
         result_types=out_types,
         operands=operands,
         operand_layouts=get_default_layouts(operands),
         result_layouts=get_default_layouts(out_types),
         has_side_effect=True,
-    ).results
+    )
 
+    results = list(result_obj.results)
+    token = results.pop(-1)
+    ctx.set_tokens_out(mlir.TokenSet({ordered_effect: (token,)}))
 
-@translation_rule_gpu
-def mpi_send_xla_encode_gpu(ctx, x, token, dest, tag, comm):
-    from ..xla_bridge.mpi_xla_bridge_gpu import build_send_descriptor
+    return results
 
+
+def mpi_send_xla_encode_device(ctx, x, dest, tag, comm):
     comm = unpack_hashable(comm)
 
     x_aval, *_ = ctx.avals_in
     x_nptype = x_aval.dtype
 
     x_type = ir.RankedTensorType(x.type)
     dims = x_type.shape
 
     # compute total number of elements in array
     nitems = _np.prod(dims, dtype=int)
     dtype_handle = to_dtype_handle(x_nptype)
 
     out_types = token_type()
 
+    token = ctx.tokens_in.get(ordered_effect)[0]
+
     operands = (
         x,
         token,
     )
 
     descriptor = build_send_descriptor(
         nitems,
         dest,
         tag,
         to_mpi_handle(comm),
         dtype_handle,
     )
 
-    return custom_call(
+    result_obj = custom_call(
         b"mpi_send",
         result_types=out_types,
         operands=operands,
         operand_layouts=get_default_layouts(operands),
         result_layouts=get_default_layouts(out_types),
         has_side_effect=True,
         backend_config=descriptor,
-    ).results
+    )
+
+    results = list(result_obj.results)
+    token = results.pop(-1)
+    ctx.set_tokens_out(mlir.TokenSet({ordered_effect: (token,)}))
+
+    return results
+
+
+mpi_send_xla_encode_xpu = translation_rule_xpu(mpi_send_xla_encode_device)
+mpi_send_xla_encode_gpu = translation_rule_gpu(mpi_send_xla_encode_device)
 
 
 # This function evaluates only the shapes during AST construction
-def mpi_send_abstract_eval(xs, token, dest, tag, comm):
-    return core.abstract_token, {effect}
+def mpi_send_abstract_eval(xs, dest, tag, comm):
+    return (), {ordered_effect}
 
 
+mpi_send_p.multiple_results = True
 mpi_send_p.def_impl(mpi_send_impl)
 mpi_send_p.def_effectful_abstract_eval(mpi_send_abstract_eval)
 
 # assign to the primitive the correct encoder
 mlir.register_lowering(mpi_send_p, mpi_send_xla_encode_cpu, platform="cpu")
 mlir.register_lowering(mpi_send_p, mpi_send_xla_encode_gpu, platform="cuda")
+mlir.register_lowering(mpi_send_p, mpi_send_xla_encode_xpu, platform="xpu")
```

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/_src/collective_ops/sendrecv.py` & `mpi4jax-0.4.1/mpi4jax/_src/collective_ops/sendrecv.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,17 +19,22 @@
     wrap_as_hashable,
     as_mhlo_constant,
     get_default_layouts,
     effect,
     prefer_notoken,
 )
 from ..jax_compat import custom_call, token_type, ShapedArray
-from ..decorators import translation_rule_cpu, translation_rule_gpu
+from ..decorators import (
+    translation_rule_cpu,
+    translation_rule_gpu,
+    translation_rule_xpu,
+)
 from ..validation import enforce_types
 from ..comm import get_default_comm
+from ..xla_bridge.device_descriptors import build_sendrecv_descriptor
 
 
 # The Jax primitive
 mpi_sendrecv_p = Primitive("sendrecv_mpi")  # Create the primitive
 mpi_sendrecv_impl = default_primitive_impl(mpi_sendrecv_p)
 
 
@@ -206,37 +211,35 @@
         operands=operands,
         operand_layouts=get_default_layouts(operands),
         result_layouts=get_default_layouts(out_types),
         has_side_effect=True,
     ).results
 
 
-@translation_rule_gpu
-def mpi_sendrecv_xla_encode_gpu(
+def mpi_sendrecv_xla_encode_device(
     ctx,
     sendbuf,
     recvbuf,
     token,
     source,
     dest,
     sendtag,
     recvtag,
     comm,
     status,
-    _must_transpose=False,
+    _must_transpose,
 ):
     if _must_transpose:
         raise RuntimeError(
             "sendrecv cannot be used with forward-mode (vjp) autodiff, because "
             "the gradient might be located on a different mpi rank than the "
             "desired one. Use reverse-mode (jvp) differentiation instead."
         )
 
     from ..xla_bridge.mpi_xla_bridge import MPI_STATUS_IGNORE_ADDR
-    from ..xla_bridge.mpi_xla_bridge_gpu import build_sendrecv_descriptor
 
     comm = unpack_hashable(comm)
     status = unpack_hashable(status)
 
     send_aval, recv_aval, *_ = ctx.avals_in
     send_nptype = send_aval.dtype
     recv_nptype = recv_aval.dtype
@@ -290,14 +293,72 @@
         operand_layouts=get_default_layouts(operands),
         result_layouts=get_default_layouts(out_types),
         has_side_effect=True,
         backend_config=descriptor,
     ).results
 
 
+@translation_rule_xpu
+def mpi_sendrecv_xla_encode_xpu(
+    ctx,
+    sendbuf,
+    recvbuf,
+    token,
+    source,
+    dest,
+    sendtag,
+    recvtag,
+    comm,
+    status,
+    _must_transpose=False,
+):
+    return mpi_sendrecv_xla_encode_device(
+        ctx,
+        sendbuf,
+        recvbuf,
+        token,
+        source,
+        dest,
+        sendtag,
+        recvtag,
+        comm,
+        status,
+        _must_transpose,
+    )
+
+
+@translation_rule_gpu
+def mpi_sendrecv_xla_encode_gpu(
+    ctx,
+    sendbuf,
+    recvbuf,
+    token,
+    source,
+    dest,
+    sendtag,
+    recvtag,
+    comm,
+    status,
+    _must_transpose=False,
+):
+    return mpi_sendrecv_xla_encode_device(
+        ctx,
+        sendbuf,
+        recvbuf,
+        token,
+        source,
+        dest,
+        sendtag,
+        recvtag,
+        comm,
+        status,
+        _must_transpose,
+    )
+
+
 # This function evaluates only the shapes during AST construction
 def mpi_sendrecv_abstract_eval(
     sendbuf,
     recvbuf,
     token,
     source,
     dest,
@@ -417,7 +478,8 @@
 
 ad.primitive_jvps[mpi_sendrecv_p] = mpi_sendrecv_value_and_jvp
 ad.primitive_transposes[mpi_sendrecv_p] = mpi_sendrecv_transpose_rule
 
 # assign to the primitive the correct encoder
 mlir.register_lowering(mpi_sendrecv_p, mpi_sendrecv_xla_encode_cpu, platform="cpu")
 mlir.register_lowering(mpi_sendrecv_p, mpi_sendrecv_xla_encode_gpu, platform="cuda")
+mlir.register_lowering(mpi_sendrecv_p, mpi_sendrecv_xla_encode_xpu, platform="xpu")
```

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/_src/jax_compat.py` & `mpi4jax-0.4.1/mpi4jax/_src/jax_compat.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/_src/utils.py` & `mpi4jax-0.4.1/mpi4jax/_src/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -160,10 +160,19 @@
     jax-arrays, False otherwise.
     """
     from . import xla_bridge
 
     return xla_bridge.HAS_GPU_EXT
 
 
+def has_sycl_support() -> bool:
+    """Returns True if mpi4jax is built with SYCL support and can be used with XPU-based
+    jax-arrays, False otherwise.
+    """
+    from . import xla_bridge
+
+    return xla_bridge.HAS_XPU_EXT
+
+
 def prefer_notoken() -> bool:
     """Returns True if primitive implementations should prefer not to use tokens."""
     return os.environ.get("MPI4JAX_PREFER_NOTOKEN", "0").lower() in ("1", "true", "on")
```

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/_src/validation.py` & `mpi4jax-0.4.1/mpi4jax/_src/validation.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/_src/xla_bridge/__init__.py` & `mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 try:
     from . import mpi_xla_bridge_gpu
 except ImportError:
     HAS_GPU_EXT = False
 else:
     HAS_GPU_EXT = True
 
+try:
+    from . import mpi_xla_bridge_xpu
+except ImportError:
+    HAS_XPU_EXT = False
+else:
+    HAS_XPU_EXT = True
 
 # setup logging
 
 
 def _is_truthy(str_val):
     return str_val.lower() in ("true", "1", "on")
 
@@ -25,7 +31,11 @@
 # register custom call targets
 for name, fn in mpi_xla_bridge_cpu.cpu_custom_call_targets.items():
     xla_client.register_custom_call_target(name, fn, platform="cpu")
 
 if HAS_GPU_EXT:
     for name, fn in mpi_xla_bridge_gpu.gpu_custom_call_targets.items():
         xla_client.register_custom_call_target(name, fn, platform="CUDA")
+
+if HAS_XPU_EXT:
+    for name, fn in mpi_xla_bridge_xpu.xpu_custom_call_targets.items():
+        xla_client.register_custom_call_target(name, fn, platform="SYCL")
```

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/_src/xla_bridge/cuda_runtime_api.pxd` & `mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/cuda_runtime_api.pxd`

 * *Files 8% similar despite different names*

```diff
@@ -10,10 +10,11 @@
         cudaMemcpyDefault = 4
 
     ctypedef cudaError cudaError_t
 
     ctypedef void* cudaStream_t
     cudaError_t cudaStreamSynchronize(cudaStream_t stream) nogil
     cudaError_t cudaMemcpy(void *dst, const void *src, size_t count, cudaMemcpyKind kind) nogil
+    cudaError_t cudaMemcpyAsync(void *dst, const void *src, size_t count, cudaMemcpyKind kind, cudaStream_t stream) nogil
 
     const char* cudaGetErrorName(cudaError_t error) nogil
     const char* cudaGetErrorString(cudaError_t error) nogil
```

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pxd` & `mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pxd`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pyx` & `mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pyx`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/_src/xla_bridge/mpi_xla_bridge_cpu.pyx` & `mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/mpi_xla_bridge_cpu.pyx`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/_src/xla_bridge/mpi_xla_bridge_gpu.pyx` & `mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/mpi_xla_bridge_gpu.pyx`

 * *Files 16% similar despite different names*

```diff
@@ -9,19 +9,34 @@
     MPI_Comm_size,
     MPI_Datatype,
     MPI_Op,
     MPI_Status,
     MPI_Type_size,
 )
 
+from .device_descriptors cimport (
+    RecvDescriptor,
+    AllgatherDescriptor,
+    AllreduceDescriptor,
+    AlltoallDescriptor,
+    BarrierDescriptor,
+    BcastDescriptor,
+    GatherDescriptor,
+    ReduceDescriptor,
+    ScanDescriptor,
+    ScatterDescriptor,
+    SendDescriptor,
+    SendrecvDescriptor,
+)
+
 from .cuda_runtime_api cimport (
     cudaGetErrorName,
     cudaGetErrorString,
     cudaError_t,
-    cudaMemcpy,
+    cudaMemcpyAsync,
     cudaMemcpyDeviceToDevice,
     cudaMemcpyDeviceToHost,
     cudaMemcpyKind,
     cudaMemcpyHostToDevice,
     cudaStream_t,
     cudaStreamSynchronize,
     cudaSuccess,
@@ -64,29 +79,29 @@
 
         mpi_xla_bridge.abort(0, comm, message)
 
     return mem
 
 
 cdef inline cudaError_t checked_cuda_memcpy(void* dst, void* src, size_t count,
-                                            cudaMemcpyKind kind, MPI_Comm comm) nogil:
+                                            cudaMemcpyKind kind, cudaStream_t stream, MPI_Comm comm) nogil:
     cdef cudaError_t ierr
-    ierr = cudaMemcpy(dst, src, count, kind)
-
+    ierr = cudaMemcpyAsync(dst, src, count, kind, stream)
     if ierr != cudaSuccess:
         with gil:
             err_str = get_error_name(ierr)
             err_des = get_error_string(ierr)
             message = (
-                f"cudaMemcpy failed with the following error:\n"
+                f"cudaMemcpyAsync failed with the following error:\n"
                 f"\tError {ierr} {err_str}: {err_des}"
             )
 
         mpi_xla_bridge.abort(0, comm, message)
 
+    ierr = checked_cuda_stream_synchronize(stream, comm)
     return ierr
 
 
 cdef inline cudaError_t checked_cuda_stream_synchronize(
     cudaStream_t stream, MPI_Comm comm
 ) nogil:
     cdef cudaError_t ierr
@@ -102,41 +117,14 @@
             )
 
         mpi_xla_bridge.abort(0, comm, message)
 
     return ierr
 
 
-#
-# GPU XLA targets
-#
-
-# Allgather
-
-cdef struct AllgatherDescriptor:
-    int sendcount
-    MPI_Datatype sendtype
-    int recvcount
-    MPI_Datatype recvtype
-    MPI_Comm comm
-
-
-cpdef bytes build_allgather_descriptor(
-    int sendcount, uintptr_t sendtype_handle,
-    int recvcount, uintptr_t recvtype_addr,
-    uintptr_t comm_handle
-):
-    cdef AllgatherDescriptor desc = AllgatherDescriptor(
-        sendcount, <MPI_Datatype> sendtype_handle,
-        recvcount, <MPI_Datatype> recvtype_addr,
-        <MPI_Comm> comm_handle
-    )
-    return bytes((<char*> &desc)[:sizeof(AllgatherDescriptor)])
-
-
 cdef void mpi_allgather_gpu(cudaStream_t stream, void** buffers,
                             const char* opaque, size_t opaque_len) nogil:
     cdef int ierr, sendtype_size, recvtype_size, comm_size
     cdef size_t sendbytes, recvbytes
 
     # decode inputs
     cdef void* data = buffers[0]
@@ -152,16 +140,14 @@
     cdef AllgatherDescriptor* desc = <AllgatherDescriptor*>(opaque)
     cdef int sendcount = desc.sendcount
     cdef MPI_Datatype sendtype = desc.sendtype
     cdef int recvcount = desc.recvcount
     cdef MPI_Datatype recvtype = desc.recvtype
     cdef MPI_Comm comm = desc.comm
 
-    checked_cuda_stream_synchronize(stream, comm)
-
     if COPY_TO_HOST:
         # copy memory to host
         ierr = MPI_Type_size(sendtype, &sendtype_size)
         mpi_xla_bridge.abort_on_error(ierr, comm, u"Type_size")
 
         sendbytes = sendtype_size * sendcount
         in_buf = checked_malloc(sendbytes, comm)
@@ -172,46 +158,31 @@
         ierr = MPI_Comm_size(comm, &comm_size)
         mpi_xla_bridge.abort_on_error(ierr, comm, u"Comm_size")
 
         # recvcount is received data *per process*
         recvbytes = recvtype_size * recvcount * comm_size
         out_buf = checked_malloc(recvbytes, comm)
 
-        checked_cuda_memcpy(in_buf, data, sendbytes, cudaMemcpyDeviceToHost, comm)
+        checked_cuda_memcpy(in_buf, data, sendbytes, cudaMemcpyDeviceToHost, stream, comm)
+    else:
+        checked_cuda_stream_synchronize(stream, comm)
 
     mpi_xla_bridge.mpi_allgather(
         in_buf, sendcount, sendtype,
         out_buf, recvcount, recvtype,
         comm
     )
 
     if COPY_TO_HOST:
         # copy back to device
-        checked_cuda_memcpy(out_data, out_buf, recvbytes, cudaMemcpyHostToDevice, comm)
+        checked_cuda_memcpy(out_data, out_buf, recvbytes, cudaMemcpyHostToDevice, stream, comm)
         free(in_buf)
         free(out_buf)
 
 
-# Allreduce
-
-cdef struct AllreduceDescriptor:
-    int nitems
-    MPI_Op op
-    MPI_Comm comm
-    MPI_Datatype dtype
-
-
-cpdef bytes build_allreduce_descriptor(int nitems, uintptr_t op_handle,
-                                       uintptr_t comm_handle, uintptr_t dtype_handle):
-    cdef AllreduceDescriptor desc = AllreduceDescriptor(
-        nitems, <MPI_Op> op_handle, <MPI_Comm> comm_handle, <MPI_Datatype> dtype_handle
-    )
-    return bytes((<char*> &desc)[:sizeof(AllreduceDescriptor)])
-
-
 cdef void mpi_allreduce_gpu(cudaStream_t stream, void** buffers,
                             const char* opaque, size_t opaque_len) nogil:
     cdef int ierr, dtype_size
     cdef size_t count
 
     # decode inputs
     cdef void* data = buffers[0]
@@ -226,58 +197,35 @@
 
     cdef AllreduceDescriptor* desc = <AllreduceDescriptor*>(opaque)
     cdef int nitems = desc.nitems
     cdef MPI_Op op = desc.op
     cdef MPI_Comm comm = desc.comm
     cdef MPI_Datatype dtype = desc.dtype
 
-    checked_cuda_stream_synchronize(stream, comm)
-
     if COPY_TO_HOST:
         # copy memory to host
         ierr = MPI_Type_size(dtype, &dtype_size)
         mpi_xla_bridge.abort_on_error(ierr, comm, u"Type_size")
 
         count = dtype_size * nitems
         in_buf = checked_malloc(count, comm)
         out_buf = checked_malloc(count, comm)
-        checked_cuda_memcpy(in_buf, data, count, cudaMemcpyDeviceToHost, comm)
+        checked_cuda_memcpy(in_buf, data, count, cudaMemcpyDeviceToHost, stream, comm)
+    else:
+        checked_cuda_stream_synchronize(stream, comm)
 
     mpi_xla_bridge.mpi_allreduce(in_buf, out_buf, nitems, dtype, op, comm)
 
     if COPY_TO_HOST:
         # copy back to device
-        checked_cuda_memcpy(out_data, out_buf, count, cudaMemcpyHostToDevice, comm)
+        checked_cuda_memcpy(out_data, out_buf, count, cudaMemcpyHostToDevice, stream, comm)
         free(in_buf)
         free(out_buf)
 
 
-# Alltoall
-
-cdef struct AlltoallDescriptor:
-    int sendcount
-    MPI_Datatype sendtype
-    int recvcount
-    MPI_Datatype recvtype
-    MPI_Comm comm
-
-
-cpdef bytes build_alltoall_descriptor(
-    int sendcount, uintptr_t sendtype_handle,
-    int recvcount, uintptr_t recvtype_addr,
-    uintptr_t comm_handle
-):
-    cdef AlltoallDescriptor desc = AlltoallDescriptor(
-        sendcount, <MPI_Datatype> sendtype_handle,
-        recvcount, <MPI_Datatype> recvtype_addr,
-        <MPI_Comm> comm_handle
-    )
-    return bytes((<char*> &desc)[:sizeof(AlltoallDescriptor)])
-
-
 cdef void mpi_alltoall_gpu(cudaStream_t stream, void** buffers,
                            const char* opaque, size_t opaque_len) nogil:
     cdef int ierr, sendtype_size, recvtype_size, comm_size
     cdef size_t sendbytes, recvbytes
 
     # decode inputs
     cdef void* data = buffers[0]
@@ -293,16 +241,14 @@
     cdef AlltoallDescriptor* desc = <AlltoallDescriptor*>(opaque)
     cdef int sendcount = desc.sendcount
     cdef MPI_Datatype sendtype = desc.sendtype
     cdef int recvcount = desc.recvcount
     cdef MPI_Datatype recvtype = desc.recvtype
     cdef MPI_Comm comm = desc.comm
 
-    checked_cuda_stream_synchronize(stream, comm)
-
     if COPY_TO_HOST:
         # copy memory to host
 
         # counts are *per process*, so multiply with comm_size
         ierr = MPI_Comm_size(comm, &comm_size)
         mpi_xla_bridge.abort_on_error(ierr, comm, u"Comm_size")
 
@@ -314,67 +260,41 @@
 
         ierr = MPI_Type_size(recvtype, &recvtype_size)
         mpi_xla_bridge.abort_on_error(ierr, comm, u"Type_size")
 
         recvbytes = recvtype_size * recvcount * comm_size
         out_buf = checked_malloc(recvbytes, comm)
 
-        checked_cuda_memcpy(in_buf, data, sendbytes, cudaMemcpyDeviceToHost, comm)
+        checked_cuda_memcpy(in_buf, data, sendbytes, cudaMemcpyDeviceToHost, stream, comm)
+    else:
+        checked_cuda_stream_synchronize(stream, comm)
 
     mpi_xla_bridge.mpi_alltoall(
         in_buf, sendcount, sendtype, out_buf, recvcount, recvtype, comm
     )
 
     if COPY_TO_HOST:
         # copy back to device
-        checked_cuda_memcpy(out_data, out_buf, recvbytes, cudaMemcpyHostToDevice, comm)
+        checked_cuda_memcpy(out_data, out_buf, recvbytes, cudaMemcpyHostToDevice, stream, comm)
         free(in_buf)
         free(out_buf)
 
 
-# Barrier
-
-cdef struct BarrierDescriptor:
-    MPI_Comm comm
-
-
-cpdef bytes build_barrier_descriptor(uintptr_t comm_handle):
-    cdef BarrierDescriptor desc = BarrierDescriptor(<MPI_Comm> comm_handle)
-    return bytes((<char*> &desc)[:sizeof(BarrierDescriptor)])
-
-
 cdef void mpi_barrier_gpu(cudaStream_t stream, void** buffers,
                           const char* opaque, size_t opaque_len) nogil:
     if opaque_len != sizeof(BarrierDescriptor):
         with gil:
             raise RuntimeError("got wrong size of opaque argument")
 
     cdef BarrierDescriptor* desc = <BarrierDescriptor*>(opaque)
     cdef MPI_Comm comm = desc.comm
 
     mpi_xla_bridge.mpi_barrier(comm)
 
 
-# Bcast
-
-cdef struct BcastDescriptor:
-    int nitems
-    int root
-    MPI_Comm comm
-    MPI_Datatype dtype
-
-
-cpdef bytes build_bcast_descriptor(int nitems, int root, uintptr_t comm_handle,
-                                   uintptr_t dtype_handle):
-    cdef BcastDescriptor desc = BcastDescriptor(
-        nitems, root, <MPI_Comm> comm_handle, <MPI_Datatype> dtype_handle
-    )
-    return bytes((<char*> &desc)[:sizeof(BcastDescriptor)])
-
-
 cdef void mpi_bcast_gpu(cudaStream_t stream, void** buffers,
                         const char* opaque, size_t opaque_len) nogil:
     cdef int ierr, dtype_size, rank
     cdef size_t count
 
     # decode inputs
     cdef void* data = buffers[0]
@@ -393,57 +313,34 @@
     cdef MPI_Datatype dtype = desc.dtype
 
     ierr = MPI_Type_size(dtype, &dtype_size)
     mpi_xla_bridge.abort_on_error(ierr, comm, u"Type_size")
     ierr = MPI_Comm_rank(comm, &rank)
     mpi_xla_bridge.abort_on_error(ierr, comm, u"Comm_rank")
 
-    checked_cuda_stream_synchronize(stream, comm)
-
     if COPY_TO_HOST:
         # copy memory to host
         count = dtype_size * nitems
         buf = checked_malloc(count, comm)
         if rank == root:
-            checked_cuda_memcpy(buf, data, count, cudaMemcpyDeviceToHost, comm)
+            checked_cuda_memcpy(buf, data, count, cudaMemcpyDeviceToHost, stream, comm)
     else:
         if rank == root:
             buf = data
+        checked_cuda_stream_synchronize(stream, comm)
 
     mpi_xla_bridge.mpi_bcast(buf, nitems, dtype, root, comm)
 
     if COPY_TO_HOST:
         if rank != root:
             # copy back to device
-            checked_cuda_memcpy(out_data, buf, count, cudaMemcpyHostToDevice, comm)
+            checked_cuda_memcpy(out_data, buf, count, cudaMemcpyHostToDevice, stream, comm)
         free(buf)
 
 
-# Gather
-
-cdef struct GatherDescriptor:
-    int sendcount
-    MPI_Datatype sendtype
-    int recvcount
-    MPI_Datatype recvtype
-    int root
-    MPI_Comm comm
-
-
-cpdef bytes build_gather_descriptor(
-    int sendcount, uintptr_t sendtype_handle,
-    int recvcount, uintptr_t recvtype_addr,
-    int root, uintptr_t comm_handle
-):
-    cdef GatherDescriptor desc = GatherDescriptor(
-        sendcount, <MPI_Datatype> sendtype_handle,
-        recvcount, <MPI_Datatype> recvtype_addr,
-        root, <MPI_Comm> comm_handle
-    )
-    return bytes((<char*> &desc)[:sizeof(GatherDescriptor)])
 
 
 cdef void mpi_gather_gpu(cudaStream_t stream, void** buffers,
                          const char* opaque, size_t opaque_len) nogil:
     cdef int ierr, sendtype_size, recvtype_size, rank, size
     cdef size_t sendbytes, recvbytes
 
@@ -462,16 +359,14 @@
     cdef int sendcount = desc.sendcount
     cdef MPI_Datatype sendtype = desc.sendtype
     cdef int recvcount = desc.recvcount
     cdef MPI_Datatype recvtype = desc.recvtype
     cdef int root = desc.root
     cdef MPI_Comm comm = desc.comm
 
-    checked_cuda_stream_synchronize(stream, comm)
-
     if COPY_TO_HOST:
         # copy memory to host
         ierr = MPI_Type_size(sendtype, &sendtype_size)
         mpi_xla_bridge.abort_on_error(ierr, comm, u"Type_size")
 
         sendbytes = sendtype_size * sendcount
         in_buf = checked_malloc(sendbytes, comm)
@@ -488,53 +383,33 @@
         recvbytes = recvtype_size * recvcount
         if rank == root:
             # output shape is larger on root
             recvbytes *= size
 
         out_buf = checked_malloc(recvbytes, comm)
 
-        checked_cuda_memcpy(in_buf, data, sendbytes, cudaMemcpyDeviceToHost, comm)
+        checked_cuda_memcpy(in_buf, data, sendbytes, cudaMemcpyDeviceToHost, stream, comm)
+    else:
+        checked_cuda_stream_synchronize(stream, comm)
 
     mpi_xla_bridge.mpi_gather(
         in_buf, sendcount, sendtype, out_buf, recvcount, recvtype, root, comm
     )
 
     if COPY_TO_HOST:
         if rank == root:
             # copy back to device
             checked_cuda_memcpy(
-                out_data, out_buf, recvbytes, cudaMemcpyHostToDevice, comm
+                out_data, out_buf, recvbytes, cudaMemcpyHostToDevice, stream, comm
             )
 
         free(in_buf)
         free(out_buf)
 
 
-# Recv
-
-cdef struct RecvDescriptor:
-    int nitems
-    int source
-    int tag
-    MPI_Comm comm
-    MPI_Datatype dtype
-    MPI_Status* status
-
-
-cpdef bytes build_recv_descriptor(int nitems, int dest, int tag, uintptr_t comm_handle,
-                                  uintptr_t dtype_handle, uintptr_t status_addr):
-    cdef RecvDescriptor desc = RecvDescriptor(
-        nitems, dest, tag,
-        <MPI_Comm> comm_handle,
-        <MPI_Datatype> dtype_handle,
-        <MPI_Status*> status_addr
-    )
-    return bytes((<char*> &desc)[:sizeof(RecvDescriptor)])
-
-
 cdef void mpi_recv_gpu(cudaStream_t stream, void** buffers,
                        const char* opaque, size_t opaque_len) nogil:
     cdef int ierr, dtype_size
     cdef size_t count
 
     # decode inputs
     cdef void* out_buf = buffers[1]
@@ -549,40 +424,31 @@
     cdef int nitems = desc.nitems
     cdef int source = desc.source
     cdef int tag = desc.tag
     cdef MPI_Comm comm = desc.comm
     cdef MPI_Datatype dtype = desc.dtype
     cdef MPI_Status* status = desc.status
 
-    checked_cuda_stream_synchronize(stream, comm)
-
     if COPY_TO_HOST:
         # copy memory to host
         ierr = MPI_Type_size(dtype, &dtype_size)
         mpi_xla_bridge.abort_on_error(ierr, comm, u"Type_size")
 
         count = dtype_size * nitems
         recvbuf = checked_malloc(count, comm)
+    else:
+        checked_cuda_stream_synchronize(stream, comm)
 
     mpi_xla_bridge.mpi_recv(recvbuf, nitems, dtype, source, tag, comm, status)
 
     if COPY_TO_HOST:
-        checked_cuda_memcpy(out_buf, recvbuf, count, cudaMemcpyHostToDevice, comm)
+        checked_cuda_memcpy(out_buf, recvbuf, count, cudaMemcpyHostToDevice, stream, comm)
         free(recvbuf)
 
 
-# Reduce
-
-cdef struct ReduceDescriptor:
-    int nitems
-    MPI_Op op
-    int root
-    MPI_Comm comm
-    MPI_Datatype dtype
-
 
 cpdef bytes build_reduce_descriptor(int nitems, uintptr_t op_handle, int root,
                                     uintptr_t comm_handle, uintptr_t dtype_handle):
     cdef ReduceDescriptor desc = ReduceDescriptor(
         nitems, <MPI_Op> op_handle, root, <MPI_Comm> comm_handle,
         <MPI_Datatype> dtype_handle
     )
@@ -608,57 +474,40 @@
     cdef ReduceDescriptor* desc = <ReduceDescriptor*>(opaque)
     cdef int nitems = desc.nitems
     cdef MPI_Op op = desc.op
     cdef int root = desc.root
     cdef MPI_Comm comm = desc.comm
     cdef MPI_Datatype dtype = desc.dtype
 
-    checked_cuda_stream_synchronize(stream, comm)
-
     if COPY_TO_HOST:
         # copy memory to host
         ierr = MPI_Type_size(dtype, &dtype_size)
         mpi_xla_bridge.abort_on_error(ierr, comm, u"Type_size")
 
         count = dtype_size * nitems
         in_buf = checked_malloc(count, comm)
         out_buf = checked_malloc(count, comm)
-        checked_cuda_memcpy(in_buf, data, count, cudaMemcpyDeviceToHost, comm)
+        checked_cuda_memcpy(in_buf, data, count, cudaMemcpyDeviceToHost, stream, comm)
+    else:
+        checked_cuda_stream_synchronize(stream, comm)
 
     mpi_xla_bridge.mpi_reduce(in_buf, out_buf, nitems, dtype, op, root, comm)
 
     if COPY_TO_HOST:
         ierr = MPI_Comm_rank(comm, &rank)
         mpi_xla_bridge.abort_on_error(ierr, comm, u"Comm_rank")
 
         if rank == root:
             # copy back to device
-            checked_cuda_memcpy(out_data, out_buf, count, cudaMemcpyHostToDevice, comm)
+            checked_cuda_memcpy(out_data, out_buf, count, cudaMemcpyHostToDevice, stream, comm)
 
         free(in_buf)
         free(out_buf)
 
 
-# Scan
-
-cdef struct ScanDescriptor:
-    int nitems
-    MPI_Op op
-    MPI_Comm comm
-    MPI_Datatype dtype
-
-
-cpdef bytes build_scan_descriptor(int nitems, uintptr_t op_handle,
-                                  uintptr_t comm_handle, uintptr_t dtype_handle):
-    cdef ScanDescriptor desc = ScanDescriptor(
-        nitems, <MPI_Op> op_handle, <MPI_Comm> comm_handle, <MPI_Datatype> dtype_handle
-    )
-    return bytes((<char*> &desc)[:sizeof(ScanDescriptor)])
-
-
 cdef void mpi_scan_gpu(cudaStream_t stream, void** buffers,
                        const char* opaque, size_t opaque_len) nogil:
     cdef int ierr, dtype_size
     cdef size_t count
 
     # decode inputs
     cdef void* data = buffers[0]
@@ -673,59 +522,35 @@
 
     cdef ScanDescriptor* desc = <ScanDescriptor*>(opaque)
     cdef int nitems = desc.nitems
     cdef MPI_Op op = desc.op
     cdef MPI_Comm comm = desc.comm
     cdef MPI_Datatype dtype = desc.dtype
 
-    checked_cuda_stream_synchronize(stream, comm)
-
     if COPY_TO_HOST:
         # copy memory to host
         ierr = MPI_Type_size(dtype, &dtype_size)
         mpi_xla_bridge.abort_on_error(ierr, comm, u"Type_size")
 
         count = dtype_size * nitems
         in_buf = checked_malloc(count, comm)
         out_buf = checked_malloc(count, comm)
-        checked_cuda_memcpy(in_buf, data, count, cudaMemcpyDeviceToHost, comm)
+        checked_cuda_memcpy(in_buf, data, count, cudaMemcpyDeviceToHost, stream, comm)
+    else:
+        checked_cuda_stream_synchronize(stream, comm)
 
     mpi_xla_bridge.mpi_scan(in_buf, out_buf, nitems, dtype, op, comm)
 
     if COPY_TO_HOST:
         # copy back to device
-        checked_cuda_memcpy(out_data, out_buf, count, cudaMemcpyHostToDevice, comm)
+        checked_cuda_memcpy(out_data, out_buf, count, cudaMemcpyHostToDevice, stream, comm)
         free(in_buf)
         free(out_buf)
 
 
-# Scatter
-
-cdef struct ScatterDescriptor:
-    int sendcount
-    MPI_Datatype sendtype
-    int recvcount
-    MPI_Datatype recvtype
-    int root
-    MPI_Comm comm
-
-
-cpdef bytes build_scatter_descriptor(
-    int sendcount, uintptr_t sendtype_handle,
-    int recvcount, uintptr_t recvtype_addr,
-    int root, uintptr_t comm_handle
-):
-    cdef ScatterDescriptor desc = ScatterDescriptor(
-        sendcount, <MPI_Datatype> sendtype_handle,
-        recvcount, <MPI_Datatype> recvtype_addr,
-        root, <MPI_Comm> comm_handle
-    )
-    return bytes((<char*> &desc)[:sizeof(ScatterDescriptor)])
-
-
 cdef void mpi_scatter_gpu(cudaStream_t stream, void** buffers,
                           const char* opaque, size_t opaque_len) nogil:
     cdef int ierr, sendtype_size, recvtype_size, rank, size
     cdef size_t sendbytes, recvbytes
 
     # decode inputs
     cdef void* data = buffers[0]
@@ -742,16 +567,14 @@
     cdef int sendcount = desc.sendcount
     cdef MPI_Datatype sendtype = desc.sendtype
     cdef int recvcount = desc.recvcount
     cdef MPI_Datatype recvtype = desc.recvtype
     cdef int root = desc.root
     cdef MPI_Comm comm = desc.comm
 
-    checked_cuda_stream_synchronize(stream, comm)
-
     if COPY_TO_HOST:
         # copy memory to host
         ierr = MPI_Comm_rank(comm, &rank)
         mpi_xla_bridge.abort_on_error(ierr, comm, u"Comm_rank")
 
         ierr = MPI_Comm_size(comm, &size)
         mpi_xla_bridge.abort_on_error(ierr, comm, u"Comm_size")
@@ -768,46 +591,30 @@
 
         ierr = MPI_Type_size(recvtype, &recvtype_size)
         mpi_xla_bridge.abort_on_error(ierr, comm, u"Type_size")
 
         recvbytes = recvtype_size * recvcount
         out_buf = checked_malloc(recvbytes, comm)
 
-        checked_cuda_memcpy(in_buf, data, sendbytes, cudaMemcpyDeviceToHost, comm)
+        checked_cuda_memcpy(in_buf, data, sendbytes, cudaMemcpyDeviceToHost, stream, comm)
+    else:
+        checked_cuda_stream_synchronize(stream, comm)
 
     mpi_xla_bridge.mpi_scatter(
         in_buf, sendcount, sendtype, out_buf, recvcount, recvtype, root, comm
     )
 
     if COPY_TO_HOST:
         # copy back to device
-        checked_cuda_memcpy(out_data, out_buf, recvbytes, cudaMemcpyHostToDevice, comm)
+        checked_cuda_memcpy(out_data, out_buf, recvbytes, cudaMemcpyHostToDevice, stream, comm)
 
         free(in_buf)
         free(out_buf)
 
 
-# Send
-
-cdef struct SendDescriptor:
-    int nitems
-    int dest
-    int tag
-    MPI_Comm comm
-    MPI_Datatype dtype
-
-
-cpdef bytes build_send_descriptor(int nitems, int dest, int tag, uintptr_t comm_handle,
-                                  uintptr_t dtype_handle):
-    cdef SendDescriptor desc = SendDescriptor(
-        nitems, dest, tag, <MPI_Comm> comm_handle, <MPI_Datatype> dtype_handle
-    )
-    return bytes((<char*> &desc)[:sizeof(SendDescriptor)])
-
-
 cdef void mpi_send_gpu(cudaStream_t stream, void** buffers,
                        const char* opaque, size_t opaque_len) nogil:
     cdef int ierr, dtype_size
     cdef size_t count
 
     # decode inputs
     cdef void* data = buffers[0]
@@ -821,59 +628,31 @@
     cdef SendDescriptor* desc = <SendDescriptor*>(opaque)
     cdef int nitems = desc.nitems
     cdef int dest = desc.dest
     cdef int tag = desc.tag
     cdef MPI_Comm comm = desc.comm
     cdef MPI_Datatype dtype = desc.dtype
 
-    checked_cuda_stream_synchronize(stream, comm)
-
     if COPY_TO_HOST:
         # copy memory to host
         ierr = MPI_Type_size(dtype, &dtype_size)
         mpi_xla_bridge.abort_on_error(ierr, comm, u"Type_size")
 
         count = dtype_size * nitems
         sendbuf = checked_malloc(count, comm)
-        checked_cuda_memcpy(sendbuf, data, count, cudaMemcpyDeviceToHost, comm)
+        checked_cuda_memcpy(sendbuf, data, count, cudaMemcpyDeviceToHost, stream, comm)
+    else:
+        checked_cuda_stream_synchronize(stream, comm)
 
     mpi_xla_bridge.mpi_send(sendbuf, nitems, dtype, dest, tag, comm)
 
     if COPY_TO_HOST:
         free(sendbuf)
 
 
-# Sendrecv
-
-cdef struct SendrecvDescriptor:
-    int sendcount
-    int dest
-    int sendtag
-    MPI_Datatype sendtype
-    int recvcount
-    int source
-    int recvtag
-    MPI_Datatype recvtype
-    MPI_Comm comm
-    MPI_Status* status
-
-
-cpdef bytes build_sendrecv_descriptor(
-    int sendcount, int dest, int sendtag, uintptr_t sendtype_handle,
-    int recvcount, int source, int recvtag, uintptr_t recvtype_addr,
-    uintptr_t comm_handle, uintptr_t status_addr
-):
-    cdef SendrecvDescriptor desc = SendrecvDescriptor(
-        sendcount, dest, sendtag, <MPI_Datatype> sendtype_handle,
-        recvcount, source, recvtag, <MPI_Datatype> recvtype_addr,
-        <MPI_Comm> comm_handle, <MPI_Status*> status_addr
-    )
-    return bytes((<char*> &desc)[:sizeof(SendrecvDescriptor)])
-
-
 cdef void mpi_sendrecv_gpu(cudaStream_t stream, void** buffers,
                            const char* opaque, size_t opaque_len) nogil:
     cdef int ierr, send_dtype_size, recv_dtype_size
     cdef size_t bytes_send, bytes_recv
 
     # decode inputs
     cdef void* in_buf = buffers[0]
@@ -894,38 +673,38 @@
     cdef int recvcount = desc.recvcount
     cdef int source = desc.source
     cdef int recvtag = desc.recvtag
     cdef MPI_Datatype recvtype = desc.recvtype
     cdef MPI_Comm comm = desc.comm
     cdef MPI_Status* status = desc.status
 
-    checked_cuda_stream_synchronize(stream, comm)
-
     if COPY_TO_HOST:
         # copy memory to host
         ierr = MPI_Type_size(sendtype, &send_dtype_size)
         mpi_xla_bridge.abort_on_error(ierr, comm, u"Type_size")
 
         ierr = MPI_Type_size(recvtype, &recv_dtype_size)
         mpi_xla_bridge.abort_on_error(ierr, comm, u"Type_size")
 
         bytes_send = send_dtype_size * sendcount
         bytes_recv = recv_dtype_size * recvcount
         sendbuf = checked_malloc(bytes_send, comm)
         recvbuf = checked_malloc(bytes_recv, comm)
-        checked_cuda_memcpy(sendbuf, in_buf, bytes_send, cudaMemcpyDeviceToHost, comm)
+        checked_cuda_memcpy(sendbuf, in_buf, bytes_send, cudaMemcpyDeviceToHost, stream, comm)
+    else:
+        checked_cuda_stream_synchronize(stream, comm)
 
     mpi_xla_bridge.mpi_sendrecv(
         sendbuf, sendcount, sendtype, dest, sendtag,
         recvbuf, recvcount, recvtype, source, recvtag,
         comm, status
     )
 
     if COPY_TO_HOST:
-        checked_cuda_memcpy(out_buf, recvbuf, bytes_recv, cudaMemcpyHostToDevice, comm)
+        checked_cuda_memcpy(out_buf, recvbuf, bytes_recv, cudaMemcpyHostToDevice, stream, comm)
         free(recvbuf)
 
 
 gpu_custom_call_targets = {}
 
 cdef register_custom_call_target(fn_name, void* fn):
     cdef const char* name = "xla._CUSTOM_CALL_TARGET"
```

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/__init__.py` & `mpi4jax-0.4.1/mpi4jax/experimental/notoken/__init__.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/allgather.py` & `mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/allgather.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,18 +14,24 @@
     unpack_hashable,
     wrap_as_hashable,
     as_mhlo_constant,
     get_default_layouts,
     ordered_effect,
 )
 from mpi4jax._src.jax_compat import custom_call, token_type, ShapedArray
-from mpi4jax._src.decorators import translation_rule_cpu, translation_rule_gpu
+from mpi4jax._src.decorators import (
+    translation_rule_cpu,
+    translation_rule_gpu,
+    translation_rule_xpu,
+)
 from mpi4jax._src.validation import enforce_types
 from mpi4jax._src.comm import get_default_comm
 
+from mpi4jax._src.xla_bridge.device_descriptors import build_allgather_descriptor
+
 # The Jax primitive
 mpi_allgather_p = Primitive("allgather_mpi")  # Create the primitive
 mpi_allgather_impl = default_primitive_impl(mpi_allgather_p)
 
 
 # This function applies the primitive to an AST
 @enforce_types(
@@ -112,18 +118,15 @@
     results = list(result_obj.results)
     token = results.pop(-1)
     ctx.set_tokens_out(mlir.TokenSet({ordered_effect: (token,)}))
 
     return results
 
 
-@translation_rule_gpu
-def mpi_allgather_xla_encode_gpu(ctx, sendbuf, comm):
-    from mpi4jax._src.xla_bridge.mpi_xla_bridge_gpu import build_allgather_descriptor
-
+def mpi_allgather_xla_encode_device(ctx, sendbuf, comm):
     comm = unpack_hashable(comm)
 
     sendbuf_aval, *_ = ctx.avals_in
     send_nptype = sendbuf_aval.dtype
 
     send_type = ir.RankedTensorType(sendbuf.type)
     send_dtype = send_type.element_type
@@ -169,20 +172,25 @@
     results = list(result_obj.results)
     token = results.pop(-1)
     ctx.set_tokens_out(mlir.TokenSet({ordered_effect: (token,)}))
 
     return results
 
 
+mpi_allgather_xla_encode_xpu = translation_rule_xpu(mpi_allgather_xla_encode_device)
+mpi_allgather_xla_encode_gpu = translation_rule_gpu(mpi_allgather_xla_encode_device)
+
+
 # This function evaluates only the shapes during AST construction
 def mpi_allgather_abstract_eval(x, comm):
     comm = unpack_hashable(comm)
     size = comm.Get_size()
     out_shape = (size, *x.shape)
     return ShapedArray(out_shape, x.dtype), {ordered_effect}
 
 
 mpi_allgather_p.def_impl(mpi_allgather_impl)
 mpi_allgather_p.def_effectful_abstract_eval(mpi_allgather_abstract_eval)
 
 mlir.register_lowering(mpi_allgather_p, mpi_allgather_xla_encode_cpu, platform="cpu")
 mlir.register_lowering(mpi_allgather_p, mpi_allgather_xla_encode_gpu, platform="cuda")
+mlir.register_lowering(mpi_allgather_p, mpi_allgather_xla_encode_xpu, platform="xpu")
```

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/allreduce.py` & `mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/allreduce.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,23 @@
     unpack_hashable,
     wrap_as_hashable,
     as_mhlo_constant,
     get_default_layouts,
     ordered_effect,
 )
 from mpi4jax._src.jax_compat import custom_call, token_type, ShapedArray
-from mpi4jax._src.decorators import translation_rule_cpu, translation_rule_gpu
+from mpi4jax._src.decorators import (
+    translation_rule_cpu,
+    translation_rule_gpu,
+    translation_rule_xpu,
+)
 from mpi4jax._src.validation import enforce_types
 from mpi4jax._src.comm import get_default_comm
 
+from mpi4jax._src.xla_bridge.device_descriptors import build_allreduce_descriptor
 
 # The Jax primitive
 mpi_allreduce_p = Primitive("allreduce_mpi")  # Create the primitive
 mpi_allreduce_impl = default_primitive_impl(mpi_allreduce_p)
 
 
 # This function applies the primitive to an AST
@@ -114,18 +119,15 @@
     results = list(result_obj.results)
     token = results.pop(-1)
     ctx.set_tokens_out(mlir.TokenSet({ordered_effect: (token,)}))
 
     return results
 
 
-@translation_rule_gpu
-def mpi_allreduce_xla_encode_gpu(ctx, x, token, op, comm, transpose):
-    from mpi4jax._src.xla_bridge.mpi_xla_bridge_gpu import build_allreduce_descriptor
-
+def mpi_allreduce_xla_encode_device(ctx, x, token, op, comm, transpose):
     del token  # unused
 
     op = unpack_hashable(op)
     comm = unpack_hashable(comm)
 
     if transpose:
         assert op == _MPI.SUM
@@ -173,14 +175,18 @@
     results = list(result_obj.results)
     token = results.pop(-1)
     ctx.set_tokens_out(mlir.TokenSet({ordered_effect: (token,)}))
 
     return results
 
 
+mpi_allreduce_xla_encode_xpu = translation_rule_xpu(mpi_allreduce_xla_encode_device)
+mpi_allreduce_xla_encode_gpu = translation_rule_gpu(mpi_allreduce_xla_encode_device)
+
+
 # This function evaluates only the shapes during AST construction
 def mpi_allreduce_abstract_eval(xs, token, op, comm, transpose):
     if not transpose:
         return ShapedArray(xs.shape, xs.dtype), {ordered_effect}
     else:
         # The transposition of an allreduce is just the identity, so it can be reordered
         # and does not come with an ordered effect.
@@ -227,7 +233,8 @@
 
 ad.primitive_jvps[mpi_allreduce_p] = mpi_allreduce_value_and_jvp
 ad.primitive_transposes[mpi_allreduce_p] = mpi_allreduce_transpose_rule
 
 # assign to the primitive the correct encoder
 mlir.register_lowering(mpi_allreduce_p, mpi_allreduce_xla_encode_cpu, platform="cpu")
 mlir.register_lowering(mpi_allreduce_p, mpi_allreduce_xla_encode_gpu, platform="cuda")
+mlir.register_lowering(mpi_allreduce_p, mpi_allreduce_xla_encode_xpu, platform="xpu")
```

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/alltoall.py` & `mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/alltoall.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,18 +14,24 @@
     unpack_hashable,
     wrap_as_hashable,
     as_mhlo_constant,
     get_default_layouts,
     ordered_effect,
 )
 from mpi4jax._src.jax_compat import custom_call, token_type, ShapedArray
-from mpi4jax._src.decorators import translation_rule_cpu, translation_rule_gpu
+from mpi4jax._src.decorators import (
+    translation_rule_cpu,
+    translation_rule_gpu,
+    translation_rule_xpu,
+)
 from mpi4jax._src.validation import enforce_types
 from mpi4jax._src.comm import get_default_comm
 
+from mpi4jax._src.xla_bridge.device_descriptors import build_alltoall_descriptor
+
 
 # The Jax primitive
 mpi_alltoall_p = Primitive("alltoall_mpi")  # Create the primitive
 mpi_alltoall_impl = default_primitive_impl(mpi_alltoall_p)
 
 
 # This function applies the primitive to an AST
@@ -113,18 +119,15 @@
     results = list(result_obj.results)
     token = results.pop(-1)
     ctx.set_tokens_out(mlir.TokenSet({ordered_effect: (token,)}))
 
     return results
 
 
-@translation_rule_gpu
-def mpi_alltoall_xla_encode_gpu(ctx, x, comm):
-    from mpi4jax._src.xla_bridge.mpi_xla_bridge_gpu import build_alltoall_descriptor
-
+def mpi_alltoall_xla_encode_device(ctx, x, comm):
     comm = unpack_hashable(comm)
 
     x_aval, *_ = ctx.avals_in
     x_nptype = x_aval.dtype
 
     x_type = ir.RankedTensorType(x.type)
     dtype = x_type.element_type
@@ -171,18 +174,23 @@
 
     results = list(result_obj.results)
     token = results.pop(-1)
     ctx.set_tokens_out(mlir.TokenSet({ordered_effect: (token,)}))
     return results
 
 
+mpi_alltoall_xla_encode_xpu = translation_rule_xpu(mpi_alltoall_xla_encode_device)
+mpi_alltoall_xla_encode_gpu = translation_rule_gpu(mpi_alltoall_xla_encode_device)
+
+
 # This function evaluates only the shapes during AST construction
 def mpi_alltoall_abstract_eval(xs, comm):
     return ShapedArray(xs.shape, xs.dtype), {ordered_effect}
 
 
 mpi_alltoall_p.def_impl(mpi_alltoall_impl)
 mpi_alltoall_p.def_effectful_abstract_eval(mpi_alltoall_abstract_eval)
 
 # assign to the primitive the correct encoder
 mlir.register_lowering(mpi_alltoall_p, mpi_alltoall_xla_encode_cpu, platform="cpu")
 mlir.register_lowering(mpi_alltoall_p, mpi_alltoall_xla_encode_gpu, platform="cuda")
+mlir.register_lowering(mpi_alltoall_p, mpi_alltoall_xla_encode_xpu, platform="xpu")
```

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/barrier.py` & `mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/barrier.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,18 +11,24 @@
     unpack_hashable,
     wrap_as_hashable,
     as_mhlo_constant,
     get_default_layouts,
     ordered_effect,
 )
 from mpi4jax._src.jax_compat import custom_call, token_type
-from mpi4jax._src.decorators import translation_rule_cpu, translation_rule_gpu
+from mpi4jax._src.decorators import (
+    translation_rule_cpu,
+    translation_rule_gpu,
+    translation_rule_xpu,
+)
 from mpi4jax._src.validation import enforce_types
 from mpi4jax._src.comm import get_default_comm
 
+from mpi4jax._src.xla_bridge.device_descriptors import build_barrier_descriptor
+
 
 # The Jax primitive
 mpi_barrier_p = Primitive("barrier_mpi")  # Create the primitive
 mpi_barrier_impl = default_primitive_impl(mpi_barrier_p)
 
 
 # This function applies the primitive to an AST
@@ -72,18 +78,15 @@
     results = list(result_obj.results)
     token = results.pop(-1)
     ctx.set_tokens_out(mlir.TokenSet({ordered_effect: (token,)}))
 
     return results
 
 
-@translation_rule_gpu
-def mpi_barrier_xla_encode_gpu(ctx, comm):
-    from mpi4jax._src.xla_bridge.mpi_xla_bridge_gpu import build_barrier_descriptor
-
+def mpi_barrier_xla_encode_device(ctx, comm):
     comm = unpack_hashable(comm)
 
     out_types = token_type()
 
     token = ctx.tokens_in.get(ordered_effect)[0]
 
     operands = (token,)
@@ -103,14 +106,18 @@
     results = list(result_obj.results)
     token = results.pop(-1)
     ctx.set_tokens_out(mlir.TokenSet({ordered_effect: (token,)}))
 
     return results
 
 
+mpi_barrier_xla_encode_xpu = translation_rule_xpu(mpi_barrier_xla_encode_device)
+mpi_barrier_xla_encode_gpu = translation_rule_gpu(mpi_barrier_xla_encode_device)
+
+
 # This function evaluates only the shapes during AST construction
 def mpi_barrier_abstract_eval(comm):
     return (), {ordered_effect}
 
 
 def mpi_barrier_batch_eval(in_args, batch_axes, comm):
     res = mpi_barrier_p.bind(comm=comm)
@@ -122,7 +129,8 @@
 mpi_barrier_p.def_effectful_abstract_eval(mpi_barrier_abstract_eval)
 
 batching.primitive_batchers[mpi_barrier_p] = mpi_barrier_batch_eval
 
 # assign to the primitive the correct encoder
 mlir.register_lowering(mpi_barrier_p, mpi_barrier_xla_encode_cpu, platform="cpu")
 mlir.register_lowering(mpi_barrier_p, mpi_barrier_xla_encode_gpu, platform="cuda")
+mlir.register_lowering(mpi_barrier_p, mpi_barrier_xla_encode_xpu, platform="xpu")
```

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/bcast.py` & `mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/bcast.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,18 +14,24 @@
     unpack_hashable,
     wrap_as_hashable,
     as_mhlo_constant,
     get_default_layouts,
     ordered_effect,
 )
 from mpi4jax._src.jax_compat import custom_call, token_type, ShapedArray
-from mpi4jax._src.decorators import translation_rule_cpu, translation_rule_gpu
+from mpi4jax._src.decorators import (
+    translation_rule_cpu,
+    translation_rule_gpu,
+    translation_rule_xpu,
+)
 from mpi4jax._src.validation import enforce_types
 from mpi4jax._src.comm import get_default_comm
 
+from mpi4jax._src.xla_bridge.device_descriptors import build_bcast_descriptor
+
 
 # The Jax primitive
 mpi_bcast_p = Primitive("bcast_mpi")  # Create the primitive
 mpi_bcast_impl = default_primitive_impl(mpi_bcast_p)
 
 
 # This function applies the primitive to an AST
@@ -114,18 +120,15 @@
     results = list(result_obj.results)
     token = results.pop(-1)
     ctx.set_tokens_out(mlir.TokenSet({ordered_effect: (token,)}))
 
     return results
 
 
-@translation_rule_gpu
-def mpi_bcast_xla_encode_gpu(ctx, x, root, comm):
-    from mpi4jax._src.xla_bridge.mpi_xla_bridge_gpu import build_bcast_descriptor
-
+def mpi_bcast_xla_encode_device(ctx, x, root, comm):
     comm = unpack_hashable(comm)
 
     x_aval, *_ = ctx.avals_in
     x_nptype = x_aval.dtype
 
     x_type = ir.RankedTensorType(x.type)
     dtype = x_type.element_type
@@ -172,14 +175,18 @@
     results = list(result_obj.results)
     token = results.pop(-1)
     ctx.set_tokens_out(mlir.TokenSet({ordered_effect: (token,)}))
 
     return results
 
 
+mpi_bcast_xla_encode_xpu = translation_rule_xpu(mpi_bcast_xla_encode_device)
+mpi_bcast_xla_encode_gpu = translation_rule_gpu(mpi_bcast_xla_encode_device)
+
+
 # This function evaluates only the shapes during AST construction
 def mpi_bcast_abstract_eval(xs, root, comm):
     comm = unpack_hashable(comm)
     rank = comm.Get_rank()
 
     if rank == root:
         dims = (0,)
@@ -191,7 +198,8 @@
 
 mpi_bcast_p.def_impl(mpi_bcast_impl)
 mpi_bcast_p.def_effectful_abstract_eval(mpi_bcast_abstract_eval)
 
 # assign to the primitive the correct encoder
 mlir.register_lowering(mpi_bcast_p, mpi_bcast_xla_encode_cpu, platform="cpu")
 mlir.register_lowering(mpi_bcast_p, mpi_bcast_xla_encode_gpu, platform="cuda")
+mlir.register_lowering(mpi_bcast_p, mpi_bcast_xla_encode_xpu, platform="xpu")
```

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/gather.py` & `mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/gather.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,23 @@
     unpack_hashable,
     wrap_as_hashable,
     as_mhlo_constant,
     get_default_layouts,
     ordered_effect,
 )
 from mpi4jax._src.jax_compat import custom_call, token_type, ShapedArray
-from mpi4jax._src.decorators import translation_rule_cpu, translation_rule_gpu
+from mpi4jax._src.decorators import (
+    translation_rule_cpu,
+    translation_rule_gpu,
+    translation_rule_xpu,
+)
 from mpi4jax._src.validation import enforce_types
 from mpi4jax._src.comm import get_default_comm
 
+from mpi4jax._src.xla_bridge.device_descriptors import build_gather_descriptor
 
 # The Jax primitive
 mpi_gather_p = Primitive("gather_mpi")  # Create the primitive
 mpi_gather_impl = default_primitive_impl(mpi_gather_p)
 
 
 # This function applies the primitive to an AST
@@ -136,18 +141,15 @@
     results = list(result_obj.results)
     token = results.pop(-1)
     ctx.set_tokens_out(mlir.TokenSet({ordered_effect: (token,)}))
 
     return results
 
 
-@translation_rule_gpu
-def mpi_gather_xla_encode_gpu(ctx, x, root, comm):
-    from mpi4jax._src.xla_bridge.mpi_xla_bridge_gpu import build_gather_descriptor
-
+def mpi_gather_xla_encode_device(ctx, x, root, comm):
     comm = unpack_hashable(comm)
 
     x_aval, *_ = ctx.avals_in
     x_nptype = x_aval.dtype
 
     x_type = ir.RankedTensorType(x.type)
     dtype = x_type.element_type
@@ -203,14 +205,18 @@
     results = list(result_obj.results)
     token = results.pop(-1)
     ctx.set_tokens_out(mlir.TokenSet({ordered_effect: (token,)}))
 
     return results
 
 
+mpi_gather_xla_encode_xpu = translation_rule_xpu(mpi_gather_xla_encode_device)
+mpi_gather_xla_encode_gpu = translation_rule_gpu(mpi_gather_xla_encode_device)
+
+
 # This function evaluates only the shapes during AST construction
 def mpi_gather_abstract_eval(x, root, comm):
     comm = unpack_hashable(comm)
     rank = comm.Get_rank()
     size = comm.Get_size()
 
     if rank == root:
@@ -223,7 +229,8 @@
 
 mpi_gather_p.def_impl(mpi_gather_impl)
 mpi_gather_p.def_effectful_abstract_eval(mpi_gather_abstract_eval)
 
 # assign to the primitive the correct encoder
 mlir.register_lowering(mpi_gather_p, mpi_gather_xla_encode_cpu, platform="cpu")
 mlir.register_lowering(mpi_gather_p, mpi_gather_xla_encode_gpu, platform="cuda")
+mlir.register_lowering(mpi_gather_p, mpi_gather_xla_encode_xpu, platform="xpu")
```

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/recv.py` & `mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/recv.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,18 +15,24 @@
     unpack_hashable,
     wrap_as_hashable,
     as_mhlo_constant,
     get_default_layouts,
     ordered_effect,
 )
 from mpi4jax._src.jax_compat import custom_call, token_type, ShapedArray
-from mpi4jax._src.decorators import translation_rule_cpu, translation_rule_gpu
+from mpi4jax._src.decorators import (
+    translation_rule_cpu,
+    translation_rule_gpu,
+    translation_rule_xpu,
+)
 from mpi4jax._src.validation import enforce_types
 from mpi4jax._src.comm import get_default_comm
 
+from mpi4jax._src.xla_bridge.device_descriptors import build_recv_descriptor
+
 
 # The Jax primitive
 mpi_recv_p = Primitive("recv_mpi")  # Create the primitive
 mpi_recv_impl = default_primitive_impl(mpi_recv_p)
 
 
 # This function applies the primitive to an AST
@@ -126,18 +132,16 @@
     results = list(result_obj.results)
     token = results.pop(-1)
     ctx.set_tokens_out(mlir.TokenSet({ordered_effect: (token,)}))
 
     return results
 
 
-@translation_rule_gpu
-def mpi_recv_xla_encode_gpu(ctx, x, source, tag, comm, status):
+def mpi_recv_xla_encode_device(ctx, x, source, tag, comm, status):
     from mpi4jax._src.xla_bridge.mpi_xla_bridge import MPI_STATUS_IGNORE_ADDR
-    from mpi4jax._src.xla_bridge.mpi_xla_bridge_gpu import build_recv_descriptor
 
     comm = unpack_hashable(comm)
     status = unpack_hashable(status)
 
     x_aval, *_ = ctx.avals_in
     x_nptype = x_aval.dtype
 
@@ -185,18 +189,23 @@
     results = list(result_obj.results)
     token = results.pop(-1)
     ctx.set_tokens_out(mlir.TokenSet({ordered_effect: (token,)}))
 
     return results
 
 
+mpi_recv_xla_encode_xpu = translation_rule_xpu(mpi_recv_xla_encode_device)
+mpi_recv_xla_encode_gpu = translation_rule_gpu(mpi_recv_xla_encode_device)
+
+
 # This function evaluates only the shapes during AST construction
 def mpi_recv_abstract_eval(xs, source, tag, comm, status):
     return ShapedArray(xs.shape, xs.dtype), {ordered_effect}
 
 
 mpi_recv_p.def_impl(mpi_recv_impl)
 mpi_recv_p.def_effectful_abstract_eval(mpi_recv_abstract_eval)
 
 # assign to the primitive the correct encoder
 mlir.register_lowering(mpi_recv_p, mpi_recv_xla_encode_cpu, platform="cpu")
 mlir.register_lowering(mpi_recv_p, mpi_recv_xla_encode_gpu, platform="cuda")
+mlir.register_lowering(mpi_recv_p, mpi_recv_xla_encode_xpu, platform="xpu")
```

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/reduce.py` & `mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/reduce.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,18 +14,23 @@
     unpack_hashable,
     wrap_as_hashable,
     as_mhlo_constant,
     get_default_layouts,
     ordered_effect,
 )
 from mpi4jax._src.jax_compat import custom_call, token_type, ShapedArray
-from mpi4jax._src.decorators import translation_rule_cpu, translation_rule_gpu
+from mpi4jax._src.decorators import (
+    translation_rule_cpu,
+    translation_rule_gpu,
+    translation_rule_xpu,
+)
 from mpi4jax._src.validation import enforce_types
 from mpi4jax._src.comm import get_default_comm
 
+from mpi4jax._src.xla_bridge.device_descriptors import build_reduce_descriptor
 
 # The Jax primitive
 mpi_reduce_p = Primitive("reduce_mpi")  # Create the primitive
 mpi_reduce_impl = default_primitive_impl(mpi_reduce_p)
 
 
 # This function applies the primitive to an AST
@@ -117,18 +122,15 @@
     results = list(result_obj.results)
     token = results.pop(-1)
     ctx.set_tokens_out(mlir.TokenSet({ordered_effect: (token,)}))
 
     return results
 
 
-@translation_rule_gpu
-def mpi_reduce_xla_encode_gpu(ctx, x, op, root, comm):
-    from mpi4jax._src.xla_bridge.mpi_xla_bridge_gpu import build_reduce_descriptor
-
+def mpi_reduce_xla_encode_device(ctx, x, op, root, comm):
     op = unpack_hashable(op)
     comm = unpack_hashable(comm)
 
     x_aval, *_ = ctx.avals_in
     x_nptype = x_aval.dtype
 
     x_type = ir.RankedTensorType(x.type)
@@ -179,14 +181,18 @@
     results = list(result_obj.results)
     token = results.pop(-1)
     ctx.set_tokens_out(mlir.TokenSet({ordered_effect: (token,)}))
 
     return results
 
 
+mpi_reduce_xla_encode_xpu = translation_rule_xpu(mpi_reduce_xla_encode_device)
+mpi_reduce_xla_encode_gpu = translation_rule_gpu(mpi_reduce_xla_encode_device)
+
+
 # This function evaluates only the shapes during AST construction
 def mpi_reduce_abstract_eval(xs, op, root, comm):
     comm = unpack_hashable(comm)
     rank = comm.Get_rank()
 
     if rank != root:
         dims = (0,)
@@ -198,7 +204,8 @@
 
 mpi_reduce_p.def_impl(mpi_reduce_impl)
 mpi_reduce_p.def_effectful_abstract_eval(mpi_reduce_abstract_eval)
 
 # assign to the primitive the correct encoder
 mlir.register_lowering(mpi_reduce_p, mpi_reduce_xla_encode_cpu, platform="cpu")
 mlir.register_lowering(mpi_reduce_p, mpi_reduce_xla_encode_gpu, platform="cuda")
+mlir.register_lowering(mpi_reduce_p, mpi_reduce_xla_encode_xpu, platform="xpu")
```

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/scan.py` & `mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/scan.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,18 +14,24 @@
     unpack_hashable,
     wrap_as_hashable,
     as_mhlo_constant,
     get_default_layouts,
     ordered_effect,
 )
 from mpi4jax._src.jax_compat import custom_call, token_type, ShapedArray
-from mpi4jax._src.decorators import translation_rule_cpu, translation_rule_gpu
+from mpi4jax._src.decorators import (
+    translation_rule_cpu,
+    translation_rule_gpu,
+    translation_rule_xpu,
+)
 from mpi4jax._src.validation import enforce_types
 from mpi4jax._src.comm import get_default_comm
 
+from mpi4jax._src.xla_bridge.device_descriptors import build_scan_descriptor
+
 
 # The Jax primitive
 mpi_scan_p = Primitive("scan_mpi")  # Create the primitive
 mpi_scan_impl = default_primitive_impl(mpi_scan_p)
 
 
 # This function applies the primitive to an AST
@@ -99,18 +105,15 @@
     results = list(result_obj.results)
     token = results.pop(-1)
     ctx.set_tokens_out(mlir.TokenSet({ordered_effect: (token,)}))
 
     return results
 
 
-@translation_rule_gpu
-def mpi_scan_xla_encode_gpu(ctx, x, op, comm):
-    from mpi4jax._src.xla_bridge.mpi_xla_bridge_gpu import build_scan_descriptor
-
+def mpi_scan_xla_encode_device(ctx, x, op, comm):
     op = unpack_hashable(op)
     comm = unpack_hashable(comm)
 
     x_aval, *_ = ctx.avals_in
     x_nptype = x_aval.dtype
 
     x_type = ir.RankedTensorType(x.type)
@@ -154,18 +157,23 @@
     results = list(result_obj.results)
     token = results.pop(-1)
     ctx.set_tokens_out(mlir.TokenSet({ordered_effect: (token,)}))
 
     return results
 
 
+mpi_scan_xla_encode_xpu = translation_rule_xpu(mpi_scan_xla_encode_device)
+mpi_scan_xla_encode_gpu = translation_rule_gpu(mpi_scan_xla_encode_device)
+
+
 # This function evaluates only the shapes during AST construction
 def mpi_scan_abstract_eval(xs, op, comm):
     return ShapedArray(xs.shape, xs.dtype), {ordered_effect}
 
 
 mpi_scan_p.def_impl(mpi_scan_impl)
 mpi_scan_p.def_effectful_abstract_eval(mpi_scan_abstract_eval)
 
 # assign to the primitive the correct encoder
 mlir.register_lowering(mpi_scan_p, mpi_scan_xla_encode_cpu, platform="cpu")
 mlir.register_lowering(mpi_scan_p, mpi_scan_xla_encode_gpu, platform="cuda")
+mlir.register_lowering(mpi_scan_p, mpi_scan_xla_encode_xpu, platform="xpu")
```

### Comparing `mpi4jax-0.4.0.post6/mpi4jax/experimental/notoken/collective_ops/sendrecv.py` & `mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/sendrecv.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,18 +17,24 @@
     unpack_hashable,
     wrap_as_hashable,
     as_mhlo_constant,
     get_default_layouts,
     ordered_effect,
 )
 from mpi4jax._src.jax_compat import custom_call, token_type, ShapedArray
-from mpi4jax._src.decorators import translation_rule_cpu, translation_rule_gpu
+from mpi4jax._src.decorators import (
+    translation_rule_cpu,
+    translation_rule_gpu,
+    translation_rule_xpu,
+)
 from mpi4jax._src.validation import enforce_types
 from mpi4jax._src.comm import get_default_comm
 
+from mpi4jax._src.xla_bridge.device_descriptors import build_sendrecv_descriptor
+
 
 # The Jax primitive
 mpi_sendrecv_p = Primitive("sendrecv_mpi")  # Create the primitive
 mpi_sendrecv_impl = default_primitive_impl(mpi_sendrecv_p)
 
 
 # This function applies the primitive to an AST
@@ -188,37 +194,35 @@
     results = list(result_obj.results)
     token = results.pop(-1)
     ctx.set_tokens_out(mlir.TokenSet({ordered_effect: (token,)}))
 
     return results
 
 
-@translation_rule_gpu
-def mpi_sendrecv_xla_encode_gpu(
+def mpi_sendrecv_xla_encode_device(
     ctx,
     sendbuf,
     recvbuf,
     token,
     source,
     dest,
     sendtag,
     recvtag,
     comm,
     status,
-    _must_transpose=False,
+    _must_transpose,
 ):
     if _must_transpose:
         raise RuntimeError(
             "sendrecv cannot be used with forward-mode (vjp) autodiff, because "
             "the gradient might be located on a different mpi rank than the "
             "desired one. Use reverse-mode (jvp) differentiation instead."
         )
 
     from mpi4jax._src.xla_bridge.mpi_xla_bridge import MPI_STATUS_IGNORE_ADDR
-    from mpi4jax._src.xla_bridge.mpi_xla_bridge_gpu import build_sendrecv_descriptor
 
     del token  # unused
 
     comm = unpack_hashable(comm)
     status = unpack_hashable(status)
 
     send_aval, recv_aval, *_ = ctx.avals_in
@@ -282,14 +286,72 @@
     results = list(result_obj.results)
     token = results.pop(-1)
     ctx.set_tokens_out(mlir.TokenSet({ordered_effect: (token,)}))
 
     return results
 
 
+@translation_rule_xpu
+def mpi_sendrecv_xla_encode_xpu(
+    ctx,
+    sendbuf,
+    recvbuf,
+    token,
+    source,
+    dest,
+    sendtag,
+    recvtag,
+    comm,
+    status,
+    _must_transpose=False,
+):
+    return mpi_sendrecv_xla_encode_device(
+        ctx,
+        sendbuf,
+        recvbuf,
+        token,
+        source,
+        dest,
+        sendtag,
+        recvtag,
+        comm,
+        status,
+        _must_transpose,
+    )
+
+
+@translation_rule_gpu
+def mpi_sendrecv_xla_encode_gpu(
+    ctx,
+    sendbuf,
+    recvbuf,
+    token,
+    source,
+    dest,
+    sendtag,
+    recvtag,
+    comm,
+    status,
+    _must_transpose=False,
+):
+    return mpi_sendrecv_xla_encode_device(
+        ctx,
+        sendbuf,
+        recvbuf,
+        token,
+        source,
+        dest,
+        sendtag,
+        recvtag,
+        comm,
+        status,
+        _must_transpose,
+    )
+
+
 # This function evaluates only the shapes during AST construction
 def mpi_sendrecv_abstract_eval(
     sendbuf,
     recvbuf,
     token,
     source,
     dest,
@@ -404,7 +466,8 @@
 
 ad.primitive_jvps[mpi_sendrecv_p] = mpi_sendrecv_value_and_jvp
 ad.primitive_transposes[mpi_sendrecv_p] = mpi_sendrecv_transpose_rule
 
 # assign to the primitive the correct encoder
 mlir.register_lowering(mpi_sendrecv_p, mpi_sendrecv_xla_encode_cpu, platform="cpu")
 mlir.register_lowering(mpi_sendrecv_p, mpi_sendrecv_xla_encode_gpu, platform="cuda")
+mlir.register_lowering(mpi_sendrecv_p, mpi_sendrecv_xla_encode_xpu, platform="xpu")
```

### Comparing `mpi4jax-0.4.0.post6/mpi4jax.egg-info/PKG-INFO` & `mpi4jax-0.4.1/mpi4jax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpi4jax
-Version: 0.4.0.post6
+Version: 0.4.1
 Summary: Zero-copy MPI communication of JAX arrays, for turbo-charged HPC applications in Python ⚡
 Home-page: https://github.com/mpi4jax/mpi4jax
 Author: Filippo Vicentini
 Author-email: filippovicentini@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Cython
```

### Comparing `mpi4jax-0.4.0.post6/mpi4jax.egg-info/SOURCES.txt` & `mpi4jax-0.4.1/mpi4jax.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -33,18 +33,22 @@
 mpi4jax/_src/collective_ops/reduce.py
 mpi4jax/_src/collective_ops/scan.py
 mpi4jax/_src/collective_ops/scatter.py
 mpi4jax/_src/collective_ops/send.py
 mpi4jax/_src/collective_ops/sendrecv.py
 mpi4jax/_src/xla_bridge/__init__.py
 mpi4jax/_src/xla_bridge/cuda_runtime_api.pxd
+mpi4jax/_src/xla_bridge/device_descriptors.pxd
+mpi4jax/_src/xla_bridge/device_descriptors.pyx
 mpi4jax/_src/xla_bridge/mpi_xla_bridge.pxd
 mpi4jax/_src/xla_bridge/mpi_xla_bridge.pyx
 mpi4jax/_src/xla_bridge/mpi_xla_bridge_cpu.pyx
 mpi4jax/_src/xla_bridge/mpi_xla_bridge_gpu.pyx
+mpi4jax/_src/xla_bridge/mpi_xla_bridge_xpu.pyx
+mpi4jax/_src/xla_bridge/sycl_runtime_api.pxd
 mpi4jax/experimental/__init__.py
 mpi4jax/experimental/notoken/__init__.py
 mpi4jax/experimental/notoken/collective_ops/__init__.py
 mpi4jax/experimental/notoken/collective_ops/allgather.py
 mpi4jax/experimental/notoken/collective_ops/allreduce.py
 mpi4jax/experimental/notoken/collective_ops/alltoall.py
 mpi4jax/experimental/notoken/collective_ops/barrier.py
@@ -57,14 +61,15 @@
 mpi4jax/experimental/notoken/collective_ops/send.py
 mpi4jax/experimental/notoken/collective_ops/sendrecv.py
 tests/conftest.py
 tests/test_decorators.py
 tests/test_examples.py
 tests/test_flush.py
 tests/test_has_cuda.py
+tests/test_has_sycl.py
 tests/test_jax_compat.py
 tests/test_validation.py
 tests/collective_ops/test_allgather.py
 tests/collective_ops/test_allreduce.py
 tests/collective_ops/test_allreduce_matvec.py
 tests/collective_ops/test_alltoall.py
 tests/collective_ops/test_barrier.py
```

### Comparing `mpi4jax-0.4.0.post6/pyproject.toml` & `mpi4jax-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post6/setup.py` & `mpi4jax-0.4.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -119,14 +119,60 @@
         _cuda_path = "/usr/local/cuda"
     else:
         _cuda_path = None
 
     return _cuda_path
 
 
+def get_sycl_path():
+    sycl_path = os.getenv("CMPLR_ROOT", "")
+    if len(sycl_path) > 0 and os.path.exists(sycl_path):
+        _sycl_path = sycl_path
+    elif os.path.exists("/opt/intel/oneapi/compiler/latest/"):
+        _sycl_path = "/opt/intel/oneapi/compiler/latest/"
+    else:
+        _sycl_path = None
+
+    return _sycl_path
+
+
+def get_sycl_info():
+    sycl_info = {"compile": [], "libdirs": [], "libs": []}
+    sycl_path = get_sycl_path()
+    if not sycl_path:
+        return sycl_info
+
+    include_suffixes = [
+        "linux/include/",
+        "linux/include/sycl",
+        "include/",
+        "include/sycl",
+    ]
+
+    for inc_suffix in include_suffixes:
+        incdir = os.path.join(sycl_path, inc_suffix)
+        if os.path.isdir(incdir):
+            sycl_info["compile"].append(incdir)
+
+    libdir_suffixes = [
+        "linux/lib/",
+        "lib/",
+    ]
+    for libdir_suffix in libdir_suffixes:
+        lib_dir = os.path.join(sycl_path, libdir_suffix)
+        if os.path.isdir(lib_dir):
+            sycl_info["libdirs"].append(lib_dir)
+
+    sycl_info["libs"].append("sycl")
+    return sycl_info
+
+
+sycl_info = get_sycl_info()
+
+
 def get_cuda_info():
     cuda_info = {"compile": [], "libdirs": [], "libs": []}
     cuda_path = get_cuda_path()
     if not cuda_path:
         return cuda_info
 
     incdir = os.path.join(cuda_path, "include")
@@ -163,17 +209,37 @@
             return []
 
     extensions = [
         Extension(
             name=f"{CYTHON_SUBMODULE_NAME}.{mod}",
             sources=[f"{CYTHON_SUBMODULE_PATH}/{mod}.pyx"],
         )
-        for mod in ("mpi_xla_bridge", "mpi_xla_bridge_cpu")
+        for mod in ("mpi_xla_bridge", "mpi_xla_bridge_cpu", "device_descriptors")
     ]
 
+    if sycl_info["compile"] and sycl_info["libdirs"]:
+        extensions.append(
+            Extension(
+                name=f"{CYTHON_SUBMODULE_NAME}.mpi_xla_bridge_xpu",
+                sources=[f"{CYTHON_SUBMODULE_PATH}/mpi_xla_bridge_xpu.pyx"],
+                include_dirs=sycl_info["compile"],
+                library_dirs=sycl_info["libdirs"],
+                libraries=sycl_info["libs"],
+                language="c++",
+                # This macro instructs C++ compiler to ignore potential existence of
+                # OpenMPI C++ bindings which are deprecated
+                define_macros=[("OMPI_SKIP_MPICXX", "1")],
+            )
+        )
+    else:
+        print_warning(
+            "SYCL (Intel Basekit) path not found",
+            "(XPU extensions will not be built)",
+        )
+
     if cuda_info["compile"] and cuda_info["libdirs"]:
         extensions.append(
             Extension(
                 name=f"{CYTHON_SUBMODULE_NAME}.mpi_xla_bridge_gpu",
                 sources=[f"{CYTHON_SUBMODULE_PATH}/mpi_xla_bridge_gpu.pyx"],
                 include_dirs=cuda_info["compile"],
                 library_dirs=cuda_info["libdirs"],
```

### Comparing `mpi4jax-0.4.0.post6/tests/collective_ops/test_allgather.py` & `mpi4jax-0.4.1/tests/collective_ops/test_allgather.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post6/tests/collective_ops/test_allreduce.py` & `mpi4jax-0.4.1/tests/collective_ops/test_allreduce.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post6/tests/collective_ops/test_allreduce_matvec.py` & `mpi4jax-0.4.1/tests/collective_ops/test_allreduce_matvec.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post6/tests/collective_ops/test_alltoall.py` & `mpi4jax-0.4.1/tests/collective_ops/test_alltoall.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post6/tests/collective_ops/test_barrier.py` & `mpi4jax-0.4.1/tests/collective_ops/test_barrier.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post6/tests/collective_ops/test_bcast.py` & `mpi4jax-0.4.1/tests/collective_ops/test_bcast.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post6/tests/collective_ops/test_common.py` & `mpi4jax-0.4.1/tests/collective_ops/test_common.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post6/tests/collective_ops/test_gather.py` & `mpi4jax-0.4.1/tests/collective_ops/test_gather.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post6/tests/collective_ops/test_reduce.py` & `mpi4jax-0.4.1/tests/collective_ops/test_reduce.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post6/tests/collective_ops/test_scan.py` & `mpi4jax-0.4.1/tests/collective_ops/test_scan.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post6/tests/collective_ops/test_scatter.py` & `mpi4jax-0.4.1/tests/collective_ops/test_scatter.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post6/tests/collective_ops/test_send_and_recv.py` & `mpi4jax-0.4.1/tests/collective_ops/test_send_and_recv.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post6/tests/collective_ops/test_sendrecv.py` & `mpi4jax-0.4.1/tests/collective_ops/test_sendrecv.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post6/tests/experimental/test_notoken.py` & `mpi4jax-0.4.1/tests/experimental/test_notoken.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post6/tests/test_jax_compat.py` & `mpi4jax-0.4.1/tests/test_jax_compat.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post6/tests/test_validation.py` & `mpi4jax-0.4.1/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.0.post6/versioneer.py` & `mpi4jax-0.4.1/versioneer.py`

 * *Files identical despite different names*

