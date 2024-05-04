# Comparing `tmp/prodsys-0.5.3.tar.gz` & `tmp/prodsys-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodsys-0.5.3.tar", max compression
+gzip compressed data, was "prodsys-0.6.0.tar", max compression
```

## Comparing `prodsys-0.5.3.tar` & `prodsys-0.6.0.tar`

### file list

```diff
@@ -1,75 +1,81 @@
--rw-r--r--   0        0        0     1096 2023-10-11 11:05:21.946526 prodsys-0.5.3/LICENSE
--rw-r--r--   0        0        0      405 2024-04-18 15:37:10.949961 prodsys-0.5.3/prodsys/__init__.py
--rw-r--r--   0        0        0     1289 2024-01-07 23:00:16.870495 prodsys-0.5.3/prodsys/adapters/__init__.py
--rw-r--r--   0        0        0    51413 2024-04-14 17:14:53.846311 prodsys-0.5.3/prodsys/adapters/adapter.py
--rw-r--r--   0        0        0     8314 2024-04-07 17:13:56.244883 prodsys-0.5.3/prodsys/adapters/json_adapter.py
--rw-r--r--   0        0        0        0 2024-01-07 23:00:16.874004 prodsys-0.5.3/prodsys/conf/__init__.py
--rw-r--r--   0        0        0     2487 2024-01-07 23:00:16.874004 prodsys-0.5.3/prodsys/conf/logging.ini
--rw-r--r--   0        0        0     1155 2024-01-07 23:00:16.874004 prodsys-0.5.3/prodsys/conf/logging_config.py
--rw-r--r--   0        0        0      148 2023-10-11 11:05:22.073479 prodsys-0.5.3/prodsys/control/__init__.py
--rw-r--r--   0        0        0     9028 2023-12-24 15:55:37.172880 prodsys-0.5.3/prodsys/control/routing_control_env.py
--rw-r--r--   0        0        0     8489 2023-10-11 11:05:22.073479 prodsys-0.5.3/prodsys/control/sequencing_control_env.py
--rw-r--r--   0        0        0     2138 2024-04-07 17:13:56.244883 prodsys-0.5.3/prodsys/express/__init__.py
--rw-r--r--   0        0        0      603 2023-10-11 11:05:22.073479 prodsys-0.5.3/prodsys/express/core.py
--rw-r--r--   0        0        0     6525 2024-04-07 17:13:56.244883 prodsys-0.5.3/prodsys/express/process.py
--rw-r--r--   0        0        0     2435 2024-04-07 17:13:56.244883 prodsys-0.5.3/prodsys/express/product.py
--rw-r--r--   0        0        0     6508 2024-04-07 17:13:56.244883 prodsys-0.5.3/prodsys/express/production_system.py
--rw-r--r--   0        0        0     8275 2024-04-07 17:13:56.260662 prodsys-0.5.3/prodsys/express/resources.py
--rw-r--r--   0        0        0     2558 2024-02-27 21:06:20.429295 prodsys-0.5.3/prodsys/express/sink.py
--rw-r--r--   0        0        0     3454 2024-01-07 23:00:16.874004 prodsys-0.5.3/prodsys/express/source.py
--rw-r--r--   0        0        0     7554 2023-10-11 11:05:22.089564 prodsys-0.5.3/prodsys/express/state.py
--rw-r--r--   0        0        0     4895 2023-10-11 11:05:22.089564 prodsys-0.5.3/prodsys/express/time_model.py
--rw-r--r--   0        0        0      913 2023-10-11 11:05:22.089564 prodsys-0.5.3/prodsys/factories/__init__.py
--rw-r--r--   0        0        0     3439 2024-04-07 17:13:56.261200 prodsys-0.5.3/prodsys/factories/process_factory.py
--rw-r--r--   0        0        0     6358 2024-03-10 14:05:36.923357 prodsys-0.5.3/prodsys/factories/product_factory.py
--rw-r--r--   0        0        0     1992 2024-03-10 14:05:36.923357 prodsys-0.5.3/prodsys/factories/queue_factory.py
--rw-r--r--   0        0        0    10419 2024-04-12 11:17:17.974120 prodsys-0.5.3/prodsys/factories/resource_factory.py
--rw-r--r--   0        0        0     3268 2023-10-11 11:05:22.089564 prodsys-0.5.3/prodsys/factories/sink_factory.py
--rw-r--r--   0        0        0     5089 2024-01-07 23:00:16.890715 prodsys-0.5.3/prodsys/factories/source_factory.py
--rw-r--r--   0        0        0     2856 2023-10-11 11:05:22.089564 prodsys-0.5.3/prodsys/factories/state_factory.py
--rw-r--r--   0        0        0     2045 2023-10-11 11:05:22.089564 prodsys-0.5.3/prodsys/factories/time_model_factory.py
--rw-r--r--   0        0        0     1436 2024-04-07 17:13:56.263212 prodsys-0.5.3/prodsys/models/__init__.py
--rw-r--r--   0        0        0      541 2023-10-11 11:05:22.089564 prodsys-0.5.3/prodsys/models/core_asset.py
--rw-r--r--   0        0        0     2971 2024-02-27 19:26:17.985971 prodsys-0.5.3/prodsys/models/performance_data.py
--rw-r--r--   0        0        0     9369 2023-10-11 11:05:22.089564 prodsys-0.5.3/prodsys/models/performance_indicators.py
--rw-r--r--   0        0        0    11648 2024-04-14 17:14:53.855074 prodsys-0.5.3/prodsys/models/processes_data.py
--rw-r--r--   0        0        0     6357 2024-04-14 17:14:53.857017 prodsys-0.5.3/prodsys/models/product_data.py
--rw-r--r--   0        0        0     1931 2024-04-14 17:14:53.857017 prodsys-0.5.3/prodsys/models/queue_data.py
--rw-r--r--   0        0        0    12337 2024-04-14 17:14:53.862626 prodsys-0.5.3/prodsys/models/resource_data.py
--rw-r--r--   0        0        0    10730 2024-04-12 11:17:17.974120 prodsys-0.5.3/prodsys/models/scenario_data.py
--rw-r--r--   0        0        0     2846 2024-04-14 17:14:53.863598 prodsys-0.5.3/prodsys/models/sink_data.py
--rw-r--r--   0        0        0     4059 2024-04-14 17:14:53.865574 prodsys-0.5.3/prodsys/models/source_data.py
--rw-r--r--   0        0        0    13852 2024-04-14 17:14:53.865574 prodsys-0.5.3/prodsys/models/state_data.py
--rw-r--r--   0        0        0     6642 2024-04-14 17:14:53.865574 prodsys-0.5.3/prodsys/models/time_model_data.py
--rw-r--r--   0        0        0     2870 2023-10-11 11:05:22.105207 prodsys-0.5.3/prodsys/optimization/__init__.py
--rw-r--r--   0        0        0    12476 2024-04-14 17:14:53.871089 prodsys-0.5.3/prodsys/optimization/evolutionary_algorithm.py
--rw-r--r--   0        0        0    28223 2024-04-14 17:14:53.874200 prodsys-0.5.3/prodsys/optimization/math_opt.py
--rw-r--r--   0        0        0     4642 2024-04-18 14:45:11.231208 prodsys-0.5.3/prodsys/optimization/optimization_analysis.py
--rw-r--r--   0        0        0    46122 2024-04-18 16:40:28.425916 prodsys-0.5.3/prodsys/optimization/optimization_util.py
--rw-r--r--   0        0        0     9577 2024-04-18 14:47:16.673364 prodsys-0.5.3/prodsys/optimization/simulated_annealing.py
--rw-r--r--   0        0        0    11871 2024-04-18 14:51:26.265202 prodsys-0.5.3/prodsys/optimization/tabu_search.py
--rw-r--r--   0        0        0     1704 2023-10-11 11:05:22.105207 prodsys-0.5.3/prodsys/simulation/__init__.py
--rw-r--r--   0        0        0    27915 2024-04-12 11:17:17.986645 prodsys-0.5.3/prodsys/simulation/control.py
--rw-r--r--   0        0        0     6855 2023-10-11 11:05:22.105207 prodsys-0.5.3/prodsys/simulation/logger.py
--rw-r--r--   0        0        0     3763 2024-01-07 23:00:16.907148 prodsys-0.5.3/prodsys/simulation/observer.py
--rw-r--r--   0        0        0     9601 2024-04-07 17:13:56.267724 prodsys-0.5.3/prodsys/simulation/proces_models.py
--rw-r--r--   0        0        0     9097 2024-04-07 17:13:56.267724 prodsys-0.5.3/prodsys/simulation/process.py
--rw-r--r--   0        0        0    11882 2024-04-07 17:13:56.267724 prodsys-0.5.3/prodsys/simulation/product.py
--rw-r--r--   0        0        0     4004 2024-04-07 17:13:56.267724 prodsys-0.5.3/prodsys/simulation/request.py
--rw-r--r--   0        0        0    17837 2024-04-12 11:17:17.986645 prodsys-0.5.3/prodsys/simulation/resources.py
--rw-r--r--   0        0        0     9574 2024-04-12 11:17:17.989996 prodsys-0.5.3/prodsys/simulation/router.py
--rw-r--r--   0        0        0     3199 2023-10-11 11:05:22.120833 prodsys-0.5.3/prodsys/simulation/sim.py
--rw-r--r--   0        0        0     2260 2024-04-12 11:17:17.990877 prodsys-0.5.3/prodsys/simulation/sink.py
--rw-r--r--   0        0        0     3809 2024-04-12 11:17:17.990877 prodsys-0.5.3/prodsys/simulation/source.py
--rw-r--r--   0        0        0    29184 2024-04-07 17:13:56.277897 prodsys-0.5.3/prodsys/simulation/state.py
--rw-r--r--   0        0        0     2232 2024-01-07 23:00:16.919358 prodsys-0.5.3/prodsys/simulation/store.py
--rw-r--r--   0        0        0     7193 2024-04-07 17:13:56.277897 prodsys-0.5.3/prodsys/simulation/time_model.py
--rw-r--r--   0        0        0       61 2023-10-11 11:05:22.120833 prodsys-0.5.3/prodsys/util/__init__.py
--rw-r--r--   0        0        0     8056 2023-11-06 17:14:55.559034 prodsys-0.5.3/prodsys/util/kpi_visualization.py
--rw-r--r--   0        0        0    30399 2024-04-18 16:37:39.544817 prodsys-0.5.3/prodsys/util/post_processing.py
--rw-r--r--   0        0        0    12118 2024-04-07 17:13:56.277897 prodsys-0.5.3/prodsys/util/runner.py
--rw-r--r--   0        0        0     2657 2023-12-24 16:10:02.245387 prodsys-0.5.3/prodsys/util/statistical_functions.py
--rw-r--r--   0        0        0     4379 2024-04-18 15:06:57.609972 prodsys-0.5.3/prodsys/util/util.py
--rw-r--r--   0        0        0     1581 2024-04-18 17:02:27.233520 prodsys-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     6375 2024-04-18 15:32:08.045325 prodsys-0.5.3/README.md
--rw-r--r--   0        0        0     8405 1970-01-01 00:00:00.000000 prodsys-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-10-11 11:05:21.946526 prodsys-0.6.0/LICENSE
+-rw-r--r--   0        0        0      405 2024-05-04 14:52:14.089697 prodsys-0.6.0/prodsys/__init__.py
+-rw-r--r--   0        0        0     1289 2024-05-01 05:54:38.231436 prodsys-0.6.0/prodsys/adapters/__init__.py
+-rw-r--r--   0        0        0    56327 2024-05-04 14:52:14.090345 prodsys-0.6.0/prodsys/adapters/adapter.py
+-rw-r--r--   0        0        0     8854 2024-05-04 14:52:14.090345 prodsys-0.6.0/prodsys/adapters/json_adapter.py
+-rw-r--r--   0        0        0        0 2024-01-07 23:00:16.874004 prodsys-0.6.0/prodsys/conf/__init__.py
+-rw-r--r--   0        0        0     2487 2024-01-07 23:00:16.874004 prodsys-0.6.0/prodsys/conf/logging.ini
+-rw-r--r--   0        0        0     1155 2024-01-07 23:00:16.874004 prodsys-0.6.0/prodsys/conf/logging_config.py
+-rw-r--r--   0        0        0      148 2023-10-11 11:05:22.073479 prodsys-0.6.0/prodsys/control/__init__.py
+-rw-r--r--   0        0        0     9030 2024-05-04 14:52:14.094243 prodsys-0.6.0/prodsys/control/routing_control_env.py
+-rw-r--r--   0        0        0     8489 2023-10-11 11:05:22.073479 prodsys-0.6.0/prodsys/control/sequencing_control_env.py
+-rw-r--r--   0        0        0     2236 2024-05-04 14:52:14.094243 prodsys-0.6.0/prodsys/express/__init__.py
+-rw-r--r--   0        0        0      603 2023-10-11 11:05:22.073479 prodsys-0.6.0/prodsys/express/core.py
+-rw-r--r--   0        0        0     1589 2024-05-04 14:52:14.094243 prodsys-0.6.0/prodsys/express/node.py
+-rw-r--r--   0        0        0    11649 2024-05-04 14:52:14.098787 prodsys-0.6.0/prodsys/express/process.py
+-rw-r--r--   0        0        0     2477 2024-05-04 14:52:14.098787 prodsys-0.6.0/prodsys/express/product.py
+-rw-r--r--   0        0        0     7129 2024-05-04 14:52:14.101328 prodsys-0.6.0/prodsys/express/production_system.py
+-rw-r--r--   0        0        0     8295 2024-05-04 14:52:14.101328 prodsys-0.6.0/prodsys/express/resources.py
+-rw-r--r--   0        0        0     2573 2024-05-04 14:52:14.101328 prodsys-0.6.0/prodsys/express/sink.py
+-rw-r--r--   0        0        0     3413 2024-05-04 14:52:14.101328 prodsys-0.6.0/prodsys/express/source.py
+-rw-r--r--   0        0        0     7554 2024-05-01 07:15:45.742369 prodsys-0.6.0/prodsys/express/state.py
+-rw-r--r--   0        0        0     4884 2024-05-04 14:52:14.101328 prodsys-0.6.0/prodsys/express/time_model.py
+-rw-r--r--   0        0        0      913 2023-10-11 11:05:22.089564 prodsys-0.6.0/prodsys/factories/__init__.py
+-rw-r--r--   0        0        0     3400 2024-05-04 14:52:14.101328 prodsys-0.6.0/prodsys/factories/link_transport_process_updater.py
+-rw-r--r--   0        0        0     1745 2024-05-04 14:52:14.101328 prodsys-0.6.0/prodsys/factories/node_factory.py
+-rw-r--r--   0        0        0     3752 2024-05-04 14:52:14.109195 prodsys-0.6.0/prodsys/factories/process_factory.py
+-rw-r--r--   0        0        0     6358 2024-03-10 14:05:36.923357 prodsys-0.6.0/prodsys/factories/product_factory.py
+-rw-r--r--   0        0        0     1992 2024-03-10 14:05:36.923357 prodsys-0.6.0/prodsys/factories/queue_factory.py
+-rw-r--r--   0        0        0    11157 2024-05-04 14:52:14.109943 prodsys-0.6.0/prodsys/factories/resource_factory.py
+-rw-r--r--   0        0        0     3268 2023-10-11 11:05:22.089564 prodsys-0.6.0/prodsys/factories/sink_factory.py
+-rw-r--r--   0        0        0     5089 2024-01-07 23:00:16.890715 prodsys-0.6.0/prodsys/factories/source_factory.py
+-rw-r--r--   0        0        0     2856 2023-10-11 11:05:22.089564 prodsys-0.6.0/prodsys/factories/state_factory.py
+-rw-r--r--   0        0        0     2045 2023-10-11 11:05:22.089564 prodsys-0.6.0/prodsys/factories/time_model_factory.py
+-rw-r--r--   0        0        0     1583 2024-05-04 14:52:14.111436 prodsys-0.6.0/prodsys/models/__init__.py
+-rw-r--r--   0        0        0      541 2023-10-11 11:05:22.089564 prodsys-0.6.0/prodsys/models/core_asset.py
+-rw-r--r--   0        0        0     1233 2024-05-04 14:52:14.111436 prodsys-0.6.0/prodsys/models/node_data.py
+-rw-r--r--   0        0        0     2971 2024-04-26 10:14:01.064800 prodsys-0.6.0/prodsys/models/performance_data.py
+-rw-r--r--   0        0        0     9369 2024-04-19 09:06:03.048928 prodsys-0.6.0/prodsys/models/performance_indicators.py
+-rw-r--r--   0        0        0    14397 2024-05-04 14:52:14.113445 prodsys-0.6.0/prodsys/models/processes_data.py
+-rw-r--r--   0        0        0     6357 2024-05-04 14:20:57.302536 prodsys-0.6.0/prodsys/models/product_data.py
+-rw-r--r--   0        0        0     1931 2024-05-04 14:20:57.303890 prodsys-0.6.0/prodsys/models/queue_data.py
+-rw-r--r--   0        0        0    12335 2024-05-04 14:52:14.113445 prodsys-0.6.0/prodsys/models/resource_data.py
+-rw-r--r--   0        0        0    10745 2024-05-04 14:52:14.115031 prodsys-0.6.0/prodsys/models/scenario_data.py
+-rw-r--r--   0        0        0     2846 2024-05-04 14:20:57.305926 prodsys-0.6.0/prodsys/models/sink_data.py
+-rw-r--r--   0        0        0     4059 2024-05-04 14:20:57.312957 prodsys-0.6.0/prodsys/models/source_data.py
+-rw-r--r--   0        0        0    13852 2024-05-04 14:20:57.312957 prodsys-0.6.0/prodsys/models/state_data.py
+-rw-r--r--   0        0        0     6642 2024-05-04 14:20:57.312957 prodsys-0.6.0/prodsys/models/time_model_data.py
+-rw-r--r--   0        0        0     2870 2023-10-11 11:05:22.105207 prodsys-0.6.0/prodsys/optimization/__init__.py
+-rw-r--r--   0        0        0    12500 2024-05-04 14:52:14.115836 prodsys-0.6.0/prodsys/optimization/evolutionary_algorithm.py
+-rw-r--r--   0        0        0    28223 2024-05-04 14:20:57.312957 prodsys-0.6.0/prodsys/optimization/math_opt.py
+-rw-r--r--   0        0        0     4642 2024-05-04 14:20:57.321008 prodsys-0.6.0/prodsys/optimization/optimization_analysis.py
+-rw-r--r--   0        0        0    46203 2024-05-04 14:52:14.116698 prodsys-0.6.0/prodsys/optimization/optimization_util.py
+-rw-r--r--   0        0        0     9601 2024-05-04 14:52:14.118464 prodsys-0.6.0/prodsys/optimization/simulated_annealing.py
+-rw-r--r--   0        0        0    11895 2024-05-04 14:52:14.119595 prodsys-0.6.0/prodsys/optimization/tabu_search.py
+-rw-r--r--   0        0        0     1704 2023-10-11 11:05:22.105207 prodsys-0.6.0/prodsys/simulation/__init__.py
+-rw-r--r--   0        0        0    31006 2024-05-04 14:52:14.120801 prodsys-0.6.0/prodsys/simulation/control.py
+-rw-r--r--   0        0        0     6855 2024-05-01 15:14:08.116047 prodsys-0.6.0/prodsys/simulation/logger.py
+-rw-r--r--   0        0        0      459 2024-05-04 14:52:14.122204 prodsys-0.6.0/prodsys/simulation/node.py
+-rw-r--r--   0        0        0     3765 2024-05-04 14:52:14.123256 prodsys-0.6.0/prodsys/simulation/observer.py
+-rw-r--r--   0        0        0     9599 2024-05-04 14:52:14.124428 prodsys-0.6.0/prodsys/simulation/proces_models.py
+-rw-r--r--   0        0        0    11900 2024-05-04 14:52:14.125901 prodsys-0.6.0/prodsys/simulation/process.py
+-rw-r--r--   0        0        0    10255 2024-05-04 14:52:14.125901 prodsys-0.6.0/prodsys/simulation/product.py
+-rw-r--r--   0        0        0     5716 2024-05-04 14:52:14.125901 prodsys-0.6.0/prodsys/simulation/request.py
+-rw-r--r--   0        0        0    18086 2024-05-04 14:52:14.125901 prodsys-0.6.0/prodsys/simulation/resources.py
+-rw-r--r--   0        0        0    10029 2024-05-04 14:52:14.125901 prodsys-0.6.0/prodsys/simulation/route_finder.py
+-rw-r--r--   0        0        0    15942 2024-05-04 14:52:14.132408 prodsys-0.6.0/prodsys/simulation/router.py
+-rw-r--r--   0        0        0     3199 2024-04-26 10:14:01.122122 prodsys-0.6.0/prodsys/simulation/sim.py
+-rw-r--r--   0        0        0     2260 2024-05-04 14:20:57.328996 prodsys-0.6.0/prodsys/simulation/sink.py
+-rw-r--r--   0        0        0     3809 2024-05-04 14:20:57.328996 prodsys-0.6.0/prodsys/simulation/source.py
+-rw-r--r--   0        0        0    29728 2024-05-04 14:52:14.132408 prodsys-0.6.0/prodsys/simulation/state.py
+-rw-r--r--   0        0        0     2232 2024-01-07 23:00:16.919358 prodsys-0.6.0/prodsys/simulation/store.py
+-rw-r--r--   0        0        0     7191 2024-05-04 14:52:14.135356 prodsys-0.6.0/prodsys/simulation/time_model.py
+-rw-r--r--   0        0        0       61 2023-10-11 11:05:22.120833 prodsys-0.6.0/prodsys/util/__init__.py
+-rw-r--r--   0        0        0     8056 2023-11-06 17:14:55.559034 prodsys-0.6.0/prodsys/util/kpi_visualization.py
+-rw-r--r--   0        0        0    30349 2024-05-04 14:20:57.328996 prodsys-0.6.0/prodsys/util/post_processing.py
+-rw-r--r--   0        0        0    12893 2024-05-04 14:52:14.136563 prodsys-0.6.0/prodsys/util/runner.py
+-rw-r--r--   0        0        0     2657 2023-12-24 16:10:02.245387 prodsys-0.6.0/prodsys/util/statistical_functions.py
+-rw-r--r--   0        0        0     4390 2024-05-04 14:52:14.137675 prodsys-0.6.0/prodsys/util/util.py
+-rw-r--r--   0        0        0     1605 2024-05-04 14:52:14.138455 prodsys-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6375 2024-05-04 14:20:57.249746 prodsys-0.6.0/README.md
+-rw-r--r--   0        0        0     8405 1970-01-01 00:00:00.000000 prodsys-0.6.0/PKG-INFO
```

### Comparing `prodsys-0.5.3/LICENSE` & `prodsys-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/adapters/__init__.py` & `prodsys-0.6.0/prodsys/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/adapters/adapter.py` & `prodsys-0.6.0/prodsys/adapters/adapter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from hashlib import md5
 import warnings
 from typing import List, Any, Set, Optional, Tuple, Union
