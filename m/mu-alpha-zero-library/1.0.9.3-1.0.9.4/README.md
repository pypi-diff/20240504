# Comparing `tmp/mu_alpha_zero_library-1.0.9.3.tar.gz` & `tmp/mu_alpha_zero_library-1.0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mu_alpha_zero_library-1.0.9.3.tar", last modified: Thu Apr  4 12:34:29 2024, max compression
+gzip compressed data, was "mu_alpha_zero_library-1.0.9.4.tar", last modified: Sat May  4 12:51:07 2024, max compression
```

## Comparing `mu_alpha_zero_library-1.0.9.3.tar` & `mu_alpha_zero_library-1.0.9.4.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:29.518195 mu_alpha_zero_library-1.0.9.3/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-04 12:34:29.518195 mu_alpha_zero_library-1.0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:29.510195 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:29.510195 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:29.510195 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/Arena/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/Arena/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4931 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/Arena/arena.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8548 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/Arena/players.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:29.514195 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/MCTS/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/MCTS/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5473 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/MCTS/az_node.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9589 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/MCTS/az_search_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:29.514195 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/Network/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/Network/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7370 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/Network/nnet.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16326 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/Network/trainer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      166 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4501 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/alpha_zero.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5294 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/checkpointer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2593 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4590 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10972 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:29.514195 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/Game/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/Game/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1349 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/Game/asteroids.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17301 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/Game/tictactoe_game.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:29.514195 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/General/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/General/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      365 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/General/arena.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3070 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/General/az_game.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      674 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/General/memory.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2239 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/General/mz_game.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3006 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/General/network.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1241 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/General/search_tree.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1685 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/General/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:29.514195 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/Hooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/Hooks/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      541 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/Hooks/hook_callables.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      653 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/Hooks/hook_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      683 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/Hooks/hook_point.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:29.514195 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:29.514195 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/JavaGateway/
--rwxr-xr-x   0 runner    (1001) docker     (127)       38 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/JavaGateway/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3004 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/JavaGateway/java_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      321 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/JavaGateway/java_networks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:29.514195 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/MZ_Arena/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/MZ_Arena/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2982 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/MZ_Arena/arena.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:29.518195 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/MZ_MCTS/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/MZ_MCTS/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2010 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/MZ_MCTS/mz_node.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7609 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/MZ_MCTS/mz_search_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:29.518195 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/Network/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/Network/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10649 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/Network/networks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      767 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/lazy_arrays.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4936 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/muzero.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2604 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/pickler.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5023 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3398 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7017 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/main.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11244 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/mem_buffer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      253 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/prepare_for_upload.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5549 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/root.root
--rwxr-xr-x   0 runner    (1001) docker     (127)      384 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/save_best_params.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1579 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/start_jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:34:29.518195 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-04 12:34:29.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-04 12:34:29.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:34:29.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-04 12:34:29.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-04 12:34:29.000000 mu_alpha_zero_library-1.0.9.3/mu_alpha_zero_library.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 12:34:29.518195 mu_alpha_zero_library-1.0.9.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      513 2024-04-04 12:32:21.000000 mu_alpha_zero_library-1.0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:51:07.593573 mu_alpha_zero_library-1.0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-04 12:51:07.593573 mu_alpha_zero_library-1.0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:51:07.585573 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:51:07.585573 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/AlphaZero/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:51:07.585573 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/AlphaZero/Arena/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/AlphaZero/Arena/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4931 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/AlphaZero/Arena/arena.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8548 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/AlphaZero/Arena/players.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:51:07.585573 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/AlphaZero/MCTS/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/AlphaZero/MCTS/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5473 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/AlphaZero/MCTS/az_node.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9865 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/AlphaZero/MCTS/az_search_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:51:07.585573 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/AlphaZero/Network/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/AlphaZero/Network/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7370 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/AlphaZero/Network/nnet.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16326 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/AlphaZero/Network/trainer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      166 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/AlphaZero/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4501 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/AlphaZero/alpha_zero.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5294 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/AlphaZero/checkpointer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2593 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/AlphaZero/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4590 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/AlphaZero/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10972 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/AlphaZero/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:51:07.589573 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/Game/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/Game/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1436 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/Game/asteroids.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17301 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/Game/tictactoe_game.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:51:07.589573 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/General/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/General/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      365 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/General/arena.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3070 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/General/az_game.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      674 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/General/memory.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2569 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/General/mz_game.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3006 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/General/network.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1241 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/General/search_tree.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1685 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/General/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:51:07.589573 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/Hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/Hooks/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      541 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/Hooks/hook_callables.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      653 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/Hooks/hook_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      683 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/Hooks/hook_point.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:51:07.589573 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/MuZero/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:51:07.589573 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/MuZero/JavaGateway/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       38 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/MuZero/JavaGateway/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3004 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/MuZero/JavaGateway/java_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      321 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/MuZero/JavaGateway/java_networks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:51:07.589573 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/MuZero/MZ_Arena/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/MuZero/MZ_Arena/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2982 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/MuZero/MZ_Arena/arena.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:51:07.589573 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/MuZero/MZ_MCTS/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/MuZero/MZ_MCTS/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2010 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/MuZero/MZ_MCTS/mz_node.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7917 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/MuZero/MZ_MCTS/mz_search_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:51:07.589573 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/MuZero/Network/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/MuZero/Network/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10649 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/MuZero/Network/networks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/MuZero/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      767 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/MuZero/lazy_arrays.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4936 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/MuZero/muzero.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2604 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/MuZero/pickler.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5174 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/MuZero/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3424 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7017 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11244 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/mem_buffer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      253 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/prepare_for_upload.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5549 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/root.root
+-rwxr-xr-x   0 runner    (1001) docker     (127)      384 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/save_best_params.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1579 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/start_jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:51:07.589573 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-04 12:51:07.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-04 12:51:07.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 12:51:07.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-04 12:51:07.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-04 12:51:07.000000 mu_alpha_zero_library-1.0.9.4/mu_alpha_zero_library.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 12:51:07.593573 mu_alpha_zero_library-1.0.9.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      513 2024-05-04 12:49:00.000000 mu_alpha_zero_library-1.0.9.4/setup.py
```

### Comparing `mu_alpha_zero_library-1.0.9.3/LICENSE` & `mu_alpha_zero_library-1.0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/PKG-INFO` & `mu_alpha_zero_library-1.0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mu_alpha_zero_library
-Version: 1.0.9.3
+Version: 1.0.9.4
 Summary: Library for running and training MuZero and AlphaZero models.
 Home-page: https://github.com/Skirlax/MuAlphaZeroLibrary
 Author: Skyr
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MuAlphaZeroLibrary
```

### Comparing `mu_alpha_zero_library-1.0.9.3/README.md` & `mu_alpha_zero_library-1.0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/Arena/arena.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/AlphaZero/Arena/arena.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/Arena/players.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/AlphaZero/Arena/players.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/MCTS/az_node.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/AlphaZero/MCTS/az_node.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/MCTS/az_search_tree.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/AlphaZero/MCTS/az_search_tree.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import copy
 from multiprocessing import Pool
 
