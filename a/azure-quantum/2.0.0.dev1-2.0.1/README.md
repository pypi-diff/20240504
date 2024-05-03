# Comparing `tmp/azure-quantum-2.0.0.dev1.tar.gz` & `tmp/azure-quantum-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-quantum-2.0.0.dev1.tar", last modified: Tue Mar 19 20:33:06 2024, max compression
+gzip compressed data, was "azure-quantum-2.0.1.tar", last modified: Fri May  3 23:30:57 2024, max compression
```

## Comparing `azure-quantum-2.0.0.dev1.tar` & `azure-quantum-2.0.1.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 20:33:06.532563 azure-quantum-2.0.0.dev1/
--rw-rw-rw-   0        0        0     5610 2024-03-19 20:33:06.532563 azure-quantum-2.0.0.dev1/PKG-INFO
--rw-rw-rw-   0        0        0     5050 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-19 20:33:06.470061 azure-quantum-2.0.0.dev1/azure/
-drwxrwxrwx   0        0        0        0 2024-03-19 20:33:06.485688 azure-quantum-2.0.0.dev1/azure/quantum/
--rw-rw-rw-   0        0        0      508 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 20:33:06.485688 azure-quantum-2.0.0.dev1/azure/quantum/_authentication/
--rw-rw-rw-   0        0        0      236 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/_authentication/__init__.py
--rw-rw-rw-   0        0        0     4848 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/_authentication/_chained.py
--rw-rw-rw-   0        0        0     6625 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/_authentication/_default.py
--rw-rw-rw-   0        0        0     3616 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/_authentication/_token.py
-drwxrwxrwx   0        0        0        0 2024-03-19 20:33:06.501312 azure-quantum-2.0.0.dev1/azure/quantum/_client/
--rw-rw-rw-   0        0        0      896 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/_client/__init__.py
--rw-rw-rw-   0        0        0     7143 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/_client/_client.py
--rw-rw-rw-   0        0        0     4440 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/_client/_configuration.py
--rw-rw-rw-   0        0        0      694 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/_client/_patch.py
--rw-rw-rw-   0        0        0    81097 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/_client/_serialization.py
--rw-rw-rw-   0        0        0      996 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/_client/_vendor.py
--rw-rw-rw-   0        0        0      500 2024-03-19 20:33:06.000000 azure-quantum-2.0.0.dev1/azure/quantum/_client/_version.py
-drwxrwxrwx   0        0        0        0 2024-03-19 20:33:06.501312 azure-quantum-2.0.0.dev1/azure/quantum/_client/models/
--rw-rw-rw-   0        0        0     2100 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/_client/models/__init__.py
--rw-rw-rw-   0        0        0     2977 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/_client/models/_enums.py
--rw-rw-rw-   0        0        0    41810 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/_client/models/_models.py
--rw-rw-rw-   0        0        0      694 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/_client/models/_patch.py
-drwxrwxrwx   0        0        0        0 2024-03-19 20:33:06.501312 azure-quantum-2.0.0.dev1/azure/quantum/_client/operations/
--rw-rw-rw-   0        0        0     1154 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/_client/operations/__init__.py
--rw-rw-rw-   0        0        0    81928 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/_client/operations/_operations.py
--rw-rw-rw-   0        0        0      694 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/_client/operations/_patch.py
--rw-rw-rw-   0        0        0     3219 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/_constants.py
--rw-rw-rw-   0        0        0    21685 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/_workspace_connection_params.py
-drwxrwxrwx   0        0        0        0 2024-03-19 20:33:06.501312 azure-quantum-2.0.0.dev1/azure/quantum/argument_types/
--rw-rw-rw-   0        0        0      271 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/argument_types/__init__.py
--rw-rw-rw-   0        0        0     1041 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/argument_types/types.py
-drwxrwxrwx   0        0        0        0 2024-03-19 20:33:06.501312 azure-quantum-2.0.0.dev1/azure/quantum/chemistry/
--rw-rw-rw-   0        0        0      351 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/chemistry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 20:33:06.501312 azure-quantum-2.0.0.dev1/azure/quantum/cirq/
--rw-rw-rw-   0        0        0      227 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/cirq/__init__.py
--rw-rw-rw-   0        0        0     3031 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/cirq/job.py
--rw-rw-rw-   0        0        0     8880 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/cirq/service.py
-drwxrwxrwx   0        0        0        0 2024-03-19 20:33:06.501312 azure-quantum-2.0.0.dev1/azure/quantum/cirq/targets/
--rw-rw-rw-   0        0        0      574 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/cirq/targets/__init__.py
--rw-rw-rw-   0        0        0     6804 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/cirq/targets/ionq.py
--rw-rw-rw-   0        0        0     4537 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/cirq/targets/quantinuum.py
--rw-rw-rw-   0        0        0     2184 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/cirq/targets/target.py
-drwxrwxrwx   0        0        0        0 2024-03-19 20:33:06.501312 azure-quantum-2.0.0.dev1/azure/quantum/job/
--rw-rw-rw-   0        0        0      829 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/job/__init__.py
--rw-rw-rw-   0        0        0    12882 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/job/base_job.py
--rw-rw-rw-   0        0        0     1877 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/job/filtered_job.py
--rw-rw-rw-   0        0        0     6390 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/job/job.py
--rw-rw-rw-   0        0        0     1597 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/job/job_failed_with_results_error.py
--rw-rw-rw-   0        0        0    11961 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/job/session.py
--rw-rw-rw-   0        0        0     1380 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/job/workspace_item.py
--rw-rw-rw-   0        0        0     1200 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/job/workspace_item_factory.py
-drwxrwxrwx   0        0        0        0 2024-03-19 20:33:06.516938 azure-quantum-2.0.0.dev1/azure/quantum/qiskit/
--rw-rw-rw-   0        0        0      314 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/qiskit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 20:33:06.516938 azure-quantum-2.0.0.dev1/azure/quantum/qiskit/backends/
--rw-rw-rw-   0        0        0     1163 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/qiskit/backends/__init__.py
--rw-rw-rw-   0        0        0    20467 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/qiskit/backends/backend.py
--rw-rw-rw-   0        0        0    18024 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/qiskit/backends/ionq.py
--rw-rw-rw-   0        0        0     3441 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/qiskit/backends/microsoft.py
--rw-rw-rw-   0        0        0     4819 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/qiskit/backends/qci.py
--rw-rw-rw-   0        0        0    13635 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/qiskit/backends/quantinuum.py
--rw-rw-rw-   0        0        0     4248 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/qiskit/backends/rigetti.py
--rw-rw-rw-   0        0        0    14370 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/qiskit/job.py
--rw-rw-rw-   0        0        0    10975 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/qiskit/provider.py
-drwxrwxrwx   0        0        0        0 2024-03-19 20:33:06.516938 azure-quantum-2.0.0.dev1/azure/quantum/qiskit/results/
--rw-rw-rw-   0        0        0        0 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/qiskit/results/__init__.py
--rw-rw-rw-   0        0        0      814 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/qiskit/results/resource_estimator.py
--rw-rw-rw-   0        0        0    12556 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/storage.py
-drwxrwxrwx   0        0        0        0 2024-03-19 20:33:06.516938 azure-quantum-2.0.0.dev1/azure/quantum/target/
--rw-rw-rw-   0        0        0      689 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/target/__init__.py
--rw-rw-rw-   0        0        0     8130 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/target/ionq.py
-drwxrwxrwx   0        0        0        0 2024-03-19 20:33:06.516938 azure-quantum-2.0.0.dev1/azure/quantum/target/microsoft/
--rw-rw-rw-   0        0        0      570 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/target/microsoft/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 20:33:06.516938 azure-quantum-2.0.0.dev1/azure/quantum/target/microsoft/elements/
--rw-rw-rw-   0        0        0       70 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/target/microsoft/elements/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 20:33:06.516938 azure-quantum-2.0.0.dev1/azure/quantum/target/microsoft/elements/dft/
--rw-rw-rw-   0        0        0      224 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/target/microsoft/elements/dft/__init__.py
--rw-rw-rw-   0        0        0     2936 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/target/microsoft/elements/dft/job.py
--rw-rw-rw-   0        0        0     2556 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/target/microsoft/elements/dft/target.py
--rw-rw-rw-   0        0        0     1249 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/target/microsoft/job.py
--rw-rw-rw-   0        0        0    18784 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/target/microsoft/result.py
--rw-rw-rw-   0        0        0    17879 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/target/microsoft/target.py
--rw-rw-rw-   0        0        0     9130 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/target/params.py
-drwxrwxrwx   0        0        0        0 2024-03-19 20:33:06.516938 azure-quantum-2.0.0.dev1/azure/quantum/target/pasqal/
--rw-rw-rw-   0        0        0      348 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/target/pasqal/__init__.py
--rw-rw-rw-   0        0        0     1463 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/target/pasqal/result.py
--rw-rw-rw-   0        0        0     4833 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/target/pasqal/target.py
--rw-rw-rw-   0        0        0     7710 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/target/quantinuum.py
-drwxrwxrwx   0        0        0        0 2024-03-19 20:33:06.532563 azure-quantum-2.0.0.dev1/azure/quantum/target/rigetti/
--rw-rw-rw-   0        0        0      378 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/target/rigetti/__init__.py
--rw-rw-rw-   0        0        0     2334 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/target/rigetti/result.py
--rw-rw-rw-   0        0        0     7219 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/target/rigetti/target.py
--rw-rw-rw-   0        0        0    13868 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/target/target.py
--rw-rw-rw-   0        0        0     5053 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/target/target_factory.py
--rw-rw-rw-   0        0        0      240 2024-03-19 20:33:06.000000 azure-quantum-2.0.0.dev1/azure/quantum/version.py
--rw-rw-rw-   0        0        0    23438 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/azure/quantum/workspace.py
-drwxrwxrwx   0        0        0        0 2024-03-19 20:33:06.532563 azure-quantum-2.0.0.dev1/azure_quantum.egg-info/
--rw-rw-rw-   0        0        0     5610 2024-03-19 20:33:06.000000 azure-quantum-2.0.0.dev1/azure_quantum.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3130 2024-03-19 20:33:06.000000 azure-quantum-2.0.0.dev1/azure_quantum.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 20:33:06.000000 azure-quantum-2.0.0.dev1/azure_quantum.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      744 2024-03-19 20:33:06.000000 azure-quantum-2.0.0.dev1/azure_quantum.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-19 20:33:06.000000 azure-quantum-2.0.0.dev1/azure_quantum.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       52 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/requirements-cirq.txt
--rw-rw-rw-   0        0        0      112 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/requirements-dev.txt
--rw-rw-rw-   0        0        0      117 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/requirements-qiskit.txt
--rw-rw-rw-   0        0        0       19 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/requirements-qsharp.txt
--rw-rw-rw-   0        0        0      275 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/requirements-quil.txt
--rw-rw-rw-   0        0        0      192 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-03-19 20:33:06.532563 azure-quantum-2.0.0.dev1/setup.cfg
--rw-rw-rw-   0        0        0     3838 2024-03-19 20:32:38.000000 azure-quantum-2.0.0.dev1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.667572 azure-quantum-2.0.1/
+-rw-rw-rw-   0        0        0     5605 2024-05-03 23:30:57.667572 azure-quantum-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5050 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.601638 azure-quantum-2.0.1/azure/
+drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.617265 azure-quantum-2.0.1/azure/quantum/
+-rw-rw-rw-   0        0        0      508 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.617265 azure-quantum-2.0.1/azure/quantum/_authentication/
+-rw-rw-rw-   0        0        0      236 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_authentication/__init__.py
+-rw-rw-rw-   0        0        0     4848 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_authentication/_chained.py
+-rw-rw-rw-   0        0        0     6625 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_authentication/_default.py
+-rw-rw-rw-   0        0        0     3616 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_authentication/_token.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.617265 azure-quantum-2.0.1/azure/quantum/_client/
+-rw-rw-rw-   0        0        0      896 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_client/__init__.py
+-rw-rw-rw-   0        0        0     7143 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_client/_client.py
+-rw-rw-rw-   0        0        0     4440 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_client/_configuration.py
+-rw-rw-rw-   0        0        0      694 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_client/_patch.py
+-rw-rw-rw-   0        0        0    81097 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_client/_serialization.py
+-rw-rw-rw-   0        0        0      996 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_client/_vendor.py
+-rw-rw-rw-   0        0        0      495 2024-05-03 23:30:57.000000 azure-quantum-2.0.1/azure/quantum/_client/_version.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.617265 azure-quantum-2.0.1/azure/quantum/_client/models/
+-rw-rw-rw-   0        0        0     2100 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_client/models/__init__.py
+-rw-rw-rw-   0        0        0     2977 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_client/models/_enums.py
+-rw-rw-rw-   0        0        0    41810 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_client/models/_models.py
+-rw-rw-rw-   0        0        0      694 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_client/models/_patch.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.617265 azure-quantum-2.0.1/azure/quantum/_client/operations/
+-rw-rw-rw-   0        0        0     1154 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_client/operations/__init__.py
+-rw-rw-rw-   0        0        0    81928 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_client/operations/_operations.py
+-rw-rw-rw-   0        0        0      694 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_client/operations/_patch.py
+-rw-rw-rw-   0        0        0     3219 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_constants.py
+-rw-rw-rw-   0        0        0    21685 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/_workspace_connection_params.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.617265 azure-quantum-2.0.1/azure/quantum/argument_types/
+-rw-rw-rw-   0        0        0      271 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/argument_types/__init__.py
+-rw-rw-rw-   0        0        0     1041 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/argument_types/types.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.617265 azure-quantum-2.0.1/azure/quantum/chemistry/
+-rw-rw-rw-   0        0        0      351 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/chemistry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.632892 azure-quantum-2.0.1/azure/quantum/cirq/
+-rw-rw-rw-   0        0        0      227 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/cirq/__init__.py
+-rw-rw-rw-   0        0        0     3031 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/cirq/job.py
+-rw-rw-rw-   0        0        0     8880 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/cirq/service.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.632892 azure-quantum-2.0.1/azure/quantum/cirq/targets/
+-rw-rw-rw-   0        0        0      574 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/cirq/targets/__init__.py
+-rw-rw-rw-   0        0        0     6804 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/cirq/targets/ionq.py
+-rw-rw-rw-   0        0        0     4537 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/cirq/targets/quantinuum.py
+-rw-rw-rw-   0        0        0     2184 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/cirq/targets/target.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.632892 azure-quantum-2.0.1/azure/quantum/job/
+-rw-rw-rw-   0        0        0      829 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/job/__init__.py
+-rw-rw-rw-   0        0        0    13876 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/job/base_job.py
+-rw-rw-rw-   0        0        0     1877 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/job/filtered_job.py
+-rw-rw-rw-   0        0        0     6390 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/job/job.py
+-rw-rw-rw-   0        0        0     1597 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/job/job_failed_with_results_error.py
+-rw-rw-rw-   0        0        0    11961 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/job/session.py
+-rw-rw-rw-   0        0        0     1380 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/job/workspace_item.py
+-rw-rw-rw-   0        0        0     1200 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/job/workspace_item_factory.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.632892 azure-quantum-2.0.1/azure/quantum/qiskit/
+-rw-rw-rw-   0        0        0      314 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/qiskit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.632892 azure-quantum-2.0.1/azure/quantum/qiskit/backends/
+-rw-rw-rw-   0        0        0     1163 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/qiskit/backends/__init__.py
+-rw-rw-rw-   0        0        0    20467 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/qiskit/backends/backend.py
+-rw-rw-rw-   0        0        0    18024 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/qiskit/backends/ionq.py
+-rw-rw-rw-   0        0        0     3478 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/qiskit/backends/microsoft.py
+-rw-rw-rw-   0        0        0     4893 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/qiskit/backends/qci.py
+-rw-rw-rw-   0        0        0    13437 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/qiskit/backends/quantinuum.py
+-rw-rw-rw-   0        0        0     4322 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/qiskit/backends/rigetti.py
+-rw-rw-rw-   0        0        0    14370 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/qiskit/job.py
+-rw-rw-rw-   0        0        0    10946 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/qiskit/provider.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.648513 azure-quantum-2.0.1/azure/quantum/qiskit/results/
+-rw-rw-rw-   0        0        0        0 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/qiskit/results/__init__.py
+-rw-rw-rw-   0        0        0      814 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/qiskit/results/resource_estimator.py
+-rw-rw-rw-   0        0        0    12556 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/storage.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.648513 azure-quantum-2.0.1/azure/quantum/target/
+-rw-rw-rw-   0        0        0      689 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/__init__.py
+-rw-rw-rw-   0        0        0     8130 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/ionq.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.648513 azure-quantum-2.0.1/azure/quantum/target/microsoft/
+-rw-rw-rw-   0        0        0      570 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/microsoft/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.648513 azure-quantum-2.0.1/azure/quantum/target/microsoft/elements/
+-rw-rw-rw-   0        0        0       70 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/microsoft/elements/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.648513 azure-quantum-2.0.1/azure/quantum/target/microsoft/elements/dft/
+-rw-rw-rw-   0        0        0      224 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/microsoft/elements/dft/__init__.py
+-rw-rw-rw-   0        0        0     2936 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/microsoft/elements/dft/job.py
+-rw-rw-rw-   0        0        0     2556 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/microsoft/elements/dft/target.py
+-rw-rw-rw-   0        0        0     1249 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/microsoft/job.py
+-rw-rw-rw-   0        0        0    18784 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/microsoft/result.py
+-rw-rw-rw-   0        0        0    17879 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/microsoft/target.py
+-rw-rw-rw-   0        0        0     9130 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/params.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.648513 azure-quantum-2.0.1/azure/quantum/target/pasqal/
+-rw-rw-rw-   0        0        0      348 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/pasqal/__init__.py
+-rw-rw-rw-   0        0        0     1463 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/pasqal/result.py
+-rw-rw-rw-   0        0        0     4833 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/pasqal/target.py
+-rw-rw-rw-   0        0        0     7612 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/quantinuum.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.664138 azure-quantum-2.0.1/azure/quantum/target/rigetti/
+-rw-rw-rw-   0        0        0      378 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/rigetti/__init__.py
+-rw-rw-rw-   0        0        0     2334 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/rigetti/result.py
+-rw-rw-rw-   0        0        0     7048 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/rigetti/target.py
+-rw-rw-rw-   0        0        0    13868 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/target.py
+-rw-rw-rw-   0        0        0     5266 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/target/target_factory.py
+-rw-rw-rw-   0        0        0      235 2024-05-03 23:30:57.000000 azure-quantum-2.0.1/azure/quantum/version.py
+-rw-rw-rw-   0        0        0    23438 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/azure/quantum/workspace.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:30:57.667572 azure-quantum-2.0.1/azure_quantum.egg-info/
+-rw-rw-rw-   0        0        0     5605 2024-05-03 23:30:57.000000 azure-quantum-2.0.1/azure_quantum.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3130 2024-05-03 23:30:57.000000 azure-quantum-2.0.1/azure_quantum.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 23:30:57.000000 azure-quantum-2.0.1/azure_quantum.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      744 2024-05-03 23:30:57.000000 azure-quantum-2.0.1/azure_quantum.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-03 23:30:57.000000 azure-quantum-2.0.1/azure_quantum.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       52 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/requirements-cirq.txt
+-rw-rw-rw-   0        0        0      112 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0      117 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/requirements-qiskit.txt
+-rw-rw-rw-   0        0        0       19 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/requirements-qsharp.txt
+-rw-rw-rw-   0        0        0      275 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/requirements-quil.txt
+-rw-rw-rw-   0        0        0      192 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 23:30:57.667572 azure-quantum-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     3838 2024-05-03 23:30:18.000000 azure-quantum-2.0.1/setup.py
```

### Comparing `azure-quantum-2.0.0.dev1/PKG-INFO` & `azure-quantum-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-quantum
-Version: 2.0.0.dev1
+Version: 2.0.1
 Summary: Python client for Azure Quantum
 Home-page: https://github.com/microsoft/azure-quantum-python
 Author: Microsoft
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `azure-quantum-2.0.0.dev1/README.md` & `azure-quantum-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/_authentication/_chained.py` & `azure-quantum-2.0.1/azure/quantum/_authentication/_chained.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/_authentication/_default.py` & `azure-quantum-2.0.1/azure/quantum/_authentication/_default.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/_authentication/_token.py` & `azure-quantum-2.0.1/azure/quantum/_authentication/_token.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/_client/__init__.py` & `azure-quantum-2.0.1/azure/quantum/_client/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/_client/_client.py` & `azure-quantum-2.0.1/azure/quantum/_client/_client.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/_client/_configuration.py` & `azure-quantum-2.0.1/azure/quantum/_client/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/_client/_patch.py` & `azure-quantum-2.0.1/azure/quantum/_client/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/_client/_serialization.py` & `azure-quantum-2.0.1/azure/quantum/_client/_serialization.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/_client/_vendor.py` & `azure-quantum-2.0.1/azure/quantum/_client/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/_client/models/__init__.py` & `azure-quantum-2.0.1/azure/quantum/_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/_client/models/_enums.py` & `azure-quantum-2.0.1/azure/quantum/_client/models/_enums.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/_client/models/_models.py` & `azure-quantum-2.0.1/azure/quantum/_client/models/_models.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/_client/models/_patch.py` & `azure-quantum-2.0.1/azure/quantum/_client/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/_client/operations/__init__.py` & `azure-quantum-2.0.1/azure/quantum/_client/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/_client/operations/_operations.py` & `azure-quantum-2.0.1/azure/quantum/_client/operations/_operations.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/_client/operations/_patch.py` & `azure-quantum-2.0.1/azure/quantum/_client/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/_constants.py` & `azure-quantum-2.0.1/azure/quantum/_constants.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/_workspace_connection_params.py` & `azure-quantum-2.0.1/azure/quantum/_workspace_connection_params.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/argument_types/types.py` & `azure-quantum-2.0.1/azure/quantum/argument_types/types.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/cirq/job.py` & `azure-quantum-2.0.1/azure/quantum/cirq/job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/cirq/service.py` & `azure-quantum-2.0.1/azure/quantum/cirq/service.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/cirq/targets/__init__.py` & `azure-quantum-2.0.1/azure/quantum/cirq/targets/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/cirq/targets/ionq.py` & `azure-quantum-2.0.1/azure/quantum/cirq/targets/ionq.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/cirq/targets/quantinuum.py` & `azure-quantum-2.0.1/azure/quantum/cirq/targets/quantinuum.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/cirq/targets/target.py` & `azure-quantum-2.0.1/azure/quantum/cirq/targets/target.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/job/__init__.py` & `azure-quantum-2.0.1/azure/quantum/job/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/job/base_job.py` & `azure-quantum-2.0.1/azure/quantum/job/base_job.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # Licensed under the MIT License.
 ##
 import abc
 import logging
 import uuid
 
 from enum import Enum
-from urllib.parse import urlparse
+from datetime import datetime, timezone, timedelta
+from urllib.parse import urlparse, parse_qs
 from typing import Any, Dict, Optional, TYPE_CHECKING
 from azure.storage.blob import BlobClient
 
 from azure.quantum.storage import upload_blob, download_blob, download_blob_properties, ContainerClient
 from azure.quantum._client.models import JobDetails
 from azure.quantum.job.workspace_item import WorkspaceItem
 
@@ -364,16 +365,35 @@
         """Get Blob URI with SAS-token if one was not specified in blob_uri parameter
         :param blob_uri: Blob URI
         :type blob_uri: str
         :return: Blob URI with SAS-token
         :rtype: str
         """
         url = urlparse(blob_uri)
-        if url.query.find("se=") == -1:
-            # blob_uri does not contains SAS token,
+        query_params = parse_qs(url.query)
+        token_expire_query_param = query_params.get("se")
+
+        token_expire_time = None
+
+        if token_expire_query_param is not None:
+            token_expire_time_str = token_expire_query_param[0]
+
+            # Since python < 3.11 can not easily parse Z suffixed UTC timestamp and 
+            # assuming that the timestamp is always UTC, we replace that suffix with UTC offset.
+            token_expire_time = datetime.fromisoformat(
+                token_expire_time_str.replace('Z', '+00:00')
+            )
+            
+            # Make an expiration time a little earlier, so there's no case where token is
+            # used a second or so before of its expiration.
+            token_expire_time = token_expire_time - timedelta(minutes=5)
+
+        current_utc_time = datetime.now(tz=timezone.utc)
+        if token_expire_time is None or current_utc_time >= token_expire_time:
+            # blob_uri does not contains SAS token or it is expired,
             # get sas url from service
             blob_client = BlobClient.from_blob_url(
                 blob_uri
             )
             blob_uri = self.workspace._get_linked_storage_sas_uri(
                 blob_client.container_name, blob_client.blob_name
             )
```

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/job/filtered_job.py` & `azure-quantum-2.0.1/azure/quantum/job/filtered_job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/job/job.py` & `azure-quantum-2.0.1/azure/quantum/job/job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/job/job_failed_with_results_error.py` & `azure-quantum-2.0.1/azure/quantum/job/job_failed_with_results_error.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/job/session.py` & `azure-quantum-2.0.1/azure/quantum/job/session.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/job/workspace_item.py` & `azure-quantum-2.0.1/azure/quantum/job/workspace_item.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/job/workspace_item_factory.py` & `azure-quantum-2.0.1/azure/quantum/job/workspace_item_factory.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/qiskit/backends/__init__.py` & `azure-quantum-2.0.1/azure/quantum/qiskit/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/qiskit/backends/backend.py` & `azure-quantum-2.0.1/azure/quantum/qiskit/backends/backend.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/qiskit/backends/ionq.py` & `azure-quantum-2.0.1/azure/quantum/qiskit/backends/ionq.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/qiskit/backends/microsoft.py` & `azure-quantum-2.0.1/azure/quantum/qiskit/backends/microsoft.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,15 @@
                 "max_shots": 1,
                 "max_experiments": 1,
                 "open_pulse": False,
                 "gates": [
                     {"name": "TODO", "parameters": [], "qasm_def": "TODO"}
                 ],  # NOTE: copied from other backends
                 "azure": self._azure_config(),