+from numpy import isin
 from pydantic import BaseModel, validator, ValidationError
 
 import logging
 logger = logging.getLogger(__name__)
 
 from prodsys.models import (
     product_data,
     queue_data,
     resource_data,
+    node_data,
     time_model_data,
     state_data,
     processes_data,
     sink_data,
     source_data,
     scenario_data,
 )
@@ -270,29 +272,31 @@
     Args:
         ID (str, optional): ID of the production system. Defaults to "".
         seed (int, optional): Seed for the random number generator used in simulation. Defaults to 0.
         time_model_data (List[time_model_data.TIME_MODEL_DATA], optional): List of time models used by the entities in the production system. Defaults to [].
         state_data (List[state_data.STATE_DATA_UNION], optional): List of states used by the resources in the production system. Defaults to [].
         process_data (List[processes_data.PROCESS_DATA_UNION], optional): List of processes required by products and provided by resources in the production system. Defaults to [].
         queue_data (List[queue_data.QueueData], optional): List of queues used by the resources, sources and sinks in the production system. Defaults to [].
+        node_data (List[resource_data.NodeData], optional): List of nodes in the production system. Defaults to [].
         resource_data (List[resource_data.RESOURCE_DATA_UNION], optional): List of resources in the production system. Defaults to [].
-        product_data (List[product_data.ProductData], optional): List of products in the production system. Defaults to [].
+        product_data (List[product_data.ProductData], optional): List of products in the production system. Defaults to []
         sink_data (List[sink_data.SinkData], optional): List of sinks in the production system. Defaults to [].
         source_data (List[source_data.SourceData], optional): List of sources in the production system. Defaults to [].
         scenario_data (Optional[scenario_data.ScenarioData], optional): Scenario data of the production system used for optimization. Defaults to None.
         valid_configuration (bool, optional): Indicates if the configuration is valid. Defaults to True.
         reconfiguration_cost (float, optional): Cost of reconfiguration in a optimization scenario. Defaults to 0.
     """
     # TODO: add check, that throws an error, if items have the same ID!
     ID: str = ""
     seed: int = 0
     time_model_data: List[time_model_data.TIME_MODEL_DATA] = []
     state_data: List[state_data.STATE_DATA_UNION] = []
     process_data: List[processes_data.PROCESS_DATA_UNION] = []
     queue_data: List[queue_data.QueueData] = []
+    node_data: List[node_data.NodeData] = []
     resource_data: List[resource_data.RESOURCE_DATA_UNION] = []
     product_data: List[product_data.ProductData] = []
     sink_data: List[sink_data.SinkData] = []
     source_data: List[source_data.SourceData] = []
     scenario_data: Optional[scenario_data.ScenarioData] = None
 
 
@@ -684,14 +688,15 @@
             ("".join(
                 [
                 *sorted([time_model.hash() for time_model in self.time_model_data]),
                 *sorted([state.hash(self) for state in self.state_data]),
                 *sorted([process.hash(self) for process in self.process_data]),
                 *sorted([res.hash(self) for res in self.resource_data]),
                 *sorted([queue.hash() for queue in self.queue_data]),
+                *sorted([node.hash() for node in self.node_data]),
                 *sorted([product.hash(self) for product in self.product_data]),
                 *sorted([sink.hash(self) for sink in self.sink_data]),
                 *sorted([source.hash(self) for source in self.source_data])
                 ]
             )).encode("utf-8")
             ).hexdigest()
 
@@ -861,59 +866,121 @@
             for process in resource.process_ids:
                 available_processes.add(process)
         if required_processes > available_processes:
             raise ValueError(
                 f"The processes {required_processes - available_processes} are not available."
             )
 
-    def physical_validation(self):
+    def validate_configuration(self):
         """
         Checks if the configuration is physically valid, i.e. if all resources are positioned at different locations and if all required processes are available.
 
         Raises:
             ValueError: If multiple objects are positioned at the same location.
             ValueError: If not all required process are available.
+            ValueError: If not all links are available for LinkTransportProcesses.
         """
-        if not check_redudant_locations(self):
-            raise ValueError(f"Multiple objects are positioned at the same location.")
-        if not check_required_processes_in_resources_available(self):
-            raise ValueError(f"Not all required process are available at resources.")
-        if not check_required_processes_in_resources_available(self):
-            raise ValueError(f"Not all required process are available at resources.")
+        assert_no_redudant_locations(self)
+        assert_required_processes_in_resources_available(self)
+        assert_all_links_available(self)
 
 
 def remove_duplicate_locations(input_list: List[List[float]]) -> List[List[float]]:
     return [list(x) for x in set(tuple(x) for x in input_list)]
 
 
-def check_redudant_locations(adapter: ProductionSystemAdapter) -> bool:
+def assert_no_redudant_locations(adapter: ProductionSystemAdapter):
+    """
+    Asserts that no multiple objects are positioned at the same location.
+
+    Args:
+        adapter (ProductionSystemAdapter): Production system configuration
+
+    Raises:
+        ValueError: If multiple objects are positioned at the same location.
+    """
     machine_locations = [machine.location for machine in get_machines(adapter)]
     source_locations = remove_duplicate_locations(
         [source.location for source in adapter.source_data]
     )
     sink_locations = remove_duplicate_locations(
         [sink.location for sink in adapter.sink_data]
     )
     positions = machine_locations + source_locations + sink_locations
-    if any(positions.count(location) > 1 for location in positions):
-        return False
-    return True
+    for location in positions:
+        if positions.count(location) > 1:
+            raise ValueError(f"Multiple objects are positioned at the same location: {location}")
+
+def assert_all_links_available(adapter: ProductionSystemAdapter):
+    """
+    Asserts that all links are valid, so that the start and target of the link are valid locations.
+
+    Args:
+        adapter (ProductionSystemAdapter): Production system configuration
+
+    Raises:
+        ValueError: If the start or target of a link is not a valid location.
+    """
+    link_transport_processes = [process for process in adapter.process_data if isinstance(process, processes_data.LinkTransportProcessData)]
+    if not link_transport_processes:
+        return 
+    nodes = get_set_of_IDs(adapter.node_data)
+    resources = get_set_of_IDs(adapter.resource_data)
+    sources = get_set_of_IDs(adapter.source_data)
+    sinks = get_set_of_IDs(adapter.sink_data)
+    all_location_ids = nodes | resources | sources | sinks
+    for link_transport_process in link_transport_processes:
+        link_pairs: List[List[str]] = []
+        if isinstance(link_transport_process.links, dict):
+            for start, targets in link_transport_process.links.items():
+                for target in targets:
+                    link_pairs.append([start, target])
+        else:
+            link_pairs = link_transport_process.links
+        for start, target in link_pairs:
+            if start not in all_location_ids:
+                raise ValueError(
+                    f"The link from {start} to {target} of process {link_transport_process.ID} is not a valid location because {start} is no valid location id."
+                )
+            if target not in all_location_ids:
+                raise ValueError(
+                    f"The link from {start} to {target} of process {link_transport_process.ID} is not a valid location because {target} is no valid location id."
+                )
 
 
 def check_for_clean_compound_processes(
         adapter_object: ProductionSystemAdapter,
 ) -> bool:
+    """
+    Checks that the compound processes are clean, i.e. that they do not contain compund processes and normal processes at the same time.
+
+    Args:
+        adapter_object (ProductionSystemAdapter): Production system configuration
+
+    Returns:
+        bool: True if the compound processes are clean, False otherwise
+    """
     possible_production_processes_ids = get_possible_production_processes_IDs(adapter_object)
     if any(isinstance(process_id, tuple) for process_id in possible_production_processes_ids) and any(isinstance(process_id, str) for process_id in possible_production_processes_ids):
         return False
     return True
 
 def get_possible_production_processes_IDs(
     adapter_object: ProductionSystemAdapter,
 ) -> Union[List[str], List[Tuple[str, ...]]]:
+    """
+    Returns all possible production processes IDs that can be used in the production system. 
+    Compund processes are grouped as touples, whereas individual processes are represented as strings.
+
+    Args:
+        adapter_object (ProductionSystemAdapter): Production system configuration
+
+    Returns:
+        Union[List[str], List[Tuple[str, ...]]]: List of production process IDs
+    """
     possible_processes = [process for process in adapter_object.process_data if not isinstance(process, processes_data.TransportProcessData) and not isinstance(process, processes_data.RequiredCapabilityProcessData)]  
     compund_processes = [process for process in adapter_object.process_data if isinstance(process, processes_data.CompoundProcessData)]
     compound_process_id_tuples = [tuple(compound_process.process_ids) for compound_process in compund_processes]
 
     compound_processes_ids = set([compound_process.ID for compound_process in compund_processes])
     compound_processes_contained_process_ids = set(util.flatten(compound_process_id_tuples))
     individual_processes_ids = [process.ID for process in possible_processes if process.ID not in compound_processes_contained_process_ids and process.ID not in compound_processes_ids]
@@ -936,35 +1003,38 @@
     adapter_object: ProductionSystemAdapter, process_ids: List[str]
 ) -> List[processes_data.PROCESS_DATA_UNION]:
     processes = []
     for process_id in process_ids:
         for process in adapter_object.process_data:
             if process.ID == process_id and isinstance(process, processes_data.ProductionProcessData):
                 processes.append(process)
+                break
     return processes
 
 
 def get_transport_processes_from_ids(
     adapter_object: ProductionSystemAdapter, process_ids: List[str]
 ) -> List[processes_data.PROCESS_DATA_UNION]:
     processes = []
     for process_id in process_ids:
         for process in adapter_object.process_data:
-            if process.ID == process_id and isinstance(process, processes_data.TransportProcessData):
+            if process.ID == process_id and isinstance(process, processes_data.TransportProcessData) and not (hasattr(process, "capability") and getattr(process, "capability")):
                 processes.append(process)
+                break
     return processes
 
 def get_capability_processes_from_ids(
         adapter_object: ProductionSystemAdapter, process_ids: List[str]
 ) -> List[processes_data.PROCESS_DATA_UNION]:
     processes = []
     for process_id in process_ids:
         for process in adapter_object.process_data:
-            if process.ID == process_id and isinstance(process, processes_data.CapabilityProcessData):
+            if process.ID == process_id and (isinstance(process, processes_data.CapabilityProcessData) or (hasattr(process, "capability") and getattr(process, "capability"))):
                 processes.append(process)
+                break
     return processes
 
 
 def get_compound_processes_from_ids(
     adapter_object: ProductionSystemAdapter, process_ids: List[str]
 ) -> List[processes_data.PROCESS_DATA_UNION]:
     processes = []
@@ -1038,51 +1108,86 @@
             if len(processes) > 1:
                 raise ValueError(f"Multiple processes with ID {process_id} found.")
             process = processes[0]
             processes.append(process)
     return processes
 
 
-def check_production_processes_available(available: List[processes_data.ProductionProcessData], required: List[processes_data.ProductionProcessData]) -> bool:
+def assert_production_processes_available(available: List[processes_data.ProductionProcessData], required: List[processes_data.ProductionProcessData]):
+    """
+    Checks if all required production processes are available.
+
+    Args:
+        available (List[processes_data.ProductionProcessData]): production processes that are available in the production system resources
+        required (List[processes_data.ProductionProcessData]): production processes that are required from the products
+    Raises:
+        ValueError: If required production processes are not available
+    """
     available = set([process.ID for process in available])
     required = set([process.ID for process in required])
     if required - available != set():
-        return False
-    return True
+        raise ValueError(f"Required production processes {required - available} are not available.")
+
+def assert_transport_processes_available(available: List[processes_data.TransportProcessData], required: List[processes_data.TransportProcessData]):
+    """
+    Checks if all required transport processes are available.
 