+import numpy as np
 import torch as th
 
 from mu_alpha_zero.AlphaZero.MCTS.az_node import AlphaZeroNode
 from mu_alpha_zero.AlphaZero.utils import augment_experience_with_symmetries, mask_invalid_actions
 from mu_alpha_zero.Game.tictactoe_game import TicTacToeGameManager
 from mu_alpha_zero.General.memory import GeneralMemoryBuffer
 from mu_alpha_zero.General.network import GeneralNetwork
@@ -89,15 +90,16 @@
             tau = self.alpha_zero_config.tau
         if self.root_node is None:
             self.root_node = AlphaZeroNode(current_player, times_visited_init=0)
         state_ = self.game_manager.get_canonical_form(state, current_player)
         # state_ = make_channels_from_single(state_)
         state_ = th.tensor(state_, dtype=th.float32, device=device).unsqueeze(0)
         probabilities, v = network.predict(state_, muzero=False)
-
+        probabilities = probabilities + np.random.dirichlet(
+            [self.alpha_zero_config.dirichlet_alpha] * self.alpha_zero_config.net_action_size).reshape(1,-1) # add noise to encourage the exploration of even the moves with probability close to 0.
         probabilities = mask_invalid_actions(probabilities, state.copy(), self.game_manager.board_size)
         probabilities = probabilities.flatten().tolist()
         self.root_node.expand(state, probabilities)
         for simulation in range(num_simulations):
             current_node = self.root_node
             path = [current_node]
             action = None