+                "is_default": True,
             }
         )
         logger.info("Initializing MicrosoftResourceEstimationBackend")
         configuration: BackendConfiguration = kwargs.pop(
             "configuration", default_config
         )
         super().__init__(configuration=configuration, provider=provider, **kwargs)
```

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/qiskit/backends/qci.py` & `azure-quantum-2.0.1/azure/quantum/qiskit/backends/qci.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,15 @@
                 "n_qubits": 29,
                 "conditional": True,
                 "max_shots": 1e6,
                 "max_experiments": 1,
                 "open_pulse": False,
                 "gates": [{"name": "TODO", "parameters": [], "qasm_def": "TODO"}],
                 "azure": self._azure_config(),
+                "is_default": True,
             }
         )
         logger.info("Initializing QCISimulatorBackend")
         configuration: BackendConfiguration = kwargs.pop(
             "configuration", default_config
         )
         super().__init__(configuration=configuration, provider=provider, **kwargs)
@@ -146,14 +147,15 @@
                 "n_qubits": 11,
                 "conditional": True,
                 "max_shots": 10000,
                 "max_experiments": 1,
                 "open_pulse": False,
                 "gates": [{"name": "TODO", "parameters": [], "qasm_def": "TODO"}],
                 "azure": self._azure_config(),
+                "is_default": True,
             }
         )
         logger.info("Initializing QCIQPUBackend")
         configuration: BackendConfiguration = kwargs.pop(
             "configuration", default_config
         )
         super().__init__(configuration=configuration, provider=provider, **kwargs)
```

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/qiskit/backends/quantinuum.py` & `azure-quantum-2.0.1/azure/quantum/qiskit/backends/quantinuum.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,14 @@
         return _get_n_qubits(name)
 
 
 class QuantinuumSyntaxCheckerQirBackend(QuantinuumQirBackendBase):
     backend_names = (
         # Note: Target names on the same line are equivalent.
         "quantinuum.sim.h1-1sc",
-        "quantinuum.sim.h1-2sc",
         "quantinuum.sim.h2-1sc",
     )
 
     def __init__(self, name: str, provider: "AzureQuantumProvider", **kwargs):
         self._provider_id = QUANTINUUM_PROVIDER_ID
         self._provider_name = QUANTINUUM_PROVIDER_NAME
 
