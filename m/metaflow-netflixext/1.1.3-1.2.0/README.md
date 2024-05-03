# Comparing `tmp/metaflow-netflixext-1.1.3.tar.gz` & `tmp/metaflow_netflixext-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaflow-netflixext-1.1.3.tar", last modified: Fri Apr  5 17:20:01 2024, max compression
+gzip compressed data, was "metaflow_netflixext-1.2.0.tar", last modified: Fri May  3 22:25:14 2024, max compression
```

## Comparing `metaflow-netflixext-1.1.3.tar` & `metaflow_netflixext-1.2.0.tar`

### file list

```diff
@@ -1,55 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:20:01.131744 metaflow-netflixext-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21928 2024-04-05 17:20:01.131744 metaflow-netflixext-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20875 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:20:01.119743 metaflow-netflixext-1.1.3/metaflow_extensions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:20:01.123743 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:20:01.123743 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/cmd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:20:01.123743 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/cmd/environment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/cmd/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44627 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/cmd/environment/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/cmd/mfextinit_netflixext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:20:01.123743 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/config/
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py
--rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/generate_vendor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:20:01.123743 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:20:01.127744 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   113856 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/conda.py
--rw-r--r--   0 runner    (1001) docker     (127)    12125 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/conda_common_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    27127 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    26543 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    51887 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py
--rw-r--r--   0 runner    (1001) docker     (127)    40232 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/envsresolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    13695 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/pypi_package_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:20:01.127744 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resolvers/
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resolvers/builder_envs_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    16754 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resolvers/conda_lock_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resolvers/conda_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resolvers/micromamba_server_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    26246 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resolvers/pip_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:20:01.127744 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png
--rw-r--r--   0 runner    (1001) docker     (127)     9605 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg
--rw-r--r--   0 runner    (1001) docker     (127)   113678 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py
--rw-r--r--   0 runner    (1001) docker     (127)    29074 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22504 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/environment_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/mfextinit_netflixext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:20:01.127744 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/toplevel/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/toplevel/mfextinit_netflixext.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/toplevel/netflixext_toplevel.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/toplevel/netflixext_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:20:01.131744 metaflow-netflixext-1.1.3/metaflow_netflixext.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21928 2024-04-05 17:20:01.000000 metaflow-netflixext-1.1.3/metaflow_netflixext.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-05 17:20:01.000000 metaflow-netflixext-1.1.3/metaflow_netflixext.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 17:20:01.000000 metaflow-netflixext-1.1.3/metaflow_netflixext.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 17:20:01.000000 metaflow-netflixext-1.1.3/metaflow_netflixext.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-05 17:20:01.000000 metaflow-netflixext-1.1.3/metaflow_netflixext.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 17:20:01.131744 metaflow-netflixext-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-05 17:19:53.000000 metaflow-netflixext-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:14.123700 metaflow_netflixext-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    25447 2024-05-03 22:25:14.123700 metaflow_netflixext-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24394 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:14.111700 metaflow_netflixext-1.2.0/metaflow_extensions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:14.111700 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:14.111700 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/cmd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:14.115700 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/cmd/debug/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/cmd/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12681 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/cmd/debug/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/cmd/debug/current_stub_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9703 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/cmd/debug/debug_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16427 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/cmd/debug/debug_script_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/cmd/debug/debug_stub_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/cmd/debug/debug_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/cmd/debug/jupyter_instructions_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/cmd/debug/jupyter_title_markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:14.115700 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/cmd/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/cmd/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44627 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/cmd/environment/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/cmd/mfextinit_netflixext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:14.115700 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/generate_vendor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:14.115700 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:14.119700 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   113856 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12125 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda_common_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26942 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26543 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52295 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40232 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/envsresolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13695 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/pypi_package_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:14.119700 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/resolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/resolvers/builder_envs_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16754 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/resolvers/conda_lock_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/resolvers/conda_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/resolvers/micromamba_server_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26564 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/resolvers/pip_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:14.119700 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9605 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   113678 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29074 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22504 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/environment_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/mfextinit_netflixext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:14.119700 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/toplevel/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/toplevel/mfextinit_netflixext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/toplevel/netflixext_toplevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/toplevel/netflixext_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:14.123700 metaflow_netflixext-1.2.0/metaflow_netflixext.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25447 2024-05-03 22:25:14.000000 metaflow_netflixext-1.2.0/metaflow_netflixext.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-03 22:25:14.000000 metaflow_netflixext-1.2.0/metaflow_netflixext.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 22:25:14.000000 metaflow_netflixext-1.2.0/metaflow_netflixext.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 22:25:14.000000 metaflow_netflixext-1.2.0/metaflow_netflixext.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-03 22:25:14.000000 metaflow_netflixext-1.2.0/metaflow_netflixext.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 22:25:14.123700 metaflow_netflixext-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-03 22:25:06.000000 metaflow_netflixext-1.2.0/setup.py
```

### Comparing `metaflow-netflixext-1.1.3/LICENSE` & `metaflow_netflixext-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.3/PKG-INFO` & `metaflow_netflixext-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow-netflixext
-Version: 1.1.3
+Version: 1.2.0
 Summary: Metaflow extensions from Netflix
 Author: Netflix Metaflow Developers
 Author-email: metaflow-dev@netflix.com
 License: Apache Software License
 Project-URL: Source, https://github.com/Netflix/metaflow-nflx-extensions
 Project-URL: Tracker, https://github.com/Netflix/metaflow-nflx-extensions/issues
 Classifier: Development Status :: 5 - Production/Stable