-def check_transport_processes_available(available: List[processes_data.TransportProcessData], required: List[processes_data.TransportProcessData]) -> bool:
+    Args:
+        available (List[processes_data.TransportProcessData]): transport processes that are available in the production system resources
+        required (List[processes_data.TransportProcessData]): transport processes that are required from the products
+
+    Raises:
+        ValueError: If required transport processes are not available
+    """
     available = set([process.ID for process in available])
     required = set([process.ID for process in required])
     if required - available != set():
-        return False
-    return True
+        raise ValueError(f"Required transport processes {required - available} are not available.")
+
+def assert_capability_processes_available(available: List[processes_data.CapabilityProcessData], required: List[processes_data.CapabilityProcessData]):
+    """
+    Checks if all required capability processes are available.
 
-def check_capability_processes_available(available: List[processes_data.CapabilityProcessData], required: List[processes_data.CapabilityProcessData]) -> bool:
+    Args:
+        available (List[processes_data.CapabilityProcessData]): capability processes that are available in the production system resources
+        required (List[processes_data.CapabilityProcessData]): capability processes that are required from the products
+
+    Raises:
+        ValueError: If required capability processes are not available
+    """
     available = set([process.capability for process in available])
     required = set([process.capability for process in required])
     if required - available != set():
-        return False
-    return True
+        raise ValueError(f"Required capability processes {required - available} are not available.")
+
+def assert_required_processes_in_resources_available(configuration: ProductionSystemAdapter):
+    """
+    Asserts that all required processes are available in the resources that are requested by the products in the configuration.
 
-def check_required_processes_in_resources_available(configuration: ProductionSystemAdapter) -> bool:
-    available = list(util.flatten([resource.process_ids for resource in configuration.resource_data]))
-    required = util.flatten([product.processes + [product.transport_process] for product in configuration.product_data if not isinstance(product.processes, dict)])
+    Args:
+        configuration (ProductionSystemAdapter): Production system configuration
+
+    Raises:
+        ValueError: If specified processes contain some logical errors.
+    """
+    available = set(list(util.flatten([resource.process_ids for resource in configuration.resource_data])))
+    required = util.flatten([product.processes for product in configuration.product_data if not isinstance(product.processes, dict)])
     required_dict_processes = util.flatten([list(product.processes.keys()) for product in configuration.product_data if isinstance(product.processes, dict)])
-    required = list(required) + list(required_dict_processes)
+    required = set(list(required) + list(required_dict_processes) + [product.transport_process for product in configuration.product_data])
 
     required_production_processes = get_production_processes_from_ids(configuration, required)
     required_transport_processes = get_transport_processes_from_ids(configuration, required)
     required_capability_processes = get_capability_processes_from_ids(configuration, required)
     required_capability_processes += get_required_capability_processes_from_ids(configuration, required)
     available_production_processes = get_production_processes_from_ids(configuration, available)
     available_transport_processes = get_transport_processes_from_ids(configuration, available)
     available_capability_processes = get_capability_processes_from_ids(configuration, available)
     available_required_capability_processes = get_required_capability_processes_from_ids(configuration, available)
     if available_required_capability_processes:
-        raise ValueError(f"Required capability processes {available_required_capability_processes} should not be available for resources since no time model is given.")
+        raise ValueError(f"Required capability processes {available_required_capability_processes} should not be used for resources since no time model is given.")
 
 
     all_process_ids = set([process.ID for process in configuration.process_data])
     compound_processes = get_compound_processes_from_ids(configuration, all_process_ids)
     for compound_process in compound_processes:
         if not all(process_id in all_process_ids for process_id in compound_process.process_ids):
             raise ValueError(f"Compound process {compound_process.ID} contains processes that are not available in the data.")
@@ -1093,14 +1198,10 @@
     required_transport_processes += get_contained_transport_processes_from_compound_processes(configuration, required_compound_processes)
     required_capability_processes += get_contained_capability_processes_from_compound_processes(configuration, required_compound_processes)
     required_capability_processes += get_contained_required_capability_processes_from_compound_processes(configuration, required_compound_processes)
     available_production_processes += get_contained_production_processes_from_compound_processes(configuration, available_compound_processes)
     available_transport_processes += get_contained_transport_processes_from_compound_processes(configuration, available_compound_processes)
     available_capability_processes += get_contained_capability_processes_from_compound_processes(configuration, available_compound_processes)
 
-    if not check_production_processes_available(available_production_processes, required_production_processes):
-        return False
-    if not check_transport_processes_available(available_transport_processes, required_transport_processes):
-        return False
-    if not check_capability_processes_available(available_capability_processes, required_capability_processes):
-        return False
-    return True
+    assert_production_processes_available(available_production_processes, required_production_processes)
+    assert_transport_processes_available(available_transport_processes, required_transport_processes)
+    assert_capability_processes_available(available_capability_processes, required_capability_processes)
```

### Comparing `prodsys-0.5.3/prodsys/adapters/json_adapter.py` & `prodsys-0.6.0/prodsys/adapters/json_adapter.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from prodsys.adapters import adapter
 
 from prodsys.models import (
     product_data,
     queue_data,
     resource_data,
+    node_data,
     time_model_data,
     state_data,
     processes_data,
     sink_data,
     source_data,
 )
 
@@ -33,21 +34,23 @@
         ID (str, optional): ID of the production system. Defaults to "".
         seed (int, optional): Seed for the random number generator used in simulation. Defaults to 0.
         time_model_data (List[time_model_data.TIME_MODEL_DATA], optional): List of time models used by the entities in the production system. Defaults to [].
         state_data (List[state_data.STATE_DATA_UNION], optional): List of states used by the resources in the production system. Defaults to [].
         process_data (List[processes_data.PROCESS_DATA_UNION], optional): List of processes required by products and provided by resources in the production system. Defaults to [].
         queue_data (List[queue_data.QueueData], optional): List of queues used by the resources, sources and sinks in the production system. Defaults to [].
         resource_data (List[resource_data.RESOURCE_DATA_UNION], optional): List of resources in the production system. Defaults to [].
+        node_data (List[resource_data.NodeData], optional): List of nodes in the production system. Defaults to [].
         product_data (List[product_data.ProductData], optional): List of products in the production system. Defaults to [].
         sink_data (List[sink_data.SinkData], optional): List of sinks in the production system. Defaults to [].
         source_data (List[source_data.SourceData], optional): List of sources in the production system. Defaults to [].
         scenario_data (Optional[scenario_data.ScenarioData], optional): Scenario data of the production system used for optimization. Defaults to None.
         valid_configuration (bool, optional): Indicates if the configuration is valid. Defaults to True.
         reconfiguration_cost (float, optional): Cost of reconfiguration in a optimization scenario. Defaults to 0.
     """
+
     def read_data_old(self, file_path: str, scenario_file_path: Optional[str] = None):
         """
         Reads the data from the given file path and scenario file path.
 
         Args:
             file_path (str): File path for the production system configuration
             scenario_file_path (Optional[str], optional): File path for the scenario data. Defaults to None.
@@ -64,14 +67,15 @@
         self.process_data = self.create_objects_from_configuration_data_old(
             data["processes"], processes_data.PROCESS_DATA_UNION
         )
 
         self.queue_data = self.create_objects_from_configuration_data_old(data["queues"], queue_data.QueueData)
         self.resource_data = self.create_objects_from_configuration_data_old(data["resources"], resource_data.RESOURCE_DATA_UNION)
         self.product_data = self.create_objects_from_configuration_data_old(data["products"], product_data.ProductData)
+        self.node_data = self.create_objects_from_configuration_data(data["links"], node_data.NodeData)
         self.sink_data = self.create_objects_from_configuration_data_old(data["sinks"], sink_data.SinkData)
         self.source_data = self.create_objects_from_configuration_data_old(data["sources"], source_data.SourceData)
         if scenario_file_path:
             self.read_scenario(scenario_file_path)
 
     def read_data(self, file_path: str, scenario_file_path: Optional[str] = None):
         """
@@ -97,14 +101,16 @@
         self.process_data = self.create_objects_from_configuration_data(
             data["process_data"], processes_data.PROCESS_DATA_UNION
         )
         self.queue_data = self.create_objects_from_configuration_data(data["queue_data"], queue_data.QueueData)
         self.resource_data = self.create_objects_from_configuration_data(data["resource_data"], resource_data.RESOURCE_DATA_UNION)
         self.product_data = self.create_objects_from_configuration_data(data["product_data"], product_data.ProductData)
         self.sink_data = self.create_objects_from_configuration_data(data["sink_data"], sink_data.SinkData)
+        if "node_data" in data:
+            self.node_data = self.create_objects_from_configuration_data(data["node_data"], node_data.NodeData)
         self.source_data = self.create_objects_from_configuration_data(data["source_data"], source_data.SourceData)
         if scenario_file_path:
             self.read_scenario(scenario_file_path)
     
     def create_objects_from_configuration_data_old(
         self, configuration_data: Dict[str, Any], type
     ):  
@@ -136,16 +142,18 @@
     def get_dict_object_of_adapter(self) -> dict:
         data = {
                 "ID": self.ID,
                 "seed": self.seed,
                 "time_model_data": self.get_list_of_dict_objects(self.time_model_data),
                 "state_data": self.get_list_of_dict_objects(self.state_data),
                 "process_data": self.get_list_of_dict_objects(self.process_data),
+                "node_data": self.get_list_of_dict_objects(self.node_data),
                 "queue_data": self.get_list_of_dict_objects(self.queue_data),
                 "resource_data": self.get_list_of_dict_objects(self.resource_data),
+                "node_data": self.get_list_of_dict_objects(self.node_data),
                 "product_data": self.get_list_of_dict_objects(self.product_data),
                 "sink_data": self.get_list_of_dict_objects(self.sink_data),
                 "source_data": self.get_list_of_dict_objects(self.source_data)
         }
         return data
     
     def write_scenario_data(self, file_path: str) -> None:
```

### Comparing `prodsys-0.5.3/prodsys/conf/logging.ini` & `prodsys-0.6.0/prodsys/conf/logging.ini`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/conf/logging_config.py` & `prodsys-0.6.0/prodsys/conf/logging_config.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/control/routing_control_env.py` & `prodsys-0.6.0/prodsys/control/routing_control_env.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         self.observation_space = observation_space
         self.action_space = action_space
         self.render_mode = render_mode
 
         self.runner = runner.Runner(adapter=self.adapter)
 
         self.router: router.Router = None
-        self.possible_resources: List[resources.Resource] = []
+        self.possible_requests: List[request.Request] = []
         self.chosen_resource: Optional[resources.Resource] = None
         self.interrupt_simulation_event: events.Event = None
         self.observers: List[observer.ResourceObserver] = []
         self.step_count = 0
         self.reward = 0
 
     @abstractmethod
@@ -119,15 +119,15 @@
         """
         super().reset(seed=seed)
 
         self.runner.initialize_simulation()
         self.interrupt_simulation_event = events.Event(self.runner.env)
         self.chose_resource_event = events.Event(self.runner.env)
         agent_routing_heuristic = partial(router.agent_routing_heuristic, self)
-        self.router = router.SimpleRouter(self.runner.resource_factory, self.runner.sink_factory, agent_routing_heuristic)  
+        self.router = router.Router(self.runner.resource_factory, self.runner.sink_factory, agent_routing_heuristic)  
         
         sources = self.runner.source_factory.sources
         for source in sources:
             source.router = self.router
         
         self.observers = []
         for resource in self.runner.resource_factory.resources:
@@ -143,22 +143,22 @@
         info = self.get_info()
 
         if self.render_mode == "human":
             self.render()
 
         return observation, info
     
-    def set_possible_resources(self, resources: List[resources.Resource]):
+    def set_possible_requests(self, requests: List[request.Request]):
         """
-        Set possible resources for the RL agent environment.
+        Set possible requests for the RL agent environment.
 
         Args:
-            resources (List[resources.Resource]): The possible resources.
+            resources (List[request.Request]): The possible requests to route.
         """
-        self.possible_resources = resources
+        self.possible_requests = requests
 
     def get_chosen_resource(self) -> resources.Resource:
         """
         Get the chosen resource of the RL agent for the router.
 
         Returns:
             resources.Resource: The chosen resource.
@@ -175,21 +175,21 @@
         Returns:
             Tuple[np.ndarray, float, bool, dict]: The observation, reward, done, and info.
         """
         # TODO: implement action masking here!
         resource_index = np.argmax(action)
 
         self.chosen_resource = self.runner.resource_factory.resources[resource_index]
-        if not self.chosen_resource.data.ID in [r.data.ID for r in self.possible_resources]:
+        if not self.chosen_resource.data.ID in [r.resource.data.ID for r in self.possible_requests]:
             invalid_action = True
-            self.chosen_resource = np.random.choice(self.possible_resources)
+            self.chosen_resource = np.random.choice(self.possible_requests)
         else:
             invalid_action = False
 
-        self.possible_resources.sort(key=lambda r: r.data.ID == self.chosen_resource.data.ID, reverse=True)
+        self.possible_requests.sort(key=lambda r: r.resource.data.ID == self.chosen_resource.data.ID, reverse=True)
 
         self.runner.env.run_until(until=self.interrupt_simulation_event)
         self.step_count += 1
         self.interrupt_simulation_event = events.Event(self.runner.env)
         
         terminated = self.get_termination_condition()
         self.reward = self.get_reward(invalid_action)
```