@@ -137,15 +136,14 @@
         super().__init__(configuration=configuration, provider=provider, **kwargs)
 
 
 class QuantinuumEmulatorQirBackend(QuantinuumQirBackendBase):
     backend_names = (
         # Note: Target names on the same line are equivalent.
         "quantinuum.sim.h1-1e",
-        "quantinuum.sim.h1-2e",
         "quantinuum.sim.h2-1e",
     )
 
     def __init__(self, name: str, provider: "AzureQuantumProvider", **kwargs):
         self._provider_id = QUANTINUUM_PROVIDER_ID
         self._provider_name = QUANTINUUM_PROVIDER_NAME
 
@@ -175,15 +173,14 @@
         super().__init__(configuration=configuration, provider=provider, **kwargs)
 
 
 class QuantinuumQPUQirBackend(QuantinuumQirBackendBase):
     backend_names = (
         # Note: Target names on the same line are equivalent.
         "quantinuum.qpu.h1-1",
-        "quantinuum.qpu.h1-2",
         "quantinuum.qpu.h2-1",
     )
 
     def __init__(self, name: str, provider: "AzureQuantumProvider", **kwargs):
         self._provider_id = QUANTINUUM_PROVIDER_ID
         self._provider_name = QUANTINUUM_PROVIDER_NAME
 