```

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/Network/nnet.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/AlphaZero/Network/nnet.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/Network/trainer.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/AlphaZero/Network/trainer.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/alpha_zero.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/AlphaZero/alpha_zero.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/checkpointer.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/AlphaZero/checkpointer.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/constants.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/AlphaZero/constants.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/logger.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/AlphaZero/logger.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/AlphaZero/utils.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/AlphaZero/utils.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/Game/asteroids.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/Game/asteroids.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import torch as th
 from gymnasium import make
 
 from mu_alpha_zero.General.mz_game import MuZeroGame
 
 
 class Asteroids(MuZeroGame):
+
     def __init__(self):
         self.env = make("ALE/Asteroids-v5")
         self.done = False
 
     def reset(self) -> np.ndarray or th.Tensor:
         obs, _ = self.env.reset()
         return obs
@@ -40,7 +41,11 @@
         return obs, rew, done
 
     def render(self):
         pass
 
     def get_random_valid_action(self,board: np.ndarray):
         return self.env.action_space.sample()
+
+    def get_invalid_actions(self):
+        return np.ones((self.get_num_actions()))
+
```

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/Game/tictactoe_game.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/Game/tictactoe_game.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/General/az_game.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/General/az_game.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/General/memory.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/General/memory.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/General/mz_game.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/General/mz_game.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,7 +72,15 @@
     @staticmethod
     def select_move(action_probs: dict):
         """
         Samples a move from the action probabilities.
         """
         moves, probs = zip(*action_probs.items())
         return np.random.choice(moves, p=probs)
+
+    @abstractmethod
+    def get_invalid_actions(self):
+        """
+        Calculates and returns the invalid actions in the given state. :return: A numpy array containing the invalid
+        actions in the current state. In this array actions marked as valid will be one, while invalid actions will
+        be 0."""
+        pass
```

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/General/network.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/General/network.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/General/search_tree.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/General/search_tree.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/General/utils.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/General/utils.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/Hooks/hook_callables.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/Hooks/hook_callables.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/Hooks/hook_manager.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/Hooks/hook_manager.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/Hooks/hook_point.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/Hooks/hook_point.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/JavaGateway/java_manager.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/MuZero/JavaGateway/java_manager.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/MZ_Arena/arena.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/MuZero/MZ_Arena/arena.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/MZ_MCTS/mz_node.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/MuZero/MZ_MCTS/mz_node.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/MZ_MCTS/mz_search_tree.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/MuZero/MZ_MCTS/mz_search_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from mu_alpha_zero.General.mz_game import MuZeroGame
 from mu_alpha_zero.General.search_tree import SearchTree
 from mu_alpha_zero.Hooks.hook_manager import HookManager
 from mu_alpha_zero.Hooks.hook_point import HookAt
 from mu_alpha_zero.MuZero.MZ_MCTS.mz_node import MzAlphaZeroNode
 from mu_alpha_zero.MuZero.Network.networks import MuZeroNet
 from mu_alpha_zero.MuZero.lazy_arrays import LazyArray
-from mu_alpha_zero.MuZero.utils import match_action_with_obs, resize_obs, scale_action, scale_reward, scale_state,scale_hidden_state
+from mu_alpha_zero.MuZero.utils import match_action_with_obs, resize_obs, scale_action, scale_reward, scale_state, \
+    scale_hidden_state, mask_invalid_actions
 from mu_alpha_zero.config import MuZeroConfig
 from mu_alpha_zero.mem_buffer import MuZeroFrameBuffer
 
 
 class MuZeroSearchTree(SearchTree):
 
     def __init__(self, game_manager: MuZeroGame, muzero_config: MuZeroConfig, hook_manager: HookManager or None = None):
@@ -64,14 +65,16 @@
             tau = self.muzero_config.tau
 
         root_node = MzAlphaZeroNode()
         state_ = network_wrapper.representation_forward(
             self.buffer.concat_frames().permute(2, 0, 1).unsqueeze(0)).squeeze(0)
         state_ = scale_hidden_state(state_)
         pi, v = network_wrapper.prediction_forward(state_.unsqueeze(0), predict=True)
+        pi = pi + np.random.dirichlet([self.muzero_config.dirichlet_alpha] * self.muzero_config.net_action_size)
+        pi = mask_invalid_actions(self.game_manager.get_invalid_actions(), pi)
         pi = pi.flatten().tolist()
         root_node.expand_node(state_, pi, 0)
         for simulation in range(num_simulations):
             current_node = root_node
             path = [current_node]
             action = None
             while current_node.was_visited():
@@ -84,14 +87,15 @@
             next_state, reward = network_wrapper.dynamics_forward(current_node_state_with_action.unsqueeze(0),
                                                                   predict=True)
             next_state = scale_hidden_state(next_state)
             reward = reward[0][0]
             v = self.game_manager.game_result(current_node.current_player)
             if v is None or not v:
                 pi, v = network_wrapper.prediction_forward(next_state.unsqueeze(0), predict=True)
+                pi = mask_invalid_actions(self.game_manager.get_invalid_actions(), pi)
                 pi = pi.flatten().tolist()
                 v = v.flatten().tolist()[0]
                 current_node.expand_node(next_state, pi, reward)
             self.backprop(v, path)
 
         action_probs = root_node.get_self_action_probabilities(tau=tau)
         root_val_latent = (root_node.get_self_value(), root_node.get_latent())
```

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/Network/networks.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/MuZero/Network/networks.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/lazy_arrays.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/MuZero/lazy_arrays.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/muzero.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/MuZero/muzero.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/pickler.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/MuZero/pickler.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/MuZero/utils.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/MuZero/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,7 +112,12 @@
     else:
         if storage is None:
             raise ValueError("Storage can't be None if in_memory is False.")
         study = optuna.load_study(study_name=study_name, storage=storage)
     study.optimize(objective, n_trials=n_trials)
     with open(f"{muzero_config.checkpoint_dir}/study_params.json", "w") as file:
         json.dump(study.best_params, file)