### Comparing `prodsys-0.5.3/prodsys/control/sequencing_control_env.py` & `prodsys-0.6.0/prodsys/control/sequencing_control_env.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/express/__init__.py` & `prodsys-0.6.0/prodsys/express/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,18 @@
     FunctionTimeModel,
     SequentialTimeModel,
     ManhattanDistanceTimeModel,
 )
 from prodsys.express.process import (
     ProductionProcess,
     CapabilityProcess,
+    RequiredCapabilityProcess,
     TransportProcess,
+    LinkTransportProcess,
 )
 from prodsys.express.state import SetupState, BreakDownState, ProcessBreakdownState
 from prodsys.express.resources import ProductionResource, TransportResource
+from prodsys.express.node import Node
 from prodsys.express.product import Product
 from prodsys.express.source import Source
 from prodsys.express.sink import Sink
 from prodsys.express.production_system import ProductionSystem
```

### Comparing `prodsys-0.5.3/prodsys/express/core.py` & `prodsys-0.6.0/prodsys/express/core.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/express/product.py` & `prodsys-0.6.0/prodsys/express/product.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from uuid import uuid1
 
 from pydantic import Field
 from pydantic.dataclasses import dataclass
 
 from prodsys.models import product_data
 
-from prodsys.express import process, core
+from prodsys.express import core, process
 
 @dataclass
 class Product(core.ExpressObject):
     """
     Class that represents a product.
 
     Args:
@@ -43,15 +43,15 @@
         psx.Product(
             processes=[welding_process_1, welding_process_2],
             transport_process=transport_process
         )
         ```
     """
     processes: List[Union[process.ProductionProcess, process.CapabilityProcess]]
-    transport_process: process.TransportProcess
+    transport_process: Union[process.TransportProcess, process.RequiredCapabilityProcess]
     ID: Optional[str] = Field(default_factory=lambda: str(uuid1()))
 
     def to_model(self) -> product_data.ProductData:
         """
         Converts the `prodsys.express` object to a data object from `prodsys.models`.
 
         Returns:
```

### Comparing `prodsys-0.5.3/prodsys/express/production_system.py` & `prodsys-0.6.0/prodsys/express/production_system.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from typing import List, Optional, Union
-from uuid import uuid1
 
-from abc import ABC
 
-from pydantic import Field, conlist
+from pydantic import Field
 from pydantic.dataclasses import dataclass
 
-from prodsys.models import core_asset, source_data, queue_data
 import prodsys
 from prodsys.util import util
 
 from prodsys.express import (
     core,
+    node,
     product,
     resources,
     source,
     sink,
     process,
     time_model,
     state,
+    process
 )
 
 
 def remove_duplicate_items(
     items: List[
         Union[
             resources.Resource,
@@ -88,41 +87,53 @@
         """
         products = [source.product for source in self.sources] + [
             sink.product for sink in self.sinks
         ]
         products = remove_duplicate_items(products)
         processes = list(
             util.flatten_object(
-                [product.processes for product in products]
+                [product.processes for product in products]+
+                [product.transport_process for product in products]
                 + [resource.processes for resource in self.resources]
             )
         )
         processes = remove_duplicate_items(processes)
 
+        nodes = []
+        for process_instance in processes:
+            if not isinstance(process_instance, process.LinkTransportProcess):
+                continue
+            for link in process_instance.links:
+                for link_element in link:
+                    if isinstance(link_element, node.Node):
+                        nodes.append(link_element)
+        nodes = remove_duplicate_items(nodes)
+
         states = list(
             util.flatten_object([resource.states for resource in self.resources])
         )
         states = remove_duplicate_items(states)
 
         time_models = (
-            [process.time_model for process in processes]
+            [process_instance.time_model for process_instance in processes if not isinstance(process_instance, process.RequiredCapabilityProcess)]
             + [state.time_model for state in states]
             + [source.time_model for source in self.sources]
         )
         time_models += [
             s.repair_time_model
             for s in states
             if isinstance(s, state.BreakDownState)
             or isinstance(s, state.ProcessBreakdownState)
         ]
         time_models = remove_duplicate_items(time_models)
 
         time_model_data = [time_model.to_model() for time_model in time_models]
         process_data = [process.to_model() for process in processes]
         state_data = [state.to_model() for state in states]
+        nodes_data = [node.to_model() for node in nodes]
         product_data = [product.to_model() for product in products]
         resource_data = [resource.to_model() for resource in self.resources]
         source_data = [source.to_model() for source in self.sources]
         sink_data = [sink.to_model() for sink in self.sinks]
 
         queue_data = list(
             util.flatten_object(
@@ -140,15 +151,17 @@
                 + [s._input_queues for s in self.sinks]
             )
         )
         return prodsys.adapters.JsonProductionSystemAdapter(
             time_model_data=time_model_data,
             process_data=process_data,
             state_data=state_data,
+            node_data=nodes_data,
             product_data=product_data,
+            nodes_data=nodes_data,
             resource_data=resource_data,
             source_data=source_data,
             sink_data=sink_data,
             queue_data=queue_data,
         )
 
     def run(self, time_range: float = 2880, seed: int = 0):
@@ -168,15 +181,15 @@
         """
         Validates the production system. Checks if the production system is valid.
 
         Raises:
             ValueError: If the production system is not valid.
         """
         adapter = self.to_model()
-        adapter.physical_validation()
+        adapter.validate_configuration()
 
     @property
     def runner(self):
         if not self._runner:
             raise ValueError(
                 "Runner has not been initialized. Please run the simulation first with the run function."
             )
```

### Comparing `prodsys-0.5.3/prodsys/express/resources.py` & `prodsys-0.6.0/prodsys/express/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 from uuid import uuid1
 
 from abc import ABC
 
 from pydantic import Field, conlist
 from pydantic.dataclasses import dataclass
 
-from prodsys.models import core_asset, resource_data, queue_data
+from prodsys.models import resource_data, queue_data
 import prodsys
 
-from prodsys.express import process, state, core
+from prodsys.express import core, process, state
+
 
 @dataclass
 class Resource(ABC):
     """
     Abstract base class to represents a resource.
 
     Args:
@@ -30,15 +31,15 @@
         capacity (int): Capacity of the resource. Defaults to 1.
         states (Optional[List[state.STATE_UNION]], optional): States of the resource. Defaults to None.
         controller (resource_data.ControllerEnum, optional): Controller of the resource. Defaults to resource_data.ControllerEnum.PipelineController.
         control_policy (resource_data.ResourceControlPolicy, optional): Control policy of the resource. Defaults to resource_data.ResourceControlPolicy.FIFO.
         ID (str): ID of the resource.
     """
     processes: List[process.PROCESS_UNION]
-    location: conlist(float, min_items=2, max_items=2)
+    location: conlist(float, min_items=2, max_items=2) # type: ignore
     capacity: int = 1
     states: Optional[List[state.STATE_UNION]] = Field(default_factory=list)
     controller: resource_data.ControllerEnum = resource_data.ControllerEnum.PipelineController
     control_policy: Union[resource_data.ResourceControlPolicy, resource_data.TransportControlPolicy] = resource_data.ResourceControlPolicy.FIFO
     ID: Optional[str] = Field(default_factory=lambda: str(uuid1()))
 
 
@@ -141,15 +142,15 @@
         psx.TransportResource(
             processes=[transport_process],
             location=[10.0, 10.0]
         )
         ```
     """
     processes: List[process.TransportProcess]
-    location: conlist(float, min_items=2, max_items=2) = Field(default_factory=list)
+    location: conlist(float, min_items=2, max_items=2) = Field(default_factory=list) # type: ignore
     # capacity: int = 1
     # states: Optional[List[state.STATE_UNION]] = Field(default_factory=list)
     controller: resource_data.ControllerEnum = resource_data.ControllerEnum.TransportController
     control_policy: resource_data.TransportControlPolicy = resource_data.TransportControlPolicy.FIFO
     # ID: Optional[str] = Field(default_factory=lambda: str(uuid1()))
 
     def __post_init_post_parse__(self):
```

### Comparing `prodsys-0.5.3/prodsys/express/sink.py` & `prodsys-0.6.0/prodsys/express/sink.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         psx.Sink(
             product=product,
             location=[0.0, 0.0],
         )
         ```
     """
     product: product.Product
-    location: conlist(float, min_items=2, max_items=2)
+    location: conlist(float, min_items=2, max_items=2) # type: ignore
     ID: Optional[str] = Field(default_factory=lambda: str(uuid1()))
 
     _input_queues: List[queue_data.QueueData] = Field(default_factory=list, init=False)
 
     def to_model(self) -> sink_data.SinkData:
         """
         Converts the `prodsys.express` object to a data object from `prodsys.models`.
```

### Comparing `prodsys-0.5.3/prodsys/express/source.py` & `prodsys-0.6.0/prodsys/express/source.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from typing import List, Optional, Union
+from typing import List, Optional
 from uuid import uuid1
 
-from abc import ABC
 
 from pydantic import Field, conlist
 from pydantic.dataclasses import dataclass
 
-from prodsys.models import core_asset, source_data, queue_data
+from prodsys.models import source_data, queue_data
 import prodsys
 
-from prodsys.express import process, product, state, core, time_model
+from prodsys.express import core, product, time_model
 
 @dataclass
 class Source(core.ExpressObject):
     """
     Class that represents a source.
 
     Args:
@@ -61,15 +60,15 @@
             time_model=arrival_time_model,
             location=[0.0, 0.0],
         )
         ```
     """
     product: product.Product
     time_model: time_model.TIME_MODEL_UNION
-    location: conlist(float, min_items=2, max_items=2)
+    location: conlist(float, min_items=2, max_items=2) # type: ignore
     routing_heuristic: source_data.RoutingHeuristic = source_data.RoutingHeuristic.random
     ID: Optional[str] = Field(default_factory=lambda: str(uuid1()))
 
     _output_queues: List[queue_data.QueueData] = Field(default_factory=list, init=False)
 
 
     def __post_init_post_parse__(self):
```

### Comparing `prodsys-0.5.3/prodsys/express/state.py` & `prodsys-0.6.0/prodsys/express/state.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/express/time_model.py` & `prodsys-0.6.0/prodsys/express/time_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 """
 from __future__ import annotations
 
 from typing import List, Optional, Union
 from uuid import uuid1
 
 from pydantic.dataclasses import dataclass
-from pydantic import validator, Field
+from pydantic import Field
 
 from prodsys.models import time_model_data
 from prodsys.express import core
 
 @dataclass
 class SequentialTimeModel(core.ExpressObject):
     """
```

### Comparing `prodsys-0.5.3/prodsys/factories/__init__.py` & `prodsys-0.6.0/prodsys/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/factories/process_factory.py` & `prodsys-0.6.0/prodsys/factories/process_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
 from typing import List, Optional, TYPE_CHECKING
 
 from pydantic import BaseModel, parse_obj_as
 
 from prodsys.factories import time_model_factory
-from prodsys.simulation import process
 from prodsys.models import processes_data
 
 if TYPE_CHECKING:
     from prodsys.adapters import adapter
+    from prodsys.simulation import process
 
 
 class ProcessFactory(BaseModel):
     """
     Factory class that creates and stores `prodsys.simulation` process objects based on the given process data according to `prodsys.models.processes_data.PROCESS_UNION`.
 
     Args:
@@ -38,15 +38,19 @@
         if not (isinstance(process_data, processes_data.CompoundProcessData) or isinstance(process_data, processes_data.RequiredCapabilityProcessData)):
             time_model = self.time_model_factory.get_time_model(process_data.time_model_id)
             values.update({"time_model": time_model})
         values.update({"process_data": process_data})
         if isinstance(process_data, processes_data.CompoundProcessData):
             contained_processes_data = [other_process_data for other_process_data in adapter.process_data if other_process_data.ID in process_data.process_ids]
             values.update({"contained_processes_data": contained_processes_data})
-        self.processes.append(parse_obj_as(process.PROCESS_UNION, values))
+        if isinstance(process_data, processes_data.LinkTransportProcessData):
+            values.update({"links": [[]]})
+            self.processes.append(parse_obj_as(process.LinkTransportProcess, values))
+        else:
+            self.processes.append(parse_obj_as(process.PROCESS_UNION, values))
 
     def get_processes_in_order(self, IDs: List[str]) -> List[process.PROCESS_UNION]:
         """
         Returns a list of process objects in the order of the given IDs.
 
         Args:
             IDs (List[str]): List of IDs that is used to sort the process objects.
@@ -75,7 +79,11 @@
         Returns:
             Optional[process.PROCESS_UNION]: Process object based on the given ID.
         """
         pr = [pr for pr in self.processes if pr.process_data.ID in ID]
         if not pr:
             raise ValueError(f"Process with ID {ID} not found")
         return pr.pop()
+
+
+from prodsys.simulation import process
+ProcessFactory.update_forward_refs()
```

### Comparing `prodsys-0.5.3/prodsys/factories/product_factory.py` & `prodsys-0.6.0/prodsys/factories/product_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/factories/queue_factory.py` & `prodsys-0.6.0/prodsys/factories/queue_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/factories/resource_factory.py` & `prodsys-0.6.0/prodsys/factories/resource_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -203,14 +203,15 @@
             ID (str): ID of the resource object.
 
         Returns:
             resources.RESOURCE_UNION: Resource object with the given ID.
         """
         return [r for r in self.resources if r.data.ID == ID].pop()
 
+
     def get_controller_of_resource(
         self, _resource: resources.Resource
     ) -> Optional[Union[control.ProductionController, control.TransportController]]:
         """
         Method returns the controller of the given resource.
 
         Args:
@@ -248,7 +249,26 @@
             List[resources.Resource]: List of resource objects that contain the given process.
         """
         return [
             res
             for res in self.resources
             if target_process.process_data.ID in res.data.process_ids
         ]
+    
+    def get_transport_resources(self) -> List[resources.TransportResource]:
+        """
+        Method returns a list of transport resource objects.
+
+        Returns:
+            List[resources.TransportResource]: List of transport resource objects.
+        """
+        return [r for r in self.resources if isinstance(r, resources.TransportResource)]
+    
+
+    def get_production_resources(self) -> List[resources.ProductionResource]:
+        """
+        Method returns a list of production resource objects.
+
+        Returns:
+            List[resources.ProductionResource]: List of production resource objects.
+        """
+        return [r for r in self.resources if isinstance(r, resources.ProductionResource)]
```

### Comparing `prodsys-0.5.3/prodsys/factories/sink_factory.py` & `prodsys-0.6.0/prodsys/factories/sink_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/factories/source_factory.py` & `prodsys-0.6.0/prodsys/factories/source_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/factories/state_factory.py` & `prodsys-0.6.0/prodsys/factories/state_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/factories/time_model_factory.py` & `prodsys-0.6.0/prodsys/factories/time_model_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/models/__init__.py` & `prodsys-0.6.0/prodsys/models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,13 +7,15 @@
 - `prodsys.models.core_asset`: Contains the abstract base class for data objects.
 - `prodsys.models.product_data`: Contains classes to represent products.
 - `prodsys.models.performance_data`: Contains classes to represent performance data.
 - `prodsys.models.performance_indicators`: Contains classes to represent performance indicators (KPIs).
 - `prodsys.models.processes_data`: Contains classes to represent processes.
 - `prodsys.models.queue_data`: Contains classes to represent queues.
 - `prodsys.models.resource_data`: Contains classes to represent resources.
+- `prodsys.models.node_data`: Contains classes to represent nodes in a link.
 - `prodsys.models.scenario_data`: Contains classes to represent scenario data.
 - `prodsys.models.sink_data`: Contains classes to represent sinks.
 - `prodsys.models.source_data`: Contains classes to represent sources.
 - `prodsys.models.state_data`: Contains classes to represent states.