@@ -277,15 +274,14 @@
         return _get_n_qubits(name)
 
 
 class QuantinuumSyntaxCheckerBackend(QuantinuumBackend):
     backend_names = (
         # Note: Target names on the same line are equivalent.
         "quantinuum.sim.h1-1sc",
-        "quantinuum.sim.h1-2sc",
         "quantinuum.sim.h2-1sc",
     )
 
     def __init__(self, name: str, provider: "AzureQuantumProvider", **kwargs):
         self._provider_id = QUANTINUUM_PROVIDER_ID
         self._provider_name = QUANTINUUM_PROVIDER_NAME
 
@@ -315,15 +311,14 @@
         super().__init__(configuration=configuration, provider=provider, **kwargs)
 
 
 class QuantinuumEmulatorBackend(QuantinuumBackend):
     backend_names = (
         # Note: Target names on the same line are equivalent.
         "quantinuum.sim.h1-1e",
-        "quantinuum.sim.h1-2e",
         "quantinuum.sim.h2-1e",
     )
 
     def __init__(self, name: str, provider: "AzureQuantumProvider", **kwargs):
         self._provider_id = QUANTINUUM_PROVIDER_ID
         self._provider_name = QUANTINUUM_PROVIDER_NAME
 
@@ -353,15 +348,14 @@
         super().__init__(configuration=configuration, provider=provider, **kwargs)
 
 
 class QuantinuumQPUBackend(QuantinuumBackend):
     backend_names = (
         # Note: Target names on the same line are equivalent.
         "quantinuum.qpu.h1-1",
-        "quantinuum.qpu.h1-2",
         "quantinuum.qpu.h2-1",
     )
 
     def __init__(self, name: str, provider: "AzureQuantumProvider", **kwargs):
         self._provider_id = QUANTINUUM_PROVIDER_ID
         self._provider_name = QUANTINUUM_PROVIDER_NAME