+
+
+def mask_invalid_actions(invalid_actions: np.ndarray,pi: np.ndarray):
+    pi = pi.reshape(-1) * invalid_actions.reshape(-1)
+    return pi / pi.sum()
```

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/__init__.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/__init__.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/config.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     max_buffer_size: int = 70_000
     num_pit_games: int = 40
     random_pit_freq: int = 2
     batch_size: int = 255
     tau: float = 1
     arena_tau: float = 1e-2
     c: float = 1
+    dirichlet_alpha = 0.3
     checkpoint_dir: str = None
     update_threshold: float = 0.6
     num_workers: int = 5
     log_epsilon: float = 1e-9
     zero_tau_after: int = 5
     az_net_linear_input_size: int = 8192
     log_dir: str = "Logs"
```

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/main.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/main.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/mem_buffer.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/mem_buffer.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/root.root` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/root.root`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero/start_jobs.py` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero/start_jobs.py`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero_library.egg-info/PKG-INFO` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero_library.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mu-alpha-zero-library
-Version: 1.0.9.3
+Version: 1.0.9.4
 Summary: Library for running and training MuZero and AlphaZero models.
 Home-page: https://github.com/Skirlax/MuAlphaZeroLibrary
 Author: Skyr
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MuAlphaZeroLibrary
```

### Comparing `mu_alpha_zero_library-1.0.9.3/mu_alpha_zero_library.egg-info/SOURCES.txt` & `mu_alpha_zero_library-1.0.9.4/mu_alpha_zero_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mu_alpha_zero_library-1.0.9.3/setup.py` & `mu_alpha_zero_library-1.0.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="mu_alpha_zero_library",
-    version="1.0.9.3",
+    version="1.0.9.4",
     description="Library for running and training MuZero and AlphaZero models.",
     author="Skyr",
     install_requires=open("requirements.txt").read().strip().split("\n"),
     long_description=open('README.md',encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     package_data={
         "mu_alpha_zero": ["*.txt", "*.root"]
```