+- `prodsys.models.links_data`: Contains classes to represent links.
 - `prodsys.models.time_model_data`: Contains classes to represent time models.
 """
```

### Comparing `prodsys-0.5.3/prodsys/models/core_asset.py` & `prodsys-0.6.0/prodsys/models/core_asset.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/models/performance_data.py` & `prodsys-0.6.0/prodsys/models/performance_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/models/performance_indicators.py` & `prodsys-0.6.0/prodsys/models/performance_indicators.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/models/processes_data.py` & `prodsys-0.6.0/prodsys/models/processes_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 - `CapabilityProcessData`: A process that can be performed on a product by a resource, based on the capability of the resource.
 - `TransportProcessData`: A process that can be performed on a product by a transport resource.
 """
 
 from __future__ import annotations
 from hashlib import md5
 from enum import Enum
-from typing import Literal, Union, List, TYPE_CHECKING
+from typing import Literal, Union, Optional, List, TYPE_CHECKING
+
+from pydantic import Field
 
 from prodsys.models.core_asset import CoreAsset
 
 if TYPE_CHECKING:
     from prodsys.adapters.adapter import ProductionSystemAdapter
 
 
@@ -29,14 +31,15 @@
     """
 
     ProductionProcesses = "ProductionProcesses"
     TransportProcesses = "TransportProcesses"
     CapabilityProcesses = "CapabilityProcesses"
     CompoundProcesses = "CompoundProcesses"
     RequiredCapabilityProcesses = "RequiredCapabilityProcesses"
+    LinkTransportProcesses = "LinkTransportProcesses"
 
 
 class ProcessData(CoreAsset):
     """
     Class that represents process data. Acts as a base class for all process data classes.
 
     Args:
@@ -308,11 +311,70 @@
 
         Returns:
             str: hash of the required capability process data.
         """
         return md5(self.capability.encode("utf-8")).hexdigest()
 
 
+class LinkTransportProcessData(TransportProcessData):
+    """
+    Class that represents all link transport process data.
+
+    Args:
+        ID (str): ID of the process.
+        description (str): Description of the process.
+        type (Literal[ProcessTypeEnum.TransportProcesses]): Type of the process.
+        links (Union[List[List[str]], Dict[str, List[str]]]): Links of the route transport process. This can be a list of links or a dictionary of links with their IDs as keys.
+        capability (Optional[str], optional): Capability of the process, which is used for matching if available. Defaults to None.
+
+    Examples:
+        A transport process with ID "TP1", description "Transport Process 1",
+        type "LinkTransportProcesses", and links [["Resource1", "Node2"], ["Node2", "Resource1"]]:
+        ``` py
+        import prodsys
+        prodsys.processes_data.LinkTransportProcessData(
+            ID="TP1",
+            description="Transport Process 1",
+            time_model_id="manhattan_time_model_1",
+            type="LinkTransportProcesses",
+            links=[["Resource1", "Node2"], ["Node2", "Resource1"]],
+            capability="automated_transport_process",
+        )
+        ```
+    """
+
+    type: Literal[ProcessTypeEnum.LinkTransportProcesses]
+    links: List[List[str]]
+    capability: Optional[str] = Field(default_factory=str)
+
+    def hash(self, adapter: ProductionSystemAdapter) -> str:
+        """
+        Returns a unique hash for the required capability process data considering the capability and type of the process. Can be used to compare two process data objects for equal functionality.
+
+        Args:
+            adapter (ProductionSystemAdapter): Adapter to access the time model data.
+
+        Returns:
+            str: hash of the required capability process data.
+        """
+        raise NotImplementedError("Hash function not implemented for LinkTransportProcessData")
+        # TODO: Implement hash function for LinkTransportProcessData and Nodes
+        # return md5("".join([*sorted(process_hashes)]).encode("utf-8")).hexdigest()
+        
+    class Config:
+        schema_extra = {
+            "example": {
+                "summary": "Transport process",
+                "value": {
+                    "ID": "TP1",
+                    "description": "Transport Process 1",
+                    "time_model_id": "manhattan_time_model_1",
+                    "type": "LinkTransportProcesses",
+                    "links": [["Resource1", "Node2"], ["Node2", "Resource1"]],
+                },
+            }
+        }
+
 PROCESS_DATA_UNION = Union[
     CompoundProcessData, RequiredCapabilityProcessData,
-    ProductionProcessData, TransportProcessData, CapabilityProcessData
+    ProductionProcessData, TransportProcessData, CapabilityProcessData, LinkTransportProcessData
 ]
```

### Comparing `prodsys-0.5.3/prodsys/models/product_data.py` & `prodsys-0.6.0/prodsys/models/product_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/models/queue_data.py` & `prodsys-0.6.0/prodsys/models/queue_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/models/resource_data.py` & `prodsys-0.6.0/prodsys/models/resource_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,14 @@
     """
 
     FIFO = "FIFO"
     SPT_transport = "SPT_transport"
     NEAREST_ORIGIN_AND_LONGEST_TARGET_QUEUES_TRANSPORT = "Nearest_origin_and_longest_target_queues_transport"
     NEAREST_ORIGIN_AND_SHORTEST_TARGET_INPUT_QUEUES_TRANSPORT = "Nearest_origin_and_shortest_target_input_queues_transport"
 
-
 class ResourceData(CoreAsset):
     """
     Class that represents resource data. Base class for ProductionResourceData and TransportResourceData.
 
     Args:
         ID (str): ID of the resource.
         description (str): Description of the resource.
```

### Comparing `prodsys-0.5.3/prodsys/models/scenario_data.py` & `prodsys-0.6.0/prodsys/models/scenario_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         ValueError: If the positions are not a list of tuples of length 2.
     """
 
     transformations: List[ReconfigurationEnum]
     machine_controllers: List[Literal["FIFO", "LIFO", "SPT"]]
     transport_controllers: List[Literal["FIFO", "SPT_transport"]]
     routing_heuristics: List[Literal["shortest_queue", "random", "FIFO"]]
-    positions: List[conlist(float, min_items=2, max_items=2)]
+    positions: List[conlist(float, min_items=2, max_items=2)] # type: ignore
 
     @validator("positions")
     def check_positions(cls, v):
         for e in v:
             if len(e) != 2:
                 raise ValueError("positions must be a list of tuples of length 2")
         return v
```

### Comparing `prodsys-0.5.3/prodsys/models/sink_data.py` & `prodsys-0.6.0/prodsys/models/sink_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/models/source_data.py` & `prodsys-0.6.0/prodsys/models/source_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/models/state_data.py` & `prodsys-0.6.0/prodsys/models/state_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/models/time_model_data.py` & `prodsys-0.6.0/prodsys/models/time_model_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/optimization/__init__.py` & `prodsys-0.6.0/prodsys/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/optimization/evolutionary_algorithm.py` & `prodsys-0.6.0/prodsys/optimization/evolutionary_algorithm.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,15 +259,15 @@
         save_folder (str): Folder to save the results in. Defaults to "results".
         initial_solutions_folder (str, optional): If specified, the initial solutions are read from this folder and considered in optimization. Defaults to "".
     """
     adapters.ProductionSystemAdapter.Config.validate = False
     adapters.ProductionSystemAdapter.Config.validate_assignment = False
     base_configuration = base_configuration.copy(deep=True)
     if not adapters.check_for_clean_compound_processes(base_configuration):
-        logger.info("Compound processes are not clean. This may lead to unexpected results.")
+        logger.warning("Both compound processes and normal processes are used. This may lead to unexpected results.")
     if not check_breakdown_states_available(base_configuration):
         create_default_breakdown_states(base_configuration)
 
     util.prepare_save_folder(save_folder + "/")
     set_seed(hyper_parameters.seed)
 
     weights = get_weights(base_configuration, "max")
```

### Comparing `prodsys-0.5.3/prodsys/optimization/math_opt.py` & `prodsys-0.6.0/prodsys/optimization/math_opt.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/optimization/optimization_analysis.py` & `prodsys-0.6.0/prodsys/optimization/optimization_analysis.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/optimization/optimization_util.py` & `prodsys-0.6.0/prodsys/optimization/optimization_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 logger = logging.getLogger(__name__)
 from uuid import uuid1
 from collections.abc import Iterable
 from pydantic import parse_obj_as
 
 from prodsys import adapters, runner
 from prodsys.adapters.adapter import add_default_queues_to_resources
-from prodsys.adapters.adapter import check_redudant_locations
-from prodsys.adapters.adapter import check_required_processes_in_resources_available
+from prodsys.adapters.adapter import assert_no_redudant_locations
+from prodsys.adapters.adapter import assert_required_processes_in_resources_available
 from prodsys.adapters.adapter import get_possible_production_processes_IDs, get_possible_transport_processes_IDs
 from prodsys.util.post_processing import PostProcessor
 from prodsys.models import (
     resource_data,
     state_data,
     processes_data,
     performance_indicators,
@@ -913,15 +913,17 @@
             > configuration.scenario_data.constraints.max_num_processes_per_machine
         ):
             return False
     return True
 
 
 def valid_positions(configuration: adapters.ProductionSystemAdapter) -> bool:
-    if not check_redudant_locations(configuration):
+    try: 
+        assert_no_redudant_locations(configuration)
+    except ValueError as e:
         return False
 
     positions = [machine.location for machine in adapters.get_machines(configuration)]
     possible_positions = configuration.scenario_data.options.positions
     if any(position not in possible_positions for position in positions):
         return False
     return True
@@ -961,15 +963,17 @@
     """
     if not valid_num_machines(configuration):
         return False
     if not valid_transport_capacity(configuration):
         return False
     if not valid_num_process_modules(configuration):
         return False
-    if not check_required_processes_in_resources_available(configuration):
+    try:
+        assert_required_processes_in_resources_available(configuration)
+    except ValueError as e:
         return False
     if not valid_positions(configuration):
         return False
     if not valid_reconfiguration_cost(configuration, base_configuration):
         return False
     return True
```

### Comparing `prodsys-0.5.3/prodsys/optimization/simulated_annealing.py` & `prodsys-0.6.0/prodsys/optimization/simulated_annealing.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         hyper_parameters (SimulatedAnnealingHyperparameters): Hyperparameters for simulated annealing.
         save_folder (str): Folder to save the results in. Defaults to "results".
         initial_solution (adapters.ProductionSystemAdapter, optional): Initial solution for optimization. Defaults to None.
     """
     adapters.ProductionSystemAdapter.Config.validate = False
     adapters.ProductionSystemAdapter.Config.validate_assignment = False
     if not adapters.check_for_clean_compound_processes(base_configuration):
-        logger.info("Compound processes are not clean. This may lead to unexpected results.")
+        logger.warning("Both compound processes and normal processes are used. This may lead to unexpected results.")
     if not check_breakdown_states_available(base_configuration):
         create_default_breakdown_states(base_configuration)
     if not initial_solution:
         initial_solution = base_configuration.copy(deep=True)
 
     set_seed(hyper_parameters.seed)
```

### Comparing `prodsys-0.5.3/prodsys/optimization/tabu_search.py` & `prodsys-0.6.0/prodsys/optimization/tabu_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,15 +232,15 @@
         hyper_parameters (SimulatedAnnealingHyperparameters): Hyperparameters for tabu search.
         save_folder (str): Folder to save the results in. Defaults to "results".
         initial_solution (adapters.ProductionSystemAdapter, optional): Initial solution for optimization. Defaults to None.
     """
     adapters.ProductionSystemAdapter.Config.validate = False
     adapters.ProductionSystemAdapter.Config.validate_assignment = False
     if not adapters.check_for_clean_compound_processes(base_configuration):
-        logger.info("Compound processes are not clean. This may lead to unexpected results.")
+        logger.warning("Both compound processes and normal processes are used. This may lead to unexpected results.")
     if not check_breakdown_states_available(base_configuration):
         create_default_breakdown_states(base_configuration)
 
     set_seed(hyper_parameters.seed)
 
     weights = get_weights(base_configuration, "max")
```

### Comparing `prodsys-0.5.3/prodsys/simulation/__init__.py` & `prodsys-0.6.0/prodsys/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/simulation/control.py` & `prodsys-0.6.0/prodsys/simulation/control.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from collections.abc import Callable
 from pydantic import BaseModel, Field, validator, Extra
-from typing import List, Generator, TYPE_CHECKING, Union, Optional
+from typing import Any, List, Generator, TYPE_CHECKING, Union, Optional
 
 import logging
+
 logger = logging.getLogger(__name__)
 
 # from process import Process
 from simpy import events
 
-from prodsys.simulation import request, sim, state
+from prodsys.simulation import node, request, route_finder, sim, state, process
+
+from prodsys.simulation.process import LinkTransportProcess, RequiredCapabilityProcess
 
 if TYPE_CHECKING:
-    from prodsys.simulation import product, process, state, resources, request, sink
+    from prodsys.simulation import product, process, state, resources, request, sink, source
     from prodsys.control import sequencing_control_env
+    from prodsys.simulation.product import Locatable
+
 
 
 class Controller(ABC, BaseModel):
     """
     A controller is responsible for controlling the processes of a resource. The controller is requested by products requiring processes. The controller decides has a control policy that determines with which sequence requests are processed.
 
     Args:
@@ -68,14 +73,44 @@
         """
         self.requests.append(process_request)
         logger.debug({"ID": "controller", "sim_time": self.env.now, "resource": self.resource.data.ID, "event": f"Got requested by {process_request.product.product_data.ID}"})
         if not self.requested.triggered:
             logger.debug({"ID": "controller", "sim_time": self.env.now, "resource": self.resource.data.ID, "event": "Triggered requested event"})
             self.requested.succeed()
 
+    def wait_for_free_process(self, resource: resources.Resource, process: process.Process) -> Generator[state.State, None, None]:
+        """
+        Wait for a free process of a resource.
+
+        Args:
+            resource (resources.TransportResource): The resource.
+            process (process.Process): The process.
+
+        Returns:
+            Generator: The generator yields when a process is free.
+
+        Yields:
+            Generator: The generator yields when a process is free.
+        """
+        possible_states = resource.get_processes(process)
+        while True:
+            free_state = resource.get_free_process(process)
+            if free_state is not None:
+                return free_state
+            logger.debug({"ID": "controller", "sim_time": self.env.now, "resource": self.resource.data.ID, "event": f"Waiting for free process"})
+            yield events.AnyOf(
+                self.env,
+                [
+                    state.process
+                    for state in possible_states
+                    if state.process is not None and state.process.is_alive
+                ],
+            )
+    
+
     @abstractmethod
     def control_loop(self) -> None:
         """
         The control loop is the main process of the controller. It has to run indefinetely.
         It should repeatedly check if requests are made or a process is finished and then start the next process.
         """
         pass
@@ -177,14 +212,15 @@
             for process in self.running_processes:
                 if not process.is_alive:
                     self.running_processes.remove(process)
             if self.resource.full or not self.requests or self.reserved_requests_count == len(self.requests):
                 logger.debug({"ID": "controller", "sim_time": self.env.now, "resource": self.resource.data.ID, "event": f"No request ({len(self.requests)}) or resource full ({self.resource.full}) or all requests reserved ({self.reserved_requests_count == len(self.requests)})"})
                 continue
             self.control_policy(self.requests)
+            self.reserved_requests_count += 1
             running_process = self.env.process(self.start_process())
             self.running_processes.append(running_process)
             if not self.resource.full:
                 logger.debug({"ID": "controller", "sim_time": self.env.now, "resource": self.resource.data.ID, "event": "Triggered requested event after process"})
                 self.requested.succeed()
 
     def start_process(self) -> Generator:
@@ -196,56 +232,45 @@
         3. Retrieve the product from the queue.
         4. Run the process and wait until finished.
         5. Place the product in the output queue.
 
         Yields:
             Generator: The generator yields when the process is finished.
         """
-        self.reserved_requests_count += 1
         logger.debug({"ID": "controller", "sim_time": self.env.now, "resource": self.resource.data.ID, "event": f"Starting process"})
         yield self.env.timeout(0)
         process_request = self.requests.pop(0)
         self.reserved_requests_count -= 1
         resource = process_request.get_resource()
         process = process_request.get_process()
         product = process_request.get_product()
         logger.debug({"ID": "controller", "sim_time": self.env.now, "resource": self.resource.data.ID, "event": f"Starting setup for process for {product.product_data.ID}"})
 
         yield self.env.process(resource.setup(process))
         with resource.request() as req:
             yield req
-            eventss = self.get_next_product_for_process(resource, product)
+            product_retrieval_events = self.get_next_product_for_process(resource, product)
             logger.debug({"ID": "controller", "sim_time": self.env.now, "resource": self.resource.data.ID, "event": f"Waiting to retrieve product {product.product_data.ID} from queue"})
-            yield events.AllOf(resource.env, eventss)
-            possible_states = resource.get_processes(process)
-            while True:
-                production_state = resource.get_free_process(process)
-                if production_state is not None:
-                    break
-                logger.debug({"ID": "controller", "sim_time": self.env.now, "resource": self.resource.data.ID, "event": f"Waiting for free process"})
-                yield events.AnyOf(
-                    self.env,
-                    [
-                        state.process
-                        for state in possible_states
-                        if state.process is not None and state.process.is_alive
-                    ],
-                )
+            yield events.AllOf(resource.env, product_retrieval_events)
+            
+            production_state: state.State = yield self.env.process(self.wait_for_free_process(resource, process))
             logger.debug({"ID": "controller", "sim_time": self.env.now, "resource": self.resource.data.ID, "event": f"Starting process for {product.product_data.ID}"})
             yield self.env.process(self.run_process(production_state, product))
             production_state.process = None
-            eventss = self.put_product_to_output_queue(resource, [product])
+            
+            product_put_events = self.put_product_to_output_queue(resource, [product])
             logger.debug({"ID": "controller", "sim_time": self.env.now, "resource": self.resource.data.ID, "event": f"Waiting to put product {product.product_data.ID} to queue"})
-            yield events.AllOf(resource.env, eventss)
+            yield events.AllOf(resource.env, product_put_events)
+            
             for next_product in [product]:
                 if not resource.got_free.triggered:
                     resource.got_free.succeed()
                 next_product.finished_process.succeed()
             logger.debug({"ID": "controller", "sim_time": self.env.now, "resource": self.resource.data.ID, "event": f"Finished process for {product.product_data.ID}"})
-
+    
     def run_process(self, input_state: state.State, target_product: product.Product):
         """
         Run the process of a product. The process is started and the product is logged.
 
         Args:
             input_state (state.State): The production state of the process.
             target_product (product.Product): The product that is processed.
@@ -272,24 +297,24 @@
     requests: List[request.TransportResquest] = Field(default_factory=list)
     control_policy: Callable[
         [
             List[request.TransportResquest],
         ],
         None,
     ]
-    _current_location: Optional[product.Location] = Field(init=False, default=None)
+    _current_locatable: Optional[product.Locatable] = Field(init=False, default=None)
 
     def get_next_product_for_process(
-        self, resource: product.Location, product: product.Product
+        self, resource: product.Locatable, product: product.Product
     ) -> List[events.Event]:
         """
         Get the next product for a process from the input queue of a resource.
 
         Args:
-            resource (product.Location): Resource or Source to get the product from.
+            resource (product.Locatable): Resource or Source to get the product from.
             product (product.Product): The product that shall be transported.
 
         Raises:
             ValueError: If the product is not in the queue.
             ValueError: If the resource is not a  ProductionResource or Source.
 
         Returns:
@@ -304,38 +329,38 @@
             if not events:
                 raise ValueError("No product in queue")
         else:
             raise ValueError(f"Resource {resource.data.ID} is not a ProductionResource or Source")
         return events
 
     def put_product_to_input_queue(
-        self, resource: product.Location, product: product.Product
+        self, locatable: product.Locatable, product: product.Product
     ) -> List[events.Event]:
         """
         Put a product to the input queue of a resource.
 
         Args:
-            resource (product.Location): Resource or Sink to put the product to.
+            locatable (product.Locatable): Resource or Sink to put the product to.
             product (product.Product): The product that shall be transported.
 
         Raises:
             ValueError: If the resource is not a  ProductionResource or Sink.
 
         Returns:
             List[events.Event]: The event that is triggered when the product is in the queue.
         """
         events = []
-        if isinstance(resource, resources.ProductionResource) or isinstance(
-            resource, sink.Sink
+        if isinstance(locatable, resources.ProductionResource) or isinstance(
+            locatable, sink.Sink
         ):
-            for queue in resource.input_queues:
+            for queue in locatable.input_queues:
                 events.append(queue.put(product.product_data))
         else:
             raise ValueError(
-                f"Resource {resource.data.ID} is not a ProductionResource or Sink"
+                f"Resource {locatable.data.ID} is not a ProductionResource or Sink"
             )
 
         return events
 
     def control_loop(self) -> Generator:
         """
         The control loop is the main process of the controller. It has to run indefinetely.
@@ -369,23 +394,23 @@
             self.control_policy(self.requests)
             running_process = self.env.process(self.start_process())
             self.running_processes.append(running_process)
             if not self.resource.full:
                 logger.debug({"ID": "controller", "sim_time": self.env.now, "resource": self.resource.data.ID, "event": "Triggered requested event after process"})
                 self.requested.succeed()
 
-    def update_location(self, location: product.Location) -> None:
+    def update_location(self, locatable: product.Locatable) -> None:
         """
         Set the current position of the transport resource.
 
         Args:
-            position (product.Location): The current position.
+            locatable (product.Locatable): The current position.
         """
-        self._current_location = location
-        self.resource.set_location(location.data.location)
+        self._current_locatable = locatable
+        self.resource.set_location(locatable.get_location())
 
     def start_process(self) -> Generator:
         """
         Start the next process.
 
         The logic is the following:
 
@@ -408,117 +433,138 @@
         process_request = self.requests.pop(0)
 
         resource = process_request.get_resource()
         process = process_request.get_process()
         product = process_request.get_product()
         origin = process_request.get_origin()
         target = process_request.get_target()
+        route_to_target = process_request.get_route()
         logger.debug({"ID": "controller", "sim_time": self.env.now, "resource": self.resource.data.ID, "event": f"Starting setup for process for {product.product_data.ID}"})
+
         yield self.env.process(resource.setup(process))
         with resource.request() as req:
             yield req
             if origin.get_location() != resource.get_location():
+                route_to_origin = self.find_route_to_origin(process_request)
                 logger.debug({"ID": "controller", "sim_time": self.env.now, "resource": self.resource.data.ID, "event": f"Empty transport needed for {product.product_data.ID} from {origin.data.ID} to {target.data.ID}"})
-                possible_states = resource.get_processes(process)
-                while True:
-                    transport_state = resource.get_free_process(process)
-                    if transport_state is not None:
-                        break
-                    logger.debug({"ID": "controller", "sim_time": self.env.now, "resource": self.resource.data.ID, "event": f"Waiting for free process"})
-                    yield events.AnyOf(
-                        self.env,
-                        [
-                            state.process
-                            for state in possible_states
-                            if state.process is not None and state.process.is_alive
-                        ],
-                    )
-                logger.debug({"ID": "controller", "sim_time": self.env.now, "resource": self.resource.data.ID, "event": f"Starting picking up {product.product_data.ID} for transport"})
-                yield self.env.process(
-                    self.run_process(transport_state, product, target=origin, empty_transport=True)
-                )
-                self.update_location(origin)
-                transport_state.process = None
-
-            # TODO: drive along nodes of path
+                transport_state: state.State = yield self.env.process(self.wait_for_free_process(resource, process))
+                logger.debug({"ID": "controller", "sim_time": self.env.now, "resource": self.resource.data.ID, "event": f"Starting transport to pick up {product.product_data.ID} for transport"})
+                yield self.env.process(self.run_transport(transport_state, product, route_to_origin, empty_transport=True))
 
-            eventss = self.get_next_product_for_process(origin, product)
+            product_retrieval_events = self.get_next_product_for_process(origin, product)
             logger.debug({"ID": "controller", "sim_time": self.env.now, "resource": self.resource.data.ID, "event": f"Waiting to retrieve product {product.product_data.ID} from queue"})
-            yield events.AllOf(resource.env, eventss)
+            yield events.AllOf(resource.env, product_retrieval_events)
             product.update_location(self.resource)
-            possible_states = resource.get_processes(process)
-            while True:
-                transport_state = resource.get_free_process(process)
-                if transport_state is not None:
-                    break
-                logger.debug({"ID": "controller", "sim_time": self.env.now, "resource": self.resource.data.ID, "event": f"Waiting for free process"})
-                yield events.AnyOf(
-                    self.env,
-                    [
-                        state.process
-                        for state in possible_states
-                        if state.process is not None and state.process.is_alive
-                    ],
-                )
+
+            transport_state: state.State = yield self.env.process(self.wait_for_free_process(resource, process))
             logger.debug({"ID": "controller", "sim_time": self.env.now, "resource": self.resource.data.ID, "event": f"Starting transport of {product.product_data.ID}"})
-            yield self.env.process(
-                self.run_process(transport_state, product, target=target, empty_transport=False)
-            )
-            self.update_location(target)
-            transport_state.process = None
-            eventss = self.put_product_to_input_queue(target, product)
+            yield self.env.process(self.run_transport(transport_state, product, route_to_target, empty_transport=False))
+            
+            product_put_events = self.put_product_to_input_queue(target, product)
             logger.debug({"ID": "controller", "sim_time": self.env.now, "resource": self.resource.data.ID, "event": f"Waiting to put product {product.product_data.ID} to queue"})
-            yield events.AllOf(resource.env, eventss)
+            yield events.AllOf(resource.env, product_put_events)
             product.update_location(target)
+            
             if isinstance(target, resources.ProductionResource):
                 target.unreserve_input_queues()
             if not resource.got_free.triggered:
                 resource.got_free.succeed()
             product.finished_process.succeed()
             logger.debug({"ID": "controller", "sim_time": self.env.now, "resource": self.resource.data.ID, "event": f"Finished transport of {product.product_data.ID}"})
 
+    def run_transport(self, transport_state: state.State, product: product.Product, route: List[product.Locatable], empty_transport: bool) -> Generator:
+        """
+        Run the transport process and every single transport step in the route of the transport process.
+
+        Args:
+            transport_state (state.State): The transport state of the process.
+            product (product.Product): The product that is transported.
+            route (List[product.Locatable]): The route of the transport with locatable objects.
+            empty_transport (bool): If the transport is empty.
+
+        Yields:
+            Generator: The generator yields when the transport is over.
+        """
+        for link_index, (location, next_location) in enumerate(zip(route, route[1:])):
+            if link_index == 0:
+                initial_transport_step = True
+            else:
+                initial_transport_step = False
+            if link_index == len(route) - 2:
+                last_transport_step = True
+            else:
+                last_transport_step = False
+            logger.debug({"ID": "controller", "sim_time": self.env.now, "resource": self.resource.data.ID, "event": f"Moving from {location.data.ID} to {next_location.data.ID}", "empty_transport": True, "initial_transport_step": initial_transport_step, "last_transport_step": last_transport_step})
+            yield self.env.process(self.run_process(transport_state, product, target=next_location, empty_transport=empty_transport, initial_transport_step=initial_transport_step, last_transport_step=last_transport_step))
+            self.update_location(next_location)
+            logger.debug({"ID": "controller", "sim_time": self.env.now, "resource": self.resource.data.ID, "event": f"Arrived at {next_location.data.ID}", "empty_transport": True, "initial_transport_step": initial_transport_step, "last_transport_step": last_transport_step})
+            transport_state.process = None
 
     def run_process(
         self,
-        input_state: state.State,
+        input_state: state.TransportState,
         product: product.Product,
-        target: product.Location,
+        target: product.Locatable,
         empty_transport: bool,
+        initial_transport_step: bool,
+        last_transport_step: bool
     ):
         """
         Run the process of a product. The process is started and the product is logged.
 
         Args:
             input_state (state.State): The transport state of the process.
             product (product.Product): The product that is transported.
-            target (product.Location): The target of the transport.
+            target (product.Locatable): The target of the transport.
+            empty_transport (bool): If the transport is empty.
+            initial_transport_step (bool): If this is the initial transport step.
+            last_transport_step (bool): If this is the last transport step.
         """
         target_location = target.get_location()
         input_state.prepare_for_run()
         input_state.state_info.log_product(product, state.StateTypeEnum.transport)
-        if self._current_location.data.ID is self.resource.data.ID:
+        if self._current_locatable.data.ID is self.resource.data.ID:
             origin = None
         else:
-            origin = self._current_location
+            origin = self._current_locatable
         input_state.state_info.log_transport(
             origin,
             target, state.StateTypeEnum.transport,
             empty_transport=empty_transport
         )
         product.product_info.log_start_process(
             self.resource,
             product,
             self.env.now,
             state.StateTypeEnum.transport,
         )
+       
         input_state.process = self.env.process(
-            input_state.process_state(target=target_location)  # type: ignore False
+            input_state.process_state(target=target_location, initial_transport_step=initial_transport_step, last_transport_step=last_transport_step)  # type: ignore False
         )
         yield input_state.process
 
+    def find_route_to_origin(self, process_request: request.TransportResquest) -> List[product.Locatable]:
+        """
+        Find the route to the origin of the transport request.
+
+        Args:
+            process_request (request.TransportResquest): The transport request.
+
+        Returns:
+            List[product.Locatable]: The route to the origin. In case of a simple transport process, the route is just the origin.
+        """
+        if isinstance(process_request.process, LinkTransportProcess):
+            route_to_origin = route_finder.find_route(request=process_request, find_route_to_origin=True, process=process_request.get_process())
+            if not route_to_origin:
+                raise ValueError(f"Route to origin for transport of {process_request.product.product_data.ID} could not be found. Router selected a transport resource that can perform the transport but does not reach the origin.")
+            return route_to_origin
+        else:
+            return [self._current_locatable, process_request.get_origin()]
+
 
 def FIFO_control_policy(requests: List[request.Request]) -> None:
     """
     Sort the requests according to the FIFO principle.
 
     Args:
         requests (List[request.Request]): The list of requests.
```

### Comparing `prodsys-0.5.3/prodsys/simulation/logger.py` & `prodsys-0.6.0/prodsys/simulation/logger.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/simulation/observer.py` & `prodsys-0.6.0/prodsys/simulation/observer.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         for product_data in queue.items:
             product = product_factory.get_product(product_data.ID)
 
             production_process_info = QueueObservation(
                 product=product_data.ID,
                 activity="waiting",
                 process=product.next_prodution_process.process_data.ID,
-                next_resource=product.current_location.data.ID,
+                next_resource=product.current_locatable.data.ID,
                 waiting_since=product.product_info.event_time
             )
             queue_observation.append(production_process_info)
 
     return queue_observation
 
 def observe_output_queue(resource: resources.Resource, product_factory: product_factory.ProductFactory) -> List[QueueObservation]:
@@ -60,15 +60,15 @@
         for product_data in queue.items:
             product = product_factory.get_product(product_data.ID)
 
             production_process_info = QueueObservation(
                 product=product_data.ID,
                 activity="waiting",
                 process=product.next_prodution_process,
-                next_resource=product.current_location,
+                next_resource=product.current_locatable,
                 waiting_since=product.product_info.event_time
             )
             queue_observation.append(production_process_info)
 
     return queue_observation
 
 class ResourceAvailableObservation(BaseModel):
```

### Comparing `prodsys-0.5.3/prodsys/simulation/proces_models.py` & `prodsys-0.6.0/prodsys/simulation/proces_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
         return [self.process_list[self.current_marking]]
 
     def update_marking_from_transition(
         self, chosen_process: process.PROCESS_UNION
     ) -> None:
         self.current_marking += 1
 