@@ -52,14 +52,15 @@
 This extension is currently tested on python 3.7+.
 
 If you have any question, feel free to open an issue here or contact us on the usual
 Metaflow slack channels.
 
 This extension currently contains:
 - refactored and improved [Conda decorator](#conda-v2)
+- improved [debugging capability](#debug)
 
 ## Conda V2
 
 *Version 1.0.0 is considered stable. Some UX changes have occurred compared to previous
 versions. Please see the [docs](https://github.com/Netflix/metaflow-nflx-extensions/blob/main/docs/conda.md) for more information*
 
 *Version 0.2.0 of this extension is not fully backward compatible with previous versions due to
@@ -392,7 +393,90 @@
 - remotely:
   - Environment descriptiosn are also stored remotely and can be fetched to be added
     to the local `conda_v2.cnd` file.
   - Packages are stored as archived and may be downloaded in the `pkgs` directory. The
     implementation takes care of properly updating the `urls.txt` file to make it
     transparent to Conda (allowing it to operate in an "offline" mode effectively).
 
+## Debug
+This extension allows user's to seamlessly debug their executed steps in an isolated Jupyter notebook instance
+with appropriate dependencies by leveraging the conda extension described above (note, this extension currently only
+works with the version of Conda in this package). 
+
+### Executing the command
+Let's say you have a step called `fit_gbrt_for_given_param` in your flow, and on executing it, the pathspec for
+this step/task is `HousePricePredictionFlow/1199/fit_gbrt_for_given_param/150671013`. To debug this step, you can run the command:
+
+```bash
+metaflow debug task <HousePricePredictionFlow/1199/fit_gbrt_for_given_param/150671013> --metaflow-root-dir ~/notebooks/debug_task`
+```
+
+Note that you can specify a partial pathspec as long as it can be resolved to a unique task:
+
+- if you specify just a flow name, it will use the latest run in your namespace and the end step
+- if you specify just a run pathspec, it will use the end step
+- if you specify just a step pathspec, it will use the unique task for that step and error if there are more than one tasks (foreach)
+
+### Using the extension
+Running the above command will:
+
+- download your code package
+- download the appropriate conda/pip packages defined for that particular step (if you use the conda extension)
+- generate stubs to access the relevant artifacts for that particular run.
+
+It will additionally generate a notebook in the defined directory where you can debug the execution of your step line by line. For the given step definition:
+```python
+@step
+def fit_gbrt_for_given_param(self):
+    """
+    Fit GBRT with given parameters
+    """
+
+    from sklearn import ensemble
+    from sklearn.model_selection import cross_val_score
+    import numpy as np
+
+
+    estimator = ensemble.GradientBoostingRegressor( n_estimators = self.input['n_estimators'], learning_rate = self.input['learning_rate'],
+        max_depth = self.input['max_depth'], min_samples_split = 2, loss = 'ls')
+
+    estimator.fit(self.features, self.labels)
+
+    mses = cross_val_score(estimator, self.features, self.labels, cv = 5, scoring='neg_mean_squared_error')
+    rmse = np.sqrt(-mses).mean()
+
+
+    self.fit = dict(
+        index=int(self.index),
+        params=self.input,
+        rmse=rmse,
+        estimator=estimator
+    )
+
+    self.next(self.select_best_model)
+```
+
+You will be able to access the artifacts/inputs in your generated notebook directly:
+```python
+>>> print(self.input['n_estimators'])  # You can access objects using `self` as we imported a stub for it in the notebook
+>>> print(self.input['learning_rate'])
+```
+
+You can also execute the whole function again:
+```python
+>>> from sklearn import ensemble  # imports work seamlessly due to conda extension
+>>> from sklearn.model_selection import cross_val_score
+>>> import numpy as np
+>>> estimator = ensemble.GradientBoostingRegressor( n_estimators = self.input['n_estimators'], learning_rate = self.input['learning_rate'],
+    max_depth = self.input['max_depth'], min_samples_split = 2, loss = 'ls')
+>>> estimator.fit(self.features, self.labels)
+>>> mses = cross_val_score(estimator, self.features, self.labels, cv = 5, scoring='neg_mean_squared_error')
+>>> rmse = np.sqrt(-mses).mean()
+>>> self.fit = dict(
+    index=int(self.index),
+    params=self.input,
+    rmse=rmse,
+    estimator=estimator
+)
+```
+
+You can examine the effects of other hyper-parameters live by modifying the `min_samples_split = 3` and re-executing the steps on the same data.
```

### Comparing `metaflow-netflixext-1.1.3/README.md` & `metaflow_netflixext-1.2.0/metaflow_netflixext.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: metaflow-netflixext
+Version: 1.2.0
+Summary: Metaflow extensions from Netflix
+Author: Netflix Metaflow Developers
+Author-email: metaflow-dev@netflix.com
+License: Apache Software License
+Project-URL: Source, https://github.com/Netflix/metaflow-nflx-extensions
+Project-URL: Tracker, https://github.com/Netflix/metaflow-nflx-extensions/issues
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.7.2
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: metaflow>=2.10.0
+
 # Metaflow Extensions from Netflix
 This repository contains extensions for Metaflow that are in use at Netflix (or being tested
 at Netflix) and that are more cutting edge than what is included in the OSS Metaflow package.
 
 You can find support for this extension on the usual Metaflow [Slack](http://slack.outerbounds.co).
 
 NOTE: of you are within Netflix and are looking for the Netflix version of Metaflow,
@@ -27,14 +52,15 @@
 This extension is currently tested on python 3.7+.
 
 If you have any question, feel free to open an issue here or contact us on the usual
 Metaflow slack channels.
 
 This extension currently contains:
 - refactored and improved [Conda decorator](#conda-v2)
+- improved [debugging capability](#debug)
 
 ## Conda V2
 
 *Version 1.0.0 is considered stable. Some UX changes have occurred compared to previous
 versions. Please see the [docs](https://github.com/Netflix/metaflow-nflx-extensions/blob/main/docs/conda.md) for more information*
 
 *Version 0.2.0 of this extension is not fully backward compatible with previous versions due to
@@ -367,7 +393,90 @@
 - remotely:
   - Environment descriptiosn are also stored remotely and can be fetched to be added
     to the local `conda_v2.cnd` file.
   - Packages are stored as archived and may be downloaded in the `pkgs` directory. The
     implementation takes care of properly updating the `urls.txt` file to make it
     transparent to Conda (allowing it to operate in an "offline" mode effectively).
 
+## Debug
+This extension allows user's to seamlessly debug their executed steps in an isolated Jupyter notebook instance
+with appropriate dependencies by leveraging the conda extension described above (note, this extension currently only
+works with the version of Conda in this package). 
+
+### Executing the command
+Let's say you have a step called `fit_gbrt_for_given_param` in your flow, and on executing it, the pathspec for
+this step/task is `HousePricePredictionFlow/1199/fit_gbrt_for_given_param/150671013`. To debug this step, you can run the command:
+
+```bash
+metaflow debug task <HousePricePredictionFlow/1199/fit_gbrt_for_given_param/150671013> --metaflow-root-dir ~/notebooks/debug_task`
+```
+
+Note that you can specify a partial pathspec as long as it can be resolved to a unique task:
+
+- if you specify just a flow name, it will use the latest run in your namespace and the end step
+- if you specify just a run pathspec, it will use the end step
+- if you specify just a step pathspec, it will use the unique task for that step and error if there are more than one tasks (foreach)
+
+### Using the extension
+Running the above command will:
+
+- download your code package
+- download the appropriate conda/pip packages defined for that particular step (if you use the conda extension)
+- generate stubs to access the relevant artifacts for that particular run.
+
+It will additionally generate a notebook in the defined directory where you can debug the execution of your step line by line. For the given step definition:
+```python
+@step
+def fit_gbrt_for_given_param(self):
+    """
+    Fit GBRT with given parameters
+    """
+
+    from sklearn import ensemble
+    from sklearn.model_selection import cross_val_score
+    import numpy as np
+
+
+    estimator = ensemble.GradientBoostingRegressor( n_estimators = self.input['n_estimators'], learning_rate = self.input['learning_rate'],
+        max_depth = self.input['max_depth'], min_samples_split = 2, loss = 'ls')
+
+    estimator.fit(self.features, self.labels)
+
+    mses = cross_val_score(estimator, self.features, self.labels, cv = 5, scoring='neg_mean_squared_error')
+    rmse = np.sqrt(-mses).mean()
+
+
+    self.fit = dict(
+        index=int(self.index),
+        params=self.input,
+        rmse=rmse,
+        estimator=estimator
+    )
+
+    self.next(self.select_best_model)
+```
+
+You will be able to access the artifacts/inputs in your generated notebook directly:
+```python
+>>> print(self.input['n_estimators'])  # You can access objects using `self` as we imported a stub for it in the notebook
+>>> print(self.input['learning_rate'])
+```
+
+You can also execute the whole function again:
+```python
+>>> from sklearn import ensemble  # imports work seamlessly due to conda extension
+>>> from sklearn.model_selection import cross_val_score
+>>> import numpy as np
+>>> estimator = ensemble.GradientBoostingRegressor( n_estimators = self.input['n_estimators'], learning_rate = self.input['learning_rate'],
+    max_depth = self.input['max_depth'], min_samples_split = 2, loss = 'ls')
+>>> estimator.fit(self.features, self.labels)
+>>> mses = cross_val_score(estimator, self.features, self.labels, cv = 5, scoring='neg_mean_squared_error')
+>>> rmse = np.sqrt(-mses).mean()
+>>> self.fit = dict(
+    index=int(self.index),
+    params=self.input,
+    rmse=rmse,
+    estimator=estimator
+)
+```
+
+You can examine the effects of other hyper-parameters live by modifying the `min_samples_split = 3` and re-executing the steps on the same data.
```

### Comparing `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py` & `metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/cmd/environment/utils.py` & `metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/cmd/environment/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py` & `metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/generate_vendor.py` & `metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/generate_vendor.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/conda.py` & `metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/conda_common_decorator.py` & `metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda_common_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py` & `metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,33 +180,29 @@
     def decospecs(self) -> Tuple[str, ...]:
         return ("conda_env_internal",) + self.base_env.decospecs()
 
     def bootstrap_commands(
         self,
         step_name: str,
         datastore_type: str,
-        default_executable_path: Optional[str] = None,
     ) -> List[str]:
         # Bootstrap conda and execution environment for step
         env_id = self.get_env_id_noconda(step_name)
         if env_id is not None:
             if isinstance(env_id, EnvID):
                 arg1 = env_id.req_id
                 arg2 = env_id.full_id
             else:
                 arg1 = env_id
                 arg2 = "_fetch_exec"
             return [
                 "export CONDA_START=$(date +%s)",
                 "echo 'Bootstrapping environment ...'",
-                '%s -m %s.remote_bootstrap "%s" "%s" %s %s %s'
+                'python -m %s.remote_bootstrap "%s" "%s" %s %s %s'
                 % (
-                    "python"
-                    if default_executable_path is None
-                    else default_executable_path,
                     "metaflow_extensions.netflix_ext.plugins.conda",
                     self._flow.name,
                     step_name,
                     arg1,
                     arg2,
                     datastore_type,
                 ),
```

### Comparing `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py` & `metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py` & `metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py` & `metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py` & `metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py`

 * *Files 1% similar despite different names*

```diff
@@ -700,14 +700,21 @@
             )
             return (
                 str(name),
                 str(version),
                 "" if len(buildtag) == 0 else "%s-%s" % (buildtag[0], buildtag[1]),
             )
 
+    def is_external_url(self, sources: Dict[str, List[str]]) -> bool:
+        # Returns True if the URL is not in the sources
+        # This is used to determine if we should consider a package as a local package to
+        # be downloaded before resolving the environment
+        pypi_sources = sources.get("pypi", [])
+        return not any(urlparse(source).netloc in self.url for source in pypi_sources)
+
 
 class ResolvedEnvironment:
     def __init__(
         self,
         user_dependencies: Dict[str, List[str]],
         user_sources: Optional[Dict[str, List[str]]],
         user_extra_args: Optional[Dict[str, List[str]]],
```

### Comparing `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/envsresolver.py` & `metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/envsresolver.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/pypi_package_builder.py` & `metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/pypi_package_builder.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py` & `metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resolvers/__init__.py` & `metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resolvers/builder_envs_resolver.py` & `metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/resolvers/builder_envs_resolver.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resolvers/conda_lock_resolver.py` & `metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/resolvers/conda_lock_resolver.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resolvers/conda_resolver.py` & `metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/resolvers/conda_resolver.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resolvers/micromamba_server_resolver.py` & `metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/resolvers/micromamba_server_resolver.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resolvers/pip_resolver.py` & `metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/resolvers/pip_resolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,18 +53,25 @@
             # packages, we need to make them available again to pip when resolving.
             # We therefore check packages that are:
             #   - not directly downloadable from their URL so, in this case, the URL is
             #     fake (ie: it contains FAKEURL_PATHCOMPONENT -- this is used when
             #     we build a package from a local directory/GIT repo, etc)
             #   - OR derived from a source package. This is the case when we build
             #     a wheel from a source package.
+            #   - OR packages that have a download URL that is not a pypi URL or belongs to
+            #     the sources we have for pypi. For instance pacakage @ github.com/..../package.wheel
             local_packages = [
                 p
                 for p in base_env.packages
-                if p.TYPE == "pypi" and (not p.is_downloadable_url() or p.is_derived())
+                if p.TYPE == "pypi"
+                and (
+                    not p.is_downloadable_url()
+                    or p.is_derived()
+                    or p.is_external_url(sources)
+                )
             ]
         else:
             local_packages = None
         # Some args may be two actual arguments like "-f <something>" thus the map
         extra_args = list(
             chain.from_iterable(
                 map(lambda x: x.split(maxsplit=1), (e for e in extras.get("pypi", [])))
```

### Comparing `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png` & `metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png` & `metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg` & `metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py` & `metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/conda/utils.py` & `metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/conda/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/environment_cli.py` & `metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/environment_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.3/metaflow_extensions/netflix_ext/plugins/mfextinit_netflixext.py` & `metaflow_netflixext-1.2.0/metaflow_extensions/netflix_ext/plugins/mfextinit_netflixext.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-1.1.3/metaflow_netflixext.egg-info/PKG-INFO` & `metaflow_netflixext-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: metaflow-netflixext
-Version: 1.1.3
-Summary: Metaflow extensions from Netflix
-Author: Netflix Metaflow Developers
-Author-email: metaflow-dev@netflix.com
-License: Apache Software License
-Project-URL: Source, https://github.com/Netflix/metaflow-nflx-extensions
-Project-URL: Tracker, https://github.com/Netflix/metaflow-nflx-extensions/issues
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.7.2
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: metaflow>=2.10.0
-
 # Metaflow Extensions from Netflix
 This repository contains extensions for Metaflow that are in use at Netflix (or being tested
 at Netflix) and that are more cutting edge than what is included in the OSS Metaflow package.
 
 You can find support for this extension on the usual Metaflow [Slack](http://slack.outerbounds.co).
 
 NOTE: of you are within Netflix and are looking for the Netflix version of Metaflow,
@@ -52,14 +27,15 @@
 This extension is currently tested on python 3.7+.
 
 If you have any question, feel free to open an issue here or contact us on the usual
 Metaflow slack channels.
 
 This extension currently contains:
 - refactored and improved [Conda decorator](#conda-v2)
+- improved [debugging capability](#debug)
 
 ## Conda V2
 
 *Version 1.0.0 is considered stable. Some UX changes have occurred compared to previous
 versions. Please see the [docs](https://github.com/Netflix/metaflow-nflx-extensions/blob/main/docs/conda.md) for more information*
 
 *Version 0.2.0 of this extension is not fully backward compatible with previous versions due to
@@ -392,7 +368,90 @@
 - remotely:
   - Environment descriptiosn are also stored remotely and can be fetched to be added
     to the local `conda_v2.cnd` file.
   - Packages are stored as archived and may be downloaded in the `pkgs` directory. The
     implementation takes care of properly updating the `urls.txt` file to make it
     transparent to Conda (allowing it to operate in an "offline" mode effectively).
 
+## Debug
+This extension allows user's to seamlessly debug their executed steps in an isolated Jupyter notebook instance
+with appropriate dependencies by leveraging the conda extension described above (note, this extension currently only
+works with the version of Conda in this package). 
+
+### Executing the command
+Let's say you have a step called `fit_gbrt_for_given_param` in your flow, and on executing it, the pathspec for
+this step/task is `HousePricePredictionFlow/1199/fit_gbrt_for_given_param/150671013`. To debug this step, you can run the command:
+
+```bash
+metaflow debug task <HousePricePredictionFlow/1199/fit_gbrt_for_given_param/150671013> --metaflow-root-dir ~/notebooks/debug_task`
+```
+
+Note that you can specify a partial pathspec as long as it can be resolved to a unique task:
+
+- if you specify just a flow name, it will use the latest run in your namespace and the end step
+- if you specify just a run pathspec, it will use the end step
+- if you specify just a step pathspec, it will use the unique task for that step and error if there are more than one tasks (foreach)
+
+### Using the extension
+Running the above command will:
+
+- download your code package
+- download the appropriate conda/pip packages defined for that particular step (if you use the conda extension)
+- generate stubs to access the relevant artifacts for that particular run.
+
+It will additionally generate a notebook in the defined directory where you can debug the execution of your step line by line. For the given step definition:
+```python
+@step
+def fit_gbrt_for_given_param(self):
+    """
+    Fit GBRT with given parameters
+    """
+
+    from sklearn import ensemble
+    from sklearn.model_selection import cross_val_score
+    import numpy as np
+
+
+    estimator = ensemble.GradientBoostingRegressor( n_estimators = self.input['n_estimators'], learning_rate = self.input['learning_rate'],
+        max_depth = self.input['max_depth'], min_samples_split = 2, loss = 'ls')
+
+    estimator.fit(self.features, self.labels)
+
+    mses = cross_val_score(estimator, self.features, self.labels, cv = 5, scoring='neg_mean_squared_error')
+    rmse = np.sqrt(-mses).mean()
+
+
+    self.fit = dict(
+        index=int(self.index),
+        params=self.input,
+        rmse=rmse,
+        estimator=estimator
+    )
+
+    self.next(self.select_best_model)
+```
+
+You will be able to access the artifacts/inputs in your generated notebook directly:
+```python
+>>> print(self.input['n_estimators'])  # You can access objects using `self` as we imported a stub for it in the notebook
+>>> print(self.input['learning_rate'])
+```
+
+You can also execute the whole function again:
+```python
+>>> from sklearn import ensemble  # imports work seamlessly due to conda extension
+>>> from sklearn.model_selection import cross_val_score
+>>> import numpy as np
+>>> estimator = ensemble.GradientBoostingRegressor( n_estimators = self.input['n_estimators'], learning_rate = self.input['learning_rate'],
+    max_depth = self.input['max_depth'], min_samples_split = 2, loss = 'ls')
+>>> estimator.fit(self.features, self.labels)
+>>> mses = cross_val_score(estimator, self.features, self.labels, cv = 5, scoring='neg_mean_squared_error')
+>>> rmse = np.sqrt(-mses).mean()
+>>> self.fit = dict(
+    index=int(self.index),
+    params=self.input,
+    rmse=rmse,
+    estimator=estimator
+)
+```
+
+You can examine the effects of other hyper-parameters live by modifying the `min_samples_split = 3` and re-executing the steps on the same data.
```

### Comparing `metaflow-netflixext-1.1.3/metaflow_netflixext.egg-info/SOURCES.txt` & `metaflow_netflixext-1.2.0/metaflow_netflixext.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 LICENSE
 README.md
 setup.py
 metaflow_extensions/netflix_ext/generate_vendor.py
 metaflow_extensions/netflix_ext/cmd/mfextinit_netflixext.py
+metaflow_extensions/netflix_ext/cmd/debug/__init__.py
+metaflow_extensions/netflix_ext/cmd/debug/constants.py
+metaflow_extensions/netflix_ext/cmd/debug/current_stub_generator.py
+metaflow_extensions/netflix_ext/cmd/debug/debug_cmd.py
+metaflow_extensions/netflix_ext/cmd/debug/debug_script_generator.py
+metaflow_extensions/netflix_ext/cmd/debug/debug_stub_generator.py
+metaflow_extensions/netflix_ext/cmd/debug/debug_utils.py
+metaflow_extensions/netflix_ext/cmd/debug/jupyter_instructions_markdown.py
+metaflow_extensions/netflix_ext/cmd/debug/jupyter_title_markdown.py
 metaflow_extensions/netflix_ext/cmd/environment/__init__.py
 metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py
 metaflow_extensions/netflix_ext/cmd/environment/utils.py
 metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py
 metaflow_extensions/netflix_ext/plugins/environment_cli.py
 metaflow_extensions/netflix_ext/plugins/mfextinit_netflixext.py
 metaflow_extensions/netflix_ext/plugins/conda/__init__.py
```

### Comparing `metaflow-netflixext-1.1.3/setup.py` & `metaflow_netflixext-1.2.0/setup.py`

 * *Files identical despite different names*