```

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/qiskit/backends/rigetti.py` & `azure-quantum-2.0.1/azure/quantum/qiskit/backends/rigetti.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,15 @@
                 "n_qubits": RigettiTarget.num_qubits(name),
                 "conditional": False,
                 "max_shots": 10000,
                 "max_experiments": 1,
                 "open_pulse": False,
                 "gates": [{"name": "TODO", "parameters": [], "qasm_def": "TODO"}],
                 "azure": self._azure_config(),
+                "is_default": True,
             }
         )
         logger.info("Initializing RigettiSimulatorBackend")
         configuration: BackendConfiguration = kwargs.pop(
             "configuration", default_config
         )
         super().__init__(configuration=configuration, provider=provider, **kwargs)
@@ -121,14 +122,15 @@
                 "n_qubits": RigettiTarget.num_qubits(name),
                 "conditional": False,
                 "max_shots": 10000,
                 "max_experiments": 1,
                 "open_pulse": False,
                 "gates": [{"name": "TODO", "parameters": [], "qasm_def": "TODO"}],
                 "azure": self._azure_config(),
+                "is_default": True,
             }
         )
         logger.info("Initializing RigettiQPUBackend")
         configuration: BackendConfiguration = kwargs.pop(
             "configuration", default_config
         )
         super().__init__(configuration=configuration, provider=provider, **kwargs)
```

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/qiskit/job.py` & `azure-quantum-2.0.1/azure/quantum/qiskit/job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/qiskit/provider.py` & `azure-quantum-2.0.1/azure/quantum/qiskit/provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,30 +67,14 @@
             QiskitBackendNotFoundError: if no backend could be found or
                 more than one backend matches the filtering criteria.
         """
 
         backends = self.backends(name=name, **kwargs)
 
         if len(backends) > 1:
-            def all_same(iterable):
-                group_iter = groupby(iterable)
-                return next(group_iter, True) and not next(group_iter, False)
-
-            # If all backends have the same name, filter for default backend
-            if all_same(backend.name() for backend in backends):
-                backends = list(
-                    filter(
-                        lambda backend: self._match_all(
-                            backend.configuration().to_dict(), {"is_default": True}
-                        ),
-                        backends,
-                    )
-                )
-
-        if len(backends) > 1:
             raise QiskitBackendNotFoundError(
                 "More than one backend matches the criteria"
             )
         if not backends:
             raise QiskitBackendNotFoundError(
                 f"Could not find target '{name}'. \
 Please make sure the target name is valid and that the associated provider is added to your Workspace. \
@@ -128,19 +112,33 @@
             allowed_targets, backend
         )
 
         # flatten the available backends
         backend_list = [x for v in self._backends.values() for x in v]
 
         # filter by properties specified in the kwargs and filter function
-        backends: List[Backend] = self._filter_backends(
+        filtered_backends: List[Backend] = self._filter_backends(
             backend_list, filters=workspace_allowed, **kwargs
         )
 
-        return backends
+        # Also filter out non-default backends.
+        default_backends = list(
+            filter(
+                lambda backend: self._match_all(
+                    backend.configuration().to_dict(), {"is_default": True}
+                ),
+                filtered_backends,
+            )
+        ) 
+       # If default backends were found - return them, otherwise return the filtered_backends collection.
+       # The latter case could happen where there's no default backend defined for the specified target.  
+        if len(default_backends) > 0:
+            return default_backends
+
+        return filtered_backends
 
     def get_job(self, job_id) -> AzureQuantumJob:
         """Returns the Job instance associated with the given id.
         
         Args:
             job_id (str): Id of the Job to return.
         Returns:
```

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/qiskit/results/resource_estimator.py` & `azure-quantum-2.0.1/azure/quantum/qiskit/results/resource_estimator.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/storage.py` & `azure-quantum-2.0.1/azure/quantum/storage.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/target/__init__.py` & `azure-quantum-2.0.1/azure/quantum/target/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/target/ionq.py` & `azure-quantum-2.0.1/azure/quantum/target/ionq.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/target/microsoft/__init__.py` & `azure-quantum-2.0.1/azure/quantum/target/microsoft/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/target/microsoft/elements/dft/job.py` & `azure-quantum-2.0.1/azure/quantum/target/microsoft/elements/dft/job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/target/microsoft/elements/dft/target.py` & `azure-quantum-2.0.1/azure/quantum/target/microsoft/elements/dft/target.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/target/microsoft/job.py` & `azure-quantum-2.0.1/azure/quantum/target/microsoft/job.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/target/microsoft/result.py` & `azure-quantum-2.0.1/azure/quantum/target/microsoft/result.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/target/microsoft/target.py` & `azure-quantum-2.0.1/azure/quantum/target/microsoft/target.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/target/params.py` & `azure-quantum-2.0.1/azure/quantum/target/params.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/target/pasqal/result.py` & `azure-quantum-2.0.1/azure/quantum/target/pasqal/result.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/target/pasqal/target.py` & `azure-quantum-2.0.1/azure/quantum/target/pasqal/target.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/target/quantinuum.py` & `azure-quantum-2.0.1/azure/quantum/target/quantinuum.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,17 +17,14 @@
 class Quantinuum(Target):
     """Quantinuum target."""
     target_names = (
         # Note: Target names on the same line are equivalent.
         "quantinuum.qpu.h1-1",
         "quantinuum.sim.h1-1sc",
         "quantinuum.sim.h1-1e",
-        "quantinuum.qpu.h1-2",
-        "quantinuum.sim.h1-2sc",
-        "quantinuum.sim.h1-2e"
         "quantinuum.qpu.h2-1",
         "quantinuum.sim.h2-1sc",
         "quantinuum.sim.h2-1e",
     )
 
     _SHOTS_PARAM_NAME = "count"
```

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/target/rigetti/result.py` & `azure-quantum-2.0.1/azure/quantum/target/rigetti/result.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/target/rigetti/target.py` & `azure-quantum-2.0.1/azure/quantum/target/rigetti/target.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,36 +25,32 @@
 
     See https://qcs.rigetti.com/qpus for details on a QPU target.
     """
 
     QVM = "rigetti.sim.qvm"
     """A simulator target for Quil. See https://github.com/quil-lang/qvm for more info."""
 