-
 class PrecendeGraphNode(BaseModel):
     """
     Class that represents a node in a precedence graph.
 
     Args:
         process (process.PROCESS_UNION): The process that is represented by the node.
         successors (Optional[List[PrecendeGraphNode]]): List of successor nodes.
```

### Comparing `prodsys-0.5.3/prodsys/simulation/process.py` & `prodsys-0.6.0/prodsys/simulation/process.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import Union, List, Optional
+from typing import TYPE_CHECKING, Union, List, Optional
 
+from numpy import isin
 from pydantic import BaseModel
 
-from prodsys.simulation import time_model, request
+
+if TYPE_CHECKING:
+    from prodsys.simulation import resources, source, sink, node
+
+from prodsys.simulation import route_finder, time_model, request
+
 from prodsys.models import processes_data
 
 
 class Process(ABC, BaseModel):
     """
     Abstract process base class that defines the interface for all processes.
     """
@@ -87,17 +93,15 @@
         time_model (time_model.TimeModel): The time model.
     """
     process_data: processes_data.CapabilityProcessData
 
     def matches_request(self, request: request.Request) -> bool:
         requested_process = request.process
         if (
-            not isinstance(requested_process, CapabilityProcess)
-            and not isinstance(requested_process, CompoundProcess)
-            and not isinstance(requested_process, RequiredCapabilityProcess)
+            not is_process_with_capability(requested_process) and not isinstance(requested_process, CompoundProcess)
         ):
             return False
         if isinstance(requested_process, CompoundProcess):
             return self.process_data.capability in [
                 p.process_data.capability
                 for p in requested_process.contained_processes_data
                 if isinstance(p, CapabilityProcess)
@@ -117,30 +121,56 @@
 
     Args:
         process_data (processes_data.TransportProcessData): The process data.
         time_model (time_model.TimeModel): The time model.
     """
     process_data: processes_data.TransportProcessData
 
-    def matches_request(self, request: request.Request) -> bool:
+    def matches_request(self, request: request.TransportResquest) -> bool:
         requested_process = request.process
         if not isinstance(requested_process, TransportProcess) and not isinstance(
             requested_process, CompoundProcess
         ):
             return False
-        if isinstance(requested_process, TransportProcess):
-            return requested_process.process_data.ID == self.process_data.ID
-        return self.process_data.ID in requested_process.process_data.process_ids
+        if isinstance(requested_process, TransportProcess) and not requested_process.process_data.ID == self.process_data.ID:
+            return False
+        if isinstance(requested_process, CompoundProcess) and not self.process_data.ID in requested_process.process_data.process_ids:
+            return False
+        request.set_route(route=[request.origin, request.target])
+        return True
 
     def get_process_time(self, origin: List[float], target: List[float]) -> float:
         return self.time_model.get_next_time(origin=origin, target=target)
 
     def get_expected_process_time(self, *args) -> float:
         return self.time_model.get_expected_time(*args)
+    
+def is_process_with_capability(process: PROCESS_UNION) -> bool:
+    """
+    Returns True if the given process is a process with capability.
+
+    Args:
+        process (PROCESS_UNION): The process.
+
+    Returns:
+        bool: True if the given process is a process with capability.
+    """
+    return isinstance(process, CapabilityProcess) or isinstance(process, RequiredCapabilityProcess) or (isinstance(process, LinkTransportProcess) and process.process_data.capability)
+
+def is_available_process_with_capability(process: PROCESS_UNION) -> bool:
+    """
+    Returns True if the given process is an available process with capability.
 
+    Args:
+        process (PROCESS_UNION): The process.
+
+    Returns:
+        bool: True if the given process is an available process with capability.
+    """
+    return isinstance(process, CapabilityProcess) or (isinstance(process, LinkTransportProcess) and process.process_data.capability)
 
 class CompoundProcess(Process):
     """
     Class that represents a compound process.
 
     Args:
         process_data (processes_data.CompoundProcessData): The process data.
@@ -149,111 +179,135 @@
     process_data: processes_data.CompoundProcessData
     contained_processes_data: List[
         Union[
             processes_data.ProductionProcessData,
             processes_data.TransportProcessData,
             processes_data.CapabilityProcessData,
             processes_data.RequiredCapabilityProcessData,
+            processes_data.LinkTransportProcessData,
         ]
     ]
 
     def matches_request(self, request: request.Request) -> bool:
         requested_process = request.process
         if isinstance(requested_process, ProductionProcess) or isinstance(
             requested_process, TransportProcess
-        ):
+        ) or (isinstance(requested_process, LinkTransportProcess) and not requested_process.process_data.capability):
             return requested_process.process_data.ID in self.process_data.process_ids
-        elif isinstance(requested_process, CapabilityProcess) or isinstance(
-            requested_process, RequiredCapabilityProcess
-        ):
+        elif is_process_with_capability(requested_process):
             return requested_process.process_data.capability in [
                 p.process_data.capability
                 for p in self.contained_processes_data
-                if isinstance(p, CapabilityProcess)
+                if is_available_process_with_capability(p)
             ]
         elif isinstance(requested_process, CompoundProcess):
             return any(
                 p.ID in self.process_data.process_ids
                 for p in requested_process.contained_processes_data
                 if isinstance(p, ProductionProcess)
             ) or any(
                 p.capability
                 in [
                     p.process_data.capability
                     for p in self.contained_processes_data
-                    if isinstance(p, CapabilityProcess)
+                    if is_available_process_with_capability(p)
                 ]
                 for p in requested_process.contained_processes_data
-                if isinstance(p, CapabilityProcess)
+                if is_available_process_with_capability(p)
             )
+        return False
 
     def get_process_time(self) -> float:
         raise NotImplementedError("CompoundProcess does not have a process time.")
 
     def get_expected_process_time(self) -> float:
         raise NotImplementedError("CompoundProcess does not have a process time.")
 
 
 class RequiredCapabilityProcess(Process):
     """
     Class that represents a required capability process.
 
     Args:
         process_data (processes_data.RequiredCapabilityProcessData): The process data.
-        time_model (time_model.TimeModel): The time model.
     """
-
     process_data: processes_data.RequiredCapabilityProcessData
 
     def matches_request(self, request: request.Request) -> bool:
-        raise NotImplementedError(
-            "RequiredCapabilityProcess cannot be matched but should only request."
-        )
+        raise NotImplementedError("RequiredCapabilityProcess does not match requests but only generates them.")
 
     def get_process_time(self) -> float:
         raise NotImplementedError(
             "RequiredCapabilityProcess does not have a process time."
         )
 
     def get_expected_process_time(self) -> float:
         raise NotImplementedError(
             "RequiredCapabilityProcess does not have a process time."
         )
-    
 
-class TransportLinkProcess(Process):
+class LinkTransportProcess(TransportProcess):
     """
     Class that represents a transport link process.
     """
+    process_data: processes_data.LinkTransportProcessData
+    links: Optional[List[List[Union[node.Node, source.Source, sink.Sink, resources.ProductionResource]]]]
 
-    # TODO: Implement LinkTransportProcess and RouteTransportProcess and their associatd data models.
-
-    def matches_request(self, request: request.Request) -> bool:
-        # 1. check if request is a transport request (if not, return False)
-        # 2. check if transport request is a link request (if not, return False)
+    def matches_request(self, request: request.TransportResquest) -> bool:
+        requested_process = request.process
 
-        # 3. check for compatibility -> transport links can links from origin to target of resquest
-        # path: List[Links] = path_finder.find_path(request.origin, request.target, self.links)
-        # return not path:
-        #     return False
-        # 4. set path of request
-        # request.path = path
-        # return True
-        pass
+        if not isinstance(requested_process, LinkTransportProcess) and not isinstance(requested_process, RequiredCapabilityProcess) and not isinstance(
+            requested_process, CompoundProcess
+        ):
+            return False
+        
+        if isinstance(requested_process, CompoundProcess):
+            possible_processes = []
+            for process_data_instance in requested_process.contained_processes_data:
+                if is_process_with_capability(process_data_instance) and self.process_data.capability and self.process_data.capability == process_data_instance.capability:
+                    possible_processes.append(process_data_instance)
+                if isinstance(process_data_instance, LinkTransportProcess) and process_data_instance.ID == self.process_data.ID:
+                    possible_processes.append(process_data_instance)
+            if not possible_processes:
+                return False
+
+        if is_process_with_capability(requested_process):
+            if not requested_process.process_data.capability == self.process_data.capability:
+                return False
+        
+        if isinstance(requested_process, LinkTransportProcess):
+            if not requested_process.process_data.ID == self.process_data.ID:
+                return False
+            
+        route = route_finder.find_route(request=request, process=self)
+        if not route:
+            return False
+        return True
     
-    def get_process_time(self) -> float:
-        # TODO: calculate based on request and path
-        pass
+    def get_process_time(self, request: request.TransportResquest) -> float:
+        route = request.get_route()
+        total_time = 0
+        link_route = [route[i:i+2] for i in range(len(route)-1)]
+
+        for link in link_route:
+            time = self.time_model.get_next_time(origin=link[0].get_location(), target=link[1].get_location())
+            total_time += time
+        return total_time
 
-    def get_expected_process_time(self) -> float:
-        pass
+    def get_expected_process_time(self, *args) -> float:
+        return self.time_model.get_expected_time(*args)
+    
+    
 
 PROCESS_UNION = Union[
     CompoundProcess,
     RequiredCapabilityProcess,
     ProductionProcess,
     TransportProcess,
     CapabilityProcess,
+    LinkTransportProcess,
 ]
 """
 Union type for all processes.
 """
+from prodsys.simulation import resources, source, sink, node
+LinkTransportProcess.update_forward_refs()
```

### Comparing `prodsys-0.5.3/prodsys/simulation/product.py` & `prodsys-0.6.0/prodsys/simulation/product.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     router,
     resources,
     sim,
     sink,
     source,
     proces_models,
     state,
+    node
 )
 
 from prodsys.models import product_data
 
 
 class ProductInfo(BaseModel, extra=Extra.allow):
     """
@@ -132,17 +133,15 @@
         self.resource_ID = resource.data.ID
         self.state_ID = resource.data.ID
         self.event_time = event_time
         self.product_ID = _product.product_data.ID
         self.activity = state.StateEnum.end_state
         self.state_type = state_type
 
-
-Location = Union[resources.Resource, source.Source, sink.Sink]
-
+Locatable= Union[resources.Resource, node.Node, source.Source, sink.Sink]
 
 class Product(BaseModel):
     """
     Class that represents a product in the discrete event simulation. For easier instantion of the class, use the ProductFactory at prodsys.factories.product_factory.
 
     Args:
         env (sim.Environment): prodsys simulation environment.
@@ -151,103 +150,59 @@
         transport_process (process.Process): Transport process that represents the required transport processes.
         product_router (router.Router): Router that is used to route the product object.
     """
 
     env: sim.Environment
     product_data: product_data.ProductData
     process_model: proces_models.ProcessModel
-    transport_process: process.TransportProcess
+    transport_process: Union[process.LinkTransportProcess, process.TransportProcess, process.RequiredCapabilityProcess]
     product_router: router.Router
 
     next_prodution_process: Optional[process.PROCESS_UNION] = Field(default=None, init=False)
     process: events.Process = Field(default=None, init=False)
-    current_location: Location = Field(default=None, init=False)
+    current_locatable: Locatable = Field(default=None, init=False)
     finished_process: events.Event = Field(default=None, init=False)
     product_info: ProductInfo = ProductInfo()
 
     class Config:
         arbitrary_types_allowed = True
 
-    def update_location(self, resource: Location):
+    def update_location(self, resource: Locatable):
         """
         Updates the location of the product object.
 
         Args:
-            resource (Location): Location of the product object.
+            resource (Locatable): Locatable objects where product object currently is.
         """
-        self.current_location = resource
-        logger.debug({"ID": self.product_data.ID, "sim_time": self.env.now, "resource": self.current_location.data.ID, "event": f"Updated location to {self.current_location.data.ID}"})
+        self.current_locatable = resource
+        logger.debug({"ID": self.product_data.ID, "sim_time": self.env.now, "resource": self.current_locatable.data.ID, "event": f"Updated location to {self.current_locatable.data.ID}"})
 
     def process_product(self):
         self.finished_process = events.Event(self.env)
         self.product_info.log_create_product(
-            resource=self.current_location, _product=self, event_time=self.env.now
+            resource=self.current_locatable, _product=self, event_time=self.env.now
         )
         """
         Processes the product object in a simpy process. The product object is processed after creation until all required production processes are performed and it reaches a sink.
         """
         logger.debug({"ID": self.product_data.ID, "sim_time": self.env.now, "event": f"Start processing of product"})
         self.set_next_production_process()
         while self.next_prodution_process:
-            production_request = self.get_request_for_production_process()
-            yield self.env.process(self.product_router.route_request(production_request))
-            transport_request = self.get_request_for_transport_process(production_request)
-            yield self.env.process(self.product_router.route_request(transport_request))
+            production_request, transport_request = yield self.env.process(self.product_router.route_product(self))
             yield self.env.process(self.request_process(transport_request))
             yield self.env.process(self.request_process(production_request))
             self.set_next_production_process()
-        transport_to_sink_request = self.get_request_for_transport_to_sink()
-        yield self.env.process(self.product_router.route_request(transport_to_sink_request))
+        transport_to_sink_request = yield self.env.process(self.product_router.route_product_to_sink(self))
         yield self.env.process(self.request_process(transport_to_sink_request))
         self.product_info.log_finish_product(
-            resource=self.current_location, _product=self, event_time=self.env.now
+            resource=self.current_locatable, _product=self, event_time=self.env.now
         )
-        self.current_location.register_finished_product(self)
+        self.current_locatable.register_finished_product(self)
         logger.debug({"ID": self.product_data.ID, "sim_time": self.env.now, "event": f"Finished processing of product"})
 
-    def get_request_for_production_process(self) -> request.Request:
-        """
-        Returns a request for the next production process of the product object.
-
-        Returns:
-            request.Request: The request for the next production process.
-        """
-        return request.Request(
-            process=self.next_prodution_process,
-            product=self,
-        )
-    
-    def get_request_for_transport_process(self, production_request: request.Request) -> request.Request:
-        """
-        Returns a request for the next transport process of the product object.
-
-        Returns:
-            request.Request: The request for the next transport process.
-        """
-        return request.TransportResquest(
-            process=self.transport_process,
-            product=self,
-            origin=self.current_location,
-            target=production_request.resource,
-        )
-    
-    def get_request_for_transport_to_sink(self) -> request.Request:
-        """
-        Returns a request for the transport to the sink of the product object.
-
-        Returns:
-            request.Request: The request for the transport to the sink.
-        """
-        return request.TransportResquest(
-            process=self.transport_process,
-            product=self,
-            origin=self.current_location,
-            target=self.product_router.get_sink(self.product_data.product_type),
-        )
-
     def request_process(self, processing_request: request.Request) -> Generator:
         """
         Requests the next production process of the product object from the next production resource by creating a request event and registering it at the environment.
         """
         if isinstance(processing_request, request.TransportResquest):
             type_ = state.StateTypeEnum.transport
         else:
```

### Comparing `prodsys-0.5.3/prodsys/simulation/request.py` & `prodsys-0.6.0/prodsys/simulation/request.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Optional
-
-from prodsys.simulation import process as prodsys_process
+from typing import TYPE_CHECKING, Dict, Optional, List, Tuple, Union
 
 if TYPE_CHECKING:
-    from prodsys.simulation import product, process, resources
+    from prodsys.simulation import product, process, resources, sink
+    from prodsys.simulation.product import Locatable
+
 
 
 class Request:
     """
     Class to represents requests of a product for a process to be executed by a resource.
 
     Args:
@@ -17,31 +17,31 @@
         product (product.Product): The product.
         resource (resources.Resource): The resource.
     """
     def __init__(
         self,
         process: process.PROCESS_UNION,
         product: product.Product,
+        resource: resources.Resource
     ):
         self.process = process
         self.product = product
-        self.resource: Optional[resources.Resource] = None
+        self.resource = resource
 
-    def set_resource(self, resource: resources.Resource):
+
+    def set_process(self, process: process.PROCESS_UNION):
         """
-        Sets the resource of the request.
+        Sets the process of the request.
 
         Args:
-            resource (resources.Resource): The resource.
+            process (process.PROCESS_UNION): The process.
         """
-        self.resource = resource
-        for process in self.resource.processes:
-            if process.matches_request(self):
-                # TODO: check whether this needs adaption for compound processes...
-                self.process = process
+        self.process = process
+        # TODO: maybe do some special handling of compound processes here
+
 
     def get_process(self) -> process.PROCESS_UNION:
         """
         Returns the process or the capability process of the request 
 
         Returns:
             process.PROCESS_UNION: The process.
@@ -61,14 +61,32 @@
         """
         Returns the resource of the request.
 
         Returns:
             resources.Resource: The resource.
         """
         return self.resource
+    
+
+class SinkRequest(Request):
+    """
+    Class to represents requests of a product for a storage in a sink to be executed by a resource.
+
+    Args:
+        Request (_type_): _description_
+    """
+    def __init__(
+        self,
+        product: product.Product,
+        sink: sink.Sink
+    ):
+        self.resource = sink
+        self.product = product
+        self.process = None
+    
 
 
 class TransportResquest(Request):
     """
     Class to represents requests of a product for a transport process to be executed by a transport resource. Additionally, it contains the origin and target locations of the transport.
 
     Args:
@@ -76,26 +94,59 @@
         product (product.Product): The product.
         resource (resources.TransportResource): The transport resource.
         origin (product.Location): The origin location, either a resource, source or sink.
         target (product.Location): The target location, either a resource, source or sink.
     """
     def __init__(
         self,
-        process: process.TransportProcess,
+        process: Union[process.TransportProcess, process.LinkTransportProcess],
         product: product.Product,
-        origin: product.Location,
-        target: product.Location,
+        resource: resources.TransportResource,
+        origin: product.Locatable,
+        target: product.Locatable,
     ):
-        self.process: process.TransportProcess = process
+        self.process: Union[process.TransportProcess, process.LinkTransportProcess] = process
         self.product: product.Product = product
-        self.resource: resources.TransportResource = None
-        self.origin: product.Location = origin
-        self.target: product.Location = target
+        self.resource: resources.TransportResource = resource
+        self.origin: product.Locatable = origin
+        self.target: product.Locatable = target
+
+        self.route: Optional[List[Locatable]] = None
+
+
+    def set_process(self, process: process.PROCESS_UNION):
+        """
+        Sets the process of the request.
+
+        Args:
+            process (process.PROCESS_UNION): The process.
+        """
+        self.process = process
+        # TODO: maybe do some special handling of compound processes here
+
+    def copy_cached_routes(self, request: TransportResquest):
+        """
+        Copies the cached routes from another transport request.
+
+        Args:
+            request (TransportResquest): The transport request.
+        """
+        self.route = request.route
 
-    def get_process(self) -> process.TransportProcess:
+    def set_route(self, route: List[Locatable]):
+        """
+        Caches a possible route of the transport request used later for setting the resource of the transport request.
+
+        Args:
+            process (process.TransportProcess): The process.
+            route (List[product.Locatable]): The route.
+        """
+        self.route = route
+
+    def get_process(self) -> Union[process.TransportProcess, process.LinkTransportProcess]:
         """
         Returns the transport process of the transport request.
 
         Returns:
             process.TransportProcess: The transport process.
         """
         return self.process
@@ -105,24 +156,34 @@
         Returns the transport resource of the transport request.
 
         Returns:
             resources.TransportResource: The transport resource.
         """
         return self.resource
 
-    def get_origin(self) -> product.Location:
+    def get_origin(self) -> product.Locatable:
         """
         Returns the origin location of the transport request.
 
         Returns:
-            product.Location: The origin location.
+            product.Locatable: The origin location.
         """
         return self.origin
 
-    def get_target(self) -> product.Location:
+    def get_target(self) -> product.Locatable:
         """
         Returns the target location of the transport request.
 
         Returns:
-            product.Location: The target location.
+            product.Locatable: The target location.
         """
         return self.target
+    
+    def get_route(self) -> List[Locatable]:
+        """
+        Returns the route of the transport request.
+
+        Returns:
+            List[product.Locatable]: The route.
+
+        """
+        return self.route
```

### Comparing `prodsys-0.5.3/prodsys/simulation/resources.py` & `prodsys-0.6.0/prodsys/simulation/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 from __future__ import annotations
 
 from abc import ABC
-from typing import List, Generator, Optional, Union
+from typing import TYPE_CHECKING, List, Generator, Optional, Union
 
 from pydantic import BaseModel, Field, Extra
 import random
 
 import logging
 logger = logging.getLogger(__name__)
 
 from simpy.resources import resource
 from simpy import events
-from prodsys.simulation import process, sim, store
-
+from prodsys.simulation import sim, store
+if TYPE_CHECKING:
+    from prodsys.simulation import process, control, state
 
 from prodsys.models.resource_data import (
     RESOURCE_DATA_UNION,
     ProductionResourceData,
     TransportResourceData,
 )
-from prodsys.simulation import control, state
 from prodsys.util import util
 
-
 class Resource(BaseModel, ABC, resource.Resource):
     """
     Base class for all resources.
 
     Args:
         env (sim.Environment): The simpy environment.
         data (RESOURCE_DATA_UNION): The resource data.
@@ -118,15 +117,15 @@
         Returns:
             bool: True if the resource is full or in setup, False otherwise.
         """
         if self.in_setup:
             return True
         return (
             self.capacity_current_setup
-            - len(self.controller.running_processes)
+            - (len(self.controller.running_processes) + self.controller.reserved_requests_count)
         ) <= 0
 
     def get_controller(self) -> control.Controller:
         """
         Returns the controller of the resource.
 
         Returns:
@@ -440,7 +439,12 @@
     """
     data: TransportResourceData
     controller: control.TransportController
 
 
 RESOURCE_UNION = Union[ProductionResource, TransportResource]
 """ Union Type for Resources. """
+
+from prodsys.simulation import process, control, state
+Resource.update_forward_refs()
+ProductionResource.update_forward_refs()
+TransportResource.update_forward_refs()
```

### Comparing `prodsys-0.5.3/prodsys/simulation/sim.py` & `prodsys-0.6.0/prodsys/simulation/sim.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/simulation/sink.py` & `prodsys-0.6.0/prodsys/simulation/sink.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/simulation/source.py` & `prodsys-0.6.0/prodsys/simulation/source.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/simulation/state.py` & `prodsys-0.6.0/prodsys/simulation/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,21 +71,23 @@
     _activity: Optional[StateEnum] = None
     _state_type: Optional[StateTypeEnum] = None
     _product_ID: str = ""
     _target_ID: str = ""
     _origin_ID: str = ""
     _empty_transport: Optional[bool] = None
 
-    def log_transport(self, origin: Optional[product.Location], target: product.Location, state_type: StateTypeEnum, empty_transport: bool):
+    def log_transport(self, origin: Optional[product.Locatable], target: product.Locatable, state_type: StateTypeEnum, empty_transport: bool):
         """
         Logs the target location of a transport state.
 
         Args:
-            target (product.Location): The target location, either a resource, source or a sink.
+            origin (Optional[product.Locatable]): The origin location, either a resource, source, node or a sink.
+            target (product.Locatable): The target location, either a resource, source, node or a sink.
             state_type (StateTypeEnum): The type of the state.
+            empty_transport (bool): Indicates if the transport is empty.
         """
         if not origin:
             self._origin_ID = "Loading station"
         else:
             self._origin_ID = origin.data.ID
         self._target_ID = target.data.ID
         self._state_type = state_type
@@ -364,18 +366,23 @@
 
     def prepare_for_run(self):
         self.finished_process = events.Event(self.env)
 
     def activate_state(self):
         self.active = events.Event(self.env).succeed()
 
-    def process_state(self, target: List[float]) -> Generator:
+    def process_state(self, target: List[float], initial_transport_step: bool, last_transport_step: bool) -> Generator:
         self.done_in = self.time_model.get_next_time(
             origin=self.resource.get_location(), target=target
         )
+        if initial_transport_step and hasattr(self.time_model, "reaction_time") and self.time_model.time_model_data.reaction_time:
+            self.done_in -= self.time_model.time_model_data.reaction_time
+
+        # TODO: also use intial and last_transport_step to add loading times
+
         while True:
             try:
                 if self.interrupted:
                     debug_logging(self, f"interrupted while waiting for activation or activation of resource")
                     yield events.AllOf(self.env, [self.active, self.resource.active])
                     self.interrupted = False
                 debug_logging(self, f"wait for activation or activation of resource before process")
```

### Comparing `prodsys-0.5.3/prodsys/simulation/store.py` & `prodsys-0.6.0/prodsys/simulation/store.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/simulation/time_model.py` & `prodsys-0.6.0/prodsys/simulation/time_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,14 @@
     """
     Class for time models that are based on the manhattan distance between two points and time calculation based on reaction time and speed.
 
     Args:
         time_model_data (ManhattanDistanceTimeModelData): The time model data object.
     """
     time_model_data: ManhattanDistanceTimeModelData
-
     def get_next_time(
         self,
         origin: Optional[List[float]] = None,
         target: Optional[List[float]] = None,
     ) -> float:
         """
         Returns the next time for a time model based on the manhattan distance between two points and time calculation based on reaction time and speed.
```

### Comparing `prodsys-0.5.3/prodsys/util/kpi_visualization.py` & `prodsys-0.6.0/prodsys/util/kpi_visualization.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/util/post_processing.py` & `prodsys-0.6.0/prodsys/util/post_processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -573,16 +573,14 @@
 
         df["WIP"] = df.groupby(by="WIP_resource")["WIP_Increment"].cumsum()
         
         # FIXME: remove bug that negative WIP is possible
         df_temp = df[["State", "State Type"]].drop_duplicates()
         sinks = df_temp.loc[df_temp["State Type"] == state.StateTypeEnum.sink, "State"].unique()
         df = df.loc[~df["WIP_resource"].isin(sinks)]
-
-        df.to_csv("data/WIP_per_resource.csv")
         
         return df
     
     @cached_property
     def df_WIP_per_resource(self) -> pd.DataFrame:
         """
         Returns a data frame with the WIP over time for each resource.
```

### Comparing `prodsys-0.5.3/prodsys/util/runner.py` & `prodsys-0.6.0/prodsys/util/runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 import numpy as np
 import time
 from functools import cached_property
 
 from prodsys.adapters import adapter
 from prodsys.simulation import sim
 from prodsys.factories import (
+    link_transport_process_updater,
     state_factory,
     time_model_factory,
     process_factory,
     queue_factory,
     resource_factory,
     product_factory,
     sink_factory,
     source_factory,
+    node_factory,
 )
 from prodsys.simulation import logger
 from prodsys.util import post_processing, kpi_visualization, util
 from prodsys.models import performance_data
 
 VERBOSE = 1
 
@@ -92,29 +94,30 @@
     time_model_factory: time_model_factory.TimeModelFactory = Field(
         init=False, default=None
     )
     state_factory: state_factory.StateFactory = Field(init=False, default=None)
     process_factory: process_factory.ProcessFactory = Field(init=False, default=None)
     queue_factory: queue_factory.QueueFactory = Field(init=False, default=None)
     resource_factory: resource_factory.ResourceFactory = Field(init=False, default=None)
+    node_factory: node_factory.NodeFactory = Field(init=False, default=None)
     sink_factory: sink_factory.SinkFactory = Field(init=False, default=None)
     source_factory: source_factory.SourceFactory = Field(init=False, default=None)
     product_factory: product_factory.ProductFactory = Field(init=False, default=None)
     event_logger: logger.Logger = Field(init=False, default=None)
     time_stamp: str = Field(init=False, default="")
     post_processor: post_processing.PostProcessor = Field(init=False, default=None)
 
     class Config:
         arbitrary_types_allowed = True
 
     def initialize_simulation(self):
         """
         Initializes the simulation by creating the factories and all simulation objects. Needs to be done before running the simulation.
         """
-        self.adapter.physical_validation()
+        self.adapter.validate_configuration()
         with temp_seed(self.adapter.seed):
 
             self.time_model_factory = time_model_factory.TimeModelFactory()
             self.time_model_factory.create_time_models(self.adapter)
 
             self.env = sim.Environment(seed=self.adapter.seed)
 
@@ -129,20 +132,24 @@
             self.process_factory.create_processes(self.adapter)
 
             self.queue_factory = queue_factory.QueueFactory(env=self.env)
             self.queue_factory.create_queues(self.adapter)
 
             self.resource_factory = resource_factory.ResourceFactory(
                 env=self.env,
-                process_factory=self.process_factory,
                 state_factory=self.state_factory,
                 queue_factory=self.queue_factory,
+                process_factory= self.process_factory
             )
             self.resource_factory.create_resources(self.adapter)
 
+            self.node_factory = node_factory.NodeFactory(
+                env=self.env)
+            self.node_factory.create_nodes(self.adapter)
+
             self.product_factory = product_factory.ProductFactory(
                 env=self.env, process_factory=self.process_factory
             )
 
             self.sink_factory = sink_factory.SinkFactory(
                 env=self.env,
                 product_factory=self.product_factory,
@@ -162,14 +169,23 @@
                 time_model_factory=self.time_model_factory,
                 queue_factory=self.queue_factory,
                 resource_factory=self.resource_factory,
                 sink_factory=self.sink_factory,
             )
             self.source_factory.create_sources(self.adapter)
 
+            link_transport_process_updater_instance = link_transport_process_updater.LinkTransportProcessUpdater(
+                process_factory=self.process_factory,
+                source_factory=self.source_factory,
+                sink_factory=self.sink_factory,
+                resource_factory=self.resource_factory,
+                node_factory=self.node_factory,
+            )
+            link_transport_process_updater_instance.update_links_with_objects()
+            
             self.resource_factory.start_resources()
             self.source_factory.start_sources()
 
     def run(self, time_range: int):
         """
         Runs the simulation for the given time range.
```

### Comparing `prodsys-0.5.3/prodsys/util/statistical_functions.py` & `prodsys-0.6.0/prodsys/util/statistical_functions.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/prodsys/util/util.py` & `prodsys-0.6.0/prodsys/util/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 from collections.abc import Iterable
 
 import random
 import os
 
 import numpy as np
-from typing import List, Generator
+from typing import Any, List, Generator
 import warnings
 
 warnings.filterwarnings("ignore", category=RuntimeWarning)
 
 from os import listdir
 from os.path import isfile, join
 
@@ -125,15 +125,15 @@
     """
     for x in xs:
         if isinstance(x, Iterable) and not isinstance(x, (str, bytes)):
             yield from flatten(x)
         else:
             yield x
 
-def flatten_object(xs: list) -> list: # type: ignore
+def flatten_object(xs: list) -> Generator[Any, Any, list]:
     """
     Flattens a nested list.
 
     Args:
         xs (list): The nested list.
 
     Yields:
```

### Comparing `prodsys-0.5.3/pyproject.toml` & `prodsys-0.6.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prodsys"
-version = "0.5.3"
+version = "0.6.0"
 description = "A useful module for production system simulation and optimization"
 authors = ["Sebastian Behrendt <sebastia.behrendt@kit.edu>"]
 license = "MIT"
 readme = ["README.md", "LICENSE"]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.13"
@@ -32,14 +32,15 @@
 [tool.poetry.group.ai.dependencies]
 torch = "^2.0.1"
 torchvision = "^0.15.2"
 torchaudio = "^2.0.2"
 tensorboard = "^2.13.0"
 gymnasium = ">=0.26.3"
 stable-baselines3 = "^2.0.0"
+pathfinding = "^1.0.9"
 
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
```

### Comparing `prodsys-0.5.3/README.md` & `prodsys-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `prodsys-0.5.3/PKG-INFO` & `prodsys-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodsys
-Version: 0.5.3
+Version: 0.6.0
 Summary: A useful module for production system simulation and optimization
 License: MIT
 Author: Sebastian Behrendt
 Author-email: sebastia.behrendt@kit.edu
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