-    ANKAA_9Q_1 = "rigetti.qpu.ankaa-9q-1"
     ANKAA_2 = "rigetti.qpu.ankaa-2"
 
     def simulators() -> List[str]:
         """Returns a list of simulator targets"""
         return [
             RigettiTarget.QVM.value,
         ]
 
     def qpus() -> List[str]:
         """Returns a list of QPU targets"""
         return [
-            RigettiTarget.ANKAA_9Q_1.value,
             RigettiTarget.ANKAA_2.value,
         ]
 
     def num_qubits(target_name) -> int:
         """Returns the number of qubits supported by the given target"""
 
-        if target_name == RigettiTarget.ANKAA_9Q_1.value:
-            return 9
-        elif target_name == RigettiTarget.QVM.value:
+        if target_name == RigettiTarget.QVM.value:
             return 20
         elif target_name == RigettiTarget.ANKAA_2.value:
             return 84
         else:
             raise ValueError(f"Unknown target {target_name}")
```

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/target/target.py` & `azure-quantum-2.0.1/azure/quantum/target/target.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/target/target_factory.py` & `azure-quantum-2.0.1/azure/quantum/target/target_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,16 +107,16 @@
         if hasattr(cls, "from_target_status"):
             return cls.from_target_status(self._workspace, status, **kwargs)
         elif cls is not None:
             return cls(name=status.id, **kwargs)
 
     def get_targets(
         self,
-        name: str,
-        provider_id: str,
+        name: str = None,
+        provider_id: str = None,
         **kwargs
     ) -> Union[Target, List[Target]]:
         """Create targets that are available to this workspace
         filtered by name and provider ID.
 
         :param name: Target name
         :type name: str
@@ -125,16 +125,21 @@
         :param provider_id: Provider name
         :type provider_id: str
         :return: One or more Target objects
         :rtype: Union[Target, List[Target]]
         """
         target_statuses = self._workspace._get_target_status(name, provider_id)
 
+        # TODO: Make this function always return a list in the next major release.
         if len(target_statuses) == 1:
-            return self.from_target_status(*target_statuses[0], **kwargs)
+            result = self.from_target_status(*target_statuses[0], **kwargs)
+            if name is None:
+                return [result]
+            else:
+                return result
 
         else:
             # Don't return redundant targets
             return [
                 self.from_target_status(_provider_id, status, **kwargs)
                 for _provider_id, status in target_statuses
                 if _provider_id.lower() in self._default_targets
```

### Comparing `azure-quantum-2.0.0.dev1/azure/quantum/workspace.py` & `azure-quantum-2.0.1/azure/quantum/workspace.py`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure_quantum.egg-info/PKG-INFO` & `azure-quantum-2.0.1/azure_quantum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-quantum
-Version: 2.0.0.dev1
+Version: 2.0.1
 Summary: Python client for Azure Quantum
 Home-page: https://github.com/microsoft/azure-quantum-python
 Author: Microsoft
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `azure-quantum-2.0.0.dev1/azure_quantum.egg-info/SOURCES.txt` & `azure-quantum-2.0.1/azure_quantum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/azure_quantum.egg-info/requires.txt` & `azure-quantum-2.0.1/azure_quantum.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `azure-quantum-2.0.0.dev1/setup.py` & `azure-quantum-2.0.1/setup.py`

 * *Files identical despite different names*

