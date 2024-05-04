# Comparing `tmp/omnisafe-0.4.0.tar.gz` & `tmp/omnisafe-0.5.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnisafe-0.4.0.tar", last modified: Mon May  8 20:07:23 2023, max compression
+gzip compressed data, was "omnisafe-0.5.0b0.tar", last modified: Thu Jun  1 18:21:46 2023, max compression
```

## Comparing `omnisafe-0.4.0.tar` & `omnisafe-0.5.0b0.tar`

### file list

```diff
@@ -1,209 +1,245 @@
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.118508 omnisafe-0.4.0/
--rw-r--r--   0 jiaming    (501) staff       (20)    11375 2023-05-08 19:46:32.000000 omnisafe-0.4.0/LICENSE
--rw-r--r--   0 jiaming    (501) staff       (20)       43 2023-05-08 19:46:32.000000 omnisafe-0.4.0/MANIFEST.in
--rw-r--r--   0 jiaming    (501) staff       (20)    17209 2023-05-08 20:07:23.118334 omnisafe-0.4.0/PKG-INFO
--rw-r--r--   0 jiaming    (501) staff       (20)    16005 2023-05-08 19:53:25.000000 omnisafe-0.4.0/README.md
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.094657 omnisafe-0.4.0/omnisafe/
--rw-r--r--   0 jiaming    (501) staff       (20)      997 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/__init__.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.096581 omnisafe-0.4.0/omnisafe/adapter/
--rw-r--r--   0 jiaming    (501) staff       (20)     1117 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/adapter/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3332 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/adapter/early_terminated_adapter.py
--rw-r--r--   0 jiaming    (501) staff       (20)    13974 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/adapter/modelbased_adapter.py
--rw-r--r--   0 jiaming    (501) staff       (20)     7703 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/adapter/offpolicy_adapter.py
--rw-r--r--   0 jiaming    (501) staff       (20)     8063 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/adapter/online_adapter.py
--rw-r--r--   0 jiaming    (501) staff       (20)     6745 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/adapter/onpolicy_adapter.py
--rw-r--r--   0 jiaming    (501) staff       (20)     9663 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/adapter/saute_adapter.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4872 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/adapter/simmer_adapter.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.097152 omnisafe-0.4.0/omnisafe/algorithms/
--rw-r--r--   0 jiaming    (501) staff       (20)     2054 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)    10644 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/algo_wrapper.py
--rw-r--r--   0 jiaming    (501) staff       (20)     2583 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/base_algo.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.098139 omnisafe-0.4.0/omnisafe/algorithms/model_based/
--rw-r--r--   0 jiaming    (501) staff       (20)     1166 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/__init__.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.098745 omnisafe-0.4.0/omnisafe/algorithms/model_based/base/
--rw-r--r--   0 jiaming    (501) staff       (20)      892 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/base/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)    30036 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/base/ensemble.py
--rw-r--r--   0 jiaming    (501) staff       (20)    16182 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/base/loop.py
--rw-r--r--   0 jiaming    (501) staff       (20)    19238 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/base/pets.py
--rw-r--r--   0 jiaming    (501) staff       (20)     5077 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/cap_pets.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3640 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/cce_pets.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.099717 omnisafe-0.4.0/omnisafe/algorithms/model_based/planner/
--rw-r--r--   0 jiaming    (501) staff       (20)     1252 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/planner/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)    13125 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/planner/arc.py
--rw-r--r--   0 jiaming    (501) staff       (20)     7088 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/planner/cap.py
--rw-r--r--   0 jiaming    (501) staff       (20)     6127 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/planner/cce.py
--rw-r--r--   0 jiaming    (501) staff       (20)    11664 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/planner/cem.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4926 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/planner/rce.py
--rw-r--r--   0 jiaming    (501) staff       (20)    10530 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/planner/safe_arc.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3567 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/rce_pets.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4071 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/algorithms/model_based/safeloop.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.100648 omnisafe-0.4.0/omnisafe/algorithms/off_policy/
--rw-r--r--   0 jiaming    (501) staff       (20)     1107 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/off_policy/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)    22970 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/off_policy/ddpg.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3989 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/off_policy/ddpg_lag.py
--rw-r--r--   0 jiaming    (501) staff       (20)     8556 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/off_policy/sac.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4068 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/off_policy/sac_lag.py
--rw-r--r--   0 jiaming    (501) staff       (20)     5071 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/off_policy/td3.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3908 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/off_policy/td3_lag.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.100782 omnisafe-0.4.0/omnisafe/algorithms/on_policy/
--rw-r--r--   0 jiaming    (501) staff       (20)     1848 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/__init__.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.101702 omnisafe-0.4.0/omnisafe/algorithms/on_policy/base/
--rw-r--r--   0 jiaming    (501) staff       (20)     1069 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/base/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)     9606 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/base/natural_pg.py
--rw-r--r--   0 jiaming    (501) staff       (20)    25220 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/base/policy_gradient.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3188 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/base/ppo.py
--rw-r--r--   0 jiaming    (501) staff       (20)     8719 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/base/trpo.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.102153 omnisafe-0.4.0/omnisafe/algorithms/on_policy/early_terminated/
--rw-r--r--   0 jiaming    (501) staff       (20)     1018 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/early_terminated/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)     2467 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/early_terminated/ppo_early_terminated.py
--rw-r--r--   0 jiaming    (501) staff       (20)     2373 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/early_terminated/trpo_early_terminated.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.102588 omnisafe-0.4.0/omnisafe/algorithms/on_policy/first_order/
--rw-r--r--   0 jiaming    (501) staff       (20)      887 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/first_order/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)     9137 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/first_order/cup.py
--rw-r--r--   0 jiaming    (501) staff       (20)     8843 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/first_order/focops.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.103370 omnisafe-0.4.0/omnisafe/algorithms/on_policy/naive_lagrange/
--rw-r--r--   0 jiaming    (501) staff       (20)     1148 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/naive_lagrange/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3068 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/naive_lagrange/crpo.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3936 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/naive_lagrange/pdo.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4057 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/naive_lagrange/ppo_lag.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4076 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/naive_lagrange/rcpo.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3973 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/naive_lagrange/trpo_lag.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.103769 omnisafe-0.4.0/omnisafe/algorithms/on_policy/penalty_function/
--rw-r--r--   0 jiaming    (501) staff       (20)      891 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/penalty_function/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)     2891 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/penalty_function/ipo.py
--rw-r--r--   0 jiaming    (501) staff       (20)     5136 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/penalty_function/p3o.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.104158 omnisafe-0.4.0/omnisafe/algorithms/on_policy/pid_lagrange/
--rw-r--r--   0 jiaming    (501) staff       (20)      907 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/pid_lagrange/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4115 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/pid_lagrange/cppo_pid.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3963 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/pid_lagrange/trpo_pid.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.104537 omnisafe-0.4.0/omnisafe/algorithms/on_policy/saute/
--rw-r--r--   0 jiaming    (501) staff       (20)      918 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/saute/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)     2927 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/saute/ppo_saute.py
--rw-r--r--   0 jiaming    (501) staff       (20)     2939 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/saute/trpo_saute.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.104951 omnisafe-0.4.0/omnisafe/algorithms/on_policy/second_order/
--rw-r--r--   0 jiaming    (501) staff       (20)      884 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/second_order/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)    19058 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/second_order/cpo.py
--rw-r--r--   0 jiaming    (501) staff       (20)     5867 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/second_order/pcpo.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.105341 omnisafe-0.4.0/omnisafe/algorithms/on_policy/simmer/
--rw-r--r--   0 jiaming    (501) staff       (20)      947 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/simmer/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3216 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/simmer/ppo_simmer_pid.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3228 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/on_policy/simmer/trpo_simmer_pid.py
--rw-r--r--   0 jiaming    (501) staff       (20)     2225 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/algorithms/registry.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.106576 omnisafe-0.4.0/omnisafe/common/
--rw-r--r--   0 jiaming    (501) staff       (20)      923 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/common/__init__.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.107466 omnisafe-0.4.0/omnisafe/common/buffer/
--rw-r--r--   0 jiaming    (501) staff       (20)     1199 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/common/buffer/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)     5226 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/common/buffer/base.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4184 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/common/buffer/offpolicy_buffer.py
--rw-r--r--   0 jiaming    (501) staff       (20)    18538 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/common/buffer/onpolicy_buffer.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4919 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/common/buffer/vector_offpolicy_buffer.py
--rw-r--r--   0 jiaming    (501) staff       (20)     5997 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/common/buffer/vector_onpolicy_buffer.py
--rw-r--r--   0 jiaming    (501) staff       (20)    26453 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/common/experiment_grid.py
--rw-r--r--   0 jiaming    (501) staff       (20)     5272 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/common/lagrange.py
--rw-r--r--   0 jiaming    (501) staff       (20)    14926 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/common/logger.py
--rw-r--r--   0 jiaming    (501) staff       (20)     5822 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/common/normalizer.py
--rw-r--r--   0 jiaming    (501) staff       (20)     5170 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/common/pid_lagrange.py
--rw-r--r--   0 jiaming    (501) staff       (20)     7026 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/common/simmer_agent.py
--rw-r--r--   0 jiaming    (501) staff       (20)    16410 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/common/statistics_tools.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.092099 omnisafe-0.4.0/omnisafe/configs/
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.108328 omnisafe-0.4.0/omnisafe/configs/model-based/
--rw-r--r--   0 jiaming    (501) staff       (20)     5127 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/configs/model-based/CAPPETS.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     4822 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/configs/model-based/CCEPETS.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     6646 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/configs/model-based/LOOP.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     4656 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/configs/model-based/PETS.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     4825 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/configs/model-based/RCEPETS.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     6757 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/configs/model-based/SafeLOOP.yaml
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.109164 omnisafe-0.4.0/omnisafe/configs/off-policy/
--rw-r--r--   0 jiaming    (501) staff       (20)     3237 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/off-policy/DDPG.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3557 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/off-policy/DDPGLag.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3438 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/off-policy/SAC.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3757 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/off-policy/SACLag.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3333 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/off-policy/TD3.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3653 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/off-policy/TD3Lag.yaml
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.112169 omnisafe-0.4.0/omnisafe/configs/on-policy/
--rw-r--r--   0 jiaming    (501) staff       (20)     4219 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/CPO.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     4347 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/CPPOPID.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3916 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/CUP.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     4086 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/FOCOPS.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3984 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/IPO.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3759 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/NaturalPG.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3611 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/OnCRPO.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3610 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/P3O.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     4219 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/PCPO.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3807 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/PDO.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3519 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/PPO.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3826 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/PPOEarlyTerminated.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3839 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/PPOLag.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3763 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/PPOSaute.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     4064 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/PPOSimmerPID.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3488 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/PolicyGradient.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     4265 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/RCPO.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     4602 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/TRPO.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3789 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/TRPOEarlyTerminated.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     4515 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/TRPOLag.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     4587 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/TRPOPID.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3969 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/TRPOSaute.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     4271 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/configs/on-policy/TRPOSimmerPID.yaml
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.112973 omnisafe-0.4.0/omnisafe/envs/
--rw-r--r--   0 jiaming    (501) staff       (20)      985 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/envs/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)    12363 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/envs/core.py
--rw-r--r--   0 jiaming    (501) staff       (20)     6122 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/envs/mujoco_env.py
--rw-r--r--   0 jiaming    (501) staff       (20)     7596 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/envs/safety_gymnasium_env.py
--rw-r--r--   0 jiaming    (501) staff       (20)    22219 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/envs/safety_gymnasium_modelbased.py
--rw-r--r--   0 jiaming    (501) staff       (20)    21885 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/envs/wrapper.py
--rw-r--r--   0 jiaming    (501) staff       (20)    20370 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/evaluator.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.113279 omnisafe-0.4.0/omnisafe/models/
--rw-r--r--   0 jiaming    (501) staff       (20)     1507 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/__init__.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.114057 omnisafe-0.4.0/omnisafe/models/actor/
--rw-r--r--   0 jiaming    (501) staff       (20)     1088 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/actor/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4165 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/actor/actor_builder.py
--rw-r--r--   0 jiaming    (501) staff       (20)     1412 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/actor/gaussian_actor.py
--rw-r--r--   0 jiaming    (501) staff       (20)     5276 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/actor/gaussian_learning_actor.py
--rw-r--r--   0 jiaming    (501) staff       (20)     6513 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/actor/gaussian_sac_actor.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4490 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/actor/mlp_actor.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.114733 omnisafe-0.4.0/omnisafe/models/actor_critic/
--rw-r--r--   0 jiaming    (501) staff       (20)     1035 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/actor_critic/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)     7170 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/actor_critic/actor_critic.py
--rw-r--r--   0 jiaming    (501) staff       (20)     6979 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/actor_critic/actor_q_critic.py
--rw-r--r--   0 jiaming    (501) staff       (20)     5182 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/actor_critic/constraint_actor_critic.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4427 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/actor_critic/constraint_actor_q_critic.py
--rw-r--r--   0 jiaming    (501) staff       (20)     8344 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/base.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.115290 omnisafe-0.4.0/omnisafe/models/critic/
--rw-r--r--   0 jiaming    (501) staff       (20)      935 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/critic/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4449 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/critic/critic_builder.py
--rw-r--r--   0 jiaming    (501) staff       (20)     5432 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/critic/q_critic.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3204 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/models/critic/v_critic.py
--rw-r--r--   0 jiaming    (501) staff       (20)     1686 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/typing.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.116719 omnisafe-0.4.0/omnisafe/utils/
--rw-r--r--   0 jiaming    (501) staff       (20)      723 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/utils/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)    16911 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/utils/command_app.py
--rw-r--r--   0 jiaming    (501) staff       (20)    15464 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/utils/config.py
--rw-r--r--   0 jiaming    (501) staff       (20)    11428 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/utils/distributed.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3249 2023-05-08 19:53:25.000000 omnisafe-0.4.0/omnisafe/utils/exp_grid_tools.py
--rw-r--r--   0 jiaming    (501) staff       (20)     7309 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/utils/math.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4027 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/utils/model.py
--rw-r--r--   0 jiaming    (501) staff       (20)    16365 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/utils/plotter.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3833 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/utils/schedule.py
--rw-r--r--   0 jiaming    (501) staff       (20)    12015 2023-05-08 19:46:32.000000 omnisafe-0.4.0/omnisafe/utils/tools.py
--rw-r--r--   0 jiaming    (501) staff       (20)     1831 2023-05-08 20:07:12.000000 omnisafe-0.4.0/omnisafe/version.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.095523 omnisafe-0.4.0/omnisafe.egg-info/
--rw-r--r--   0 jiaming    (501) staff       (20)    17209 2023-05-08 20:07:23.000000 omnisafe-0.4.0/omnisafe.egg-info/PKG-INFO
--rw-r--r--   0 jiaming    (501) staff       (20)     6816 2023-05-08 20:07:23.000000 omnisafe-0.4.0/omnisafe.egg-info/SOURCES.txt
--rw-r--r--   0 jiaming    (501) staff       (20)        1 2023-05-08 20:07:23.000000 omnisafe-0.4.0/omnisafe.egg-info/dependency_links.txt
--rw-r--r--   0 jiaming    (501) staff       (20)       60 2023-05-08 20:07:23.000000 omnisafe-0.4.0/omnisafe.egg-info/entry_points.txt
--rw-r--r--   0 jiaming    (501) staff       (20)      379 2023-05-08 20:07:23.000000 omnisafe-0.4.0/omnisafe.egg-info/requires.txt
--rw-r--r--   0 jiaming    (501) staff       (20)        9 2023-05-08 20:07:23.000000 omnisafe-0.4.0/omnisafe.egg-info/top_level.txt
--rw-r--r--   0 jiaming    (501) staff       (20)     5318 2023-05-08 19:46:32.000000 omnisafe-0.4.0/pyproject.toml
--rw-r--r--   0 jiaming    (501) staff       (20)       38 2023-05-08 20:07:23.118550 omnisafe-0.4.0/setup.cfg
--rw-r--r--   0 jiaming    (501) staff       (20)      988 2023-05-08 19:46:32.000000 omnisafe-0.4.0/setup.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-05-08 20:07:23.118090 omnisafe-0.4.0/tests/
--rw-r--r--   0 jiaming    (501) staff       (20)    15876 2023-05-08 19:46:32.000000 omnisafe-0.4.0/tests/test_buffer.py
--rw-r--r--   0 jiaming    (501) staff       (20)     2799 2023-05-08 19:46:32.000000 omnisafe-0.4.0/tests/test_cli.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4480 2023-05-08 19:53:25.000000 omnisafe-0.4.0/tests/test_env.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3325 2023-05-08 19:53:25.000000 omnisafe-0.4.0/tests/test_experiment_grid.py
--rw-r--r--   0 jiaming    (501) staff       (20)     7114 2023-05-08 19:46:32.000000 omnisafe-0.4.0/tests/test_model.py
--rw-r--r--   0 jiaming    (501) staff       (20)     1564 2023-05-08 19:46:32.000000 omnisafe-0.4.0/tests/test_normalizer.py
--rw-r--r--   0 jiaming    (501) staff       (20)    19763 2023-05-08 19:53:25.000000 omnisafe-0.4.0/tests/test_policy.py
--rw-r--r--   0 jiaming    (501) staff       (20)     1045 2023-05-08 19:46:32.000000 omnisafe-0.4.0/tests/test_registry.py
--rw-r--r--   0 jiaming    (501) staff       (20)     1478 2023-05-08 19:46:32.000000 omnisafe-0.4.0/tests/test_statistics_tools.py
--rw-r--r--   0 jiaming    (501) staff       (20)     6008 2023-05-08 19:53:25.000000 omnisafe-0.4.0/tests/test_utils.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.641961 omnisafe-0.5.0b0/
+-rw-r--r--   0 jiaming    (501) staff       (20)    11375 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/LICENSE
+-rw-r--r--   0 jiaming    (501) staff       (20)       43 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/MANIFEST.in
+-rw-r--r--   0 jiaming    (501) staff       (20)    19458 2023-06-01 18:21:46.641733 omnisafe-0.5.0b0/PKG-INFO
+-rw-r--r--   0 jiaming    (501) staff       (20)    18243 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/README.md
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.613420 omnisafe-0.5.0b0/omnisafe/
+-rw-r--r--   0 jiaming    (501) staff       (20)      992 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/__init__.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.615841 omnisafe-0.5.0b0/omnisafe/adapter/
+-rw-r--r--   0 jiaming    (501) staff       (20)     1235 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/adapter/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3395 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/adapter/early_terminated_adapter.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    15567 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/adapter/modelbased_adapter.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     5045 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/adapter/offline_adapter.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     7703 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/adapter/offpolicy_adapter.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     7691 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/adapter/online_adapter.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     6745 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/adapter/onpolicy_adapter.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     9709 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/adapter/saute_adapter.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4995 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/adapter/simmer_adapter.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.616594 omnisafe-0.5.0b0/omnisafe/algorithms/
+-rw-r--r--   0 jiaming    (501) staff       (20)     2286 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    10682 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/algo_wrapper.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     2567 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/base_algo.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.617226 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/
+-rw-r--r--   0 jiaming    (501) staff       (20)     1161 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/__init__.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.617774 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/base/
+-rw-r--r--   0 jiaming    (501) staff       (20)      887 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/base/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    35440 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/base/ensemble.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    20235 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/base/loop.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    23759 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/base/pets.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     6872 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/cap_pets.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4844 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/cce_pets.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.618636 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/planner/
+-rw-r--r--   0 jiaming    (501) staff       (20)     1247 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/planner/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    12841 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/planner/arc.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     7115 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/planner/cap.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     6158 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/planner/cce.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    11612 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/planner/cem.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4953 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/planner/rce.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    10712 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/planner/safe_arc.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4852 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/rce_pets.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     5305 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/safeloop.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.620046 omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/
+-rw-r--r--   0 jiaming    (501) staff       (20)     1314 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    23856 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/ddpg.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4108 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/ddpg_lag.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3913 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/ddpg_pid.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     8201 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/sac.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4128 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/sac_lag.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4065 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/sac_pid.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4716 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/td3.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3978 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/td3_lag.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3955 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/td3_pid.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.621507 omnisafe-0.5.0b0/omnisafe/algorithms/offline/
+-rw-r--r--   0 jiaming    (501) staff       (20)     1089 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/offline/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     5806 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/offline/base.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     8828 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/offline/bcq.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     7842 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/offline/bcq_lag.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     8291 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/offline/c_crr.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    12636 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/offline/coptidice.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     8122 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/offline/crr.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3742 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/offline/vae_bc.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.621652 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/
+-rw-r--r--   0 jiaming    (501) staff       (20)     1924 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/__init__.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.622443 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/base/
+-rw-r--r--   0 jiaming    (501) staff       (20)     1064 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/base/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     9611 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/base/natural_pg.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    25247 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/base/policy_gradient.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3210 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/base/ppo.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     9116 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/base/trpo.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.622951 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/early_terminated/
+-rw-r--r--   0 jiaming    (501) staff       (20)     1013 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/early_terminated/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     2462 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/early_terminated/ppo_early_terminated.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     2368 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/early_terminated/trpo_early_terminated.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.623450 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/first_order/
+-rw-r--r--   0 jiaming    (501) staff       (20)      882 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/first_order/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     8793 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/first_order/cup.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     8476 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/first_order/focops.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.624190 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/naive_lagrange/
+-rw-r--r--   0 jiaming    (501) staff       (20)     1060 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/naive_lagrange/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3974 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/naive_lagrange/pdo.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4043 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/naive_lagrange/ppo_lag.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4114 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/naive_lagrange/rcpo.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3958 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/naive_lagrange/trpo_lag.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.624661 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/penalty_function/
+-rw-r--r--   0 jiaming    (501) staff       (20)      886 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/penalty_function/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     2875 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/penalty_function/ipo.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     5162 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/penalty_function/p3o.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.625093 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/pid_lagrange/
+-rw-r--r--   0 jiaming    (501) staff       (20)      902 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/pid_lagrange/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4110 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/pid_lagrange/cppo_pid.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3958 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/pid_lagrange/trpo_pid.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.625394 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/primal/
+-rw-r--r--   0 jiaming    (501) staff       (20)      797 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/primal/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3040 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/primal/crpo.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.625800 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/saute/
+-rw-r--r--   0 jiaming    (501) staff       (20)      913 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/saute/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     2922 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/saute/ppo_saute.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     2934 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/saute/trpo_saute.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.626186 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/second_order/
+-rw-r--r--   0 jiaming    (501) staff       (20)      879 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/second_order/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    19058 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/second_order/cpo.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     5867 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/second_order/pcpo.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.626550 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/simmer/
+-rw-r--r--   0 jiaming    (501) staff       (20)      942 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/simmer/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3211 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/simmer/ppo_simmer_pid.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3223 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/simmer/trpo_simmer_pid.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     2220 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/registry.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.627572 omnisafe-0.5.0b0/omnisafe/common/
+-rw-r--r--   0 jiaming    (501) staff       (20)      918 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/__init__.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.628353 omnisafe-0.5.0b0/omnisafe/common/buffer/
+-rw-r--r--   0 jiaming    (501) staff       (20)     1194 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/buffer/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     5221 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/buffer/base.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4184 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/buffer/offpolicy_buffer.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    18534 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/buffer/onpolicy_buffer.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4914 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/buffer/vector_offpolicy_buffer.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     5346 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/buffer/vector_onpolicy_buffer.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    26545 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/experiment_grid.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     5266 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/lagrange.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    14965 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/logger.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     5837 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/normalizer.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.628737 omnisafe-0.5.0b0/omnisafe/common/offline/
+-rw-r--r--   0 jiaming    (501) staff       (20)      893 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/offline/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     8201 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/offline/data_collector.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    18021 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/offline/dataset.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     5165 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/pid_lagrange.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     7026 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/simmer_agent.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    16468 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/statistics_tools.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.611028 omnisafe-0.5.0b0/omnisafe/configs/
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.629517 omnisafe-0.5.0b0/omnisafe/configs/model-based/
+-rw-r--r--   0 jiaming    (501) staff       (20)     5127 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/model-based/CAPPETS.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     4822 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/model-based/CCEPETS.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     6646 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/model-based/LOOP.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     4656 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/model-based/PETS.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     4825 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/model-based/RCEPETS.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     6757 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/model-based/SafeLOOP.yaml
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.630812 omnisafe-0.5.0b0/omnisafe/configs/off-policy/
+-rw-r--r--   0 jiaming    (501) staff       (20)     4361 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/off-policy/DDPG.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     6025 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/off-policy/DDPGLag.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     6434 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/off-policy/DDPGPID.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     4905 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/off-policy/SAC.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     6757 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/off-policy/SACLag.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     6810 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/off-policy/SACPID.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     4457 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/off-policy/TD3.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     6477 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/off-policy/TD3Lag.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     6530 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/off-policy/TD3PID.yaml
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.631587 omnisafe-0.5.0b0/omnisafe/configs/offline/
+-rw-r--r--   0 jiaming    (501) staff       (20)     2760 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/offline/BCQ.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3201 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/offline/BCQLag.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3141 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/offline/CCRR.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3371 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/offline/COptiDICE.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     2754 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/offline/CRR.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     2142 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/offline/VAEBC.yaml
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.634587 omnisafe-0.5.0b0/omnisafe/configs/on-policy/
+-rw-r--r--   0 jiaming    (501) staff       (20)     3787 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/CPO.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     4349 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/CPPOPID.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3918 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/CUP.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     4088 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/FOCOPS.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3986 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/IPO.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3761 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/NaturalPG.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3613 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/OnCRPO.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3612 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/P3O.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3787 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/PCPO.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3809 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/PDO.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3521 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/PPO.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3582 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/PPOEarlyTerminated.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3841 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/PPOLag.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3762 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/PPOSaute.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     4063 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/PPOSimmerPID.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3490 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/PolicyGradient.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     4050 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/RCPO.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3730 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/TRPO.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3791 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/TRPOEarlyTerminated.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     4050 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/TRPOLag.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     4589 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/TRPOPID.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     3971 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/TRPOSaute.yaml
+-rw-r--r--   0 jiaming    (501) staff       (20)     4272 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/TRPOSimmerPID.yaml
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.635342 omnisafe-0.5.0b0/omnisafe/envs/
+-rw-r--r--   0 jiaming    (501) staff       (20)      980 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/envs/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    12724 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/envs/core.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     6402 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/envs/mujoco_env.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     8218 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/envs/safety_gymnasium_env.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    20570 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/envs/safety_gymnasium_modelbased.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    22475 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/envs/wrapper.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    22578 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/evaluator.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.635614 omnisafe-0.5.0b0/omnisafe/models/
+-rw-r--r--   0 jiaming    (501) staff       (20)     1731 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/__init__.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.636546 omnisafe-0.5.0b0/omnisafe/models/actor/
+-rw-r--r--   0 jiaming    (501) staff       (20)     1207 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/actor/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4928 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/actor/actor_builder.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     1407 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/actor/gaussian_actor.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     5292 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/actor/gaussian_learning_actor.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     6527 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/actor/gaussian_sac_actor.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4531 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/actor/mlp_actor.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4122 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/actor/perturbation_actor.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     5516 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/actor/vae_actor.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.637119 omnisafe-0.5.0b0/omnisafe/models/actor_critic/
+-rw-r--r--   0 jiaming    (501) staff       (20)     1030 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/actor_critic/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     7299 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/actor_critic/actor_critic.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     7107 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/actor_critic/actor_q_critic.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     5177 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/actor_critic/constraint_actor_critic.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4427 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/actor_critic/constraint_actor_q_critic.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     8341 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/base.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.637672 omnisafe-0.5.0b0/omnisafe/models/critic/
+-rw-r--r--   0 jiaming    (501) staff       (20)      930 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/critic/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4463 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/critic/critic_builder.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     5443 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/critic/q_critic.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3217 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/critic/v_critic.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.637942 omnisafe-0.5.0b0/omnisafe/models/offline/
+-rw-r--r--   0 jiaming    (501) staff       (20)      776 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/offline/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3265 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/offline/dice.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     1709 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/typing.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.639521 omnisafe-0.5.0b0/omnisafe/utils/
+-rw-r--r--   0 jiaming    (501) staff       (20)      718 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/utils/__init__.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    17241 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/utils/command_app.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    15410 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/utils/config.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    11396 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/utils/distributed.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3305 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/utils/exp_grid_tools.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     7276 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/utils/math.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4022 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/utils/model.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    16404 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/utils/plotter.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3828 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/utils/schedule.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    12016 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/utils/tools.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     1833 2023-06-01 18:21:33.000000 omnisafe-0.5.0b0/omnisafe/version.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.614242 omnisafe-0.5.0b0/omnisafe.egg-info/
+-rw-r--r--   0 jiaming    (501) staff       (20)    19458 2023-06-01 18:21:46.000000 omnisafe-0.5.0b0/omnisafe.egg-info/PKG-INFO
+-rw-r--r--   0 jiaming    (501) staff       (20)     7968 2023-06-01 18:21:46.000000 omnisafe-0.5.0b0/omnisafe.egg-info/SOURCES.txt
+-rw-r--r--   0 jiaming    (501) staff       (20)        1 2023-06-01 18:21:46.000000 omnisafe-0.5.0b0/omnisafe.egg-info/dependency_links.txt
+-rw-r--r--   0 jiaming    (501) staff       (20)       60 2023-06-01 18:21:46.000000 omnisafe-0.5.0b0/omnisafe.egg-info/entry_points.txt
+-rw-r--r--   0 jiaming    (501) staff       (20)      392 2023-06-01 18:21:46.000000 omnisafe-0.5.0b0/omnisafe.egg-info/requires.txt
+-rw-r--r--   0 jiaming    (501) staff       (20)        9 2023-06-01 18:21:46.000000 omnisafe-0.5.0b0/omnisafe.egg-info/top_level.txt
+-rw-r--r--   0 jiaming    (501) staff       (20)     5348 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/pyproject.toml
+-rw-r--r--   0 jiaming    (501) staff       (20)       38 2023-06-01 18:21:46.642014 omnisafe-0.5.0b0/setup.cfg
+-rw-r--r--   0 jiaming    (501) staff       (20)      988 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/setup.py
+drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.641420 omnisafe-0.5.0b0/tests/
+-rw-r--r--   0 jiaming    (501) staff       (20)    15872 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/tests/test_buffer.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3294 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/tests/test_cli.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     2552 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/tests/test_ensemble.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4476 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/tests/test_env.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     3735 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/tests/test_experiment_grid.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     7110 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/tests/test_model.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     1560 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/tests/test_normalizer.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     4951 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/tests/test_offline_data.py
+-rw-r--r--   0 jiaming    (501) staff       (20)    16357 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/tests/test_policy.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     1045 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/tests/test_registry.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     1594 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/tests/test_statistics_tools.py
+-rw-r--r--   0 jiaming    (501) staff       (20)     7140 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/tests/test_utils.py
```

### Comparing `omnisafe-0.4.0/LICENSE` & `omnisafe-0.5.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `omnisafe-0.4.0/PKG-INFO` & `omnisafe-0.5.0b0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,223 +1,262 @@
-Metadata-Version: 2.1
-Name: omnisafe
-Version: 0.4.0
-Summary: A comprehensive and reliable benchmark for safe reinforcement learning.
-Author: OmniSafe Contributors
-License: Apache License, Version 2.0
-Project-URL: Homepage, https://github.com/OmniSafeAI/omnisafe
-Project-URL: Repository, https://github.com/OmniSafeAI/omnisafe
-Project-URL: Documentation, https://omnisafe.readthedocs.io
-Project-URL: Bug Report, https://github.com/OmniSafeAI/omnisafe/issues
-Keywords: Safe Reinforcement Learning,Reinforcement Learning,PyTorch
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: lint
-Provides-Extra: test
-License-File: LICENSE
-
 <!-- markdownlint-disable first-line-h1 -->
 <!-- markdownlint-disable html -->
 
 <div align="center">
-  <img src="https://github.com/OmniSafeAI/omnisafe/raw/HEAD/images/logo.png" width="75%"/>
+  <img src="https://github.com/PKU-Alignment/omnisafe/raw/HEAD/images/logo.png" width="75%"/>
 </div>
 
 <div align="center">
 
-  [![Organization](https://img.shields.io/badge/Organization-PKU_MARL-blue.svg)](https://github.com/OmniSafeAI)
+  [![Organization](https://img.shields.io/badge/Organization-PKU--Alignment-blue)](https://github.com/PKU-Alignment)
   [![PyPI](https://img.shields.io/pypi/v/omnisafe?logo=pypi)](https://pypi.org/project/omnisafe)
-  [![tests](https://img.shields.io/github/actions/workflow/status/OmniSafeAI/omnisafe/test.yml?label=tests&logo=github)](https://github.com/OmniSafeAI/omnisafe/tree/HEAD/tests)
+  [![tests](https://img.shields.io/github/actions/workflow/status/PKU-Alignment/omnisafe/test.yml?label=tests&logo=github)](https://github.com/PKU-Alignment/omnisafe/tree/HEAD/tests)
   [![Documentation Status](https://img.shields.io/readthedocs/omnisafe?logo=readthedocs)](https://omnisafe.readthedocs.io)
   [![Downloads](https://static.pepy.tech/personalized-badge/omnisafe?period=total&left_color=grey&right_color=blue&left_text=downloads)](https://pepy.tech/project/omnisafe)
-  [![GitHub Repo Stars](https://img.shields.io/github/stars/OmniSafeAI/omnisafe?color=brightgreen&logo=github)](https://github.com/OmniSafeAI/OmniSafe/stargazers)
+  [![GitHub Repo Stars](https://img.shields.io/github/stars/PKU-Alignment/omnisafe?color=brightgreen&logo=github)](https://github.com/PKU-Alignment/OmniSafe/stargazers)
   [![codestyle](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-  [![License](https://img.shields.io/github/license/OmniSafeAI/OmniSafe?label=license)](#license)
-  [![CodeCov](https://img.shields.io/codecov/c/github/OmniSafeAI/omnisafe/main?logo=codecov)](https://app.codecov.io/gh/OmniSafeAI/omnisafe)
-  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/OmniSafeAI/omnisafe/)
+  [![License](https://img.shields.io/github/license/PKU-Alignment/OmniSafe?label=license)](#license)
+  [![CodeCov](https://img.shields.io/codecov/c/github/PKU-Alignment/omnisafe/main?logo=codecov)](https://app.codecov.io/gh/PKU-Alignment/omnisafe)
+  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/PKU-Alignment/omnisafe/)
 
 </div>
 
 <p align="center">
   <a href="https://omnisafe.readthedocs.io">Documentation</a> |
-  <a href="https://github.com/OmniSafeAI/omnisafe#implemented-algorithms">Implemented Algorithms</a> |
-  <a href="https://github.com/OmniSafeAI/omnisafe#installation">Installation</a> |
-  <a href="https://github.com/OmniSafeAI/omnisafe#getting-started">Getting Started</a> |
-  <a href="https://github.com/OmniSafeAI/omnisafe#license">License</a>
+  <a href="https://github.com/PKU-Alignment/omnisafe#implemented-algorithms">Implemented Algorithms</a> |
+  <a href="https://github.com/PKU-Alignment/omnisafe#installation">Installation</a> |
+  <a href="https://github.com/PKU-Alignment/omnisafe#getting-started">Getting Started</a> |
+  <a href="https://github.com/PKU-Alignment/omnisafe#license">License</a>
 </p>
 
 --------------------------------------------------------------------------------
 
-**This library is currently under heavy development - if you have suggestions on the API or use-cases you'd like to be covered, please open a GitHub issue or reach out. We'd love to hear about how you're using the library.**
+OmniSafe is an infrastructural framework designed to accelerate safe reinforcement learning (RL) research.
+It provides a comprehensive and reliable benchmark for safe RL algorithms, and also an out-of-box modular toolkit for researchers.
+SafeRL intends to develop algorithms that minimize the risk of unintended harm or unsafe behavior.
+
+OmniSafe stands as the inaugural unified learning framework in the realm of safe reinforcement learning, aiming to foster the Growth of SafeRL Learning Community.
+The key features of OmniSafe:
+
+- **Highly Modular Framework.** OmniSafe presents a highly modular framework, incorporating an extensive collection of tens of algorithms tailored for safe reinforcement learning across diverse domains. This framework is versatile due to its abstraction of various algorithm types and well-designed API, using the Adapter and Wrapper design components to bridge gaps and enable seamless interactions between different components. This design allows for easy extension and customization, making it a powerful tool for developers working with different types of algorithms.
+
+- **High-performance parallel computing acceleration.** By harnessing the capabilities of `torch.distributed`, OmniSafe accelerates the learning process of algorithms
+with process parallelism. This enables OmniSafe not only to support environment-level asynchronous parallelism but also incorporates agent asynchronous learning. This methodology bolsters training stability and expedites the training process via the deployment of a parallel exploration mechanism. The integration of agent asynchronous learning in OmniSafe underscores its commitment to providing a versatile and robust platform for advancing SafeRL research.
 
-OmniSafe is an infrastructural framework designed to accelerate safe reinforcement learning (RL) research by providing a comprehensive and reliable benchmark for safe RL algorithms.
-The field of RL has great potential to benefit the society, and safety concerns are a significant issue, and RL algorithms have raised concerns about unintended harm or unsafe behavior.
-Safe RL intends to develop algorithms that minimize the risk of unintended harm or unsafe behavior, but there is currently a lack of commonly recognized safe RL algorithm benchmarks.
-
-OmniSafe addresses these issues by providing more than 40 experimentally validated algorithms and a sound and efficient simulation environment.
-Researchers can use OmniSafe to conduct experiments and verify their ideas, ensuring consistency and enabling more efficient development of safe RL algorithms.
-By using OmniSafe as a benchmark, researchers can evaluate the performance of their own safe RL algorithms and contribute to the advancement of safe RL research.
+- **Out-of-box toolkits.** OmniSafe offers customizable toolkits for tasks like training, benchmarking, analyzing, and rendering. [Tutorials](https://github.com/PKU-Alignment/omnisafe#getting-started) and user-friendly [APIs](https://omnisafe.readthedocs.io/en/latest/baserlapi/on_policy.html) make it easy for beginners and average users, while advanced researchers can enhance their efficiency without complex code.
+
+![Train video](https://github-production-user-asset-6210df.s3.amazonaws.com/73586554/237139607-d1e6f413-aa2c-4f68-b8ee-08a4361493a0.gif)
 
 --------------------------------------------------------------------------------
 
 ### Table of Contents  <!-- omit in toc --> <!-- markdownlint-disable heading-increment -->
 
-- [Implemented Algorithms](#implemented-algorithms)
-  - [Latest SafeRL Papers](#latest-saferl-papers)
-  - [List of Algorithms](#list-of-algorithms)
-    - [On-Policy Safe](#on-policy-safe)
-    - [Off-Policy Safe](#off-policy-safe)
-    - [Model-Based Safe](#model-based-safe)
-    - [Offline Safe](#offline-safe)
-    - [Others](#others)
-- [Installation](#installation)
-  - [Prerequisites](#prerequisites)
+- [Quick Start](#quick-start)
+  - [Installation](#installation)
+    - [Prerequisites](#prerequisites)
     - [Install from source](#install-from-source)
     - [Install from PyPI](#install-from-pypi)
+- [Implemented Algorithms](#implemented-algorithms)
   - [Examples](#examples)
+    - [Algorithms Registry](#algorithms-registry)
+    - [Supported Environments](#supported-environments)
     - [Try with CLI](#try-with-cli)
 - [Getting Started](#getting-started)
   - [Important Hints](#important-hints)
   - [Quickstart: Colab on the Cloud](#quickstart-colab-on-the-cloud)
 - [Changelog](#changelog)
+- [Citing OmniSafe](#citing-omnisafe)
 - [The OmniSafe Team](#the-omnisafe-team)
 - [License](#license)
 
 --------------------------------------------------------------------------------
 
-## Implemented Algorithms
+## Quick Start
+
+### Installation
+
+#### Prerequisites
+
+OmniSafe requires Python 3.8+ and PyTorch 1.10+.
+
+> We support and test for Python 3.8, 3.9, 3.10 on Linux. Meanwhile, we also support M1 and M2 versions of macOS. We will accept PRs related to Windows, but do not officially support it.
+
+#### Install from source
+
+```bash
+# Clone the repo
+git clone https://github.com/PKU-Alignment/omnisafe.git
+cd omnisafe
+
+# Create a conda environment
+conda env create --file conda-recipe.yaml
+conda activate omnisafe
+
+# Install omnisafe
+pip install -e .
+```
 
-The supported interface algorithms currently include:
+#### Install from PyPI
+
+OmniSafe is hosted in [![PyPI](https://img.shields.io/pypi/v/omnisafe?label=pypi&logo=pypi)](https://pypi.org/project/omnisafe) / ![Status](https://img.shields.io/pypi/status/omnisafe?label=status).
+
+```bash
+pip install omnisafe
+```
 
-### Latest SafeRL Papers
+## Implemented Algorithms
+
+<details>
+<summary><b><big>Latest SafeRL Papers</big></b></summary>
 
 - **[AAAI 2023]** Augmented Proximal Policy Optimization for Safe Reinforcement Learning (APPO)
 - **[NeurIPS 2022]** [Constrained Update Projection Approach to Safe Policy Optimization (CUP)](https://arxiv.org/abs/2209.07089)
 - **[NeurIPS 2022]** [Effects of Safety State Augmentation on Safe Exploration (Simmer)](https://arxiv.org/abs/2206.02675)
 - **[NeurIPS 2022]** [Model-based Safe Deep Reinforcement Learning via a Constrained Proximal Policy Optimization Algorithm](https://arxiv.org/abs/2210.07573)
 - **[ICML 2022]** [Sauté RL: Almost Surely Safe Reinforcement Learning Using State Augmentation (SauteRL)](https://arxiv.org/abs/2202.06558)
-- **[ICML 2022]** [Constrained Variational Policy Optimization for Safe Reinforcement Learning (CVPO)](https://arxiv.org/abs/2201.11927)
 - **[IJCAI 2022]** [Penalized Proximal Policy Optimization for Safe Reinforcement Learning](https://arxiv.org/abs/2205.11814)
-- **[ICLR 2022]** [Constrained Policy Optimization via Bayesian World Models (LA-MBDA)](https://arxiv.org/abs/2201.09802)
 - **[AAAI 2022]** [Conservative and Adaptive Penalty for Model-Based Safe Reinforcement Learning (CAP)](https://arxiv.org/abs/2112.07701)
 
-### List of Algorithms
+</details>
 
-#### On-Policy Safe
+<details>
+<summary><b><big>List of Algorithms</big></b></summary>
 
-- [X] [The Lagrange version of PPO (PPO-Lag)](https://cdn.openai.com/safexp-short.pdf)
-- [X] [The Lagrange version of TRPO (TRPO-Lag)](https://cdn.openai.com/safexp-short.pdf)
-- [X] **[ICML 2017]** [Constrained Policy Optimization (CPO)](https://proceedings.mlr.press/v70/achiam17a)
-- [X] **[ICLR 2019]** [Reward Constrained Policy Optimization (RCPO)](https://openreview.net/forum?id=SkfrvsA9FX)
-- [X] **[ICML 2020]** [Responsive Safety in Reinforcement Learning by PID Lagrangian Methods (PID-Lag)](https://arxiv.org/abs/2007.03964)
-- [X] **[NeurIPS 2020]** [First Order Constrained Optimization in Policy Space (FOCOPS)](https://arxiv.org/abs/2002.06506)
-- [X] **[AAAI 2020]** [IPO: Interior-point Policy Optimization under Constraints (IPO)](https://arxiv.org/abs/1910.09615)
-- [X] **[ICLR 2020]** [Projection-Based Constrained Policy Optimization (PCPO)](https://openreview.net/forum?id=rke3TJrtPS)
-- [X] **[ICML 2021]** [CRPO: A New Approach for Safe Reinforcement Learning with Convergence Guarantee](https://arxiv.org/abs/2011.05869)
+<summary><b><big>On Policy SafeRL</big></b></summary>
+
+- [x] [The Lagrange version of PPO (PPO-Lag)](https://cdn.openai.com/safexp-short.pdf)
+- [x] [The Lagrange version of TRPO (TRPO-Lag)](https://cdn.openai.com/safexp-short.pdf)
+- [x] **[ICML 2017]** [Constrained Policy Optimization (CPO)](https://proceedings.mlr.press/v70/achiam17a)
+- [x] **[ICLR 2019]** [Reward Constrained Policy Optimization (RCPO)](https://openreview.net/forum?id=SkfrvsA9FX)
+- [x] **[ICML 2020]** [Responsive Safety in Reinforcement Learning by PID Lagrangian Methods (PID-Lag)](https://arxiv.org/abs/2007.03964)
+- [x] **[NeurIPS 2020]** [First Order Constrained Optimization in Policy Space (FOCOPS)](https://arxiv.org/abs/2002.06506)
+- [x] **[AAAI 2020]** [IPO: Interior-point Policy Optimization under Constraints (IPO)](https://arxiv.org/abs/1910.09615)
+- [x] **[ICLR 2020]** [Projection-Based Constrained Policy Optimization (PCPO)](https://openreview.net/forum?id=rke3TJrtPS)
+- [x] **[ICML 2021]** [CRPO: A New Approach for Safe Reinforcement Learning with Convergence Guarantee](https://arxiv.org/abs/2011.05869)
 - [x] **[IJCAI 2022]** [Penalized Proximal Policy Optimization for Safe Reinforcement Learning(P3O)](https://arxiv.org/pdf/2205.11814.pdf)
 
-#### Off-Policy Safe
+<summary><b><big>Off Policy SafeRL</big></b></summary>
 
-- [X] The Lagrange version of TD3 (TD3-Lag)
-- [X] The Lagrange version of DDPG (DDPG-Lag)
-- [X] The Lagrange version of SAC (SAC-Lag)
-- [X] **[ICML 2019]** [Lyapunov-based Safe Policy Optimization for Continuous Control (SDDPG)](https://arxiv.org/abs/1901.10031)
-- [X] **[ICML 2019]** [Lyapunov-based Safe Policy Optimization for Continuous Control (SDDPG-modular)](https://arxiv.org/abs/1901.10031)
-- [ ] **[ICML 2022]** [Constrained Variational Policy Optimization for Safe Reinforcement Learning (CVPO)](https://arxiv.org/abs/2201.11927)
+- **[Preprint 2019]** [The Lagrangian version of DDPG (DDPGLag)](https://cdn.openai.com/safexp-short.pdf)
+- **[Preprint 2019]** [The Lagrangian version of TD3 (TD3Lag)](https://cdn.openai.com/safexp-short.pdf)
+- **[Preprint 2019]** [The Lagrangian version of SAC (SACLag)](https://cdn.openai.com/safexp-short.pdf)
+- **[ICML 2020]** [Responsive Safety in Reinforcement Learning by PID Lagrangian Methods (DDPGPID)](https://arxiv.org/abs/2007.03964)
+- **[ICML 2020]** [Responsive Safety in Reinforcement Learning by PID Lagrangian Methods (TD3PID)](https://arxiv.org/abs/2007.03964)
+- **[ICML 2020]** [Responsive Safety in Reinforcement Learning by PID Lagrangian Methods (SACPID)](https://arxiv.org/abs/2007.03964)
 
-#### Model-Based Safe
+<summary><b><big>Model-Based SafeRL</big></b></summary>
 
 - [ ] **[NeurIPS 2021]** [Safe Reinforcement Learning by Imagining the Near Future (SMBPO)](https://arxiv.org/abs/2202.07789)
-- [X] **[CoRL 2021 (Oral)]** [Learning Off-Policy with Online Planning (SafeLOOP)](https://arxiv.org/abs/2008.10066)
-- [X] **[AAAI 2022]** [Conservative and Adaptive Penalty for Model-Based Safe Reinforcement Learning (CAP)](https://arxiv.org/abs/2112.07701)
-- [X] **[NeurIPS 2022]** [Model-based Safe Deep Reinforcement Learning via a Constrained Proximal Policy Optimization Algorithm](https://arxiv.org/abs/2210.07573)
+- [x] **[CoRL 2021 (Oral)]** [Learning Off-Policy with Online Planning (SafeLOOP)](https://arxiv.org/abs/2008.10066)
+- [x] **[AAAI 2022]** [Conservative and Adaptive Penalty for Model-Based Safe Reinforcement Learning (CAP)](https://arxiv.org/abs/2112.07701)
+- [x] **[NeurIPS 2022]** [Model-based Safe Deep Reinforcement Learning via a Constrained Proximal Policy Optimization Algorithm](https://arxiv.org/abs/2210.07573)
 - [ ] **[ICLR 2022]** [Constrained Policy Optimization via Bayesian World Models (LA-MBDA)](https://arxiv.org/abs/2201.09802)
-- [X] **[ICML 2022 Workshop]** [Constrained Model-based Reinforcement Learning with Robust Cross-Entropy Method (RCE)](https://arxiv.org/abs/2010.07968)
-- [X] **[NeurIPS 2018]** [Constrained Cross-Entropy Method for Safe Reinforcement Learning (CCE)](https://proceedings.neurips.cc/paper/2018/hash/34ffeb359a192eb8174b6854643cc046-Abstract.html)
+- [x] **[ICML 2022 Workshop]** [Constrained Model-based Reinforcement Learning with Robust Cross-Entropy Method (RCE)](https://arxiv.org/abs/2010.07968)
+- [x] **[NeurIPS 2018]** [Constrained Cross-Entropy Method for Safe Reinforcement Learning (CCE)](https://proceedings.neurips.cc/paper/2018/hash/34ffeb359a192eb8174b6854643cc046-Abstract.html)
 
-#### Offline Safe
+<summary><b><big>Offline SafeRL</big></b></summary>
 
-- [X] [The Lagrange version of BCQ (BCQ-Lag)](https://arxiv.org/abs/1812.02900)
-- [X] [The Constrained version of CRR (C-CRR)](https://proceedings.neurips.cc/paper/2020/hash/588cb956d6bbe67078f29f8de420a13d-Abstract.html)
+- [x] [The Lagrange version of BCQ (BCQ-Lag)](https://arxiv.org/abs/1812.02900)
+- [x] [The Constrained version of CRR (C-CRR)](https://proceedings.neurips.cc/paper/2020/hash/588cb956d6bbe67078f29f8de420a13d-Abstract.html)
 - [ ] **[AAAI 2022]** [Constraints Penalized Q-learning for Safe Offline Reinforcement Learning CPQ](https://arxiv.org/abs/2107.09003)
-- [ ] **[ICLR 2022 (Spotlight)]** [COptiDICE: Offline Constrained Reinforcement Learning via Stationary Distribution Correction Estimation](https://arxiv.org/abs/2204.08957?context=cs.AI)
+- [x] **[ICLR 2022 (Spotlight)]** [COptiDICE: Offline Constrained Reinforcement Learning via Stationary Distribution Correction Estimation](https://arxiv.org/abs/2204.08957?context=cs.AI)
 - [ ] **[ICML 2022]** [Constrained Offline Policy Optimization (COPO)](https://proceedings.mlr.press/v162/polosky22a.html)
 
-#### Others
+<summary><b><big>Others</big></b></summary>
 
-- [X] [Safe Exploration in Continuous Action Spaces (Safety Layer)](https://arxiv.org/abs/1801.08757)
 - [ ] **[RA-L 2021]** [Recovery RL: Safe Reinforcement Learning with Learned Recovery Zones](https://arxiv.org/abs/2010.15920)
-- [X] **[ICML 2022]** [Sauté RL: Almost Surely Safe Reinforcement Learning Using State Augmentation (SauteRL)](https://arxiv.org/abs/2202.06558)
-- [X] **[NeurIPS 2022]** [Effects of Safety State Augmentation on Safe Exploration](https://arxiv.org/abs/2206.02675)
-
---------------------------------------------------------------------------------
-
-## Installation
-
-### Prerequisites
-
-OmniSafe requires Python 3.8+ and PyTorch 1.10+.
-
-> We support and test for Python 3.8, 3.9, 3.10 on Linux. Meanwhile, we also support M1 and M2 versions of macOS. We will accept PRs related to Windows, but do not officially support it.
-
-#### Install from source
-
-```bash
-# Clone the repo
-git clone https://github.com/OmniSafeAI/omnisafe
-cd omnisafe
-
-# Create a conda environment
-conda env create --file conda-recipe.yaml
-conda activate omnisafe
+- [x] **[ICML 2022]** [Sauté RL: Almost Surely Safe Reinforcement Learning Using State Augmentation (SauteRL)](https://arxiv.org/abs/2202.06558)
+- [x] **[NeurIPS 2022]** [Effects of Safety State Augmentation on Safe Exploration](https://arxiv.org/abs/2206.02675)
 
-# Install omnisafe
-pip install -e .
-```
-
-#### Install from PyPI
-
-OmniSafe is hosted in [![PyPI](https://img.shields.io/pypi/v/omnisafe?label=pypi&logo=pypi)](https://pypi.org/project/omnisafe) / ![Status](https://img.shields.io/pypi/status/omnisafe?label=status).
+</details>
 
-```bash
-pip install omnisafe
-```
+--------------------------------------------------------------------------------
 
 ### Examples
 
 ```bash
 cd examples
-python train_policy.py --algo PPOLag --env-id SafetyPointGoal1-v0 --parallel 1 --total-steps 1024000 --device cpu --vector-env-nums 1 --torch-threads 1
+python train_policy.py --algo PPOLag --env-id SafetyPointGoal1-v0 --parallel 1 --total-steps 10000000 --device cpu --vector-env-nums 1 --torch-threads 1
 ```
 
-**algo:**
-| Type              | Name                                                             |
-| ----------------- | ---------------------------------------------------------------- |
-| `Base-On-Policy`  | `PolicyGradient, PPO`<br> `NaturalPG, TRPO`                      |
-| `Base-Off-Policy` | `DDPG, TD3, SAC`                                                 |
-| `Naive Lagrange`  | `RCPO, PPOLag, TRPOLag`<br> `DDPGLag, TD3Lag, SACLag`            |
-| `PID Lagrange`    | `CPPOPid, TRPOPid`                                               |
-| `First Order`     | `FOCOPS, CUP`                                                    |
-| `Second Order`    | `SDDPG, CPO, PCPO`                                               |
-| `Saute RL`        | `PPOSaute, PPOLagSaute`                                          |
-| `Simmer RL`       | `PPOSimmerQ, PPOSimmerPid` <br> `PPOLagSimmerQ, PPOLagSimmerPid` |
-| `EarlyTerminated` | `PPOEarlyTerminated` <br> `PPOLagEarlyTerminated`                |
-| `Model-Based`     | `CAP, MBPPOLag, SafeLOOP`                                        |
+#### Algorithms Registry
+
+<table>
+<thead>
+  <tr>
+    <th>Domains</th>
+    <th>Types</th>
+    <th>Algorithms Registry</th>
+  </tr>
+</thead>
+<tbody>
+  <tr>
+    <td rowspan="5">On Policy</td>
+    <td rowspan="2">Primal Dual</td>
+    <td>TRPOLag; PPOLag; PDO; RCPO</td>
+  </tr>
+  <tr>
+    <td>TRPOPID; CPPOPID</td>
+  </tr>
+  <tr>
+    <td>Convex Optimization</td>
+    <td><span style="font-weight:400;font-style:normal">CPO; PCPO; </span>FOCOPS; CUP</td>
+  </tr>
+  <tr>
+    <td>Penalty Function</td>
+    <td>IPO; P3O</td>
+  </tr>
+  <tr>
+    <td>Primal</td>
+    <td>OnCRPO</td>
+  </tr>
+  <tr>
+    <td rowspan="2">Off Policy</td>
+    <td rowspan="2">Primal-Dual</td>
+    <td>DDPGLag; TD3Lag; SACLag</td>
+  </tr>
+  <tr>
+    <td><span style="font-weight:400;font-style:normal">DDPGPID; TD3PID; SACPID</span></td>
+  </tr>
+  <tr>
+    <td rowspan="2">Model-based</td>
+    <td>Online Plan</td>
+    <td>SafeLOOP; CCEPETS; RCEPETS</td>
+  </tr>
+  <tr>
+    <td><span style="font-weight:400;font-style:normal">Pessimistic Estimate</span></td>
+    <td>CAPPETS</td>
+  </tr>
+    <td rowspan="2">Offline</td>
+    <td>Q-Learning Based</td>
+    <td>BCQLag; C-CRR</td>
+  </tr>
+  <tr>
+    <td>DICE Based</td>
+    <td>COptDICE</td>
+  </tr>
+  <tr>
+    <td rowspan="3">Other Formulation MDP</td>
+    <td>ET-MDP</td>
+    <td><span style="font-weight:400;font-style:normal">PPO</span>EarlyTerminated; TRPOEarlyTerminated</td>
+  </tr>
+  <tr>
+    <td>SauteRL</td>
+    <td>PPOSaute; TRPOSaute</td>
+  </tr>
+  <tr>
+    <td>SimmerRL</td>
+    <td><span style="font-weight:400;font-style:normal">PPOSimmerPID; TRPOSimmerPID</span></td>
+  </tr>
+</tbody>
+</table>
+
+#### Supported Environments
 
-**env-id:** Environment id in [Safety Gymnasium](https://www.safety-gymnasium.com/), here a list of envs that safety-gymnasium supports.
+Here is a list of environments that [Safety-Gymnasium](https://www.safety-gymnasium.com) supports:
 
 <table border="1">
 <thead>
   <tr>
     <th>Category</th>
     <th>Task</th>
     <th>Agent</th>
@@ -245,72 +284,91 @@
     <td>Velocity</td>
     <td>HalfCheetah, Hopper, Swimmer, Walker2d, Ant, Humanoid</td>
     <td>SafetyHumanoidVelocity-v1</td>
   </tr>
 </tbody>
 </table>
 
-More information about environments, please refer to [Safety Gymnasium](https://www.safety-gymnasium.com/)
-
-**parallel:** `Number of parallels`
+For more information about environments, please refer to [Safety-Gymnasium](https://www.safety-gymnasium.com).
 
 #### Try with CLI
 
-**A video example**
-
-![Segmentfault](https://github.com/OmniSafeAI/omnisafe/blob/main/images/CLI_example.svg)
-
 ```bash
 pip install omnisafe
 
-omnisafe --help # Ask for help
-
-omnisafe benchmark --help # The benchmark also can be replaced with 'eval', 'train', 'train-config'
+omnisafe --help  # Ask for help
 
-# Quick benchmarking for your research, just specify: 1.exp_name, 2.num_pool(how much processes are concurrent), 3.path of the config file(refer to omnisafe/examples/benchmarks for format)
-omnisafe benchmark test_benchmark 2 ./saved_source/benchmark_config.yaml
+omnisafe benchmark --help  # The benchmark also can be replaced with 'eval', 'train', 'train-config'
 
-# Quick evaluating and rendering your trained policy, just specify: 1.path of algorithm which you trained
-omnisafe eval ./saved_source/PPO-{SafetyPointGoal1-v0} --num-episode 1
+# Quick benchmarking for your research, just specify:
+# 1. exp_name
+# 2. num_pool(how much processes are concurrent)
+# 3. path of the config file (refer to omnisafe/examples/benchmarks for format)
+
+# Here we provide an exampe in ./tests/saved_source.
+# And you can set your benchmark_config.yaml by following it
+omnisafe benchmark test_benchmark 2 ./tests/saved_source/benchmark_config.yaml
+
+# Quick evaluating and rendering your trained policy, just specify:
+# 1. path of algorithm which you trained
+omnisafe eval ./tests/saved_source/PPO-{SafetyPointGoal1-v0} --num-episode 1
 
 # Quick training some algorithms to validate your thoughts
 # Note: use `key1:key2`, your can select key of hyperparameters which are recursively contained, and use `--custom-cfgs`, you can add custom cfgs via CLI
 omnisafe train --algo PPO --total-steps 2048 --vector-env-nums 1 --custom-cfgs algo_cfgs:steps_per_epoch --custom-cfgs 1024
 
 # Quick training some algorithms via a saved config file, the format is as same as default format
-omnisafe train-config ./saved_source/train_config.yaml
+omnisafe train-config ./tests/saved_source/train_config.yaml
 ```
 
 --------------------------------------------------------------------------------
 
 ## Getting Started
 
 ### Important Hints
 
-- `train_cfgs:torch_threads` is especially important for training speed, and is varying with users' machine, this value shouldn't be too small or too large.
+We have provided benchmark results for various algorithms, including on-policy, off-policy, model-based, and offline approaches, along with parameter tuning analysis. Please refer to the following:
+
+- [On-Policy](./benchmarks/on-policy/)
+- [Off-Policy](./benchmarks/off-policy/)
+- [Model-based](./benchmarks/model-based/)
+- [Offline](./benchmarks/offline/)
 
 ### Quickstart: Colab on the Cloud
 
-Explore OmniSafe easily and quickly through a series of colab notebooks:
+Explore OmniSafe easily and quickly through a series of Google Colab notebooks:
 
-- [Getting Started](https://colab.research.google.com/github/OmniSafeAI/omnisafe/blob/main/tutorials/English/1.Getting_Started.ipynb) Introduce the basic usage of OmniSafe so that users can quickly hand on it.
-- [CLI Command](https://colab.research.google.com/github/OmniSafeAI/omnisafe/blob/main/tutorials/English/2.CLI_Command.ipynb) Introduce how to use the CLI tool of OmniSafe.
+- [Getting Started](https://colab.research.google.com/github/PKU-Alignment/omnisafe/blob/main/tutorials/English/1.Getting_Started.ipynb) Introduce the basic usage of OmniSafe so that users can quickly hand it.
+- [CLI Command](https://colab.research.google.com/github/PKU-Alignment/omnisafe/blob/main/tutorials/English/2.CLI_Command.ipynb) Introduce how to use the CLI tool of OmniSafe.
 
 We take great pleasure in collaborating with our users to create tutorials in various languages.
 Please refer to our list of currently supported languages.
 If you are interested in translating the tutorial into a new language or improving an existing version, kindly submit a PR to us.
 
 --------------------------------------------------------------------------------
 
 ## Changelog
 
-See [CHANGELOG.md](https://github.com/OmniSafeAI/omnisafe/blob/main/CHANGELOG.md).
+See [CHANGELOG.md](https://github.com/PKU-Alignment/omnisafe/blob/main/CHANGELOG.md).
+
+## Citing OmniSafe
+
+If you find OmniSafe useful or use OmniSafe in your research, please cite it in your publications.
+
+```bibtex
+@article{omnisafe,
+  title   = {OmniSafe: An Infrastructure for Accelerating Safe Reinforcement Learning Research},
+  author  = {Jiaming Ji, Jiayi Zhou, Borong Zhang, Juntao Dai, Xuehai Pan, Ruiyang Sun, Weidong Huang, Yiran Geng, Mickel Liu, Yaodong Yang},
+  journal = {arXiv preprint arXiv:2305.09304},
+  year    = {2023}
+}
+```
 
 ## The OmniSafe Team
 
-OmniSafe is mainly developed by the SafeRL research team directed by Prof. [Yaodong Yang](https://github.com/orgs/OmniSafeAI/people/PKU-YYang).
+OmniSafe is mainly developed by the SafeRL research team directed by Prof. [Yaodong Yang](https://www.yangyaodong.com/).
 Our SafeRL research team members include [Borong Zhang](https://github.com/muchvo), [Jiayi Zhou](https://github.com/Gaiejj), [JTao Dai](https://github.com/calico-1226), [Weidong Huang](https://github.com/hdadong), [Ruiyang Sun](https://github.com/rockmagma02), [Xuehai Pan](https://github.com/XuehaiPan) and [Jiaming Ji](https://github.com/zmsn-2077).
-If you have any questions in the process of using omnisafe, don't hesitate to ask your questions on [the GitHub issue page](https://github.com/OmniSafeAI/omnisafe/issues/new/choose), we will reply to you in 2-3 working days.
+If you have any questions in the process of using OmniSafe, don't hesitate to ask your questions on [the GitHub issue page](https://github.com/PKU-Alignment/omnisafe/issues/new/choose), we will reply to you in 2-3 working days.
 
 ## License
 
 OmniSafe is released under Apache License 2.0.
```

#### html2text {}

```diff
@@ -1,217 +1,224 @@
-Metadata-Version: 2.1 Name: omnisafe Version: 0.4.0 Summary: A comprehensive
-and reliable benchmark for safe reinforcement learning. Author: OmniSafe
-Contributors License: Apache License, Version 2.0 Project-URL: Homepage, https:
-//github.com/OmniSafeAI/omnisafe Project-URL: Repository, https://github.com/
-OmniSafeAI/omnisafe Project-URL: Documentation, https://omnisafe.readthedocs.io
-Project-URL: Bug Report, https://github.com/OmniSafeAI/omnisafe/issues
-Keywords: Safe Reinforcement Learning,Reinforcement Learning,PyTorch
-Classifier: Development Status :: 4 - Beta Classifier: License :: OSI Approved
-:: Apache Software License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Intended
-Audience :: Science/Research Classifier: Topic :: Scientific/Engineering ::
-Artificial Intelligence Classifier: Topic :: Software Development :: Libraries
-:: Python Modules Requires-Python: >=3.8 Description-Content-Type: text/
-markdown Provides-Extra: lint Provides-Extra: test License-File: LICENSE
-       [https://github.com/OmniSafeAI/omnisafe/raw/HEAD/images/logo.png]
-[![Organization](https://img.shields.io/badge/Organization-PKU_MARL-blue.svg)]
-    (https://github.com/OmniSafeAI) [![PyPI](https://img.shields.io/pypi/v/
-  omnisafe?logo=pypi)](https://pypi.org/project/omnisafe) [![tests](https://
-      img.shields.io/github/actions/workflow/status/OmniSafeAI/omnisafe/
-test.yml?label=tests&logo=github)](https://github.com/OmniSafeAI/omnisafe/tree/
-   HEAD/tests) [![Documentation Status](https://img.shields.io/readthedocs/
+     [https://github.com/PKU-Alignment/omnisafe/raw/HEAD/images/logo.png]
+  [![Organization](https://img.shields.io/badge/Organization-PKU--Alignment-
+blue)](https://github.com/PKU-Alignment) [![PyPI](https://img.shields.io/pypi/
+ v/omnisafe?logo=pypi)](https://pypi.org/project/omnisafe) [![tests](https://
+     img.shields.io/github/actions/workflow/status/PKU-Alignment/omnisafe/
+ test.yml?label=tests&logo=github)](https://github.com/PKU-Alignment/omnisafe/
+ tree/HEAD/tests) [![Documentation Status](https://img.shields.io/readthedocs/
   omnisafe?logo=readthedocs)](https://omnisafe.readthedocs.io) [![Downloads]
                  (https://static.pepy.tech/personalized-badge/
  omnisafe?period=total&left_color=grey&right_color=blue&left_text=downloads)]
       (https://pepy.tech/project/omnisafe) [![GitHub Repo Stars](https://
-img.shields.io/github/stars/OmniSafeAI/omnisafe?color=brightgreen&logo=github)]
-  (https://github.com/OmniSafeAI/OmniSafe/stargazers) [![codestyle](https://
- img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/
-     black) [![License](https://img.shields.io/github/license/OmniSafeAI/
-OmniSafe?label=license)](#license) [![CodeCov](https://img.shields.io/codecov/
-  c/github/OmniSafeAI/omnisafe/main?logo=codecov)](https://app.codecov.io/gh/
-   OmniSafeAI/omnisafe) [![Open In Colab](https://colab.research.google.com/
- assets/colab-badge.svg)](https://colab.research.google.com/github/OmniSafeAI/
-                                  omnisafe/)
+                  img.shields.io/github/stars/PKU-Alignment/
+  omnisafe?color=brightgreen&logo=github)](https://github.com/PKU-Alignment/
+ OmniSafe/stargazers) [![codestyle](https://img.shields.io/badge/code%20style-
+     black-000000.svg)](https://github.com/psf/black) [![License](https://
+img.shields.io/github/license/PKU-Alignment/OmniSafe?label=license)](#license)
+  [![CodeCov](https://img.shields.io/codecov/c/github/PKU-Alignment/omnisafe/
+ main?logo=codecov)](https://app.codecov.io/gh/PKU-Alignment/omnisafe) [![Open
+ In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
+           colab.research.google.com/github/PKU-Alignment/omnisafe/)
    _D_o_c_u_m_e_n_t_a_t_i_o_n | _I_m_p_l_e_m_e_n_t_e_d_ _A_l_g_o_r_i_t_h_m_s | _I_n_s_t_a_l_l_a_t_i_o_n | _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d |
                                     _L_i_c_e_n_s_e
 -------------------------------------------------------------------------------
-- **This library is currently under heavy development - if you have suggestions
-on the API or use-cases you'd like to be covered, please open a GitHub issue or
-reach out. We'd love to hear about how you're using the library.** OmniSafe is
-an infrastructural framework designed to accelerate safe reinforcement learning
-(RL) research by providing a comprehensive and reliable benchmark for safe RL
-algorithms. The field of RL has great potential to benefit the society, and
-safety concerns are a significant issue, and RL algorithms have raised concerns
-about unintended harm or unsafe behavior. Safe RL intends to develop algorithms
-that minimize the risk of unintended harm or unsafe behavior, but there is
-currently a lack of commonly recognized safe RL algorithm benchmarks. OmniSafe
-addresses these issues by providing more than 40 experimentally validated
-algorithms and a sound and efficient simulation environment. Researchers can
-use OmniSafe to conduct experiments and verify their ideas, ensuring
-consistency and enabling more efficient development of safe RL algorithms. By
-using OmniSafe as a benchmark, researchers can evaluate the performance of
-their own safe RL algorithms and contribute to the advancement of safe RL
-research. ---------------------------------------------------------------------
------------ ### Table of Contents - [Implemented Algorithms](#implemented-
-algorithms) - [Latest SafeRL Papers](#latest-saferl-papers) - [List of
-Algorithms](#list-of-algorithms) - [On-Policy Safe](#on-policy-safe) - [Off-
-Policy Safe](#off-policy-safe) - [Model-Based Safe](#model-based-safe) -
-[Offline Safe](#offline-safe) - [Others](#others) - [Installation]
-(#installation) - [Prerequisites](#prerequisites) - [Install from source]
-(#install-from-source) - [Install from PyPI](#install-from-pypi) - [Examples]
-(#examples) - [Try with CLI](#try-with-cli) - [Getting Started](#getting-
-started) - [Important Hints](#important-hints) - [Quickstart: Colab on the
-Cloud](#quickstart-colab-on-the-cloud) - [Changelog](#changelog) - [The
-OmniSafe Team](#the-omnisafe-team) - [License](#license) ----------------------
----------------------------------------------------------- ## Implemented
-Algorithms The supported interface algorithms currently include: ### Latest
-SafeRL Papers - **[AAAI 2023]** Augmented Proximal Policy Optimization for Safe
-Reinforcement Learning (APPO) - **[NeurIPS 2022]** [Constrained Update
-Projection Approach to Safe Policy Optimization (CUP)](https://arxiv.org/abs/
-2209.07089) - **[NeurIPS 2022]** [Effects of Safety State Augmentation on Safe
-Exploration (Simmer)](https://arxiv.org/abs/2206.02675) - **[NeurIPS 2022]**
-[Model-based Safe Deep Reinforcement Learning via a Constrained Proximal Policy
-Optimization Algorithm](https://arxiv.org/abs/2210.07573) - **[ICML 2022]**
-[SautÃ© RL: Almost Surely Safe Reinforcement Learning Using State Augmentation
-(SauteRL)](https://arxiv.org/abs/2202.06558) - **[ICML 2022]** [Constrained
-Variational Policy Optimization for Safe Reinforcement Learning (CVPO)](https:/
-/arxiv.org/abs/2201.11927) - **[IJCAI 2022]** [Penalized Proximal Policy
-Optimization for Safe Reinforcement Learning](https://arxiv.org/abs/2205.11814)
-- **[ICLR 2022]** [Constrained Policy Optimization via Bayesian World Models
-(LA-MBDA)](https://arxiv.org/abs/2201.09802) - **[AAAI 2022]** [Conservative
-and Adaptive Penalty for Model-Based Safe Reinforcement Learning (CAP)](https:/
-/arxiv.org/abs/2112.07701) ### List of Algorithms #### On-Policy Safe - [X]
-[The Lagrange version of PPO (PPO-Lag)](https://cdn.openai.com/safexp-
-short.pdf) - [X] [The Lagrange version of TRPO (TRPO-Lag)](https://
-cdn.openai.com/safexp-short.pdf) - [X] **[ICML 2017]** [Constrained Policy
-Optimization (CPO)](https://proceedings.mlr.press/v70/achiam17a) - [X] **[ICLR
-2019]** [Reward Constrained Policy Optimization (RCPO)](https://openreview.net/
-forum?id=SkfrvsA9FX) - [X] **[ICML 2020]** [Responsive Safety in Reinforcement
-Learning by PID Lagrangian Methods (PID-Lag)](https://arxiv.org/abs/2007.03964)
-- [X] **[NeurIPS 2020]** [First Order Constrained Optimization in Policy Space
-(FOCOPS)](https://arxiv.org/abs/2002.06506) - [X] **[AAAI 2020]** [IPO:
-Interior-point Policy Optimization under Constraints (IPO)](https://arxiv.org/
-abs/1910.09615) - [X] **[ICLR 2020]** [Projection-Based Constrained Policy
-Optimization (PCPO)](https://openreview.net/forum?id=rke3TJrtPS) - [X] **[ICML
-2021]** [CRPO: A New Approach for Safe Reinforcement Learning with Convergence
-Guarantee](https://arxiv.org/abs/2011.05869) - [x] **[IJCAI 2022]** [Penalized
-Proximal Policy Optimization for Safe Reinforcement Learning(P3O)](https://
-arxiv.org/pdf/2205.11814.pdf) #### Off-Policy Safe - [X] The Lagrange version
-of TD3 (TD3-Lag) - [X] The Lagrange version of DDPG (DDPG-Lag) - [X] The
-Lagrange version of SAC (SAC-Lag) - [X] **[ICML 2019]** [Lyapunov-based Safe
-Policy Optimization for Continuous Control (SDDPG)](https://arxiv.org/abs/
-1901.10031) - [X] **[ICML 2019]** [Lyapunov-based Safe Policy Optimization for
-Continuous Control (SDDPG-modular)](https://arxiv.org/abs/1901.10031) - [ ] **
-[ICML 2022]** [Constrained Variational Policy Optimization for Safe
-Reinforcement Learning (CVPO)](https://arxiv.org/abs/2201.11927) #### Model-
-Based Safe - [ ] **[NeurIPS 2021]** [Safe Reinforcement Learning by Imagining
-the Near Future (SMBPO)](https://arxiv.org/abs/2202.07789) - [X] **[CoRL 2021
-(Oral)]** [Learning Off-Policy with Online Planning (SafeLOOP)](https://
-arxiv.org/abs/2008.10066) - [X] **[AAAI 2022]** [Conservative and Adaptive
-Penalty for Model-Based Safe Reinforcement Learning (CAP)](https://arxiv.org/
-abs/2112.07701) - [X] **[NeurIPS 2022]** [Model-based Safe Deep Reinforcement
-Learning via a Constrained Proximal Policy Optimization Algorithm](https://
-arxiv.org/abs/2210.07573) - [ ] **[ICLR 2022]** [Constrained Policy
-Optimization via Bayesian World Models (LA-MBDA)](https://arxiv.org/abs/
-2201.09802) - [X] **[ICML 2022 Workshop]** [Constrained Model-based
+- OmniSafe is an infrastructural framework designed to accelerate safe
+reinforcement learning (RL) research. It provides a comprehensive and reliable
+benchmark for safe RL algorithms, and also an out-of-box modular toolkit for
+researchers. SafeRL intends to develop algorithms that minimize the risk of
+unintended harm or unsafe behavior. OmniSafe stands as the inaugural unified
+learning framework in the realm of safe reinforcement learning, aiming to
+foster the Growth of SafeRL Learning Community. The key features of OmniSafe: -
+**Highly Modular Framework.** OmniSafe presents a highly modular framework,
+incorporating an extensive collection of tens of algorithms tailored for safe
+reinforcement learning across diverse domains. This framework is versatile due
+to its abstraction of various algorithm types and well-designed API, using the
+Adapter and Wrapper design components to bridge gaps and enable seamless
+interactions between different components. This design allows for easy
+extension and customization, making it a powerful tool for developers working
+with different types of algorithms. - **High-performance parallel computing
+acceleration.** By harnessing the capabilities of `torch.distributed`, OmniSafe
+accelerates the learning process of algorithms with process parallelism. This
+enables OmniSafe not only to support environment-level asynchronous parallelism
+but also incorporates agent asynchronous learning. This methodology bolsters
+training stability and expedites the training process via the deployment of a
+parallel exploration mechanism. The integration of agent asynchronous learning
+in OmniSafe underscores its commitment to providing a versatile and robust
+platform for advancing SafeRL research. - **Out-of-box toolkits.** OmniSafe
+offers customizable toolkits for tasks like training, benchmarking, analyzing,
+and rendering. [Tutorials](https://github.com/PKU-Alignment/omnisafe#getting-
+started) and user-friendly [APIs](https://omnisafe.readthedocs.io/en/latest/
+baserlapi/on_policy.html) make it easy for beginners and average users, while
+advanced researchers can enhance their efficiency without complex code. ![Train
+video](https://github-production-user-asset-6210df.s3.amazonaws.com/73586554/
+237139607-d1e6f413-aa2c-4f68-b8ee-08a4361493a0.gif) ---------------------------
+----------------------------------------------------- ### Table of Contents -
+[Quick Start](#quick-start) - [Installation](#installation) - [Prerequisites]
+(#prerequisites) - [Install from source](#install-from-source) - [Install from
+PyPI](#install-from-pypi) - [Implemented Algorithms](#implemented-algorithms) -
+[Examples](#examples) - [Algorithms Registry](#algorithms-registry) -
+[Supported Environments](#supported-environments) - [Try with CLI](#try-with-
+cli) - [Getting Started](#getting-started) - [Important Hints](#important-
+hints) - [Quickstart: Colab on the Cloud](#quickstart-colab-on-the-cloud) -
+[Changelog](#changelog) - [Citing OmniSafe](#citing-omnisafe) - [The OmniSafe
+Team](#the-omnisafe-team) - [License](#license) -------------------------------
+------------------------------------------------- ## Quick Start ###
+Installation #### Prerequisites OmniSafe requires Python 3.8+ and PyTorch
+1.10+. > We support and test for Python 3.8, 3.9, 3.10 on Linux. Meanwhile, we
+also support M1 and M2 versions of macOS. We will accept PRs related to
+Windows, but do not officially support it. #### Install from source ```bash #
+Clone the repo git clone https://github.com/PKU-Alignment/omnisafe.git cd
+omnisafe # Create a conda environment conda env create --file conda-recipe.yaml
+conda activate omnisafe # Install omnisafe pip install -e . ``` #### Install
+from PyPI OmniSafe is hosted in [![PyPI](https://img.shields.io/pypi/v/
+omnisafe?label=pypi&logo=pypi)](https://pypi.org/project/omnisafe) / ![Status]
+(https://img.shields.io/pypi/status/omnisafe?label=status). ```bash pip install
+omnisafe ``` ## Implemented Algorithms LLaatteesstt SSaaffeeRRLL PPaappeerrss - **[AAAI 2023]**
+Augmented Proximal Policy Optimization for Safe Reinforcement Learning (APPO) -
+**[NeurIPS 2022]** [Constrained Update Projection Approach to Safe Policy
+Optimization (CUP)](https://arxiv.org/abs/2209.07089) - **[NeurIPS 2022]**
+[Effects of Safety State Augmentation on Safe Exploration (Simmer)](https://
+arxiv.org/abs/2206.02675) - **[NeurIPS 2022]** [Model-based Safe Deep
+Reinforcement Learning via a Constrained Proximal Policy Optimization
+Algorithm](https://arxiv.org/abs/2210.07573) - **[ICML 2022]** [SautÃ© RL:
+Almost Surely Safe Reinforcement Learning Using State Augmentation (SauteRL)]
+(https://arxiv.org/abs/2202.06558) - **[IJCAI 2022]** [Penalized Proximal
+Policy Optimization for Safe Reinforcement Learning](https://arxiv.org/abs/
+2205.11814) - **[AAAI 2022]** [Conservative and Adaptive Penalty for Model-
+Based Safe Reinforcement Learning (CAP)](https://arxiv.org/abs/2112.07701) LLiisstt
+ooff AAllggoorriitthhmmss OOnn PPoolliiccyy SSaaffeeRRLL - [x] [The Lagrange version of PPO (PPO-Lag)]
+(https://cdn.openai.com/safexp-short.pdf) - [x] [The Lagrange version of TRPO
+(TRPO-Lag)](https://cdn.openai.com/safexp-short.pdf) - [x] **[ICML 2017]**
+[Constrained Policy Optimization (CPO)](https://proceedings.mlr.press/v70/
+achiam17a) - [x] **[ICLR 2019]** [Reward Constrained Policy Optimization
+(RCPO)](https://openreview.net/forum?id=SkfrvsA9FX) - [x] **[ICML 2020]**
+[Responsive Safety in Reinforcement Learning by PID Lagrangian Methods (PID-
+Lag)](https://arxiv.org/abs/2007.03964) - [x] **[NeurIPS 2020]** [First Order
+Constrained Optimization in Policy Space (FOCOPS)](https://arxiv.org/abs/
+2002.06506) - [x] **[AAAI 2020]** [IPO: Interior-point Policy Optimization
+under Constraints (IPO)](https://arxiv.org/abs/1910.09615) - [x] **[ICLR
+2020]** [Projection-Based Constrained Policy Optimization (PCPO)](https://
+openreview.net/forum?id=rke3TJrtPS) - [x] **[ICML 2021]** [CRPO: A New Approach
+for Safe Reinforcement Learning with Convergence Guarantee](https://arxiv.org/
+abs/2011.05869) - [x] **[IJCAI 2022]** [Penalized Proximal Policy Optimization
+for Safe Reinforcement Learning(P3O)](https://arxiv.org/pdf/2205.11814.pdf) OOffff
+PPoolliiccyy SSaaffeeRRLL - **[Preprint 2019]** [The Lagrangian version of DDPG (DDPGLag)]
+(https://cdn.openai.com/safexp-short.pdf) - **[Preprint 2019]** [The Lagrangian
+version of TD3 (TD3Lag)](https://cdn.openai.com/safexp-short.pdf) - **[Preprint
+2019]** [The Lagrangian version of SAC (SACLag)](https://cdn.openai.com/safexp-
+short.pdf) - **[ICML 2020]** [Responsive Safety in Reinforcement Learning by
+PID Lagrangian Methods (DDPGPID)](https://arxiv.org/abs/2007.03964) - **[ICML
+2020]** [Responsive Safety in Reinforcement Learning by PID Lagrangian Methods
+(TD3PID)](https://arxiv.org/abs/2007.03964) - **[ICML 2020]** [Responsive
+Safety in Reinforcement Learning by PID Lagrangian Methods (SACPID)](https://
+arxiv.org/abs/2007.03964) MMooddeell--BBaasseedd SSaaffeeRRLL - [ ] **[NeurIPS 2021]** [Safe
+Reinforcement Learning by Imagining the Near Future (SMBPO)](https://arxiv.org/
+abs/2202.07789) - [x] **[CoRL 2021 (Oral)]** [Learning Off-Policy with Online
+Planning (SafeLOOP)](https://arxiv.org/abs/2008.10066) - [x] **[AAAI 2022]**
+[Conservative and Adaptive Penalty for Model-Based Safe Reinforcement Learning
+(CAP)](https://arxiv.org/abs/2112.07701) - [x] **[NeurIPS 2022]** [Model-based
+Safe Deep Reinforcement Learning via a Constrained Proximal Policy Optimization
+Algorithm](https://arxiv.org/abs/2210.07573) - [ ] **[ICLR 2022]** [Constrained
+Policy Optimization via Bayesian World Models (LA-MBDA)](https://arxiv.org/abs/
+2201.09802) - [x] **[ICML 2022 Workshop]** [Constrained Model-based
 Reinforcement Learning with Robust Cross-Entropy Method (RCE)](https://
-arxiv.org/abs/2010.07968) - [X] **[NeurIPS 2018]** [Constrained Cross-Entropy
+arxiv.org/abs/2010.07968) - [x] **[NeurIPS 2018]** [Constrained Cross-Entropy
 Method for Safe Reinforcement Learning (CCE)](https://proceedings.neurips.cc/
-paper/2018/hash/34ffeb359a192eb8174b6854643cc046-Abstract.html) #### Offline
-Safe - [X] [The Lagrange version of BCQ (BCQ-Lag)](https://arxiv.org/abs/
-1812.02900) - [X] [The Constrained version of CRR (C-CRR)](https://
-proceedings.neurips.cc/paper/2020/hash/588cb956d6bbe67078f29f8de420a13d-
-Abstract.html) - [ ] **[AAAI 2022]** [Constraints Penalized Q-learning for Safe
-Offline Reinforcement Learning CPQ](https://arxiv.org/abs/2107.09003) - [ ] **
-[ICLR 2022 (Spotlight)]** [COptiDICE: Offline Constrained Reinforcement
-Learning via Stationary Distribution Correction Estimation](https://arxiv.org/
-abs/2204.08957?context=cs.AI) - [ ] **[ICML 2022]** [Constrained Offline Policy
-Optimization (COPO)](https://proceedings.mlr.press/v162/polosky22a.html) ####
-Others - [X] [Safe Exploration in Continuous Action Spaces (Safety Layer)]
-(https://arxiv.org/abs/1801.08757) - [ ] **[RA-L 2021]** [Recovery RL: Safe
-Reinforcement Learning with Learned Recovery Zones](https://arxiv.org/abs/
-2010.15920) - [X] **[ICML 2022]** [SautÃ© RL: Almost Surely Safe Reinforcement
-Learning Using State Augmentation (SauteRL)](https://arxiv.org/abs/2202.06558)
-- [X] **[NeurIPS 2022]** [Effects of Safety State Augmentation on Safe
-Exploration](https://arxiv.org/abs/2206.02675) --------------------------------
------------------------------------------------- ## Installation ###
-Prerequisites OmniSafe requires Python 3.8+ and PyTorch 1.10+. > We support and
-test for Python 3.8, 3.9, 3.10 on Linux. Meanwhile, we also support M1 and M2
-versions of macOS. We will accept PRs related to Windows, but do not officially
-support it. #### Install from source ```bash # Clone the repo git clone https:/
-/github.com/OmniSafeAI/omnisafe cd omnisafe # Create a conda environment conda
-env create --file conda-recipe.yaml conda activate omnisafe # Install omnisafe
-pip install -e . ``` #### Install from PyPI OmniSafe is hosted in [![PyPI]
-(https://img.shields.io/pypi/v/omnisafe?label=pypi&logo=pypi)](https://
-pypi.org/project/omnisafe) / ![Status](https://img.shields.io/pypi/status/
-omnisafe?label=status). ```bash pip install omnisafe ``` ### Examples ```bash
-cd examples python train_policy.py --algo PPOLag --env-id SafetyPointGoal1-v0 -
--parallel 1 --total-steps 1024000 --device cpu --vector-env-nums 1 --torch-
-threads 1 ``` **algo:** | Type | Name | | ----------------- | -----------------
------------------------------------------------ | | `Base-On-Policy` |
-`PolicyGradient, PPO`
-`NaturalPG, TRPO` | | `Base-Off-Policy` | `DDPG, TD3, SAC` | | `Naive Lagrange`
-| `RCPO, PPOLag, TRPOLag`
-`DDPGLag, TD3Lag, SACLag` | | `PID Lagrange` | `CPPOPid, TRPOPid` | | `First
-Order` | `FOCOPS, CUP` | | `Second Order` | `SDDPG, CPO, PCPO` | | `Saute RL` |
-`PPOSaute, PPOLagSaute` | | `Simmer RL` | `PPOSimmerQ, PPOSimmerPid`
-`PPOLagSimmerQ, PPOLagSimmerPid` | | `EarlyTerminated` | `PPOEarlyTerminated`
-`PPOLagEarlyTerminated` | | `Model-Based` | `CAP, MBPPOLag, SafeLOOP` | **env-
-id:** Environment id in [Safety Gymnasium](https://www.safety-gymnasium.com/),
-here a list of envs that safety-gymnasium supports.
+paper/2018/hash/34ffeb359a192eb8174b6854643cc046-Abstract.html) OOfffflliinnee SSaaffeeRRLL
+- [x] [The Lagrange version of BCQ (BCQ-Lag)](https://arxiv.org/abs/1812.02900)
+- [x] [The Constrained version of CRR (C-CRR)](https://proceedings.neurips.cc/
+paper/2020/hash/588cb956d6bbe67078f29f8de420a13d-Abstract.html) - [ ] **[AAAI
+2022]** [Constraints Penalized Q-learning for Safe Offline Reinforcement
+Learning CPQ](https://arxiv.org/abs/2107.09003) - [x] **[ICLR 2022
+(Spotlight)]** [COptiDICE: Offline Constrained Reinforcement Learning via
+Stationary Distribution Correction Estimation](https://arxiv.org/abs/
+2204.08957?context=cs.AI) - [ ] **[ICML 2022]** [Constrained Offline Policy
+Optimization (COPO)](https://proceedings.mlr.press/v162/polosky22a.html) OOtthheerrss
+- [ ] **[RA-L 2021]** [Recovery RL: Safe Reinforcement Learning with Learned
+Recovery Zones](https://arxiv.org/abs/2010.15920) - [x] **[ICML 2022]** [SautÃ©
+RL: Almost Surely Safe Reinforcement Learning Using State Augmentation
+(SauteRL)](https://arxiv.org/abs/2202.06558) - [x] **[NeurIPS 2022]** [Effects
+of Safety State Augmentation on Safe Exploration](https://arxiv.org/abs/
+2206.02675) -------------------------------------------------------------------
+------------- ### Examples ```bash cd examples python train_policy.py --algo
+PPOLag --env-id SafetyPointGoal1-v0 --parallel 1 --total-steps 10000000 --
+device cpu --vector-env-nums 1 --torch-threads 1 ``` #### Algorithms Registry
+DDoommaaiinnss               TTyyppeess                AAllggoorriitthhmmss RReeggiissttrryy
+                      Primal Dual          TRPOLag; PPOLag; PDO; RCPO
+                                           TRPOPID; CPPOPID
+On Policy             Convex Optimization  CPO; PCPO; FOCOPS; CUP
+                      Penalty Function     IPO; P3O
+                      Primal               OnCRPO
+Off Policy            Primal-Dual          DDPGLag; TD3Lag; SACLag
+                                           DDPGPID; TD3PID; SACPID
+Model-based           Online Plan          SafeLOOP; CCEPETS; RCEPETS
+                      Pessimistic Estimate CAPPETS
+DICE Based            COptDICE
+                      ET-MDP               PPOEarlyTerminated;
+Other Formulation MDP                      TRPOEarlyTerminated
+                      SauteRL              PPOSaute; TRPOSaute
+                      SimmerRL             PPOSimmerPID; TRPOSimmerPID
+#### Supported Environments Here is a list of environments that [Safety-
+Gymnasium](https://www.safety-gymnasium.com) supports:
  _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
 |_CC_aa_tt_ee_gg_oo_rr_yy_ _ _ _ _ _ _ _|_TT_aa_ss_kk_ _ _ _ _ _ _ _|_AA_gg_ee_nn_tt_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_EE_xx_aa_mm_pp_ll_ee_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |               |_G_o_a_l_[_0_1_2_]_ _ |                        |                       |
 |Safe Navigation|_B_u_t_t_o_n_[_0_1_2_]|Point, Car, Racecar, Ant|SafetyPointGoal1-v0    |
 |               |_P_u_s_h_[_0_1_2_]_ _ |                        |                       |
 |_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_C_i_r_c_l_e_[_0_1_2_]_|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |               |           |HalfCheetah, Hopper,    |SafetyHumanoidVelocity-|
 |Safe Velocity  |Velocity   |Swimmer, Walker2d, Ant, |v1                     |
 |_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _|_H_u_m_a_n_o_i_d_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
-More information about environments, please refer to [Safety Gymnasium](https:/
-/www.safety-gymnasium.com/) **parallel:** `Number of parallels` #### Try with
-CLI **A video example** ![Segmentfault](https://github.com/OmniSafeAI/omnisafe/
-blob/main/images/CLI_example.svg) ```bash pip install omnisafe omnisafe --help
-# Ask for help omnisafe benchmark --help # The benchmark also can be replaced
-with 'eval', 'train', 'train-config' # Quick benchmarking for your research,
-just specify: 1.exp_name, 2.num_pool(how much processes are concurrent), 3.path
-of the config file(refer to omnisafe/examples/benchmarks for format) omnisafe
-benchmark test_benchmark 2 ./saved_source/benchmark_config.yaml # Quick
-evaluating and rendering your trained policy, just specify: 1.path of algorithm
-which you trained omnisafe eval ./saved_source/PPO-{SafetyPointGoal1-v0} --num-
-episode 1 # Quick training some algorithms to validate your thoughts # Note:
-use `key1:key2`, your can select key of hyperparameters which are recursively
-contained, and use `--custom-cfgs`, you can add custom cfgs via CLI omnisafe
-train --algo PPO --total-steps 2048 --vector-env-nums 1 --custom-cfgs
-algo_cfgs:steps_per_epoch --custom-cfgs 1024 # Quick training some algorithms
-via a saved config file, the format is as same as default format omnisafe
-train-config ./saved_source/train_config.yaml ``` -----------------------------
---------------------------------------------------- ## Getting Started ###
-Important Hints - `train_cfgs:torch_threads` is especially important for
-training speed, and is varying with users' machine, this value shouldn't be too
-small or too large. ### Quickstart: Colab on the Cloud Explore OmniSafe easily
-and quickly through a series of colab notebooks: - [Getting Started](https://
-colab.research.google.com/github/OmniSafeAI/omnisafe/blob/main/tutorials/
-English/1.Getting_Started.ipynb) Introduce the basic usage of OmniSafe so that
-users can quickly hand on it. - [CLI Command](https://
-colab.research.google.com/github/OmniSafeAI/omnisafe/blob/main/tutorials/
+For more information about environments, please refer to [Safety-Gymnasium]
+(https://www.safety-gymnasium.com). #### Try with CLI ```bash pip install
+omnisafe omnisafe --help # Ask for help omnisafe benchmark --help # The
+benchmark also can be replaced with 'eval', 'train', 'train-config' # Quick
+benchmarking for your research, just specify: # 1. exp_name # 2. num_pool(how
+much processes are concurrent) # 3. path of the config file (refer to omnisafe/
+examples/benchmarks for format) # Here we provide an exampe in ./tests/
+saved_source. # And you can set your benchmark_config.yaml by following it
+omnisafe benchmark test_benchmark 2 ./tests/saved_source/benchmark_config.yaml
+# Quick evaluating and rendering your trained policy, just specify: # 1. path
+of algorithm which you trained omnisafe eval ./tests/saved_source/PPO-
+{SafetyPointGoal1-v0} --num-episode 1 # Quick training some algorithms to
+validate your thoughts # Note: use `key1:key2`, your can select key of
+hyperparameters which are recursively contained, and use `--custom-cfgs`, you
+can add custom cfgs via CLI omnisafe train --algo PPO --total-steps 2048 --
+vector-env-nums 1 --custom-cfgs algo_cfgs:steps_per_epoch --custom-cfgs 1024 #
+Quick training some algorithms via a saved config file, the format is as same
+as default format omnisafe train-config ./tests/saved_source/train_config.yaml
+``` ---------------------------------------------------------------------------
+----- ## Getting Started ### Important Hints We have provided benchmark results
+for various algorithms, including on-policy, off-policy, model-based, and
+offline approaches, along with parameter tuning analysis. Please refer to the
+following: - [On-Policy](./benchmarks/on-policy/) - [Off-Policy](./benchmarks/
+off-policy/) - [Model-based](./benchmarks/model-based/) - [Offline](./
+benchmarks/offline/) ### Quickstart: Colab on the Cloud Explore OmniSafe easily
+and quickly through a series of Google Colab notebooks: - [Getting Started]
+(https://colab.research.google.com/github/PKU-Alignment/omnisafe/blob/main/
+tutorials/English/1.Getting_Started.ipynb) Introduce the basic usage of
+OmniSafe so that users can quickly hand it. - [CLI Command](https://
+colab.research.google.com/github/PKU-Alignment/omnisafe/blob/main/tutorials/
 English/2.CLI_Command.ipynb) Introduce how to use the CLI tool of OmniSafe. We
 take great pleasure in collaborating with our users to create tutorials in
 various languages. Please refer to our list of currently supported languages.
 If you are interested in translating the tutorial into a new language or
 improving an existing version, kindly submit a PR to us. ----------------------
 ---------------------------------------------------------- ## Changelog See
-[CHANGELOG.md](https://github.com/OmniSafeAI/omnisafe/blob/main/CHANGELOG.md).
-## The OmniSafe Team OmniSafe is mainly developed by the SafeRL research team
-directed by Prof. [Yaodong Yang](https://github.com/orgs/OmniSafeAI/people/PKU-
-YYang). Our SafeRL research team members include [Borong Zhang](https://
-github.com/muchvo), [Jiayi Zhou](https://github.com/Gaiejj), [JTao Dai](https:/
-/github.com/calico-1226), [Weidong Huang](https://github.com/hdadong), [Ruiyang
-Sun](https://github.com/rockmagma02), [Xuehai Pan](https://github.com/
-XuehaiPan) and [Jiaming Ji](https://github.com/zmsn-2077). If you have any
-questions in the process of using omnisafe, don't hesitate to ask your
-questions on [the GitHub issue page](https://github.com/OmniSafeAI/omnisafe/
-issues/new/choose), we will reply to you in 2-3 working days. ## License
-OmniSafe is released under Apache License 2.0.
+[CHANGELOG.md](https://github.com/PKU-Alignment/omnisafe/blob/main/
+CHANGELOG.md). ## Citing OmniSafe If you find OmniSafe useful or use OmniSafe
+in your research, please cite it in your publications. ```bibtex @article
+{omnisafe, title = {OmniSafe: An Infrastructure for Accelerating Safe
+Reinforcement Learning Research}, author = {Jiaming Ji, Jiayi Zhou, Borong
+Zhang, Juntao Dai, Xuehai Pan, Ruiyang Sun, Weidong Huang, Yiran Geng, Mickel
+Liu, Yaodong Yang}, journal = {arXiv preprint arXiv:2305.09304}, year = {2023}
+} ``` ## The OmniSafe Team OmniSafe is mainly developed by the SafeRL research
+team directed by Prof. [Yaodong Yang](https://www.yangyaodong.com/). Our SafeRL
+research team members include [Borong Zhang](https://github.com/muchvo), [Jiayi
+Zhou](https://github.com/Gaiejj), [JTao Dai](https://github.com/calico-1226),
+[Weidong Huang](https://github.com/hdadong), [Ruiyang Sun](https://github.com/
+rockmagma02), [Xuehai Pan](https://github.com/XuehaiPan) and [Jiaming Ji]
+(https://github.com/zmsn-2077). If you have any questions in the process of
+using OmniSafe, don't hesitate to ask your questions on [the GitHub issue page]
+(https://github.com/PKU-Alignment/omnisafe/issues/new/choose), we will reply to
+you in 2-3 working days. ## License OmniSafe is released under Apache License
+2.0.
```

### Comparing `omnisafe-0.4.0/README.md` & `omnisafe-0.5.0b0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,196 +1,289 @@
+Metadata-Version: 2.1
+Name: omnisafe
+Version: 0.5.0b0
+Summary: A comprehensive and reliable benchmark for safe reinforcement learning.
+Author: OmniSafe Contributors
+License: Apache License, Version 2.0
+Project-URL: Homepage, https://github.com/PKU-Alignment/omnisafe
+Project-URL: Repository, https://github.com/PKU-Alignment/omnisafe
+Project-URL: Documentation, https://omnisafe.readthedocs.io
+Project-URL: Bug Report, https://github.com/PKU-Alignment/omnisafe/issues
+Keywords: Safe Reinforcement Learning,Reinforcement Learning,PyTorch
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: lint
+Provides-Extra: test
+License-File: LICENSE
+
 <!-- markdownlint-disable first-line-h1 -->
 <!-- markdownlint-disable html -->
 
 <div align="center">
-  <img src="https://github.com/OmniSafeAI/omnisafe/raw/HEAD/images/logo.png" width="75%"/>
+  <img src="https://github.com/PKU-Alignment/omnisafe/raw/HEAD/images/logo.png" width="75%"/>
 </div>
 
 <div align="center">
 
-  [![Organization](https://img.shields.io/badge/Organization-PKU_MARL-blue.svg)](https://github.com/OmniSafeAI)
+  [![Organization](https://img.shields.io/badge/Organization-PKU--Alignment-blue)](https://github.com/PKU-Alignment)
   [![PyPI](https://img.shields.io/pypi/v/omnisafe?logo=pypi)](https://pypi.org/project/omnisafe)
-  [![tests](https://img.shields.io/github/actions/workflow/status/OmniSafeAI/omnisafe/test.yml?label=tests&logo=github)](https://github.com/OmniSafeAI/omnisafe/tree/HEAD/tests)
+  [![tests](https://img.shields.io/github/actions/workflow/status/PKU-Alignment/omnisafe/test.yml?label=tests&logo=github)](https://github.com/PKU-Alignment/omnisafe/tree/HEAD/tests)
   [![Documentation Status](https://img.shields.io/readthedocs/omnisafe?logo=readthedocs)](https://omnisafe.readthedocs.io)
   [![Downloads](https://static.pepy.tech/personalized-badge/omnisafe?period=total&left_color=grey&right_color=blue&left_text=downloads)](https://pepy.tech/project/omnisafe)
-  [![GitHub Repo Stars](https://img.shields.io/github/stars/OmniSafeAI/omnisafe?color=brightgreen&logo=github)](https://github.com/OmniSafeAI/OmniSafe/stargazers)
+  [![GitHub Repo Stars](https://img.shields.io/github/stars/PKU-Alignment/omnisafe?color=brightgreen&logo=github)](https://github.com/PKU-Alignment/OmniSafe/stargazers)
   [![codestyle](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-  [![License](https://img.shields.io/github/license/OmniSafeAI/OmniSafe?label=license)](#license)
-  [![CodeCov](https://img.shields.io/codecov/c/github/OmniSafeAI/omnisafe/main?logo=codecov)](https://app.codecov.io/gh/OmniSafeAI/omnisafe)
-  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/OmniSafeAI/omnisafe/)
+  [![License](https://img.shields.io/github/license/PKU-Alignment/OmniSafe?label=license)](#license)
+  [![CodeCov](https://img.shields.io/codecov/c/github/PKU-Alignment/omnisafe/main?logo=codecov)](https://app.codecov.io/gh/PKU-Alignment/omnisafe)
+  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/PKU-Alignment/omnisafe/)
 
 </div>
 
 <p align="center">
   <a href="https://omnisafe.readthedocs.io">Documentation</a> |
-  <a href="https://github.com/OmniSafeAI/omnisafe#implemented-algorithms">Implemented Algorithms</a> |
-  <a href="https://github.com/OmniSafeAI/omnisafe#installation">Installation</a> |
-  <a href="https://github.com/OmniSafeAI/omnisafe#getting-started">Getting Started</a> |
-  <a href="https://github.com/OmniSafeAI/omnisafe#license">License</a>
+  <a href="https://github.com/PKU-Alignment/omnisafe#implemented-algorithms">Implemented Algorithms</a> |
+  <a href="https://github.com/PKU-Alignment/omnisafe#installation">Installation</a> |
+  <a href="https://github.com/PKU-Alignment/omnisafe#getting-started">Getting Started</a> |
+  <a href="https://github.com/PKU-Alignment/omnisafe#license">License</a>
 </p>
 
 --------------------------------------------------------------------------------
 
-**This library is currently under heavy development - if you have suggestions on the API or use-cases you'd like to be covered, please open a GitHub issue or reach out. We'd love to hear about how you're using the library.**
+OmniSafe is an infrastructural framework designed to accelerate safe reinforcement learning (RL) research.
+It provides a comprehensive and reliable benchmark for safe RL algorithms, and also an out-of-box modular toolkit for researchers.
+SafeRL intends to develop algorithms that minimize the risk of unintended harm or unsafe behavior.
+
+OmniSafe stands as the inaugural unified learning framework in the realm of safe reinforcement learning, aiming to foster the Growth of SafeRL Learning Community.
+The key features of OmniSafe:
+
+- **Highly Modular Framework.** OmniSafe presents a highly modular framework, incorporating an extensive collection of tens of algorithms tailored for safe reinforcement learning across diverse domains. This framework is versatile due to its abstraction of various algorithm types and well-designed API, using the Adapter and Wrapper design components to bridge gaps and enable seamless interactions between different components. This design allows for easy extension and customization, making it a powerful tool for developers working with different types of algorithms.
+
+- **High-performance parallel computing acceleration.** By harnessing the capabilities of `torch.distributed`, OmniSafe accelerates the learning process of algorithms
+with process parallelism. This enables OmniSafe not only to support environment-level asynchronous parallelism but also incorporates agent asynchronous learning. This methodology bolsters training stability and expedites the training process via the deployment of a parallel exploration mechanism. The integration of agent asynchronous learning in OmniSafe underscores its commitment to providing a versatile and robust platform for advancing SafeRL research.
 
-OmniSafe is an infrastructural framework designed to accelerate safe reinforcement learning (RL) research by providing a comprehensive and reliable benchmark for safe RL algorithms.
-The field of RL has great potential to benefit the society, and safety concerns are a significant issue, and RL algorithms have raised concerns about unintended harm or unsafe behavior.
-Safe RL intends to develop algorithms that minimize the risk of unintended harm or unsafe behavior, but there is currently a lack of commonly recognized safe RL algorithm benchmarks.
-
-OmniSafe addresses these issues by providing more than 40 experimentally validated algorithms and a sound and efficient simulation environment.
-Researchers can use OmniSafe to conduct experiments and verify their ideas, ensuring consistency and enabling more efficient development of safe RL algorithms.
-By using OmniSafe as a benchmark, researchers can evaluate the performance of their own safe RL algorithms and contribute to the advancement of safe RL research.
+- **Out-of-box toolkits.** OmniSafe offers customizable toolkits for tasks like training, benchmarking, analyzing, and rendering. [Tutorials](https://github.com/PKU-Alignment/omnisafe#getting-started) and user-friendly [APIs](https://omnisafe.readthedocs.io/en/latest/baserlapi/on_policy.html) make it easy for beginners and average users, while advanced researchers can enhance their efficiency without complex code.
+
+![Train video](https://github-production-user-asset-6210df.s3.amazonaws.com/73586554/237139607-d1e6f413-aa2c-4f68-b8ee-08a4361493a0.gif)
 
 --------------------------------------------------------------------------------
 
 ### Table of Contents  <!-- omit in toc --> <!-- markdownlint-disable heading-increment -->
 
-- [Implemented Algorithms](#implemented-algorithms)
-  - [Latest SafeRL Papers](#latest-saferl-papers)
-  - [List of Algorithms](#list-of-algorithms)
-    - [On-Policy Safe](#on-policy-safe)
-    - [Off-Policy Safe](#off-policy-safe)
-    - [Model-Based Safe](#model-based-safe)
-    - [Offline Safe](#offline-safe)
-    - [Others](#others)
-- [Installation](#installation)
-  - [Prerequisites](#prerequisites)
+- [Quick Start](#quick-start)
+  - [Installation](#installation)
+    - [Prerequisites](#prerequisites)
     - [Install from source](#install-from-source)
     - [Install from PyPI](#install-from-pypi)
+- [Implemented Algorithms](#implemented-algorithms)
   - [Examples](#examples)
+    - [Algorithms Registry](#algorithms-registry)
+    - [Supported Environments](#supported-environments)
     - [Try with CLI](#try-with-cli)
 - [Getting Started](#getting-started)
   - [Important Hints](#important-hints)
   - [Quickstart: Colab on the Cloud](#quickstart-colab-on-the-cloud)
 - [Changelog](#changelog)
+- [Citing OmniSafe](#citing-omnisafe)
 - [The OmniSafe Team](#the-omnisafe-team)
 - [License](#license)
 
 --------------------------------------------------------------------------------
 
-## Implemented Algorithms
+## Quick Start
+
+### Installation
+
+#### Prerequisites
+
+OmniSafe requires Python 3.8+ and PyTorch 1.10+.
+
+> We support and test for Python 3.8, 3.9, 3.10 on Linux. Meanwhile, we also support M1 and M2 versions of macOS. We will accept PRs related to Windows, but do not officially support it.
+
+#### Install from source
+
+```bash
+# Clone the repo
+git clone https://github.com/PKU-Alignment/omnisafe.git
+cd omnisafe
+
+# Create a conda environment
+conda env create --file conda-recipe.yaml
+conda activate omnisafe
+
+# Install omnisafe
+pip install -e .
+```
 
-The supported interface algorithms currently include:
+#### Install from PyPI
+
+OmniSafe is hosted in [![PyPI](https://img.shields.io/pypi/v/omnisafe?label=pypi&logo=pypi)](https://pypi.org/project/omnisafe) / ![Status](https://img.shields.io/pypi/status/omnisafe?label=status).
+
+```bash
+pip install omnisafe
+```
 
-### Latest SafeRL Papers
+## Implemented Algorithms
+
+<details>
+<summary><b><big>Latest SafeRL Papers</big></b></summary>
 
 - **[AAAI 2023]** Augmented Proximal Policy Optimization for Safe Reinforcement Learning (APPO)
 - **[NeurIPS 2022]** [Constrained Update Projection Approach to Safe Policy Optimization (CUP)](https://arxiv.org/abs/2209.07089)
 - **[NeurIPS 2022]** [Effects of Safety State Augmentation on Safe Exploration (Simmer)](https://arxiv.org/abs/2206.02675)
 - **[NeurIPS 2022]** [Model-based Safe Deep Reinforcement Learning via a Constrained Proximal Policy Optimization Algorithm](https://arxiv.org/abs/2210.07573)
 - **[ICML 2022]** [Sauté RL: Almost Surely Safe Reinforcement Learning Using State Augmentation (SauteRL)](https://arxiv.org/abs/2202.06558)
-- **[ICML 2022]** [Constrained Variational Policy Optimization for Safe Reinforcement Learning (CVPO)](https://arxiv.org/abs/2201.11927)
 - **[IJCAI 2022]** [Penalized Proximal Policy Optimization for Safe Reinforcement Learning](https://arxiv.org/abs/2205.11814)
-- **[ICLR 2022]** [Constrained Policy Optimization via Bayesian World Models (LA-MBDA)](https://arxiv.org/abs/2201.09802)
 - **[AAAI 2022]** [Conservative and Adaptive Penalty for Model-Based Safe Reinforcement Learning (CAP)](https://arxiv.org/abs/2112.07701)
 
-### List of Algorithms
+</details>
 
-#### On-Policy Safe
+<details>
+<summary><b><big>List of Algorithms</big></b></summary>
 
-- [X] [The Lagrange version of PPO (PPO-Lag)](https://cdn.openai.com/safexp-short.pdf)
-- [X] [The Lagrange version of TRPO (TRPO-Lag)](https://cdn.openai.com/safexp-short.pdf)
-- [X] **[ICML 2017]** [Constrained Policy Optimization (CPO)](https://proceedings.mlr.press/v70/achiam17a)
-- [X] **[ICLR 2019]** [Reward Constrained Policy Optimization (RCPO)](https://openreview.net/forum?id=SkfrvsA9FX)
-- [X] **[ICML 2020]** [Responsive Safety in Reinforcement Learning by PID Lagrangian Methods (PID-Lag)](https://arxiv.org/abs/2007.03964)
-- [X] **[NeurIPS 2020]** [First Order Constrained Optimization in Policy Space (FOCOPS)](https://arxiv.org/abs/2002.06506)
-- [X] **[AAAI 2020]** [IPO: Interior-point Policy Optimization under Constraints (IPO)](https://arxiv.org/abs/1910.09615)
-- [X] **[ICLR 2020]** [Projection-Based Constrained Policy Optimization (PCPO)](https://openreview.net/forum?id=rke3TJrtPS)
-- [X] **[ICML 2021]** [CRPO: A New Approach for Safe Reinforcement Learning with Convergence Guarantee](https://arxiv.org/abs/2011.05869)
+<summary><b><big>On Policy SafeRL</big></b></summary>
+
+- [x] [The Lagrange version of PPO (PPO-Lag)](https://cdn.openai.com/safexp-short.pdf)
+- [x] [The Lagrange version of TRPO (TRPO-Lag)](https://cdn.openai.com/safexp-short.pdf)
+- [x] **[ICML 2017]** [Constrained Policy Optimization (CPO)](https://proceedings.mlr.press/v70/achiam17a)
+- [x] **[ICLR 2019]** [Reward Constrained Policy Optimization (RCPO)](https://openreview.net/forum?id=SkfrvsA9FX)
+- [x] **[ICML 2020]** [Responsive Safety in Reinforcement Learning by PID Lagrangian Methods (PID-Lag)](https://arxiv.org/abs/2007.03964)
+- [x] **[NeurIPS 2020]** [First Order Constrained Optimization in Policy Space (FOCOPS)](https://arxiv.org/abs/2002.06506)
+- [x] **[AAAI 2020]** [IPO: Interior-point Policy Optimization under Constraints (IPO)](https://arxiv.org/abs/1910.09615)
+- [x] **[ICLR 2020]** [Projection-Based Constrained Policy Optimization (PCPO)](https://openreview.net/forum?id=rke3TJrtPS)
+- [x] **[ICML 2021]** [CRPO: A New Approach for Safe Reinforcement Learning with Convergence Guarantee](https://arxiv.org/abs/2011.05869)
 - [x] **[IJCAI 2022]** [Penalized Proximal Policy Optimization for Safe Reinforcement Learning(P3O)](https://arxiv.org/pdf/2205.11814.pdf)
 
-#### Off-Policy Safe
+<summary><b><big>Off Policy SafeRL</big></b></summary>
 
-- [X] The Lagrange version of TD3 (TD3-Lag)
-- [X] The Lagrange version of DDPG (DDPG-Lag)
-- [X] The Lagrange version of SAC (SAC-Lag)
-- [X] **[ICML 2019]** [Lyapunov-based Safe Policy Optimization for Continuous Control (SDDPG)](https://arxiv.org/abs/1901.10031)
-- [X] **[ICML 2019]** [Lyapunov-based Safe Policy Optimization for Continuous Control (SDDPG-modular)](https://arxiv.org/abs/1901.10031)
-- [ ] **[ICML 2022]** [Constrained Variational Policy Optimization for Safe Reinforcement Learning (CVPO)](https://arxiv.org/abs/2201.11927)
+- **[Preprint 2019]** [The Lagrangian version of DDPG (DDPGLag)](https://cdn.openai.com/safexp-short.pdf)
+- **[Preprint 2019]** [The Lagrangian version of TD3 (TD3Lag)](https://cdn.openai.com/safexp-short.pdf)
+- **[Preprint 2019]** [The Lagrangian version of SAC (SACLag)](https://cdn.openai.com/safexp-short.pdf)
+- **[ICML 2020]** [Responsive Safety in Reinforcement Learning by PID Lagrangian Methods (DDPGPID)](https://arxiv.org/abs/2007.03964)
+- **[ICML 2020]** [Responsive Safety in Reinforcement Learning by PID Lagrangian Methods (TD3PID)](https://arxiv.org/abs/2007.03964)
+- **[ICML 2020]** [Responsive Safety in Reinforcement Learning by PID Lagrangian Methods (SACPID)](https://arxiv.org/abs/2007.03964)
 
-#### Model-Based Safe
+<summary><b><big>Model-Based SafeRL</big></b></summary>
 
 - [ ] **[NeurIPS 2021]** [Safe Reinforcement Learning by Imagining the Near Future (SMBPO)](https://arxiv.org/abs/2202.07789)
-- [X] **[CoRL 2021 (Oral)]** [Learning Off-Policy with Online Planning (SafeLOOP)](https://arxiv.org/abs/2008.10066)
-- [X] **[AAAI 2022]** [Conservative and Adaptive Penalty for Model-Based Safe Reinforcement Learning (CAP)](https://arxiv.org/abs/2112.07701)
-- [X] **[NeurIPS 2022]** [Model-based Safe Deep Reinforcement Learning via a Constrained Proximal Policy Optimization Algorithm](https://arxiv.org/abs/2210.07573)
+- [x] **[CoRL 2021 (Oral)]** [Learning Off-Policy with Online Planning (SafeLOOP)](https://arxiv.org/abs/2008.10066)
+- [x] **[AAAI 2022]** [Conservative and Adaptive Penalty for Model-Based Safe Reinforcement Learning (CAP)](https://arxiv.org/abs/2112.07701)
+- [x] **[NeurIPS 2022]** [Model-based Safe Deep Reinforcement Learning via a Constrained Proximal Policy Optimization Algorithm](https://arxiv.org/abs/2210.07573)
 - [ ] **[ICLR 2022]** [Constrained Policy Optimization via Bayesian World Models (LA-MBDA)](https://arxiv.org/abs/2201.09802)
-- [X] **[ICML 2022 Workshop]** [Constrained Model-based Reinforcement Learning with Robust Cross-Entropy Method (RCE)](https://arxiv.org/abs/2010.07968)
-- [X] **[NeurIPS 2018]** [Constrained Cross-Entropy Method for Safe Reinforcement Learning (CCE)](https://proceedings.neurips.cc/paper/2018/hash/34ffeb359a192eb8174b6854643cc046-Abstract.html)
+- [x] **[ICML 2022 Workshop]** [Constrained Model-based Reinforcement Learning with Robust Cross-Entropy Method (RCE)](https://arxiv.org/abs/2010.07968)
+- [x] **[NeurIPS 2018]** [Constrained Cross-Entropy Method for Safe Reinforcement Learning (CCE)](https://proceedings.neurips.cc/paper/2018/hash/34ffeb359a192eb8174b6854643cc046-Abstract.html)
 
-#### Offline Safe
+<summary><b><big>Offline SafeRL</big></b></summary>
 
-- [X] [The Lagrange version of BCQ (BCQ-Lag)](https://arxiv.org/abs/1812.02900)
-- [X] [The Constrained version of CRR (C-CRR)](https://proceedings.neurips.cc/paper/2020/hash/588cb956d6bbe67078f29f8de420a13d-Abstract.html)
+- [x] [The Lagrange version of BCQ (BCQ-Lag)](https://arxiv.org/abs/1812.02900)
+- [x] [The Constrained version of CRR (C-CRR)](https://proceedings.neurips.cc/paper/2020/hash/588cb956d6bbe67078f29f8de420a13d-Abstract.html)
 - [ ] **[AAAI 2022]** [Constraints Penalized Q-learning for Safe Offline Reinforcement Learning CPQ](https://arxiv.org/abs/2107.09003)
-- [ ] **[ICLR 2022 (Spotlight)]** [COptiDICE: Offline Constrained Reinforcement Learning via Stationary Distribution Correction Estimation](https://arxiv.org/abs/2204.08957?context=cs.AI)
+- [x] **[ICLR 2022 (Spotlight)]** [COptiDICE: Offline Constrained Reinforcement Learning via Stationary Distribution Correction Estimation](https://arxiv.org/abs/2204.08957?context=cs.AI)
 - [ ] **[ICML 2022]** [Constrained Offline Policy Optimization (COPO)](https://proceedings.mlr.press/v162/polosky22a.html)
 
-#### Others
+<summary><b><big>Others</big></b></summary>
 
-- [X] [Safe Exploration in Continuous Action Spaces (Safety Layer)](https://arxiv.org/abs/1801.08757)
 - [ ] **[RA-L 2021]** [Recovery RL: Safe Reinforcement Learning with Learned Recovery Zones](https://arxiv.org/abs/2010.15920)
-- [X] **[ICML 2022]** [Sauté RL: Almost Surely Safe Reinforcement Learning Using State Augmentation (SauteRL)](https://arxiv.org/abs/2202.06558)
-- [X] **[NeurIPS 2022]** [Effects of Safety State Augmentation on Safe Exploration](https://arxiv.org/abs/2206.02675)
-
---------------------------------------------------------------------------------
-
-## Installation
-
-### Prerequisites
-
-OmniSafe requires Python 3.8+ and PyTorch 1.10+.
-
-> We support and test for Python 3.8, 3.9, 3.10 on Linux. Meanwhile, we also support M1 and M2 versions of macOS. We will accept PRs related to Windows, but do not officially support it.
-
-#### Install from source
-
-```bash
-# Clone the repo
-git clone https://github.com/OmniSafeAI/omnisafe
-cd omnisafe
-
-# Create a conda environment
-conda env create --file conda-recipe.yaml
-conda activate omnisafe
+- [x] **[ICML 2022]** [Sauté RL: Almost Surely Safe Reinforcement Learning Using State Augmentation (SauteRL)](https://arxiv.org/abs/2202.06558)
+- [x] **[NeurIPS 2022]** [Effects of Safety State Augmentation on Safe Exploration](https://arxiv.org/abs/2206.02675)
 
-# Install omnisafe
-pip install -e .
-```
-
-#### Install from PyPI
-
-OmniSafe is hosted in [![PyPI](https://img.shields.io/pypi/v/omnisafe?label=pypi&logo=pypi)](https://pypi.org/project/omnisafe) / ![Status](https://img.shields.io/pypi/status/omnisafe?label=status).
+</details>
 
-```bash
-pip install omnisafe
-```
+--------------------------------------------------------------------------------
 
 ### Examples
 
 ```bash
 cd examples
-python train_policy.py --algo PPOLag --env-id SafetyPointGoal1-v0 --parallel 1 --total-steps 1024000 --device cpu --vector-env-nums 1 --torch-threads 1
+python train_policy.py --algo PPOLag --env-id SafetyPointGoal1-v0 --parallel 1 --total-steps 10000000 --device cpu --vector-env-nums 1 --torch-threads 1
 ```
 
-**algo:**
-| Type              | Name                                                             |
-| ----------------- | ---------------------------------------------------------------- |
-| `Base-On-Policy`  | `PolicyGradient, PPO`<br> `NaturalPG, TRPO`                      |
-| `Base-Off-Policy` | `DDPG, TD3, SAC`                                                 |
-| `Naive Lagrange`  | `RCPO, PPOLag, TRPOLag`<br> `DDPGLag, TD3Lag, SACLag`            |
-| `PID Lagrange`    | `CPPOPid, TRPOPid`                                               |
-| `First Order`     | `FOCOPS, CUP`                                                    |
-| `Second Order`    | `SDDPG, CPO, PCPO`                                               |
-| `Saute RL`        | `PPOSaute, PPOLagSaute`                                          |
-| `Simmer RL`       | `PPOSimmerQ, PPOSimmerPid` <br> `PPOLagSimmerQ, PPOLagSimmerPid` |
-| `EarlyTerminated` | `PPOEarlyTerminated` <br> `PPOLagEarlyTerminated`                |
-| `Model-Based`     | `CAP, MBPPOLag, SafeLOOP`                                        |
+#### Algorithms Registry
+
+<table>
+<thead>
+  <tr>
+    <th>Domains</th>
+    <th>Types</th>
+    <th>Algorithms Registry</th>
+  </tr>
+</thead>
+<tbody>
+  <tr>
+    <td rowspan="5">On Policy</td>
+    <td rowspan="2">Primal Dual</td>
+    <td>TRPOLag; PPOLag; PDO; RCPO</td>
+  </tr>
+  <tr>
+    <td>TRPOPID; CPPOPID</td>
+  </tr>
+  <tr>
+    <td>Convex Optimization</td>
+    <td><span style="font-weight:400;font-style:normal">CPO; PCPO; </span>FOCOPS; CUP</td>
+  </tr>
+  <tr>
+    <td>Penalty Function</td>
+    <td>IPO; P3O</td>
+  </tr>
+  <tr>
+    <td>Primal</td>
+    <td>OnCRPO</td>
+  </tr>
+  <tr>
+    <td rowspan="2">Off Policy</td>
+    <td rowspan="2">Primal-Dual</td>
+    <td>DDPGLag; TD3Lag; SACLag</td>
+  </tr>
+  <tr>
+    <td><span style="font-weight:400;font-style:normal">DDPGPID; TD3PID; SACPID</span></td>
+  </tr>
+  <tr>
+    <td rowspan="2">Model-based</td>
+    <td>Online Plan</td>
+    <td>SafeLOOP; CCEPETS; RCEPETS</td>
+  </tr>
+  <tr>
+    <td><span style="font-weight:400;font-style:normal">Pessimistic Estimate</span></td>
+    <td>CAPPETS</td>
+  </tr>
+    <td rowspan="2">Offline</td>
+    <td>Q-Learning Based</td>
+    <td>BCQLag; C-CRR</td>
+  </tr>
+  <tr>
+    <td>DICE Based</td>
+    <td>COptDICE</td>
+  </tr>
+  <tr>
+    <td rowspan="3">Other Formulation MDP</td>
+    <td>ET-MDP</td>
+    <td><span style="font-weight:400;font-style:normal">PPO</span>EarlyTerminated; TRPOEarlyTerminated</td>
+  </tr>
+  <tr>
+    <td>SauteRL</td>
+    <td>PPOSaute; TRPOSaute</td>
+  </tr>
+  <tr>
+    <td>SimmerRL</td>
+    <td><span style="font-weight:400;font-style:normal">PPOSimmerPID; TRPOSimmerPID</span></td>
+  </tr>
+</tbody>
+</table>
+
+#### Supported Environments
 
-**env-id:** Environment id in [Safety Gymnasium](https://www.safety-gymnasium.com/), here a list of envs that safety-gymnasium supports.
+Here is a list of environments that [Safety-Gymnasium](https://www.safety-gymnasium.com) supports:
 
 <table border="1">
 <thead>
   <tr>
     <th>Category</th>
     <th>Task</th>
     <th>Agent</th>
@@ -218,72 +311,91 @@
     <td>Velocity</td>
     <td>HalfCheetah, Hopper, Swimmer, Walker2d, Ant, Humanoid</td>
     <td>SafetyHumanoidVelocity-v1</td>
   </tr>
 </tbody>
 </table>
 
-More information about environments, please refer to [Safety Gymnasium](https://www.safety-gymnasium.com/)
-
-**parallel:** `Number of parallels`
+For more information about environments, please refer to [Safety-Gymnasium](https://www.safety-gymnasium.com).
 
 #### Try with CLI
 
-**A video example**
-
-![Segmentfault](https://github.com/OmniSafeAI/omnisafe/blob/main/images/CLI_example.svg)
-
 ```bash
 pip install omnisafe
 
-omnisafe --help # Ask for help
-
-omnisafe benchmark --help # The benchmark also can be replaced with 'eval', 'train', 'train-config'
+omnisafe --help  # Ask for help
 
-# Quick benchmarking for your research, just specify: 1.exp_name, 2.num_pool(how much processes are concurrent), 3.path of the config file(refer to omnisafe/examples/benchmarks for format)
-omnisafe benchmark test_benchmark 2 ./saved_source/benchmark_config.yaml
+omnisafe benchmark --help  # The benchmark also can be replaced with 'eval', 'train', 'train-config'
 
-# Quick evaluating and rendering your trained policy, just specify: 1.path of algorithm which you trained
-omnisafe eval ./saved_source/PPO-{SafetyPointGoal1-v0} --num-episode 1
+# Quick benchmarking for your research, just specify:
+# 1. exp_name
+# 2. num_pool(how much processes are concurrent)
+# 3. path of the config file (refer to omnisafe/examples/benchmarks for format)
+
+# Here we provide an exampe in ./tests/saved_source.
+# And you can set your benchmark_config.yaml by following it
+omnisafe benchmark test_benchmark 2 ./tests/saved_source/benchmark_config.yaml
+
+# Quick evaluating and rendering your trained policy, just specify:
+# 1. path of algorithm which you trained
+omnisafe eval ./tests/saved_source/PPO-{SafetyPointGoal1-v0} --num-episode 1
 
 # Quick training some algorithms to validate your thoughts
 # Note: use `key1:key2`, your can select key of hyperparameters which are recursively contained, and use `--custom-cfgs`, you can add custom cfgs via CLI
 omnisafe train --algo PPO --total-steps 2048 --vector-env-nums 1 --custom-cfgs algo_cfgs:steps_per_epoch --custom-cfgs 1024
 
 # Quick training some algorithms via a saved config file, the format is as same as default format
-omnisafe train-config ./saved_source/train_config.yaml
+omnisafe train-config ./tests/saved_source/train_config.yaml
 ```
 
 --------------------------------------------------------------------------------
 
 ## Getting Started
 
 ### Important Hints
 
-- `train_cfgs:torch_threads` is especially important for training speed, and is varying with users' machine, this value shouldn't be too small or too large.
+We have provided benchmark results for various algorithms, including on-policy, off-policy, model-based, and offline approaches, along with parameter tuning analysis. Please refer to the following:
+
+- [On-Policy](./benchmarks/on-policy/)
+- [Off-Policy](./benchmarks/off-policy/)
+- [Model-based](./benchmarks/model-based/)
+- [Offline](./benchmarks/offline/)
 
 ### Quickstart: Colab on the Cloud
 
-Explore OmniSafe easily and quickly through a series of colab notebooks:
+Explore OmniSafe easily and quickly through a series of Google Colab notebooks:
 
-- [Getting Started](https://colab.research.google.com/github/OmniSafeAI/omnisafe/blob/main/tutorials/English/1.Getting_Started.ipynb) Introduce the basic usage of OmniSafe so that users can quickly hand on it.
-- [CLI Command](https://colab.research.google.com/github/OmniSafeAI/omnisafe/blob/main/tutorials/English/2.CLI_Command.ipynb) Introduce how to use the CLI tool of OmniSafe.
+- [Getting Started](https://colab.research.google.com/github/PKU-Alignment/omnisafe/blob/main/tutorials/English/1.Getting_Started.ipynb) Introduce the basic usage of OmniSafe so that users can quickly hand it.
+- [CLI Command](https://colab.research.google.com/github/PKU-Alignment/omnisafe/blob/main/tutorials/English/2.CLI_Command.ipynb) Introduce how to use the CLI tool of OmniSafe.
 
 We take great pleasure in collaborating with our users to create tutorials in various languages.
 Please refer to our list of currently supported languages.
 If you are interested in translating the tutorial into a new language or improving an existing version, kindly submit a PR to us.
 
 --------------------------------------------------------------------------------
 
 ## Changelog
 
-See [CHANGELOG.md](https://github.com/OmniSafeAI/omnisafe/blob/main/CHANGELOG.md).
+See [CHANGELOG.md](https://github.com/PKU-Alignment/omnisafe/blob/main/CHANGELOG.md).
+
+## Citing OmniSafe
+
+If you find OmniSafe useful or use OmniSafe in your research, please cite it in your publications.
+
+```bibtex
+@article{omnisafe,
+  title   = {OmniSafe: An Infrastructure for Accelerating Safe Reinforcement Learning Research},
+  author  = {Jiaming Ji, Jiayi Zhou, Borong Zhang, Juntao Dai, Xuehai Pan, Ruiyang Sun, Weidong Huang, Yiran Geng, Mickel Liu, Yaodong Yang},
+  journal = {arXiv preprint arXiv:2305.09304},
+  year    = {2023}
+}
+```
 
 ## The OmniSafe Team
 
-OmniSafe is mainly developed by the SafeRL research team directed by Prof. [Yaodong Yang](https://github.com/orgs/OmniSafeAI/people/PKU-YYang).
+OmniSafe is mainly developed by the SafeRL research team directed by Prof. [Yaodong Yang](https://www.yangyaodong.com/).
 Our SafeRL research team members include [Borong Zhang](https://github.com/muchvo), [Jiayi Zhou](https://github.com/Gaiejj), [JTao Dai](https://github.com/calico-1226), [Weidong Huang](https://github.com/hdadong), [Ruiyang Sun](https://github.com/rockmagma02), [Xuehai Pan](https://github.com/XuehaiPan) and [Jiaming Ji](https://github.com/zmsn-2077).
-If you have any questions in the process of using omnisafe, don't hesitate to ask your questions on [the GitHub issue page](https://github.com/OmniSafeAI/omnisafe/issues/new/choose), we will reply to you in 2-3 working days.
+If you have any questions in the process of using OmniSafe, don't hesitate to ask your questions on [the GitHub issue page](https://github.com/PKU-Alignment/omnisafe/issues/new/choose), we will reply to you in 2-3 working days.
 
 ## License
 
 OmniSafe is released under Apache License 2.0.
```

#### html2text {}

```diff
@@ -1,201 +1,241 @@
-       [https://github.com/OmniSafeAI/omnisafe/raw/HEAD/images/logo.png]
-[![Organization](https://img.shields.io/badge/Organization-PKU_MARL-blue.svg)]
-    (https://github.com/OmniSafeAI) [![PyPI](https://img.shields.io/pypi/v/
-  omnisafe?logo=pypi)](https://pypi.org/project/omnisafe) [![tests](https://
-      img.shields.io/github/actions/workflow/status/OmniSafeAI/omnisafe/
-test.yml?label=tests&logo=github)](https://github.com/OmniSafeAI/omnisafe/tree/
-   HEAD/tests) [![Documentation Status](https://img.shields.io/readthedocs/
+Metadata-Version: 2.1 Name: omnisafe Version: 0.5.0b0 Summary: A comprehensive
+and reliable benchmark for safe reinforcement learning. Author: OmniSafe
+Contributors License: Apache License, Version 2.0 Project-URL: Homepage, https:
+//github.com/PKU-Alignment/omnisafe Project-URL: Repository, https://
+github.com/PKU-Alignment/omnisafe Project-URL: Documentation, https://
+omnisafe.readthedocs.io Project-URL: Bug Report, https://github.com/PKU-
+Alignment/omnisafe/issues Keywords: Safe Reinforcement Learning,Reinforcement
+Learning,PyTorch Classifier: Development Status :: 4 - Beta Classifier: License
+:: OSI Approved :: Apache Software License Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Intended Audience :: Science/Research Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Requires-Python: >=3.8 Description-
+Content-Type: text/markdown Provides-Extra: lint Provides-Extra: test License-
+File: LICENSE
+     [https://github.com/PKU-Alignment/omnisafe/raw/HEAD/images/logo.png]
+  [![Organization](https://img.shields.io/badge/Organization-PKU--Alignment-
+blue)](https://github.com/PKU-Alignment) [![PyPI](https://img.shields.io/pypi/
+ v/omnisafe?logo=pypi)](https://pypi.org/project/omnisafe) [![tests](https://
+     img.shields.io/github/actions/workflow/status/PKU-Alignment/omnisafe/
+ test.yml?label=tests&logo=github)](https://github.com/PKU-Alignment/omnisafe/
+ tree/HEAD/tests) [![Documentation Status](https://img.shields.io/readthedocs/
   omnisafe?logo=readthedocs)](https://omnisafe.readthedocs.io) [![Downloads]
                  (https://static.pepy.tech/personalized-badge/
  omnisafe?period=total&left_color=grey&right_color=blue&left_text=downloads)]
       (https://pepy.tech/project/omnisafe) [![GitHub Repo Stars](https://
-img.shields.io/github/stars/OmniSafeAI/omnisafe?color=brightgreen&logo=github)]
-  (https://github.com/OmniSafeAI/OmniSafe/stargazers) [![codestyle](https://
- img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/
-     black) [![License](https://img.shields.io/github/license/OmniSafeAI/
-OmniSafe?label=license)](#license) [![CodeCov](https://img.shields.io/codecov/
-  c/github/OmniSafeAI/omnisafe/main?logo=codecov)](https://app.codecov.io/gh/
-   OmniSafeAI/omnisafe) [![Open In Colab](https://colab.research.google.com/
- assets/colab-badge.svg)](https://colab.research.google.com/github/OmniSafeAI/
-                                  omnisafe/)
+                  img.shields.io/github/stars/PKU-Alignment/
+  omnisafe?color=brightgreen&logo=github)](https://github.com/PKU-Alignment/
+ OmniSafe/stargazers) [![codestyle](https://img.shields.io/badge/code%20style-
+     black-000000.svg)](https://github.com/psf/black) [![License](https://
+img.shields.io/github/license/PKU-Alignment/OmniSafe?label=license)](#license)
+  [![CodeCov](https://img.shields.io/codecov/c/github/PKU-Alignment/omnisafe/
+ main?logo=codecov)](https://app.codecov.io/gh/PKU-Alignment/omnisafe) [![Open
+ In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
+           colab.research.google.com/github/PKU-Alignment/omnisafe/)
    _D_o_c_u_m_e_n_t_a_t_i_o_n | _I_m_p_l_e_m_e_n_t_e_d_ _A_l_g_o_r_i_t_h_m_s | _I_n_s_t_a_l_l_a_t_i_o_n | _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d |
                                     _L_i_c_e_n_s_e
 -------------------------------------------------------------------------------
-- **This library is currently under heavy development - if you have suggestions
-on the API or use-cases you'd like to be covered, please open a GitHub issue or
-reach out. We'd love to hear about how you're using the library.** OmniSafe is
-an infrastructural framework designed to accelerate safe reinforcement learning
-(RL) research by providing a comprehensive and reliable benchmark for safe RL
-algorithms. The field of RL has great potential to benefit the society, and
-safety concerns are a significant issue, and RL algorithms have raised concerns
-about unintended harm or unsafe behavior. Safe RL intends to develop algorithms
-that minimize the risk of unintended harm or unsafe behavior, but there is
-currently a lack of commonly recognized safe RL algorithm benchmarks. OmniSafe
-addresses these issues by providing more than 40 experimentally validated
-algorithms and a sound and efficient simulation environment. Researchers can
-use OmniSafe to conduct experiments and verify their ideas, ensuring
-consistency and enabling more efficient development of safe RL algorithms. By
-using OmniSafe as a benchmark, researchers can evaluate the performance of
-their own safe RL algorithms and contribute to the advancement of safe RL
-research. ---------------------------------------------------------------------
------------ ### Table of Contents - [Implemented Algorithms](#implemented-
-algorithms) - [Latest SafeRL Papers](#latest-saferl-papers) - [List of
-Algorithms](#list-of-algorithms) - [On-Policy Safe](#on-policy-safe) - [Off-
-Policy Safe](#off-policy-safe) - [Model-Based Safe](#model-based-safe) -
-[Offline Safe](#offline-safe) - [Others](#others) - [Installation]
-(#installation) - [Prerequisites](#prerequisites) - [Install from source]
-(#install-from-source) - [Install from PyPI](#install-from-pypi) - [Examples]
-(#examples) - [Try with CLI](#try-with-cli) - [Getting Started](#getting-
-started) - [Important Hints](#important-hints) - [Quickstart: Colab on the
-Cloud](#quickstart-colab-on-the-cloud) - [Changelog](#changelog) - [The
-OmniSafe Team](#the-omnisafe-team) - [License](#license) ----------------------
----------------------------------------------------------- ## Implemented
-Algorithms The supported interface algorithms currently include: ### Latest
-SafeRL Papers - **[AAAI 2023]** Augmented Proximal Policy Optimization for Safe
-Reinforcement Learning (APPO) - **[NeurIPS 2022]** [Constrained Update
-Projection Approach to Safe Policy Optimization (CUP)](https://arxiv.org/abs/
-2209.07089) - **[NeurIPS 2022]** [Effects of Safety State Augmentation on Safe
-Exploration (Simmer)](https://arxiv.org/abs/2206.02675) - **[NeurIPS 2022]**
-[Model-based Safe Deep Reinforcement Learning via a Constrained Proximal Policy
-Optimization Algorithm](https://arxiv.org/abs/2210.07573) - **[ICML 2022]**
-[SautÃ© RL: Almost Surely Safe Reinforcement Learning Using State Augmentation
-(SauteRL)](https://arxiv.org/abs/2202.06558) - **[ICML 2022]** [Constrained
-Variational Policy Optimization for Safe Reinforcement Learning (CVPO)](https:/
-/arxiv.org/abs/2201.11927) - **[IJCAI 2022]** [Penalized Proximal Policy
-Optimization for Safe Reinforcement Learning](https://arxiv.org/abs/2205.11814)
-- **[ICLR 2022]** [Constrained Policy Optimization via Bayesian World Models
-(LA-MBDA)](https://arxiv.org/abs/2201.09802) - **[AAAI 2022]** [Conservative
-and Adaptive Penalty for Model-Based Safe Reinforcement Learning (CAP)](https:/
-/arxiv.org/abs/2112.07701) ### List of Algorithms #### On-Policy Safe - [X]
-[The Lagrange version of PPO (PPO-Lag)](https://cdn.openai.com/safexp-
-short.pdf) - [X] [The Lagrange version of TRPO (TRPO-Lag)](https://
-cdn.openai.com/safexp-short.pdf) - [X] **[ICML 2017]** [Constrained Policy
-Optimization (CPO)](https://proceedings.mlr.press/v70/achiam17a) - [X] **[ICLR
-2019]** [Reward Constrained Policy Optimization (RCPO)](https://openreview.net/
-forum?id=SkfrvsA9FX) - [X] **[ICML 2020]** [Responsive Safety in Reinforcement
-Learning by PID Lagrangian Methods (PID-Lag)](https://arxiv.org/abs/2007.03964)
-- [X] **[NeurIPS 2020]** [First Order Constrained Optimization in Policy Space
-(FOCOPS)](https://arxiv.org/abs/2002.06506) - [X] **[AAAI 2020]** [IPO:
-Interior-point Policy Optimization under Constraints (IPO)](https://arxiv.org/
-abs/1910.09615) - [X] **[ICLR 2020]** [Projection-Based Constrained Policy
-Optimization (PCPO)](https://openreview.net/forum?id=rke3TJrtPS) - [X] **[ICML
-2021]** [CRPO: A New Approach for Safe Reinforcement Learning with Convergence
-Guarantee](https://arxiv.org/abs/2011.05869) - [x] **[IJCAI 2022]** [Penalized
-Proximal Policy Optimization for Safe Reinforcement Learning(P3O)](https://
-arxiv.org/pdf/2205.11814.pdf) #### Off-Policy Safe - [X] The Lagrange version
-of TD3 (TD3-Lag) - [X] The Lagrange version of DDPG (DDPG-Lag) - [X] The
-Lagrange version of SAC (SAC-Lag) - [X] **[ICML 2019]** [Lyapunov-based Safe
-Policy Optimization for Continuous Control (SDDPG)](https://arxiv.org/abs/
-1901.10031) - [X] **[ICML 2019]** [Lyapunov-based Safe Policy Optimization for
-Continuous Control (SDDPG-modular)](https://arxiv.org/abs/1901.10031) - [ ] **
-[ICML 2022]** [Constrained Variational Policy Optimization for Safe
-Reinforcement Learning (CVPO)](https://arxiv.org/abs/2201.11927) #### Model-
-Based Safe - [ ] **[NeurIPS 2021]** [Safe Reinforcement Learning by Imagining
-the Near Future (SMBPO)](https://arxiv.org/abs/2202.07789) - [X] **[CoRL 2021
-(Oral)]** [Learning Off-Policy with Online Planning (SafeLOOP)](https://
-arxiv.org/abs/2008.10066) - [X] **[AAAI 2022]** [Conservative and Adaptive
-Penalty for Model-Based Safe Reinforcement Learning (CAP)](https://arxiv.org/
-abs/2112.07701) - [X] **[NeurIPS 2022]** [Model-based Safe Deep Reinforcement
-Learning via a Constrained Proximal Policy Optimization Algorithm](https://
-arxiv.org/abs/2210.07573) - [ ] **[ICLR 2022]** [Constrained Policy
-Optimization via Bayesian World Models (LA-MBDA)](https://arxiv.org/abs/
-2201.09802) - [X] **[ICML 2022 Workshop]** [Constrained Model-based
+- OmniSafe is an infrastructural framework designed to accelerate safe
+reinforcement learning (RL) research. It provides a comprehensive and reliable
+benchmark for safe RL algorithms, and also an out-of-box modular toolkit for
+researchers. SafeRL intends to develop algorithms that minimize the risk of
+unintended harm or unsafe behavior. OmniSafe stands as the inaugural unified
+learning framework in the realm of safe reinforcement learning, aiming to
+foster the Growth of SafeRL Learning Community. The key features of OmniSafe: -
+**Highly Modular Framework.** OmniSafe presents a highly modular framework,
+incorporating an extensive collection of tens of algorithms tailored for safe
+reinforcement learning across diverse domains. This framework is versatile due
+to its abstraction of various algorithm types and well-designed API, using the
+Adapter and Wrapper design components to bridge gaps and enable seamless
+interactions between different components. This design allows for easy
+extension and customization, making it a powerful tool for developers working
+with different types of algorithms. - **High-performance parallel computing
+acceleration.** By harnessing the capabilities of `torch.distributed`, OmniSafe
+accelerates the learning process of algorithms with process parallelism. This
+enables OmniSafe not only to support environment-level asynchronous parallelism
+but also incorporates agent asynchronous learning. This methodology bolsters
+training stability and expedites the training process via the deployment of a
+parallel exploration mechanism. The integration of agent asynchronous learning
+in OmniSafe underscores its commitment to providing a versatile and robust
+platform for advancing SafeRL research. - **Out-of-box toolkits.** OmniSafe
+offers customizable toolkits for tasks like training, benchmarking, analyzing,
+and rendering. [Tutorials](https://github.com/PKU-Alignment/omnisafe#getting-
+started) and user-friendly [APIs](https://omnisafe.readthedocs.io/en/latest/
+baserlapi/on_policy.html) make it easy for beginners and average users, while
+advanced researchers can enhance their efficiency without complex code. ![Train
+video](https://github-production-user-asset-6210df.s3.amazonaws.com/73586554/
+237139607-d1e6f413-aa2c-4f68-b8ee-08a4361493a0.gif) ---------------------------
+----------------------------------------------------- ### Table of Contents -
+[Quick Start](#quick-start) - [Installation](#installation) - [Prerequisites]
+(#prerequisites) - [Install from source](#install-from-source) - [Install from
+PyPI](#install-from-pypi) - [Implemented Algorithms](#implemented-algorithms) -
+[Examples](#examples) - [Algorithms Registry](#algorithms-registry) -
+[Supported Environments](#supported-environments) - [Try with CLI](#try-with-
+cli) - [Getting Started](#getting-started) - [Important Hints](#important-
+hints) - [Quickstart: Colab on the Cloud](#quickstart-colab-on-the-cloud) -
+[Changelog](#changelog) - [Citing OmniSafe](#citing-omnisafe) - [The OmniSafe
+Team](#the-omnisafe-team) - [License](#license) -------------------------------
+------------------------------------------------- ## Quick Start ###
+Installation #### Prerequisites OmniSafe requires Python 3.8+ and PyTorch
+1.10+. > We support and test for Python 3.8, 3.9, 3.10 on Linux. Meanwhile, we
+also support M1 and M2 versions of macOS. We will accept PRs related to
+Windows, but do not officially support it. #### Install from source ```bash #
+Clone the repo git clone https://github.com/PKU-Alignment/omnisafe.git cd
+omnisafe # Create a conda environment conda env create --file conda-recipe.yaml
+conda activate omnisafe # Install omnisafe pip install -e . ``` #### Install
+from PyPI OmniSafe is hosted in [![PyPI](https://img.shields.io/pypi/v/
+omnisafe?label=pypi&logo=pypi)](https://pypi.org/project/omnisafe) / ![Status]
+(https://img.shields.io/pypi/status/omnisafe?label=status). ```bash pip install
+omnisafe ``` ## Implemented Algorithms LLaatteesstt SSaaffeeRRLL PPaappeerrss - **[AAAI 2023]**
+Augmented Proximal Policy Optimization for Safe Reinforcement Learning (APPO) -
+**[NeurIPS 2022]** [Constrained Update Projection Approach to Safe Policy
+Optimization (CUP)](https://arxiv.org/abs/2209.07089) - **[NeurIPS 2022]**
+[Effects of Safety State Augmentation on Safe Exploration (Simmer)](https://
+arxiv.org/abs/2206.02675) - **[NeurIPS 2022]** [Model-based Safe Deep
+Reinforcement Learning via a Constrained Proximal Policy Optimization
+Algorithm](https://arxiv.org/abs/2210.07573) - **[ICML 2022]** [SautÃ© RL:
+Almost Surely Safe Reinforcement Learning Using State Augmentation (SauteRL)]
+(https://arxiv.org/abs/2202.06558) - **[IJCAI 2022]** [Penalized Proximal
+Policy Optimization for Safe Reinforcement Learning](https://arxiv.org/abs/
+2205.11814) - **[AAAI 2022]** [Conservative and Adaptive Penalty for Model-
+Based Safe Reinforcement Learning (CAP)](https://arxiv.org/abs/2112.07701) LLiisstt
+ooff AAllggoorriitthhmmss OOnn PPoolliiccyy SSaaffeeRRLL - [x] [The Lagrange version of PPO (PPO-Lag)]
+(https://cdn.openai.com/safexp-short.pdf) - [x] [The Lagrange version of TRPO
+(TRPO-Lag)](https://cdn.openai.com/safexp-short.pdf) - [x] **[ICML 2017]**
+[Constrained Policy Optimization (CPO)](https://proceedings.mlr.press/v70/
+achiam17a) - [x] **[ICLR 2019]** [Reward Constrained Policy Optimization
+(RCPO)](https://openreview.net/forum?id=SkfrvsA9FX) - [x] **[ICML 2020]**
+[Responsive Safety in Reinforcement Learning by PID Lagrangian Methods (PID-
+Lag)](https://arxiv.org/abs/2007.03964) - [x] **[NeurIPS 2020]** [First Order
+Constrained Optimization in Policy Space (FOCOPS)](https://arxiv.org/abs/
+2002.06506) - [x] **[AAAI 2020]** [IPO: Interior-point Policy Optimization
+under Constraints (IPO)](https://arxiv.org/abs/1910.09615) - [x] **[ICLR
+2020]** [Projection-Based Constrained Policy Optimization (PCPO)](https://
+openreview.net/forum?id=rke3TJrtPS) - [x] **[ICML 2021]** [CRPO: A New Approach
+for Safe Reinforcement Learning with Convergence Guarantee](https://arxiv.org/
+abs/2011.05869) - [x] **[IJCAI 2022]** [Penalized Proximal Policy Optimization
+for Safe Reinforcement Learning(P3O)](https://arxiv.org/pdf/2205.11814.pdf) OOffff
+PPoolliiccyy SSaaffeeRRLL - **[Preprint 2019]** [The Lagrangian version of DDPG (DDPGLag)]
+(https://cdn.openai.com/safexp-short.pdf) - **[Preprint 2019]** [The Lagrangian
+version of TD3 (TD3Lag)](https://cdn.openai.com/safexp-short.pdf) - **[Preprint
+2019]** [The Lagrangian version of SAC (SACLag)](https://cdn.openai.com/safexp-
+short.pdf) - **[ICML 2020]** [Responsive Safety in Reinforcement Learning by
+PID Lagrangian Methods (DDPGPID)](https://arxiv.org/abs/2007.03964) - **[ICML
+2020]** [Responsive Safety in Reinforcement Learning by PID Lagrangian Methods
+(TD3PID)](https://arxiv.org/abs/2007.03964) - **[ICML 2020]** [Responsive
+Safety in Reinforcement Learning by PID Lagrangian Methods (SACPID)](https://
+arxiv.org/abs/2007.03964) MMooddeell--BBaasseedd SSaaffeeRRLL - [ ] **[NeurIPS 2021]** [Safe
+Reinforcement Learning by Imagining the Near Future (SMBPO)](https://arxiv.org/
+abs/2202.07789) - [x] **[CoRL 2021 (Oral)]** [Learning Off-Policy with Online
+Planning (SafeLOOP)](https://arxiv.org/abs/2008.10066) - [x] **[AAAI 2022]**
+[Conservative and Adaptive Penalty for Model-Based Safe Reinforcement Learning
+(CAP)](https://arxiv.org/abs/2112.07701) - [x] **[NeurIPS 2022]** [Model-based
+Safe Deep Reinforcement Learning via a Constrained Proximal Policy Optimization
+Algorithm](https://arxiv.org/abs/2210.07573) - [ ] **[ICLR 2022]** [Constrained
+Policy Optimization via Bayesian World Models (LA-MBDA)](https://arxiv.org/abs/
+2201.09802) - [x] **[ICML 2022 Workshop]** [Constrained Model-based
 Reinforcement Learning with Robust Cross-Entropy Method (RCE)](https://
-arxiv.org/abs/2010.07968) - [X] **[NeurIPS 2018]** [Constrained Cross-Entropy
+arxiv.org/abs/2010.07968) - [x] **[NeurIPS 2018]** [Constrained Cross-Entropy
 Method for Safe Reinforcement Learning (CCE)](https://proceedings.neurips.cc/
-paper/2018/hash/34ffeb359a192eb8174b6854643cc046-Abstract.html) #### Offline
-Safe - [X] [The Lagrange version of BCQ (BCQ-Lag)](https://arxiv.org/abs/
-1812.02900) - [X] [The Constrained version of CRR (C-CRR)](https://
-proceedings.neurips.cc/paper/2020/hash/588cb956d6bbe67078f29f8de420a13d-
-Abstract.html) - [ ] **[AAAI 2022]** [Constraints Penalized Q-learning for Safe
-Offline Reinforcement Learning CPQ](https://arxiv.org/abs/2107.09003) - [ ] **
-[ICLR 2022 (Spotlight)]** [COptiDICE: Offline Constrained Reinforcement
-Learning via Stationary Distribution Correction Estimation](https://arxiv.org/
-abs/2204.08957?context=cs.AI) - [ ] **[ICML 2022]** [Constrained Offline Policy
-Optimization (COPO)](https://proceedings.mlr.press/v162/polosky22a.html) ####
-Others - [X] [Safe Exploration in Continuous Action Spaces (Safety Layer)]
-(https://arxiv.org/abs/1801.08757) - [ ] **[RA-L 2021]** [Recovery RL: Safe
-Reinforcement Learning with Learned Recovery Zones](https://arxiv.org/abs/
-2010.15920) - [X] **[ICML 2022]** [SautÃ© RL: Almost Surely Safe Reinforcement
-Learning Using State Augmentation (SauteRL)](https://arxiv.org/abs/2202.06558)
-- [X] **[NeurIPS 2022]** [Effects of Safety State Augmentation on Safe
-Exploration](https://arxiv.org/abs/2206.02675) --------------------------------
------------------------------------------------- ## Installation ###
-Prerequisites OmniSafe requires Python 3.8+ and PyTorch 1.10+. > We support and
-test for Python 3.8, 3.9, 3.10 on Linux. Meanwhile, we also support M1 and M2
-versions of macOS. We will accept PRs related to Windows, but do not officially
-support it. #### Install from source ```bash # Clone the repo git clone https:/
-/github.com/OmniSafeAI/omnisafe cd omnisafe # Create a conda environment conda
-env create --file conda-recipe.yaml conda activate omnisafe # Install omnisafe
-pip install -e . ``` #### Install from PyPI OmniSafe is hosted in [![PyPI]
-(https://img.shields.io/pypi/v/omnisafe?label=pypi&logo=pypi)](https://
-pypi.org/project/omnisafe) / ![Status](https://img.shields.io/pypi/status/
-omnisafe?label=status). ```bash pip install omnisafe ``` ### Examples ```bash
-cd examples python train_policy.py --algo PPOLag --env-id SafetyPointGoal1-v0 -
--parallel 1 --total-steps 1024000 --device cpu --vector-env-nums 1 --torch-
-threads 1 ``` **algo:** | Type | Name | | ----------------- | -----------------
------------------------------------------------ | | `Base-On-Policy` |
-`PolicyGradient, PPO`
-`NaturalPG, TRPO` | | `Base-Off-Policy` | `DDPG, TD3, SAC` | | `Naive Lagrange`
-| `RCPO, PPOLag, TRPOLag`
-`DDPGLag, TD3Lag, SACLag` | | `PID Lagrange` | `CPPOPid, TRPOPid` | | `First
-Order` | `FOCOPS, CUP` | | `Second Order` | `SDDPG, CPO, PCPO` | | `Saute RL` |
-`PPOSaute, PPOLagSaute` | | `Simmer RL` | `PPOSimmerQ, PPOSimmerPid`
-`PPOLagSimmerQ, PPOLagSimmerPid` | | `EarlyTerminated` | `PPOEarlyTerminated`
-`PPOLagEarlyTerminated` | | `Model-Based` | `CAP, MBPPOLag, SafeLOOP` | **env-
-id:** Environment id in [Safety Gymnasium](https://www.safety-gymnasium.com/),
-here a list of envs that safety-gymnasium supports.
+paper/2018/hash/34ffeb359a192eb8174b6854643cc046-Abstract.html) OOfffflliinnee SSaaffeeRRLL
+- [x] [The Lagrange version of BCQ (BCQ-Lag)](https://arxiv.org/abs/1812.02900)
+- [x] [The Constrained version of CRR (C-CRR)](https://proceedings.neurips.cc/
+paper/2020/hash/588cb956d6bbe67078f29f8de420a13d-Abstract.html) - [ ] **[AAAI
+2022]** [Constraints Penalized Q-learning for Safe Offline Reinforcement
+Learning CPQ](https://arxiv.org/abs/2107.09003) - [x] **[ICLR 2022
+(Spotlight)]** [COptiDICE: Offline Constrained Reinforcement Learning via
+Stationary Distribution Correction Estimation](https://arxiv.org/abs/
+2204.08957?context=cs.AI) - [ ] **[ICML 2022]** [Constrained Offline Policy
+Optimization (COPO)](https://proceedings.mlr.press/v162/polosky22a.html) OOtthheerrss
+- [ ] **[RA-L 2021]** [Recovery RL: Safe Reinforcement Learning with Learned
+Recovery Zones](https://arxiv.org/abs/2010.15920) - [x] **[ICML 2022]** [SautÃ©
+RL: Almost Surely Safe Reinforcement Learning Using State Augmentation
+(SauteRL)](https://arxiv.org/abs/2202.06558) - [x] **[NeurIPS 2022]** [Effects
+of Safety State Augmentation on Safe Exploration](https://arxiv.org/abs/
+2206.02675) -------------------------------------------------------------------
+------------- ### Examples ```bash cd examples python train_policy.py --algo
+PPOLag --env-id SafetyPointGoal1-v0 --parallel 1 --total-steps 10000000 --
+device cpu --vector-env-nums 1 --torch-threads 1 ``` #### Algorithms Registry
+DDoommaaiinnss               TTyyppeess                AAllggoorriitthhmmss RReeggiissttrryy
+                      Primal Dual          TRPOLag; PPOLag; PDO; RCPO
+                                           TRPOPID; CPPOPID
+On Policy             Convex Optimization  CPO; PCPO; FOCOPS; CUP
+                      Penalty Function     IPO; P3O
+                      Primal               OnCRPO
+Off Policy            Primal-Dual          DDPGLag; TD3Lag; SACLag
+                                           DDPGPID; TD3PID; SACPID
+Model-based           Online Plan          SafeLOOP; CCEPETS; RCEPETS
+                      Pessimistic Estimate CAPPETS
+DICE Based            COptDICE
+                      ET-MDP               PPOEarlyTerminated;
+Other Formulation MDP                      TRPOEarlyTerminated
+                      SauteRL              PPOSaute; TRPOSaute
+                      SimmerRL             PPOSimmerPID; TRPOSimmerPID
+#### Supported Environments Here is a list of environments that [Safety-
+Gymnasium](https://www.safety-gymnasium.com) supports:
  _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
 |_CC_aa_tt_ee_gg_oo_rr_yy_ _ _ _ _ _ _ _|_TT_aa_ss_kk_ _ _ _ _ _ _ _|_AA_gg_ee_nn_tt_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_EE_xx_aa_mm_pp_ll_ee_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |               |_G_o_a_l_[_0_1_2_]_ _ |                        |                       |
 |Safe Navigation|_B_u_t_t_o_n_[_0_1_2_]|Point, Car, Racecar, Ant|SafetyPointGoal1-v0    |
 |               |_P_u_s_h_[_0_1_2_]_ _ |                        |                       |
 |_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_C_i_r_c_l_e_[_0_1_2_]_|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |               |           |HalfCheetah, Hopper,    |SafetyHumanoidVelocity-|
 |Safe Velocity  |Velocity   |Swimmer, Walker2d, Ant, |v1                     |
 |_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _|_H_u_m_a_n_o_i_d_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
-More information about environments, please refer to [Safety Gymnasium](https:/
-/www.safety-gymnasium.com/) **parallel:** `Number of parallels` #### Try with
-CLI **A video example** ![Segmentfault](https://github.com/OmniSafeAI/omnisafe/
-blob/main/images/CLI_example.svg) ```bash pip install omnisafe omnisafe --help
-# Ask for help omnisafe benchmark --help # The benchmark also can be replaced
-with 'eval', 'train', 'train-config' # Quick benchmarking for your research,
-just specify: 1.exp_name, 2.num_pool(how much processes are concurrent), 3.path
-of the config file(refer to omnisafe/examples/benchmarks for format) omnisafe
-benchmark test_benchmark 2 ./saved_source/benchmark_config.yaml # Quick
-evaluating and rendering your trained policy, just specify: 1.path of algorithm
-which you trained omnisafe eval ./saved_source/PPO-{SafetyPointGoal1-v0} --num-
-episode 1 # Quick training some algorithms to validate your thoughts # Note:
-use `key1:key2`, your can select key of hyperparameters which are recursively
-contained, and use `--custom-cfgs`, you can add custom cfgs via CLI omnisafe
-train --algo PPO --total-steps 2048 --vector-env-nums 1 --custom-cfgs
-algo_cfgs:steps_per_epoch --custom-cfgs 1024 # Quick training some algorithms
-via a saved config file, the format is as same as default format omnisafe
-train-config ./saved_source/train_config.yaml ``` -----------------------------
---------------------------------------------------- ## Getting Started ###
-Important Hints - `train_cfgs:torch_threads` is especially important for
-training speed, and is varying with users' machine, this value shouldn't be too
-small or too large. ### Quickstart: Colab on the Cloud Explore OmniSafe easily
-and quickly through a series of colab notebooks: - [Getting Started](https://
-colab.research.google.com/github/OmniSafeAI/omnisafe/blob/main/tutorials/
-English/1.Getting_Started.ipynb) Introduce the basic usage of OmniSafe so that
-users can quickly hand on it. - [CLI Command](https://
-colab.research.google.com/github/OmniSafeAI/omnisafe/blob/main/tutorials/
+For more information about environments, please refer to [Safety-Gymnasium]
+(https://www.safety-gymnasium.com). #### Try with CLI ```bash pip install
+omnisafe omnisafe --help # Ask for help omnisafe benchmark --help # The
+benchmark also can be replaced with 'eval', 'train', 'train-config' # Quick
+benchmarking for your research, just specify: # 1. exp_name # 2. num_pool(how
+much processes are concurrent) # 3. path of the config file (refer to omnisafe/
+examples/benchmarks for format) # Here we provide an exampe in ./tests/
+saved_source. # And you can set your benchmark_config.yaml by following it
+omnisafe benchmark test_benchmark 2 ./tests/saved_source/benchmark_config.yaml
+# Quick evaluating and rendering your trained policy, just specify: # 1. path
+of algorithm which you trained omnisafe eval ./tests/saved_source/PPO-
+{SafetyPointGoal1-v0} --num-episode 1 # Quick training some algorithms to
+validate your thoughts # Note: use `key1:key2`, your can select key of
+hyperparameters which are recursively contained, and use `--custom-cfgs`, you
+can add custom cfgs via CLI omnisafe train --algo PPO --total-steps 2048 --
+vector-env-nums 1 --custom-cfgs algo_cfgs:steps_per_epoch --custom-cfgs 1024 #
+Quick training some algorithms via a saved config file, the format is as same
+as default format omnisafe train-config ./tests/saved_source/train_config.yaml
+``` ---------------------------------------------------------------------------
+----- ## Getting Started ### Important Hints We have provided benchmark results
+for various algorithms, including on-policy, off-policy, model-based, and
+offline approaches, along with parameter tuning analysis. Please refer to the
+following: - [On-Policy](./benchmarks/on-policy/) - [Off-Policy](./benchmarks/
+off-policy/) - [Model-based](./benchmarks/model-based/) - [Offline](./
+benchmarks/offline/) ### Quickstart: Colab on the Cloud Explore OmniSafe easily
+and quickly through a series of Google Colab notebooks: - [Getting Started]
+(https://colab.research.google.com/github/PKU-Alignment/omnisafe/blob/main/
+tutorials/English/1.Getting_Started.ipynb) Introduce the basic usage of
+OmniSafe so that users can quickly hand it. - [CLI Command](https://
+colab.research.google.com/github/PKU-Alignment/omnisafe/blob/main/tutorials/
 English/2.CLI_Command.ipynb) Introduce how to use the CLI tool of OmniSafe. We
 take great pleasure in collaborating with our users to create tutorials in
 various languages. Please refer to our list of currently supported languages.
 If you are interested in translating the tutorial into a new language or
 improving an existing version, kindly submit a PR to us. ----------------------
 ---------------------------------------------------------- ## Changelog See
-[CHANGELOG.md](https://github.com/OmniSafeAI/omnisafe/blob/main/CHANGELOG.md).
-## The OmniSafe Team OmniSafe is mainly developed by the SafeRL research team
-directed by Prof. [Yaodong Yang](https://github.com/orgs/OmniSafeAI/people/PKU-
-YYang). Our SafeRL research team members include [Borong Zhang](https://
-github.com/muchvo), [Jiayi Zhou](https://github.com/Gaiejj), [JTao Dai](https:/
-/github.com/calico-1226), [Weidong Huang](https://github.com/hdadong), [Ruiyang
-Sun](https://github.com/rockmagma02), [Xuehai Pan](https://github.com/
-XuehaiPan) and [Jiaming Ji](https://github.com/zmsn-2077). If you have any
-questions in the process of using omnisafe, don't hesitate to ask your
-questions on [the GitHub issue page](https://github.com/OmniSafeAI/omnisafe/
-issues/new/choose), we will reply to you in 2-3 working days. ## License
-OmniSafe is released under Apache License 2.0.
+[CHANGELOG.md](https://github.com/PKU-Alignment/omnisafe/blob/main/
+CHANGELOG.md). ## Citing OmniSafe If you find OmniSafe useful or use OmniSafe
+in your research, please cite it in your publications. ```bibtex @article
+{omnisafe, title = {OmniSafe: An Infrastructure for Accelerating Safe
+Reinforcement Learning Research}, author = {Jiaming Ji, Jiayi Zhou, Borong
+Zhang, Juntao Dai, Xuehai Pan, Ruiyang Sun, Weidong Huang, Yiran Geng, Mickel
+Liu, Yaodong Yang}, journal = {arXiv preprint arXiv:2305.09304}, year = {2023}
+} ``` ## The OmniSafe Team OmniSafe is mainly developed by the SafeRL research
+team directed by Prof. [Yaodong Yang](https://www.yangyaodong.com/). Our SafeRL
+research team members include [Borong Zhang](https://github.com/muchvo), [Jiayi
+Zhou](https://github.com/Gaiejj), [JTao Dai](https://github.com/calico-1226),
+[Weidong Huang](https://github.com/hdadong), [Ruiyang Sun](https://github.com/
+rockmagma02), [Xuehai Pan](https://github.com/XuehaiPan) and [Jiaming Ji]
+(https://github.com/zmsn-2077). If you have any questions in the process of
+using OmniSafe, don't hesitate to ask your questions on [the GitHub issue page]
+(https://github.com/PKU-Alignment/omnisafe/issues/new/choose), we will reply to
+you in 2-3 working days. ## License OmniSafe is released under Apache License
+2.0.
```

### Comparing `omnisafe-0.4.0/omnisafe/__init__.py` & `omnisafe-0.5.0b0/omnisafe/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/adapter/__init__.py` & `omnisafe-0.5.0b0/omnisafe/adapter/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,11 +12,13 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Adapter for the environment and the algorithm."""
 
 from omnisafe.adapter.early_terminated_adapter import EarlyTerminatedAdapter
 from omnisafe.adapter.modelbased_adapter import ModelBasedAdapter
+from omnisafe.adapter.offline_adapter import OfflineAdapter
 from omnisafe.adapter.offpolicy_adapter import OffPolicyAdapter
 from omnisafe.adapter.online_adapter import OnlineAdapter
 from omnisafe.adapter.onpolicy_adapter import OnPolicyAdapter
 from omnisafe.adapter.saute_adapter import SauteAdapter
+from omnisafe.adapter.simmer_adapter import SimmerAdapter
```

### Comparing `omnisafe-0.4.0/omnisafe/adapter/early_terminated_adapter.py` & `omnisafe-0.5.0b0/omnisafe/adapter/early_terminated_adapter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -40,15 +40,15 @@
     def __init__(self, env_id: str, num_envs: int, seed: int, cfgs: Config) -> None:
         """Initialize an instance of :class:`EarlyTerminatedAdapter`."""
         assert num_envs == 1, 'EarlyTerminatedAdapter only supports num_envs=1.'
 
         super().__init__(env_id, num_envs, seed, cfgs)
 
         self._cost_limit: float = cfgs.algo_cfgs.cost_limit
-        self._cost_logger: torch.Tensor = torch.zeros(self._env.num_envs)
+        self._cost_logger: torch.Tensor = torch.zeros(self._env.num_envs).to(self._device)
 
     def step(
         self,
         action: torch.Tensor,
     ) -> tuple[
         torch.Tensor,
         torch.Tensor,
@@ -75,13 +75,13 @@
             info: Some information logged by the environment.
         """
         next_obs, reward, cost, terminated, truncated, info = super().step(action)
 
         self._cost_logger += info.get('original_cost', cost)
 
         if self._cost_logger > self._cost_limit:
-            reward = torch.zeros(self._env.num_envs)
-            terminated = torch.ones(self._env.num_envs)
+            reward = torch.zeros(self._env.num_envs).to(self._device)
+            terminated = torch.ones(self._env.num_envs).to(self._device)
             next_obs, _ = self._env.reset()
-            self._cost_logger = torch.zeros(self._env.num_envs)
+            self._cost_logger = torch.zeros(self._env.num_envs).to(self._device)
 
         return next_obs, reward, cost, terminated, truncated, info
```

### Comparing `omnisafe-0.4.0/omnisafe/adapter/modelbased_adapter.py` & `omnisafe-0.5.0b0/omnisafe/adapter/modelbased_adapter.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,160 +9,167 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Model-based Adapter for OmniSafe."""
+
+
 from __future__ import annotations
 
 import time
 from typing import Any, Callable
 
+import numpy as np
 import torch
+from gymnasium.spaces import Box
 
 from omnisafe.adapter.online_adapter import OnlineAdapter
 from omnisafe.common.logger import Logger
-from omnisafe.envs.core import make, support_envs
+from omnisafe.envs.core import CMDP, make, support_envs
 from omnisafe.envs.wrapper import (
     ActionRepeat,
     ActionScale,
     AutoReset,
     CostNormalize,
     ObsNormalize,
     RewardNormalize,
     TimeLimit,
     Unsqueeze,
 )
 from omnisafe.utils.config import Config
+from omnisafe.utils.tools import get_device
 
 
 class ModelBasedAdapter(
     OnlineAdapter,
 ):  # pylint: disable=too-many-instance-attributes,super-init-not-called
     """Model Based Adapter for OmniSafe.
 
     :class:`ModelBasedAdapter` is used to adapt the environment to the model-based training.
-
+    It trains a world model to provide data for algorithms training.
 
     Args:
         env_id (str): The environment id.
         num_envs (int): The number of environments.
         seed (int): The random seed.
         cfgs (Config): The configuration.
-        kwargs(dict): The other keyword arguments.
+
+    Keyword Args:
+        render_mode (str, optional): The render mode ranges from 'human' to 'rgb_array' and 'rgb_array_list'.
+            Defaults to 'rgb_array'.
+        camera_name (str, optional): The camera name.
+        camera_id (int, optional): The camera id.
+        width (int, optional): The width of the rendered image. Defaults to 256.
+        height (int, optional): The height of the rendered image. Defaults to 256.
 
     Attributes:
-        _env_id (str): The environment id.
-        _device (torch.device): The device.
-        _env (CMDP): The environment.
-        _cfgs (Config): The configuration.
-        _ep_ret (torch.Tensor): The episode return.
-        _ep_cost (torch.Tensor): The episode cost.
-        _ep_len (torch.Tensor): The episode length.
-        _last_dynamics_update (float): The last time of dynamics update.
-        _last_policy_update (float): The last time of policy update.
-        _last_eval (float): The last time of evaluation.
         coordinate_observation_space (OmnisafeSpace): The coordinate observation space.
         lidar_observation_space (OmnisafeSpace): The lidar observation space.
         task (str): The task. eg. The task of SafetyPointGoal-v0 is 'goal'
     """
 
+    coordinate_observation_space: Box | None
+    lidar_observation_space: Box | None
+    task: str | None
+    _ep_ret: torch.Tensor
+    _ep_cost: torch.Tensor
+    _ep_len: torch.Tensor
+    _current_obs: torch.Tensor
+
     def __init__(  # pylint: disable=too-many-arguments
         self,
         env_id: str,
         num_envs: int,
         seed: int,
         cfgs: Config,
-        **kwargs: Any,
+        **env_kwargs: Any,
     ) -> None:
         """Initialize the model-based adapter."""
         assert env_id in support_envs(), f'Env {env_id} is not supported.'
 
-        self._env_id = env_id
-        self._device = cfgs.train_cfgs.device
+        self._env_id: str = env_id
+        self._device: torch.device = get_device(cfgs.train_cfgs.device)
 
-        self._env = make(env_id, num_envs=num_envs, device=cfgs.train_cfgs.device, **kwargs)
+        self._env: CMDP = make(
+            env_id,
+            num_envs=num_envs,
+            device=cfgs.train_cfgs.device,
+            **env_kwargs,
+        )
 
         # wrap the environment, use the action repeat in model-based setting.
         self._wrapper(
             obs_normalize=cfgs.algo_cfgs.obs_normalize,
             reward_normalize=cfgs.algo_cfgs.reward_normalize,
             cost_normalize=cfgs.algo_cfgs.cost_normalize,
             action_repeat=cfgs.algo_cfgs.action_repeat,
         )
         self._env.set_seed(seed)
-        self._cfgs = cfgs
+        self._cfgs: Config = cfgs
         if hasattr(self._env, 'coordinate_observation_space') and hasattr(
             self._env,
             'lidar_observation_space',
         ):
             self.coordinate_observation_space = self._env.coordinate_observation_space
             self.lidar_observation_space = self._env.lidar_observation_space
         else:
             self.coordinate_observation_space = None
             self.lidar_observation_space = None
         if hasattr(self._env, 'task'):
             self.task = self._env.task
         else:
             self.task = None
 
-        self._ep_ret: torch.Tensor
-        self._ep_cost: torch.Tensor
-        self._ep_len: torch.Tensor
         self._current_obs, _ = self.reset()
-        self._max_ep_len = 1000
+        self._max_ep_len: int = 1000
         self._reset_log()
-        self._last_dynamics_update = 0
-        self._last_policy_update = 0
-        self._last_eval = 0
-        self._first_log = False
-
-    def get_goal_flag_from_obs_tensor(self, obs: torch.Tensor) -> torch.Tensor | None:
-        """Get goal flag from tensor observation.
+        self._last_dynamics_update: int = 0
+        self._last_policy_update: int = 0
+        self._last_eval: int = 0
+        self._first_log: bool = False
 
-        Args:
-            obs (torch.Tensor): The observation.
-        """
-        return (
-            self._env.get_goal_flag_from_obs_tensor(obs)
-            if hasattr(self._env, 'get_goal_flag_from_obs_tensor')
-            else None
-        )
-
-    def get_cost_from_obs_tensor(self, obs: torch.Tensor) -> torch.Tensor | None:
+    def get_cost_from_obs_tensor(self, obs: torch.Tensor) -> torch.Tensor:
         """Get cost from tensor observation.
 
         Args:
-            obs (torch.Tensor): The observation.
+            obs (torch.Tensor): The tensor version of observation.
         """
         return (
             self._env.get_cost_from_obs_tensor(obs)
             if hasattr(self._env, 'get_cost_from_obs_tensor')
-            else None
+            else torch.zeros(1)
         )
 
-    def get_lidar_from_coordinate(self, obs: torch.Tensor) -> torch.Tensor | None:
+    def get_lidar_from_coordinate(self, obs: np.ndarray) -> torch.Tensor | None:
         """Get lidar from numpy coordinate.
 
         Args:
             obs (np.ndarray): The observation.
         """
         return (
             self._env.get_lidar_from_coordinate(obs)
             if hasattr(self._env, 'get_lidar_from_coordinate')
             else None
         )
 
-    def render(self, *args: str, **kwargs: int) -> Any:
+    def render(self, *args: str, **kwargs: Any) -> Any:
         """Render the environment.
 
         Args:
             args (str): The arguments.
-            kwargs (int): The keyword arguments.
+
+        Keyword Args:
+            render_mode (str, optional): The render mode, ranging from ``human``, ``rgb_array``, ``rgb_array_list``.
+                Defaults to ``rgb_array``.
+            camera_name (str, optional): The camera name.
+            camera_id (int, optional): The camera id.
+            width (int, optional): The width of the rendered image. Defaults to 256.
+            height (int, optional): The height of the rendered image. Defaults to 256.
         """
         return self._env.render(*args, **kwargs)
 
     def _wrapper(
         self,
         obs_normalize: bool = True,
         reward_normalize: bool = True,
@@ -171,34 +178,33 @@
     ) -> None:
         """Wrapper the environment.
 
         .. hint::
 
             OmniSafe supports the following wrappers:
 
-            .. list-table::
-
-                *   -   Wrapper
-                    -   Description
-                *   -   TimeLimit
-                    -   Limit the time steps of the environment.
-                *   -   AutoReset
-                    -   Reset the environment when the episode is done.
-                *   -   ObsNormalize
-                    -   Normalize the observation.
-                *   -   RewardNormalize
-                    -   Normalize the reward.
-                *   -   CostNormalize
-                    -   Normalize the cost.
-                *   -   ActionScale
-                    -   Scale the action.
-                *   -   ActionRepeat
-                    -   Repeat the action.
-                *   -   Unsqueeze
-                    -   Unsqueeze the step result for single environment case.
+            +-----------------+--------------------------------------------------------+
+            | Wrapper         | Description                                            |
+            +=================+========================================================+
+            | TimeLimit       | Limit the time steps of the environment.               |
+            +-----------------+--------------------------------------------------------+
+            | AutoReset       | Reset the environment when the episode is done.        |
+            +-----------------+--------------------------------------------------------+
+            | ObsNormalize    | Normalize the observation.                             |
+            +-----------------+--------------------------------------------------------+
+            | RewardNormalize | Normalize the reward.                                  |
+            +-----------------+--------------------------------------------------------+
+            | CostNormalize   | Normalize the cost.                                    |
+            +-----------------+--------------------------------------------------------+
+            | ActionScale     | Scale the action.                                      |
+            +-----------------+--------------------------------------------------------+
+            | ActionRepeat    | Repeat the action.                                     |
+            +-----------------+--------------------------------------------------------+
+            | Unsqueeze       | Unsqueeze the step result for single environment case. |
+            +-----------------+--------------------------------------------------------+
 
         Args:
             obs_normalize (bool): Whether to normalize the observation.
             reward_normalize (bool): Whether to normalize the reward.
             cost_normalize (bool): Whether to normalize the cost.
             action_repeat (int): The action repeat times.
         """
@@ -214,87 +220,96 @@
             self._env = CostNormalize(self._env, device=self._device)
         self._env = ActionScale(self._env, device=self._device, low=-1.0, high=1.0)
         self._env = ActionRepeat(self._env, times=action_repeat, device=self._device)
 
         if self._env.num_envs == 1:
             self._env = Unsqueeze(self._env, device=self._device)
 
-    def roll_out(  # pylint: disable=too-many-arguments,too-many-locals
+    def rollout(  # pylint: disable=too-many-arguments,too-many-locals
         self,
         current_step: int,
-        roll_out_step: int,
+        rollout_step: int,
         use_actor_critic: bool,
-        act_func: Callable,
-        store_data_func: Callable,
-        update_dynamics_func: Callable,
+        act_func: Callable[[int, torch.Tensor], torch.Tensor],
+        store_data_func: Callable[
+            [
+                torch.Tensor,
+                torch.Tensor,
+                torch.Tensor,
+                torch.Tensor,
+                torch.Tensor,
+                torch.Tensor,
+                torch.Tensor,
+                dict[str, Any],
+            ],
+            None,
+        ],
+        update_dynamics_func: Callable[[], None],
         logger: Logger,
         use_eval: bool,
-        eval_func: Callable,
-        algo_reset_func: Callable,
-        update_actor_func: Callable,
+        eval_func: Callable[[int, bool], None],
+        algo_reset_func: Callable[[], None],
+        update_actor_func: Callable[[int], None],
     ) -> int:
         """Roll out the environment and store the data in the buffer.
 
         Args:
             current_step (int): Current training step.
-            roll_out_step (int): Number of steps to roll out.
+            rollout_step (int): Number of steps to roll out.
             use_actor_critic (bool): Whether to use actor-critic.
-            act_func (Callable): Function to get action.
-            store_data_func (Callable): Function to store data.
-            update_dynamics_func (Callable): Function to update dynamics.
-            logger (Logger): Logger.
+            act_func (Callable[[int, torch.Tensor], torch.Tensor]): Function to get action.
+            store_data_func (Callable[[torch.Tensor, ..., dict[str, Any], ], None,]): Function to store data.
+            update_dynamics_func (Callable[[], None]): Function to update dynamics.
+            logger (Logger): Logger, to log ``EpRet``, ``EpCost``, ``EpLen``.
             use_eval (bool): Whether to use evaluation.
-            eval_func (Callable): Function to evaluate the agent.
-            algo_reset_func (Callable): Function to reset the algorithm.
-            update_actor_func (Callable): Function to update the actor.
+            eval_func (Callable[[int, bool], None]): Function to evaluate the agent.
+            algo_reset_func (Callable[[], None]): Function to reset the algorithm.
+            update_actor_func (Callable[[int], None]): Function to update the actor.
         """
         epoch_start_time = time.time()
 
         update_actor_critic_time = 0.0
         update_dynamics_time = 0.0
         if use_eval:
             eval_time = 0.0
 
         epoch_steps = 0
 
-        while epoch_steps < roll_out_step and current_step < self._cfgs.train_cfgs.total_steps:
-            action, action_info = act_func(current_step, self._current_obs, self._env)
+        while epoch_steps < rollout_step and current_step < self._cfgs.train_cfgs.total_steps:
+            action = act_func(current_step, self._current_obs)
             next_state, reward, cost, terminated, truncated, info = self.step(action)
             epoch_steps += info['num_step']
             current_step += info['num_step']
             self._log_value(reward=reward, cost=cost, info=info)
 
             store_data_func(
-                current_step,
-                self._ep_len,
                 self._current_obs,
                 action,
                 reward,
                 cost,
                 terminated,
                 truncated,
                 next_state,
                 info,
-                action_info,
             )
             self._current_obs = next_state
             if terminated or truncated:
                 self._log_metrics(logger)
                 self._reset_log()
                 self._current_obs, _ = self.reset()
                 if algo_reset_func is not None:
-                    algo_reset_func(current_step)
+                    algo_reset_func()
             if (
                 current_step % self._cfgs.algo_cfgs.update_dynamics_cycle
                 < self._cfgs.algo_cfgs.action_repeat
                 and current_step - self._last_dynamics_update
                 >= self._cfgs.algo_cfgs.update_dynamics_cycle
             ):
                 update_dynamics_start = time.time()
-                update_dynamics_func(current_step)
+                update_dynamics_func()
                 self._last_dynamics_update = current_step
                 update_dynamics_time += time.time() - update_dynamics_start
 
             if (
                 use_actor_critic
                 and current_step % self._cfgs.algo_cfgs.update_policy_cycle
                 < self._cfgs.algo_cfgs.action_repeat
@@ -309,74 +324,70 @@
             if (
                 use_eval
                 and current_step % self._cfgs.evaluation_cfgs.eval_cycle
                 < self._cfgs.algo_cfgs.action_repeat
                 and current_step - self._last_eval >= self._cfgs.evaluation_cfgs.eval_cycle
             ):
                 eval_start = time.time()
-                eval_func(current_step)
+                eval_func(current_step, True)
                 self._last_eval = current_step
                 eval_time += time.time() - eval_start
 
         if not self._first_log or current_step >= self._cfgs.train_cfgs.total_steps:
             self._log_metrics(logger)
 
         epoch_time = time.time() - epoch_start_time
         logger.store(**{'Time/Epoch': epoch_time})
         logger.store(**{'Time/UpdateDynamics': update_dynamics_time})
-        roll_out_time = epoch_time - update_dynamics_time
+        rollout_time = epoch_time - update_dynamics_time
 
         if use_eval:
             logger.store(**{'Time/Eval': eval_time})
-            roll_out_time -= eval_time
+            rollout_time -= eval_time
 
         if use_actor_critic:
             logger.store(**{'Time/UpdateActorCritic': update_actor_critic_time})
-            roll_out_time -= update_actor_critic_time
-        logger.store(**{'Time/Rollout': roll_out_time})
+            rollout_time -= update_actor_critic_time
+        logger.store(**{'Time/Rollout': rollout_time})
         return current_step
 
     def _log_value(
         self,
         reward: torch.Tensor,
         cost: torch.Tensor,
-        info: dict,
+        info: dict[str, Any],
     ) -> None:
         """Log value.
 
         .. note::
             OmniSafe uses :class:`RewardNormalizer` wrapper, so the original reward and cost will
             be stored in ``info['original_reward']`` and ``info['original_cost']``.
 
         Args:
-            reward (torch.Tensor): The reward.
-            cost (torch.Tensor): The cost.
-            info (dict): Information.
+            reward (torch.Tensor): The immediate step reward.
+            cost (torch.Tensor): The immediate step cost.
+            info (dict[str, Any]): Some information logged by the environment.
         """
         self._ep_ret += info.get('original_reward', reward).cpu()
         self._ep_cost += info.get('original_cost', cost).cpu()
         self._ep_len += info.get('num_step', 1)
 
     def _log_metrics(self, logger: Logger) -> None:
         """Log metrics.
 
         Args:
-            logger (Logger): Logger.
+            logger (Logger): Logger, to log ``EpRet``, ``EpCost``, ``EpLen``.
         """
         self._first_log = True
         logger.store(
-            **{
+            {
                 'Metrics/EpRet': self._ep_ret,
                 'Metrics/EpCost': self._ep_cost,
                 'Metrics/EpLen': self._ep_len,
             },
         )
 
-    def _reset_log(self, idx: int | None = None) -> None:  # pylint: disable=unused-argument
-        """Reset log.
-
-        Args:
-            idx (int | None): The index of the environment.
-        """
+    def _reset_log(self) -> None:
+        """Reset log."""
         self._ep_ret = torch.zeros(1)
         self._ep_cost = torch.zeros(1)
         self._ep_len = torch.zeros(1)
```

### Comparing `omnisafe-0.4.0/omnisafe/adapter/offpolicy_adapter.py` & `omnisafe-0.5.0b0/omnisafe/adapter/offpolicy_adapter.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.4.0/omnisafe/adapter/online_adapter.py` & `omnisafe-0.5.0b0/omnisafe/adapter/online_adapter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -38,21 +38,14 @@
 class OnlineAdapter:
     """Online Adapter for OmniSafe.
 
     OmniSafe is a framework for safe reinforcement learning. It is designed to be compatible with
     any existing RL algorithms. The online adapter is used to adapt the environment to the
     framework.
 
-    OmniSafe provides a set of adapters to adapt the environment to the framework.
-
-    - OnPolicyAdapter: Adapt the environment to the on-policy framework.
-    - OffPolicyAdapter: Adapt the environment to the off-policy framework.
-    - SauteAdapter: Adapt the environment to the SAUTE framework.
-    - SimmerAdapter: Adapt the environment to the SIMMER framework.
-
     Args:
         env_id (str): The environment id.
         num_envs (int): The number of parallel environments.
         seed (int): The random seed.
         cfgs (Config): The configuration.
     """
```

### Comparing `omnisafe-0.4.0/omnisafe/adapter/onpolicy_adapter.py` & `omnisafe-0.5.0b0/omnisafe/adapter/onpolicy_adapter.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.4.0/omnisafe/adapter/saute_adapter.py` & `omnisafe-0.5.0b0/omnisafe/adapter/saute_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -63,15 +63,15 @@
 
         self._safety_budget: torch.Tensor = (
             self._cfgs.algo_cfgs.safety_budget
             * (1 - self._cfgs.algo_cfgs.saute_gamma**self._cfgs.algo_cfgs.max_ep_len)
             / (1 - self._cfgs.algo_cfgs.saute_gamma)
             / self._cfgs.algo_cfgs.max_ep_len
             * torch.ones(num_envs, 1)
-        )
+        ).to(self._device)
 
         assert isinstance(self._env.observation_space, Box), 'Observation space must be Box'
         self._observation_space: Box = Box(
             low=-np.inf,
             high=np.inf,
             shape=(self._env.observation_space.shape[0] + 1,),
         )
@@ -116,15 +116,15 @@
             Additionally, the safety observation will be reset.
 
         Returns:
             observation: The initial observation of the space.
             info: Some information logged by the environment.
         """
         obs, info = self._env.reset()
-        self._safety_obs = torch.ones(self._env.num_envs, 1)
+        self._safety_obs = torch.ones(self._env.num_envs, 1).to(self._device)
         obs = self._augment_obs(obs)
         return obs, info
 
     def step(
         self,
         action: torch.Tensor,
     ) -> tuple[
@@ -232,15 +232,15 @@
 
         Args:
             idx (int or None, optional): The index of the environment. Defaults to None
                 (single environment).
         """
         super()._reset_log(idx)
         if idx is None:
-            self._ep_budget = torch.zeros(self._env.num_envs)
+            self._ep_budget = torch.zeros(self._env.num_envs).to(self._device)
         else:
             self._ep_budget[idx] = 0
 
     def _log_metrics(self, logger: Logger, idx: int) -> None:
         """Log metrics, including ``EpRet``, ``EpCost``, ``EpLen`` and ``EpBudget``.
 
         Args:
```

### Comparing `omnisafe-0.4.0/omnisafe/adapter/simmer_adapter.py` & `omnisafe-0.5.0b0/omnisafe/adapter/simmer_adapter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -61,48 +61,50 @@
         self._num_envs: int = num_envs
         self._safety_budget: torch.Tensor = (
             self._cfgs.algo_cfgs.safety_budget
             * (1 - self._cfgs.algo_cfgs.saute_gamma**self._cfgs.algo_cfgs.max_ep_len)
             / (1 - self._cfgs.algo_cfgs.saute_gamma)
             / self._cfgs.algo_cfgs.max_ep_len
             * torch.ones(num_envs, 1)
-        )
+        ).to(self._device)
         self._upper_budget: torch.Tensor = (
             self._cfgs.algo_cfgs.upper_budget
             * (1 - self._cfgs.algo_cfgs.saute_gamma**self._cfgs.algo_cfgs.max_ep_len)
             / (1 - self._cfgs.algo_cfgs.saute_gamma)
             / self._cfgs.algo_cfgs.max_ep_len
             * torch.ones(num_envs, 1)
+        ).to(self._device)
+        self._rel_safety_budget: torch.Tensor = (self._safety_budget / self._upper_budget).to(
+            self._device,
         )
-        self._rel_safety_budget: torch.Tensor = self._safety_budget / self._upper_budget
 
         assert isinstance(self._env.observation_space, Box), 'Observation space must be Box'
         self._observation_space: Box = Box(
             low=-np.inf,
             high=np.inf,
             shape=(self._env.observation_space.shape[0] + 1,),
         )
         self._controller: BaseSimmerAgent = SimmerPIDAgent(
             cfgs=cfgs.control_cfgs,
-            budget_bound=self._upper_budget,
+            budget_bound=self._upper_budget.cpu(),
         )
 
     def reset(self) -> tuple[torch.Tensor, dict[str, Any]]:
         """Reset the environment and returns an initial observation.
 
         .. note::
             Additionally, the safety observation will be reset. And the safety budget will be reset
             to the value of current ``rel_safety_budget``.
 
         Returns:
             observation: The initial observation of the space.
             info: Some information logged by the environment.
         """
         obs, info = self._env.reset()
-        self._safety_obs = self._rel_safety_budget * torch.ones(self._num_envs, 1)
+        self._safety_obs = self._rel_safety_budget * torch.ones(self._num_envs, 1).to(self._device)
         obs = self._augment_obs(obs)
         return obs, info
 
     def control_budget(self, ep_costs: torch.Tensor) -> None:
         """Control the safety budget.
 
         Args:
@@ -111,10 +113,10 @@
         ep_costs = (
             ep_costs
             * (1 - self._cfgs.algo_cfgs.saute_gamma**self._cfgs.algo_cfgs.max_ep_len)
             / (1 - self._cfgs.algo_cfgs.saute_gamma)
             / self._cfgs.algo_cfgs.max_ep_len
         )
         self._safety_budget = self._controller.act(
-            safety_budget=self._safety_budget,
-            observation=ep_costs,
-        )
+            safety_budget=self._safety_budget.cpu(),
+            observation=ep_costs.cpu(),
+        ).to(self._device)
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/__init__.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,19 +13,35 @@
 # limitations under the License.
 # ==============================================================================
 """Safe Reinforcement Learning algorithms."""
 
 import itertools
 from types import MappingProxyType
 
-from omnisafe.algorithms import model_based, off_policy, on_policy
+from omnisafe.algorithms import model_based, off_policy, offline, on_policy
 from omnisafe.algorithms.base_algo import BaseAlgo
 
+# Model-based Safe
+from omnisafe.algorithms.model_based import CAPPETS, CCEPETS, LOOP, PETS, RCEPETS, SafeLOOP
+
 # Off-Policy Safe
-from omnisafe.algorithms.off_policy import DDPG, SAC, TD3, DDPGLag, SACLag, TD3Lag
+from omnisafe.algorithms.off_policy import (
+    DDPG,
+    DDPGPID,
+    SAC,
+    SACPID,
+    TD3,
+    TD3PID,
+    DDPGLag,
+    SACLag,
+    TD3Lag,
+)
+
+# Offline Safe
+from omnisafe.algorithms.offline import BCQ, CCRR, CRR, VAEBC, BCQLag, COptiDICE
 
 # On-Policy Safe
 from omnisafe.algorithms.on_policy import (
     CPO,
     CPPOPID,
     CUP,
     FOCOPS,
@@ -45,22 +61,19 @@
     TRPOEarlyTerminated,
     TRPOLag,
     TRPOSaute,
     TRPOSimmerPID,
 )
 
 
-# Model-based Safe
-# from omnisafe.algorithms.model_based import CAP, MBPPOLag, SafeLOOP
-
-
 ALGORITHMS = {
     'on-policy': tuple(on_policy.__all__),
     'off-policy': tuple(off_policy.__all__),
     'model-based': tuple(model_based.__all__),
+    'offline': tuple(offline.__all__),
 }
 
 ALGORITHM2TYPE = {
     algo: algo_type for algo_type, algorithms in ALGORITHMS.items() for algo in algorithms
 }
 
 __all__ = ALGORITHMS['all'] = tuple(itertools.chain.from_iterable(ALGORITHMS.values()))
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/algo_wrapper.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/algo_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,21 +84,22 @@
         Raises:
             AssertionError: If the algorithm name is not in the supported algorithms.
         """
         assert (
             self.algo in ALGORITHMS['all']
         ), f"{self.algo} doesn't exist. Please choose from {ALGORITHMS['all']}."
         self.algo_type = ALGORITHM2TYPE.get(self.algo, '')
-        if self.algo_type in ['model-based'] and self.train_terminal_cfgs is not None:
+        if self.algo_type in ['model-based', 'offline'] and self.train_terminal_cfgs is not None:
             assert (
                 self.train_terminal_cfgs['parallel'] == 1
-            ), 'model-based only support parallel==1!'
+            ), 'model-based and offline only support parallel==1!'
             assert (
                 self.train_terminal_cfgs['vector_env_nums'] == 1
-            ), 'model-based only support vector_env_nums==1!'
+            ), 'model-based and offline only support vector_env_nums==1!'
+
         cfgs = get_default_kwargs_yaml(self.algo, self.env_id, self.algo_type)
 
         # update the cfgs from custom configurations
         if self.custom_cfgs:
             # avoid repeatedly record the env_id and algo
             if 'env_id' in self.custom_cfgs:
                 self.custom_cfgs.pop('env_id')
@@ -157,15 +158,15 @@
             # re-launches the current script with workers linked by MPI
             sys.exit()
         self.agent: BaseAlgo = registry.get(self.algo)(
             env_id=self.env_id,
             cfgs=self.cfgs,
         )
 
-    def learn(self) -> tuple[float, float, int]:
+    def learn(self) -> tuple[float, float, float]:
         """Agent learning.
 
         Returns:
             ep_ret: The episode return of the final episode.
             ep_cost: The episode cost of the final episode.
             ep_len: The episode length of the final episode.
         """
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/base_algo.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/base_algo.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Implementation of the Policy Gradient algorithm."""
+"""Implementation of the Base algorithms."""
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 
 import torch
 
@@ -28,15 +28,15 @@
 
 class BaseAlgo(ABC):  # pylint: disable=too-few-public-methods
     """Base class for all algorithms."""
 
     _logger: Logger
 
     def __init__(self, env_id: str, cfgs: Config) -> None:
-        """Initialize an instance of :class:`BaseAlgo`."""
+        """Initialize an instance of algorithm."""
         self._env_id: str = env_id
         self._cfgs: Config = cfgs
 
         assert hasattr(cfgs, 'seed'), 'Please specify the seed in the config file.'
         self._seed: int = int(cfgs.seed) + distributed.get_rank() * 1000
         seed_all(self._seed)
 
@@ -75,9 +75,9 @@
         """Initialize the model."""
 
     @abstractmethod
     def _init_log(self) -> None:
         """Initialize the logger."""
 
     @abstractmethod
-    def learn(self) -> tuple[float, float, int]:
+    def learn(self) -> tuple[float, float, float]:
         """Learn the policy."""
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/model_based/__init__.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/model_based/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/model_based/base/__init__.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/model_based/base/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/model_based/base/ensemble.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/model_based/base/ensemble.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 # Modified version of model.py from  https://github.com/Xingyu-Lin/mbpo_pytorch/blob/main/model.py
 # original version doesn't validate model error batch-wise and is highly memory intensive.
 # ==============================================================================
 """The Dynamics Model of MBPO and PETS."""
+
+
 from __future__ import annotations
 
 import itertools
 from collections import defaultdict
 from functools import partial
 from typing import Callable
 
@@ -34,59 +36,77 @@
 
 def swish(data: torch.Tensor) -> torch.Tensor:
     """Transform data using sigmoid function."""
     return data * torch.sigmoid(data)
 
 
 class StandardScaler:
-    """Normalize data."""
+    """Normalizes data using standardization.
+
+    This class provides methods to fit the scaler to the input data and transform
+    the input data using the parameters learned during the fitting process.
+
+    Args:
+        device (torch.device): The device to use.
+    """
 
     def __init__(self, device: torch.device) -> None:
         """Initialize an instance of :class:`StandardScaler`."""
-        self._mean = 0.0
-        self._std = 1.0
-        self._mean_t = torch.tensor(self._mean).to(device)
-        self._std_t = torch.tensor(self._std).to(device)
-        self._device = device
+        self._mean: float = 0.0
+        self._std: float = 1.0
+        self._mean_t: torch.Tensor = torch.tensor(self._mean).to(device)
+        self._std_t: torch.Tensor = torch.tensor(self._std).to(device)
+        self._device: torch.device = device
 
-    def fit(self, data: torch.Tensor | np.ndarray) -> None:
+    def fit(self, data: np.ndarray) -> None:
         """Fits the scaler to the input data.
 
         Args:
-            data (np.ndarray): A numpy array containing the input
+            data (np.ndarray): A numpy array containing the input.
         """
         self._mean = np.mean(data, axis=0, keepdims=True)
         self._std = np.std(data, axis=0, keepdims=True)
         self._std = np.maximum(self._std, 1e-12)
         self._mean_t = torch.FloatTensor(self._mean).to(self._device)
         self._std_t = torch.FloatTensor(self._std).to(self._device)
 
-    def transform(self, data: torch.Tensor | np.ndarray) -> torch.Tensor | np.ndarray:
+    def transform(self, data: torch.Tensor) -> torch.Tensor:
         """Transforms the input matrix data using the parameters of this scaler.
 
-        Arguments:
-            data (torch.Tensor|np.ndarray): A numpy array containing the input
+        Args:
+            data (torch.Tensor): The input data to transform.
 
         Returns:
-            transformed_data (torch.Tensor|np.ndarray): The transformed data.
+            transformed_data: The transformed data.
         """
-        if torch.is_tensor(data):
-            return (data - self._mean_t) / self._std_t
-        return (data - self._mean) / self._std
+        return (data - self._mean_t) / self._std_t
 
 
 def init_weights(layer: nn.Module) -> None:
-    """Initialize network weight."""
+    """Initialize network weight.
+
+    Args:
+        layer (nn.Module): The layer to initialize.
+    """
 
     def truncated_normal_init(
         weight: torch.Tensor,
         mean: float = 0.0,
         std: float = 0.01,
     ) -> torch.Tensor:
-        """Initialize network weight."""
+        """Initialize network weight.
+
+        Args:
+            weight (torch.Tensor): The weight to be initialized.
+            mean (float): The mean of the normal distribution.
+            std (float): The standard deviation of the normal distribution.
+
+        Returns:
+            weight: The initialized weight.
+        """
         torch.nn.init.normal_(weight, mean=mean, std=std)
         while True:
             cond = torch.logical_or(weight < mean - 2 * std, weight > mean + 2 * std)
             if not torch.sum(cond):
                 break
             weight = torch.where(
                 cond,
@@ -105,147 +125,215 @@
     layer: nn.Module | EnsembleFC,
     input_data: torch.Tensor,
     index: int,
 ) -> torch.Tensor:
     """Special forward for nn.Sequential modules which contain BatchedLinear layers we want to use.
 
     Args:
-        layer (nn.Module|EnsembleFC): The layer to forward through.
+        layer (nn.Module | EnsembleFC): The layer to forward through.
         input_data (torch.Tensor): The input data.
         index (int): The index of the model to use.
 
     Returns:
-        output (torch.Tensor): The output of the layer.
+        output: The output of the layer.
     """
     if isinstance(layer, EnsembleFC):
         output = F.linear(
             input_data,
             torch.transpose(layer.weight[index].squeeze(0), 0, 1),
             layer.bias[index],
         )
 
     else:
         output = layer(input_data)
     return output
 
 
 class EnsembleFC(nn.Module):
-    """Ensemble fully connected network."""
+    """Ensemble fully connected network.
+
+    A fully connected network with ensemble_size models.
 
-    _constants_ = ['in_features', 'out_features']
+    Args:
+        in_features (int): The number of input features.
+        out_features (int): The number of output features.
+        ensemble_size (int): The number of models in the ensemble.
+        weight_decay (float): The decaying factor.
+        bias (bool): Whether to use bias.
+
+    Attributes:
+        in_features (int): The number of input features.
+        out_features (int): The number of output features.
+        ensemble_size (int): The number of models in the ensemble.
+        weight (nn.Parameter): The weight of the network.
+        bias (nn.Parameter): The bias of the network.
+    """
+
+    _constants_: list[str]
     in_features: int
     out_features: int
     ensemble_size: int
-    weight: torch.Tensor
+    weight: nn.Parameter
 
     def __init__(
         self,
         in_features: int,
         out_features: int,
         ensemble_size: int,
         weight_decay: float = 0.0,
         bias: bool = True,
     ) -> None:
-        """Initialize network weight."""
+        """Initialize an instance of fully connected network."""
         super().__init__()
+        self._constants_ = ['in_features', 'out_features']
         self.in_features = in_features
         self.out_features = out_features
         self.ensemble_size = ensemble_size
         self.weight = nn.Parameter(torch.Tensor(ensemble_size, in_features, out_features))
         self.weight_decay = weight_decay
         if bias:
             self.bias = nn.Parameter(torch.Tensor(ensemble_size, out_features))
         else:
             self.register_parameter('bias', None)
 
     def forward(self, input_data: torch.Tensor) -> torch.Tensor:
-        """Forward pass."""
+        """Forward pass.
+
+        Args:
+            input_data (torch.Tensor): The input data.
+
+        Returns:
+            The forward output of the network.
+        """
         w_times_x = torch.bmm(input_data, self.weight)
-        return torch.add(w_times_x, self.bias[:, None, :])  # w times x + b
+        if self.bias is not None:
+            return torch.add(w_times_x, self.bias[:, None, :])  # w times x + b
+        return w_times_x  # type: ignore
 
 
 # pylint: disable-next=too-many-instance-attributes
 class EnsembleModel(nn.Module):
-    """Ensemble dynamics model."""
+    """Ensemble dynamics model.
+
+    A dynamics model with ensemble_size models.
+
+    Args:
+        device (torch.device): The device to use.
+        state_size (int): The size of the state.
+        action_size (int): The size of the action.
+        reward_size (int): The size of the reward.
+        cost_size (int): The size of the cost.
+        ensemble_size (int): The number of models in the ensemble.
+        predict_reward (bool): Whether to predict reward.
+        predict_cost (bool): Whether to predict cost.
+        hidden_size (int): The size of the hidden layer.
+        learning_rate (float): The learning rate.
+        use_decay (bool): Whether to use weight decay.
+
+    Attributes:
+        max_logvar (torch.Tensor): The maximum log variance.
+        min_logvar (torch.Tensor): The minimum log variance.
+        scaler (StandardScaler): The scaler.
+    """
+
+    max_logvar: torch.Tensor
+    min_logvar: torch.Tensor
 
     # pylint: disable-next=too-many-arguments
     def __init__(
         self,
         device: torch.device,
         state_size: int,
         action_size: int,
         reward_size: int,
         cost_size: int,
         ensemble_size: int,
         predict_reward: bool,
-        predict_cost: bool | None = None,
+        predict_cost: bool = False,
         hidden_size: int = 200,
         learning_rate: float = 1e-3,
         use_decay: bool = False,
     ) -> None:
         """Initialize network weight."""
         super().__init__()
 
-        self._state_size = state_size
-        self._reward_size = reward_size
-        self._cost_size = cost_size
-        self._predict_reward = predict_reward
-        self._predict_cost = predict_cost
+        self._state_size: int = state_size
+        self._reward_size: int = reward_size
+        self._cost_size: int = cost_size
+        self._predict_reward: bool = predict_reward
+        self._predict_cost: bool = predict_cost
 
-        self._output_dim = state_size
+        self._output_dim: int = state_size
         if predict_reward:
             self._output_dim += reward_size
         if predict_cost:
             self._output_dim += cost_size
 
-        self._hidden_size = hidden_size
-        self._use_decay = use_decay
+        self._hidden_size: int = hidden_size
+        self._use_decay: bool = use_decay
 
-        self._nn1 = EnsembleFC(
+        self._nn1: EnsembleFC = EnsembleFC(
             state_size + action_size,
             hidden_size,
             ensemble_size,
             weight_decay=0.000025,
         )
-        self._nn2 = EnsembleFC(hidden_size, hidden_size, ensemble_size, weight_decay=0.00005)
-        self._nn3 = EnsembleFC(hidden_size, hidden_size, ensemble_size, weight_decay=0.000075)
-        self._nn4 = EnsembleFC(hidden_size, hidden_size, ensemble_size, weight_decay=0.000075)
-        self._nn5 = EnsembleFC(
+        self._nn2: EnsembleFC = EnsembleFC(
+            hidden_size,
+            hidden_size,
+            ensemble_size,
+            weight_decay=0.00005,
+        )
+        self._nn3: EnsembleFC = EnsembleFC(
+            hidden_size,
+            hidden_size,
+            ensemble_size,
+            weight_decay=0.000075,
+        )
+        self._nn4: EnsembleFC = EnsembleFC(
+            hidden_size,
+            hidden_size,
+            ensemble_size,
+            weight_decay=0.000075,
+        )
+        self._nn5: EnsembleFC = EnsembleFC(
             hidden_size,
             self._output_dim * 2,
             ensemble_size,
             weight_decay=0.0001,
         )
 
         self.register_buffer('max_logvar', (torch.ones((1, self._output_dim)).float() / 2))
         self.register_buffer('min_logvar', (-torch.ones((1, self._output_dim)).float() * 10))
-        self._optimizer = torch.optim.Adam(self.parameters(), lr=learning_rate)
+        self._optimizer: torch.optim.Adam = torch.optim.Adam(self.parameters(), lr=learning_rate)
         self.apply(init_weights)
-        self._device = device
-        self.scaler = StandardScaler(self._device)
+        self._device: torch.device = device
+        self.scaler: StandardScaler = StandardScaler(self._device)
 
     def forward(
         self,
         data: torch.Tensor | np.ndarray,
         ret_log_var: bool = False,
     ) -> tuple[torch.Tensor, torch.Tensor]:
         """Compute next state, reward, cost using all models.
 
         Args:
             data (torch.Tensor): Input data.
-            ret_log_var (bool): Whether to return the log variance.
+            ret_log_var (bool, optional): Whether to return the log variance, defaults to False.
 
         Returns:
-            mean (torch.Tensor): Mean of the next state, reward, cost.
-            logvar or var (torch.Tensor): Log variance of the next state, reward, cost.
+            mean: Mean of the next state, reward, cost.
+            logvar or var: Log variance of the next state, reward, cost.
         """
-        if not torch.is_tensor(data):
-            data = torch.tensor(data, dtype=torch.float32, device=self._device)
-        data = self.scaler.transform(data)
-        nn1_output = swish(self._nn1(data))
+        if isinstance(data, torch.Tensor):
+            data_t = data
+        else:
+            data_t = torch.tensor(data, dtype=torch.float32, device=self._device)
+        data_t = self.scaler.transform(data_t)
+        nn1_output = swish(self._nn1(data_t))
         nn2_output = swish(self._nn2(nn1_output))
         nn3_output = swish(self._nn3(nn2_output))
         nn4_output = swish(self._nn4(nn3_output))
         nn5_output = self._nn5(nn4_output)
         mean = nn5_output[:, :, : self._output_dim]
         logvar = self.max_logvar - F.softplus(
             self.max_logvar - nn5_output[:, :, self._output_dim :],
@@ -261,28 +349,30 @@
         data: torch.Tensor | np.ndarray,
         idx_model: int,
         ret_log_var: bool = False,
     ) -> tuple[torch.Tensor, torch.Tensor]:
         """Compute next state, reward, cost from an certain model.
 
         Args:
-            data (torch.Tensor): Input data.
+            data (torch.Tensor | np.ndarray): Input data.
             idx_model (int): Index of the model.
             ret_log_var (bool): Whether to return the log variance.
 
         Returns:
-            mean (torch.Tensor): Mean of the next state, reward, cost.
-            logvar or var (torch.Tensor): Log variance of the next state, reward, cost.
+            mean: Mean of the next state, reward, cost.
+            logvar or var: Log variance of the next state, reward, cost.
         """
         assert data.shape[0] == 1
-        if not torch.is_tensor(data):
-            data = torch.tensor(data, dtype=torch.float32, device=self._device)
-        data = self.scaler.transform(data[0])
+        if isinstance(data, torch.Tensor):
+            data_t = data
+        else:
+            data_t = torch.tensor(data, dtype=torch.float32, device=self._device)
+        data_t = self.scaler.transform(data_t[0])
         unbatched_forward_fn = partial(unbatched_forward, index=idx_model)
-        nn1_output = swish(unbatched_forward_fn(self._nn1, data))
+        nn1_output = swish(unbatched_forward_fn(self._nn1, data_t))
         nn2_output = swish(unbatched_forward_fn(self._nn2, nn1_output))
         nn3_output = swish(unbatched_forward_fn(self._nn3, nn2_output))
         nn4_output = swish(unbatched_forward_fn(self._nn4, nn3_output))
         nn5_output = unbatched_forward_fn(self._nn5, nn4_output)
         mean = nn5_output[:, : self._output_dim]
         logvar = self.max_logvar - F.softplus(self.max_logvar - nn5_output[:, self._output_dim :])
         logvar = self.min_logvar + F.softplus(logvar - self.min_logvar)
@@ -309,15 +399,15 @@
     ) -> tuple[torch.Tensor, torch.Tensor]:
         """Compute loss.
 
         Args:
             mean (torch.Tensor): Mean of the next state, reward, cost.
             logvar (torch.Tensor): Log variance of the next state, reward, cost.
             labels (torch.Tensor): Ground truth of the next state, reward, cost.
-            inc_var_loss (bool): Whether to include the variance loss.
+            inc_var_loss (bool, optional): Whether to include the variance loss. Defaults to True.
 
         Returns:
             total_loss (torch.Tensor): Total loss.
             mse_loss (torch.Tensor): MSE loss.
         """
         assert len(mean.shape) == len(logvar.shape) == len(labels.shape) == 3
         inv_var = torch.exp(-logvar)
@@ -328,89 +418,111 @@
             total_loss = torch.sum(mse_loss) + torch.sum(var_loss)
         else:
             mse_loss = torch.mean(torch.pow(mean - labels, 2), dim=(1, 2))
             total_loss = torch.sum(mse_loss)
         return total_loss, mse_loss
 
     def train_ensemble(self, loss: torch.Tensor) -> None:
-        """Train the dynamics model."""
+        """Train the dynamics model.
+
+        Args:
+            loss (torch.Tensor): The loss of the dynamics model.
+        """
         self._optimizer.zero_grad()
         loss += 0.01 * torch.sum(torch.Tensor(self.max_logvar)) - 0.01 * torch.sum(
             torch.Tensor(self.min_logvar),
         )
         if self._use_decay:
             loss += self._get_decay_loss()
         loss.backward()
         self._optimizer.step()
 
 
 # pylint: disable-next=too-many-instance-attributes
 class EnsembleDynamicsModel:
-    """Dynamics model for predict next state, reward and cost."""
+    """Dynamics model for predict next state, reward and cost.
+
+    Args:
+        model_cfgs (Config): The configuration of the dynamics model.
+        device (torch.device): The device to use.
+        state_shape (tuple[int, ...]): The shape of the state.
+        action_shape (tuple[int, ...]): The shape of the action.
+        actor_critic (ConstraintActorCritic | ConstraintActorQCritic | None, optional): The actor critic model.
+            Defaults to None.
+        rew_func (Callable[[torch.Tensor], torch.Tensor] | None, optional): The reward function. Defaults to None.
+        cost_func (Callable[[torch.Tensor], torch.Tensor] | None, optional): The cost function.
+            Defaults to None.
+        terminal_func (Callable[[torch.Tensor], torch.Tensor] | None, optional): The terminal function.
+            Defaults to None.
+
+    Attributes:
+        elite_model_idxes (list[int]): The index of the elite models.
+    """
 
     # pylint: disable-next=too-many-arguments
     def __init__(
         self,
         model_cfgs: Config,
         device: torch.device,
         state_shape: tuple[int, ...],
         action_shape: tuple[int, ...],
         actor_critic: ConstraintActorCritic | ConstraintActorQCritic | None = None,
-        rew_func: Callable | None = None,
-        cost_func: Callable | None = None,
-        terminal_func: Callable | None = None,
+        rew_func: Callable[[torch.Tensor], torch.Tensor] | None = None,
+        cost_func: Callable[[torch.Tensor], torch.Tensor] | None = None,
+        terminal_func: Callable[[torch.Tensor], torch.Tensor] | None = None,
     ) -> None:
         """Initialize the dynamics model."""
-        self._num_ensemble = model_cfgs.num_ensemble
-        self._elite_size = model_cfgs.elite_size
-        self._predict_reward = model_cfgs.predict_reward
-        self._predict_cost = model_cfgs.predict_cost
-        self._batch_size = model_cfgs.batch_size
-        self._max_epoch_since_update = model_cfgs.max_epoch
-
-        self._reward_size = model_cfgs.reward_size
-        self._cost_size = model_cfgs.cost_size
-        self._use_cost = model_cfgs.use_cost
-        self._use_terminal = model_cfgs.use_terminal
-        self._use_var = model_cfgs.use_var
-        self._use_reward_critic = model_cfgs.use_reward_critic
-        self._use_cost_critic = model_cfgs.use_cost_critic
-
-        self._device = device
-
-        self._state_size = state_shape[0]
-        self._action_size = action_shape[0]
-
-        self._rew_func = rew_func
-        self._cost_func = cost_func
-        self._terminal_func = terminal_func
+        self._num_ensemble: int = model_cfgs.num_ensemble
+        self._elite_size: int = model_cfgs.elite_size
+        self._predict_reward: bool = model_cfgs.predict_reward
+        self._predict_cost: bool = model_cfgs.predict_cost
+        self._batch_size: int = model_cfgs.batch_size
+        self._max_epoch_since_update: int = model_cfgs.max_epoch
+
+        self._reward_size: int = model_cfgs.reward_size
+        self._cost_size: int = model_cfgs.cost_size
+        self._use_cost: bool = model_cfgs.use_cost
+        self._use_terminal: bool = model_cfgs.use_terminal
+        self._use_var: bool = model_cfgs.use_var
+        self._use_reward_critic: bool = model_cfgs.use_reward_critic
+        self._use_cost_critic: bool = model_cfgs.use_cost_critic
+
+        self._device: torch.device = device
+
+        self._state_size: int = state_shape[0]
+        self._action_size: int = action_shape[0]
+
+        self._rew_func: Callable[[torch.Tensor], torch.Tensor] | None = rew_func
+        self._cost_func: Callable[[torch.Tensor], torch.Tensor] | None = cost_func
+        self._terminal_func: Callable[[torch.Tensor], torch.Tensor] | None = terminal_func
 
-        self._actor_critic = actor_critic
+        self._actor_critic: ConstraintActorCritic | ConstraintActorQCritic | None = actor_critic
 
         self._model_list: list[int] = []
 
-        self.elite_model_idxes = list(range(self._elite_size))
-        self._ensemble_model = EnsembleModel(
+        self.elite_model_idxes: list[int] = list(range(self._elite_size))
+        self._ensemble_model: EnsembleModel = EnsembleModel(
             device=self._device,
             state_size=self._state_size,
             action_size=self._action_size,
             reward_size=self._reward_size,
             cost_size=self._cost_size,
             ensemble_size=self._num_ensemble,
             predict_reward=model_cfgs.predict_reward,
             predict_cost=model_cfgs.predict_cost,
             hidden_size=model_cfgs.hidden_size,
             learning_rate=1e-3,
             use_decay=model_cfgs.use_decay,
         )
         self._ensemble_model.to(self._device)
-
         self._max_epoch_since_update = 5
-        self._epochs_since_update = 0
-        self._snapshots = {i: (0, 1e10) for i in range(self._num_ensemble)}
+        self._epochs_since_update: int = 0
+        self._snapshots: dict[int, tuple[int, float]] = {
+            i: (0, 1e10) for i in range(self._num_ensemble)
+        }
 
         if self._predict_reward is False:
             assert rew_func is not None, 'rew_func should not be None'
         if self._use_cost is True and self._predict_cost is False:
             assert cost_func is not None, 'cost_func should not be None'
             assert (
                 cost_func(torch.zeros((1, self._state_size)).to(self._device)) is not None
@@ -421,25 +533,25 @@
         self._state_start_dim = (
             int(self._predict_reward) * self._reward_size
             + int(self._predict_cost) * self._cost_size
         )
 
     @property
     def ensemble_model(self) -> EnsembleModel:
-        """Return the ensemble model."""
+        """The ensemble model."""
         return self._ensemble_model
 
     @property
     def num_models(self) -> int:
-        """Return the number of ensemble."""
+        """The number of ensemble."""
         return self._num_ensemble
 
     @property
     def state_size(self) -> int:
-        """Return the state size."""
+        """The state size."""
         return self._state_size
 
     # pylint: disable-next=too-many-locals, too-many-arguments
     def train(
         self,
         inputs: np.ndarray,
         labels: np.ndarray,
@@ -447,29 +559,34 @@
     ) -> tuple[np.ndarray, np.ndarray]:
         """Train the dynamics, holdout_ratio is the data ratio hold out for validation.
 
         Args:
             inputs (np.ndarray): Input data.
             labels (np.ndarray): Ground truth of the next state, reward, cost.
             holdout_ratio (float): The ratio of the data hold out for validation.
+
+        Returns:
+            train_mse_losses: The training loss.
+            val_mse_losses: The validation loss.
         """
         self._epochs_since_update = 0
         self._snapshots = {i: (0, 1e10) for i in range(self._num_ensemble)}
 
         num_holdout = int(inputs.shape[0] * holdout_ratio)
         permutation = np.random.permutation(inputs.shape[0])
         inputs, labels = inputs[permutation], labels[permutation]
 
         # split training and testing dataset
         train_inputs, train_labels = inputs[num_holdout:], labels[num_holdout:]
         holdout_inputs, holdout_labels = inputs[:num_holdout], labels[:num_holdout]
         self._ensemble_model.scaler.fit(train_inputs)
 
+        train_mse_losses = []
+        val_losses = []
         for epoch in itertools.count():
-            train_mse_losses = []
             # training
             train_idx = np.vstack(
                 [np.random.permutation(train_inputs.shape[0]) for _ in range(self._num_ensemble)],
             )
             # shape: [train_inputs.shape[0],num_ensemble]
 
             for start_pos in range(0, train_inputs.shape[0], self._batch_size):
@@ -483,17 +600,15 @@
 
             # validation
             val_idx = np.vstack(
                 [np.random.permutation(holdout_inputs.shape[0]) for _ in range(self._num_ensemble)],
             )
             val_batch_size = 512
             val_losses_list = []
-            for _len_valid, start_pos in enumerate(
-                range(0, holdout_inputs.shape[0], val_batch_size),
-            ):
+            for start_pos in range(0, holdout_inputs.shape[0], val_batch_size):
                 with torch.no_grad():
                     idx = val_idx[:, start_pos : start_pos + val_batch_size]
                     val_input = torch.from_numpy(holdout_inputs[idx]).float().to(self._device)
                     val_label = torch.from_numpy(holdout_labels[idx]).float().to(self._device)
                     holdout_mean, holdout_logvar = self._ensemble_model.forward(
                         val_input,
                         ret_log_var=True,
@@ -502,28 +617,38 @@
                         holdout_mean,
                         holdout_logvar,
                         val_label,
                         inc_var_loss=False,
                     )
                     holdout_mse_losses = holdout_mse_losses.detach().cpu().numpy()
                     val_losses_list.append(holdout_mse_losses)
-            val_losses = np.array(val_losses_list)
-            val_losses = np.sum(val_losses, axis=0) / (_len_valid + 1)
-            sorted_loss_idx = np.argsort(val_losses)
+            current_loss = np.sum(np.array(val_losses_list), axis=0) / (
+                int(holdout_inputs.shape[0] / val_batch_size) + 1
+            )
+            val_losses.append(current_loss)
+            sorted_loss_idx = np.argsort(current_loss)
             self.elite_model_idxes = sorted_loss_idx[: self._elite_size].tolist()
-            break_train = self._save_best(epoch, val_losses)
+            break_train = self._save_best(epoch, current_loss)
             if break_train:
                 break
 
         train_mse_losses = np.array(train_mse_losses).mean()
         val_mse_losses = np.array(val_losses).mean()
         return np.array(train_mse_losses), np.array(val_mse_losses)
 
     def _save_best(self, epoch: int, holdout_losses: list) -> bool:
-        """Save the best model."""
+        """Save the best model.
+
+        Args:
+            epoch (int): The current epoch.
+            holdout_losses (list): The holdout loss.
+
+        Returns:
+            Whether to break the training.
+        """
         updated = False
         for i, current_loss in enumerate(holdout_losses):
             _, best = self._snapshots[i]
             improvement = (best - current_loss) / best
             if improvement > 0.01:
                 self._snapshots[i] = (epoch, current_loss)
                 updated = True
@@ -535,41 +660,71 @@
         return self._epochs_since_update > self._max_epoch_since_update
 
     @torch.no_grad()
     def _compute_reward(
         self,
         network_output: torch.Tensor,
     ) -> torch.Tensor:
-        """Compute the reward from the network output."""
+        """Compute the reward from the network output.
+
+        Args:
+            network_output (torch.Tensor): The output of the network.
+
+        Returns:
+            reward: The reward, from the network output or the reward function.
+
+        Raises:
+            ValueError: If the reward function is not defined.
+        """
         if self._predict_reward:
             reward_start_dim = int(self._predict_cost) * self._cost_size
             reward_end_dim = reward_start_dim + self._reward_size
             return network_output[:, :, reward_start_dim:reward_end_dim]
         if self._rew_func is not None:
             return self._rew_func(network_output[:, :, self._state_start_dim :])
         raise ValueError('Reward function is not defined.')
 
     @torch.no_grad()
     def _compute_cost(
         self,
         network_output: torch.Tensor,
     ) -> torch.Tensor:
-        """Compute the cost from the network output."""
+        """Compute the cost from the network output.
+
+        Args:
+            network_output (torch.Tensor): The output of the network.
+
+        Returns:
+            cost: The cost, from the network output or the cost function.
+
+        Raises:
+            ValueError: If the cost function is not defined.
+        """
         if self._predict_cost:
             return network_output[:, :, : self._cost_size]
         if self._cost_func is not None:
             return self._cost_func(network_output[:, :, self._state_start_dim :])
         raise ValueError('Cost function is not defined.')
 
     @torch.no_grad()
     def _compute_terminal(
         self,
         network_output: torch.Tensor,
     ) -> torch.Tensor:
-        """Compute the terminal from the network output."""
+        """Compute the terminal from the network output.
+
+        Args:
+            network_output (torch.Tensor): The output of the network.
+
+        Returns:
+            terminal: The terminal signal, from the network output or the terminal function.
+
+        Raises:
+            ValueError: If the terminal function is not defined.
+        """
         if self._terminal_func is not None:
             return self._terminal_func(network_output[:, :, self._state_start_dim :])
         raise ValueError('Terminal function is not defined.')
 
     def _predict(
         self,
         inputs: torch.Tensor,
@@ -580,14 +735,18 @@
         """Input type and output type both are tensor, used for planning loop.
 
         Args:
             inputs (torch.Tensor): the inputs to the network.
             batch_size (int, optional): the batch size for prediction.
             idx (Union[int, None], optional): the index of the model to use.
             ret_log_var (bool, optional): whether to return the log variance.
+
+        Returns:
+            ensemble_mean_tensor: The mean of the ensemble.
+            ensemble_var_tensor: The variance of the ensemble.
         """
         if idx is not None:
             assert inputs.shape[0] == 1
         else:
             assert inputs.shape[0] == self._num_ensemble
         # input shape: [networ_size, (num_gaus+num_actor)*paritcle ,state_dim + action_dim]
         assert inputs.shape[2] == self._state_size + self._action_size
@@ -633,15 +792,15 @@
             actions (torch.Tensor): the actions.
             idx (Union[int, None], optional): the index of the model to use. Defaults to None.
             deterministic (bool, optional): whether to use the deterministic version of the model. Defaults to False.
 
         Returns:
             sample_states (torch.Tensor): the sampled states.
             rewards (torch.Tensor): the rewards.
-            info (Dict[str, List[torch.Tensor]]): the info dict, contains the costs if use_cost is True
+            info: the info dict, contains the costs if `use_cost` is True.
         """
         assert (
             states.shape[:-1] == actions.shape[:-1]
         ), 'states and actions must have the same shape except the last dimension'
         # shape: [network_size, (num_gaus+num_actor)*paritcle ,state_dim]
         inputs = torch.cat((states, actions), dim=-1)
 
@@ -703,15 +862,15 @@
             states (torch.Tensor): the states.
             horizon (int): the horizon.
             actions (torch.Tensor, optional): the actions.
             actor_critic (ConstraintActorQCritic, optional): the actor_critic to use if actions is None.
             idx (int, optional): the index of the model to use.
 
         Returns:
-            traj (Dict[str, List[torch.Tensor]]): the trajectory dict, contains the states, rewards, etc.
+            traj: the trajectory dict, contains the states, rewards, etc.
         """
         assert (
             states.shape[1] == self._state_size
         ), 'states should be of shape (batch_size, state_size)'
         num_ensemble = self._num_ensemble if idx is None else 1
         if actions is not None:
             assert actions.shape == torch.Size(
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/model_based/base/loop.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/model_based/base/loop.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,95 +10,118 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Implementation of the Learning Off-Policy with Online Planning algorithm."""
 
+
 from __future__ import annotations
 
 from typing import Any
 
 import torch
 from gymnasium.spaces import Box
 from torch import nn, optim
 from torch.nn.utils.clip_grad import clip_grad_norm_
 
-from omnisafe.adapter import ModelBasedAdapter
 from omnisafe.algorithms import registry
 from omnisafe.algorithms.model_based.base.ensemble import EnsembleDynamicsModel
 from omnisafe.algorithms.model_based.base.pets import PETS
 from omnisafe.algorithms.model_based.planner.arc import ARCPlanner
 from omnisafe.common.buffer import OffPolicyBuffer
 from omnisafe.models.actor_critic.constraint_actor_q_critic import ConstraintActorQCritic
+from omnisafe.typing import OmnisafeSpace
 
 
 @registry.register
 # pylint: disable-next=too-many-instance-attributes, too-few-public-methods
 class LOOP(PETS):
     """The Learning Off-Policy with Online Planning (LOOP) algorithm.
 
     References:
         - Title: Learning Off-Policy with Online Planning
         - Authors: Harshit Sikchi, Wenxuan Zhou, David Held.
         - URL: `LOOP <https://arxiv.org/abs/2008.10066>`_
     """
 
+    _log_alpha: torch.Tensor
+    _alpha_optimizer: optim.Optimizer
+    _target_entropy: float
+
     def _init_model(self) -> None:
-        """Initialize the dynamics model and the planner."""
-        self._dynamics_state_space = (
+        """Initialize the dynamics model and the planner.
+
+        LOOP uses following models:
+
+        - dynamics model: to predict the next state and the cost.
+        - actor_critic: to predict the action and the value.
+        - planner: to generate the action.
+        """
+        self._dynamics_state_space: OmnisafeSpace = (
             self._env.coordinate_observation_space
             if self._env.coordinate_observation_space is not None
             else self._env.observation_space
         )
+        assert self._dynamics_state_space is not None and isinstance(
+            self._dynamics_state_space.shape,
+            tuple,
+        )
         assert self._env.action_space is not None and isinstance(
             self._env.action_space.shape,
             tuple,
         )
         if isinstance(self._env.action_space, Box):
             self._action_space = self._env.action_space
         else:
             raise NotImplementedError
-        self._actor_critic = ConstraintActorQCritic(
+        self._actor_critic: ConstraintActorQCritic = ConstraintActorQCritic(
             obs_space=self._dynamics_state_space,
             act_space=self._env.action_space,
             model_cfgs=self._cfgs.model_cfgs,
             epochs=self._epochs,
         ).to(self._device)
-        self._use_actor_critic = True
-        self._update_count = 0
-        self._dynamics = EnsembleDynamicsModel(
+        self._use_actor_critic: bool = True
+        self._update_count: int = 0
+        self._dynamics: EnsembleDynamicsModel = EnsembleDynamicsModel(
             model_cfgs=self._cfgs.dynamics_cfgs,
             device=self._device,
             state_shape=self._dynamics_state_space.shape,
             action_shape=self._env.action_space.shape,
             actor_critic=self._actor_critic,
             rew_func=None,
             cost_func=None,
             terminal_func=None,
         )
         self._update_dynamics_cycle = int(self._cfgs.algo_cfgs.update_dynamics_cycle)
-        self._planner = ARCPlanner(
+        self._planner: ARCPlanner = ARCPlanner(
             dynamics=self._dynamics,
             planner_cfgs=self._cfgs.planner_cfgs,
             gamma=float(self._cfgs.algo_cfgs.gamma),
             cost_gamma=float(self._cfgs.algo_cfgs.cost_gamma),
             dynamics_state_shape=self._dynamics_state_space.shape,
             action_shape=self._action_space.shape,
             action_max=1.0,
             action_min=-1.0,
             device=self._device,
             actor_critic=self._actor_critic,
         )
 
     def _init(self) -> None:
+        """The initialization of the algorithm.
+
+        User can define the initialization of the algorithm by inheriting this method.
+
+        Examples:
+            >>> def _init(self) -> None:
+            ...     super()._init()
+            ...     self._buffer = CustomBuffer()
+            ...     self._model = CustomModel()
+        """
         super()._init()
-        self._log_alpha: torch.Tensor
-        self._alpha_optimizer: optim.Optimizer
-        self._target_entropy: float
 
         self._alpha = self._cfgs.algo_cfgs.alpha
         self._alpha_gamma = self._cfgs.algo_cfgs.alpha_gamma
         self._policy_buf = OffPolicyBuffer(
             obs_space=self._dynamics_state_space,
             act_space=self._env.action_space,
             size=self._cfgs.train_cfgs.total_steps,
@@ -107,15 +130,32 @@
         )
 
     def _alpha_discount(self) -> None:
         """Alpha discount."""
         self._alpha *= self._alpha_gamma
 
     def _init_log(self) -> None:
-        """Initialize logger."""
+        """Initialize logger.
+
+        +-------------------------+----------------------------------------------------------------------+
+        | Things to log           | Description                                                          |
+        +=========================+======================================================================+
+        | Value/alpha             | The value of alpha.                                                  |
+        +-------------------------+----------------------------------------------------------------------+
+        | Values/reward_critic    | Average value in :meth:`rollout` (from critic network) of the epoch. |
+        +-------------------------+----------------------------------------------------------------------+
+        | Values/cost_critic      | Average cost in :meth:`rollout` (from critic network) of the epoch.  |
+        +-------------------------+----------------------------------------------------------------------+
+        | Loss/Loss_cost_critic   | Loss of the cost critic network.                                     |
+        +-------------------------+----------------------------------------------------------------------+
+        | Loss/Loss_reward_critic | Loss of the cost critic network.                                     |
+        +-------------------------+----------------------------------------------------------------------+
+        | Loss/Loss_pi            | Loss of the policy network.                                          |
+        +-------------------------+----------------------------------------------------------------------+
+        """
         super()._init_log()
         self._logger.register_key('Value/alpha')
         # log information about actor
         self._logger.register_key('Loss/Loss_pi', delta=True)
 
         # log information about critic
         self._logger.register_key('Loss/Loss_reward_critic', delta=True)
@@ -140,44 +180,69 @@
         self._logger.setup_torch_saver(what_to_save)
         self._logger.torch_save()
 
     def _select_action(  # pylint: disable=unused-argument
         self,
         current_step: int,
         state: torch.Tensor,
-        env: ModelBasedAdapter,
-    ) -> tuple[torch.Tensor, dict]:
+    ) -> torch.Tensor:
         """Select action.
 
         Args:
-            current_step (int): current step
-            state (torch.Tensor): current state
-            env (ModelBasedAdapter): environment
+            current_step (int): The current step.
+            state (torch.Tensor): The current state.
 
         Returns:
-            action (torch.Tensor): action
-            action_info (dict): action information
+            The selected action.
         """
         if current_step < self._cfgs.algo_cfgs.start_learning_steps:
             action = torch.tensor(self._env.action_space.sample()).to(self._device).unsqueeze(0)
         else:
             action, info = self._planner.output_action(state)
             self._logger.store(**info)
 
         assert action.shape == torch.Size(
             [1, *self._action_space.shape],
         ), 'action shape should be [batch_size, action_dim]'
-        info = {}
-        return action, info
+        return action
 
     def _update_policy(self, current_step: int) -> None:
         """Update policy.
 
+        -  Get the ``data`` from buffer
+
+        .. note::
+
+            +----------+---------------------------------------+
+            | obs      | ``observaion`` stored in buffer.      |
+            +==========+=======================================+
+            | act      | ``action`` stored in buffer.          |
+            +----------+---------------------------------------+
+            | reward   | ``reward`` stored in buffer.          |
+            +----------+---------------------------------------+
+            | cost     | ``cost`` stored in buffer.            |
+            +----------+---------------------------------------+
+            | next_obs | ``next observaion`` stored in buffer. |
+            +----------+---------------------------------------+
+            | done     | ``terminated`` stored in buffer.      |
+            +----------+---------------------------------------+
+
+        -  Update value net by :meth:`_update_reward_critic`.
+        -  Update cost net by :meth:`_update_cost_critic`.
+        -  Update policy net by :meth:`_update_actor`.
+
+        The basic process of each update is as follows:
+
+        #. Get the mini-batch data from buffer.
+        #. Get the loss of network.
+        #. Update the network by loss.
+        #. Repeat steps 2, 3 until the ``update_policy_iters`` times.
+
         Args:
-            current_step (int): current step
+            current_step (int): The current step.
         """
         if current_step >= self._cfgs.algo_cfgs.start_learning_steps:
             for _step in range(self._cfgs.algo_cfgs.update_policy_iters):
                 self._update_count += 1
 
                 data = self._policy_buf.sample_batch()
                 obs, act, reward, cost, done, next_obs = (
@@ -214,40 +279,34 @@
                     self._actor_critic.polyak_update(self._cfgs.algo_cfgs.polyak)
 
                 if self._cfgs.algo_cfgs.alpha_discount:
                     self._alpha_discount()
 
     def _store_real_data(  # pylint: disable=too-many-arguments,unused-argument
         self,
-        current_step: int,
-        ep_len: int,
         state: torch.Tensor,
         action: torch.Tensor,
         reward: torch.Tensor,
         cost: torch.Tensor,
         terminated: torch.Tensor,
         truncated: torch.Tensor,
         next_state: torch.Tensor,
-        info: dict,
-        action_info: dict,
+        info: dict[str, Any],
     ) -> None:  # pylint: disable=too-many-arguments
         """Store real data in buffer.
 
         Args:
-            current_step (int): current step
-            ep_len (int): episode length
-            state (torch.Tensor): current state
-            action (torch.Tensor): action
-            reward (torch.Tensor): reward
-            cost (torch.Tensor): cost
-            terminated (torch.Tensor): terminated
-            truncated (torch.Tensor): truncated
-            next_state (torch.Tensor): next state
-            info (dict): information
-            action_info (dict): action information
+            state (torch.Tensor): The state from the environment.
+            action (torch.Tensor): The action from the agent.
+            reward (torch.Tensor): The reward signal from the environment.
+            cost (torch.Tensor): The cost signal from the environment.
+            terminated (torch.Tensor): The terminated signal from the environment.
+            truncated (torch.Tensor): The truncated signal from the environment.
+            next_state (torch.Tensor): The next state from the environment.
+            info (dict[str, Any]): The information from the environment.
         """
         done = terminated or truncated
         goal_met = False if 'goal_met' not in info.keys() else info['goal_met']
         if not done and not goal_met:
             # when goal_met == true:
             # current goal position is not related to the last goal position,
             # this huge transition will confuse the dynamics model.
@@ -275,20 +334,24 @@
         action: torch.Tensor,
         reward: torch.Tensor,
         done: torch.Tensor,
         next_obs: torch.Tensor,
     ) -> None:
         """Update reward critic using Soft Actor-Critic.
 
+        - Get the TD loss of reward critic.
+        - Update critic network by loss.
+        - Log useful information.
+
         Args:
-            obs (torch.Tensor): observation
-            action (torch.Tensor): action
-            reward (torch.Tensor): reward
-            done (torch.Tensor): done
-            next_obs (torch.Tensor): next observation
+            obs (torch.Tensor): The ``observation`` sampled from buffer.
+            action (torch.Tensor): The ``action`` sampled from buffer.
+            reward (torch.Tensor): The ``reward`` sampled from buffer.
+            done (torch.Tensor): The ``terminated`` sampled from buffer.
+            next_obs (torch.Tensor): The ``next observation`` sampled from buffer.
         """
         self._actor_critic.reward_critic_optimizer.zero_grad()
 
         with torch.no_grad():
             next_action = self._actor_critic.actor.predict(next_obs, deterministic=False)
             next_logp = self._actor_critic.actor.log_prob(next_action)
             next_q1_value_r, next_q2_value_r = self._actor_critic.target_reward_critic(
@@ -327,20 +390,24 @@
         action: torch.Tensor,
         cost: torch.Tensor,
         done: torch.Tensor,
         next_obs: torch.Tensor,
     ) -> None:
         """Update cost critic using TD3 algorithm.
 
+        - Get the TD loss of cost critic.
+        - Update critic network by loss.
+        - Log useful information.
+
         Args:
-            obs (torch.Tensor): current observation
-            action (torch.Tensor): current action
-            cost (torch.Tensor): current cost
-            done (torch.Tensor): current done signal
-            next_obs (torch.Tensor): next observation
+            obs (torch.Tensor): The ``observation`` sampled from buffer.
+            action (torch.Tensor): The ``action`` sampled from buffer.
+            cost (torch.Tensor): The ``cost`` sampled from buffer.
+            done (torch.Tensor): The ``terminated`` sampled from buffer.
+            next_obs (torch.Tensor): The ``next observation`` sampled from buffer.
         """
         with torch.no_grad():
             next_action = self._actor_critic.actor.predict(next_obs, deterministic=True)
             next_q_value_c = self._actor_critic.target_cost_critic(next_obs, next_action)[0]
             target_q_value_c = cost + self._cfgs.algo_cfgs.gamma * (1 - done) * next_q_value_c
         q_value_c = self._actor_critic.cost_critic(obs, action)[0]
         loss = nn.functional.mse_loss(q_value_c, target_q_value_c)
@@ -368,16 +435,20 @@
 
     def _update_actor(
         self,
         obs: torch.Tensor,
     ) -> None:
         """Update actor using Soft Actor-Critic algorithm.
 
+        - Get the loss of actor.
+        - Update actor by loss.
+        - Log useful information.
+
         Args:
-            obs (torch.Tensor): observation
+            obs (torch.Tensor): The ``observation`` sampled from buffer.
         """
         self._actor_critic.actor_optimizer.zero_grad()
         loss = self._loss_pi(obs)
         loss.backward()
         if self._cfgs.algo_cfgs.use_grad_norm:
             clip_grad_norm_(
                 self._actor_critic.actor.parameters(),
@@ -396,36 +467,31 @@
             },
         )
 
     def _loss_pi(
         self,
         obs: torch.Tensor,
     ) -> torch.Tensor:
-        """Compute loss for actor using Soft Actor-Critic algorithm.
+        r"""Computing ``pi/actor`` loss.
+
+        The loss function in SAC is defined as:
+
+        .. math::
+
+            L = -Q^V (s, \pi (s)) + \alpha \log \pi (s)
+
+        where :math:`Q^V` is the min value of two reward critic networks, and :math:`\pi` is the
+        policy network, and :math:`\alpha` is the temperature parameter.
 
         Args:
-            obs (torch.Tensor): observation
+            obs (torch.Tensor): The ``observation`` sampled from buffer.
+
+        Returns:
+            The loss of pi/actor.
         """
         action = self._actor_critic.actor.predict(
             obs,
             deterministic=self._cfgs.algo_cfgs.loss_pi_deterministic,
         )
         log_prob = self._actor_critic.actor.log_prob(action)
         q1_value_r, q2_value_r = self._actor_critic.reward_critic(obs, action)
         return (self._alpha * log_prob - torch.min(q1_value_r, q2_value_r)).mean()
-
-    def _log_when_not_update(self) -> None:
-        """Log when not update."""
-        self._logger.store(
-            **{
-                'Loss/Loss_reward_critic': 0.0,
-                'Loss/Loss_pi': 0.0,
-                'Value/reward_critic': 0.0,
-            },
-        )
-        if self._cfgs.algo_cfgs.use_cost:
-            self._logger.store(
-                **{
-                    'Loss/Loss_cost_critic': 0.0,
-                    'Value/cost_critic': 0.0,
-                },
-            )
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/model_based/base/pets.py` & `omnisafe-0.5.0b0/omnisafe/evaluator.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,491 +8,547 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Implementation of the Probabilistic Ensembles with Trajectory Sampling algorithm."""
+"""Implementation of Evaluator."""
+
 from __future__ import annotations
 
+import json
 import os
-import time
+import warnings
 from typing import Any
 
 import numpy as np
 import torch
 from gymnasium.spaces import Box
 from gymnasium.utils.save_video import save_video
-from matplotlib import pylab
 
-from omnisafe.adapter import ModelBasedAdapter
-from omnisafe.algorithms import registry
-from omnisafe.algorithms.base_algo import BaseAlgo
 from omnisafe.algorithms.model_based.base.ensemble import EnsembleDynamicsModel
-from omnisafe.algorithms.model_based.planner.cem import CEMPlanner
-from omnisafe.common.buffer import OffPolicyBuffer
-from omnisafe.common.logger import Logger
+from omnisafe.algorithms.model_based.planner import (
+    ARCPlanner,
+    CAPPlanner,
+    CCEPlanner,
+    CEMPlanner,
+    RCEPlanner,
+    SafeARCPlanner,
+)
+from omnisafe.common import Normalizer
+from omnisafe.envs.core import CMDP, make
+from omnisafe.envs.wrapper import ActionRepeat, ActionScale, ObsNormalize, TimeLimit
+from omnisafe.models.actor import ActorBuilder
+from omnisafe.models.actor_critic import ConstraintActorCritic, ConstraintActorQCritic
+from omnisafe.models.base import Actor
+from omnisafe.utils.config import Config
+
+
+class Evaluator:  # pylint: disable=too-many-instance-attributes
+    """This class includes common evaluation methods for safe RL algorithms.
+
+    Args:
+        env (CMDP or None, optional): The environment. Defaults to None.
+        actor (Actor or None, optional): The actor. Defaults to None.
+        render_mode (str, optional): The render mode. Defaults to 'rgb_array'.
+    """
 
+    _cfgs: Config
+    _save_dir: str
+    _model_name: str
+    _cost_count: torch.Tensor
 
-@registry.register
-# pylint: disable-next=too-many-instance-attributes, too-few-public-methods
-class PETS(BaseAlgo):
-    """The Probabilistic Ensembles with Trajectory Sampling (PETS) algorithm.
-
-    References:
-        - Title: Deep Reinforcement Learning in a Handful of Trials using Probabilistic Dynamics Models
-        - Authors: Kurtland Chua, Roberto Calandra, Rowan McAllister, Sergey Levine.
-        - URL: `PETS <https://arxiv.org/abs/1805.12114>`_
-    """
+    # pylint: disable-next=too-many-arguments
+    def __init__(
+        self,
+        env: CMDP | None = None,
+        actor: Actor | None = None,
+        actor_critic: ConstraintActorCritic | ConstraintActorQCritic | None = None,
+        dynamics: EnsembleDynamicsModel | None = None,
+        planner: CEMPlanner
+        | ARCPlanner
+        | SafeARCPlanner
+        | CCEPlanner
+        | CAPPlanner
+        | RCEPlanner
+        | None = None,
+        render_mode: str = 'rgb_array',
+    ) -> None:
+        """Initialize an instance of :class:`Evaluator`."""
+        self._env: CMDP | None = env
+        self._actor: Actor | None = actor
+        self._actor_critic: ConstraintActorCritic | ConstraintActorQCritic | None = actor_critic
+        self._dynamics: EnsembleDynamicsModel | None = dynamics
+        self._planner = planner
+        self._dividing_line: str = '\n' + '#' * 50 + '\n'
+
+        self._safety_budget: torch.Tensor
+        self._safety_obs = torch.ones(1)
+        self._cost_count = torch.zeros(1)
+        self.__set_render_mode(render_mode)
 
-    def _init_env(self) -> None:
-        self._env = ModelBasedAdapter(
-            self._env_id,
-            1,
-            self._seed,
-            self._cfgs,
-        )
-        self._total_steps = int(self._cfgs.train_cfgs.total_steps)
-        self._steps_per_epoch = int(self._cfgs.algo_cfgs.steps_per_epoch)
-        self._epochs = self._total_steps // self._cfgs.algo_cfgs.steps_per_epoch
-        print(f'Total steps: {self._total_steps}, epochs: {self._epochs}')
-
-    def _init_model(self) -> None:
-        """Initialize dynamics model and planner."""
-        self._dynamics_state_space = (
-            self._env.coordinate_observation_space
-            if self._env.coordinate_observation_space is not None
-            else self._env.observation_space
-        )
-        if isinstance(self._env.action_space, Box):
-            self._action_space = self._env.action_space
-        else:
-            raise NotImplementedError
-        self._dynamics = EnsembleDynamicsModel(
-            model_cfgs=self._cfgs.dynamics_cfgs,
-            device=self._device,
-            state_shape=self._dynamics_state_space.shape,
-            action_shape=self._action_space.shape,
-            actor_critic=None,
-            rew_func=None,
-            cost_func=None,
-            terminal_func=None,
-        )
+    def __set_render_mode(self, render_mode: str) -> None:
+        """Set the render mode.
 
-        self._planner = CEMPlanner(
-            dynamics=self._dynamics,
-            planner_cfgs=self._cfgs.planner_cfgs,
-            gamma=float(self._cfgs.algo_cfgs.gamma),
-            cost_gamma=float(self._cfgs.algo_cfgs.cost_gamma),
-            dynamics_state_shape=self._dynamics_state_space.shape,
-            action_shape=self._action_space.shape,
-            action_max=1.0,
-            action_min=-1.0,
-            device=self._device,
-        )
-        self._use_actor_critic = False
-        self._update_dynamics_cycle = int(self._cfgs.algo_cfgs.update_dynamics_cycle)
+        Args:
+            render_mode (str, optional): The render mode. Defaults to 'rgb_array'.
 
-    def _init(self) -> None:
-        """Initialize the algorithm."""
-        self._dynamics_buf = OffPolicyBuffer(
-            obs_space=self._dynamics_state_space,
-            act_space=self._env.action_space,
-            size=self._cfgs.train_cfgs.total_steps,
-            batch_size=self._cfgs.dynamics_cfgs.batch_size,
-            device=self._device,
-        )
-        env_kwargs: dict[str, Any] = {
-            'render_mode': 'rgb_array',
-            'camera_name': 'track',
-        }
-        self._eval_env = ModelBasedAdapter(
-            self._env_id,
-            1,
-            self._seed,
-            self._cfgs,
-            **env_kwargs,
-        )
-        self._eval_fn = self._evaluation_single_step
+        Raises:
+            NotImplementedError: If the render mode is not implemented.
+        """
+        # set the render mode
+        if render_mode in ['human', 'rgb_array', 'rgb_array_list']:
+            self._render_mode: str = render_mode
+        else:
+            raise NotImplementedError('The render mode is not implemented.')
 
-    def _init_log(self) -> None:
-        """Initialize logger."""
-        self._logger = Logger(
-            output_dir=self._cfgs.logger_cfgs.log_dir,
-            exp_name=self._cfgs.exp_name,
-            seed=self._cfgs.seed,
-            use_tensorboard=self._cfgs.logger_cfgs.use_tensorboard,
-            use_wandb=self._cfgs.logger_cfgs.use_wandb,
-            config=self._cfgs,
-        )
+    def __load_cfgs(self, save_dir: str) -> None:
+        """Load the config from the save directory.
 
-        self._logger.register_key('Train/Epoch')
-        self._logger.register_key('TotalEnvSteps')
-        self._logger.register_key('Metrics/EpRet', window_length=50)
-        self._logger.register_key('Metrics/EpCost', window_length=50)
-        self._logger.register_key('Metrics/EpLen', window_length=50)
-        if self._cfgs.evaluation_cfgs.use_eval:
-            self._logger.register_key('EvalMetrics/EpRet', window_length=5)
-            self._logger.register_key('EvalMetrics/EpCost', window_length=5)
-            self._logger.register_key('EvalMetrics/EpLen', window_length=5)
-        self._logger.register_key('Loss/DynamicsTrainMseLoss')
-        self._logger.register_key('Loss/DynamicsValMseLoss')
-
-        self._logger.register_key('Plan/iter')
-        self._logger.register_key('Plan/last_var_mean')
-        self._logger.register_key('Plan/last_var_max')
-        self._logger.register_key('Plan/last_var_min')
-        self._logger.register_key('Plan/episode_returns_max')
-        self._logger.register_key('Plan/episode_returns_mean')
-        self._logger.register_key('Plan/episode_returns_min')
-
-        self._logger.register_key('Time/Total')
-        self._logger.register_key('Time/Rollout')
-        self._logger.register_key('Time/UpdateDynamics')
-        if self._use_actor_critic:
-            self._logger.register_key('Time/UpdateActorCritic')
-        if self._cfgs.evaluation_cfgs.use_eval:
-            self._logger.register_key('Time/Eval')
-        self._logger.register_key('Time/Epoch')
-        self._logger.register_key('Time/FPS')
-        self._save_model()
-
-    def _save_model(self) -> None:
-        """Save the model."""
-        what_to_save: dict[str, Any] = {}
-        # set up model saving
-        what_to_save = {
-            'dynamics': self._dynamics.ensemble_model,
-        }
-        if self._cfgs.algo_cfgs.obs_normalize:
-            obs_normalizer = self._env.save()['obs_normalizer']
-            what_to_save['obs_normalizer'] = obs_normalizer
-        self._logger.setup_torch_saver(what_to_save)
-        self._logger.torch_save()
-
-    def learn(self) -> tuple[float, float, int]:
-        """This is main function for algorithm update.
-
-        It is divided into the following steps:
-        - :meth:`rollout`: collect interactive data from environment.
-        - :meth:`update`: perform actor/critic updates.
-        - :meth:`log`: epoch/update information for visualization and terminal log print.
+        Args:
+            save_dir (str): Directory where the model is saved.
 
-        Returns:
-            ep_ret: average episode return in final epoch.
-            ep_cost: average episode cost in final epoch.
-            ep_len: average episode length in final epoch.
+        Raises:
+            FileNotFoundError: If the config file is not found.
         """
-        self._logger.log('INFO: Start training')
-        start_time = time.time()
-        current_step = 0
-        for epoch in range(self._epochs):
-            current_step = self._env.roll_out(
-                current_step=current_step,
-                roll_out_step=self._steps_per_epoch,
-                use_actor_critic=self._use_actor_critic,
-                act_func=self._select_action,
-                store_data_func=self._store_real_data,
-                update_dynamics_func=self._update_dynamics_model,
-                use_eval=self._cfgs.evaluation_cfgs.use_eval,
-                eval_func=self._eval_fn,
-                logger=self._logger,
-                algo_reset_func=self._algo_reset,
-                update_actor_func=self._update_policy,
-            )
-            if current_step > self._cfgs.algo_cfgs.start_learning_steps:
-                # update something per epoch
-                # e.g. update lagrange multiplier
-                self._update_epoch()
-            # evaluate episode
-            self._logger.store(
-                **{
-                    'Train/Epoch': epoch,
-                    'TotalEnvSteps': current_step,
-                    'Time/Total': time.time() - start_time,
-                },
-            )
-            self._logger.dump_tabular()
-            # save model to disk
-            if (epoch + 1) % self._cfgs.logger_cfgs.save_model_freq == 0:
-                self._logger.torch_save()
-
-        ep_ret = self._logger.get_stats('Metrics/EpRet')[0]
-        ep_cost = self._logger.get_stats('Metrics/EpCost')[0]
-        ep_len = int(self._logger.get_stats('Metrics/EpLen')[0])
-        self._logger.close()
+        cfg_path = os.path.join(save_dir, 'config.json')
+        try:
+            with open(cfg_path, encoding='utf-8') as file:
+                kwargs = json.load(file)
+        except FileNotFoundError as error:
+            raise FileNotFoundError(
+                f'The config file is not found in the save directory{save_dir}.',
+            ) from error
+        self._cfgs = Config.dict2config(kwargs)
 
-        return ep_ret, ep_cost, ep_len
-
-    def _algo_reset(
+    # pylint: disable-next=too-many-branches
+    def __load_model_and_env(
         self,
-        current_step: int,  # pylint: disable=unused-argument
+        save_dir: str,
+        model_name: str,
+        env_kwargs: dict[str, Any],
     ) -> None:
-        ...
+        """Load the model from the save directory.
 
-    def _update_policy(
-        self,
-        current_step: int,  # pylint: disable=unused-argument
-    ) -> None:
-        ...
+        Args:
+            save_dir (str): Directory where the model is saved.
+            model_name (str): Name of the model.
+            env_kwargs (dict[str, Any]): Keyword arguments for the environment.
+
+        Raises:
+            FileNotFoundError: If the model is not found.
+        """
+        # load the saved model
+        model_path = os.path.join(save_dir, 'torch_save', model_name)
+        try:
+            model_params = torch.load(model_path)
+        except FileNotFoundError as error:
+            raise FileNotFoundError('The model is not found in the save directory.') from error
+
+        # load the environment
+        self._env = make(**env_kwargs)
+
+        observation_space = self._env.observation_space
+        action_space = self._env.action_space
+        if 'Saute' in self._cfgs['algo'] or 'Simmer' in self._cfgs['algo']:
+            self._safety_budget = (
+                self._cfgs.algo_cfgs.safety_budget
+                * (1 - self._cfgs.algo_cfgs.saute_gamma**self._cfgs.algo_cfgs.max_ep_len)
+                / (1 - self._cfgs.algo_cfgs.saute_gamma)
+                / self._cfgs.algo_cfgs.max_ep_len
+                * torch.ones(1)
+            )
+        assert isinstance(observation_space, Box), 'The observation space must be Box.'
+        assert isinstance(action_space, Box), 'The action space must be Box.'
+
+        if self._cfgs['algo_cfgs']['obs_normalize']:
+            obs_normalizer = Normalizer(shape=observation_space.shape, clip=5)
+            obs_normalizer.load_state_dict(model_params['obs_normalizer'])
+            self._env = ObsNormalize(self._env, device=torch.device('cpu'), norm=obs_normalizer)
+        if self._env.need_time_limit_wrapper:
+            self._env = TimeLimit(self._env, device=torch.device('cpu'), time_limit=1000)
+        self._env = ActionScale(self._env, device=torch.device('cpu'), low=-1.0, high=1.0)
+
+        if hasattr(self._cfgs['algo_cfgs'], 'action_repeat'):
+            self._env = ActionRepeat(
+                self._env,
+                device=torch.device('cpu'),
+                times=self._cfgs['algo_cfgs']['action_repeat'],
+            )
+        if hasattr(self._cfgs, 'algo') and self._cfgs['algo'] in [
+            'LOOP',
+            'SafeLOOP',
+            'PETS',
+            'CAPPETS',
+            'RCEPETS',
+            'CCEPETS',
+        ]:
+            dynamics_state_space = (
+                self._env.coordinate_observation_space
+                if self._env.coordinate_observation_space is not None
+                else self._env.observation_space
+            )
+            assert self._env.action_space is not None and isinstance(
+                self._env.action_space.shape,
+                tuple,
+            )
+            if isinstance(self._env.action_space, Box):
+                action_space = self._env.action_space
+            else:
+                raise NotImplementedError
+            if self._cfgs['algo'] in ['LOOP', 'SafeLOOP']:
+                self._actor_critic = ConstraintActorQCritic(
+                    obs_space=dynamics_state_space,
+                    act_space=action_space,
+                    model_cfgs=self._cfgs.model_cfgs,
+                    epochs=1,
+                )
+            if self._actor_critic is not None:
+                self._actor_critic.load_state_dict(model_params['actor_critic'])
+                self._actor_critic.to('cpu')
+            self._dynamics = EnsembleDynamicsModel(
+                model_cfgs=self._cfgs.dynamics_cfgs,
+                device=torch.device('cpu'),
+                state_shape=dynamics_state_space.shape,
+                action_shape=action_space.shape,
+                actor_critic=self._actor_critic,
+                rew_func=None,
+                cost_func=self._env.get_cost_from_obs_tensor,
+                terminal_func=None,
+            )
+            self._dynamics.ensemble_model.load_state_dict(model_params['dynamics'])
+            self._dynamics.ensemble_model.to('cpu')
+            if self._cfgs['algo'] in ['CCEPETS', 'RCEPETS', 'SafeLOOP']:
+                algo_to_planner = {
+                    'CCEPETS': (
+                        'CCEPlanner',
+                        {'cost_limit': self._cfgs['algo_cfgs']['cost_limit']},
+                    ),
+                    'RCEPETS': (
+                        'RCEPlanner',
+                        {'cost_limit': self._cfgs['algo_cfgs']['cost_limit']},
+                    ),
+                    'SafeLOOP': (
+                        'SafeARCPlanner',
+                        {
+                            'cost_limit': self._cfgs['algo_cfgs']['cost_limit'],
+                            'actor_critic': self._actor_critic,
+                        },
+                    ),
+                }
+            elif self._cfgs['algo'] in ['PETS', 'LOOP']:
+                algo_to_planner = {
+                    'PETS': ('CEMPlanner', {}),
+                    'LOOP': ('ARCPlanner', {'actor_critic': self._actor_critic}),
+                }
+            elif self._cfgs['algo'] in ['CAPPETS']:
+                lagrange: torch.nn.Parameter = torch.nn.Parameter(
+                    model_params['lagrangian_multiplier'].to('cpu'),
+                    requires_grad=False,
+                )
+                algo_to_planner = {
+                    'CAPPETS': (
+                        'CAPPlanner',
+                        {
+                            'cost_limit': self._cfgs['lagrange_cfgs']['cost_limit'],
+                            'lagrange': lagrange,
+                        },
+                    ),
+                }
+            planner_name = algo_to_planner[self._cfgs['algo']][0]
+            planner_special_cfgs = algo_to_planner[self._cfgs['algo']][1]
+            planner_cls = globals()[f'{planner_name}']
+            self._planner = planner_cls(
+                dynamics=self._dynamics,
+                planner_cfgs=self._cfgs.planner_cfgs,
+                gamma=float(self._cfgs.algo_cfgs.gamma),
+                cost_gamma=float(self._cfgs.algo_cfgs.cost_gamma),
+                dynamics_state_shape=dynamics_state_space.shape,
+                action_shape=action_space.shape,
+                action_max=1.0,
+                action_min=-1.0,
+                device='cpu',
+                **planner_special_cfgs,
+            )
 
-    def _update_dynamics_model(
+        else:
+            if 'Saute' in self._cfgs['algo'] or 'Simmer' in self._cfgs['algo']:
+                observation_space = Box(
+                    low=np.hstack((observation_space.low, -np.inf)),
+                    high=np.hstack((observation_space.high, np.inf)),
+                    shape=(observation_space.shape[0] + 1,),
+                )
+            actor_type = self._cfgs['model_cfgs']['actor_type']
+            pi_cfg = self._cfgs['model_cfgs']['actor']
+            weight_initialization_mode = self._cfgs['model_cfgs']['weight_initialization_mode']
+            actor_builder = ActorBuilder(
+                obs_space=observation_space,
+                act_space=action_space,
+                hidden_sizes=pi_cfg['hidden_sizes'],
+                activation=pi_cfg['activation'],
+                weight_initialization_mode=weight_initialization_mode,
+            )
+            self._actor = actor_builder.build_actor(actor_type)
+            self._actor.load_state_dict(model_params['pi'])
+
+    # pylint: disable-next=too-many-locals
+    def load_saved(
         self,
-        current_step: int,  # pylint: disable=unused-argument
+        save_dir: str,
+        model_name: str,
+        render_mode: str = 'rgb_array',
+        camera_name: str | None = None,
+        camera_id: int | None = None,
+        width: int = 256,
+        height: int = 256,
     ) -> None:
-        """Update dynamics.
+        """Load a saved model.
 
         Args:
-            current_step (int): current step.
+            save_dir (str): The directory where the model is saved.
+            model_name (str): The name of the model.
+            render_mode (str, optional): The render mode, ranging from 'human', 'rgb_array',
+                'rgb_array_list'. Defaults to 'rgb_array'.
+            camera_name (str or None, optional): The name of the camera. Defaults to None.
+            camera_id (int or None, optional): The id of the camera. Defaults to None.
+            width (int, optional): The width of the image. Defaults to 256.
+            height (int, optional): The height of the image. Defaults to 256.
         """
-        state = self._dynamics_buf.data['obs'][: self._dynamics_buf.size, :]
-        action = self._dynamics_buf.data['act'][: self._dynamics_buf.size, :]
-        reward = self._dynamics_buf.data['reward'][: self._dynamics_buf.size]
-        cost = self._dynamics_buf.data['cost'][: self._dynamics_buf.size]
-        next_state = self._dynamics_buf.data['next_obs'][: self._dynamics_buf.size, :]
-        delta_state = next_state - state
-        if torch.is_tensor(delta_state):
-            inputs = torch.cat((state, action), -1)
-            inputs = torch.reshape(inputs, (inputs.shape[0], -1))
-
-            labels = torch.reshape(delta_state, (delta_state.shape[0], -1))
-            if self._cfgs.dynamics_cfgs.predict_reward:
-                labels = torch.cat(((torch.reshape(reward, (reward.shape[0], -1))), labels), -1)
-            if self._cfgs.dynamics_cfgs.predict_cost:
-                labels = torch.cat(((torch.reshape(cost, (cost.shape[0], -1))), labels), -1)
-            inputs = inputs.cpu().detach().numpy()
-            labels = labels.cpu().detach().numpy()
-        assert not torch.is_tensor(inputs) and not torch.is_tensor(
-            labels,
-        ), 'inputs and labels should be numpy array'
-        train_mse_losses, val_mse_losses = self._dynamics.train(
-            inputs,
-            labels,
-            holdout_ratio=0.2,
-        )
-        self._logger.store(
-            **{
-                'Loss/DynamicsTrainMseLoss': train_mse_losses.item(),
-                'Loss/DynamicsValMseLoss': val_mse_losses.item(),
-            },
-        )
+        # load the config
+        self._save_dir = save_dir
+        self._model_name = model_name
+
+        self.__load_cfgs(save_dir)
+
+        self.__set_render_mode(render_mode)
+
+        env_kwargs = {
+            'env_id': self._cfgs['env_id'],
+            'num_envs': 1,
+            'render_mode': self._render_mode,
+            'camera_id': camera_id,
+            'camera_name': camera_name,
+            'width': width,
+            'height': height,
+        }
 
-    def _update_epoch(self) -> None:
-        ...
+        self.__load_model_and_env(save_dir, model_name, env_kwargs)
 
-    def _select_action(  # pylint: disable=unused-argument
+    def evaluate(
         self,
-        current_step: int,
-        state: torch.Tensor,
-        env: ModelBasedAdapter,
-    ) -> tuple[torch.Tensor, dict]:
-        """Action selection.
+        num_episodes: int = 10,
+        cost_criteria: float = 1.0,
+    ) -> tuple[list[float], list[float]]:
+        """Evaluate the agent for num_episodes episodes.
 
         Args:
-            current_step (int): current step.
-            state (torch.Tensor): current state.
-            env (ModelBasedAdapter): environment.
+            num_episodes (int, optional): The number of episodes to evaluate. Defaults to 10.
+            cost_criteria (float, optional): The cost criteria. Defaults to 1.0.
 
         Returns:
-            action (torch.Tensor): action.
-            info (dict): information.
+            (episode_rewards, episode_costs): The episode rewards and costs.
+
+        Raises:
+            ValueError: If the environment and the policy are not provided or created.
         """
-        assert state.shape[0] == 1, 'state shape should be [1, state_dim]'
-        if current_step < self._cfgs.algo_cfgs.start_learning_steps:
-            action = torch.tensor(self._env.action_space.sample()).to(self._device).unsqueeze(0)
-        else:
-            action, info = self._planner.output_action(state)
-            self._logger.store(**info)
-        assert action.shape == torch.Size(
-            [1, *self._action_space.shape],
-        ), 'action shape should be [batch_size, action_dim]'
-        info = {}
-        return action, info
+        if self._env is None or (self._actor is None and self._planner is None):
+            raise ValueError(
+                'The environment and the policy must be provided or created before evaluating the agent.',
+            )
 
-    def _store_real_data(  # pylint: disable=too-many-arguments,unused-argument
-        self,
-        current_step: int,
-        ep_len: int,
-        state: torch.Tensor,
-        action: torch.Tensor,
-        reward: torch.Tensor,
-        cost: torch.Tensor,
-        terminated: torch.Tensor,
-        truncated: torch.Tensor,
-        next_state: torch.Tensor,
-        info: dict,
-        action_info: dict,
-    ) -> None:  # pylint: disable=too-many-arguments
-        """Store real data in buffer.
+        episode_rewards: list[float] = []
+        episode_costs: list[float] = []
+        episode_lengths: list[float] = []
+
+        for episode in range(num_episodes):
+            obs, _ = self._env.reset()
+            self._safety_obs = torch.ones(1)
+            ep_ret, ep_cost, length = 0.0, 0.0, 0.0
+
+            done = False
+            while not done:
+                if 'Saute' in self._cfgs['algo'] or 'Simmer' in self._cfgs['algo']:
+                    obs = torch.cat([obs, self._safety_obs], dim=-1)
+                with torch.no_grad():
+                    if self._actor is not None:
+                        act = self._actor.predict(
+                            obs,
+                            deterministic=True,
+                        )
+                    elif self._planner is not None:
+                        act = self._planner.output_action(
+                            obs.unsqueeze(0).to('cpu'),
+                        )[
+                            0
+                        ].squeeze(0)
+                    else:
+                        raise ValueError(
+                            'The policy must be provided or created before evaluating the agent.',
+                        )
+                obs, rew, cost, terminated, truncated, _ = self._env.step(act)
+                if 'Saute' in self._cfgs['algo'] or 'Simmer' in self._cfgs['algo']:
+                    self._safety_obs -= cost.unsqueeze(-1) / self._safety_budget
+                    self._safety_obs /= self._cfgs.algo_cfgs.saute_gamma
+
+                ep_ret += rew.item()
+                ep_cost += (cost_criteria**length) * cost.item()
+                if (
+                    'EarlyTerminated' in self._cfgs['algo']
+                    and ep_cost >= self._cfgs.algo_cfgs.cost_limit
+                ):
+                    terminated = torch.as_tensor(True)
+                length += 1
+
+                done = bool(terminated or truncated)
+
+            episode_rewards.append(ep_ret)
+            episode_costs.append(ep_cost)
+            episode_lengths.append(length)
+
+            print(f'Episode {episode+1} results:')
+            print(f'Episode reward: {ep_ret}')
+            print(f'Episode cost: {ep_cost}')
+            print(f'Episode length: {length}')
+
+        print(self._dividing_line)
+        print('Evaluation results:')
+        print(f'Average episode reward: {np.mean(a=episode_rewards)}')
+        print(f'Average episode cost: {np.mean(a=episode_costs)}')
+        print(f'Average episode length: {np.mean(a=episode_lengths)}')
+        return (
+            episode_rewards,
+            episode_costs,
+        )
 
-        Args:
-            current_step (int): current step.
-            ep_len (int): episode length.
-            state (torch.Tensor): current state.
-            action (torch.Tensor): action.
-            reward (torch.Tensor): reward.
-            cost (torch.Tensor): cost.
-            terminated (torch.Tensor): terminated.
-            truncated (torch.Tensor): truncated.
-            next_state (torch.Tensor): next state.
-            info (dict): information.
-            action_info (dict): action information.
+    @property
+    def fps(self) -> int:
+        """The fps of the environment.
+
+        Raises:
+            AssertionError: If the environment is not provided or created.
+            AtrributeError: If the fps is not found.
         """
-        done = terminated or truncated
-        goal_met = False if 'goal_met' not in info.keys() else info['goal_met']
-        if not terminated and not truncated and not goal_met:
-            # pylint: disable-next=line-too-long
-            # if goal_met == true, Current goal position is not related to the last goal position, this huge transition will confuse the dynamics model.
-            self._dynamics_buf.store(
-                obs=state,
-                act=action,
-                reward=reward,
-                cost=cost,
-                next_obs=next_state,
-                done=done,
-            )
+        assert (
+            self._env is not None
+        ), 'The environment must be provided or created before getting the fps.'
+        try:
+            fps = self._env.metadata['render_fps']
+        except AttributeError:
+            fps = 30
+            warnings.warn('The fps is not found, use 30 as default.', stacklevel=2)
+
+        return fps
 
-    def _evaluation_single_step(  # pylint: disable=too-many-locals
+    def render(  # pylint: disable=too-many-locals,too-many-arguments,too-many-branches,too-many-statements
         self,
-        current_step: int,
-        use_real_input: bool = True,
-    ) -> None:
-        """Evaluation dynamics model single step.
+        num_episodes: int = 1,
+        save_replay_path: str | None = None,
+        max_render_steps: int = 2000,
+        cost_criteria: float = 1.0,
+    ) -> None:  # pragma: no cover
+        """Render the environment for one episode.
 
         Args:
-            current_step (int): current step.
-            use_real_input (bool): use real input or not.
-
+            num_episodes (int, optional): The number of episodes to render. Defaults to 1.
+            save_replay_path (str or None, optional): The path to save the replay video. Defaults to
+                None.
+            max_render_steps (int, optional): The maximum number of steps to render. Defaults to 2000.
+            cost_criteria (float, optional): The discount factor for the cost. Defaults to 1.0.
         """
-        obs, _ = self._eval_env.reset()
-        obs_dynamics = obs
-        ep_len, ep_ret, ep_cost = 0, 0, 0
-        terminated, truncated = torch.tensor([False]), torch.tensor([False])
-        frames: list[np.ndarray] = []
-        obs_pred: list[float] = []
-        obs_true: list[float] = []
-        reward_pred: list[float] = []
-        reward_true: list[float] = []
-        num_episode = 0
-        while True:
-            if terminated or truncated:
-                print(f'Eval Episode Return: {ep_ret} \t Cost: {ep_cost}')
-                save_replay_path = os.path.join(self._logger.log_dir, 'video-pic')
-                self._logger.store(
-                    **{
-                        'EvalMetrics/EpRet': ep_ret,
-                        'EvalMetrics/EpCost': ep_cost,
-                        'EvalMetrics/EpLen': ep_len,
-                    },
-                )
+        assert (
+            self._env is not None
+        ), 'The environment must be provided or created before rendering.'
+        assert (
+            self._actor is not None or self._planner is not None
+        ), 'The policy or planner must be provided or created before rendering.'
+        if save_replay_path is None:
+            save_replay_path = os.path.join(self._save_dir, 'video', self._model_name.split('.')[0])
+        result_path = os.path.join(save_replay_path, 'result.txt')
+        print(self._dividing_line)
+        print(f'Saving the replay video to {save_replay_path},\n and the result to {result_path}.')
+        print(self._dividing_line)
+
+        horizon = 1000
+        frames = []
+        obs, _ = self._env.reset()
+        if self._render_mode == 'human':
+            self._env.render()
+        elif self._render_mode == 'rgb_array':
+            frames.append(self._env.render())
+
+        episode_rewards: list[float] = []
+        episode_costs: list[float] = []
+        episode_lengths: list[float] = []
+
+        for episode_idx in range(num_episodes):
+            self._safety_obs = torch.ones(1)
+            step = 0
+            done = False
+            ep_ret, ep_cost, length = 0.0, 0.0, 0.0
+            while (
+                not done and step <= max_render_steps
+            ):  # a big number to make sure the episode will end
+                if 'Saute' in self._cfgs['algo'] or 'Simmer' in self._cfgs['algo']:
+                    obs = torch.cat([obs, self._safety_obs], dim=-1)
+                with torch.no_grad():
+                    if self._actor is not None:
+                        act = self._actor.predict(
+                            obs,
+                            deterministic=True,
+                        )
+                    elif self._planner is not None:
+                        act = self._planner.output_action(
+                            obs.unsqueeze(0).to('cpu'),
+                        )[
+                            0
+                        ].squeeze(0)
+                    else:
+                        raise ValueError(
+                            'The policy must be provided or created before evaluating the agent.',
+                        )
+                obs, rew, cost, terminated, truncated, _ = self._env.step(act)
+                if 'Saute' in self._cfgs['algo'] or 'Simmer' in self._cfgs['algo']:
+                    self._safety_obs -= cost.unsqueeze(-1) / self._safety_budget
+                    self._safety_obs /= self._cfgs.algo_cfgs.saute_gamma
+                step += 1
+                done = bool(terminated or truncated)
+                ep_ret += rew.item()
+                ep_cost += (cost_criteria**length) * cost.item()
+                if (
+                    'EarlyTerminated' in self._cfgs['algo']
+                    and ep_cost >= self._cfgs.algo_cfgs.cost_limit
+                ):
+                    terminated = torch.as_tensor(True)
+                length += 1
+
+                if self._render_mode == 'rgb_array':
+                    frames.append(self._env.render())
+
+            if self._render_mode == 'rgb_array_list':
+                frames = self._env.render()
+            if save_replay_path is not None:
                 save_video(
                     frames,
                     save_replay_path,
-                    fps=30,
+                    fps=self.fps,
                     episode_trigger=lambda x: True,
-                    episode_index=current_step + num_episode,
+                    video_length=horizon,
+                    episode_index=episode_idx,
                     name_prefix='eval',
                 )
-                self.draw_picture(
-                    timestep=current_step,
-                    num_episode=self._cfgs.evaluation_cfgs.num_episode,
-                    pred_state=obs_pred,
-                    true_state=obs_true,
-                    save_replay_path=save_replay_path,
-                    name='obs_mean',
-                )
-                self.draw_picture(
-                    timestep=current_step,
-                    num_episode=self._cfgs.evaluation_cfgs.num_episode,
-                    pred_state=reward_pred,
-                    true_state=reward_true,
-                    save_replay_path=save_replay_path,
-                    name='reward',
-                )
-                frames = []
-                obs_pred, obs_true = [], []
-
-                reward_pred, reward_true = [], []
-
-                ep_len, ep_ret, ep_cost = 0, 0, 0
-                obs, _ = self._eval_env.reset()
-                num_episode += 1
-                if num_episode == self._cfgs.evaluation_cfgs.num_episode:
-                    break
-            action, _ = self._select_action(current_step, obs, self._eval_env)
-
-            idx = np.random.choice(self._dynamics.elite_model_idxes, size=1)[0]
-            traj = self._dynamics.imagine(
-                states=obs_dynamics,
-                horizon=1,
-                idx=idx,
-                actions=action.unsqueeze(0),
-            )
-
-            pred_next_obs_mean = traj['states'][0][0].mean()
-            pred_reward = traj['rewards'][0][0]
-
-            obs, reward, cost, terminated, truncated, info = self._eval_env.step(action)
-
-            obs_dynamics = obs if use_real_input else traj['states'][0][0]
-
-            true_next_obs_mean = obs.mean()
-
-            obs_pred.append(pred_next_obs_mean.item())
-            obs_true.append(true_next_obs_mean.item())
-
-            reward_pred.append(pred_reward.item())
-            reward_true.append(reward.item())
-
-            ep_ret += reward.cpu().numpy().item()
-            ep_cost += cost.cpu().numpy().item()
-            ep_len += info['num_step']
-            frames.append(self._eval_env.render())
-
-    def draw_picture(
-        self,
-        timestep: int,
-        num_episode: int,
-        pred_state: list,
-        true_state: list,
-        save_replay_path: str = './',
-        name: str = 'reward',
-    ) -> None:
-        """Draw a curve of the predicted value and the ground true value.
-
-        Args:
-            timestep (int): current step.
-            num_episode (int): number of episodes.
-            pred_state (list): predicted state.
-            true_state (list): true state.
-            save_replay_path (str): save replay path.
-            name (str): name of the curve.
-        """
-        target1 = list(pred_state)
-        target2 = list(true_state)
-        input1 = np.arange(0, np.array(pred_state).shape[0], 1)
-        input2 = np.arange(0, np.array(pred_state).shape[0], 1)
-
-        pylab.plot(input1, target1, 'r-', label='pred')
-        pylab.plot(input2, target2, 'b-', label='true')
-        pylab.xlabel('Step')
-        pylab.ylabel(name)
-        pylab.xticks(np.arange(0, np.array(pred_state).shape[0], 50))  # set the axis numbers
-        if name == 'reward':
-            pylab.yticks(np.arange(0, 3, 0.2))
-        else:
-            pylab.yticks(np.arange(0, 1, 0.2))
-        pylab.legend(
-            loc=3,
-            borderaxespad=2.0,
-            bbox_to_anchor=(0.7, 0.7),
-        )  # set the position of that box for what each line is
-        pylab.grid()  # draw grid
-        pylab.savefig(
-            os.path.join(
-                save_replay_path,
-                str(name) + str(timestep) + '_' + str(num_episode) + '.png',
-            ),
-            dpi=200,
-        )  # save as picture
-        pylab.close()
+            self._env.reset()
+            frames = []
+            episode_rewards.append(ep_ret)
+            episode_costs.append(ep_cost)
+            episode_lengths.append(length)
+            with open(result_path, 'a+', encoding='utf-8') as f:
+                print(f'Episode {episode_idx+1} results:', file=f)
+                print(f'Episode reward: {ep_ret}', file=f)
+                print(f'Episode cost: {ep_cost}', file=f)
+                print(f'Episode length: {length}', file=f)
+        with open(result_path, 'a+', encoding='utf-8') as f:
+            print(self._dividing_line)
+            print('Evaluation results:', file=f)
+            print(f'Average episode reward: {np.mean(episode_rewards)}', file=f)
+            print(f'Average episode cost: {np.mean(episode_costs)}', file=f)
+            print(f'Average episode length: {np.mean(episode_lengths)}', file=f)
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/model_based/cap_pets.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/model_based/cce_pets.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,114 +8,105 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Implementation of the Conservative and Adaptive Penalty algorithm."""
-from __future__ import annotations
+"""Implementation of the Constrained Cross-Entropy algorithm."""
+
 
-from typing import Any
+from __future__ import annotations
 
-import numpy as np
 from gymnasium.spaces import Box
 
 from omnisafe.algorithms import registry
 from omnisafe.algorithms.model_based.base import PETS
 from omnisafe.algorithms.model_based.base.ensemble import EnsembleDynamicsModel
-from omnisafe.algorithms.model_based.planner.cap import CAPPlanner
-from omnisafe.common.lagrange import Lagrange
+from omnisafe.algorithms.model_based.planner.cce import CCEPlanner
+from omnisafe.typing import OmnisafeSpace
 
 
 @registry.register
 # pylint: disable-next=too-many-instance-attributes, too-few-public-methods
-class CAPPETS(PETS):
-    """The Conservative and Adaptive Penalty (CAP) algorithm implementation based on PETS.
+class CCEPETS(PETS):
+    """The Constrained Cross-Entropy (CCE) algorithm implementation based on PETS.
 
     References:
-        - Title: Conservative and Adaptive Penalty for Model-Based Safe Reinforcement Learning
-        - Authors: Yecheng Jason Ma, Andrew Shen, Osbert Bastani, Dinesh Jayaraman.
-        - URL: `CAP <https://arxiv.org/abs/2112.07701>`_
+        - Title: Constrained Cross-Entropy Method for Safe Reinforcement Learning
+        - Authors: Timothy P. Lillicrap, Jonathan J. Hunt, Alexander Pritzel, Nicolas Heess,
+            Tom Erez, Yuval Tassa, David Silver, Daan Wierstra.
+        - URL: `CCE <https://proceedings.neurips.cc/paper/2018/hash/34ffeb359a192eb8174b6854643cc046-Abstract.html>`_
     """
 
     def _init_model(self) -> None:
-        """Initialize the dynamics model and the planner."""
-        self._dynamics_state_space = (
+        """Initialize the dynamics model and the planner.
+
+        CCEPETS uses following models:
+
+        - dynamics model: to predict the next state and the cost.
+        - planner: to generate the action.
+        """
+        self._dynamics_state_space: OmnisafeSpace = (
             self._env.coordinate_observation_space
             if self._env.coordinate_observation_space is not None
             else self._env.observation_space
         )
+        assert self._dynamics_state_space is not None and isinstance(
+            self._dynamics_state_space.shape,
+            tuple,
+        )
         assert self._env.action_space is not None and isinstance(
             self._env.action_space.shape,
             tuple,
         )
         if isinstance(self._env.action_space, Box):
             self._action_space = self._env.action_space
         else:
             raise NotImplementedError
-
-        self._dynamics = EnsembleDynamicsModel(
+        self._dynamics: EnsembleDynamicsModel = EnsembleDynamicsModel(
             model_cfgs=self._cfgs.dynamics_cfgs,
             device=self._device,
             state_shape=self._dynamics_state_space.shape,
             action_shape=self._action_space.shape,
             actor_critic=None,
             rew_func=None,
             cost_func=self._env.get_cost_from_obs_tensor,
             terminal_func=None,
         )
 
-        self._lagrange = Lagrange(**self._cfgs.lagrange_cfgs)
-
-        self._planner = CAPPlanner(
+        self._planner: CCEPlanner = CCEPlanner(
             dynamics=self._dynamics,
             planner_cfgs=self._cfgs.planner_cfgs,
             gamma=float(self._cfgs.algo_cfgs.gamma),
             cost_gamma=float(self._cfgs.algo_cfgs.cost_gamma),
             dynamics_state_shape=self._dynamics_state_space.shape,
             action_shape=self._action_space.shape,
             action_max=1.0,
             action_min=-1.0,
             device=self._device,
-            cost_limit=self._cfgs.lagrange_cfgs.cost_limit,
-            lagrange=self._lagrange.lagrangian_multiplier,
+            cost_limit=self._cfgs.algo_cfgs.cost_limit,
         )
 
-        self._use_actor_critic = False
-        self._update_dynamics_cycle = int(self._cfgs.algo_cfgs.update_dynamics_cycle)
+        self._use_actor_critic: bool = False
+        self._update_dynamics_cycle: int = int(self._cfgs.algo_cfgs.update_dynamics_cycle)
 
     def _init_log(self) -> None:
-        """Initialize the logger."""
+        """Initialize the logger keys for the CCE algorithm.
+
+        +----------------------------+-------------------------------+
+        | Things to log              | Description                   |
+        +============================+===============================+
+        | Plan/feasible_num          | The number of feasible plans. |
+        +----------------------------+-------------------------------+
+        | Plan/episode_costs_max     | The maximum planning cost.    |
+        +----------------------------+-------------------------------+
+        | Plan/episode_costs_mean    | The mean planning cost.       |
+        +----------------------------+-------------------------------+
+        | Plan/episode_costs_min     | The minimum planning cost.    |
+        +----------------------------+-------------------------------+
+        """
         super()._init_log()
         self._logger.register_key('Plan/feasible_num')
         self._logger.register_key('Plan/episode_costs_max')
         self._logger.register_key('Plan/episode_costs_mean')
         self._logger.register_key('Plan/episode_costs_min')
-        self._logger.register_key('Metrics/LagrangeMultiplier')
-        self._logger.register_key('Plan/var_penalty_max')
-        self._logger.register_key('Plan/var_penalty_mean')
-        self._logger.register_key('Plan/var_penalty_min')
-
-    def _save_model(self) -> None:
-        """Save the model."""
-        what_to_save: dict[str, Any] = {}
-        # set up model saving
-        what_to_save = {
-            'dynamics': self._dynamics.ensemble_model,
-            'lagrangian_multiplier': self._lagrange.lagrangian_multiplier,
-        }
-        if self._cfgs.algo_cfgs.obs_normalize:
-            obs_normalizer = self._env.save()['obs_normalizer']
-            what_to_save['obs_normalizer'] = obs_normalizer
-        self._logger.setup_torch_saver(what_to_save)
-        # self._logger.planner_save()
-        self._logger.torch_save()
-
-    def _update_epoch(self) -> None:
-        # note that logger already uses MPI statistics across all processes..
-        Jc = self._logger.get_stats('Metrics/EpCost')[0]
-        assert not np.isnan(Jc), 'cost for updating lagrange multiplier is nan'
-        # first update Lagrange multiplier parameter
-        self._lagrange.update_lagrange_multiplier(Jc)
-        # then update the policy and value function
-        self._logger.store(**{'Metrics/LagrangeMultiplier': self._lagrange.lagrangian_multiplier})
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/model_based/cce_pets.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/model_based/rce_pets.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,79 +8,106 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Implementation of the Constrained Cross-Entropy algorithm."""
+"""Implementation of the Robust Cross Entropy algorithm."""
+
+
 from __future__ import annotations
 
 from gymnasium.spaces import Box
 
 from omnisafe.algorithms import registry
 from omnisafe.algorithms.model_based.base import PETS
 from omnisafe.algorithms.model_based.base.ensemble import EnsembleDynamicsModel
-from omnisafe.algorithms.model_based.planner.cce import CCEPlanner
+from omnisafe.algorithms.model_based.planner.rce import RCEPlanner
 
 
 @registry.register
 # pylint: disable-next=too-many-instance-attributes, too-few-public-methods
-class CCEPETS(PETS):
-    """The Constrained Cross-Entropy (CCE) algorithm implementation based on PETS.
+class RCEPETS(PETS):
+    """The Robust Cross Entropy (RCE) algorithm implementation based on PETS.
 
     References:
-        - Title: Constrained Cross-Entropy Method for Safe Reinforcement Learning
-        - Authors: Timothy P. Lillicrap, Jonathan J. Hunt, Alexander Pritzel, Nicolas Heess,
-        Tom Erez, Yuval Tassa, David Silver, Daan Wierstra.
-        - URL: `CCE <https://proceedings.neurips.cc/paper/2018/hash/34ffeb359a192eb8174b6854643cc046-Abstract.html>`_
+        - Title: Constrained Model-based Reinforcement Learning with Robust Cross-Entropy Method
+        - Authors: Zuxin Liu, Hongyi Zhou, Baiming Chen, Sicheng Zhong, Martial Hebert, Ding Zhao.
+        - URL: `RCE <https://arxiv.org/abs/2010.07968>`_
     """
 
     def _init_model(self) -> None:
-        """Initialize the dynamics model and the planner."""
+        """Initialize the dynamics model and the planner.
+
+        RCEPETS uses following models:
+
+        - dynamics model: to predict the next state and the cost.
+        - planner: to generate the action.
+        """
         self._dynamics_state_space = (
             self._env.coordinate_observation_space
             if self._env.coordinate_observation_space is not None
             else self._env.observation_space
         )
+        assert self._dynamics_state_space is not None and isinstance(
+            self._dynamics_state_space.shape,
+            tuple,
+        )
         assert self._env.action_space is not None and isinstance(
             self._env.action_space.shape,
             tuple,
         )
         if isinstance(self._env.action_space, Box):
             self._action_space = self._env.action_space
         else:
             raise NotImplementedError
-        self._dynamics = EnsembleDynamicsModel(
+        self._dynamics: EnsembleDynamicsModel = EnsembleDynamicsModel(
             model_cfgs=self._cfgs.dynamics_cfgs,
             device=self._device,
             state_shape=self._dynamics_state_space.shape,
             action_shape=self._action_space.shape,
             actor_critic=None,
             rew_func=None,
             cost_func=self._env.get_cost_from_obs_tensor,
             terminal_func=None,
         )
 
-        self._planner = CCEPlanner(
+        self._planner: RCEPlanner = RCEPlanner(
             dynamics=self._dynamics,
             planner_cfgs=self._cfgs.planner_cfgs,
             gamma=float(self._cfgs.algo_cfgs.gamma),
             cost_gamma=float(self._cfgs.algo_cfgs.cost_gamma),
             dynamics_state_shape=self._dynamics_state_space.shape,
             action_shape=self._action_space.shape,
             action_max=1.0,
             action_min=-1.0,
             device=self._device,
             cost_limit=self._cfgs.algo_cfgs.cost_limit,
         )
 
-        self._use_actor_critic = False
-        self._update_dynamics_cycle = int(self._cfgs.algo_cfgs.update_dynamics_cycle)
+        self._use_actor_critic: bool = False
+        self._update_dynamics_cycle: int = int(self._cfgs.algo_cfgs.update_dynamics_cycle)
 
     def _init_log(self) -> None:
-        """Initialize the logger keys for the CCE algorithm."""
+        """Initialize the logger.
+
+        +----------------------------+-------------------------------+
+        | Things to log              | Description                   |
+        +============================+===============================+
+        | Plan/feasible_num          | The number of feasible plans. |
+        +----------------------------+-------------------------------+
+        | Plan/episode_costs_max     | The maximum planning cost.    |
+        +----------------------------+-------------------------------+
+        | Plan/episode_costs_mean    | The mean planning cost.       |
+        +----------------------------+-------------------------------+
+        | Plan/episode_costs_min     | The minimum planning cost.    |
+        +----------------------------+-------------------------------+
+        | Metrics/LagrangeMultiplier | The lagrange multiplier.      |
+        +----------------------------+-------------------------------+
+        """
         super()._init_log()
         self._logger.register_key('Plan/feasible_num')
         self._logger.register_key('Plan/episode_costs_max')
         self._logger.register_key('Plan/episode_costs_mean')
         self._logger.register_key('Plan/episode_costs_min')
+        self._logger.register_key('Metrics/LagrangeMultiplier')
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/model_based/planner/__init__.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/model_based/planner/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/model_based/planner/arc.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/model_based/planner/cem.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,34 +8,35 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Model Predictive Control Planner of the Actor Regularized Control (ARC) algorithm."""
+"""Model Predictive Control Planner of Cross-Entropy Method optimization algorithm."""
+
+
 from __future__ import annotations
 
 from typing import Any
 
 import torch
 
 from omnisafe.algorithms.model_based.base.ensemble import EnsembleDynamicsModel
-from omnisafe.algorithms.model_based.planner.cem import CEMPlanner
-from omnisafe.models.actor_critic.constraint_actor_q_critic import ConstraintActorQCritic
 from omnisafe.utils.config import Config
 
 
-class ARCPlanner(CEMPlanner):  # pylint: disable=too-many-instance-attributes
-    """The planner of Actor Regularized Control (ARC) algorithm.
+class CEMPlanner:  # pylint: disable=too-many-instance-attributes
+    """The planner of  Cross-Entropy Method optimization (CEM) algorithm.
 
     References:
-        - Title: Learning Off-Policy with Online Planning
-        - Authors: Harshit Sikchi, Wenxuan Zhou, David Held.
-        - URL: `ARC <https://arxiv.org/abs/2008.10066>`_
+        - Title: Sample-efficient Cross-Entropy Method for Real-time Planning
+        - Authors: Cristina Pinneri, Shambhuraj Sawant, Sebastian Blaes, Jan Achterhold,
+            Joerg Stueckler, Michal Rolinek, Georg Martius
+        - URL: `CEM <https://arxiv.org/pdf/2008.06389.pdf>`_
     """
 
     def __init__(  # pylint: disable=too-many-locals, too-many-arguments
         self,
         dynamics: EnsembleDynamicsModel,
         planner_cfgs: Config,
         gamma: float,
@@ -43,46 +44,60 @@
         dynamics_state_shape: tuple[int, ...],
         action_shape: tuple[int, ...],
         action_max: float,
         action_min: float,
         device: torch.device,
         **kwargs: Any,
     ) -> None:
-        """Initialize the planner of Actor Regularized Control (ARC) algorithm."""
-        super().__init__(
-            dynamics,
-            planner_cfgs,
-            gamma,
-            cost_gamma,
-            dynamics_state_shape,
-            action_shape,
-            action_max,
-            action_min,
-            device,
-            **kwargs,
-        )
-        self._actor_critic: ConstraintActorQCritic = kwargs['actor_critic']
-        self._mixture_coefficient: float = planner_cfgs.mixture_coefficient
-        self._temperature: float = planner_cfgs.temperature
-        self._actor_traj = int(self._mixture_coefficient * self._num_samples)
-        self._num_action = self._actor_traj + self._num_samples
+        """Initializes the planner of Cross-Entropy Method optimization (CEM) algorithm."""
+        assert (
+            planner_cfgs.num_samples * planner_cfgs.num_particles
+        ) % dynamics.num_models == 0, 'num_samples * num_elites should be divisible by num_models'
         assert (
-            self._num_samples + self._mixture_coefficient * self._num_samples
-        ) > self._num_elites, 'The number of samples should be larger than the number of elites.'
+            planner_cfgs.num_samples > planner_cfgs.num_elites
+        ), 'num_samples should be greater than num_elites'
+        self._dynamics = dynamics
+        self._num_models = dynamics.num_models
+        self._horizon = planner_cfgs.plan_horizon
+        self._num_iterations = planner_cfgs.num_iterations
+        self._num_particles = planner_cfgs.num_particles
+        self._num_samples = planner_cfgs.num_samples
+        self._num_elites = planner_cfgs.num_elites
+        self._momentum = planner_cfgs.momentum
+        self._epsilon = planner_cfgs.epsilon
+        self._dynamics_state_shape = dynamics_state_shape
+        self._action_shape = action_shape
+        self._action_max = action_max
+        self._action_min = action_min
+        self._gamma = gamma
+        self._cost_gamma = cost_gamma
+        self._device = device
+        self._action_sequence_mean = torch.zeros(
+            self._horizon,
+            *self._action_shape,
+            device=self._device,
+        )
+        self._init_var = planner_cfgs.init_var
+        self._action_sequence_var = self._init_var * torch.ones(
+            self._horizon,
+            *self._action_shape,
+            device=self._device,
+        )
+        self.kwargs = kwargs
 
     @torch.no_grad()
     def _act_from_last_gaus(self, last_mean: torch.Tensor, last_var: torch.Tensor) -> torch.Tensor:
         """Sample actions from the last gaussian distribution.
 
         Args:
             last_mean (torch.Tensor): Last mean of the gaussian distribution.
             last_var (torch.Tensor): Last variance of the gaussian distribution.
 
         Returns:
-            Sample actions (torch.Tensor): Sampled actions from the last gaussian distribution.
+            sampled actions: Sampled actions from the last gaussian distribution.
         """
         constrained_std = torch.sqrt(last_var)
         actions = torch.clamp(
             last_mean.unsqueeze(1)
             + constrained_std.unsqueeze(1)
             * torch.randn(
                 self._horizon,
@@ -93,232 +108,164 @@
             self._action_min,
             self._action_max,
         )
         actions.clamp_(min=self._action_min, max=self._action_max)  # clip action range
         return actions
 
     @torch.no_grad()
-    def _act_from_actor(self, state: torch.Tensor) -> torch.Tensor:
-        """Sample actions from the actor.
-
-        Args:
-            state (torch.Tensor): Current state.
-
-        Returns:
-            Sample actions (torch.Tensor): Sampled actions from the actor.
-        """
-        assert state.shape == torch.Size(
-            [1, *self._dynamics_state_shape],
-        ), 'state dimension one should be 1'
-        assert (
-            self._actor_traj % self._num_models == 0
-        ), 'actor_traj should be divisible by num_models'
-        traj = self._dynamics.imagine(
-            states=state,
-            horizon=self._horizon,
-            actions=None,
-            actor_critic=self._actor_critic,
-            idx=0,
-        )
-        return (
-            traj['actions']
-            .reshape(self._horizon, 1, *self._action_shape)
-            .clone()
-            .repeat([1, self._actor_traj, 1])
-        )
-
-    @torch.no_grad()
     def _state_action_repeat(
         self,
         state: torch.Tensor,
         action: torch.Tensor,
     ) -> tuple[torch.Tensor, torch.Tensor]:
         """Repeat the state for num_repeat * action.shape[0] times and action for num_repeat times.
 
         Args:
-            state (torch.Tensor): Current state.
-            action (torch.Tensor): Sampled actions.
+            state (torch.Tensor): The current state.
+            action (torch.Tensor): The sampled actions.
 
         Returns:
-            states (torch.Tensor): Repeated states.
-            actions (torch.Tensor): Repeated actions.
+            states: The repeated states.
+            actions: The repeated actions.
         """
+        assert (
+            self._num_particles % self._num_models == 0
+        ), 'num_particles should be divisible by num_models'
         assert action.shape == torch.Size(
-            [self._horizon, self._num_action, *self._action_shape],
+            [self._horizon, self._num_samples, *self._action_shape],
         ), 'Input action dimension should be equal to (self._num_samples, self._action_shape)'
         assert state.shape == torch.Size(
             [1, *self._dynamics_state_shape],
         ), 'state dimension one should be 1'
-        states = state.repeat(int(self._num_particles * self._num_action), 1)
-        actions = action.unsqueeze(1).repeat(1, int(self._num_particles), 1, 1)
+        states = state.repeat(int(self._num_particles / self._num_models * self._num_samples), 1)
+        actions = action.unsqueeze(1).repeat(1, int(self._num_particles / self._num_models), 1, 1)
         actions = actions.reshape(
             self._horizon,
-            int(self._num_particles * self._num_action),
+            int(self._num_particles / self._num_models * self._num_samples),
             *self._action_shape,
         )
         return states, actions
 
     @torch.no_grad()
     def _select_elites(
         self,
         actions: torch.Tensor,
-        traj: dict,
-    ) -> tuple[torch.Tensor, torch.Tensor, dict]:
+        traj: dict[str, torch.Tensor],
+    ) -> tuple[torch.Tensor, torch.Tensor, dict[str, float]]:
         """Select elites from the sampled actions.
 
         Args:
             actions (torch.Tensor): Sampled actions.
-            traj (dict): Trajectory dictionary.
+            traj (dict[str, torch.Tensor]): Trajectory dictionary.
 
         Returns:
-            elites_value (torch.Tensor): Value of the elites.
-            elites_action (torch.Tensor): Action of the elites.
-            info (dict): Dictionary containing the information of elites value and action.
+            elites_value: The value of the elites.
+            elites_action: The action of the elites.
+            info: The dictionary containing the information of elites value and action.
         """
         rewards = traj['rewards']
-        values = traj['values']
         assert actions.shape == torch.Size(
-            [self._horizon, self._num_action, *self._action_shape],
-            # pylint: disable-next=line-too-long
+            [self._horizon, self._num_samples, *self._action_shape],
         ), 'Input action dimension should be equal to (self._horizon, self._num_samples, self._action_shape)'
         assert rewards.shape == torch.Size(
-            [self._horizon, self._num_models, int(self._num_particles * self._num_action), 1],
-            # pylint: disable-next=line-too-long
-        ), 'Input rewards dimension should be equal to (self._horizon, self._num_models, self._num_particles*self._num_samples, 1)'
-        assert values.shape == torch.Size(
-            [self._horizon, self._num_models, int(self._num_particles * self._num_action), 1],
+            [
+                self._horizon,
+                self._num_models,
+                int(self._num_particles / self._num_models * self._num_samples),
+                1,
+            ],
             # pylint: disable-next=line-too-long
-        ), 'Input values dimension should be equal to (self._horizon, self._num_models, self._num_particles*self._num_samples, 1)'
-
-        rewards = rewards.reshape(
-            self._horizon,
-            self._num_models * self._num_particles,
-            self._num_action,
-            1,
-        )
-        values = values.reshape(
-            self._horizon,
-            self._num_models * self._num_particles,
-            self._num_action,
-            1,
-        )
-        sum_horizon_returns = torch.sum(rewards, dim=0) + values[-1, :, :, :]
+        ), 'Input rewards dimension should be equal to (self._horizon, self._num_models, self._num_particles/self._num_models*self._num_samples, 1)'
+        returns = rewards.reshape(self._horizon, self._num_particles, self._num_samples, 1)
+        sum_horizon_returns = torch.sum(returns, dim=0)
         mean_particles_returns = sum_horizon_returns.mean(dim=0)
         mean_episode_returns = mean_particles_returns * (1000 / self._horizon)
+        assert mean_episode_returns.shape == torch.Size(
+            [self._num_samples, 1],
+        ), 'Input returns dimension should be equal to (self._num_samples, 1)'
+        elite_idxs = torch.topk(mean_episode_returns.squeeze(1), self._num_elites, dim=0).indices
+        elite_values, elite_actions = mean_episode_returns[elite_idxs], actions[:, elite_idxs]
 
-        assert mean_episode_returns.shape[0] == self._num_action
-
-        elite_actions = actions
-        elite_values = mean_episode_returns
         info = {
             'Plan/episode_returns_max': mean_episode_returns.max().item(),
             'Plan/episode_returns_mean': mean_episode_returns.mean().item(),
             'Plan/episode_returns_min': mean_episode_returns.min().item(),
         }
 
         return elite_values, elite_actions, info
 
     @torch.no_grad()
-    def _update_mean_var(
+    def _update_mean_var(  # pylint: disable=unused-argument
         self,
         elite_actions: torch.Tensor,
         elite_values: torch.Tensor,
-        info: dict,
-    ) -> tuple[torch.Tensor, torch.Tensor]:  # pylint: disable-next=unused-argument
+        info: dict[str, int | float],
+    ) -> tuple[torch.Tensor, torch.Tensor]:
         """Update the mean and variance of the elite actions.
 
         Args:
-            elite_actions (torch.Tensor): Elite actions.
-            elite_values (torch.Tensor): Elite values.
-            kwargs (dict): Keyword arguments.
+            elite_actions (torch.Tensor): The elite actions.
+            elite_values (torch.Tensor): The elite values.
+            info (dict[str, int | float]): The dictionary containing the information of the elite values and actions.
 
         Returns:
-            new_mean (torch.Tensor): New mean of the elite actions.
-            new_var (torch.Tensor): New variance of the elite actions.
+            new_mean: The new mean of the elite actions.
+            new_var: The new variance of the elite actions.
         """
-        assert (
-            elite_actions.shape[0] == self._horizon
-            and elite_actions.shape[-1] == self._action_shape[0]
+        assert elite_actions.shape == torch.Size(
+            [self._horizon, self._num_elites, *self._action_shape],
         ), 'Input elite_actions dimension should be equal to (self._horizon, self._num_elites, self._action_shape)'
-        assert (
-            elite_values.shape[-1] == 1
+        assert elite_values.shape == torch.Size(
+            [self._num_elites, 1],
         ), 'Input elite_values dimension should be equal to (self._num_elites, 1)'
-        assert (
-            elite_actions.shape[1] == elite_values.shape[0]
-        ), 'Number of action should be the same'
 
-        max_value = elite_values.max(0)[0]
-        score = torch.exp(self._temperature * (elite_values - max_value))
-        score /= score.sum(0)
-        new_mean = torch.sum(score.unsqueeze(0) * elite_actions, dim=1) / (score.sum(0) + 1e-9)
-        new_var = torch.sum(
-            score.unsqueeze(0) * (elite_actions - new_mean.unsqueeze(1)) ** 2,
-            dim=1,
-        ) / (score.sum(0) + 1e-9)
-        new_var = new_var.clamp_(0, 2)
+        new_mean = elite_actions.mean(dim=1)
+        new_var = elite_actions.var(dim=1)
 
         return new_mean, new_var
 
     @torch.no_grad()
     def output_action(self, state: torch.Tensor) -> tuple[torch.Tensor, dict]:
         """Output the action given the state.
 
         Args:
             state (torch.Tensor): State of the environment.
 
         Returns:
-            action (torch.Tensor): Action of the environment.
-            logger_info (dict): Dictionary containing the information of the action.
+            action: The action of the agent.
+            info: The dictionary containing the information of the action.
         """
         assert state.shape == torch.Size(
             [1, *self._dynamics_state_shape],
         ), 'Input state dimension should be equal to (1, self._dynamics_state_shape)'
         last_mean = torch.zeros_like(self._action_sequence_mean)
         last_var = self._action_sequence_var.clone()
         last_mean[:-1] = self._action_sequence_mean[1:].clone()
         last_mean[-1] = self._action_sequence_mean[-1].clone()
 
         current_iter = 0
-        actions_actor = self._act_from_actor(state)
-        while current_iter < self._num_iterations and last_var.max() > self._epsilon:
-            actions_gauss = self._act_from_last_gaus(last_mean=last_mean, last_var=last_var)
-            actions = torch.cat([actions_gauss, actions_actor], dim=1)
+        info: dict[str, float | int] = {}
+        while current_iter < self._num_iterations:
+            actions = self._act_from_last_gaus(last_mean=last_mean, last_var=last_var)
             # [horizon, num_sample, action_shape]
             states_repeat, actions_repeat = self._state_action_repeat(state, actions)
             # pylint: disable-next=line-too-long
             # [num_particles * num_samples/num_ensemble, state_shape], [horizon, num_particles * num_samples/num_ensemble, action_shape]
             traj = self._dynamics.imagine(states_repeat, self._horizon, actions_repeat)
             # pylint: disable-next=line-too-long
             # {states, rewards, values}, each value shape is [horizon, num_ensemble, num_particles * num_samples/num_ensemble, 1]
 
             elite_values, elite_actions, info = self._select_elites(actions, traj)
             # [num_sample, 1]
-            new_mean, new_var = self._update_mean_var(
-                elite_actions,
-                elite_values,
-                info,
-            )
+            new_mean, new_var = self._update_mean_var(elite_actions, elite_values, info)
             last_mean = self._momentum * last_mean + (1 - self._momentum) * new_mean
             last_var = self._momentum * last_var + (1 - self._momentum) * new_var
             current_iter += 1
         logger_info = {
             'Plan/iter': current_iter,
             'Plan/last_var_mean': last_var.mean().item(),
             'Plan/last_var_max': last_var.max().item(),
             'Plan/last_var_min': last_var.min().item(),
         }
         logger_info.update(info)
         self._action_sequence_mean = last_mean.clone()
         return last_mean[0].clone().unsqueeze(0), logger_info
-
-    def reset_planner(self) -> None:
-        """Reset the planner."""
-        self._action_sequence_mean = torch.zeros(
-            self._horizon,
-            *self._action_shape,
-            device=self._device,
-        )
-        self._action_sequence_var = self._init_var * torch.ones(
-            self._horizon,
-            *self._action_shape,
-            device=self._device,
-        )
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/model_based/planner/cap.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/model_based/planner/cap.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Model Predictive Control Planner of the Conservative and Adaptive Penalty algorithm."""
+
+
 from __future__ import annotations
 
 from typing import Any
 
 import torch
 
 from omnisafe.algorithms.model_based.base.ensemble import EnsembleDynamicsModel
@@ -61,26 +63,26 @@
         )
         self._lagrange: torch.Tensor = kwargs['lagrange']
 
     @torch.no_grad()
     def _select_elites(  # pylint: disable=too-many-locals
         self,
         actions: torch.Tensor,
-        traj: dict,
-    ) -> tuple[torch.Tensor, torch.Tensor, dict]:
+        traj: dict[str, torch.Tensor],
+    ) -> tuple[torch.Tensor, torch.Tensor, dict[str, float]]:
         """Select elites from the sampled actions.
 
         Args:
             actions (torch.Tensor): Sampled actions.
-            traj (dict): Trajectory dictionary.
+            traj (dict[str, torch.Tensor]): Trajectory dictionary.
 
         Returns:
-            elites_value (torch.Tensor): Value of the elites.
-            elites_action (torch.Tensor): Action of the elites.
-            info (dict): Dictionary containing the information of elites value and action.
+            elites_value: The value of the elites.
+            elites_action: The action of the elites.
+            info: The dictionary containing the information of elites value and action.
         """
         rewards = traj['rewards']
         costs = traj['costs']
         state_vars = traj['vars']
         assert actions.shape == torch.Size(
             [self._horizon, self._num_samples, *self._action_shape],
             # pylint: disable-next=line-too-long
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/model_based/planner/cce.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/model_based/planner/cce.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Model Predictive Control Planner of the Constrained Cross-Entropy algorithm."""
+
+
 from __future__ import annotations
 
 from typing import Any
 
 import torch
 
 from omnisafe.algorithms.model_based.base.ensemble import EnsembleDynamicsModel
@@ -26,15 +28,15 @@
 
 class CCEPlanner(CEMPlanner):
     """The planner of Constrained Cross-Entropy (CCE) algorithm.
 
     References:
         - Title: Constrained Cross-Entropy Method for Safe Reinforcement Learning
         - Authors: Timothy P. Lillicrap, Jonathan J. Hunt, Alexander Pritzel, Nicolas Heess,
-        Tom Erez, Yuval Tassa, David Silver, Daan Wierstra.
+            Tom Erez, Yuval Tassa, David Silver, Daan Wierstra.
         - URL: `CCE <https://proceedings.neurips.cc/paper/2018/hash/34ffeb359a192eb8174b6854643cc046-Abstract.html>`_
     """
 
     def __init__(  # pylint: disable=too-many-locals, too-many-arguments
         self,
         dynamics: EnsembleDynamicsModel,
         planner_cfgs: Config,
@@ -62,26 +64,26 @@
         )
         self._cost_limit: float = kwargs['cost_limit']
 
     @torch.no_grad()
     def _select_elites(
         self,
         actions: torch.Tensor,
-        traj: dict,
-    ) -> tuple[torch.Tensor, torch.Tensor, dict]:
+        traj: dict[str, torch.Tensor],
+    ) -> tuple[torch.Tensor, torch.Tensor, dict[str, float]]:
         """Select elites from the sampled actions.
 
         Args:
             actions (torch.Tensor): Sampled actions.
-            traj (dict): Trajectory dictionary.
+            traj (dict[str, torch.Tensor]): Trajectory dictionary.
 
         Returns:
-            elites_value (torch.Tensor): Value of the elites.
-            elites_action (torch.Tensor): Action of the elites.
-            info (dict): Dictionary containing the information of elites value and action.
+            elites_value: The value of the elites.
+            elites_action: The action of the elites.
+            info: The dictionary containing the information of elites value and action.
         """
         rewards = traj['rewards']
         costs = traj['costs']
         assert actions.shape == torch.Size(  # pylint: disable=line-too-long
             [self._horizon, self._num_samples, *self._action_shape],
             # pylint: disable-next=line-too-long
         ), 'Input action dimension should be equal to (self._horizon, self._num_samples, self._action_shape)'
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/model_based/planner/cem.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/model_based/planner/arc.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,30 +8,36 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Model Predictive Control Planner of Cross-Entropy Method optimization algorithm."""
+"""Model Predictive Control Planner of the Actor Regularized Control (ARC) algorithm."""
+
+
 from __future__ import annotations
 
 from typing import Any
 
 import torch
 
 from omnisafe.algorithms.model_based.base.ensemble import EnsembleDynamicsModel
+from omnisafe.algorithms.model_based.planner.cem import CEMPlanner
+from omnisafe.models.actor_critic.constraint_actor_q_critic import ConstraintActorQCritic
 from omnisafe.utils.config import Config
 
 
-class CEMPlanner:  # pylint: disable=too-many-instance-attributes
-    """The planner of  Cross-Entropy Method optimization (CEM) algorithm.
+class ARCPlanner(CEMPlanner):  # pylint: disable=too-many-instance-attributes
+    """The planner of Actor Regularized Control (ARC) algorithm.
 
     References:
-        - URL: `A good description of CEM <https://arxiv.org/pdf/2008.06389.pdf>`_
+        - Title: Learning Off-Policy with Online Planning
+        - Authors: Harshit Sikchi, Wenxuan Zhou, David Held.
+        - URL: `ARC <https://arxiv.org/abs/2008.10066>`_
     """
 
     def __init__(  # pylint: disable=too-many-locals, too-many-arguments
         self,
         dynamics: EnsembleDynamicsModel,
         planner_cfgs: Config,
         gamma: float,
@@ -39,60 +45,46 @@
         dynamics_state_shape: tuple[int, ...],
         action_shape: tuple[int, ...],
         action_max: float,
         action_min: float,
         device: torch.device,
         **kwargs: Any,
     ) -> None:
-        """Initializes the planner of Cross-Entropy Method optimization (CEM) algorithm."""
-        assert (
-            planner_cfgs.num_samples * planner_cfgs.num_particles
-        ) % dynamics.num_models == 0, 'num_samples * num_elites should be divisible by num_models'
-        assert (
-            planner_cfgs.num_samples > planner_cfgs.num_elites
-        ), 'num_samples should be greater than num_elites'
-        self._dynamics = dynamics
-        self._num_models = dynamics.num_models
-        self._horizon = planner_cfgs.plan_horizon
-        self._num_iterations = planner_cfgs.num_iterations
-        self._num_particles = planner_cfgs.num_particles
-        self._num_samples = planner_cfgs.num_samples
-        self._num_elites = planner_cfgs.num_elites
-        self._momentum = planner_cfgs.momentum
-        self._epsilon = planner_cfgs.epsilon
-        self._dynamics_state_shape = dynamics_state_shape
-        self._action_shape = action_shape
-        self._action_max = action_max
-        self._action_min = action_min
-        self._gamma = gamma
-        self._cost_gamma = cost_gamma
-        self._device = device
-        self._action_sequence_mean = torch.zeros(
-            self._horizon,
-            *self._action_shape,
-            device=self._device,
+        """Initialize the planner of Actor Regularized Control (ARC) algorithm."""
+        super().__init__(
+            dynamics,
+            planner_cfgs,
+            gamma,
+            cost_gamma,
+            dynamics_state_shape,
+            action_shape,
+            action_max,
+            action_min,
+            device,
+            **kwargs,
         )
-        self._init_var = planner_cfgs.init_var
-        self._action_sequence_var = self._init_var * torch.ones(
-            self._horizon,
-            *self._action_shape,
-            device=self._device,
-        )
-        self.kwargs = kwargs
+        self._actor_critic: ConstraintActorQCritic = kwargs['actor_critic']
+        self._mixture_coefficient: float = planner_cfgs.mixture_coefficient
+        self._temperature: float = planner_cfgs.temperature
+        self._actor_traj: int = int(self._mixture_coefficient * self._num_samples)
+        self._num_action: int = self._actor_traj + self._num_samples
+        assert (
+            self._num_samples + self._mixture_coefficient * self._num_samples
+        ) > self._num_elites, 'The number of samples should be larger than the number of elites.'
 
     @torch.no_grad()
     def _act_from_last_gaus(self, last_mean: torch.Tensor, last_var: torch.Tensor) -> torch.Tensor:
         """Sample actions from the last gaussian distribution.
 
         Args:
             last_mean (torch.Tensor): Last mean of the gaussian distribution.
             last_var (torch.Tensor): Last variance of the gaussian distribution.
 
         Returns:
-            Sample actions (torch.Tensor): Sampled actions from the last gaussian distribution.
+            sampled actions: Sampled actions from the last gaussian distribution.
         """
         constrained_std = torch.sqrt(last_var)
         actions = torch.clamp(
             last_mean.unsqueeze(1)
             + constrained_std.unsqueeze(1)
             * torch.randn(
                 self._horizon,
@@ -103,175 +95,220 @@
             self._action_min,
             self._action_max,
         )
         actions.clamp_(min=self._action_min, max=self._action_max)  # clip action range
         return actions
 
     @torch.no_grad()
+    def _act_from_actor(self, state: torch.Tensor) -> torch.Tensor:
+        """Sample actions from the actor.
+
+        Args:
+            state (torch.Tensor): The current state.
+
+        Returns:
+            sampled actions: Sampled actions from the actor.
+        """
+        assert state.shape == torch.Size(
+            [1, *self._dynamics_state_shape],
+        ), 'state dimension one should be 1'
+        assert (
+            self._actor_traj % self._num_models == 0
+        ), 'actor_traj should be divisible by num_models'
+        traj = self._dynamics.imagine(
+            states=state,
+            horizon=self._horizon,
+            actions=None,
+            actor_critic=self._actor_critic,
+            idx=0,
+        )
+        return (
+            traj['actions']
+            .reshape(self._horizon, 1, *self._action_shape)
+            .clone()
+            .repeat([1, self._actor_traj, 1])
+        )
+
+    @torch.no_grad()
     def _state_action_repeat(
         self,
         state: torch.Tensor,
         action: torch.Tensor,
     ) -> tuple[torch.Tensor, torch.Tensor]:
         """Repeat the state for num_repeat * action.shape[0] times and action for num_repeat times.
 
         Args:
-            state (torch.Tensor): Current state.
-            action (torch.Tensor): Sampled actions.
+            state (torch.Tensor): The current state.
+            action (torch.Tensor): The sampled actions.
 
         Returns:
-            states (torch.Tensor): Repeated states.
-            actions (torch.Tensor): Repeated actions.
+            states: The repeated states.
+            actions: The repeated actions.
         """
-        assert (
-            self._num_particles % self._num_models == 0
-        ), 'num_particles should be divisible by num_models'
         assert action.shape == torch.Size(
-            [self._horizon, self._num_samples, *self._action_shape],
+            [self._horizon, self._num_action, *self._action_shape],
         ), 'Input action dimension should be equal to (self._num_samples, self._action_shape)'
         assert state.shape == torch.Size(
             [1, *self._dynamics_state_shape],
         ), 'state dimension one should be 1'
-        states = state.repeat(int(self._num_particles / self._num_models * self._num_samples), 1)
-        actions = action.unsqueeze(1).repeat(1, int(self._num_particles / self._num_models), 1, 1)
+        states = state.repeat(int(self._num_particles * self._num_action), 1)
+        actions = action.unsqueeze(1).repeat(1, int(self._num_particles), 1, 1)
         actions = actions.reshape(
             self._horizon,
-            int(self._num_particles / self._num_models * self._num_samples),
+            int(self._num_particles * self._num_action),
             *self._action_shape,
         )
         return states, actions
 
     @torch.no_grad()
     def _select_elites(
         self,
         actions: torch.Tensor,
-        traj: dict,
-    ) -> tuple[torch.Tensor, torch.Tensor, dict]:
+        traj: dict[str, torch.Tensor],
+    ) -> tuple[torch.Tensor, torch.Tensor, dict[str, float]]:
         """Select elites from the sampled actions.
 
         Args:
             actions (torch.Tensor): Sampled actions.
-            traj (dict): Trajectory dictionary.
+            traj (dict[str, torch.Tensor]): Trajectory dictionary.
 
         Returns:
-            elites_value (torch.Tensor): Value of the elites.
-            elites_action (torch.Tensor): Action of the elites.
-            info (dict): Dictionary containing the information of elites value and action.
+            elites_value: The value of the elites.
+            elites_action: The action of the elites.
+            info: The dictionary containing the information of elites value and action.
         """
         rewards = traj['rewards']
+        values = traj['values']
         assert actions.shape == torch.Size(
-            [self._horizon, self._num_samples, *self._action_shape],
+            [self._horizon, self._num_action, *self._action_shape],
+            # pylint: disable-next=line-too-long
         ), 'Input action dimension should be equal to (self._horizon, self._num_samples, self._action_shape)'
         assert rewards.shape == torch.Size(
-            [
-                self._horizon,
-                self._num_models,
-                int(self._num_particles / self._num_models * self._num_samples),
-                1,
-            ],
+            [self._horizon, self._num_models, int(self._num_particles * self._num_action), 1],
+            # pylint: disable-next=line-too-long
+        ), 'Input rewards dimension should be equal to (self._horizon, self._num_models, self._num_particles*self._num_samples, 1)'
+        assert values.shape == torch.Size(
+            [self._horizon, self._num_models, int(self._num_particles * self._num_action), 1],
             # pylint: disable-next=line-too-long
-        ), 'Input rewards dimension should be equal to (self._horizon, self._num_models, self._num_particles/self._num_models*self._num_samples, 1)'
-        returns = rewards.reshape(self._horizon, self._num_particles, self._num_samples, 1)
-        sum_horizon_returns = torch.sum(returns, dim=0)
+        ), 'Input values dimension should be equal to (self._horizon, self._num_models, self._num_particles*self._num_samples, 1)'
+
+        rewards = rewards.reshape(
+            self._horizon,
+            self._num_models * self._num_particles,
+            self._num_action,
+            1,
+        )
+        values = values.reshape(
+            self._horizon,
+            self._num_models * self._num_particles,
+            self._num_action,
+            1,
+        )
+        sum_horizon_returns = torch.sum(rewards, dim=0) + values[-1, :, :, :]
         mean_particles_returns = sum_horizon_returns.mean(dim=0)
         mean_episode_returns = mean_particles_returns * (1000 / self._horizon)
-        assert mean_episode_returns.shape == torch.Size(
-            [self._num_samples, 1],
-        ), 'Input returns dimension should be equal to (self._num_samples, 1)'
-        elite_idxs = torch.topk(mean_episode_returns.squeeze(1), self._num_elites, dim=0).indices
-        elite_values, elite_actions = mean_episode_returns[elite_idxs], actions[:, elite_idxs]
 
+        assert mean_episode_returns.shape[0] == self._num_action
+
+        elite_actions = actions
+        elite_values = mean_episode_returns
         info = {
             'Plan/episode_returns_max': mean_episode_returns.max().item(),
             'Plan/episode_returns_mean': mean_episode_returns.mean().item(),
             'Plan/episode_returns_min': mean_episode_returns.min().item(),
         }
 
         return elite_values, elite_actions, info
 
     @torch.no_grad()
-    def _update_mean_var(  # pylint: disable=unused-argument
+    def _update_mean_var(
         self,
         elite_actions: torch.Tensor,
         elite_values: torch.Tensor,
-        info: dict,
-    ) -> tuple[torch.Tensor, torch.Tensor]:
+        info: dict[str, int | float],
+    ) -> tuple[torch.Tensor, torch.Tensor]:  # pylint: disable-next=unused-argument
         """Update the mean and variance of the elite actions.
 
         Args:
-            elite_actions (torch.Tensor): Elite actions.
-            elite_values (torch.Tensor): Elite values.
+            elite_actions (torch.Tensor): The elite actions.
+            elite_values (torch.Tensor): The elite values.
+            info (dict[str, int | float]): The dictionary containing the information of the elite values and actions.
 
         Returns:
-            new_mean (torch.Tensor): New mean of the elite actions.
-            new_var (torch.Tensor): New variance of the elite actions.
+            new_mean: The new mean of the elite actions.
+            new_var: The new variance of the elite actions.
         """
-        assert elite_actions.shape == torch.Size(
-            [self._horizon, self._num_elites, *self._action_shape],
+        assert (
+            elite_actions.shape[0] == self._horizon
+            and elite_actions.shape[-1] == self._action_shape[0]
         ), 'Input elite_actions dimension should be equal to (self._horizon, self._num_elites, self._action_shape)'
-        assert elite_values.shape == torch.Size(
-            [self._num_elites, 1],
+        assert (
+            elite_values.shape[-1] == 1
         ), 'Input elite_values dimension should be equal to (self._num_elites, 1)'
+        assert (
+            elite_actions.shape[1] == elite_values.shape[0]
+        ), 'Number of action should be the same'
 
-        new_mean = elite_actions.mean(dim=1)
-        new_var = elite_actions.var(dim=1)
+        max_value = elite_values.max(0)[0]
+        score = torch.exp(self._temperature * (elite_values - max_value))
+        score /= score.sum(0)
+        new_mean = torch.sum(score.unsqueeze(0) * elite_actions, dim=1) / (score.sum(0) + 1e-9)
+        new_var = torch.sum(
+            score.unsqueeze(0) * (elite_actions - new_mean.unsqueeze(1)) ** 2,
+            dim=1,
+        ) / (score.sum(0) + 1e-9)
+        new_var = new_var.clamp_(0, 2)
 
         return new_mean, new_var
 
     @torch.no_grad()
-    def output_action(self, state: torch.Tensor) -> tuple[torch.Tensor, dict]:
+    def output_action(self, state: torch.Tensor) -> tuple[torch.Tensor, dict[str, int | float]]:
         """Output the action given the state.
 
         Args:
             state (torch.Tensor): State of the environment.
 
         Returns:
-            action (torch.Tensor): Action of the environment.
-            logger_info (dict): Dictionary containing the information of the action.
+            action: The action of the agent.
+            info: The dictionary containing the information of the action.
         """
         assert state.shape == torch.Size(
             [1, *self._dynamics_state_shape],
         ), 'Input state dimension should be equal to (1, self._dynamics_state_shape)'
         last_mean = torch.zeros_like(self._action_sequence_mean)
         last_var = self._action_sequence_var.clone()
         last_mean[:-1] = self._action_sequence_mean[1:].clone()
         last_mean[-1] = self._action_sequence_mean[-1].clone()
 
         current_iter = 0
-        while current_iter < self._num_iterations:
-            actions = self._act_from_last_gaus(last_mean=last_mean, last_var=last_var)
+        actions_actor = self._act_from_actor(state)
+        info: dict[str, float | int] = {}
+        while current_iter < self._num_iterations and last_var.max() > self._epsilon:
+            actions_gauss = self._act_from_last_gaus(last_mean=last_mean, last_var=last_var)
+            actions = torch.cat([actions_gauss, actions_actor], dim=1)
             # [horizon, num_sample, action_shape]
             states_repeat, actions_repeat = self._state_action_repeat(state, actions)
             # pylint: disable-next=line-too-long
             # [num_particles * num_samples/num_ensemble, state_shape], [horizon, num_particles * num_samples/num_ensemble, action_shape]
             traj = self._dynamics.imagine(states_repeat, self._horizon, actions_repeat)
             # pylint: disable-next=line-too-long
             # {states, rewards, values}, each value shape is [horizon, num_ensemble, num_particles * num_samples/num_ensemble, 1]
 
             elite_values, elite_actions, info = self._select_elites(actions, traj)
             # [num_sample, 1]
-            new_mean, new_var = self._update_mean_var(elite_actions, elite_values, info)
+            new_mean, new_var = self._update_mean_var(
+                elite_actions,
+                elite_values,
+                info,
+            )
             last_mean = self._momentum * last_mean + (1 - self._momentum) * new_mean
             last_var = self._momentum * last_var + (1 - self._momentum) * new_var
             current_iter += 1
         logger_info = {
             'Plan/iter': current_iter,
             'Plan/last_var_mean': last_var.mean().item(),
             'Plan/last_var_max': last_var.max().item(),
             'Plan/last_var_min': last_var.min().item(),
         }
         logger_info.update(info)
         self._action_sequence_mean = last_mean.clone()
         return last_mean[0].clone().unsqueeze(0), logger_info
-
-    def reset_planner(self) -> None:
-        """Reset the planner."""
-        self._action_sequence_mean = torch.zeros(
-            self._horizon,
-            *self._action_shape,
-            device=self._device,
-        )
-        self._action_sequence_var = self._init_var * torch.ones(
-            self._horizon,
-            *self._action_shape,
-            device=self._device,
-        )
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/model_based/planner/rce.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/model_based/planner/rce.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Model Predictive Control Planner of Robust Cross Entropy algorithm."""
+
+
 from __future__ import annotations
 
 import torch
 
 from omnisafe.algorithms.model_based.planner.cce import CCEPlanner
 
 
@@ -29,26 +31,26 @@
         - URL: `RCE <https://arxiv.org/abs/2010.07968>`_
     """
 
     @torch.no_grad()
     def _select_elites(
         self,
         actions: torch.Tensor,
-        traj: dict,
-    ) -> tuple[torch.Tensor, torch.Tensor, dict]:
+        traj: dict[str, torch.Tensor],
+    ) -> tuple[torch.Tensor, torch.Tensor, dict[str, float]]:
         """Select elites from the sampled actions.
 
         Args:
             actions (torch.Tensor): Sampled actions.
-            traj (dict): Trajectory dictionary.
+            traj (dict[str, torch.Tensor]): Trajectory dictionary.
 
         Returns:
-            elites_value (torch.Tensor): Value of the elites.
-            elites_action (torch.Tensor): Action of the elites.
-            info (dict): Dictionary containing the information of elites value and action.
+            elites_value: The value of the elites.
+            elites_action: The action of the elites.
+            info: The dictionary containing the information of elites value and action.
         """
         rewards = traj['rewards']
         costs = traj['costs']
         assert actions.shape == torch.Size(
             [self._horizon, self._num_samples, *self._action_shape],
             # pylint: disable-next=line-too-long
         ), 'Input action dimension should be equal to (self._horizon, self._num_samples, self._action_shape)'
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/model_based/planner/safe_arc.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/model_based/planner/safe_arc.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Model Predictive Control Planner of the Safe Actor Regularized Control algorithm."""
+
+
 from __future__ import annotations
 
 from typing import Any
 
 import torch
 
 from omnisafe.algorithms.model_based.base.ensemble import EnsembleDynamicsModel
@@ -63,25 +65,26 @@
         self._cost_temperature: float = planner_cfgs.cost_temperature
 
     @torch.no_grad()
     def _update_mean_var(
         self,
         elite_actions: torch.Tensor,
         elite_values: torch.Tensor,
-        info: dict,
+        info: dict[str, int | float],
     ) -> tuple[torch.Tensor, torch.Tensor]:
         """Update the mean and variance of the elite actions.
 
         Args:
-            elite_actions (torch.Tensor): Elite actions.
-            elite_values (torch.Tensor): Elite values.
+            elite_actions (torch.Tensor): The elite actions.
+            elite_values (torch.Tensor): The elite values.
+            info (dict[str, int | float]): The dictionary containing the information of the elite values and actions.
 
         Returns:
-            new_mean (torch.Tensor): New mean of the elite actions.
-            new_var (torch.Tensor): New variance of the elite actions.
+            new_mean: The new mean of the elite actions.
+            new_var: The new variance of the elite actions.
         """
         assert (
             elite_actions.shape[0] == self._horizon
             and elite_actions.shape[-1] == self._action_shape[0]
         ), 'Input elite_actions dimension should be equal to (self._horizon, self._num_elites, self._action_shape)'
         assert (
             elite_values.shape[-1] == 1
@@ -106,26 +109,26 @@
 
         return new_mean, new_var
 
     @torch.no_grad()
     def _select_elites(
         self,
         actions: torch.Tensor,
-        traj: dict,
-    ) -> tuple[torch.Tensor, torch.Tensor, dict]:
+        traj: dict[str, torch.Tensor],
+    ) -> tuple[torch.Tensor, torch.Tensor, dict[str, float]]:
         """Select elites from the sampled actions.
 
         Args:
             actions (torch.Tensor): Sampled actions.
-            traj (dict): Trajectory dictionary.
+            traj (dict[str, torch.Tensor]): Trajectory dictionary.
 
         Returns:
-            elites_value (torch.Tensor): Value of the elites.
-            elites_action (torch.Tensor): Action of the elites.
-            info (dict): Dictionary containing the information of elites value and action.
+            elites_value: The value of the elites.
+            elites_action: The action of the elites.
+            info: The dictionary containing the information of elites value and action.
         """
         rewards = traj['rewards']
         values = traj['values']
         costs = traj['costs']
         assert actions.shape == torch.Size(
             [self._horizon, self._num_action, *self._action_shape],
             # pylint: disable-next=line-too-long
@@ -190,34 +193,35 @@
             'Plan/episode_costs_mean': mean_episode_costs.mean().item(),
             'Plan/episode_costs_min': mean_episode_costs.min().item(),
         }
 
         return elite_values, elite_actions, info
 
     @torch.no_grad()
-    def output_action(self, state: torch.Tensor) -> tuple[torch.Tensor, dict]:
+    def output_action(self, state: torch.Tensor) -> tuple[torch.Tensor, dict[str, int | float]]:
         """Output the action given the state.
 
         Args:
             state (torch.Tensor): State of the environment.
 
         Returns:
-            action (torch.Tensor): Action of the environment.
-            logger_info (dict): Dictionary containing the information of the action.
+            action: The action of the agent.
+            info: The dictionary containing the information of the action.
         """
         assert state.shape == torch.Size(
             [1, *self._dynamics_state_shape],
         ), 'Input state dimension should be equal to (1, self._dynamics_state_shape)'
         last_mean = torch.zeros_like(self._action_sequence_mean)
         last_var = self._action_sequence_var.clone()
         last_mean[:-1] = self._action_sequence_mean[1:].clone()
         last_mean[-1] = self._action_sequence_mean[-1].clone()
 
         current_iter = 0
         actions_actor = self._act_from_actor(state)
+        info: dict[str, int | float] = {}
         while current_iter < self._num_iterations and last_var.max() > self._epsilon:
             actions_gauss = self._act_from_last_gaus(last_mean=last_mean, last_var=last_var)
             actions = torch.cat([actions_gauss, actions_actor], dim=1)
             # [horizon, num_sample, action_shape]
             states_repeat, actions_repeat = self._state_action_repeat(state, actions)
             # pylint: disable-next=line-too-long
             # [num_particles * num_samples/num_ensemble, state_shape], [horizon, num_particles * num_samples/num_ensemble, action_shape]
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/model_based/safeloop.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/model_based/safeloop.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,23 +9,26 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Implementation of the Safe Learning Off-Policy with Online Planning algorithm."""
+
+
 from __future__ import annotations
 
 from gymnasium.spaces import Box
 
 from omnisafe.algorithms import registry
 from omnisafe.algorithms.model_based.base.ensemble import EnsembleDynamicsModel
 from omnisafe.algorithms.model_based.base.loop import LOOP
 from omnisafe.algorithms.model_based.planner.safe_arc import SafeARCPlanner
 from omnisafe.models.actor_critic.constraint_actor_q_critic import ConstraintActorQCritic
+from omnisafe.typing import OmnisafeSpace
 from omnisafe.utils import distributed
 
 
 @registry.register
 # pylint: disable-next=too-many-instance-attributes, too-few-public-methods
 class SafeLOOP(LOOP):
     """The Safe Learning Off-Policy with Online Planning (SafeLOOP) algorithm.
@@ -33,64 +36,87 @@
     References:
         - Title: Learning Off-Policy with Online Planning
         - Authors: Harshit Sikchi, Wenxuan Zhou, David Held.
         - URL: `SafeLOOP <https://arxiv.org/abs/2008.10066>`_
     """
 
     def _init_model(self) -> None:
-        """Initialize the dynamics model and the planner."""
-        self._dynamics_state_space = (
+        """Initialize the dynamics model and the planner.
+
+        SafeLOOP uses following models:
+
+        - dynamics model: to predict the next state and the cost.
+        - planner: to generate the action.
+        """
+        self._dynamics_state_space: OmnisafeSpace = (
             self._env.coordinate_observation_space
             if self._env.coordinate_observation_space is not None
             else self._env.observation_space
         )
+        assert self._dynamics_state_space is not None and isinstance(
+            self._dynamics_state_space.shape,
+            tuple,
+        )
         assert self._env.action_space is not None and isinstance(
             self._env.action_space.shape,
             tuple,
         )
         if isinstance(self._env.action_space, Box):
             self._action_space = self._env.action_space
         else:
             raise NotImplementedError
-        self._actor_critic = ConstraintActorQCritic(
+        self._actor_critic: ConstraintActorQCritic = ConstraintActorQCritic(
             obs_space=self._dynamics_state_space,
             act_space=self._action_space,
             model_cfgs=self._cfgs.model_cfgs,
             epochs=self._epochs,
         ).to(self._device)
         if distributed.world_size() > 1:
             distributed.sync_params(self._actor_critic)
-        self._use_actor_critic = True
-        self._update_count = 0
-        self._dynamics = EnsembleDynamicsModel(
+        self._use_actor_critic: bool = True
+        self._update_count: int = 0
+        self._dynamics: EnsembleDynamicsModel = EnsembleDynamicsModel(
             model_cfgs=self._cfgs.dynamics_cfgs,
             device=self._device,
             state_shape=self._dynamics_state_space.shape,
             action_shape=self._action_space.shape,
             actor_critic=self._actor_critic,
             rew_func=None,
             cost_func=self._env.get_cost_from_obs_tensor,
             terminal_func=None,
         )
-        self._update_dynamics_cycle = int(self._cfgs.algo_cfgs.update_dynamics_cycle)
+        self._update_dynamics_cycle: int = int(self._cfgs.algo_cfgs.update_dynamics_cycle)
 
-        self._planner = SafeARCPlanner(
+        self._planner: SafeARCPlanner = SafeARCPlanner(
             dynamics=self._dynamics,
             planner_cfgs=self._cfgs.planner_cfgs,
             gamma=float(self._cfgs.algo_cfgs.gamma),
             cost_gamma=float(self._cfgs.algo_cfgs.cost_gamma),
             dynamics_state_shape=self._dynamics_state_space.shape,
             action_shape=self._action_space.shape,
             action_max=1.0,
             action_min=-1.0,
             device=self._device,
             cost_limit=float(self._cfgs.algo_cfgs.cost_limit),
             actor_critic=self._actor_critic,
         )
 
     def _init_log(self) -> None:
-        """Initialize the logger keys for the algorithm."""
+        """Initialize the logger keys for the algorithm.
+
+        +----------------------------+-------------------------------+
+        | Things to log              | Description                   |
+        +============================+===============================+
+        | Plan/feasible_num          | The number of feasible plans. |
+        +----------------------------+-------------------------------+
+        | Plan/episode_costs_max     | The maximum planning cost.    |
+        +----------------------------+-------------------------------+
+        | Plan/episode_costs_mean    | The mean planning cost.       |
+        +----------------------------+-------------------------------+
+        | Plan/episode_costs_min     | The minimum planning cost.    |
+        +----------------------------+-------------------------------+
+        """
         super()._init_log()
         self._logger.register_key('Plan/feasible_num')
         self._logger.register_key('Plan/episode_costs_max')
         self._logger.register_key('Plan/episode_costs_mean')
         self._logger.register_key('Plan/episode_costs_min')
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/off_policy/__init__.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/naive_lagrange/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,18 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Off-policy algorithms."""
+"""Naive Lagrange algorithms."""
 
-from omnisafe.algorithms.off_policy.ddpg import DDPG
-from omnisafe.algorithms.off_policy.ddpg_lag import DDPGLag
-from omnisafe.algorithms.off_policy.sac import SAC
-from omnisafe.algorithms.off_policy.sac_lag import SACLag
-from omnisafe.algorithms.off_policy.td3 import TD3
-from omnisafe.algorithms.off_policy.td3_lag import TD3Lag
+from omnisafe.algorithms.on_policy.naive_lagrange.pdo import PDO
+from omnisafe.algorithms.on_policy.naive_lagrange.ppo_lag import PPOLag
+from omnisafe.algorithms.on_policy.naive_lagrange.rcpo import RCPO
+from omnisafe.algorithms.on_policy.naive_lagrange.trpo_lag import TRPOLag
 
 
-__all__ = ['DDPG', 'TD3', 'SAC', 'DDPGLag', 'TD3Lag', 'SACLag']
+__all__ = [
+    'RCPO',
+    'PDO',
+    'PPOLag',
+    'TRPOLag',
+]
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/off_policy/ddpg.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/ddpg.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,16 @@
     References:
         - Title: Continuous control with deep reinforcement learning
         - Authors: Timothy P. Lillicrap, Jonathan J. Hunt, Alexander Pritzel, Nicolas Heess,
             Tom Erez, Yuval Tassa, David Silver, Daan Wierstra.
         - URL: `DDPG <https://arxiv.org/abs/1509.02971>`_
     """
 
+    _epoch: int
+
     def _init_env(self) -> None:
         """Initialize the environment.
 
         OmniSafe uses :class:`omnisafe.adapter.OffPolicyAdapter` to adapt the environment to this
         algorithm.
 
         User can customize the environment by inheriting this method.
@@ -161,15 +163,21 @@
         +-------------------------+----------------------------------------------------------------------+
         | Train/LR                | Learning rate of the policy network.                                 |
         +-------------------------+----------------------------------------------------------------------+
         | Misc/Seed               | Seed of the experiment.                                              |
         +-------------------------+----------------------------------------------------------------------+
         | Misc/TotalEnvSteps      | Total steps of the experiment.                                       |
         +-------------------------+----------------------------------------------------------------------+
-        | Time                    | Total time.                                                          |
+        | Time/Total              | Total time.                                                          |
+        +-------------------------+----------------------------------------------------------------------+
+        | Time/Rollout            | Rollout time.                                                        |
+        +-------------------------+----------------------------------------------------------------------+
+        | Time/Update             | Update time.                                                         |
+        +-------------------------+----------------------------------------------------------------------+
+        | Time/Evaluate           | Evaluate time.                                                       |
         +-------------------------+----------------------------------------------------------------------+
         | FPS                     | Frames per second of the epoch.                                      |
         +-------------------------+----------------------------------------------------------------------+
         """
         self._logger: Logger = Logger(
             output_dir=self._cfgs.logger_cfgs.log_dir,
             exp_name=self._cfgs.exp_name,
@@ -212,18 +220,19 @@
             # log information about cost critic
             self._logger.register_key('Loss/Loss_cost_critic', delta=True)
             self._logger.register_key('Value/cost_critic')
 
         self._logger.register_key('Time/Total')
         self._logger.register_key('Time/Rollout')
         self._logger.register_key('Time/Update')
+        self._logger.register_key('Time/Evaluate')
         self._logger.register_key('Time/Epoch')
         self._logger.register_key('Time/FPS')
 
-    def learn(self) -> tuple[float, float, int]:
+    def learn(self) -> tuple[float, float, float]:
         """This is main function for algorithm update.
 
         It is divided into the following steps:
 
         - :meth:`rollout`: collect interactive data from environment.
         - :meth:`update`: perform actor/critic updates.
         - :meth:`log`: epoch/update information for visualization and terminal log print.
@@ -233,14 +242,15 @@
             ep_cost: average episode cost in final epoch.
             ep_len: average episode length in final epoch.
         """
         self._logger.log('INFO: Start training')
         start_time = time.time()
         step = 0
         for epoch in range(self._epochs):
+            self._epoch = epoch
             rollout_time = 0.0
             update_time = 0.0
             epoch_time = time.time()
 
             for sample_step in range(
                 epoch * self._samples_per_epoch,
                 (epoch + 1) * self._samples_per_epoch,
@@ -267,22 +277,25 @@
                 if step > self._cfgs.algo_cfgs.start_learning_steps:
                     self._update()
                 # if we haven't updated the network, log 0 for the loss
                 else:
                     self._log_when_not_update()
                 update_time += time.time() - update_start
 
+            eval_start = time.time()
             self._env.eval_policy(
-                episode=2,
+                episode=1,
                 agent=self._actor_critic,
                 logger=self._logger,
             )
+            eval_time = time.time() - eval_start
 
             self._logger.store({'Time/Update': update_time})
             self._logger.store({'Time/Rollout': rollout_time})
+            self._logger.store({'Time/Evaluate': eval_time})
 
             if (
                 step > self._cfgs.algo_cfgs.start_learning_steps
                 and self._cfgs.model_cfgs.linear_lr_decay
             ):
                 self._actor_critic.actor_scheduler.step()
 
@@ -301,15 +314,15 @@
 
             # save model to disk
             if (epoch + 1) % self._cfgs.logger_cfgs.save_model_freq == 0:
                 self._logger.torch_save()
 
         ep_ret = self._logger.get_stats('Metrics/EpRet')[0]
         ep_cost = self._logger.get_stats('Metrics/EpCost')[0]
-        ep_len = int(self._logger.get_stats('Metrics/EpLen')[0])
+        ep_len = self._logger.get_stats('Metrics/EpLen')[0]
         self._logger.close()
 
         return ep_ret, ep_cost, ep_len
 
     def _update(self) -> None:
         """Update actor, critic.
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/off_policy/ddpg_lag.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/ddpg_lag.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -58,15 +58,16 @@
         """Update actor, critic, as we used in the :class:`PolicyGradient` algorithm.
 
         Additionally, we update the Lagrange multiplier parameter by calling the
         :meth:`update_lagrange_multiplier` method.
         """
         super()._update()
         Jc = self._logger.get_stats('Metrics/EpCost')[0]
-        self._lagrange.update_lagrange_multiplier(Jc)
+        if self._epoch > self._cfgs.algo_cfgs.warmup_epochs:
+            self._lagrange.update_lagrange_multiplier(Jc)
         self._logger.store(
             {
                 'Metrics/LagrangeMultiplier': self._lagrange.lagrangian_multiplier.data.item(),
             },
         )
 
     def _loss_pi(
@@ -77,16 +78,16 @@
 
         The loss function in DDPGLag is defined as:
 
         .. math::
 
             L = -Q^V (s, \pi (s)) + \lambda Q^C (s, \pi (s))
 
-        where :math:`Q^V` is the value of reward critic network output,
-        and :math:`\pi` is the policy network.
+        where :math:`Q^V` is the min value of two reward critic networks outputs, :math:`Q^C` is the
+        value of cost critic network, and :math:`\pi` is the policy network.
 
         Args:
             obs (torch.Tensor): The ``observation`` sampled from buffer.
 
         Returns:
             The loss of pi/actor.
         """
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/off_policy/sac.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/sac.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,25 +38,15 @@
     _log_alpha: torch.Tensor
     _alpha_optimizer: optim.Optimizer
     _target_entropy: float
 
     def _init_model(self) -> None:
         """Initialize the model.
 
-        OmniSafe uses :class:`omnisafe.models.actor_critic.constraint_actor_q_critic.ConstraintActorQCritic`
-        as the default model.
-
-        User can customize the model by inheriting this method.
-
-        .. note::
-            The ``num_critics`` in ``critic`` configuration must be 2.
-
-        Examples:
-            >>> def _init_model(self) -> None:
-            ...     self._actor_critic = CustomActorQCritic()
+        The ``num_critics`` in ``critic`` configuration must be 2.
         """
         self._cfgs.model_cfgs.critic['num_critics'] = 2
         self._actor_critic = ConstraintActorQCritic(
             obs_space=self._env.observation_space,
             act_space=self._env.action_space,
             model_cfgs=self._cfgs.model_cfgs,
             epochs=self._epochs,
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/off_policy/sac_lag.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/sac_lag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -57,15 +57,16 @@
         """Update actor, critic, as we used in the :class:`PolicyGradient` algorithm.
 
         Additionally, we update the Lagrange multiplier parameter by calling the
         :meth:`update_lagrange_multiplier` method.
         """
         super()._update()
         Jc = self._logger.get_stats('Metrics/EpCost')[0]
-        self._lagrange.update_lagrange_multiplier(Jc)
+        if self._epoch > self._cfgs.algo_cfgs.warmup_epochs:
+            self._lagrange.update_lagrange_multiplier(Jc)
         self._logger.store(
             {
                 'Metrics/LagrangeMultiplier': self._lagrange.lagrangian_multiplier.data.item(),
             },
         )
 
     def _loss_pi(
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/off_policy/td3.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/td3.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,25 +34,15 @@
         - Authors: Scott Fujimoto, Herke van Hoof, David Meger.
         - URL: `TD3 <https://arxiv.org/abs/1802.09477>`_
     """
 
     def _init_model(self) -> None:
         """Initialize the model.
 
-        OmniSafe uses :class:`omnisafe.models.actor_critic.constraint_actor_q_critic.ConstraintActorQCritic`
-        as the default model.
-
-        User can customize the model by inheriting this method.
-
-        .. note::
-            The ``num_critics`` in ``critic`` configuration must be 2.
-
-        Examples:
-            >>> def _init_model(self) -> None:
-            ...     self._actor_critic = CustomActorQCritic()
+        The ``num_critics`` in ``critic`` configuration must be 2.
         """
         self._cfgs.model_cfgs.critic['num_critics'] = 2
         self._actor_critic = ConstraintActorQCritic(
             obs_space=self._env.observation_space,
             act_space=self._env.action_space,
             model_cfgs=self._cfgs.model_cfgs,
             epochs=self._epochs,
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/off_policy/td3_lag.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/td3_lag.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -57,15 +57,16 @@
         """Update actor, critic, as we used in the :class:`PolicyGradient` algorithm.
 
         Additionally, we update the Lagrange multiplier parameter by calling the
         :meth:`update_lagrange_multiplier` method.
         """
         super()._update()
         Jc = self._logger.get_stats('Metrics/EpCost')[0]
-        self._lagrange.update_lagrange_multiplier(Jc)
+        if self._epoch > self._cfgs.algo_cfgs.warmup_epochs:
+            self._lagrange.update_lagrange_multiplier(Jc)
         self._logger.store(
             {
                 'Metrics/LagrangeMultiplier': self._lagrange.lagrangian_multiplier.data.item(),
             },
         )
 
     def _loss_pi(
@@ -76,16 +77,16 @@
 
         The loss function in TD3Lag is defined as:
 
         .. math::
 
             L = -Q^V (s, \pi (s)) + \lambda Q^C (s, \pi (s))
 
-        where :math:`Q^V` is the value of reward critic network output, :math:`Q^C` is the value of
-        cost critic network, and :math:`\pi` is the policy network.
+        where :math:`Q^V` is the min value of two reward critic networks outputs, :math:`Q^C` is the
+        value of cost critic network, and :math:`\pi` is the policy network.
 
         Args:
             obs (torch.Tensor): The ``observation`` sampled from buffer.
 
         Returns:
             The loss of pi/actor.
         """
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/__init__.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -17,33 +17,36 @@
 from omnisafe.algorithms.on_policy import (
     base,
     early_terminated,
     first_order,
     naive_lagrange,
     penalty_function,
     pid_lagrange,
+    primal,
     saute,
     second_order,
     simmer,
 )
 from omnisafe.algorithms.on_policy.base import PPO, TRPO, NaturalPG, PolicyGradient
 from omnisafe.algorithms.on_policy.early_terminated import PPOEarlyTerminated, TRPOEarlyTerminated
 from omnisafe.algorithms.on_policy.first_order import CUP, FOCOPS
-from omnisafe.algorithms.on_policy.naive_lagrange import PDO, RCPO, OnCRPO, PPOLag, TRPOLag
+from omnisafe.algorithms.on_policy.naive_lagrange import PDO, RCPO, PPOLag, TRPOLag
 from omnisafe.algorithms.on_policy.penalty_function import IPO, P3O
 from omnisafe.algorithms.on_policy.pid_lagrange import CPPOPID, TRPOPID
+from omnisafe.algorithms.on_policy.primal import OnCRPO
 from omnisafe.algorithms.on_policy.saute import PPOSaute, TRPOSaute
 from omnisafe.algorithms.on_policy.second_order import CPO, PCPO
 from omnisafe.algorithms.on_policy.simmer import PPOSimmerPID, TRPOSimmerPID
 
 
 __all__ = [
     *base.__all__,
     *early_terminated.__all__,
     *first_order.__all__,
     *naive_lagrange.__all__,
+    *primal.__all__,
     *penalty_function.__all__,
     *pid_lagrange.__all__,
     *saute.__all__,
     *second_order.__all__,
     *simmer.__all__,
 ]
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/base/__init__.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/base/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/base/natural_pg.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/base/natural_pg.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
         Build the `Hessian-vector product <https://en.wikipedia.org/wiki/Hessian_matrix>`_ , which
         is the second-order derivative of the KL-divergence.
 
         The Hessian-vector product is approximated by the Fisher information matrix, which is the
         second-order derivative of the KL-divergence.
 
-        For details see John Schulman's PhD thesis (pp. 40) http://joschu.net/docs/thesis.pdf .
+        For details see `John Schulman's PhD thesis (pp. 40) <http://joschu.net/docs/thesis.pdf>`_ .
 
         Args:
             params (torch.Tensor): The parameters of the actor network.
 
         Returns:
             The Fisher vector product.
         """
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/base/policy_gradient.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/base/policy_gradient.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,27 +218,27 @@
 
         self._logger.register_key('Time/Total')
         self._logger.register_key('Time/Rollout')
         self._logger.register_key('Time/Update')
         self._logger.register_key('Time/Epoch')
         self._logger.register_key('Time/FPS')
 
-    def learn(self) -> tuple[float, float, int]:
+    def learn(self) -> tuple[float, float, float]:
         """This is main function for algorithm update.
 
         It is divided into the following steps:
 
         - :meth:`rollout`: collect interactive data from environment.
         - :meth:`update`: perform actor/critic updates.
         - :meth:`log`: epoch/update information for visualization and terminal log print.
 
         Returns:
-            ep_ret: average episode return in final epoch.
-            ep_cost: average episode cost in final epoch.
-            ep_len: average episode length in final epoch.
+            ep_ret: Average episode return in final epoch.
+            ep_cost: Average episode cost in final epoch.
+            ep_len: Average episode length in final epoch.
         """
         start_time = time.time()
         self._logger.log('INFO: Start training')
 
         for epoch in range(self._cfgs.train_cfgs.epochs):
             epoch_time = time.time()
 
@@ -278,15 +278,15 @@
 
             # save model to disk
             if (epoch + 1) % self._cfgs.logger_cfgs.save_model_freq == 0:
                 self._logger.torch_save()
 
         ep_ret = self._logger.get_stats('Metrics/EpRet')[0]
         ep_cost = self._logger.get_stats('Metrics/EpCost')[0]
-        ep_len = int(self._logger.get_stats('Metrics/EpLen')[0])
+        ep_len = self._logger.get_stats('Metrics/EpLen')[0]
         self._logger.close()
 
         return ep_ret, ep_cost, ep_len
 
     def _update(self) -> None:
         """Update actor, critic.
 
@@ -516,15 +516,15 @@
         Policy Gradient only use reward advantage.
 
         Args:
             adv_r (torch.Tensor): The ``reward_advantage`` sampled from buffer.
             adv_c (torch.Tensor): The ``cost_advantage`` sampled from buffer.
 
         Returns:
-            The ``reward_advantage`` used to update policy network.
+            The advantage function of reward to update policy network.
         """
         return adv_r
 
     def _loss_pi(
         self,
         obs: torch.Tensor,
         act: torch.Tensor,
@@ -533,27 +533,27 @@
     ) -> torch.Tensor:
         r"""Computing pi/actor loss.
 
         In Policy Gradient, the loss is defined as:
 
         .. math::
 
-            L = -\mathbb{E}_{s_t \sim \rho_{\theta}} [
+            L = -\underset{s_t \sim \rho_{\theta}}{\mathbb{E}} [
                 \sum_{t=0}^T ( \frac{\pi^{'}_{\theta}(a_t|s_t)}{\pi_{\theta}(a_t|s_t)} )
                  A^{R}_{\pi_{\theta}}(s_t, a_t)
             ]
 
         where :math:`\pi_{\theta}` is the policy network, :math:`\pi^{'}_{\theta}`
         is the new policy network, :math:`A^{R}_{\pi_{\theta}}(s_t, a_t)` is the advantage.
 
         Args:
             obs (torch.Tensor): The ``observation`` sampled from buffer.
             act (torch.Tensor): The ``action`` sampled from buffer.
             logp (torch.Tensor): The ``log probability`` of action sampled from buffer.
-            adv (torch.Tensor): The ``advantage`` sampled from buffer.
+            adv (torch.Tensor): The ``advantage`` processed. ``reward_advantage`` here.
 
         Returns:
             The loss of pi/actor.
         """
         distribution = self._actor_critic.actor(obs)
         logp_ = self._actor_critic.actor.log_prob(act)
         std = self._actor_critic.actor.std
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/base/ppo.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/base/ppo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -41,28 +41,28 @@
     ) -> torch.Tensor:
         r"""Computing pi/actor loss.
 
         In Proximal Policy Optimization, the loss is defined as:
 
         .. math::
 
-            L^{CLIP} = \mathbb{E}_{s_t \sim \rho_{\theta}} \left[
+            L^{CLIP} = \underset{s_t \sim \rho_{\theta}}{\mathbb{E}} \left[
                 \min ( r_t A^{R}_{\pi_{\theta}} (s_t, a_t) , \text{clip} (r_t, 1 - \epsilon, 1 + \epsilon)
                 A^{R}_{\pi_{\theta}} (s_t, a_t)
             \right]
 
         where :math:`r_t = \frac{\pi_{\theta}^{'} (a_t|s_t)}{\pi_{\theta} (a_t|s_t)}`,
         :math:`\epsilon` is the clip parameter, and :math:`A^{R}_{\pi_{\theta}} (s_t, a_t)` is the
         advantage.
 
         Args:
             obs (torch.Tensor): The ``observation`` sampled from buffer.
             act (torch.Tensor): The ``action`` sampled from buffer.
             logp (torch.Tensor): The ``log probability`` of action sampled from buffer.
-            adv (torch.Tensor): The ``advantage`` sampled from buffer.
+            adv (torch.Tensor): The ``advantage`` processed. ``reward_advantage`` here.
 
         Returns:
             The loss of pi/actor.
         """
         distribution = self._actor_critic.actor(obs)
         logp_ = self._actor_critic.actor.log_prob(act)
         std = self._actor_critic.actor.std
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/base/trpo.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/base/trpo.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,22 @@
     References:
         - Title: Trust Region Policy Optimization
         - Authors: John Schulman, Sergey Levine, Philipp Moritz, Michael I. Jordan, Pieter Abbeel.
         - URL: `TRPO <https://arxiv.org/abs/1502.05477>`_
     """
 
     def _init_log(self) -> None:
+        """Log the Trust Region Policy Optimization specific information.
+
+        +---------------------+-----------------------------+
+        | Things to log       | Description                 |
+        +=====================+=============================+
+        | Misc/AcceptanceStep | The acceptance step size.   |
+        +---------------------+-----------------------------+
+        """
         super()._init_log()
         self._logger.register_key('Misc/AcceptanceStep')
 
     # pylint: disable-next=too-many-arguments,too-many-locals,arguments-differ
     def _search_step_size(
         self,
         step_direction: torch.Tensor,
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/early_terminated/__init__.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/early_terminated/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/early_terminated/ppo_early_terminated.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/early_terminated/ppo_early_terminated.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/early_terminated/trpo_early_terminated.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/early_terminated/trpo_early_terminated.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/first_order/__init__.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/first_order/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/first_order/cup.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/first_order/cup.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,23 +128,15 @@
             },
         )
         return loss
 
     def _update(self) -> None:
         r"""Update actor, critic, and Lagrange multiplier parameters.
 
-        In CUP, the Lagrange multiplier is updated as the naive lagrange multiplier update:
-
-        .. math::
-
-            \lambda_{k+1} = \lambda_k + \eta (J^{C}_{\pi_{\theta}} - C)
-
-        where :math:`\lambda_k` is the Lagrange multiplier at iteration :math:`k`, :math:`\eta` is
-        the Lagrange multiplier learning rate, :math:`J^{C}_{\pi_{\theta}}` is the cost of the
-        current policy, and :math:`C` is the cost limit.
+        In CUP, the Lagrange multiplier is updated as the naive lagrange multiplier update.
 
         Then in each iteration of the policy update, CUP calculates current policy's distribution,
         which used to calculate the policy loss.
         """
         # note that logger already uses MPI statistics across all processes..
         Jc = self._logger.get_stats('Metrics/EpCost')[0]
         # first update Lagrange multiplier parameter
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/first_order/focops.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/first_order/focops.py`

 * *Files 7% similar despite different names*

```diff
@@ -131,32 +131,24 @@
             ]
 
         Args:
             adv_r (torch.Tensor): The ``reward_advantage`` sampled from buffer.
             adv_c (torch.Tensor): The ``cost_advantage`` sampled from buffer.
 
         Returns:
-            The ``advantage`` combined with ``reward_advantage`` and ``cost_advantage``.
+            The advantage function combined with reward and cost.
         """
         return (adv_r - self._lagrange.lagrangian_multiplier * adv_c) / (
             1 + self._lagrange.lagrangian_multiplier
         )
 
     def _update(self) -> None:
         r"""Update actor, critic, and Lagrange multiplier parameters.
 
-        In FOCOPS, the Lagrange multiplier is updated as the naive lagrange multiplier update:
-
-        .. math::
-
-            \lambda_{k+1} = \lambda_k + \eta (J^{C}_{\pi_{\theta}} - C)
-
-        where :math:`\lambda_k` is the Lagrange multiplier at iteration :math:`k`, :math:`\eta` is
-        the Lagrange multiplier learning rate, :math:`J^{C}_{\pi_{\theta}}` is the cost of the current
-        policy, and :math:`C` is the cost limit.
+        In FOCOPS, the Lagrange multiplier is updated as the naive lagrange multiplier update.
 
         Then in each iteration of the policy update, FOCOPS calculates current policy's
         distribution, which used to calculate the policy loss.
         """
         # note that logger already uses MPI statistics across all processes..
         Jc = self._logger.get_stats('Metrics/EpCost')[0]
         # first update Lagrange multiplier parameter
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/naive_lagrange/__init__.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/pid_lagrange/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,24 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Naive Lagrange algorithms."""
+"""PID Lagrange algorithms."""
 
-from omnisafe.algorithms.on_policy.naive_lagrange.crpo import OnCRPO
-from omnisafe.algorithms.on_policy.naive_lagrange.pdo import PDO
-from omnisafe.algorithms.on_policy.naive_lagrange.ppo_lag import PPOLag
-from omnisafe.algorithms.on_policy.naive_lagrange.rcpo import RCPO
-from omnisafe.algorithms.on_policy.naive_lagrange.trpo_lag import TRPOLag
+from omnisafe.algorithms.on_policy.pid_lagrange.cppo_pid import CPPOPID
+from omnisafe.algorithms.on_policy.pid_lagrange.trpo_pid import TRPOPID
 
 
 __all__ = [
-    'OnCRPO',
-    'RCPO',
-    'PDO',
-    'PPOLag',
-    'TRPOLag',
+    'CPPOPID',
+    'TRPOPID',
 ]
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/naive_lagrange/crpo.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/primal/crpo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -60,15 +60,15 @@
         cost.
 
         Args:
             adv_r (torch.Tensor): The ``reward_advantage`` sampled from buffer.
             adv_c (torch.Tensor): The ``cost_advantage`` sampled from buffer.
 
         Returns:
-            The ``advantage`` chosen from ``reward_advantage`` and ``cost_advantage``.
+            The advantage function chosen from reward and cost.
         """
         Jc = self._logger.get_stats('Metrics/EpCost')[0]
         if Jc <= self._cfgs.algo_cfgs.cost_limit + self._cfgs.algo_cfgs.distance:
             self._rew_update += 1
             return adv_r
         self._cost_update += 1
         return -adv_c
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/naive_lagrange/pdo.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/naive_lagrange/pdo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -57,17 +57,17 @@
         .. note::
             The :meth:`compute_loss_pi` is defined in the :class:`PolicyGradient` algorithm. When a
             lagrange multiplier is used, the :meth:`compute_loss_pi` method will return the loss of
             the policy as:
 
             .. math::
 
-                L_{\pi} = \mathbb{E}_{s_t \sim \rho_{\pi}} \left[
-                    \frac{\pi_{\theta} (a_t|s_t)}{\pi_{\theta}^{old} (a_t|s_t)}
-                    [ A^{R} (s_t, a_t) - \lambda A^{C} (s_t, a_t) ]
+                L_{\pi} = -\underset{s_t \sim \rho_{\theta}}{\mathbb{E}} \left[
+                    \frac{\pi_{\theta} (a_t|s_t)}{\pi_{\theta}^{old}(a_t|s_t)}
+                    [ A^{R}_{\pi_{\theta}} (s_t, a_t) - \lambda A^{C}_{\pi_{\theta}} (s_t, a_t) ]
                 \right]
 
             where :math:`\lambda` is the Lagrange multiplier parameter.
         """
         # note that logger already uses MPI statistics across all processes..
         Jc = self._logger.get_stats('Metrics/EpCost')[0]
         # first update Lagrange multiplier parameter
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/naive_lagrange/ppo_lag.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/naive_lagrange/ppo_lag.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -58,15 +58,15 @@
         .. note::
             The :meth:`_loss_pi` is defined in the :class:`PolicyGradient` algorithm. When a
             lagrange multiplier is used, the :meth:`_loss_pi` method will return the loss of the
             policy as:
 
             .. math::
 
-                L_{\pi} = \mathbb{E}_{s_t \sim \rho_{\pi}} \left[
+                L_{\pi} = -\underset{s_t \sim \rho_{\theta}}{\mathbb{E}} \left[
                     \frac{\pi_{\theta} (a_t|s_t)}{\pi_{\theta}^{old}(a_t|s_t)}
                     [ A^{R}_{\pi_{\theta}} (s_t, a_t) - \lambda A^{C}_{\pi_{\theta}} (s_t, a_t) ]
                 \right]
 
             where :math:`\lambda` is the Lagrange multiplier parameter.
         """
         # note that logger already uses MPI statistics across all processes..
@@ -92,11 +92,11 @@
             ]
 
         Args:
             adv_r (torch.Tensor): The ``reward_advantage`` sampled from buffer.
             adv_c (torch.Tensor): The ``cost_advantage`` sampled from buffer.
 
         Returns:
-            The ``advantage`` combined with ``reward_advantage`` and ``cost_advantage``.
+            The advantage function combined with reward and cost.
         """
         penalty = self._lagrange.lagrangian_multiplier.item()
         return (adv_r - penalty * adv_c) / (1 + penalty)
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/naive_lagrange/rcpo.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/naive_lagrange/rcpo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -60,17 +60,17 @@
         .. note::
             The :meth:`compute_loss_pi` is defined in the :class:`PolicyGradient` algorithm. When a
             lagrange multiplier is used, the :meth:`compute_loss_pi` method will return the loss of
             the policy as:
 
             .. math::
 
-                L_{\pi} = \mathbb{E}_{s_t \sim \rho_{\pi}} \left[
-                    \frac{\pi_{\theta} (a_t|s_t)}{\pi_{\theta}^{old} (a_t|s_t)}
-                    [ A^{R} (s_t, a_t) - \lambda A^{C} (s_t, a_t) ]
+                L_{\pi} = -\underset{s_t \sim \rho_{\theta}}{\mathbb{E}} \left[
+                    \frac{\pi_{\theta} (a_t|s_t)}{\pi_{\theta}^{old}(a_t|s_t)}
+                    [ A^{R}_{\pi_{\theta}} (s_t, a_t) - \lambda A^{C}_{\pi_{\theta}} (s_t, a_t) ]
                 \right]
 
             where :math:`\lambda` is the Lagrange multiplier parameter.
         """
         # note that logger already uses MPI statistics across all processes..
         Jc = self._logger.get_stats('Metrics/EpCost')[0]
         # first update Lagrange multiplier parameter
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/naive_lagrange/trpo_lag.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/naive_lagrange/trpo_lag.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -57,16 +57,16 @@
         .. note::
             The :meth:`_loss_pi` is defined in the :class:`PolicyGradient` algorithm. When a
             lagrange multiplier is used, the :meth:`_loss_pi` method will return the loss of the
             policy as:
 
             .. math::
 
-                L_{\pi} = \mathbb{E}_{s_t \sim \rho_{\pi}} \left[
-                    \frac{\pi_{\theta} (a_t|s_t)}{\pi_{\theta}^{old} (a_t|s_t)}
+                L_{\pi} = -\underset{s_t \sim \rho_{\theta}}{\mathbb{E}} \left[
+                    \frac{\pi_{\theta} (a_t|s_t)}{\pi_{\theta}^{old}(a_t|s_t)}
                     [ A^{R}_{\pi_{\theta}} (s_t, a_t) - \lambda A^{C}_{\pi_{\theta}} (s_t, a_t) ]
                 \right]
 
             where :math:`\lambda` is the Lagrange multiplier parameter.
         """
         # note that logger already uses MPI statistics across all processes..
         Jc = self._logger.get_stats('Metrics/EpCost')[0]
@@ -90,11 +90,11 @@
             ]
 
         Args:
             adv_r (torch.Tensor): The ``reward_advantage`` sampled from buffer.
             adv_c (torch.Tensor): The ``cost_advantage`` sampled from buffer.
 
         Returns:
-            The ``advantage`` combined with ``reward_advantage`` and ``cost_advantage``.
+            The advantage function combined with reward and cost.
         """
         penalty = self._lagrange.lagrangian_multiplier.item()
         return (adv_r - penalty * adv_c) / (1 + penalty)
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/penalty_function/__init__.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/penalty_function/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/penalty_function/ipo.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/penalty_function/ipo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -45,28 +45,28 @@
     def _compute_adv_surrogate(self, adv_r: torch.Tensor, adv_c: torch.Tensor) -> torch.Tensor:
         r"""Compute surrogate loss.
 
         IPO uses the following surrogate loss:
 
         .. math::
 
-            L = \mathbb{E}_{s_t \sim \pi_{\theta}} \left[
+            L = -\underset{s_t \sim \rho_{\theta}}{\mathbb{E}} \left[
                 \frac{\pi_{\theta}^{'} (a_t|s_t)}{\pi_{\theta} (a_t|s_t)} A (s_t, a_t)
                 - \kappa \frac{J^{C}_{\pi_{\theta}} (s_t, a_t)}{C - J^{C}_{\pi_{\theta}} (s_t, a_t) + \epsilon}
             \right]
 
         Where :math:`\kappa` is the penalty coefficient, :math:`C` is the cost limit,
         and :math:`\epsilon` is a small number to avoid division by zero.
 
         Args:
             adv_r (torch.Tensor): The ``reward_advantage`` sampled from buffer.
             adv_c (torch.Tensor): The ``cost_advantage`` sampled from buffer.
 
         Returns:
-            The ``advantage`` combined with ``reward_advantage`` and ``cost_advantage``.
+            The advantage function combined with reward and cost.
         """
         Jc = self._logger.get_stats('Metrics/EpCost')[0]
         penalty = self._cfgs.algo_cfgs.kappa / (self._cfgs.algo_cfgs.cost_limit - Jc + 1e-8)
         if penalty < 0 or penalty > self._cfgs.algo_cfgs.penalty_max:
             penalty = self._cfgs.algo_cfgs.penalty_max
 
         self._logger.store({'Misc/Penalty': penalty})
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/penalty_function/p3o.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/penalty_function/p3o.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -54,15 +54,15 @@
     ) -> torch.Tensor:
         r"""Compute the performance of cost on this moment.
 
         We compute the loss of cost of policy cost from real cost.
 
         .. math::
 
-            L = \mathbb{E}_{\pi} \left[
+            L = -\underset{s_t \sim \rho_{\theta}}{\mathbb{E}}  \left[
                 \frac{\pi^{'} (a|s)}{\pi (a|s)} A^{C}_{\pi_{\theta}} (s, a)
             \right]
 
         where :math:`A^{C}_{\pi_{\theta}} (s, a)` is the cost advantage, :math:`\pi (a|s)` is the
         old policy, and :math:`\pi^{'} (a|s)` is the current policy.
 
         Args:
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/pid_lagrange/__init__.py` & `omnisafe-0.5.0b0/omnisafe/utils/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,15 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""PID Lagrange algorithms."""
-
-from omnisafe.algorithms.on_policy.pid_lagrange.cppo_pid import CPPOPID
-from omnisafe.algorithms.on_policy.pid_lagrange.trpo_pid import TRPOPID
-
-
-__all__ = [
-    'CPPOPID',
-    'TRPOPID',
-]
+"""Utility functions for OmniSafe."""
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/pid_lagrange/cppo_pid.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/pid_lagrange/cppo_pid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/pid_lagrange/trpo_pid.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/pid_lagrange/trpo_pid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/saute/__init__.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/saute/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/saute/ppo_saute.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/saute/ppo_saute.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/saute/trpo_saute.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/saute/trpo_saute.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/second_order/__init__.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/second_order/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/second_order/cpo.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/second_order/cpo.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/second_order/pcpo.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/second_order/pcpo.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/simmer/__init__.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/simmer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/simmer/ppo_simmer_pid.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/simmer/ppo_simmer_pid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/on_policy/simmer/trpo_simmer_pid.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/simmer/trpo_simmer_pid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/algorithms/registry.py` & `omnisafe-0.5.0b0/omnisafe/algorithms/registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/common/__init__.py` & `omnisafe-0.5.0b0/omnisafe/common/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/common/buffer/__init__.py` & `omnisafe-0.5.0b0/omnisafe/common/buffer/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/common/buffer/base.py` & `omnisafe-0.5.0b0/omnisafe/common/buffer/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/common/buffer/offpolicy_buffer.py` & `omnisafe-0.5.0b0/omnisafe/common/buffer/offpolicy_buffer.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.4.0/omnisafe/common/buffer/onpolicy_buffer.py` & `omnisafe-0.5.0b0/omnisafe/common/buffer/onpolicy_buffer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -24,15 +24,15 @@
 from omnisafe.utils.math import discount_cumsum
 
 
 class OnPolicyBuffer(BaseBuffer):  # pylint: disable=too-many-instance-attributes
     """A buffer for storing trajectories experienced by an agent interacting with the environment.
 
     Besides, The buffer also provides the functionality of calculating the advantages of
-    state-action pairs, ranging from ``GAE``, ``GAE-RTG`` ,``V-trace`` to ``Plain`` method.
+    state-action pairs, ranging from ``GAE``, ``GAE-RTG`` , ``V-trace`` to ``Plain`` method.
 
     .. warning::
         The buffer only supports Box spaces.
 
     Compared to the base buffer, the on-policy buffer stores extra data:
 
     +----------------+---------+---------------+----------------------------------------+
```

### Comparing `omnisafe-0.4.0/omnisafe/common/buffer/vector_offpolicy_buffer.py` & `omnisafe-0.5.0b0/omnisafe/common/buffer/vector_offpolicy_buffer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/common/buffer/vector_onpolicy_buffer.py` & `omnisafe-0.5.0b0/omnisafe/common/buffer/vector_onpolicy_buffer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -90,51 +90,38 @@
 
     @property
     def num_buffers(self) -> int:
         """Number of buffers."""
         return self._num_buffers
 
     def store(self, **data: torch.Tensor) -> None:
-        """Store data into the buffer.
-
-        .. hint::
-            The data should be a list of tensors, each of which corresponds to one environment. Then
-            the data will be stored into the corresponding buffer.
-        """
+        """Store vectorized data into vectorized buffer."""
         for i, buffer in enumerate(self.buffers):
             buffer.store(**{k: v[i] for k, v in data.items()})
 
     def finish_path(
         self,
         last_value_r: torch.Tensor | None = None,
         last_value_c: torch.Tensor | None = None,
         idx: int = 0,
     ) -> None:
         """Get the data in the buffer.
 
         In vector-on-policy buffer, we get the data from each buffer and then concatenate them.
-
-        .. hint::
-            We provide a trick to standardize the advantages of state-action pairs. We calculate the
-            mean and standard deviation of the advantages of state-action pairs and then standardize
-            the advantages of state-action pairs. You can turn on this trick by setting the
-            ``standardized_adv_r`` to ``True``. The same trick is applied to the advantages of the
-            cost.
         """
         self.buffers[idx].finish_path(last_value_r, last_value_c)
 
     def get(self) -> dict[str, torch.Tensor]:
         """Get the data in the buffer.
 
-        .. hint::
-            We provide a trick to standardize the advantages of state-action pairs. We calculate the
-            mean and standard deviation of the advantages of state-action pairs and then standardize
-            the advantages of state-action pairs. You can turn on this trick by setting the
-            ``standardized_adv_r`` to ``True``. The same trick is applied to the advantages of the
-            cost.
+        We provide a trick to standardize the advantages of state-action pairs. We calculate the
+        mean and standard deviation of the advantages of state-action pairs and then standardize
+        the advantages of state-action pairs. You can turn on this trick by setting the
+        ``standardized_adv_r`` to ``True``. The same trick is applied to the advantages of the
+        cost.
 
         Returns:
             The data stored and calculated in the buffer.
         """
         data_pre = {k: [v] for k, v in self.buffers[0].get().items()}
         for buffer in self.buffers[1:]:
             for k, v in buffer.get().items():
```

### Comparing `omnisafe-0.4.0/omnisafe/common/experiment_grid.py` & `omnisafe-0.5.0b0/omnisafe/common/experiment_grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 
 # pylint: disable-next=too-many-instance-attributes
 class ExperimentGrid:
     """Tool for running many experiments given hyper-parameters ranges.
 
     Args:
-        exp_name (str, optional): Name of the experiment grid. Defaults to ''.
+        exp_name (str, optional): Name of the experiment grid. Defaults to ' '.
 
     Attributes:
         keys (list[str]): The keys of the configurations for the experiments.
         vals (list[Any]): The values of the configurations for the experiments.
         shs (list[str]): The shorthands of the configurations for the experiments.
         in_names (list[bool]): Whether the shorthand is included in the name of the experiment.
         div_line_width (int): The width of the dividing line.
@@ -86,19 +86,19 @@
         """Print a helpful report about the experiment grid.
 
         This function prints a helpful report about the experiment grid, including the name of the
         experiment grid, the parameters being varied, and the possible values for each parameter.
 
         In Command Line:
 
-        .. code-block:: text
+        .. code-block:: bash
 
             ===================== ExperimentGrid [test] runs over parameters: =====================
             env_name                                [env]
-            ['SafetyPointGoal1-v0', 'MountainCar-v0', 'Acrobot-v1']
+            ['SafetyPointGoal1-v0', 'SafetyAntVelocity-v1']
             algo                                    [algo]
             ['SAC', 'DDPG', 'TD3']
             seed                                    [seed]
             [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
         """
         print('=' * self.div_line_width)
 
@@ -173,15 +173,15 @@
         By default, if a shorthand isn't given, one is automatically generated from the key using
         the first three letters of each colon-separated term.
 
         .. hint::
             This function is called in ``omnisafe/examples/benchmarks/run_experiment_grid.py``.
 
         Examples:
-            >>> add('env_id', ['SafetyPointGoal1-v0', 'MountainCar-v0', 'Acrobot-v1'])
+            >>> add('env_id', ['SafetyPointGoal1-v0', 'SafetyAntVelocity-v1'])
             >>> add('algo', ['SAC', 'DDPG', 'TD3'])
             >>> add('seed', [0, 1, 2, 3, 4, 5, 6, 7, 8, 9])
 
         Args:
             key (str): Name of parameter.
             vals (list or object): Possible values for parameter.
             shorthand (str, optional): Shorthand for parameter.
@@ -381,15 +381,15 @@
             return new_var
 
         return [check_duplicate(var) for var in flat_variants]
 
     # pylint: disable-next=too-many-locals
     def run(
         self,
-        thunk: Callable[[str, str, str, dict[str, Any]], tuple[float, float, int]],
+        thunk: Callable[[str, str, str, dict[str, Any]], tuple[float, float, float]],
         num_pool: int = 1,
         parent_dir: str | None = None,
         is_test: bool = False,
         gpu_id: list[int] | None = None,
     ) -> None:
         """Run each variant in the grid with function 'thunk'.
 
@@ -454,14 +454,16 @@
                 device_id = gpu_id[idx % len(gpu_id)]
                 device = f'cuda:{device_id}'
                 self.update_dict(var, {'train_cfgs': {'device': device}})
             exp_name = recursive_dict2json(clean_var)
             hashed_exp_name = var['env_id'][:30] + '---' + hash_string(exp_name)
             exp_names.append(':'.join((hashed_exp_name[:5], exp_name)))
             exp_log_dir = os.path.join(self.log_dir, hashed_exp_name, '')
+            if not var.get('logger_cfgs'):
+                var['logger_cfgs'] = {'log_dir': './exp'}
             var['logger_cfgs'].update({'log_dir': exp_log_dir})
             self.save_same_exps_config(exp_log_dir, var)
             results.append(pool.submit(thunk, str(idx), var['algo'], var['env_id'], var))
         pool.shutdown()
 
         if not is_test:
             self.save_results(exp_names, variants, results)
@@ -541,15 +543,15 @@
         compare_num: int | None = None,
         cost_limit: float | None = None,
         show_image: bool = False,
     ) -> None:
         """Analyze the experiment results.
 
         .. note::
-            `values` and `compare_num` cannot be set at the same time.
+            ``values`` and ``compare_num`` cannot be set at the same time.
 
         Args:
             parameter (str): Name of parameter to analyze.
             values (list[Any] or None, optional): Specific values of attribute, if it is specified,
                 will only compare values in it. Defaults to None.
             compare_num (int or None, optional): Number of values to compare, if it is specified,
                 will combine any potential combination to compare. Defaults to None.
```

### Comparing `omnisafe-0.4.0/omnisafe/common/lagrange.py` & `omnisafe-0.5.0b0/omnisafe/common/lagrange.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -73,15 +73,15 @@
         lagrangian_upper_bound: float | None = None,
     ) -> None:
         """Initialize an instance of :class:`Lagrange`."""
         self.cost_limit: float = cost_limit
         self.lambda_lr: float = lambda_lr
         self.lagrangian_upper_bound: float | None = lagrangian_upper_bound
 
-        init_value = max(lagrangian_multiplier_init, 1e-5)
+        init_value = max(lagrangian_multiplier_init, 0.0)
         self.lagrangian_multiplier: torch.nn.Parameter = torch.nn.Parameter(
             torch.as_tensor(init_value),
             requires_grad=True,
         )
         self.lambda_range_projection: torch.nn.ReLU = torch.nn.ReLU()
         # fetch optimizer from PyTorch optimizer package
         assert hasattr(
@@ -114,18 +114,18 @@
     def update_lagrange_multiplier(self, Jc: float) -> None:
         r"""Update Lagrange multiplier (lambda).
 
         We update the Lagrange multiplier by minimizing the penalty loss, which is defined as:
 
         .. math::
 
-            \lambda ^{'} = \lambda + \eta \cdot (J_c - J_c^*)
+            \lambda ^{'} = \lambda + \eta \cdot (J_C - J_C^*)
 
         where :math:`\lambda` is the Lagrange multiplier, :math:`\eta` is the learning rate,
-        :math:`J_c` is the mean episode cost, and :math:`J_c^*` is the cost limit.
+        :math:`J_C` is the mean episode cost, and :math:`J_C^*` is the cost limit.
 
         Args:
             Jc (float): mean episode cost.
         """
         self.lambda_optimizer.zero_grad()
         lambda_loss = self.compute_lambda_loss(Jc)
         lambda_loss.backward()
```

### Comparing `omnisafe-0.4.0/omnisafe/common/logger.py` & `omnisafe-0.5.0b0/omnisafe/common/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 from __future__ import annotations
 
 import atexit
 import csv
 import os
 import time
 from collections import deque
-from typing import Any, Deque, TextIO
+from typing import Any, TextIO
 
 import numpy as np
 import torch
 import wandb
-from rich import print  # pylint: disable=redefined-builtin
-from rich.console import Console
-from rich.table import Table
+from rich import print  # pylint: disable=redefined-builtin,wrong-import-order
+from rich.console import Console  # pylint: disable=wrong-import-order
+from rich.table import Table  # pylint: disable=wrong-import-order
 
 from omnisafe.utils.config import Config
 from omnisafe.utils.distributed import dist_statistics_scalar, get_rank
 
 
 # As of torch v1.9.0, torch.utils.tensorboard has a bug that is exposed by setuptools 59.6.0.  The
 # bug is that it attempts to import distutils then access distutils.version without actually
@@ -113,15 +113,15 @@
             atexit.register(self._output_file.close)
             self.log(f'Logging data to {self._output_file.name}', 'cyan', bold=True)
             self._csv_writer = csv.writer(self._output_file)
 
         self._epoch: int = 0
         self._first_row: bool = True
         self._what_to_save: dict[str, Any] | None = None
-        self._data: dict[str, Deque[int | float] | list[int | float]] = {}
+        self._data: dict[str, deque[int | float] | list[int | float]] = {}
         self._headers_windows: dict[str, int | None] = {}
         self._headers_minmax: dict[str, bool] = {}
         self._headers_delta: dict[str, bool] = {}
         self._current_row: dict[str, int | float] = {}
 
         if config is not None:
             self.save_config(config)
@@ -243,27 +243,29 @@
             self._headers_windows[key] = window_length
         else:
             self._data[key] = []
             self._headers_windows[key] = None
 
     def store(
         self,
-        data: dict[str, int | float | np.ndarray | torch.Tensor] | None = None,
+        data: dict[str, Any] | None = None,
         /,
-        **kwargs: int | float | np.ndarray | torch.Tensor,
+        **kwargs: Any | float | np.ndarray | torch.Tensor,
     ) -> None:
         """Store the data to the logger.
 
         .. note ::
             The data stored in ``data`` will be updated by ``kwargs``.
 
         Args:
             data (dict[str, int | float | np.ndarray | torch.Tensor] or None, optional): The data to
                 be stored. Defaults to None.
-            **kwargs (int, float, np.ndarray, or torch.Tensor): The data to be stored.
+
+        Keyword Args:
+            kwargs (int, float, np.ndarray, or torch.Tensor): The data to be stored.
         """
         if data is not None:
             kwargs.update(data)
         for key, val in kwargs.items():
             assert key in self._current_row, f'Key {key} has not been registered'
             if isinstance(val, (int, float)):
                 self._data[key].append(val)
@@ -275,19 +277,18 @@
                 raise ValueError(f'Unsupported type {type(val)}')
 
     def dump_tabular(self) -> None:
         """Dump the tabular data to the console and the file.
 
         The dumped data will be separated by the following steps:
 
-        .. hint::
-            - If the key is registered with window_length, the data will be averaged in the window.
-            - Write the data to the csv file.
-            - Write the data to the tensorboard.
-            - Update the progress logger.
+        - If the key is registered with window_length, the data will be averaged in the window.
+        - Write the data to the csv file.
+        - Write the data to the tensorboard.
+        - Update the progress logger.
         """
         self._update_current_row()
         table = Table('Metrics', 'Value')
         if self._maste_proc:
             self._epoch += 1
             key_lens = list(map(len, self._current_row.keys()))
             max_key_len = max(15, *key_lens)
```

### Comparing `omnisafe-0.4.0/omnisafe/common/normalizer.py` & `omnisafe-0.5.0b0/omnisafe/common/normalizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -25,15 +25,15 @@
 
 class Normalizer(nn.Module):
     """Calculate normalized raw_data from running mean and std.
 
     References:
         - Title: Updating Formulae and a Pairwise Algorithm for Computing Sample Variances
         - Author: Tony F. Chan, Gene H. Golub, Randall J. LeVeque
-        - URL: http://i.stanford.edu/pub/cstr/reports/cs/tr/79/773/CS-TR-79-773.pdf
+        - URL: `Normalizer <http://i.stanford.edu/pub/cstr/reports/cs/tr/79/773/CS-TR-79-773.pdf>`_
     """
 
     _mean: torch.Tensor  # running mean
     _sumsq: torch.Tensor  # running sum of squares
     _var: torch.Tensor  # running variance
     _std: torch.Tensor  # running standard deviation
     _count: torch.Tensor  # number of samples
@@ -75,15 +75,15 @@
         """Return the std of the normalize."""
         return self._std
 
     def forward(self, data: torch.Tensor) -> torch.Tensor:
         """Normalize the data.
 
         Args:
-            data (torch.Tensor): raw data to be normalized.
+            data (torch.Tensor): The raw data to be normalized.
 
         Returns:
             The normalized data.
         """
         return self.normalize(data)
 
     def normalize(self, data: torch.Tensor) -> torch.Tensor:
```

### Comparing `omnisafe-0.4.0/omnisafe/common/pid_lagrange.py` & `omnisafe-0.5.0b0/omnisafe/common/pid_lagrange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/common/simmer_agent.py` & `omnisafe-0.5.0b0/omnisafe/common/simmer_agent.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.4.0/omnisafe/common/statistics_tools.py` & `omnisafe-0.5.0b0/omnisafe/common/statistics_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
                     smooth,
                     None,
                     None,
                     'mean',
                     save_name=save_name,
                     show_image=show_image,
                 )
-            except Exception:  # noqa # pylint: disable=broad-except
+            except Exception:  # noqa # pragma: no cover # pylint: disable=broad-except
                 print(
                     f'Cannot generate graph for {save_name[:5] + str(decompressed_img_name_cfgs)}',
                 )
                 print(Exception)
 
     def make_config_groups(
         self,
@@ -215,15 +215,16 @@
             )
             # if compare_num is specified, will combine any potential combination to compare
             parameter_values_combination = list(self.combine(parameter_values, compare_num))
         group_config = deepcopy(self.grid_config)
         # value of parameter is determined above
         group_config.pop(parameter)
         # seed is not a parameter
-        group_config.pop('seed')
+        if 'seed' in group_config:
+            group_config.pop('seed')
         if 'train_cfgs' in group_config:
             group_config['train_cfgs'].pop('device', None)
         # combine all possible combinations of other parameters
         # fix them in a single graph and only vary values of parameter which is specified by us
         for pinned_config in self.dict_permutations(group_config):
             group_config.update(pinned_config)
             for compare_value in parameter_values_combination:
```

### Comparing `omnisafe-0.4.0/omnisafe/configs/model-based/CAPPETS.yaml` & `omnisafe-0.5.0b0/omnisafe/configs/model-based/CAPPETS.yaml`

 * *Files identical despite different names*

### Comparing `omnisafe-0.4.0/omnisafe/configs/model-based/CCEPETS.yaml` & `omnisafe-0.5.0b0/omnisafe/configs/model-based/CCEPETS.yaml`

 * *Files identical despite different names*

### Comparing `omnisafe-0.4.0/omnisafe/configs/model-based/LOOP.yaml` & `omnisafe-0.5.0b0/omnisafe/configs/model-based/LOOP.yaml`

 * *Files identical despite different names*

### Comparing `omnisafe-0.4.0/omnisafe/configs/model-based/PETS.yaml` & `omnisafe-0.5.0b0/omnisafe/configs/model-based/PETS.yaml`

 * *Files identical despite different names*

### Comparing `omnisafe-0.4.0/omnisafe/configs/model-based/RCEPETS.yaml` & `omnisafe-0.5.0b0/omnisafe/configs/model-based/RCEPETS.yaml`

 * *Files identical despite different names*

### Comparing `omnisafe-0.4.0/omnisafe/configs/model-based/SafeLOOP.yaml` & `omnisafe-0.5.0b0/omnisafe/configs/model-based/SafeLOOP.yaml`

 * *Files identical despite different names*

### Comparing `omnisafe-0.4.0/omnisafe/configs/off-policy/DDPG.yaml` & `omnisafe-0.5.0b0/omnisafe/configs/on-policy/P3O.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -23,86 +23,102 @@
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
     vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
-    total_steps: 1000000
+    total_steps: 10000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    steps_per_epoch: 2000
-    # number of steps per sample
-    update_cycle: 1
+    steps_per_epoch: 20000
     # number of iterations to update the policy
-    update_iters: 1
-    # The size of replay buffer
-    size: 1000000
-    # The size of batch
-    batch_size: 256
+    update_iters: 10
+    # batch size for each iteration
+    batch_size: 64
+    # target kl divergence
+    target_kl: 0.02
+    # the coefficient of cost penalty
+    kappa: 20.0
+    # entropy coefficient
+    entropy_coef: 0.0
     # normalize reward
     reward_normalize: False
     # normalize cost
     cost_normalize: False
     # normalize observation
-    obs_normalize: False
+    obs_normalize: True
+    # early stop when kl divergence is bigger than target kl
+    kl_early_stop: True
+    # use max gradient norm
+    use_max_grad_norm: True
     # max gradient norm
-    max_grad_norm: 40
+    max_grad_norm: 40.0
     # use critic norm
-    use_critic_norm: False
+    use_critic_norm: True
     # critic norm coefficient
-    critic_norm_coeff: 0.001
-    # The soft update coefficient
-    polyak: 0.005
-    # The discount factor of GAE
+    critic_norm_coef: 0.001
+    # reward discount factor
     gamma: 0.99
-    # Actor perdorm random action before `start_learning_steps` steps
-    start_learning_steps: 25000
-    # The delay step of policy update
-    policy_delay: 1
-    # Whether to use the exploration noise
-    use_exploration_noise: True
-    # The exploration noise
-    exploration_noise: 0.1
+    # cost discount factor
+    cost_gamma: 0.99
+    # lambda for gae
+    lam: 0.95
+    # lambda for cost gae
+    lam_c: 0.95
+    # clip ratio
+    clip: 0.2
+    # cost limit
+    cost_limit: 25.0
+    # advantage estimation method, options: gae, retrace
+    adv_estimation_method: gae
+    # standardize reward advantage
+    standardized_rew_adv: True
+    # standardize cost advantage
+    standardized_cost_adv: True
+    # penalty coefficient
+    penalty_coef: 0.0
     # use cost
-    use_cost: False
+    use_cost: True
   # logger configurations
   logger_cfgs:
     # use wandb for logging
     use_wandb: False
     # wandb project name
     wandb_project: omnisafe
     # use tensorboard for logging
     use_tensorboard: True
     # save model frequency
     save_model_freq: 100
     # save logger path
     log_dir: "./runs"
     # save model path
-    window_lens: 10
+    window_lens: 100
   # model configurations
   model_cfgs:
     # weight initialization mode
     weight_initialization_mode: "kaiming_uniform"
-    # actor type
-    actor_type: mlp
+    # actor type, options: gaussian, gaussian_learning
+    actor_type: gaussian_learning
     # linear learning rate decay
-    linear_lr_decay: False
-    # Configuration of Actor network
+    linear_lr_decay: True
+    # exploration noise anneal
+    exploration_noise_anneal: False
+    # std upper bound, and lower bound
+    std_range: [0.5, 0.1]
+    # actor network configurations
     actor:
-      # Size of hidden layers
-      hidden_sizes: [256, 256]
-      # Activation function
-      activation: relu
-      # The learning rate of Actor network
+      # hidden layer sizes
+      hidden_sizes: [64, 64]
+      # activation function
+      activation: tanh
+      # out_activation: tanh
+      # learning rate
       lr: 0.0003
-    # Configuration of Critic network
     critic:
-      # The number of critic networks
-      num_critics: 1
-      # Size of hidden layers
-      hidden_sizes: [256, 256]
-      # Activation function
-      activation: relu
-      # The learning rate of Critic network
+      # hidden layer sizes
+      hidden_sizes: [64, 64]
+      # activation function
+      activation: tanh
+      # learning rate
       lr: 0.0003
```

### Comparing `omnisafe-0.4.0/omnisafe/configs/off-policy/DDPGLag.yaml` & `omnisafe-0.5.0b0/omnisafe/configs/on-policy/PDO.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -23,51 +23,61 @@
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
     vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
-    total_steps: 1000000
+    total_steps: 10000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    steps_per_epoch: 2000
-    # number of steps per sample
-    update_cycle: 1
+    steps_per_epoch: 20000
     # number of iterations to update the policy
-    update_iters: 1
-    # The size of replay buffer
-    size: 1000000
-    # The size of batch
-    batch_size: 256
+    update_iters: 40
+    # batch size for each iteration
+    batch_size: 64
+    # target kl divergence
+    target_kl: 0.02
+    # entropy coefficient
+    entropy_coef: 0.0
     # normalize reward
-    reward_normalize: False
+    reward_normalize: True
     # normalize cost
-    cost_normalize: False
+    cost_normalize: True
     # normalize observation
-    obs_normalize: False
+    obs_normalize: True
+    # early stop when kl divergence is bigger than target kl
+    kl_early_stop: True
+    # use max gradient norm
+    use_max_grad_norm: True
     # max gradient norm
-    max_grad_norm: 40
+    max_grad_norm: 40.0
     # use critic norm
-    use_critic_norm: False
+    use_critic_norm: True
     # critic norm coefficient
-    critic_norm_coeff: 0.001
-    # The soft update coefficient
-    polyak: 0.005
-    # The discount factor of GAE
+    critic_norm_coef: 0.001
+    # reward discount factor
     gamma: 0.99
-    # Actor perdorm random action before `start_learning_steps` steps
-    start_learning_steps: 25000
-    # The delay step of policy update
-    policy_delay: 1
-    # Whether to use the exploration noise
-    use_exploration_noise: True
-    # The exploration noise
-    exploration_noise: 0.1
+    # cost discount factor
+    cost_gamma: 0.99
+    # lambda for gae
+    lam: 0.95
+    # lambda for cost gae
+    lam_c: 0.95
+    # clip ratio
+    clip: 0.2
+    # advantage estimation method, options: gae, retrace
+    adv_estimation_method: gae
+    # standardize reward advantage
+    standardized_rew_adv: True
+    # standardize cost advantage
+    standardized_cost_adv: True
+    # penalty coefficient
+    penalty_coef: 0.0
     # use cost
     use_cost: True
   # logger configurations
   logger_cfgs:
     # use wandb for logging
     use_wandb: False
     # wandb project name
@@ -75,44 +85,45 @@
     # use tensorboard for logging
     use_tensorboard: True
     # save model frequency
     save_model_freq: 100
     # save logger path
     log_dir: "./runs"
     # save model path
-    window_lens: 10
+    window_lens: 100
   # model configurations
   model_cfgs:
     # weight initialization mode
     weight_initialization_mode: "kaiming_uniform"
-    # actor type
-    actor_type: mlp
+    # actor type, options: gaussian, gaussian_learning
+    actor_type: gaussian_learning
     # linear learning rate decay
-    linear_lr_decay: False
-    # Configuration of Actor network
+    linear_lr_decay: True
+    # exploration noise anneal
+    exploration_noise_anneal: False
+    # std upper bound, and lower bound
+    std_range: [0.5, 0.1]
+    # actor network configurations
     actor:
-      # Size of hidden layers
-      hidden_sizes: [256, 256]
-      # Activation function
-      activation: relu
-      # The learning rate of Actor network
+      # hidden layer sizes
+      hidden_sizes: [64, 64]
+      # activation function
+      activation: tanh
+      # out_activation: tanh
+      # learning rate
       lr: 0.0003
-    # Configuration of Critic network
     critic:
-      # The number of critic networks
-      num_critics: 1
-      # Size of hidden layers
-      hidden_sizes: [256, 256]
-      # Activation function
-      activation: relu
-      # The learning rate of Critic network
+      # hidden layer sizes
+      hidden_sizes: [64, 64]
+      # activation function
+      activation: tanh
+      # learning rate
       lr: 0.0003
-  # lagrangian configurations
   lagrange_cfgs:
     # Tolerance of constraint violation
     cost_limit: 25.0
     # Initial value of lagrangian multiplier
     lagrangian_multiplier_init: 0.001
     # Learning rate of lagrangian multiplier
-    lambda_lr: 0.001
+    lambda_lr: 0.035
     # Type of lagrangian optimizer
     lambda_optimizer: "Adam"
```

### Comparing `omnisafe-0.4.0/omnisafe/configs/off-policy/SAC.yaml` & `omnisafe-0.5.0b0/omnisafe/configs/on-policy/PolicyGradient.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -23,59 +23,59 @@
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
     vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
-    total_steps: 1000000
+    total_steps: 10000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    steps_per_epoch: 2000
-    # number of steps per sample
-    update_cycle: 1
+    steps_per_epoch: 20000
     # number of iterations to update the policy
-    update_iters: 1
-    # The size of replay buffer
-    size: 1000000
-    # The size of batch
-    batch_size: 256
+    update_iters: 10
+    # batch size for each iteration
+    batch_size: 64
+    # target kl divergence
+    target_kl: 0.02
+    # entropy coefficient
+    entropy_coef: 0.0
     # normalize reward
     reward_normalize: False
     # normalize cost
     cost_normalize: False
     # normalize observation
-    obs_normalize: False
+    obs_normalize: True
+    # early stop when kl divergence is bigger than target kl
+    kl_early_stop: True
+    # use max gradient norm
+    use_max_grad_norm: True
     # max gradient norm
-    max_grad_norm: 40
+    max_grad_norm: 40.0
     # use critic norm
-    use_critic_norm: False
+    use_critic_norm: True
     # critic norm coefficient
-    critic_norm_coeff: 0.001
-    # The soft update coefficient
-    polyak: 0.005
-    # The discount factor of GAE
+    critic_norm_coef: 0.001
+    # reward discount factor
     gamma: 0.99
-    # Actor perdorm random action before `start_learning_steps` steps
-    start_learning_steps: 10000
-    # The delay step of policy update
-    policy_delay: 2
-    # Whether to use the exploration noise
-    use_exploration_noise: False
-    # The exploration noise
-    exploration_noise: 0.1
-    # The policy noise
-    policy_noise: 0.2
-    # policy_noise_clip
-    policy_noise_clip: 0.5
-    # The value of alpha
-    alpha: 0.01
-    # Whether to use auto alpha
-    auto_alpha: False
+    # cost discount factor
+    cost_gamma: 0.99
+    # lambda for gae
+    lam: 0.95
+    # lambda for cost gae
+    lam_c: 0.95
+    # advantage estimation method, options: gae, retrace
+    adv_estimation_method: gae
+    # standardize reward advantage
+    standardized_rew_adv: True
+    # standardize cost advantage
+    standardized_cost_adv: True
+    # penalty coefficient
+    penalty_coef: 0.0
     # use cost
     use_cost: False
   # logger configurations
   logger_cfgs:
     # use wandb for logging
     use_wandb: False
     # wandb project name
@@ -83,34 +83,36 @@
     # use tensorboard for logging
     use_tensorboard: True
     # save model frequency
     save_model_freq: 100
     # save logger path
     log_dir: "./runs"
     # save model path
-    window_lens: 10
+    window_lens: 100
   # model configurations
   model_cfgs:
     # weight initialization mode
     weight_initialization_mode: "kaiming_uniform"
-    # actor type
-    actor_type: gaussian_sac
+    # actor type, options: gaussian, gaussian_learning
+    actor_type: gaussian_learning
     # linear learning rate decay
-    linear_lr_decay: False
-    # Configuration of Actor network
+    linear_lr_decay: True
+    # exploration noise anneal
+    exploration_noise_anneal: False
+    # std upper bound, and lower bound
+    std_range: [0.5, 0.1]
+    # actor network configurations
     actor:
-      # Size of hidden layers
-      hidden_sizes: [256, 256]
-      # Activation function
-      activation: relu
-      # The learning rate of Actor network
+      # hidden layer sizes
+      hidden_sizes: [64, 64]
+      # activation function
+      activation: tanh
+      # out_activation: tanh
+      # learning rate
       lr: 0.0003
-    # Configuration of Critic network
     critic:
-      # The number of critic networks
-      num_critics: 2
-      # Size of hidden layers
-      hidden_sizes: [256, 256]
-      # Activation function
-      activation: relu
-      # The learning rate of Critic network
+      # hidden layer sizes
+      hidden_sizes: [64, 64]
+      # activation function
+      activation: tanh
+      # learning rate
       lr: 0.0003
```

### Comparing `omnisafe-0.4.0/omnisafe/configs/off-policy/SACLag.yaml` & `omnisafe-0.5.0b0/omnisafe/configs/on-policy/CUP.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -23,59 +23,61 @@
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
     vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
-    total_steps: 1000000
+    total_steps: 10000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    steps_per_epoch: 2000
-    # number of steps per sample
-    update_cycle: 1
+    steps_per_epoch: 20000
     # number of iterations to update the policy
-    update_iters: 1
-    # The size of replay buffer
-    size: 1000000
-    # The size of batch
-    batch_size: 256
+    update_iters: 40
+    # batch size for each iteration
+    batch_size: 64
+    # target kl divergence
+    target_kl: 0.01
+    # entropy coefficient
+    entropy_coef: 0.0
     # normalize reward
     reward_normalize: False
     # normalize cost
     cost_normalize: False
     # normalize observation
-    obs_normalize: False
+    obs_normalize: True
+    # early stop when kl divergence is bigger than target kl
+    kl_early_stop: True
+    # use max gradient norm
+    use_max_grad_norm: True
     # max gradient norm
-    max_grad_norm: 40
+    max_grad_norm: 40.0
     # use critic norm
-    use_critic_norm: False
+    use_critic_norm: True
     # critic norm coefficient
-    critic_norm_coeff: 0.001
-    # The soft update coefficient
-    polyak: 0.005
-    # The discount factor of GAE
+    critic_norm_coef: 0.001
+    # reward discount factor
     gamma: 0.99
-    # Actor perdorm random action before `start_learning_steps` steps
-    start_learning_steps: 10000
-    # The delay step of policy update
-    policy_delay: 2
-    # Whether to use the exploration noise
-    use_exploration_noise: False
-    # The exploration noise
-    exploration_noise: 0.1
-    # The policy noise
-    policy_noise: 0.2
-    # policy_noise_clip
-    policy_noise_clip: 0.5
-    # The value of alpha
-    alpha: 0.2
-    # Whether to use auto alpha
-    auto_alpha: False
+    # cost discount factor
+    cost_gamma: 0.99
+    # lambda for gae
+    lam: 0.95
+    # lambda for cost gae
+    lam_c: 0.95
+    # clip ratio
+    clip: 0.2
+    # advantage estimation method, options: gae, retrace
+    adv_estimation_method: gae
+    # standardize reward advantage
+    standardized_rew_adv: True
+    # standardize cost advantage
+    standardized_cost_adv: True
+    # penalty coefficient
+    penalty_coef: 0.0
     # use cost
     use_cost: True
   # logger configurations
   logger_cfgs:
     # use wandb for logging
     use_wandb: False
     # wandb project name
@@ -83,44 +85,48 @@
     # use tensorboard for logging
     use_tensorboard: True
     # save model frequency
     save_model_freq: 100
     # save logger path
     log_dir: "./runs"
     # save model path
-    window_lens: 10
+    window_lens: 100
   # model configurations
   model_cfgs:
     # weight initialization mode
     weight_initialization_mode: "kaiming_uniform"
-    # actor type
-    actor_type: gaussian_sac
+    # actor type, options: gaussian, gaussian_learning
+    actor_type: gaussian_learning
     # linear learning rate decay
-    linear_lr_decay: False
-    # Configuration of Actor network
+    linear_lr_decay: True
+    # exploration noise anneal
+    exploration_noise_anneal: False
+    # std upper bound, and lower bound
+    std_range: [0.5, 0.1]
+    # actor network configurations
     actor:
-      # Size of hidden layers
-      hidden_sizes: [256, 256]
-      # Activation function
-      activation: relu
-      # The learning rate of Actor network
+      # hidden layer sizes
+      hidden_sizes: [64, 64]
+      # activation function
+      activation: tanh
+      # out_activation: tanh
+      # learning rate
       lr: 0.0003
-    # Configuration of Critic network
     critic:
-      # The number of critic networks
-      num_critics: 2
-      # Size of hidden layers
-      hidden_sizes: [256, 256]
-      # Activation function
-      activation: relu
-      # The learning rate of Critic network
+      # hidden layer sizes
+      hidden_sizes: [64, 64]
+      # activation function
+      activation: tanh
+      # learning rate
       lr: 0.0003
   # lagrangian configurations
   lagrange_cfgs:
     # Tolerance of constraint violation
     cost_limit: 25.0
     # Initial value of lagrangian multiplier
     lagrangian_multiplier_init: 0.001
     # Learning rate of lagrangian multiplier
-    lambda_lr: 0.001
+    lambda_lr: 0.035
     # Type of lagrangian optimizer
     lambda_optimizer: "Adam"
+    # The upper bound of lagrange multiplier
+    lagrangian_upper_bound: 2.0
```

### Comparing `omnisafe-0.4.0/omnisafe/configs/off-policy/TD3.yaml` & `omnisafe-0.5.0b0/omnisafe/configs/on-policy/PPOEarlyTerminated.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -23,90 +23,100 @@
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
     vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
-    total_steps: 1000000
+    total_steps: 10000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    steps_per_epoch: 2000
-    # number of steps per sample
-    update_cycle: 1
+    steps_per_epoch: 20000
     # number of iterations to update the policy
-    update_iters: 1
-    # The size of replay buffer
-    size: 1000000
-    # The size of batch
-    batch_size: 256
+    update_iters: 40
+    # batch size for each iteration
+    batch_size: 64
+    # target kl divergence
+    target_kl: 0.02
+    # entropy coefficient
+    entropy_coef: 0.0
     # normalize reward
     reward_normalize: False
     # normalize cost
     cost_normalize: False
     # normalize observation
-    obs_normalize: False
+    obs_normalize: True
+    # early stop when kl divergence is bigger than target kl
+    kl_early_stop: True
+    # use max gradient norm
+    use_max_grad_norm: True
     # max gradient norm
-    max_grad_norm: 40
+    max_grad_norm: 40.0
     # use critic norm
-    use_critic_norm: False
+    use_critic_norm: True
     # critic norm coefficient
-    critic_norm_coeff: 0.001
-    # The soft update coefficient
-    polyak: 0.005
-    # The discount factor of GAE
+    critic_norm_coef: 0.001
+    # reward discount factor
     gamma: 0.99
-    # Actor perdorm random action before `start_learning_steps` steps
-    start_learning_steps: 25000
-    # The delay step of policy update
-    policy_delay: 2
-    # Whether to use the exploration noise
-    use_exploration_noise: True
-    # The exploration noise
-    exploration_noise: 0.1
-    # The policy noise
-    policy_noise: 0.2
-    # policy_noise_clip
-    policy_noise_clip: 0.5
+    # cost discount factor
+    cost_gamma: 0.99
+    # lambda for gae
+    lam: 0.95
+    # lambda for cost gae
+    lam_c: 0.95
+    # clip ratio
+    clip: 0.2
+    # advantage estimation method, options: gae, retrace
+    adv_estimation_method: gae
+    # standardize reward advantage
+    standardized_rew_adv: True
+    # standardize cost advantage
+    standardized_cost_adv: True
+    # penalty coefficient
+    penalty_coef: 0.0
     # use cost
     use_cost: False
+    # Tolerance of constraint violation
+    cost_limit: 25.0
   # logger configurations
   logger_cfgs:
     # use wandb for logging
     use_wandb: False
     # wandb project name
     wandb_project: omnisafe
     # use tensorboard for logging
     use_tensorboard: True
     # save model frequency
     save_model_freq: 100
     # save logger path
     log_dir: "./runs"
     # save model path
-    window_lens: 10
+    window_lens: 100
   # model configurations
   model_cfgs:
     # weight initialization mode
     weight_initialization_mode: "kaiming_uniform"
-    # actor type
-    actor_type: mlp
+    # actor type, options: gaussian, gaussian_learning
+    actor_type: gaussian_learning
     # linear learning rate decay
-    linear_lr_decay: False
-    # Configuration of Actor network
+    linear_lr_decay: True
+    # exploration noise anneal
+    exploration_noise_anneal: False
+    # std upper bound, and lower bound
+    std_range: [0.5, 0.1]
+    # actor network configurations
     actor:
-      # Size of hidden layers
-      hidden_sizes: [256, 256]
-      # Activation function
-      activation: relu
-      # The learning rate of Actor network
+      # hidden layer sizes
+      hidden_sizes: [64, 64]
+      # activation function
+      activation: tanh
+      # out_activation: tanh
+      # learning rate
       lr: 0.0003
-    # Configuration of Critic network
     critic:
-      # The number of critic networks
-      num_critics: 2
-      # Size of hidden layers
-      hidden_sizes: [256, 256]
-      # Activation function
-      activation: relu
-      # The learning rate of Critic network
+      # hidden layer sizes
+      hidden_sizes: [64, 64]
+      # activation function
+      activation: tanh
+      # learning rate
       lr: 0.0003
```

### Comparing `omnisafe-0.4.0/omnisafe/configs/off-policy/TD3Lag.yaml` & `omnisafe-0.5.0b0/omnisafe/configs/offline/COptiDICE.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -18,105 +18,87 @@
   seed: 0
   # training configurations
   train_cfgs:
     # device to use for training, options: cpu, cuda, cuda:0, cuda:0,1, etc.
     device: cpu
     # number of threads for torch
     torch_threads: 16
-    # number of vectorized environments
-    vector_env_nums: 1
-    # number of parallel agent, similar to a3c
-    parallel: 1
     # total number of steps to train
     total_steps: 1000000
+    # dataset name
+    dataset: SafetyPointCircle1-v0_mixed_0.5
+    # evaluate_epoisodes
+    evaluate_epoisodes: 10
+    # parallel, offline only supports 1
+    parallel: 1
+    # vector_env_nums, offline only supports 1
+    vector_env_nums: 1
   # algorithm configurations
   algo_cfgs:
-    # number of steps to update the policy
-    steps_per_epoch: 2000
-    # number of steps per sample
-    update_cycle: 1
-    # number of iterations to update the policy
-    update_iters: 1
-    # The size of replay buffer
-    size: 1000000
-    # The size of batch
+    # gamma used in RL
+    gamma: 0.99
+    # batch size
     batch_size: 256
-    # normalize reward
-    reward_normalize: False
-    # normalize cost
-    cost_normalize: False
-    # normalize observation
-    obs_normalize: False
-    # max gradient norm
-    max_grad_norm: 40
-    # use critic norm
-    use_critic_norm: False
-    # critic norm coefficient
-    critic_norm_coeff: 0.001
+    # step per epoch, algo will log and eval every epoch
+    steps_per_epoch: 1000
+    # dicvrgence type, optional: chisquare, kl, softchi
+    fn_type: softchi
+    # Regularizer on Df(d|dD).
+    alpha: 0.0008
+    # Adjusts the degree of overestimation of cost value.
+    cost_ub_eps: 0.05
+    # Tolerance of constraint violation
+    cost_limit: 0.06
     # The soft update coefficient
     polyak: 0.005
-    # The discount factor of GAE
-    gamma: 0.99
-    # Actor perdorm random action before `start_learning_steps` steps
-    start_learning_steps: 25000
-    # The delay step of policy update
-    policy_delay: 2
-    # Whether to use the exploration noise
-    use_exploration_noise: True
-    # The exploration noise
-    exploration_noise: 0.1
-    # The policy noise
-    policy_noise: 0.2
-    # policy_noise_clip
-    policy_noise_clip: 0.5
-    # use cost
-    use_cost: True
   # logger configurations
   logger_cfgs:
     # use wandb for logging
     use_wandb: False
     # wandb project name
     wandb_project: omnisafe
     # use tensorboard for logging
     use_tensorboard: True
     # save model frequency
     save_model_freq: 100
     # save logger path
     log_dir: "./runs"
-    # save model path
-    window_lens: 10
   # model configurations
   model_cfgs:
-    # weight initialization mode
+    # The mode to initiate the weight of network, choosing from "kaiming_uniform", "xavier_normal", "glorot" and "orthogonal".
     weight_initialization_mode: "kaiming_uniform"
-    # actor type
-    actor_type: mlp
-    # linear learning rate decay
-    linear_lr_decay: False
     # Configuration of Actor network
     actor:
       # Size of hidden layers
-      hidden_sizes: [256, 256]
-      # Activation function
+      hidden_sizes: [256, 256, 256]
+      # Type of activation function, choosing from "tanh", "relu", "sigmoid", "identity", "softplus"
       activation: relu
-      # The learning rate of Actor network
-      lr: 0.0003
-    # Configuration of Critic network
-    critic:
-      # The number of critic networks
-      num_critics: 2
+      # Learning rate of model
+      lr: 0.003
+    # Configuration of Nu network
+    nu:
       # Size of hidden layers
-      hidden_sizes: [256, 256]
-      # Activation function
+      hidden_sizes: [256, 256, 256]
+      # Type of activation function, choosing from "tanh", "relu", "sigmoid", "identity", "softplus"
       activation: relu
-      # The learning rate of Critic network
-      lr: 0.0003
-  # lagrangian configurations
-  lagrange_cfgs:
-    # Tolerance of constraint violation
-    cost_limit: 25.0
-    # Initial value of lagrangian multiplier
-    lagrangian_multiplier_init: 0.001
-    # Learning rate of lagrangian multiplier
-    lambda_lr: 0.001
-    # Type of lagrangian optimizer
-    lambda_optimizer: "Adam"
+      # Learning rate of model
+      lr: 0.003
+    # Configuration of Chi network
+    chi:
+      # Size of hidden layers
+      hidden_sizes: [256, 256, 256]
+      # Type of activation function, choosing from "tanh", "relu", "sigmoid", "identity", "softplus"
+      activation: relu
+      # Learning rate of model
+      lr: 0.003
+    # Configuration of parameters lamb
+    lamb:
+      # init value
+      init: 0
+      # Learning rate of model
+      lr: 0.035
+    # Configuration of parameters lamb
+    tau:
+      # init value
+      init: 1
+      # Learning rate of model
+      lr: 0.003
```

### Comparing `omnisafe-0.4.0/omnisafe/configs/on-policy/CPO.yaml` & `omnisafe-0.5.0b0/omnisafe/configs/on-policy/CPO.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -19,35 +19,35 @@
   # training configurations
   train_cfgs:
     # device to use for training, options: cpu, cuda, cuda:0, cuda:0,1, etc.
     device: cpu
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
-    vector_env_nums: 2
+    vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
-    total_steps: 1024000
+    total_steps: 10000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    steps_per_epoch: 2048
+    steps_per_epoch: 20000
     # number of iterations to update the policy
     update_iters: 10
     # batch size for each iteration
     batch_size: 128
     # target kl divergence
     target_kl: 0.01
     # entropy coefficient
     entropy_coef: 0.0
     # normalize reward
-    reward_normalize: True
+    reward_normalize: False
     # normalize cost
-    cost_normalize: True
+    cost_normalize: False
     # normalize observation
     obs_normalize: True
     # early stop when kl divergence is bigger than target kl
     kl_early_stop: False
     # use max gradient norm
     use_max_grad_norm: True
     # max gradient norm
@@ -122,27 +122,7 @@
     critic:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # learning rate
       lr: 0.001
-
-SafetyHopperVelocity-v1:
-  # algorithm configurations
-  algo_cfgs:
-    # normalize reward
-    reward_normalize: False
-    # normalize cost
-    cost_normalize: True
-    # normalize observation
-    obs_normalize: True
-
-SafetyWalker2dVelocity-v1:
-  # algorithm configurations
-  algo_cfgs:
-    # normalize reward
-    reward_normalize: False
-    # normalize cost
-    cost_normalize: True
-    # normalize observation
-    obs_normalize: True
```

### Comparing `omnisafe-0.4.0/omnisafe/configs/on-policy/CPPOPID.yaml` & `omnisafe-0.5.0b0/omnisafe/configs/on-policy/CPPOPID.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -19,23 +19,23 @@
   # training configurations
   train_cfgs:
     # device to use for training, options: cpu, cuda, cuda:0, cuda:0,1, etc.
     device: cpu
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
-    vector_env_nums: 2
+    vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
-    total_steps: 1024000
+    total_steps: 10000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    steps_per_epoch: 2048
+    steps_per_epoch: 20000
     # number of iterations to update the policy
     update_iters: 40
     # batch size for each iteration
     batch_size: 64
     # target kl divergence
     target_kl: 0.02
     # entropy coefficient
```

### Comparing `omnisafe-0.4.0/omnisafe/configs/on-policy/CUP.yaml` & `omnisafe-0.5.0b0/omnisafe/configs/on-policy/PPOLag.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -23,25 +23,25 @@
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
     vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
-    total_steps: 1024000
+    total_steps: 10000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    steps_per_epoch: 2048
+    steps_per_epoch: 20000
     # number of iterations to update the policy
     update_iters: 40
     # batch size for each iteration
     batch_size: 64
     # target kl divergence
-    target_kl: 0.01
+    target_kl: 0.02
     # entropy coefficient
     entropy_coef: 0.0
     # normalize reward
     reward_normalize: False
     # normalize cost
     cost_normalize: False
     # normalize observation
@@ -124,9 +124,7 @@
     cost_limit: 25.0
     # Initial value of lagrangian multiplier
     lagrangian_multiplier_init: 0.001
     # Learning rate of lagrangian multiplier
     lambda_lr: 0.035
     # Type of lagrangian optimizer
     lambda_optimizer: "Adam"
-    # The upper bound of lagrange multiplier
-    lagrangian_upper_bound: 2.0
```

### Comparing `omnisafe-0.4.0/omnisafe/configs/on-policy/FOCOPS.yaml` & `omnisafe-0.5.0b0/omnisafe/configs/on-policy/FOCOPS.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -23,19 +23,19 @@
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
     vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
-    total_steps: 1024000
+    total_steps: 10000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    steps_per_epoch: 2048
+    steps_per_epoch: 20000
     # number of iterations to update the policy
     update_iters: 40
     # batch size for each iteration
     batch_size: 64
     # target kl divergence
     target_kl: 0.02
     # entropy coefficient
```

### Comparing `omnisafe-0.4.0/omnisafe/configs/on-policy/IPO.yaml` & `omnisafe-0.5.0b0/omnisafe/configs/on-policy/IPO.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -19,23 +19,23 @@
   # training configurations
   train_cfgs:
     # device to use for training, options: cpu, cuda, cuda:0, cuda:0,1, etc.
     device: cpu
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
-    vector_env_nums: 2
+    vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
-    total_steps: 1024000
+    total_steps: 10000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    steps_per_epoch: 2048
+    steps_per_epoch: 20000
     # number of iterations to update the policy
     update_iters: 10
     # batch size for each iteration
     batch_size: 64
     # target kl divergence
     target_kl: 0.02
     # entropy coefficient
```

### Comparing `omnisafe-0.4.0/omnisafe/configs/on-policy/NaturalPG.yaml` & `omnisafe-0.5.0b0/omnisafe/configs/on-policy/NaturalPG.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -19,23 +19,23 @@
   # training configurations
   train_cfgs:
     # device to use for training, options: cpu, cuda, cuda:0, cuda:0,1, etc.
     device: cpu
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
-    vector_env_nums: 2
+    vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
-    total_steps: 1024000
+    total_steps: 10000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    steps_per_epoch: 2048
+    steps_per_epoch: 20000
     # number of iterations to update the policy
     update_iters: 10
     # batch size for each iteration
     batch_size: 128
     # target kl divergence
     target_kl: 0.01
     # entropy coefficient
```

### Comparing `omnisafe-0.4.0/omnisafe/configs/on-policy/OnCRPO.yaml` & `omnisafe-0.5.0b0/omnisafe/configs/on-policy/OnCRPO.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -19,23 +19,23 @@
   # training configurations
   train_cfgs:
     # device to use for training, options: cpu, cuda, cuda:0, cuda:0,1, etc.
     device: cpu
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
-    vector_env_nums: 2
+    vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
-    total_steps: 1024000
+    total_steps: 10000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    steps_per_epoch: 2048
+    steps_per_epoch: 20000
     # number of iterations to update the policy
     update_iters: 40
     # batch size for each iteration
     batch_size: 64
     # target kl divergence
     target_kl: 0.02
     # entropy coefficient
```

### Comparing `omnisafe-0.4.0/omnisafe/configs/on-policy/P3O.yaml` & `omnisafe-0.5.0b0/omnisafe/configs/on-policy/PPO.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -23,27 +23,25 @@
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
     vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
-    total_steps: 1024000
+    total_steps: 10000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    steps_per_epoch: 2048
+    steps_per_epoch: 20000
     # number of iterations to update the policy
-    update_iters: 10
+    update_iters: 40
     # batch size for each iteration
     batch_size: 64
     # target kl divergence
     target_kl: 0.02
-    # the coefficient of cost penalty
-    kappa: 20.0
     # entropy coefficient
     entropy_coef: 0.0
     # normalize reward
     reward_normalize: False
     # normalize cost
     cost_normalize: False
     # normalize observation
@@ -64,26 +62,24 @@
     cost_gamma: 0.99
     # lambda for gae
     lam: 0.95
     # lambda for cost gae
     lam_c: 0.95
     # clip ratio
     clip: 0.2
-    # cost limit
-    cost_limit: 25.0
     # advantage estimation method, options: gae, retrace
     adv_estimation_method: gae
     # standardize reward advantage
     standardized_rew_adv: True
     # standardize cost advantage
     standardized_cost_adv: True
     # penalty coefficient
     penalty_coef: 0.0
     # use cost
-    use_cost: True
+    use_cost: False
   # logger configurations
   logger_cfgs:
     # use wandb for logging
     use_wandb: False
     # wandb project name
     wandb_project: omnisafe
     # use tensorboard for logging
```

### Comparing `omnisafe-0.4.0/omnisafe/configs/on-policy/PCPO.yaml` & `omnisafe-0.5.0b0/omnisafe/configs/on-policy/PCPO.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -19,35 +19,35 @@
   # training configurations
   train_cfgs:
     # device to use for training, options: cpu, cuda, cuda:0, cuda:0,1, etc.
     device: cpu
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
-    vector_env_nums: 2
+    vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
-    total_steps: 1024000
+    total_steps: 10000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    steps_per_epoch: 2048
+    steps_per_epoch: 20000
     # number of iterations to update the policy
     update_iters: 10
     # batch size for each iteration
     batch_size: 128
     # target kl divergence
     target_kl: 0.01
     # entropy coefficient
     entropy_coef: 0.0
     # normalize reward
-    reward_normalize: True
+    reward_normalize: False
     # normalize cost
-    cost_normalize: True
+    cost_normalize: False
     # normalize observation
     obs_normalize: True
     # early stop when kl divergence is bigger than target kl
     kl_early_stop: False
     # use max gradient norm
     use_max_grad_norm: True
     # max gradient norm
@@ -122,27 +122,7 @@
     critic:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # learning rate
       lr: 0.001
-
-SafetyHopperVelocity-v1:
-  # algorithm configurations
-  algo_cfgs:
-    # normalize reward
-    reward_normalize: False
-    # normalize cost
-    cost_normalize: True
-    # normalize observation
-    obs_normalize: True
-
-SafetyWalker2dVelocity-v1:
-  # algorithm configurations
-  algo_cfgs:
-    # normalize reward
-    reward_normalize: False
-    # normalize cost
-    cost_normalize: True
-    # normalize observation
-    obs_normalize: True
```

### Comparing `omnisafe-0.4.0/omnisafe/configs/on-policy/PDO.yaml` & `omnisafe-0.5.0b0/omnisafe/configs/on-policy/RCPO.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -19,39 +19,39 @@
   # training configurations
   train_cfgs:
     # device to use for training, options: cpu, cuda, cuda:0, cuda:0,1, etc.
     device: cpu
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
-    vector_env_nums: 2
+    vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
-    total_steps: 1024000
+    total_steps: 10000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    steps_per_epoch: 2048
+    steps_per_epoch: 20000
     # number of iterations to update the policy
-    update_iters: 40
+    update_iters: 10
     # batch size for each iteration
-    batch_size: 64
+    batch_size: 128
     # target kl divergence
-    target_kl: 0.02
+    target_kl: 0.01
     # entropy coefficient
     entropy_coef: 0.0
     # normalize reward
-    reward_normalize: True
+    reward_normalize: False
     # normalize cost
-    cost_normalize: True
+    cost_normalize: False
     # normalize observation
     obs_normalize: True
     # early stop when kl divergence is bigger than target kl
-    kl_early_stop: True
+    kl_early_stop: False
     # use max gradient norm
     use_max_grad_norm: True
     # max gradient norm
     max_grad_norm: 40.0
     # use critic norm
     use_critic_norm: True
     # critic norm coefficient
@@ -60,26 +60,32 @@
     gamma: 0.99
     # cost discount factor
     cost_gamma: 0.99
     # lambda for gae
     lam: 0.95
     # lambda for cost gae
     lam_c: 0.95
-    # clip ratio
-    clip: 0.2
     # advantage estimation method, options: gae, retrace
     adv_estimation_method: gae
     # standardize reward advantage
     standardized_rew_adv: True
     # standardize cost advantage
     standardized_cost_adv: True
     # penalty coefficient
     penalty_coef: 0.0
     # use cost
     use_cost: True
+    # Damping value for conjugate gradient
+    cg_damping: 0.1
+    # Number of conjugate gradient iterations
+    cg_iters: 15
+    # Subsampled observation
+    fvp_obs: None
+    # The sub-sampling rate of the observation
+    fvp_sample_freq: 1
   # logger configurations
   logger_cfgs:
     # use wandb for logging
     use_wandb: False
     # wandb project name
     wandb_project: omnisafe
     # use tensorboard for logging
@@ -93,35 +99,36 @@
   # model configurations
   model_cfgs:
     # weight initialization mode
     weight_initialization_mode: "kaiming_uniform"
     # actor type, options: gaussian, gaussian_learning
     actor_type: gaussian_learning
     # linear learning rate decay
-    linear_lr_decay: True
+    linear_lr_decay: False
     # exploration noise anneal
     exploration_noise_anneal: False
     # std upper bound, and lower bound
     std_range: [0.5, 0.1]
     # actor network configurations
     actor:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # out_activation: tanh
       # learning rate
-      lr: 0.0003
+      lr: ~
     critic:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # learning rate
-      lr: 0.0003
+      lr: 0.001
+  # lagrangian configurations
   lagrange_cfgs:
     # Tolerance of constraint violation
     cost_limit: 25.0
     # Initial value of lagrangian multiplier
     lagrangian_multiplier_init: 0.001
     # Learning rate of lagrangian multiplier
     lambda_lr: 0.035
```

### Comparing `omnisafe-0.4.0/omnisafe/configs/on-policy/PPO.yaml` & `omnisafe-0.5.0b0/omnisafe/configs/on-policy/PPOSaute.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -23,19 +23,19 @@
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
     vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
-    total_steps: 1024000
+    total_steps: 10000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    steps_per_epoch: 2048
+    steps_per_epoch: 20000
     # number of iterations to update the policy
     update_iters: 40
     # batch size for each iteration
     batch_size: 64
     # target kl divergence
     target_kl: 0.02
     # entropy coefficient
@@ -72,14 +72,22 @@
     standardized_rew_adv: True
     # standardize cost advantage
     standardized_cost_adv: True
     # penalty coefficient
     penalty_coef: 0.0
     # use cost
     use_cost: False
+    # The safety budget, equal to the cost limit
+    safety_budget: 25.0
+    # The saute gamma
+    saute_gamma: 0.999
+    # The max length of the episode
+    max_ep_len: 1000
+    # The reward when the agent is unsafe
+    unsafe_reward: -1.0
   # logger configurations
   logger_cfgs:
     # use wandb for logging
     use_wandb: False
     # wandb project name
     wandb_project: omnisafe
     # use tensorboard for logging
```

### Comparing `omnisafe-0.4.0/omnisafe/configs/on-policy/PPOEarlyTerminated.yaml` & `omnisafe-0.5.0b0/omnisafe/configs/on-policy/TRPOEarlyTerminated.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -23,19 +23,19 @@
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
     vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
-    total_steps: 1024000
+    total_steps: 10000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    steps_per_epoch: 2048
+    steps_per_epoch: 20000
     # number of iterations to update the policy
     update_iters: 10
     # batch size for each iteration
     batch_size: 128
     # target kl divergence
     target_kl: 0.01
     # entropy coefficient
@@ -80,16 +80,14 @@
     cg_iters: 15
     # Subsampled observation
     fvp_obs: None
     # The sub-sampling rate of the observation
     fvp_sample_freq: 1
     # Tolerance of constraint violation
     cost_limit: 25.0
-    # clip ratio
-    clip: 0.2
   # logger configurations
   logger_cfgs:
     # use wandb for logging
     use_wandb: False
     # wandb project name
     wandb_project: omnisafe
     # use tensorboard for logging
@@ -116,15 +114,15 @@
     actor:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # out_activation: tanh
       # learning rate
-      lr: 0.0003
+      lr: ~
     critic:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # learning rate
-      lr: 0.0003
+      lr: 0.001
```

### Comparing `omnisafe-0.4.0/omnisafe/configs/on-policy/PPOLag.yaml` & `omnisafe-0.5.0b0/omnisafe/configs/on-policy/TRPOLag.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -23,35 +23,35 @@
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
     vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
-    total_steps: 1024000
+    total_steps: 10000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    steps_per_epoch: 2048
+    steps_per_epoch: 20000
     # number of iterations to update the policy
-    update_iters: 40
+    update_iters: 10
     # batch size for each iteration
-    batch_size: 64
+    batch_size: 128
     # target kl divergence
-    target_kl: 0.02
+    target_kl: 0.01
     # entropy coefficient
     entropy_coef: 0.0
     # normalize reward
     reward_normalize: False
     # normalize cost
     cost_normalize: False
     # normalize observation
     obs_normalize: True
     # early stop when kl divergence is bigger than target kl
-    kl_early_stop: True
+    kl_early_stop: False
     # use max gradient norm
     use_max_grad_norm: True
     # max gradient norm
     max_grad_norm: 40.0
     # use critic norm
     use_critic_norm: True
     # critic norm coefficient
@@ -60,26 +60,32 @@
     gamma: 0.99
     # cost discount factor
     cost_gamma: 0.99
     # lambda for gae
     lam: 0.95
     # lambda for cost gae
     lam_c: 0.95
-    # clip ratio
-    clip: 0.2
     # advantage estimation method, options: gae, retrace
     adv_estimation_method: gae
     # standardize reward advantage
     standardized_rew_adv: True
     # standardize cost advantage
     standardized_cost_adv: True
     # penalty coefficient
     penalty_coef: 0.0
     # use cost
     use_cost: True
+    # Damping value for conjugate gradient
+    cg_damping: 0.1
+    # Number of conjugate gradient iterations
+    cg_iters: 15
+    # Subsampled observation
+    fvp_obs: None
+    # The sub-sampling rate of the observation
+    fvp_sample_freq: 1
   # logger configurations
   logger_cfgs:
     # use wandb for logging
     use_wandb: False
     # wandb project name
     wandb_project: omnisafe
     # use tensorboard for logging
@@ -93,35 +99,35 @@
   # model configurations
   model_cfgs:
     # weight initialization mode
     weight_initialization_mode: "kaiming_uniform"
     # actor type, options: gaussian, gaussian_learning
     actor_type: gaussian_learning
     # linear learning rate decay
-    linear_lr_decay: True
+    linear_lr_decay: False
     # exploration noise anneal
     exploration_noise_anneal: False
     # std upper bound, and lower bound
     std_range: [0.5, 0.1]
     # actor network configurations
     actor:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # out_activation: tanh
       # learning rate
-      lr: 0.0003
+      lr: ~
     critic:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # learning rate
-      lr: 0.0003
+      lr: 0.001
   # lagrangian configurations
   lagrange_cfgs:
     # Tolerance of constraint violation
     cost_limit: 25.0
     # Initial value of lagrangian multiplier
     lagrangian_multiplier_init: 0.001
     # Learning rate of lagrangian multiplier
```

### Comparing `omnisafe-0.4.0/omnisafe/configs/on-policy/PPOSaute.yaml` & `omnisafe-0.5.0b0/omnisafe/configs/on-policy/TRPOSaute.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -19,23 +19,23 @@
   # training configurations
   train_cfgs:
     # device to use for training, options: cpu, cuda, cuda:0, cuda:0,1, etc.
     device: cpu
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
-    vector_env_nums: 2
+    vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
-    total_steps: 1000000
+    total_steps: 10000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    steps_per_epoch: 2000
+    steps_per_epoch: 20000
     # number of iterations to update the policy
     update_iters: 10
     # batch size for each iteration
     batch_size: 128
     # target kl divergence
     target_kl: 0.01
     # entropy coefficient
@@ -70,24 +70,30 @@
     standardized_rew_adv: True
     # standardize cost advantage
     standardized_cost_adv: True
     # penalty coefficient
     penalty_coef: 0.0
     # use cost
     use_cost: False
+    # Damping value for conjugate gradient
+    cg_damping: 0.1
+    # Number of conjugate gradient iterations
+    cg_iters: 15
+    # Subsampled observation
+    fvp_obs: None
+    # The sub-sampling rate of the observation
+    fvp_sample_freq: 1
     # The safety budget, equal to the cost limit
     safety_budget: 25.0
     # The saute gamma
     saute_gamma: 0.999
     # The max length of the episode
     max_ep_len: 1000
     # The reward when the agent is unsafe
     unsafe_reward: -1.0
-    # clip ratio
-    clip: 0.2
   # logger configurations
   logger_cfgs:
     # use wandb for logging
     use_wandb: False
     # wandb project name
     wandb_project: omnisafe
     # use tensorboard for logging
@@ -114,15 +120,15 @@
     actor:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # out_activation: tanh
       # learning rate
-      lr: 0.0003
+      lr: ~
     critic:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # learning rate
-      lr: 0.0003
+      lr: 0.001
```

### Comparing `omnisafe-0.4.0/omnisafe/configs/on-policy/PPOSimmerPID.yaml` & `omnisafe-0.5.0b0/omnisafe/configs/on-policy/PPOSimmerPID.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -19,39 +19,39 @@
   # training configurations
   train_cfgs:
     # device to use for training, options: cpu, cuda, cuda:0, cuda:0,1, etc.
     device: cpu
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
-    vector_env_nums: 2
+    vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
-    total_steps: 1000000
+    total_steps: 10000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    steps_per_epoch: 2000
+    steps_per_epoch: 20000
     # number of iterations to update the policy
-    update_iters: 10
+    update_iters: 40
     # batch size for each iteration
-    batch_size: 128
+    batch_size: 64
     # target kl divergence
-    target_kl: 0.01
+    target_kl: 0.02
     # entropy coefficient
     entropy_coef: 0.0
     # normalize reward
     reward_normalize: False
     # normalize cost
     cost_normalize: False
     # normalize observation
     obs_normalize: True
     # early stop when kl divergence is bigger than target kl
-    kl_early_stop: False
+    kl_early_stop: True
     # use max gradient norm
     use_max_grad_norm: True
     # max gradient norm
     max_grad_norm: 40.0
     # use critic norm
     use_critic_norm: True
     # critic norm coefficient
@@ -60,14 +60,16 @@
     gamma: 0.99
     # cost discount factor
     cost_gamma: 0.99
     # lambda for gae
     lam: 0.95
     # lambda for cost gae
     lam_c: 0.95
+    # clip ratio
+    clip: 0.2
     # advantage estimation method, options: gae, retrace
     adv_estimation_method: gae
     # standardize reward advantage
     standardized_rew_adv: True
     # standardize cost advantage
     standardized_cost_adv: True
     # penalty coefficient
@@ -80,16 +82,14 @@
     upper_budget: 25.0
     # The saute gamma
     saute_gamma: 0.999
     # The max length of the episode
     max_ep_len: 1000
     # The reward when the agent is unsafe
     unsafe_reward: -1.0
-    # clip ratio
-    clip: 0.2
   # logger configurations
   logger_cfgs:
     # use wandb for logging
     use_wandb: False
     # wandb project name
     wandb_project: omnisafe
     # use tensorboard for logging
@@ -103,15 +103,15 @@
   # model configurations
   model_cfgs:
     # weight initialization mode
     weight_initialization_mode: "kaiming_uniform"
     # actor type, options: gaussian, gaussian_learning
     actor_type: gaussian_learning
     # linear learning rate decay
-    linear_lr_decay: False
+    linear_lr_decay: True
     # exploration noise anneal
     exploration_noise_anneal: False
     # std upper bound, and lower bound
     std_range: [0.5, 0.1]
     # actor network configurations
     actor:
       # hidden layer sizes
```

### Comparing `omnisafe-0.4.0/omnisafe/configs/on-policy/PolicyGradient.yaml` & `omnisafe-0.5.0b0/omnisafe/configs/on-policy/TRPO.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -23,35 +23,35 @@
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
     vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
-    total_steps: 1024000
+    total_steps: 10000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    steps_per_epoch: 2048
+    steps_per_epoch: 20000
     # number of iterations to update the policy
     update_iters: 10
     # batch size for each iteration
-    batch_size: 64
+    batch_size: 128
     # target kl divergence
-    target_kl: 0.02
+    target_kl: 0.01
     # entropy coefficient
     entropy_coef: 0.0
     # normalize reward
     reward_normalize: False
     # normalize cost
     cost_normalize: False
     # normalize observation
     obs_normalize: True
     # early stop when kl divergence is bigger than target kl
-    kl_early_stop: True
+    kl_early_stop: False
     # use max gradient norm
     use_max_grad_norm: True
     # max gradient norm
     max_grad_norm: 40.0
     # use critic norm
     use_critic_norm: True
     # critic norm coefficient
@@ -70,14 +70,22 @@
     standardized_rew_adv: True
     # standardize cost advantage
     standardized_cost_adv: True
     # penalty coefficient
     penalty_coef: 0.0
     # use cost
     use_cost: False
+    # Damping value for conjugate gradient
+    cg_damping: 0.1
+    # Number of conjugate gradient iterations
+    cg_iters: 15
+    # Subsampled observation
+    fvp_obs: None
+    # The sub-sampling rate of the observation
+    fvp_sample_freq: 1
   # logger configurations
   logger_cfgs:
     # use wandb for logging
     use_wandb: False
     # wandb project name
     wandb_project: omnisafe
     # use tensorboard for logging
@@ -91,28 +99,28 @@
   # model configurations
   model_cfgs:
     # weight initialization mode
     weight_initialization_mode: "kaiming_uniform"
     # actor type, options: gaussian, gaussian_learning
     actor_type: gaussian_learning
     # linear learning rate decay
-    linear_lr_decay: True
+    linear_lr_decay: False
     # exploration noise anneal
     exploration_noise_anneal: False
     # std upper bound, and lower bound
     std_range: [0.5, 0.1]
     # actor network configurations
     actor:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # out_activation: tanh
       # learning rate
-      lr: 0.0003
+      lr: ~
     critic:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # learning rate
-      lr: 0.0003
+      lr: 0.001
```

### Comparing `omnisafe-0.4.0/omnisafe/configs/on-policy/RCPO.yaml` & `omnisafe-0.5.0b0/omnisafe/configs/on-policy/TRPOSimmerPID.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -19,35 +19,35 @@
   # training configurations
   train_cfgs:
     # device to use for training, options: cpu, cuda, cuda:0, cuda:0,1, etc.
     device: cpu
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
-    vector_env_nums: 2
+    vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
-    total_steps: 1024000
+    total_steps: 10000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    steps_per_epoch: 2048
+    steps_per_epoch: 20000
     # number of iterations to update the policy
     update_iters: 10
     # batch size for each iteration
     batch_size: 128
     # target kl divergence
     target_kl: 0.01
     # entropy coefficient
     entropy_coef: 0.0
     # normalize reward
     reward_normalize: False
     # normalize cost
-    cost_normalize: True
+    cost_normalize: False
     # normalize observation
     obs_normalize: True
     # early stop when kl divergence is bigger than target kl
     kl_early_stop: False
     # use max gradient norm
     use_max_grad_norm: True
     # max gradient norm
@@ -69,23 +69,33 @@
     # standardize reward advantage
     standardized_rew_adv: True
     # standardize cost advantage
     standardized_cost_adv: True
     # penalty coefficient
     penalty_coef: 0.0
     # use cost
-    use_cost: True
+    use_cost: False
     # Damping value for conjugate gradient
     cg_damping: 0.1
     # Number of conjugate gradient iterations
     cg_iters: 15
     # Subsampled observation
     fvp_obs: None
     # The sub-sampling rate of the observation
     fvp_sample_freq: 1
+    # The safety budget, equal to the cost limit
+    safety_budget: 25.0
+    # the upper bound of safety budget
+    upper_budget: 25.0
+    # The saute gamma
+    saute_gamma: 0.999
+    # The max length of the episode
+    max_ep_len: 1000
+    # The reward when the agent is unsafe
+    unsafe_reward: -1.0
   # logger configurations
   logger_cfgs:
     # use wandb for logging
     use_wandb: False
     # wandb project name
     wandb_project: omnisafe
     # use tensorboard for logging
@@ -120,27 +130,17 @@
     critic:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # learning rate
       lr: 0.001
-  # lagrangian configurations
-  lagrange_cfgs:
-    # Tolerance of constraint violation
-    cost_limit: 25.0
-    # Initial value of lagrangian multiplier
-    lagrangian_multiplier_init: 0.001
-    # Learning rate of lagrangian multiplier
-    lambda_lr: 0.035
-    # Type of lagrangian optimizer
-    lambda_optimizer: "Adam"
-
-SafetyHumanoidVelocity-v1:
-  # algorithm configurations
-  algo_cfgs:
-    # normalize reward
-    reward_normalize: True
-    # normalize cost
-    cost_normalize: True
-    # normalize observation
-    obs_normalize: True
+  # controller configurations
+  control_cfgs:
+    # The Kp of PID controller
+    kp: 1.0
+    # The Ki of PID controller
+    ki: 0.001
+    # The Kd of PID controller
+    kd: 0.01
+    # The polyak coefficient of the target
+    polyak: 0.995
```

### Comparing `omnisafe-0.4.0/omnisafe/configs/on-policy/TRPO.yaml` & `omnisafe-0.5.0b0/omnisafe/configs/on-policy/TRPOPID.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -19,23 +19,23 @@
   # training configurations
   train_cfgs:
     # device to use for training, options: cpu, cuda, cuda:0, cuda:0,1, etc.
     device: cpu
     # number of threads for torch
     torch_threads: 16
     # number of vectorized environments
-    vector_env_nums: 2
+    vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
-    total_steps: 1024000
+    total_steps: 10000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
-    steps_per_epoch: 2048
+    steps_per_epoch: 20000
     # number of iterations to update the policy
     update_iters: 10
     # batch size for each iteration
     batch_size: 128
     # target kl divergence
     target_kl: 0.01
     # entropy coefficient
@@ -60,24 +60,26 @@
     gamma: 0.99
     # cost discount factor
     cost_gamma: 0.99
     # lambda for gae
     lam: 0.95
     # lambda for cost gae
     lam_c: 0.95
+    # clip ratio
+    clip: 0.2
     # advantage estimation method, options: gae, retrace
     adv_estimation_method: gae
     # standardize reward advantage
     standardized_rew_adv: True
     # standardize cost advantage
     standardized_cost_adv: True
     # penalty coefficient
     penalty_coef: 0.0
     # use cost
-    use_cost: False
+    use_cost: True
     # Damping value for conjugate gradient
     cg_damping: 0.1
     # Number of conjugate gradient iterations
     cg_iters: 15
     # Subsampled observation
     fvp_obs: None
     # The sub-sampling rate of the observation
@@ -120,47 +122,31 @@
     critic:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # learning rate
       lr: 0.001
-
-SafetyAntVelocity-v1:
-  # algorithm configurations
-  algo_cfgs:
-    # normalize reward
-    reward_normalize: True
-    # normalize cost
-    cost_normalize: False
-    # normalize observation
-    obs_normalize: True
-
-SafetyHalfCheetahVelocity-v1:
-  # algorithm configurations
-  algo_cfgs:
-    # normalize reward
-    reward_normalize: True
-    # normalize cost
-    cost_normalize: False
-    # normalize observation
-    obs_normalize: False
-
-SafetyHumanoidVelocity-v1:
-  # algorithm configurations
-  algo_cfgs:
-    # normalize reward
-    reward_normalize: True
-    # normalize cost
-    cost_normalize: False
-    # normalize observation
-    obs_normalize: True
-
-SafetySwimmerVelocity-v1:
-  # algorithm configurations
-  algo_cfgs:
-    # normalize reward
-    reward_normalize: True
-    # normalize cost
-    cost_normalize: False
-    # normalize observation
-    obs_normalize: True
+  # lagrangian configurations
+  lagrange_cfgs:
+    # The Kp of PID controller
+    pid_kp: 0.1
+    # The Ki of PID controller
+    pid_ki: 0.01
+    # The Kd of PID controller
+    pid_kd: 0.01
+    #The delay of PID controller
+    pid_d_delay: 10
+    # The exponential moving average alpha of the proportional term of the PID controller.
+    pid_delta_p_ema_alpha: 0.95
+    # The exponential moving average alpha of the derivative term of the PID controller.
+    pid_delta_d_ema_alpha: 0.95
+    # Whether to normalize the sum of the cost.
+    sum_norm: True
+    # Whether to normalize the derivate of the cost.
+    diff_norm: False
+    # Tolerance of constraint violation
+    cost_limit: 25.0
+    # The max penalty coefficient
+    penalty_max: 100.0
+    # Initial value of lagrangian multiplier
+    lagrangian_multiplier_init: 0.001
```

### Comparing `omnisafe-0.4.0/omnisafe/envs/__init__.py` & `omnisafe-0.5.0b0/omnisafe/envs/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/envs/core.py` & `omnisafe-0.5.0b0/omnisafe/envs/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -151,16 +151,16 @@
         """
 
     @abstractmethod
     def render(self) -> Any:
         """Compute the render frames as specified by :attr:`render_mode` during the initialization of the environment.
 
         Returns:
-            The render frames, we recommend to use `np.ndarray` which could construct video by
-            moviepy.
+            The render frames: we recommend to use `np.ndarray`
+                which could construct video by moviepy.
         """
 
     def save(self) -> dict[str, torch.nn.Module]:
         """Save the important components of the environment.
 
         .. note::
             The saved components will be stored in the wrapped environment. If the environment is
@@ -264,16 +264,16 @@
         """
         return self._env.sample_action()
 
     def render(self) -> Any:
         """Compute the render frames as specified by :attr:`render_mode` during the initialization of the environment.
 
         Returns:
-            The render frames, we recommend to use `np.ndarray` which could construct video by
-            moviepy.
+            The render frames: we recommend to use `np.ndarray`
+                which could construct video by moviepy.
         """
         return self._env.render()
 
     def save(self) -> dict[str, torch.nn.Module]:
         """Save the important components of the environment.
 
         .. note::
@@ -380,14 +380,21 @@
 
 def make(env_id: str, class_name: str | None = None, **kwargs: Any) -> CMDP:
     """Create an environment.
 
     Args:
         env_id (str): The environment id.
         class_name (str or None): The environment class name.
-        **kwargs: the keyword arguments for the environment initialization.
+
+    Keyword Args:
+        render_mode (str, optional): The render mode ranges from 'human' to 'rgb_array' and 'rgb_array_list'.
+            Defaults to 'rgb_array'.
+        camera_name (str, optional): The camera name.
+        camera_id (int, optional): The camera id.
+        width (int, optional): The width of the rendered image. Defaults to 256.
+        height (int, optional): The height of the rendered image. Defaults to 256.
 
     Returns:
         The environment class.
     """
     env_class = ENV_REGISTRY.get_class(env_id, class_name)
     return env_class(env_id, **kwargs)
```

### Comparing `omnisafe-0.4.0/omnisafe/envs/mujoco_env.py` & `omnisafe-0.5.0b0/omnisafe/envs/mujoco_env.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -26,15 +26,14 @@
 
 
 @env_register
 class MujocoEnv(CMDP):
     """Gymnasium Mujoco environment.
 
     Attributes:
-        _support_envs (list[str]): List of supported environments.
         need_auto_reset_wrapper (bool): Whether to use auto reset wrapper.
         need_time_limit_wrapper (bool): Whether to use time limit wrapper.
     """
 
     _support_envs = [
         'Ant-v4',
         'Hopper-v4',
@@ -57,15 +56,22 @@
     ) -> None:
         """Initialize the environment.
 
         Args:
             env_id (str): Environment id.
             num_envs (int, optional): Number of environments. Defaults to 1.
             device (torch.device, optional): Device to store the data. Defaults to 'cpu'.
-            **kwargs: Other arguments.
+
+        Keyword Args:
+            render_mode (str, optional): The render mode, ranging from ``human``, ``rgb_array``, ``rgb_array_list``.
+                Defaults to ``rgb_array``.
+            camera_name (str, optional): The camera name.
+            camera_id (int, optional): The camera id.
+            width (int, optional): The width of the rendered image. Defaults to 256.
+            height (int, optional): The height of the rendered image. Defaults to 256.
         """
         super().__init__(env_id)
         self._env_id = env_id
         if num_envs == 1:
             # set healthy_reward=0.0 for removing the safety constraint in reward
             self._env = gymnasium.make(id=env_id, autoreset=False, **kwargs)
             assert isinstance(self._env.action_space, Box), 'Only support Box action space.'
@@ -81,33 +87,40 @@
 
         self._num_envs = num_envs
         self._metadata = self._env.metadata
 
     def step(
         self,
         action: torch.Tensor,
-    ) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, dict]:
+    ) -> tuple[
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        dict[str, Any],
+    ]:
         """Step the environment.
 
         .. note::
 
             OmniSafe use auto reset wrapper to reset the environment when the episode is
             terminated. So the ``obs`` will be the first observation of the next episode.
             And the true ``final_observation`` in ``info`` will be stored in the ``final_observation`` key of ``info``.
 
         Args:
             action (torch.Tensor): Action to take.
 
         Returns:
-            observation (torch.Tensor): agent's observation of the current environment.
-            reward (torch.Tensor): amount of reward returned after previous action.
-            cost (torch.Tensor): amount of cost returned after previous action.
-            terminated (torch.Tensor): whether the episode has ended.
-            truncated (torch.Tensor): whether the episode has been truncated due to a time limit.
-            info (Dict): contains auxiliary diagnostic information (helpful for debugging, and sometimes learning).
+            observation: Agent's observation of the current environment.
+            reward: Amount of reward returned after previous action.
+            cost: Amount of cost returned after previous action.
+            terminated: Whether the episode has ended.
+            truncated: Whether the episode has been truncated due to a time limit.
+            info: Auxiliary diagnostic information (helpful for debugging, and sometimes learning).
         """
         obs, reward, terminated, truncated, info = self._env.step(
             action.detach().cpu().numpy(),
         )
         obs, reward, terminated, truncated = (
             torch.as_tensor(x, dtype=torch.float32, device=self._device)
             for x in (obs, reward, terminated, truncated)
@@ -131,16 +144,16 @@
     def reset(self, seed: int | None = None) -> tuple[torch.Tensor, dict]:
         """Reset the environment.
 
         Args:
             seed (int, optional): Seed to reset the environment. Defaults to None.
 
         Returns:
-            observation (torch.Tensor): agent's observation of the current environment.
-            info (Dict): contains auxiliary diagnostic information (helpful for debugging, and sometimes learning).
+            observation: Agent's observation of the current environment.
+            info: Auxiliary diagnostic information (helpful for debugging, and sometimes learning).
         """
         obs, info = self._env.reset(seed=seed)
         return torch.as_tensor(obs, dtype=torch.float32, device=self._device), info
 
     def set_seed(self, seed: int) -> None:
         """Set the seed for the environment.
 
@@ -149,26 +162,26 @@
         """
         self.reset(seed=seed)
 
     def sample_action(self) -> torch.Tensor:
         """Sample a random action.
 
         Returns:
-            torch.Tensor: A random action.
+            A random action.
         """
         return torch.as_tensor(
             self._env.action_space.sample(),
             dtype=torch.float32,
             device=self._device,
         )
 
     def render(self) -> Any:
         """Render the environment.
 
         Returns:
-            Any: Rendered environment.
+            Rendered environment.
         """
         return self._env.render()
 
     def close(self) -> None:
         """Close the environment."""
         self._env.close()
```

### Comparing `omnisafe-0.4.0/omnisafe/envs/safety_gymnasium_env.py` & `omnisafe-0.5.0b0/omnisafe/envs/safety_gymnasium_env.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -31,15 +31,22 @@
     """Safety Gymnasium Environment.
 
     Args:
         env_id (str): Environment id.
         num_envs (int, optional): Number of environments. Defaults to 1.
         device (torch.device, optional): Device to store the data. Defaults to
             ``torch.device('cpu')``.
-        **kwargs (Any): Other arguments.
+
+    Keyword Args:
+        render_mode (str, optional): The render mode ranges from 'human' to 'rgb_array' and 'rgb_array_list'.
+            Defaults to 'rgb_array'.
+        camera_name (str, optional): The camera name.
+        camera_id (int, optional): The camera id.
+        width (int, optional): The width of the rendered image. Defaults to 256.
+        height (int, optional): The height of the rendered image. Defaults to 256.
 
     Attributes:
         need_auto_reset_wrapper (bool): Whether to use auto reset wrapper.
         need_time_limit_wrapper (bool): Whether to use time limit wrapper.
     """
 
     need_auto_reset_wrapper: bool = False
@@ -83,14 +90,16 @@
         'SafetyAntCircle2-v0',
         'SafetyHalfCheetahVelocity-v1',
         'SafetyHopperVelocity-v1',
         'SafetySwimmerVelocity-v1',
         'SafetyWalker2dVelocity-v1',
         'SafetyAntVelocity-v1',
         'SafetyHumanoidVelocity-v1',
+        'SafetyPointRun0-v0',
+        'SafetyCarRun0-v0',
     ]
 
     def __init__(
         self,
         env_id: str,
         num_envs: int = 1,
         device: torch.device = DEVICE_CPU,
@@ -205,17 +214,18 @@
         return torch.as_tensor(
             self._env.action_space.sample(),
             dtype=torch.float32,
             device=self._device,
         )
 
     def render(self) -> Any:
-        """Render the environment.
+        """Compute the render frames as specified by :attr:`render_mode` during the initialization of the environment.
 
         Returns:
-            Rendered image.
+            The render frames: we recommend to use `np.ndarray`
+                which could construct video by moviepy.
         """
         return self._env.render()
 
     def close(self) -> None:
         """Close the environment."""
         self._env.close()
```

### Comparing `omnisafe-0.4.0/omnisafe/envs/safety_gymnasium_modelbased.py` & `omnisafe-0.5.0b0/omnisafe/envs/safety_gymnasium_modelbased.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,35 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Environments in the Safety Gymnasium."""
+"""World model of the Safety Gymnasium."""
+
 
 from __future__ import annotations
 
 from typing import Any
 
 import gymnasium
 import numpy as np
 import safety_gymnasium
 import torch
 
 from omnisafe.envs.core import CMDP, env_register
+from omnisafe.typing import Box, OmnisafeSpace
 
 
 @env_register
 class SafetyGymnasiumModelBased(CMDP):  # pylint: disable=too-many-instance-attributes
     """Safety Gymnasium environment for Model-based algorithms.
 
     Attributes:
@@ -58,108 +60,120 @@
         """Initialize the environment.
 
         Args:
             env_id (str): Environment id.
             num_envs (int, optional): Number of environments. Defaults to 1.
             device (torch.device, optional): Device to store the data. Defaults to 'cpu'.
             use_lidar (bool, optional): Whether to use lidar observation. Defaults to False.
-            **kwargs: Other arguments.
+
+        Keyword Args:
+            render_mode (str, optional): The render mode, ranging from ``human``, ``rgb_array``, ``rgb_array_list``.
+                Defaults to ``rgb_array``.
+            camera_name (str, optional): The camera name.
+            camera_id (int, optional): The camera id.
+            width (int, optional): The width of the rendered image. Defaults to 256.
+            height (int, optional): The height of the rendered image. Defaults to 256.
         """
         super().__init__(env_id)
         self._use_lidar = use_lidar
         if num_envs == 1:
             self._env = safety_gymnasium.make(
                 id=env_id.replace('-modelbased', ''),
                 autoreset=False,
                 **kwargs,
             )
+            assert isinstance(self._env.action_space, Box), 'Only support Box action space.'
+            assert isinstance(
+                self._env.observation_space,
+                Box,
+            ), 'Only support Box observation space.'
             self._action_space = self._env.action_space
         else:
             raise NotImplementedError
 
         self._device = torch.device(device)
 
         self._num_envs = num_envs
         self._metadata = self._env.metadata
-        self._constraints = ['hazards']  # gremlins, vase, buttons
-        self._xyz_sensors = ['velocimeter', 'accelerometer']
-        self._angle_sensors = ['gyro', 'magnetometer']
-        self._flatten_order = (
+        self._constraints: list[str] = ['hazards']  # gremlins, vase, buttons
+        self._xyz_sensors: list[str] = ['velocimeter', 'accelerometer']
+        self._angle_sensors: list[str] = ['gyro', 'magnetometer']
+        self._flatten_order: list[str] = (
             self._xyz_sensors
             + self._angle_sensors
             + ['goal']
             + self._constraints
             + ['robot_m']
             + ['robot']
         )
-        self._base_state = self._xyz_sensors + self._angle_sensors
-        self._task = 'Goal'
+        self._base_state: list[str] = self._xyz_sensors + self._angle_sensors
+        self._task: str = 'Goal'
         self._env.reset()
-        self.goal_position = self._env.task.goal.pos
-        self.robot_position = self._env.task.agent.pos
-        self.hazards_position = self._env.task.hazards.pos
-        self.goal_distance = self._dist_xy(self.robot_position, self.goal_position)
+        self.goal_position: np.ndarray = self._env.task.goal.pos
+        self.robot_position: np.ndarray = self._env.task.agent.pos
+        self.hazards_position: list[np.ndarray] = self._env.task.hazards.pos
+        self.goal_distance: float = self._dist_xy(self.robot_position, self.goal_position)
 
-        coordinate_sensor_obs = self._get_coordinate_sensor()
-        self._coordinate_obs_size = sum(
+        coordinate_sensor_obs: dict[str, Any] = self._get_coordinate_sensor()
+        self._coordinate_obs_size: int = sum(
             np.prod(i.shape) for i in list(coordinate_sensor_obs.values())
         )
-        offset = 0
-        self.key_to_slice = {}
-        self.key_to_slice_tensor = {}
+        offset: int = 0
+        self.key_to_slice: dict[str, slice] = {}
+        self.key_to_slice_tensor: dict[str, torch.Tensor] = {}
 
         for k in self._flatten_order:
             k_size = np.prod(coordinate_sensor_obs[k].shape)
             self.key_to_slice[k] = slice(offset, offset + k_size)
             self.key_to_slice_tensor[k] = torch.arange(offset, offset + k_size)
 
             offset += k_size
-        self._base_state_size = sum(
+        self._base_state_size: int = sum(
             np.prod(coordinate_sensor_obs[k].shape) for k in list(self._base_state)
         )
         self.key_to_slice['base_state'] = slice(0, self._base_state_size)
         self.key_to_slice_tensor['base_state'] = torch.arange(0, self._base_state_size)
 
-        self._num_lidar_bin = 16
-        self._max_lidar_dist = 3
-        self.hazards_size = 0.2
-        self.goal_size = 0.3
-        self.original_observation_space = self._env.observation_space
-        self.coordinate_observation_space = gymnasium.spaces.Box(
+        self._num_lidar_bin: int = 16
+        self._max_lidar_dist: int = 3
+        self.hazards_size: float = 0.2
+        self.goal_size: float = 0.3
+        self.original_observation_space: OmnisafeSpace = self._env.observation_space
+        self.coordinate_observation_space: OmnisafeSpace = gymnasium.spaces.Box(
             -np.inf,
             np.inf,
             (self._coordinate_obs_size,),
             dtype=np.float32,
         )
         flat_coordinate_obs = self._get_flat_coordinate(coordinate_sensor_obs)
-        self.lidar_observation_space = gymnasium.spaces.Box(
+        self.lidar_observation_space: OmnisafeSpace = gymnasium.spaces.Box(
             -np.inf,
             np.inf,
             (self.get_lidar_from_coordinate(flat_coordinate_obs).shape[0],),
             dtype=np.float32,
         )
         if self._use_lidar:
             self._observation_space = self.lidar_observation_space
         else:
             self._observation_space = self.coordinate_observation_space
 
     @property
     def task(self) -> str:
-        """Get the name of the task."""
+        """The name of the task."""
         return self._task
 
     def get_cost_from_obs_tensor(self, obs: torch.Tensor, is_binary: bool = True) -> torch.Tensor:
         """Get batch cost from batch observation.
 
         Args:
             obs (torch.Tensor): Batch observation.
             is_binary (bool, optional): Whether to use binary cost. Defaults to True.
 
         Returns:
-            cost (torch.Tensor): Batch cost.
+            cost: Batch cost.
         """
         assert torch.is_tensor(obs), 'obs must be tensor'
         hazards_key = self.key_to_slice_tensor['hazards']
         if len(obs.shape) == 2:
             batch_size = obs.shape[0]
             hazard_obs = obs[:, hazards_key].reshape(batch_size, -1, 2)
         elif len(obs.shape) == 3:
@@ -179,95 +193,29 @@
             ) * 10
         if len(obs.shape) == 2:
             cost = cost.reshape(obs.shape[0], 1)
         elif len(obs.shape) == 3:
             cost = cost.reshape(obs.shape[0], obs.shape[1], 1)
         return cost
 
-    def get_goal_flag_from_obs_tensor(self, obs: torch.Tensor) -> torch.Tensor:
-        """Get goal flag from batch observation.
-
-        Args:
-            obs (torch.Tensor): Batch observation.
-
-        Returns:
-            goal_flat (torch.Tensor): Batch goal flag.
-        """
-        assert torch.is_tensor(obs), 'obs must be tensor'
-        goal_key = self.key_to_slice_tensor['goal']
-        if len(obs.shape) == 2:
-            batch_size = obs.shape[0]
-            goal_obs = obs[:, goal_key].reshape(batch_size, -1, 2)
-        elif len(obs.shape) == 3:
-            batch_size = obs.shape[0] * obs.shape[1]
-            goal_obs = obs[:, :, goal_key].reshape(batch_size, -1, 2)
-        goal_dist = torch.sqrt(torch.sum(torch.square(goal_obs), dim=2)).reshape(batch_size, -1)
-        goal_flat = goal_dist <= self.goal_size
-
-        if len(obs.shape) == 2:
-            goal_flat = goal_flat.reshape(obs.shape[0], 1)
-        elif len(obs.shape) == 3:
-            goal_flat = goal_flat.reshape(obs.shape[0], obs.shape[1], 1)
-        return goal_flat
-
-    def get_cost_from_obs(self, obs: np.ndarray, is_binary: bool, use_lidar: bool) -> np.ndarray:
-        """Get batch cost from batch numpy observation.
-
-        Args:
-            obs (np.ndarray): Batch observation.
-            is_binary (bool): Whether to use binary cost.
-            use_lidar (bool): Whether to use lidar.
-
-        Returns:
-            cost (np.ndarray): Batch cost.
-        """
-        assert not torch.is_tensor(obs), 'obs should be numpy array'
-        if not use_lidar:
-            batch_size = obs.shape[0]
-            hazards_key = self.key_to_slice['hazards']
-            hazard_obs = obs[:, hazards_key].reshape(batch_size, -1, 2)
-            hazards_dist = np.sqrt(np.sum(np.square(hazard_obs), axis=2)).reshape(batch_size, -1)
-            if is_binary:
-                cost = np.where(hazards_dist <= self.hazards_size, 1.0, 0.0)
-                cost = cost.sum(1)
-                cost = np.where(cost >= 1, 1.0, 0.0)
-            else:
-                cost = (
-                    (hazards_dist < self.hazards_size) * (self.hazards_size - hazards_dist)
-                ).sum(
-                    1,
-                ) * 10
-        else:
-            batch_size = obs.shape[0]
-            hazards_key = self.key_to_slice['hazards_lidar']
-            hazard_obs = obs[:, hazards_key].reshape(batch_size, self._env.task.lidar_conf.num_bins)
-            lidar_hazards_threshold = (
-                max(0, self._env.task.lidar_conf.max_dist - self._env.task.hazards.size)
-                / self._env.task.lidar_conf.max_dist
-            )
-            cost = np.where(hazard_obs >= lidar_hazards_threshold, 1.0, 0.0)
-            cost = cost.sum(1)
-            cost = np.where(cost >= 1, 1.0, 0.0)
-        return cost
-
     def get_lidar_from_coordinate(self, obs: np.ndarray) -> torch.Tensor:
         """Get lidar observation.
 
         Args:
-            obs (np.ndarray): observation.
+            obs (np.ndarray): The observation.
 
         Returns:
-            lidar_obs (np.ndarray): lidar observation.
+            lidar_obs: The lidar observation.
         """
         robot_matrix_x_y = obs[self.key_to_slice['robot_m']]
-        robot_matrix_x = robot_matrix_x_y[0]
-        robot_matrix_y = robot_matrix_x_y[1]
-        first_row = [robot_matrix_x, robot_matrix_y, 0]
-        second_row = [-robot_matrix_y, robot_matrix_x, 0]
-        third_row = [0, 0, 1]
+        robot_matrix_x = float(robot_matrix_x_y[0])
+        robot_matrix_y = float(robot_matrix_x_y[1])
+        first_row = [robot_matrix_x, robot_matrix_y, 0.0]
+        second_row = [-robot_matrix_y, robot_matrix_x, 0.0]
+        third_row = [0.0, 0.0, 1.0]
         robot_matrix = [first_row, second_row, third_row]
         robot_pos = obs[self.key_to_slice['robot']]
         hazards_lidar_vec = self._obs_lidar_pseudo(robot_matrix, robot_pos, self.hazards_position)
 
         goal_lidar_vec = self._obs_lidar_pseudo(robot_matrix, robot_pos, [self.goal_position])
         base_state_vec = obs[self.key_to_slice['base_state']]
 
@@ -276,43 +224,43 @@
         # obs_vec = self.make_observation(obs, lidar_vec)
         obs_vec = np.array(obs_vec)
         obs_vec = torch.as_tensor(obs_vec, dtype=torch.float32, device=self._device).unsqueeze(0)
         return obs_vec
 
     def _ego_xy(
         self,
-        robot_matrix: list,
+        robot_matrix: list[list[float]],
         robot_pos: np.ndarray,
         pos: np.ndarray,
     ) -> np.ndarray:
         """Return the egocentric XY vector to a position from the robot.
 
         Args:
-            robot_matrix (np.ndarray): 3x3 rotation matrix.
+            robot_matrix (list[list[float]]): 3x3 rotation matrix.
             robot_pos (np.ndarray): 2D robot position.
             pos (np.ndarray): 2D position.
 
         Returns:
-            2D_egocentric_vector (np.ndarray): 2D egocentric vector.
+            2D_egocentric_vector: The 2D egocentric vector.
         """
         assert pos.shape == (2,), f'Bad pos {pos}'
         assert robot_pos.shape == (2,), f'Bad robot_pos {robot_pos}'
         robot_3vec = robot_pos
         robot_mat = robot_matrix
 
         pos_3vec = np.concatenate([pos, [0]])  # add a zero z-coordinate
         robot_3vec = np.concatenate([robot_3vec, [0]])
         world_3vec = pos_3vec - robot_3vec
         return np.matmul(world_3vec, robot_mat)[:2]
 
     def _obs_lidar_pseudo(
         self,
-        robot_matrix: list,
+        robot_matrix: list[list[float]],
         robot_pos: np.ndarray,
-        positions: list,
+        positions: list[np.ndarray],
     ) -> np.ndarray:  # pylint: disable=too-many-locals
         """Return a robot-centric lidar observation of a list of positions.
 
         Lidar is a set of bins around the robot (divided evenly in a circle).
         The detection directions are exclusive and exhaustive for a full 360 view.
         Each bin reads 0 if there are no objects in that direction.
         If there are multiple objects, the distance to the closest one is used.
@@ -326,20 +274,20 @@
             - bins read 0 when empty
             - bins smoothly increase as objects get close
             - maximum reading is 1.0 (where the object overlaps the robot)
             - close objects occlude far objects
             - constant size observation with variable numbers of objects
 
         Args:
-            robot_matrix (np.ndarray): 3x3 rotation matrix.
+            robot_matrix (list[list[float]]): 3x3 rotation matrix.
             robot_pos (np.ndarray): 2D robot position.
-            positions (np.ndarray): 2D positions.
+            positions (list[np.ndarray]): 2D positions.
 
         Returns:
-            lidar_observation (np.ndarray): lidar observation.
+            lidar_observation: The lidar observation.
         """
         obs = np.zeros(self._num_lidar_bin)
         for pos in positions:
             pos = np.asarray(pos)
             if pos.shape == (3,):
                 pos = pos[:2]  # Truncate Z coordinate
             position_z = complex(
@@ -359,37 +307,40 @@
             ), f'bad alias {alias}, dist {dist}, angle {angle}, bin {sensor_bin}'
             bin_plus = (sensor_bin + 1) % self._num_lidar_bin
             bin_minus = (sensor_bin - 1) % self._num_lidar_bin
             obs[bin_plus] = max(obs[bin_plus], alias * sensor)
             obs[bin_minus] = max(obs[bin_minus], (1 - alias) * sensor)
         return obs
 
-    def _get_flat_coordinate(self, coordinate_obs: dict) -> np.ndarray:
+    def _get_flat_coordinate(self, coordinate_obs: dict[str, Any]) -> np.ndarray:
         """Get the flattened obs.
 
         Args:
-            coordinate_obs: dict of coordinate and sensor observations.
+            coordinate_obs (dict[str, Any]): The dict of coordinate and sensor observations.
 
         Returns:
-            flat_obs (np.ndarray): flattened observation.
+            flat_obs: The flattened observation.
         """
+        assert (
+            self.coordinate_observation_space.shape is not None
+        ), 'Bad coordinate_observation_space'
         flat_obs = np.zeros(self.coordinate_observation_space.shape[0])
         for k in self._flatten_order:
             idx = self.key_to_slice[k]
             flat_obs[idx] = coordinate_obs[k].flat
         return flat_obs
 
-    def _get_coordinate_sensor(self) -> dict:
+    def _get_coordinate_sensor(self) -> dict[str, Any]:
         """Return the coordinate observation and sensor observation.
 
         We will ignore the z-axis coordinates in every poses.
         The returned obs coordinates are all in the robot coordinates.
 
         Returns:
-            coordinate_obs (dict): coordinate observation.
+            coordinate_obs: The coordinate observation.
         """
         obs = {}
         robot_matrix = self._env.task.agent.mat
         obs['robot_m'] = np.array(robot_matrix[0][:2])
 
         robot_pos = self._env.task.agent.pos
         goal_pos = self._env.task.goal.pos
@@ -422,56 +373,63 @@
         obs['hazards'] = np.array(ego_hazards_pos_list)  # (hazard_num, 2)
         obs['goal'] = ego_goal_pos  # (2,)
         # obs['vases'] = np.array(ego_vases_pos_list)  # (vase_num, 2)
         return obs
 
     def _dist_xy(
         self,
-        pos1: np.ndarray | list,
-        pos2: np.ndarray | list,
+        pos1: np.ndarray | list[np.ndarray],
+        pos2: np.ndarray | list[np.ndarray],
     ) -> float:
         """Return the distance from the robot to an XY position.
 
         Args:
-            pos1 (np.ndarray | list): The first position.
-            pos2 (np.ndarray | list): The second position.
+            pos1 (np.ndarray | list[np.ndarray]): The first position.
+            pos2 (np.ndarray | list[np.ndarray]): The second position.
 
         Returns:
-            distance (float): The distance between the two positions.
+            distance: The distance between the two positions.
         """
         pos1 = np.asarray(pos1)
         pos2 = np.asarray(pos2)
         if pos1.shape == (3,):
             pos1 = pos1[:2]
         if pos2.shape == (3,):
             pos2 = pos2[:2]
         return np.sqrt(np.sum(np.square(pos1 - pos2)))
 
     def step(
         self,
         action: torch.Tensor,
-    ) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, dict]:
+    ) -> tuple[
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        dict[str, Any],
+    ]:
         """Step the environment.
 
         .. note::
 
             OmniSafe use auto reset wrapper to reset the environment when the episode is
             terminated. So the ``obs`` will be the first observation of the next episode.
             And the true ``final_observation`` in ``info`` will be stored in the ``final_observation`` key of ``info``.
 
         Args:
             action (torch.Tensor): Action to take.
 
         Returns:
-            observation (torch.Tensor): agent's observation of the current environment.
-            reward (torch.Tensor): amount of reward returned after previous action.
-            cost (torch.Tensor): amount of cost returned after previous action.
-            terminated (torch.Tensor): whether the episode has ended.
-            truncated (torch.Tensor): whether the episode has been truncated due to a time limit.
-            info (Dict): contains auxiliary diagnostic information (helpful for debugging, and sometimes learning).
+            observation: The agent's observation of the current environment.
+            reward: The amount of reward returned after previous action.
+            cost: The amount of cost returned after previous action.
+            terminated: Whether the episode has ended.
+            truncated: Whether the episode has been truncated due to a time limit.
+            info: Some information logged by the environment.
         """
         obs_original, reward, cost, terminated, truncated, info = self._env.step(
             action.detach().cpu().numpy(),
         )
 
         if self._task == 'Goal':
             info['old_goal_distance'] = self.goal_distance
@@ -502,23 +460,23 @@
                 info['final_observation'],
                 dtype=torch.float32,
                 device=self._device,
             )
 
         return obs, reward, cost, terminated, truncated, info
 
-    def reset(self, seed: int | None = None) -> tuple[torch.Tensor, dict]:
+    def reset(self, seed: int | None = None) -> tuple[torch.Tensor, dict[str, Any]]:
         """Reset the environment.
 
         Args:
             seed (int, optional): Seed to reset the environment. Defaults to None.
 
         Returns:
-            observation (torch.Tensor): agent's observation of the current environment.
-            info (Dict): contains auxiliary diagnostic information (helpful for debugging, and sometimes learning).
+            observation: The initial observation of the space.
+            info: Some information logged by the environment.
         """
         obs_original, info = self._env.reset(seed=seed)
         if self._task == 'Goal':
             self.goal_position = self._env.task.goal.pos
             self.robot_position = self._env.task.agent.pos
             self.hazards_position = self._env.task.hazards.pos
             self.goal_distance = self._dist_xy(self.robot_position, self.goal_position)
@@ -539,26 +497,27 @@
         """
         self.reset(seed=seed)
 
     def sample_action(self) -> torch.Tensor:
         """Sample a random action.
 
         Returns:
-            torch.Tensor: A random action.
+            The sampled action.
         """
         return torch.as_tensor(
             self._env.action_space.sample(),
             dtype=torch.float32,
             device=self._device,
         )
 
     def render(self) -> Any:
         """Render the environment.
 
         Returns:
-            Any: Rendered environment.
+            The rendered frames, we recommend using `np.ndarray` which could construct video by
+            moviepy.
         """
         return self._env.render()
 
     def close(self) -> None:
         """Close the environment."""
         self._env.close()
```

### Comparing `omnisafe-0.4.0/omnisafe/envs/wrapper.py` & `omnisafe-0.5.0b0/omnisafe/envs/wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -500,15 +500,15 @@
         action = self._old_min_action + (self._old_max_action - self._old_min_action) * (
             action - self._min_action
         ) / (self._max_action - self._min_action)
         return super().step(action)
 
 
 class ActionRepeat(Wrapper):
-    """Repeat ab action given times.
+    """Repeat action given times.
 
     Example:
         >>> env = ActionRepeat(env, times=3)
     """
 
     def __init__(
         self,
@@ -526,16 +526,35 @@
         super().__init__(env=env, device=device)
         self._times = times
         self._device = device
 
     def step(
         self,
         action: torch.Tensor,
-    ) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, dict]:
-        """Run self._times timesteps of the environment's dynamics using the agent actions."""
+    ) -> tuple[
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        torch.Tensor,
+        dict[str, Any],
+    ]:
+        """Run self._times timesteps of the environment's dynamics using the agent actions.
+
+        Args:
+            action (torch.Tensor): The action from the agent or random.
+
+        Returns:
+            observation: The agent's observation of the current environment.
+            reward: The amount of reward returned after previous action.
+            cost: The amount of cost returned after previous action.
+            terminated: Whether the episode has ended.
+            truncated: Whether the episode has been truncated due to a time limit.
+            info: Some information logged by the environment.
+        """
         rewards, costs = torch.tensor(0.0).to(self._device), torch.tensor(0.0).to(self._device)
         for _step, _ in enumerate(range(self._times)):
             obs, reward, cost, terminated, truncated, info = super().step(action)
             rewards += reward
             costs += cost
             goal_met = info.get('goal_met', False)
             if terminated or truncated or goal_met:
```

### Comparing `omnisafe-0.4.0/omnisafe/models/__init__.py` & `omnisafe-0.5.0b0/omnisafe/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,19 @@
 # ==============================================================================
 """This module contains the model for all methods."""
 
 from omnisafe.models.actor import ActorBuilder
 from omnisafe.models.actor.gaussian_actor import GaussianActor
 from omnisafe.models.actor.gaussian_learning_actor import GaussianLearningActor
 from omnisafe.models.actor.gaussian_sac_actor import GaussianSACActor
+from omnisafe.models.actor.mlp_actor import MLPActor
+from omnisafe.models.actor.perturbation_actor import PerturbationActor
+from omnisafe.models.actor.vae_actor import VAE
 from omnisafe.models.actor_critic.actor_critic import ActorCritic
 from omnisafe.models.actor_critic.actor_q_critic import ActorQCritic
 from omnisafe.models.actor_critic.constraint_actor_critic import ConstraintActorCritic
 from omnisafe.models.actor_critic.constraint_actor_q_critic import ConstraintActorQCritic
 from omnisafe.models.base import Actor, Critic
 from omnisafe.models.critic import CriticBuilder
 from omnisafe.models.critic.q_critic import QCritic
 from omnisafe.models.critic.v_critic import VCritic
+from omnisafe.models.offline.dice import ObsEncoder
```

### Comparing `omnisafe-0.4.0/omnisafe/models/actor/__init__.py` & `omnisafe-0.5.0b0/omnisafe/models/actor/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,7 +15,9 @@
 """The abstract interfaces of Actor networks for the Actor-Critic algorithm."""
 
 from omnisafe.models.actor.actor_builder import ActorBuilder
 from omnisafe.models.actor.gaussian_actor import GaussianActor
 from omnisafe.models.actor.gaussian_learning_actor import GaussianLearningActor
 from omnisafe.models.actor.gaussian_sac_actor import GaussianSACActor
 from omnisafe.models.actor.mlp_actor import MLPActor
+from omnisafe.models.actor.perturbation_actor import PerturbationActor
+from omnisafe.models.actor.vae_actor import VAE
```

### Comparing `omnisafe-0.4.0/omnisafe/models/actor/actor_builder.py` & `omnisafe-0.5.0b0/omnisafe/models/actor/actor_builder.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 """Implementation of ActorBuilder."""
 
 from __future__ import annotations
 
 from omnisafe.models.actor.gaussian_learning_actor import GaussianLearningActor
 from omnisafe.models.actor.gaussian_sac_actor import GaussianSACActor
 from omnisafe.models.actor.mlp_actor import MLPActor
+from omnisafe.models.actor.perturbation_actor import PerturbationActor
+from omnisafe.models.actor.vae_actor import VAE
 from omnisafe.typing import Activation, ActorType, InitFunction, OmnisafeSpace
 
 
 # pylint: disable-next=too-few-public-methods
 class ActorBuilder:
     """Class for building actor networks.
 
@@ -50,27 +52,27 @@
         self._activation: Activation = activation
         self._hidden_sizes: list[int] = hidden_sizes
 
     # pylint: disable-next=too-many-return-statements
     def build_actor(
         self,
         actor_type: ActorType,
-    ) -> GaussianLearningActor | GaussianSACActor | MLPActor:
+    ) -> GaussianLearningActor | GaussianSACActor | MLPActor | VAE | PerturbationActor:
         """Build actor network.
 
         Currently, we support the following actor types:
             - ``gaussian_learning``: Gaussian actor with learnable standard deviation parameters.
             - ``gaussian_sac``: Gaussian actor with learnable standard deviation network.
             - ``mlp``: Multi-layer perceptron actor, used in ``DDPG`` and ``TD3``.
 
         Args:
             actor_type (ActorType): Type of actor network, e.g. ``gaussian_learning``.
 
         Returns:
-            Actor network, ranging from ``GaussianLearningActor``, ``GaussianSACActor`` to ``MLPActor``.
+            Actor network, ranging from GaussianLearningActor, GaussianSACActor to MLPActor.
 
         Raises:
             NotImplementedError: If the actor type is not implemented.
         """
         if actor_type == 'gaussian_learning':
             return GaussianLearningActor(
                 self._obs_space,
@@ -91,11 +93,27 @@
             return MLPActor(
                 self._obs_space,
                 self._act_space,
                 self._hidden_sizes,
                 activation=self._activation,
                 weight_initialization_mode=self._weight_initialization_mode,
             )
+        if actor_type == 'vae':
+            return VAE(
+                self._obs_space,
+                self._act_space,
+                self._hidden_sizes,
+                activation=self._activation,
+                weight_initialization_mode=self._weight_initialization_mode,
+            )
+        if actor_type == 'perturbation':
+            return PerturbationActor(
+                self._obs_space,
+                self._act_space,
+                self._hidden_sizes,
+                activation=self._activation,
+                weight_initialization_mode=self._weight_initialization_mode,
+            )
         raise NotImplementedError(
             f'Actor type {actor_type} is not implemented! '
-            f'Available actor types are: gaussian_learning, gaussian_sac, mlp.',
+            f'Available actor types are: gaussian_learning, gaussian_sac, mlp, vae, perturbation.',
         )
```

### Comparing `omnisafe-0.4.0/omnisafe/models/actor/gaussian_actor.py` & `omnisafe-0.5.0b0/omnisafe/models/actor/gaussian_actor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/models/actor/gaussian_learning_actor.py` & `omnisafe-0.5.0b0/omnisafe/models/actor/gaussian_learning_actor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -87,16 +87,15 @@
         - If ``deterministic`` is ``False``, the predicted action is sampled from the distribution.
 
         Args:
             obs (torch.Tensor): Observation from environments.
             deterministic (bool, optional): Whether to use deterministic policy. Defaults to False.
 
         Returns:
-            The mean of the distribution if ``deterministic`` is ``True``, otherwise the sampled
-            action.
+            The mean of the distribution if deterministic is True, otherwise the sampled action.
         """
         self._current_dist = self._distribution(obs)
         self._after_inference = True
         if deterministic:
             return self._current_dist.mean
         return self._current_dist.rsample()
 
@@ -116,15 +115,15 @@
     def log_prob(self, act: torch.Tensor) -> torch.Tensor:
         """Compute the log probability of the action given the current distribution.
 
         .. warning::
             You must call :meth:`forward` or :meth:`predict` before calling this method.
 
         Args:
-            act (torch.Tensor): Action.
+            act (torch.Tensor): Action from :meth:`predict` or :meth:`forward` .
 
         Returns:
             Log probability of the action.
         """
         assert self._after_inference, 'log_prob() should be called after predict() or forward()'
         self._after_inference = False
         return self._current_dist.log_prob(act).sum(axis=-1)
```

### Comparing `omnisafe-0.4.0/omnisafe/models/actor/gaussian_sac_actor.py` & `omnisafe-0.5.0b0/omnisafe/models/actor/gaussian_sac_actor.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from omnisafe.utils.model import build_mlp_network
 
 
 class GaussianSACActor(Actor):
     """Implementation of GaussianSACActor.
 
     GaussianSACActor is a Gaussian actor with a learnable standard deviation network.
-    It is used in ``SAC``, and other off-line or model-based algorithms related to ``SAC``.
+    It is used in ``SAC``, and other offline or model-based algorithms related to ``SAC``.
 
     Args:
         obs_space (OmnisafeSpace): Observation space.
         act_space (OmnisafeSpace): Action space.
         hidden_sizes (list of int): List of hidden layer sizes.
         activation (Activation, optional): Activation function. Defaults to ``'relu'``.
         weight_initialization_mode (InitFunction, optional): Weight initialization mode. Defaults to
@@ -93,16 +93,15 @@
         - If ``deterministic`` is ``False``, the predicted action is sampled from the distribution.
 
         Args:
             obs (torch.Tensor): Observation from environments.
             deterministic (bool, optional): Whether to use deterministic policy. Defaults to False.
 
         Returns:
-            The mean of the distribution if ``deterministic`` is ``True``, otherwise the sampled
-            action.
+            The mean of the distribution if deterministic is True, otherwise the sampled action.
         """
         self._current_dist = self._distribution(obs)
         self._after_inference = True
 
         action = self._current_dist.mean if deterministic else self._current_dist.rsample()
 
         self._current_raw_action = action
@@ -130,21 +129,21 @@
 
         .. note::
             In this method, we will regularize the log probability of the action. The regularization
             is as follows:
 
             .. math::
 
-                \log \pi (a|s) = \log \pi (a|s) - \sum_{i=1}^n (2 \log 2 - a_i - \log (1 + e^{-2 a_i}))
+                \log prob = \log \pi (a|s) - \sum_{i=1}^n (2 \log 2 - a_i - \log (1 + e^{-2 a_i}))
 
             where :math:`a` is the action, :math:`s` is the observation, and :math:`n` is the
             dimension of the action.
 
         Args:
-            act (torch.Tensor): Action.
+            act (torch.Tensor): Action from :meth:`predict` or :meth:`forward`.
 
         Returns:
             Log probability of the action.
         """
         assert self._after_inference, 'log_prob() should be called after predict() or forward()'
         self._after_inference = False
```

### Comparing `omnisafe-0.4.0/omnisafe/models/actor/mlp_actor.py` & `omnisafe-0.5.0b0/omnisafe/models/actor/mlp_actor.py`

 * *Files 8% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         """
         return self._distribution(obs)
 
     def log_prob(self, act: torch.Tensor) -> torch.Tensor:
         """Log probability of the action.
 
         Args:
-            act (torch.Tensor): Action tensor.
+            act (torch.Tensor): Action from :meth:`predict` or :meth:`forward`  tensor.
 
         Raises:
             NotImplementedError: The method is not implemented.
         """
         raise NotImplementedError
 
     @property
```

### Comparing `omnisafe-0.4.0/omnisafe/models/actor_critic/__init__.py` & `omnisafe-0.5.0b0/omnisafe/models/actor_critic/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/models/actor_critic/actor_critic.py` & `omnisafe-0.5.0b0/omnisafe/models/actor_critic/actor_critic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,15 +16,21 @@
 
 from __future__ import annotations
 
 import torch
 from torch import nn, optim
 from torch.optim.lr_scheduler import ConstantLR, LinearLR
 
-from omnisafe.models.actor import GaussianLearningActor, GaussianSACActor, MLPActor
+from omnisafe.models.actor import (
+    VAE,
+    GaussianLearningActor,
+    GaussianSACActor,
+    MLPActor,
+    PerturbationActor,
+)
 from omnisafe.models.actor.actor_builder import ActorBuilder
 from omnisafe.models.base import Critic
 from omnisafe.models.critic.critic_builder import CriticBuilder
 from omnisafe.typing import OmnisafeSpace
 from omnisafe.utils.config import ModelConfig
 from omnisafe.utils.schedule import PiecewiseSchedule, Schedule
 
@@ -63,21 +69,23 @@
         act_space: OmnisafeSpace,
         model_cfgs: ModelConfig,
         epochs: int,
     ) -> None:
         """Initialize an instance of :class:`ActorCritic`."""
         super().__init__()
 
-        self.actor: GaussianLearningActor | GaussianSACActor | MLPActor = ActorBuilder(
+        self.actor: GaussianLearningActor | GaussianSACActor | MLPActor | VAE | PerturbationActor = ActorBuilder(
             obs_space=obs_space,
             act_space=act_space,
             hidden_sizes=model_cfgs.actor.hidden_sizes,
             activation=model_cfgs.actor.activation,
             weight_initialization_mode=model_cfgs.weight_initialization_mode,
-        ).build_actor(actor_type=model_cfgs.actor_type)
+        ).build_actor(
+            actor_type=model_cfgs.actor_type,
+        )
         self.reward_critic: Critic = CriticBuilder(
             obs_space=obs_space,
             act_space=act_space,
             hidden_sizes=model_cfgs.critic.hidden_sizes,
             activation=model_cfgs.critic.activation,
             weight_initialization_mode=model_cfgs.weight_initialization_mode,
             num_critics=1,
@@ -116,15 +124,15 @@
         self,
         obs: torch.Tensor,
         deterministic: bool = False,
     ) -> tuple[torch.Tensor, ...]:
         """Choose the action based on the observation. used in rollout without gradient.
 
         Args:
-            obs (torch.tensor): The observation.
+            obs (torch.tensor): The observation from environments.
             deterministic (bool, optional): Whether to use deterministic action. Defaults to False.
 
         Returns:
             action: The deterministic action if ``deterministic`` is True, otherwise the action with
                 Gaussian noise.
             value_r: The reward value of the observation.
             log_prob: The log probability of the action.
@@ -139,15 +147,15 @@
         self,
         obs: torch.Tensor,
         deterministic: bool = False,
     ) -> tuple[torch.Tensor, ...]:
         """Choose the action based on the observation. used in training with gradient.
 
         Args:
-            obs (torch.tensor): The observation.
+            obs (torch.tensor): The observation from environments.
             deterministic (bool, optional): Whether to use deterministic action. Defaults to False.
 
         Returns:
             action: The deterministic action if ``deterministic`` is True, otherwise the action with
                 Gaussian noise.
             value_r: The reward value of the observation.
             log_prob: The log probability of the action.
```

### Comparing `omnisafe-0.4.0/omnisafe/models/actor_critic/actor_q_critic.py` & `omnisafe-0.5.0b0/omnisafe/models/actor_critic/actor_q_critic.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,21 @@
 
 from copy import deepcopy
 
 import torch
 from torch import nn, optim
 from torch.optim.lr_scheduler import ConstantLR, LinearLR
 
-from omnisafe.models.actor import GaussianLearningActor, GaussianSACActor, MLPActor
+from omnisafe.models.actor import (
+    VAE,
+    GaussianLearningActor,
+    GaussianSACActor,
+    MLPActor,
+    PerturbationActor,
+)
 from omnisafe.models.actor.actor_builder import ActorBuilder
 from omnisafe.models.base import Critic
 from omnisafe.models.critic.critic_builder import CriticBuilder
 from omnisafe.typing import OmnisafeSpace
 from omnisafe.utils.config import ModelConfig
 
 
@@ -66,34 +72,36 @@
         act_space: OmnisafeSpace,
         model_cfgs: ModelConfig,
         epochs: int,
     ) -> None:
         """Initialize an instance of :class:`ActorQCritic`."""
         super().__init__()
 
-        self.actor: GaussianLearningActor | GaussianSACActor | MLPActor = ActorBuilder(
+        self.actor: GaussianLearningActor | GaussianSACActor | MLPActor | VAE | PerturbationActor = ActorBuilder(
             obs_space=obs_space,
             act_space=act_space,
             hidden_sizes=model_cfgs.actor.hidden_sizes,
             activation=model_cfgs.actor.activation,
             weight_initialization_mode=model_cfgs.weight_initialization_mode,
-        ).build_actor(actor_type=model_cfgs.actor_type)
+        ).build_actor(
+            actor_type=model_cfgs.actor_type,
+        )
         self.reward_critic: Critic = CriticBuilder(
             obs_space=obs_space,
             act_space=act_space,
             hidden_sizes=model_cfgs.critic.hidden_sizes,
             activation=model_cfgs.critic.activation,
             weight_initialization_mode=model_cfgs.weight_initialization_mode,
             num_critics=model_cfgs.critic.num_critics,
             use_obs_encoder=False,
         ).build_critic(critic_type='q')
         self.target_reward_critic: Critic = deepcopy(self.reward_critic)
         for param in self.target_reward_critic.parameters():
             param.requires_grad = False
-        self.target_actor: GaussianLearningActor | GaussianSACActor | MLPActor = deepcopy(
+        self.target_actor: GaussianLearningActor | GaussianSACActor | MLPActor | VAE | PerturbationActor = deepcopy(
             self.actor,
         )
         for param in self.target_actor.parameters():
             param.requires_grad = False
         self.add_module('actor', self.actor)
         self.add_module('reward_critic', self.reward_critic)
 
@@ -124,34 +132,34 @@
                 verbose=True,
             )
 
     def step(self, obs: torch.Tensor, deterministic: bool = False) -> torch.Tensor:
         """Choose the action based on the observation. used in rollout without gradient.
 
         Args:
-            obs (torch.tensor): The observation.
+            obs (torch.tensor): The observation from environments.
             deterministic (bool, optional): Whether to use deterministic action. Defaults to False.
 
         Returns:
-            The deterministic action if ``deterministic`` is True, otherwise the action with
-            Gaussian noise.
+            The deterministic action if deterministic is True.
+            Action with noise other wise.
         """
         with torch.no_grad():
             return self.actor.predict(obs, deterministic=deterministic)
 
     def forward(self, obs: torch.Tensor, deterministic: bool = False) -> torch.Tensor:
         """Choose the action based on the observation. used in training with gradient.
 
         Args:
-            obs (torch.tensor): The observation.
+            obs (torch.tensor): The observation from environments.
             deterministic (bool, optional): Whether to use deterministic action. Defaults to False.
 
         Returns:
-            The deterministic action if ``deterministic`` is True, otherwise the action with
-            Gaussian noise.
+            The deterministic action if deterministic is True.
+            Action with noise other wise.
         """
         return self.step(obs, deterministic=deterministic)
 
     def polyak_update(self, tau: float) -> None:
         """Update the target network with polyak averaging.
 
         Args:
```

### Comparing `omnisafe-0.4.0/omnisafe/models/actor_critic/constraint_actor_critic.py` & `omnisafe-0.5.0b0/omnisafe/models/actor_critic/constraint_actor_critic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/models/actor_critic/constraint_actor_q_critic.py` & `omnisafe-0.5.0b0/omnisafe/models/actor_critic/constraint_actor_q_critic.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.4.0/omnisafe/models/base.py` & `omnisafe-0.5.0b0/omnisafe/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -23,15 +23,15 @@
 from gymnasium import spaces
 from torch.distributions import Distribution
 
 from omnisafe.typing import Activation, InitFunction, OmnisafeSpace
 
 
 class Actor(nn.Module, ABC):
-    """A abstract class for actor.
+    """An abstract class for actor.
 
     An actor approximates the policy function that maps observations to actions. Actor is
     parameterized by a neural network that takes observations as input, and outputs the mean and
     standard deviation of the action distribution.
 
     .. note::
         You can use this class to implement your own actor by inheriting it.
@@ -125,23 +125,23 @@
         ``deterministic=False``).
 
         When testing the actor, we want to know the actual action that the agent will take, so we
         should use deterministic actions (set ``deterministic=True``).
 
         .. math::
 
-            L = -\mathbb{E}_{s \sim p(s)} [ \log p (a | s) A^R (s, a) ]
+            L = -\underset{s \sim p(s)}{\mathbb{E}}[ \log p (a | s) A^R (s, a) ]
 
         where :math:`p (s)` is the distribution of observation, :math:`p (a | s)` is the
         distribution of action, and :math:`\log p (a | s)` is the log probability of action under
         the distribution., and :math:`A^R (s, a)` is the advantage function.
 
         Args:
             obs (torch.Tensor): Observation from environments.
-            deterministic (bool, optional): whether to predict deterministic action. Defaults to False.
+            deterministic (bool, optional): Whether to predict deterministic action. Defaults to False.
         """
 
     @abstractmethod
     def log_prob(self, act: torch.Tensor) -> torch.Tensor:
         """Return the log probability of action under the distribution.
 
         :meth:`log_prob` only can be called after calling :meth:`predict` or :meth:`forward`.
@@ -151,29 +151,29 @@
 
         Returns:
             The log probability of action under the distribution.
         """
 
 
 class Critic(nn.Module, ABC):
-    """A abstract class for critic.
+    """An abstract class for critic.
 
     A critic approximates the value function that maps observations to values. Critic is
     parameterized by a neural network that takes observations as input, (Q critic also takes actions
-    as input) and outputs the value of the observation.
+    as input) and outputs the value estimated.
 
     .. note::
         OmniSafe provides two types of critic:
         Q critic (Input = ``observation`` + ``action`` , Output = ``value``),
         and V critic (Input = ``observation`` , Output = ``value``).
         You can also use this class to implement your own actor by inheriting it.
 
     Args:
-        obs_space (OmnisafeSpace): observation space.
-        act_space (OmnisafeSpace): action space.
+        obs_space (OmnisafeSpace): Observation space.
+        act_space (OmnisafeSpace): Action space.
         hidden_sizes (list of int): List of hidden layer sizes.
         activation (Activation, optional): Activation function. Defaults to ``'relu'``.
         weight_initialization_mode (InitFunction, optional): Weight initialization mode. Defaults to
             ``'kaiming_uniform'``.
         num_critics (int, optional): Number of critics. Defaults to 1.
         use_obs_encoder (bool, optional): Whether to use observation encoder, only used in q critic.
             Defaults to False.
```

### Comparing `omnisafe-0.4.0/omnisafe/models/critic/__init__.py` & `omnisafe-0.5.0b0/omnisafe/models/critic/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/models/critic/critic_builder.py` & `omnisafe-0.5.0b0/omnisafe/models/critic/critic_builder.py`

 * *Files 7% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         Currently, we support two types of critics: ``q`` and ``v``.
         If you want to add a new critic type, you can simply add it here.
 
         Args:
             critic_type (str): Critic type.
 
         Returns:
-            V-Critic or Q-Critic.
+            An instance of V-Critic or Q-Critic
 
         Raises:
             NotImplementedError: If the critic type is not ``q`` or ``v``.
         """
         if critic_type == 'q':
             return QCritic(
                 obs_space=self._obs_space,
```

### Comparing `omnisafe-0.4.0/omnisafe/models/critic/q_critic.py` & `omnisafe-0.5.0b0/omnisafe/models/critic/q_critic.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Implementation of QCritic."""
+"""Implementation of Q Critic."""
 
 from __future__ import annotations
 
 import torch
 import torch.nn as nn
 
 from omnisafe.models.base import Critic
 from omnisafe.typing import Activation, InitFunction, OmnisafeSpace
 from omnisafe.utils.model import build_mlp_network
 
 
 class QCritic(Critic):
-    """Implementation of QCritic.
+    """Implementation of Q Critic.
 
     A Q-function approximator that uses a multi-layer perceptron (MLP) to map observation-action
     pairs to Q-values. This class is an inherit class of :class:`Critic`. You can design your own
     Q-function approximator by inheriting this class or :class:`Critic`.
 
     The Q critic network has two modes:
 
@@ -93,15 +93,15 @@
                     [hidden_sizes[0] + self._act_dim] + hidden_sizes[1:] + [1],
                     activation=activation,
                     weight_initialization_mode=weight_initialization_mode,
                 )
                 critic = nn.Sequential(obs_encoder, net)
             else:
                 net = build_mlp_network(
-                    [self._obs_dim + self._act_dim, *hidden_sizes] + [1],
+                    [self._obs_dim + self._act_dim, *hidden_sizes, 1],
                     activation=activation,
                     weight_initialization_mode=weight_initialization_mode,
                 )
                 critic = nn.Sequential(net)
             self.net_lst.append(critic)
             self.add_module(f'critic_{idx}', critic)
 
@@ -114,15 +114,15 @@
 
         As a multi-critic network, the output of the network is a list of Q-values. If you want to
         use it as a single-critic network, you only need to set the ``num_critics`` parameter to 1
         when initializing the network, and then use the index 0 to get the Q-value.
 
         Args:
             obs (torch.Tensor): Observation from environments.
-            act (torch.Tensor): Action.
+            act (torch.Tensor): Action from actor .
 
         Returns:
             A list of Q critic values of action and observation pair.
         """
         res = []
         for critic in self.net_lst:
             if self._use_obs_encoder:
```

### Comparing `omnisafe-0.4.0/omnisafe/models/critic/v_critic.py` & `omnisafe-0.5.0b0/omnisafe/models/critic/v_critic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -77,15 +77,15 @@
         obs: torch.Tensor,
     ) -> list[torch.Tensor]:
         """Forward function.
 
         Specifically, V function approximator maps observations to V-values.
 
         Args:
-            obs (torch.Tensor): Observations.
+            obs (torch.Tensor): Observations from environments.
 
         Returns:
             The V critic value of observation.
         """
         res = []
         for critic in self.net_lst:
             res.append(torch.squeeze(critic(obs), -1))
```

### Comparing `omnisafe-0.4.0/omnisafe/typing.py` & `omnisafe-0.5.0b0/omnisafe/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 RenderFrame = TypeVar('RenderFrame')
 OmnisafeSpace = Union[Box, Discrete]
 Activation = Literal['identity', 'relu', 'sigmoid', 'softplus', 'tanh']
 AdvatageEstimator = Literal['gae', 'gae-rtg', 'vtrace', 'plain']
 InitFunction = Literal['kaiming_uniform', 'xavier_normal', 'glorot', 'xavier_uniform', 'orthogonal']
 CriticType = Literal['v', 'q']
-ActorType = Literal['gaussian_learning', 'gaussian_sac', 'mlp']
+ActorType = Literal['gaussian_learning', 'gaussian_sac', 'mlp', 'vae', 'perturbation']
 DEVICE_CPU = torch.device('cpu')
 
 
 __all__ = [
     'Activation',
     'AdvatageEstimator',
     'InitFunction',
```

### Comparing `omnisafe-0.4.0/omnisafe/utils/__init__.py` & `omnisafe-0.5.0b0/omnisafe/common/offline/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Utility functions for OmniSafe."""
+"""Useful Tools for Offline Algorithms."""
+
+
+from omnisafe.common.offline.data_collector import OfflineDataCollector
+from omnisafe.common.offline.dataset import OfflineDataset, OfflineDatasetWithInit, OfflineMeta
```

### Comparing `omnisafe-0.4.0/omnisafe/utils/command_app.py` & `omnisafe-0.5.0b0/omnisafe/utils/command_app.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,23 +49,23 @@
         case_sensitive=False,
     ),
     parallel: int = typer.Option(
         1,
         help='number of paralleled progress for calculations.',
     ),
     total_steps: int = typer.Option(
-        1638400,
+        10000000,
         help='total number of steps to train for algorithm',
     ),
     device: str = typer.Option(
         'cpu',
         help='device to use for training',
     ),
     vector_env_nums: int = typer.Option(
-        16,
+        1,
         help='number of vector envs to use for training',
     ),
     torch_threads: int = typer.Option(
         16,
         help='number of threads to use for torch',
     ),
     log_dir: str = typer.Option(
@@ -141,26 +141,29 @@
         custom_cfgs=parsed_custom_cfgs,
     )
     agent.learn()
 
     if plot:
         try:
             agent.plot(smooth=1)
-        except RuntimeError:
+        except Exception:  # noqa # pragma: no cover # pylint: disable=broad-except
             console.print('failed to plot data', style='red bold')
+            console.print(Exception, style='red bold')
     if render:
         try:
             agent.render(num_episodes=10, render_mode='rgb_array', width=256, height=256)
-        except RuntimeError:
+        except Exception:  # noqa # pragma: no cover # pylint: disable=broad-except
             console.print('failed to render model', style='red bold')
+            console.print(Exception, style='red bold')
     if evaluate:
         try:
             agent.evaluate(num_episodes=10)
-        except RuntimeError:
+        except Exception:  # noqa # pragma: no cover # pylint: disable=broad-except
             console.print('failed to evaluate model', style='red bold')
+            console.print(Exception, style='red bold')
 
 
 @app.command()
 def benchmark(
     exp_name: str = typer.Argument(
         ...,
         help='experiment name',
```

### Comparing `omnisafe-0.4.0/omnisafe/utils/config.py` & `omnisafe-0.5.0b0/omnisafe/utils/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -75,16 +75,16 @@
         env_kwargs (dict): Environment keyword arguments.
         normalize_obs (bool): Whether to normalize observation.
         normalize_rew (bool): Whether to normalize reward.
         normalize_cost (bool): Whether to normalize cost.
         max_len (int): Maximum length.
         num_threads (int): Number of threads.
 
-    Args:
-        **kwargs (Any): Keyword arguments to set config.
+    Keyword Args:
+        kwargs (Any): keyword arguments to set the attributes.
     """
 
     seed: int
     device: str
     device_id: int
     wrapper_type: str
     epochs: int
@@ -260,33 +260,32 @@
 
     This function is used to check the configs.
 
     Args:
         configs (Config): The configs to be checked.
         algo_type (str): The algorithm type.
     """
-    # check algo configs
     __check_algo_configs(configs.algo_cfgs, algo_type)
-    __check_logger_configs(configs.logger_cfgs, algo_type)
     __check_parallel_and_vectorized(configs, algo_type)
+    __check_logger_configs(configs.logger_cfgs)
 
 
 def __check_parallel_and_vectorized(configs: Config, algo_type: str) -> None:
     """Check parallel and vectorized configs.
 
     This function is used to check the parallel and vectorized configs.
 
     Args:
         configs (Config): The configs to be checked.
         algo_type (str): The algorithm type.
     """
-    if algo_type in {'off-policy', 'model-based'}:
+    if algo_type in {'off-policy', 'model-based', 'offline'}:
         assert (
             configs.train_cfgs.parallel == 1
-        ), 'off-policy or model-based only support parallel==1!'
+        ), 'off-policy, offline and model-based only support parallel==1!'
     if configs.algo in ['PPOEarlyTerminated', 'TRPOEarlyTerminated']:
         assert (
             configs.train_cfgs.vector_env_nums == 1
         ), 'PPOEarlyTerminated or TRPOEarlyTerminated only support vector_env_nums == 1!'
 
 
 def __check_algo_configs(configs: Config, algo_type: str) -> None:
@@ -381,25 +380,23 @@
             isinstance(configs.penalty_coef, float)
             and configs.penalty_coef >= 0.0
             and configs.penalty_coef <= 1.0
         ), 'penalty_coef must be float, and it values must be [0.0, 1.0]'
         assert isinstance(configs.use_cost, bool), 'penalty_coef must be bool'
 
 
-def __check_logger_configs(configs: Config, algo_type: str) -> None:
+def __check_logger_configs(configs: Config) -> None:
     """Check logger configs.
 
     Args:
         configs (Config): The configs to be checked.
         algo_type (str): The algorithm type.
     """
-    if algo_type == 'on-policy':
-        assert isinstance(configs.use_wandb, bool) and isinstance(
-            configs.wandb_project,
-            str,
-        ), 'use_wandb and wandb_project must be bool and string'
-        assert isinstance(configs.use_tensorboard, bool), 'use_tensorboard must be bool'
-        assert isinstance(configs.save_model_freq, int) and isinstance(
-            configs.window_lens,
-            int,
-        ), 'save_model_freq and window_lens must be int'
-        assert isinstance(configs.log_dir, str), 'log_dir must be string'
+    assert isinstance(configs.use_wandb, bool) and isinstance(
+        configs.wandb_project,
+        str,
+    ), 'use_wandb and wandb_project must be bool and string'
+    assert isinstance(configs.use_tensorboard, bool), 'use_tensorboard must be bool'
+    assert isinstance(configs.save_model_freq, int), 'save_model_freq must be int'
+    if window_lens := configs.get('window_lens'):
+        assert isinstance(window_lens, int), 'window_lens must be int'
+    assert isinstance(configs.log_dir, str), 'log_dir must be string'
```

### Comparing `omnisafe-0.4.0/omnisafe/utils/distributed.py` & `omnisafe-0.5.0b0/omnisafe/utils/distributed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -24,15 +24,15 @@
 import numpy as np
 import torch
 import torch.distributed as dist
 from torch.distributed import ReduceOp
 
 
 def setup_distributed() -> None:
-    """Setup distributed training environment.
+    """Setup the distributed training environment.
 
     Avoid slowdowns caused by each separate process's PyTorch, using more than its fair share of CPU
     resources.
     """
     old_num_threads = torch.get_num_threads()
     # decrease number of torch threads for MPI
     if old_num_threads > 1 and world_size() > 1:
@@ -42,15 +42,15 @@
             f'Proc {get_rank()}: Decreased number of Torch threads from '
             f'{old_num_threads} to {torch.get_num_threads()}',
             flush=True,
         )
 
 
 def get_rank() -> int:
-    """Get rank of calling process.
+    """Get the rank of calling process.
 
     Examples:
         >>> # In process 0
         >>> get_rank()
         0
 
     Returns:
@@ -81,15 +81,15 @@
 
 
 def fork(
     parallel: int,
     device: str = 'cpu',
     manual_args: list[str] | None = None,
 ) -> bool:
-    """The entrance of multi-processing.
+    """The entrance method of multi-processing.
 
     Re-launches the current script with workers linked by MPI. Also, terminates the original process
     that launched it. Taken almost without modification from the Baselines function of the
     `same name <https://github.com/openai/baselines/blob/master/baselines/common/mpi_fork.py>`_.
 
     Args:
         parallel (int): The number of processes to launch.
@@ -347,31 +347,30 @@
     return value[0] if scalar else value
 
 
 def dist_statistics_scalar(
     value: torch.Tensor,
     with_min_and_max: bool = False,
 ) -> tuple[torch.Tensor, ...]:
-    """Get mean/std and optional min/max of scalar x across MPI processes.
+    r"""Get mean/std and optional min/max of scalar x across MPI processes.
 
     Examples:
         >>> # In process 0
         >>> x = torch.tensor(1.0)
         >>> # In process 1
         >>> x = torch.tensor(2.0)
         >>> dist_statistics_scalar(x)
         (tensor(1.5), tensor(0.5))
 
     Args:
         value (torch.Tensor): Value to be operated.
         with_min_and_max (bool, optional): whether to return min and max. Defaults to False.
 
     Returns:
-        The (mean, std) or (mean, std, min, max) of the input tensor, depends on the value of
-        ``with_min_and_max``.
+        A tuple of the [mean, std] or [mean, std, min, max] of the input tensor.
     """
     global_sum = dist_sum(torch.sum(value))
     global_n = dist_sum(len(value))
     mean = global_sum / global_n
 
     global_sum_sq = dist_sum(torch.sum((value - mean) ** 2))
     # compute global std
```

### Comparing `omnisafe-0.4.0/omnisafe/utils/exp_grid_tools.py` & `omnisafe-0.5.0b0/omnisafe/utils/exp_grid_tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Tools for Experiment Grid."""
 
+
 from __future__ import annotations
 
 import os
 import string
 import sys
 from typing import Any
 
@@ -61,15 +62,15 @@
 
 
 def train(
     exp_id: str,
     algo: str,
     env_id: str,
     custom_cfgs: dict[str, Any],
-) -> Tuple[float, float, int]:
+) -> Tuple[float, float, float]:
     """Train a policy from exp-x config with OmniSafe.
 
     Args:
         exp_id (str): Experiment ID.
         algo (str): Algorithm to train.
         env_id (str): The name of test environment.
         custom_cfgs (Config): Custom configurations.
@@ -80,22 +81,28 @@
         terminal_log_name = f'seed{custom_cfgs["seed"]}_{terminal_log_name}'
         error_log_name = f'seed{custom_cfgs["seed"]}_{error_log_name}'
     sys.stdout = sys.__stdout__
     sys.stderr = sys.__stderr__
     print(f'exp-x: {exp_id} is training...')
     if not os.path.exists(custom_cfgs['logger_cfgs']['log_dir']):
         os.makedirs(custom_cfgs['logger_cfgs']['log_dir'], exist_ok=True)
-    # pylint: disable-next=consider-using-with
-    sys.stdout = open(  # noqa: SIM115
-        os.path.join(f'{custom_cfgs["logger_cfgs"]["log_dir"]}', terminal_log_name),
-        'w',
-        encoding='utf-8',
-    )
-    # pylint: disable-next=consider-using-with
-    sys.stderr = open(  # noqa: SIM115
-        os.path.join(f'{custom_cfgs["logger_cfgs"]["log_dir"]}', error_log_name),
+    with open(
+        os.path.join(
+            f'{custom_cfgs["logger_cfgs"]["log_dir"]}',
+            terminal_log_name,
+        ),
         'w',
         encoding='utf-8',
-    )
-    agent = omnisafe.Agent(algo, env_id, custom_cfgs=custom_cfgs)
-    reward, cost, ep_len = agent.learn()
+    ) as f_out:
+        sys.stdout = f_out
+        with open(
+            os.path.join(
+                f'{custom_cfgs["logger_cfgs"]["log_dir"]}',
+                error_log_name,
+            ),
+            'w',
+            encoding='utf-8',
+        ) as f_error:
+            sys.stderr = f_error
+            agent = omnisafe.Agent(algo, env_id, custom_cfgs=custom_cfgs)
+            reward, cost, ep_len = agent.learn()
     return reward, cost, ep_len
```

### Comparing `omnisafe-0.4.0/omnisafe/utils/math.py` & `omnisafe-0.5.0b0/omnisafe/utils/math.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -22,34 +22,34 @@
 from torch.distributions import Normal, TanhTransform, TransformedDistribution, constraints
 
 
 def get_transpose(tensor: torch.Tensor) -> torch.Tensor:
     """Transpose the last two dimensions of a tensor.
 
     Examples:
-        >>> tensor = torch.rand(2, 3, 4)
+        >>> tensor = torch.rand(2, 3)
         >>> get_transpose(tensor).shape
-        torch.Size([2, 4, 3])
+        torch.Size([3, 2])
 
     Args:
         tensor(torch.Tensor): The tensor to transpose.
 
     Returns:
         Transposed tensor.
     """
     return tensor.transpose(dim0=-2, dim1=-1)
 
 
 def get_diagonal(tensor: torch.Tensor) -> torch.Tensor:
     """Get the diagonal of the last two dimensions of a tensor.
 
     Examples:
-        >>> tensor = torch.rand(2, 3, 4)
+        >>> tensor = torch.rand(3, 3)
         >>> get_diagonal(tensor).shape
-        torch.Size([2, 3])
+        torch.Size([1, 3])
 
     Args:
         tensor (torch.Tensor): The tensor to get the diagonal from.
 
     Returns:
         Diagonal part of the tensor.
     """
@@ -60,15 +60,15 @@
     """Compute the discounted cumulative sum of vectors.
 
     Examples:
         >>> vector_x = torch.arange(1, 5)
         >>> vector_x
         tensor([1, 2, 3, 4])
         >>> discount_cumsum(vector_x, 0.9)
-        tensor([4.00, 3.90, 3.00, 1.00])
+        tensor([8.15, 5.23, 2.80, 1.00])
 
     Args:
         vector_x (torch.Tensor): A sequence of shape (B, T).
         discount (float): The discount factor.
 
     Returns:
         The discounted cumulative sum of vectors.
@@ -107,15 +107,15 @@
             product.
         vector_b (torch.Tensor): The vector :math:`b` in the equation :math:`A x = b`.
         num_steps (int, optional): The number of steps to run the algorithm for. Defaults to 10.
         residual_tol (float, optional): The tolerance for the residual. Defaults to 1e-10.
         eps (float, optional): A small number to avoid dividing by zero. Defaults to 1e-6.
 
     Returns:
-        The vector :math:`x` in the equation :math:`A x = b`.
+        The vector x in the equation Ax=b.
     """
     vector_x = torch.zeros_like(vector_b)
     vector_r = vector_b - fisher_product(vector_x)
     vector_p = vector_r.clone()
     rdotr = torch.dot(vector_r, vector_r)
 
     for _ in range(num_steps):
```

### Comparing `omnisafe-0.4.0/omnisafe/utils/model.py` & `omnisafe-0.5.0b0/omnisafe/utils/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/utils/plotter.py` & `omnisafe-0.5.0b0/omnisafe/utils/plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,17 @@
         Args:
             sub_figures (np.ndarray): The subplots.
             data (list of DataFrame): The data to plot.
             xaxis (str, optional): The x-axis label. Defaults to 'Steps'.
             value (str, optional): The y-axis label. Defaults to 'Rewards'.
             condition (str, optional): The condition label. Defaults to 'Condition1'.
             smooth (int, optional): The smoothing window size. Defaults to 1.
-            **kwargs (Any): Additional arguments.
+
+        Keyword Args:
+            kwargs: Other keyword arguments for ``sns.lineplot``.
         """
         if smooth > 1:
             y = np.ones(smooth)
             for datum in data:
                 x = np.asarray(datum[value])
                 z = np.ones(len(x))
                 smoothed_x = np.convolve(x, y, 'same') / np.convolve(z, y, 'same')
```

### Comparing `omnisafe-0.4.0/omnisafe/utils/schedule.py` & `omnisafe-0.5.0b0/omnisafe/utils/schedule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright 2022 OmniSafe Team. All Rights Reserved.
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `omnisafe-0.4.0/omnisafe/utils/tools.py` & `omnisafe-0.5.0b0/omnisafe/utils/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -243,16 +243,16 @@
 
     Raises:
         AssertionError: If the ``yaml`` file is not found.
     """
     with open(path, encoding='utf-8') as file:
         try:
             kwargs = yaml.load(file, Loader=yaml.FullLoader)  # noqa: S506
-        except yaml.YAMLError as exc:
-            raise AssertionError(f'{path} error: {exc}') from exc
+        except FileNotFoundError as exc:
+            raise FileNotFoundError(f'{path} error: {exc}') from exc
 
     return kwargs
 
 
 def recursive_check_config(
     config: dict[str, Any],
     default_config: dict[str, Any],
```

### Comparing `omnisafe-0.4.0/omnisafe/version.py` & `omnisafe-0.5.0b0/omnisafe/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """OmniSafe: A comprehensive and reliable benchmark for safe reinforcement learning."""
 
-__version__ = '0.4.0'
+__version__ = '0.5.0b0'
 __license__ = 'Apache License, Version 2.0'
 __author__ = 'OmniSafe Contributors'
 __release__ = True
 
 if not __release__:
     import os
     import subprocess
```

### Comparing `omnisafe-0.4.0/omnisafe.egg-info/PKG-INFO` & `omnisafe-0.5.0b0/omnisafe.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: omnisafe
-Version: 0.4.0
+Version: 0.5.0b0
 Summary: A comprehensive and reliable benchmark for safe reinforcement learning.
 Author: OmniSafe Contributors
 License: Apache License, Version 2.0
-Project-URL: Homepage, https://github.com/OmniSafeAI/omnisafe
-Project-URL: Repository, https://github.com/OmniSafeAI/omnisafe
+Project-URL: Homepage, https://github.com/PKU-Alignment/omnisafe
+Project-URL: Repository, https://github.com/PKU-Alignment/omnisafe
 Project-URL: Documentation, https://omnisafe.readthedocs.io
-Project-URL: Bug Report, https://github.com/OmniSafeAI/omnisafe/issues
+Project-URL: Bug Report, https://github.com/PKU-Alignment/omnisafe/issues
 Keywords: Safe Reinforcement Learning,Reinforcement Learning,PyTorch
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -25,199 +25,265 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!-- markdownlint-disable first-line-h1 -->
 <!-- markdownlint-disable html -->
 
 <div align="center">
-  <img src="https://github.com/OmniSafeAI/omnisafe/raw/HEAD/images/logo.png" width="75%"/>
+  <img src="https://github.com/PKU-Alignment/omnisafe/raw/HEAD/images/logo.png" width="75%"/>
 </div>
 
 <div align="center">
 
-  [![Organization](https://img.shields.io/badge/Organization-PKU_MARL-blue.svg)](https://github.com/OmniSafeAI)
+  [![Organization](https://img.shields.io/badge/Organization-PKU--Alignment-blue)](https://github.com/PKU-Alignment)
   [![PyPI](https://img.shields.io/pypi/v/omnisafe?logo=pypi)](https://pypi.org/project/omnisafe)
-  [![tests](https://img.shields.io/github/actions/workflow/status/OmniSafeAI/omnisafe/test.yml?label=tests&logo=github)](https://github.com/OmniSafeAI/omnisafe/tree/HEAD/tests)
+  [![tests](https://img.shields.io/github/actions/workflow/status/PKU-Alignment/omnisafe/test.yml?label=tests&logo=github)](https://github.com/PKU-Alignment/omnisafe/tree/HEAD/tests)
   [![Documentation Status](https://img.shields.io/readthedocs/omnisafe?logo=readthedocs)](https://omnisafe.readthedocs.io)
   [![Downloads](https://static.pepy.tech/personalized-badge/omnisafe?period=total&left_color=grey&right_color=blue&left_text=downloads)](https://pepy.tech/project/omnisafe)
-  [![GitHub Repo Stars](https://img.shields.io/github/stars/OmniSafeAI/omnisafe?color=brightgreen&logo=github)](https://github.com/OmniSafeAI/OmniSafe/stargazers)
+  [![GitHub Repo Stars](https://img.shields.io/github/stars/PKU-Alignment/omnisafe?color=brightgreen&logo=github)](https://github.com/PKU-Alignment/OmniSafe/stargazers)
   [![codestyle](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-  [![License](https://img.shields.io/github/license/OmniSafeAI/OmniSafe?label=license)](#license)
-  [![CodeCov](https://img.shields.io/codecov/c/github/OmniSafeAI/omnisafe/main?logo=codecov)](https://app.codecov.io/gh/OmniSafeAI/omnisafe)
-  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/OmniSafeAI/omnisafe/)
+  [![License](https://img.shields.io/github/license/PKU-Alignment/OmniSafe?label=license)](#license)
+  [![CodeCov](https://img.shields.io/codecov/c/github/PKU-Alignment/omnisafe/main?logo=codecov)](https://app.codecov.io/gh/PKU-Alignment/omnisafe)
+  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/PKU-Alignment/omnisafe/)
 
 </div>
 
 <p align="center">
   <a href="https://omnisafe.readthedocs.io">Documentation</a> |
-  <a href="https://github.com/OmniSafeAI/omnisafe#implemented-algorithms">Implemented Algorithms</a> |
-  <a href="https://github.com/OmniSafeAI/omnisafe#installation">Installation</a> |
-  <a href="https://github.com/OmniSafeAI/omnisafe#getting-started">Getting Started</a> |
-  <a href="https://github.com/OmniSafeAI/omnisafe#license">License</a>
+  <a href="https://github.com/PKU-Alignment/omnisafe#implemented-algorithms">Implemented Algorithms</a> |
+  <a href="https://github.com/PKU-Alignment/omnisafe#installation">Installation</a> |
+  <a href="https://github.com/PKU-Alignment/omnisafe#getting-started">Getting Started</a> |
+  <a href="https://github.com/PKU-Alignment/omnisafe#license">License</a>
 </p>
 
 --------------------------------------------------------------------------------
 
-**This library is currently under heavy development - if you have suggestions on the API or use-cases you'd like to be covered, please open a GitHub issue or reach out. We'd love to hear about how you're using the library.**
+OmniSafe is an infrastructural framework designed to accelerate safe reinforcement learning (RL) research.
+It provides a comprehensive and reliable benchmark for safe RL algorithms, and also an out-of-box modular toolkit for researchers.
+SafeRL intends to develop algorithms that minimize the risk of unintended harm or unsafe behavior.
 
-OmniSafe is an infrastructural framework designed to accelerate safe reinforcement learning (RL) research by providing a comprehensive and reliable benchmark for safe RL algorithms.
-The field of RL has great potential to benefit the society, and safety concerns are a significant issue, and RL algorithms have raised concerns about unintended harm or unsafe behavior.
-Safe RL intends to develop algorithms that minimize the risk of unintended harm or unsafe behavior, but there is currently a lack of commonly recognized safe RL algorithm benchmarks.
-
-OmniSafe addresses these issues by providing more than 40 experimentally validated algorithms and a sound and efficient simulation environment.
-Researchers can use OmniSafe to conduct experiments and verify their ideas, ensuring consistency and enabling more efficient development of safe RL algorithms.
-By using OmniSafe as a benchmark, researchers can evaluate the performance of their own safe RL algorithms and contribute to the advancement of safe RL research.
+OmniSafe stands as the inaugural unified learning framework in the realm of safe reinforcement learning, aiming to foster the Growth of SafeRL Learning Community.
+The key features of OmniSafe:
+
+- **Highly Modular Framework.** OmniSafe presents a highly modular framework, incorporating an extensive collection of tens of algorithms tailored for safe reinforcement learning across diverse domains. This framework is versatile due to its abstraction of various algorithm types and well-designed API, using the Adapter and Wrapper design components to bridge gaps and enable seamless interactions between different components. This design allows for easy extension and customization, making it a powerful tool for developers working with different types of algorithms.
+
+- **High-performance parallel computing acceleration.** By harnessing the capabilities of `torch.distributed`, OmniSafe accelerates the learning process of algorithms
+with process parallelism. This enables OmniSafe not only to support environment-level asynchronous parallelism but also incorporates agent asynchronous learning. This methodology bolsters training stability and expedites the training process via the deployment of a parallel exploration mechanism. The integration of agent asynchronous learning in OmniSafe underscores its commitment to providing a versatile and robust platform for advancing SafeRL research.
+
+- **Out-of-box toolkits.** OmniSafe offers customizable toolkits for tasks like training, benchmarking, analyzing, and rendering. [Tutorials](https://github.com/PKU-Alignment/omnisafe#getting-started) and user-friendly [APIs](https://omnisafe.readthedocs.io/en/latest/baserlapi/on_policy.html) make it easy for beginners and average users, while advanced researchers can enhance their efficiency without complex code.
+
+![Train video](https://github-production-user-asset-6210df.s3.amazonaws.com/73586554/237139607-d1e6f413-aa2c-4f68-b8ee-08a4361493a0.gif)
 
 --------------------------------------------------------------------------------
 
 ### Table of Contents  <!-- omit in toc --> <!-- markdownlint-disable heading-increment -->
 
-- [Implemented Algorithms](#implemented-algorithms)
-  - [Latest SafeRL Papers](#latest-saferl-papers)
-  - [List of Algorithms](#list-of-algorithms)
-    - [On-Policy Safe](#on-policy-safe)
-    - [Off-Policy Safe](#off-policy-safe)
-    - [Model-Based Safe](#model-based-safe)
-    - [Offline Safe](#offline-safe)
-    - [Others](#others)
-- [Installation](#installation)
-  - [Prerequisites](#prerequisites)
+- [Quick Start](#quick-start)
+  - [Installation](#installation)
+    - [Prerequisites](#prerequisites)
     - [Install from source](#install-from-source)
     - [Install from PyPI](#install-from-pypi)
+- [Implemented Algorithms](#implemented-algorithms)
   - [Examples](#examples)
+    - [Algorithms Registry](#algorithms-registry)
+    - [Supported Environments](#supported-environments)
     - [Try with CLI](#try-with-cli)
 - [Getting Started](#getting-started)
   - [Important Hints](#important-hints)
   - [Quickstart: Colab on the Cloud](#quickstart-colab-on-the-cloud)
 - [Changelog](#changelog)
+- [Citing OmniSafe](#citing-omnisafe)
 - [The OmniSafe Team](#the-omnisafe-team)
 - [License](#license)
 
 --------------------------------------------------------------------------------
 
-## Implemented Algorithms
+## Quick Start
+
+### Installation
+
+#### Prerequisites
+
+OmniSafe requires Python 3.8+ and PyTorch 1.10+.
+
+> We support and test for Python 3.8, 3.9, 3.10 on Linux. Meanwhile, we also support M1 and M2 versions of macOS. We will accept PRs related to Windows, but do not officially support it.
+
+#### Install from source
+
+```bash
+# Clone the repo
+git clone https://github.com/PKU-Alignment/omnisafe.git
+cd omnisafe
+
+# Create a conda environment
+conda env create --file conda-recipe.yaml
+conda activate omnisafe
+
+# Install omnisafe
+pip install -e .
+```
+
+#### Install from PyPI
+
+OmniSafe is hosted in [![PyPI](https://img.shields.io/pypi/v/omnisafe?label=pypi&logo=pypi)](https://pypi.org/project/omnisafe) / ![Status](https://img.shields.io/pypi/status/omnisafe?label=status).
+
+```bash
+pip install omnisafe
+```
 
-The supported interface algorithms currently include:
+## Implemented Algorithms
 
-### Latest SafeRL Papers
+<details>
+<summary><b><big>Latest SafeRL Papers</big></b></summary>
 
 - **[AAAI 2023]** Augmented Proximal Policy Optimization for Safe Reinforcement Learning (APPO)
 - **[NeurIPS 2022]** [Constrained Update Projection Approach to Safe Policy Optimization (CUP)](https://arxiv.org/abs/2209.07089)
 - **[NeurIPS 2022]** [Effects of Safety State Augmentation on Safe Exploration (Simmer)](https://arxiv.org/abs/2206.02675)
 - **[NeurIPS 2022]** [Model-based Safe Deep Reinforcement Learning via a Constrained Proximal Policy Optimization Algorithm](https://arxiv.org/abs/2210.07573)
 - **[ICML 2022]** [Sauté RL: Almost Surely Safe Reinforcement Learning Using State Augmentation (SauteRL)](https://arxiv.org/abs/2202.06558)
-- **[ICML 2022]** [Constrained Variational Policy Optimization for Safe Reinforcement Learning (CVPO)](https://arxiv.org/abs/2201.11927)
 - **[IJCAI 2022]** [Penalized Proximal Policy Optimization for Safe Reinforcement Learning](https://arxiv.org/abs/2205.11814)
-- **[ICLR 2022]** [Constrained Policy Optimization via Bayesian World Models (LA-MBDA)](https://arxiv.org/abs/2201.09802)
 - **[AAAI 2022]** [Conservative and Adaptive Penalty for Model-Based Safe Reinforcement Learning (CAP)](https://arxiv.org/abs/2112.07701)
 
-### List of Algorithms
+</details>
+
+<details>
+<summary><b><big>List of Algorithms</big></b></summary>
 
-#### On-Policy Safe
+<summary><b><big>On Policy SafeRL</big></b></summary>
 
-- [X] [The Lagrange version of PPO (PPO-Lag)](https://cdn.openai.com/safexp-short.pdf)
-- [X] [The Lagrange version of TRPO (TRPO-Lag)](https://cdn.openai.com/safexp-short.pdf)
-- [X] **[ICML 2017]** [Constrained Policy Optimization (CPO)](https://proceedings.mlr.press/v70/achiam17a)
-- [X] **[ICLR 2019]** [Reward Constrained Policy Optimization (RCPO)](https://openreview.net/forum?id=SkfrvsA9FX)
-- [X] **[ICML 2020]** [Responsive Safety in Reinforcement Learning by PID Lagrangian Methods (PID-Lag)](https://arxiv.org/abs/2007.03964)
-- [X] **[NeurIPS 2020]** [First Order Constrained Optimization in Policy Space (FOCOPS)](https://arxiv.org/abs/2002.06506)
-- [X] **[AAAI 2020]** [IPO: Interior-point Policy Optimization under Constraints (IPO)](https://arxiv.org/abs/1910.09615)
-- [X] **[ICLR 2020]** [Projection-Based Constrained Policy Optimization (PCPO)](https://openreview.net/forum?id=rke3TJrtPS)
-- [X] **[ICML 2021]** [CRPO: A New Approach for Safe Reinforcement Learning with Convergence Guarantee](https://arxiv.org/abs/2011.05869)
+- [x] [The Lagrange version of PPO (PPO-Lag)](https://cdn.openai.com/safexp-short.pdf)
+- [x] [The Lagrange version of TRPO (TRPO-Lag)](https://cdn.openai.com/safexp-short.pdf)
+- [x] **[ICML 2017]** [Constrained Policy Optimization (CPO)](https://proceedings.mlr.press/v70/achiam17a)
+- [x] **[ICLR 2019]** [Reward Constrained Policy Optimization (RCPO)](https://openreview.net/forum?id=SkfrvsA9FX)
+- [x] **[ICML 2020]** [Responsive Safety in Reinforcement Learning by PID Lagrangian Methods (PID-Lag)](https://arxiv.org/abs/2007.03964)
+- [x] **[NeurIPS 2020]** [First Order Constrained Optimization in Policy Space (FOCOPS)](https://arxiv.org/abs/2002.06506)
+- [x] **[AAAI 2020]** [IPO: Interior-point Policy Optimization under Constraints (IPO)](https://arxiv.org/abs/1910.09615)
+- [x] **[ICLR 2020]** [Projection-Based Constrained Policy Optimization (PCPO)](https://openreview.net/forum?id=rke3TJrtPS)
+- [x] **[ICML 2021]** [CRPO: A New Approach for Safe Reinforcement Learning with Convergence Guarantee](https://arxiv.org/abs/2011.05869)
 - [x] **[IJCAI 2022]** [Penalized Proximal Policy Optimization for Safe Reinforcement Learning(P3O)](https://arxiv.org/pdf/2205.11814.pdf)
 
-#### Off-Policy Safe
+<summary><b><big>Off Policy SafeRL</big></b></summary>
 
-- [X] The Lagrange version of TD3 (TD3-Lag)
-- [X] The Lagrange version of DDPG (DDPG-Lag)
-- [X] The Lagrange version of SAC (SAC-Lag)
-- [X] **[ICML 2019]** [Lyapunov-based Safe Policy Optimization for Continuous Control (SDDPG)](https://arxiv.org/abs/1901.10031)
-- [X] **[ICML 2019]** [Lyapunov-based Safe Policy Optimization for Continuous Control (SDDPG-modular)](https://arxiv.org/abs/1901.10031)
-- [ ] **[ICML 2022]** [Constrained Variational Policy Optimization for Safe Reinforcement Learning (CVPO)](https://arxiv.org/abs/2201.11927)
+- **[Preprint 2019]** [The Lagrangian version of DDPG (DDPGLag)](https://cdn.openai.com/safexp-short.pdf)
+- **[Preprint 2019]** [The Lagrangian version of TD3 (TD3Lag)](https://cdn.openai.com/safexp-short.pdf)
+- **[Preprint 2019]** [The Lagrangian version of SAC (SACLag)](https://cdn.openai.com/safexp-short.pdf)
+- **[ICML 2020]** [Responsive Safety in Reinforcement Learning by PID Lagrangian Methods (DDPGPID)](https://arxiv.org/abs/2007.03964)
+- **[ICML 2020]** [Responsive Safety in Reinforcement Learning by PID Lagrangian Methods (TD3PID)](https://arxiv.org/abs/2007.03964)
+- **[ICML 2020]** [Responsive Safety in Reinforcement Learning by PID Lagrangian Methods (SACPID)](https://arxiv.org/abs/2007.03964)
 
-#### Model-Based Safe
+<summary><b><big>Model-Based SafeRL</big></b></summary>
 
 - [ ] **[NeurIPS 2021]** [Safe Reinforcement Learning by Imagining the Near Future (SMBPO)](https://arxiv.org/abs/2202.07789)
-- [X] **[CoRL 2021 (Oral)]** [Learning Off-Policy with Online Planning (SafeLOOP)](https://arxiv.org/abs/2008.10066)
-- [X] **[AAAI 2022]** [Conservative and Adaptive Penalty for Model-Based Safe Reinforcement Learning (CAP)](https://arxiv.org/abs/2112.07701)
-- [X] **[NeurIPS 2022]** [Model-based Safe Deep Reinforcement Learning via a Constrained Proximal Policy Optimization Algorithm](https://arxiv.org/abs/2210.07573)
+- [x] **[CoRL 2021 (Oral)]** [Learning Off-Policy with Online Planning (SafeLOOP)](https://arxiv.org/abs/2008.10066)
+- [x] **[AAAI 2022]** [Conservative and Adaptive Penalty for Model-Based Safe Reinforcement Learning (CAP)](https://arxiv.org/abs/2112.07701)
+- [x] **[NeurIPS 2022]** [Model-based Safe Deep Reinforcement Learning via a Constrained Proximal Policy Optimization Algorithm](https://arxiv.org/abs/2210.07573)
 - [ ] **[ICLR 2022]** [Constrained Policy Optimization via Bayesian World Models (LA-MBDA)](https://arxiv.org/abs/2201.09802)
-- [X] **[ICML 2022 Workshop]** [Constrained Model-based Reinforcement Learning with Robust Cross-Entropy Method (RCE)](https://arxiv.org/abs/2010.07968)
-- [X] **[NeurIPS 2018]** [Constrained Cross-Entropy Method for Safe Reinforcement Learning (CCE)](https://proceedings.neurips.cc/paper/2018/hash/34ffeb359a192eb8174b6854643cc046-Abstract.html)
+- [x] **[ICML 2022 Workshop]** [Constrained Model-based Reinforcement Learning with Robust Cross-Entropy Method (RCE)](https://arxiv.org/abs/2010.07968)
+- [x] **[NeurIPS 2018]** [Constrained Cross-Entropy Method for Safe Reinforcement Learning (CCE)](https://proceedings.neurips.cc/paper/2018/hash/34ffeb359a192eb8174b6854643cc046-Abstract.html)
 
-#### Offline Safe
+<summary><b><big>Offline SafeRL</big></b></summary>
 
-- [X] [The Lagrange version of BCQ (BCQ-Lag)](https://arxiv.org/abs/1812.02900)
-- [X] [The Constrained version of CRR (C-CRR)](https://proceedings.neurips.cc/paper/2020/hash/588cb956d6bbe67078f29f8de420a13d-Abstract.html)
+- [x] [The Lagrange version of BCQ (BCQ-Lag)](https://arxiv.org/abs/1812.02900)
+- [x] [The Constrained version of CRR (C-CRR)](https://proceedings.neurips.cc/paper/2020/hash/588cb956d6bbe67078f29f8de420a13d-Abstract.html)
 - [ ] **[AAAI 2022]** [Constraints Penalized Q-learning for Safe Offline Reinforcement Learning CPQ](https://arxiv.org/abs/2107.09003)
-- [ ] **[ICLR 2022 (Spotlight)]** [COptiDICE: Offline Constrained Reinforcement Learning via Stationary Distribution Correction Estimation](https://arxiv.org/abs/2204.08957?context=cs.AI)
+- [x] **[ICLR 2022 (Spotlight)]** [COptiDICE: Offline Constrained Reinforcement Learning via Stationary Distribution Correction Estimation](https://arxiv.org/abs/2204.08957?context=cs.AI)
 - [ ] **[ICML 2022]** [Constrained Offline Policy Optimization (COPO)](https://proceedings.mlr.press/v162/polosky22a.html)
 
-#### Others
+<summary><b><big>Others</big></b></summary>
 
-- [X] [Safe Exploration in Continuous Action Spaces (Safety Layer)](https://arxiv.org/abs/1801.08757)
 - [ ] **[RA-L 2021]** [Recovery RL: Safe Reinforcement Learning with Learned Recovery Zones](https://arxiv.org/abs/2010.15920)
-- [X] **[ICML 2022]** [Sauté RL: Almost Surely Safe Reinforcement Learning Using State Augmentation (SauteRL)](https://arxiv.org/abs/2202.06558)
-- [X] **[NeurIPS 2022]** [Effects of Safety State Augmentation on Safe Exploration](https://arxiv.org/abs/2206.02675)
-
---------------------------------------------------------------------------------
-
-## Installation
-
-### Prerequisites
-
-OmniSafe requires Python 3.8+ and PyTorch 1.10+.
-
-> We support and test for Python 3.8, 3.9, 3.10 on Linux. Meanwhile, we also support M1 and M2 versions of macOS. We will accept PRs related to Windows, but do not officially support it.
-
-#### Install from source
-
-```bash
-# Clone the repo
-git clone https://github.com/OmniSafeAI/omnisafe
-cd omnisafe
+- [x] **[ICML 2022]** [Sauté RL: Almost Surely Safe Reinforcement Learning Using State Augmentation (SauteRL)](https://arxiv.org/abs/2202.06558)
+- [x] **[NeurIPS 2022]** [Effects of Safety State Augmentation on Safe Exploration](https://arxiv.org/abs/2206.02675)
 
-# Create a conda environment
-conda env create --file conda-recipe.yaml
-conda activate omnisafe
+</details>
 
-# Install omnisafe
-pip install -e .
-```
-
-#### Install from PyPI
-
-OmniSafe is hosted in [![PyPI](https://img.shields.io/pypi/v/omnisafe?label=pypi&logo=pypi)](https://pypi.org/project/omnisafe) / ![Status](https://img.shields.io/pypi/status/omnisafe?label=status).
-
-```bash
-pip install omnisafe
-```
+--------------------------------------------------------------------------------
 
 ### Examples
 
 ```bash
 cd examples
-python train_policy.py --algo PPOLag --env-id SafetyPointGoal1-v0 --parallel 1 --total-steps 1024000 --device cpu --vector-env-nums 1 --torch-threads 1
+python train_policy.py --algo PPOLag --env-id SafetyPointGoal1-v0 --parallel 1 --total-steps 10000000 --device cpu --vector-env-nums 1 --torch-threads 1
 ```
 
-**algo:**
-| Type              | Name                                                             |
-| ----------------- | ---------------------------------------------------------------- |
-| `Base-On-Policy`  | `PolicyGradient, PPO`<br> `NaturalPG, TRPO`                      |
-| `Base-Off-Policy` | `DDPG, TD3, SAC`                                                 |
-| `Naive Lagrange`  | `RCPO, PPOLag, TRPOLag`<br> `DDPGLag, TD3Lag, SACLag`            |
-| `PID Lagrange`    | `CPPOPid, TRPOPid`                                               |
-| `First Order`     | `FOCOPS, CUP`                                                    |
-| `Second Order`    | `SDDPG, CPO, PCPO`                                               |
-| `Saute RL`        | `PPOSaute, PPOLagSaute`                                          |
-| `Simmer RL`       | `PPOSimmerQ, PPOSimmerPid` <br> `PPOLagSimmerQ, PPOLagSimmerPid` |
-| `EarlyTerminated` | `PPOEarlyTerminated` <br> `PPOLagEarlyTerminated`                |
-| `Model-Based`     | `CAP, MBPPOLag, SafeLOOP`                                        |
+#### Algorithms Registry
 
-**env-id:** Environment id in [Safety Gymnasium](https://www.safety-gymnasium.com/), here a list of envs that safety-gymnasium supports.
+<table>
+<thead>
+  <tr>
+    <th>Domains</th>
+    <th>Types</th>
+    <th>Algorithms Registry</th>
+  </tr>
+</thead>
+<tbody>
+  <tr>
+    <td rowspan="5">On Policy</td>
+    <td rowspan="2">Primal Dual</td>
+    <td>TRPOLag; PPOLag; PDO; RCPO</td>
+  </tr>
+  <tr>
+    <td>TRPOPID; CPPOPID</td>
+  </tr>
+  <tr>
+    <td>Convex Optimization</td>
+    <td><span style="font-weight:400;font-style:normal">CPO; PCPO; </span>FOCOPS; CUP</td>
+  </tr>
+  <tr>
+    <td>Penalty Function</td>
+    <td>IPO; P3O</td>
+  </tr>
+  <tr>
+    <td>Primal</td>
+    <td>OnCRPO</td>
+  </tr>
+  <tr>
+    <td rowspan="2">Off Policy</td>
+    <td rowspan="2">Primal-Dual</td>
+    <td>DDPGLag; TD3Lag; SACLag</td>
+  </tr>
+  <tr>
+    <td><span style="font-weight:400;font-style:normal">DDPGPID; TD3PID; SACPID</span></td>
+  </tr>
+  <tr>
+    <td rowspan="2">Model-based</td>
+    <td>Online Plan</td>
+    <td>SafeLOOP; CCEPETS; RCEPETS</td>
+  </tr>
+  <tr>
+    <td><span style="font-weight:400;font-style:normal">Pessimistic Estimate</span></td>
+    <td>CAPPETS</td>
+  </tr>
+    <td rowspan="2">Offline</td>
+    <td>Q-Learning Based</td>
+    <td>BCQLag; C-CRR</td>
+  </tr>
+  <tr>
+    <td>DICE Based</td>
+    <td>COptDICE</td>
+  </tr>
+  <tr>
+    <td rowspan="3">Other Formulation MDP</td>
+    <td>ET-MDP</td>
+    <td><span style="font-weight:400;font-style:normal">PPO</span>EarlyTerminated; TRPOEarlyTerminated</td>
+  </tr>
+  <tr>
+    <td>SauteRL</td>
+    <td>PPOSaute; TRPOSaute</td>
+  </tr>
+  <tr>
+    <td>SimmerRL</td>
+    <td><span style="font-weight:400;font-style:normal">PPOSimmerPID; TRPOSimmerPID</span></td>
+  </tr>
+</tbody>
+</table>
+
+#### Supported Environments
+
+Here is a list of environments that [Safety-Gymnasium](https://www.safety-gymnasium.com) supports:
 
 <table border="1">
 <thead>
   <tr>
     <th>Category</th>
     <th>Task</th>
     <th>Agent</th>
@@ -245,72 +311,91 @@
     <td>Velocity</td>
     <td>HalfCheetah, Hopper, Swimmer, Walker2d, Ant, Humanoid</td>
     <td>SafetyHumanoidVelocity-v1</td>
   </tr>
 </tbody>
 </table>
 
-More information about environments, please refer to [Safety Gymnasium](https://www.safety-gymnasium.com/)
-
-**parallel:** `Number of parallels`
+For more information about environments, please refer to [Safety-Gymnasium](https://www.safety-gymnasium.com).
 
 #### Try with CLI
 
-**A video example**
-
-![Segmentfault](https://github.com/OmniSafeAI/omnisafe/blob/main/images/CLI_example.svg)
-
 ```bash
 pip install omnisafe
 
-omnisafe --help # Ask for help
+omnisafe --help  # Ask for help
 
-omnisafe benchmark --help # The benchmark also can be replaced with 'eval', 'train', 'train-config'
+omnisafe benchmark --help  # The benchmark also can be replaced with 'eval', 'train', 'train-config'
 
-# Quick benchmarking for your research, just specify: 1.exp_name, 2.num_pool(how much processes are concurrent), 3.path of the config file(refer to omnisafe/examples/benchmarks for format)
-omnisafe benchmark test_benchmark 2 ./saved_source/benchmark_config.yaml
-
-# Quick evaluating and rendering your trained policy, just specify: 1.path of algorithm which you trained
-omnisafe eval ./saved_source/PPO-{SafetyPointGoal1-v0} --num-episode 1
+# Quick benchmarking for your research, just specify:
+# 1. exp_name
+# 2. num_pool(how much processes are concurrent)
+# 3. path of the config file (refer to omnisafe/examples/benchmarks for format)
+
+# Here we provide an exampe in ./tests/saved_source.
+# And you can set your benchmark_config.yaml by following it
+omnisafe benchmark test_benchmark 2 ./tests/saved_source/benchmark_config.yaml
+
+# Quick evaluating and rendering your trained policy, just specify:
+# 1. path of algorithm which you trained
+omnisafe eval ./tests/saved_source/PPO-{SafetyPointGoal1-v0} --num-episode 1
 
 # Quick training some algorithms to validate your thoughts
 # Note: use `key1:key2`, your can select key of hyperparameters which are recursively contained, and use `--custom-cfgs`, you can add custom cfgs via CLI
 omnisafe train --algo PPO --total-steps 2048 --vector-env-nums 1 --custom-cfgs algo_cfgs:steps_per_epoch --custom-cfgs 1024
 
 # Quick training some algorithms via a saved config file, the format is as same as default format
-omnisafe train-config ./saved_source/train_config.yaml
+omnisafe train-config ./tests/saved_source/train_config.yaml
 ```
 
 --------------------------------------------------------------------------------
 
 ## Getting Started
 
 ### Important Hints
 
-- `train_cfgs:torch_threads` is especially important for training speed, and is varying with users' machine, this value shouldn't be too small or too large.
+We have provided benchmark results for various algorithms, including on-policy, off-policy, model-based, and offline approaches, along with parameter tuning analysis. Please refer to the following:
+
+- [On-Policy](./benchmarks/on-policy/)
+- [Off-Policy](./benchmarks/off-policy/)
+- [Model-based](./benchmarks/model-based/)
+- [Offline](./benchmarks/offline/)
 
 ### Quickstart: Colab on the Cloud
 
-Explore OmniSafe easily and quickly through a series of colab notebooks:
+Explore OmniSafe easily and quickly through a series of Google Colab notebooks:
 
-- [Getting Started](https://colab.research.google.com/github/OmniSafeAI/omnisafe/blob/main/tutorials/English/1.Getting_Started.ipynb) Introduce the basic usage of OmniSafe so that users can quickly hand on it.
-- [CLI Command](https://colab.research.google.com/github/OmniSafeAI/omnisafe/blob/main/tutorials/English/2.CLI_Command.ipynb) Introduce how to use the CLI tool of OmniSafe.
+- [Getting Started](https://colab.research.google.com/github/PKU-Alignment/omnisafe/blob/main/tutorials/English/1.Getting_Started.ipynb) Introduce the basic usage of OmniSafe so that users can quickly hand it.
+- [CLI Command](https://colab.research.google.com/github/PKU-Alignment/omnisafe/blob/main/tutorials/English/2.CLI_Command.ipynb) Introduce how to use the CLI tool of OmniSafe.
 
 We take great pleasure in collaborating with our users to create tutorials in various languages.
 Please refer to our list of currently supported languages.
 If you are interested in translating the tutorial into a new language or improving an existing version, kindly submit a PR to us.
 
 --------------------------------------------------------------------------------
 
 ## Changelog
 
-See [CHANGELOG.md](https://github.com/OmniSafeAI/omnisafe/blob/main/CHANGELOG.md).
+See [CHANGELOG.md](https://github.com/PKU-Alignment/omnisafe/blob/main/CHANGELOG.md).
+
+## Citing OmniSafe
+
+If you find OmniSafe useful or use OmniSafe in your research, please cite it in your publications.
+
+```bibtex
+@article{omnisafe,
+  title   = {OmniSafe: An Infrastructure for Accelerating Safe Reinforcement Learning Research},
+  author  = {Jiaming Ji, Jiayi Zhou, Borong Zhang, Juntao Dai, Xuehai Pan, Ruiyang Sun, Weidong Huang, Yiran Geng, Mickel Liu, Yaodong Yang},
+  journal = {arXiv preprint arXiv:2305.09304},
+  year    = {2023}
+}
+```
 
 ## The OmniSafe Team
 
-OmniSafe is mainly developed by the SafeRL research team directed by Prof. [Yaodong Yang](https://github.com/orgs/OmniSafeAI/people/PKU-YYang).
+OmniSafe is mainly developed by the SafeRL research team directed by Prof. [Yaodong Yang](https://www.yangyaodong.com/).
 Our SafeRL research team members include [Borong Zhang](https://github.com/muchvo), [Jiayi Zhou](https://github.com/Gaiejj), [JTao Dai](https://github.com/calico-1226), [Weidong Huang](https://github.com/hdadong), [Ruiyang Sun](https://github.com/rockmagma02), [Xuehai Pan](https://github.com/XuehaiPan) and [Jiaming Ji](https://github.com/zmsn-2077).
-If you have any questions in the process of using omnisafe, don't hesitate to ask your questions on [the GitHub issue page](https://github.com/OmniSafeAI/omnisafe/issues/new/choose), we will reply to you in 2-3 working days.
+If you have any questions in the process of using OmniSafe, don't hesitate to ask your questions on [the GitHub issue page](https://github.com/PKU-Alignment/omnisafe/issues/new/choose), we will reply to you in 2-3 working days.
 
 ## License
 
 OmniSafe is released under Apache License 2.0.
```

#### html2text {}

```diff
@@ -1,217 +1,241 @@
-Metadata-Version: 2.1 Name: omnisafe Version: 0.4.0 Summary: A comprehensive
+Metadata-Version: 2.1 Name: omnisafe Version: 0.5.0b0 Summary: A comprehensive
 and reliable benchmark for safe reinforcement learning. Author: OmniSafe
 Contributors License: Apache License, Version 2.0 Project-URL: Homepage, https:
-//github.com/OmniSafeAI/omnisafe Project-URL: Repository, https://github.com/
-OmniSafeAI/omnisafe Project-URL: Documentation, https://omnisafe.readthedocs.io
-Project-URL: Bug Report, https://github.com/OmniSafeAI/omnisafe/issues
-Keywords: Safe Reinforcement Learning,Reinforcement Learning,PyTorch
-Classifier: Development Status :: 4 - Beta Classifier: License :: OSI Approved
-:: Apache Software License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Intended
-Audience :: Science/Research Classifier: Topic :: Scientific/Engineering ::
-Artificial Intelligence Classifier: Topic :: Software Development :: Libraries
-:: Python Modules Requires-Python: >=3.8 Description-Content-Type: text/
-markdown Provides-Extra: lint Provides-Extra: test License-File: LICENSE
-       [https://github.com/OmniSafeAI/omnisafe/raw/HEAD/images/logo.png]
-[![Organization](https://img.shields.io/badge/Organization-PKU_MARL-blue.svg)]
-    (https://github.com/OmniSafeAI) [![PyPI](https://img.shields.io/pypi/v/
-  omnisafe?logo=pypi)](https://pypi.org/project/omnisafe) [![tests](https://
-      img.shields.io/github/actions/workflow/status/OmniSafeAI/omnisafe/
-test.yml?label=tests&logo=github)](https://github.com/OmniSafeAI/omnisafe/tree/
-   HEAD/tests) [![Documentation Status](https://img.shields.io/readthedocs/
+//github.com/PKU-Alignment/omnisafe Project-URL: Repository, https://
+github.com/PKU-Alignment/omnisafe Project-URL: Documentation, https://
+omnisafe.readthedocs.io Project-URL: Bug Report, https://github.com/PKU-
+Alignment/omnisafe/issues Keywords: Safe Reinforcement Learning,Reinforcement
+Learning,PyTorch Classifier: Development Status :: 4 - Beta Classifier: License
+:: OSI Approved :: Apache Software License Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Intended Audience :: Science/Research Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Requires-Python: >=3.8 Description-
+Content-Type: text/markdown Provides-Extra: lint Provides-Extra: test License-
+File: LICENSE
+     [https://github.com/PKU-Alignment/omnisafe/raw/HEAD/images/logo.png]
+  [![Organization](https://img.shields.io/badge/Organization-PKU--Alignment-
+blue)](https://github.com/PKU-Alignment) [![PyPI](https://img.shields.io/pypi/
+ v/omnisafe?logo=pypi)](https://pypi.org/project/omnisafe) [![tests](https://
+     img.shields.io/github/actions/workflow/status/PKU-Alignment/omnisafe/
+ test.yml?label=tests&logo=github)](https://github.com/PKU-Alignment/omnisafe/
+ tree/HEAD/tests) [![Documentation Status](https://img.shields.io/readthedocs/
   omnisafe?logo=readthedocs)](https://omnisafe.readthedocs.io) [![Downloads]
                  (https://static.pepy.tech/personalized-badge/
  omnisafe?period=total&left_color=grey&right_color=blue&left_text=downloads)]
       (https://pepy.tech/project/omnisafe) [![GitHub Repo Stars](https://
-img.shields.io/github/stars/OmniSafeAI/omnisafe?color=brightgreen&logo=github)]
-  (https://github.com/OmniSafeAI/OmniSafe/stargazers) [![codestyle](https://
- img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/
-     black) [![License](https://img.shields.io/github/license/OmniSafeAI/
-OmniSafe?label=license)](#license) [![CodeCov](https://img.shields.io/codecov/
-  c/github/OmniSafeAI/omnisafe/main?logo=codecov)](https://app.codecov.io/gh/
-   OmniSafeAI/omnisafe) [![Open In Colab](https://colab.research.google.com/
- assets/colab-badge.svg)](https://colab.research.google.com/github/OmniSafeAI/
-                                  omnisafe/)
+                  img.shields.io/github/stars/PKU-Alignment/
+  omnisafe?color=brightgreen&logo=github)](https://github.com/PKU-Alignment/
+ OmniSafe/stargazers) [![codestyle](https://img.shields.io/badge/code%20style-
+     black-000000.svg)](https://github.com/psf/black) [![License](https://
+img.shields.io/github/license/PKU-Alignment/OmniSafe?label=license)](#license)
+  [![CodeCov](https://img.shields.io/codecov/c/github/PKU-Alignment/omnisafe/
+ main?logo=codecov)](https://app.codecov.io/gh/PKU-Alignment/omnisafe) [![Open
+ In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
+           colab.research.google.com/github/PKU-Alignment/omnisafe/)
    _D_o_c_u_m_e_n_t_a_t_i_o_n | _I_m_p_l_e_m_e_n_t_e_d_ _A_l_g_o_r_i_t_h_m_s | _I_n_s_t_a_l_l_a_t_i_o_n | _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d |
                                     _L_i_c_e_n_s_e
 -------------------------------------------------------------------------------
-- **This library is currently under heavy development - if you have suggestions
-on the API or use-cases you'd like to be covered, please open a GitHub issue or
-reach out. We'd love to hear about how you're using the library.** OmniSafe is
-an infrastructural framework designed to accelerate safe reinforcement learning
-(RL) research by providing a comprehensive and reliable benchmark for safe RL
-algorithms. The field of RL has great potential to benefit the society, and
-safety concerns are a significant issue, and RL algorithms have raised concerns
-about unintended harm or unsafe behavior. Safe RL intends to develop algorithms
-that minimize the risk of unintended harm or unsafe behavior, but there is
-currently a lack of commonly recognized safe RL algorithm benchmarks. OmniSafe
-addresses these issues by providing more than 40 experimentally validated
-algorithms and a sound and efficient simulation environment. Researchers can
-use OmniSafe to conduct experiments and verify their ideas, ensuring
-consistency and enabling more efficient development of safe RL algorithms. By
-using OmniSafe as a benchmark, researchers can evaluate the performance of
-their own safe RL algorithms and contribute to the advancement of safe RL
-research. ---------------------------------------------------------------------
------------ ### Table of Contents - [Implemented Algorithms](#implemented-
-algorithms) - [Latest SafeRL Papers](#latest-saferl-papers) - [List of
-Algorithms](#list-of-algorithms) - [On-Policy Safe](#on-policy-safe) - [Off-
-Policy Safe](#off-policy-safe) - [Model-Based Safe](#model-based-safe) -
-[Offline Safe](#offline-safe) - [Others](#others) - [Installation]
-(#installation) - [Prerequisites](#prerequisites) - [Install from source]
-(#install-from-source) - [Install from PyPI](#install-from-pypi) - [Examples]
-(#examples) - [Try with CLI](#try-with-cli) - [Getting Started](#getting-
-started) - [Important Hints](#important-hints) - [Quickstart: Colab on the
-Cloud](#quickstart-colab-on-the-cloud) - [Changelog](#changelog) - [The
-OmniSafe Team](#the-omnisafe-team) - [License](#license) ----------------------
----------------------------------------------------------- ## Implemented
-Algorithms The supported interface algorithms currently include: ### Latest
-SafeRL Papers - **[AAAI 2023]** Augmented Proximal Policy Optimization for Safe
-Reinforcement Learning (APPO) - **[NeurIPS 2022]** [Constrained Update
-Projection Approach to Safe Policy Optimization (CUP)](https://arxiv.org/abs/
-2209.07089) - **[NeurIPS 2022]** [Effects of Safety State Augmentation on Safe
-Exploration (Simmer)](https://arxiv.org/abs/2206.02675) - **[NeurIPS 2022]**
-[Model-based Safe Deep Reinforcement Learning via a Constrained Proximal Policy
-Optimization Algorithm](https://arxiv.org/abs/2210.07573) - **[ICML 2022]**
-[SautÃ© RL: Almost Surely Safe Reinforcement Learning Using State Augmentation
-(SauteRL)](https://arxiv.org/abs/2202.06558) - **[ICML 2022]** [Constrained
-Variational Policy Optimization for Safe Reinforcement Learning (CVPO)](https:/
-/arxiv.org/abs/2201.11927) - **[IJCAI 2022]** [Penalized Proximal Policy
-Optimization for Safe Reinforcement Learning](https://arxiv.org/abs/2205.11814)
-- **[ICLR 2022]** [Constrained Policy Optimization via Bayesian World Models
-(LA-MBDA)](https://arxiv.org/abs/2201.09802) - **[AAAI 2022]** [Conservative
-and Adaptive Penalty for Model-Based Safe Reinforcement Learning (CAP)](https:/
-/arxiv.org/abs/2112.07701) ### List of Algorithms #### On-Policy Safe - [X]
-[The Lagrange version of PPO (PPO-Lag)](https://cdn.openai.com/safexp-
-short.pdf) - [X] [The Lagrange version of TRPO (TRPO-Lag)](https://
-cdn.openai.com/safexp-short.pdf) - [X] **[ICML 2017]** [Constrained Policy
-Optimization (CPO)](https://proceedings.mlr.press/v70/achiam17a) - [X] **[ICLR
-2019]** [Reward Constrained Policy Optimization (RCPO)](https://openreview.net/
-forum?id=SkfrvsA9FX) - [X] **[ICML 2020]** [Responsive Safety in Reinforcement
-Learning by PID Lagrangian Methods (PID-Lag)](https://arxiv.org/abs/2007.03964)
-- [X] **[NeurIPS 2020]** [First Order Constrained Optimization in Policy Space
-(FOCOPS)](https://arxiv.org/abs/2002.06506) - [X] **[AAAI 2020]** [IPO:
-Interior-point Policy Optimization under Constraints (IPO)](https://arxiv.org/
-abs/1910.09615) - [X] **[ICLR 2020]** [Projection-Based Constrained Policy
-Optimization (PCPO)](https://openreview.net/forum?id=rke3TJrtPS) - [X] **[ICML
-2021]** [CRPO: A New Approach for Safe Reinforcement Learning with Convergence
-Guarantee](https://arxiv.org/abs/2011.05869) - [x] **[IJCAI 2022]** [Penalized
-Proximal Policy Optimization for Safe Reinforcement Learning(P3O)](https://
-arxiv.org/pdf/2205.11814.pdf) #### Off-Policy Safe - [X] The Lagrange version
-of TD3 (TD3-Lag) - [X] The Lagrange version of DDPG (DDPG-Lag) - [X] The
-Lagrange version of SAC (SAC-Lag) - [X] **[ICML 2019]** [Lyapunov-based Safe
-Policy Optimization for Continuous Control (SDDPG)](https://arxiv.org/abs/
-1901.10031) - [X] **[ICML 2019]** [Lyapunov-based Safe Policy Optimization for
-Continuous Control (SDDPG-modular)](https://arxiv.org/abs/1901.10031) - [ ] **
-[ICML 2022]** [Constrained Variational Policy Optimization for Safe
-Reinforcement Learning (CVPO)](https://arxiv.org/abs/2201.11927) #### Model-
-Based Safe - [ ] **[NeurIPS 2021]** [Safe Reinforcement Learning by Imagining
-the Near Future (SMBPO)](https://arxiv.org/abs/2202.07789) - [X] **[CoRL 2021
-(Oral)]** [Learning Off-Policy with Online Planning (SafeLOOP)](https://
-arxiv.org/abs/2008.10066) - [X] **[AAAI 2022]** [Conservative and Adaptive
-Penalty for Model-Based Safe Reinforcement Learning (CAP)](https://arxiv.org/
-abs/2112.07701) - [X] **[NeurIPS 2022]** [Model-based Safe Deep Reinforcement
-Learning via a Constrained Proximal Policy Optimization Algorithm](https://
-arxiv.org/abs/2210.07573) - [ ] **[ICLR 2022]** [Constrained Policy
-Optimization via Bayesian World Models (LA-MBDA)](https://arxiv.org/abs/
-2201.09802) - [X] **[ICML 2022 Workshop]** [Constrained Model-based
+- OmniSafe is an infrastructural framework designed to accelerate safe
+reinforcement learning (RL) research. It provides a comprehensive and reliable
+benchmark for safe RL algorithms, and also an out-of-box modular toolkit for
+researchers. SafeRL intends to develop algorithms that minimize the risk of
+unintended harm or unsafe behavior. OmniSafe stands as the inaugural unified
+learning framework in the realm of safe reinforcement learning, aiming to
+foster the Growth of SafeRL Learning Community. The key features of OmniSafe: -
+**Highly Modular Framework.** OmniSafe presents a highly modular framework,
+incorporating an extensive collection of tens of algorithms tailored for safe
+reinforcement learning across diverse domains. This framework is versatile due
+to its abstraction of various algorithm types and well-designed API, using the
+Adapter and Wrapper design components to bridge gaps and enable seamless
+interactions between different components. This design allows for easy
+extension and customization, making it a powerful tool for developers working
+with different types of algorithms. - **High-performance parallel computing
+acceleration.** By harnessing the capabilities of `torch.distributed`, OmniSafe
+accelerates the learning process of algorithms with process parallelism. This
+enables OmniSafe not only to support environment-level asynchronous parallelism
+but also incorporates agent asynchronous learning. This methodology bolsters
+training stability and expedites the training process via the deployment of a
+parallel exploration mechanism. The integration of agent asynchronous learning
+in OmniSafe underscores its commitment to providing a versatile and robust
+platform for advancing SafeRL research. - **Out-of-box toolkits.** OmniSafe
+offers customizable toolkits for tasks like training, benchmarking, analyzing,
+and rendering. [Tutorials](https://github.com/PKU-Alignment/omnisafe#getting-
+started) and user-friendly [APIs](https://omnisafe.readthedocs.io/en/latest/
+baserlapi/on_policy.html) make it easy for beginners and average users, while
+advanced researchers can enhance their efficiency without complex code. ![Train
+video](https://github-production-user-asset-6210df.s3.amazonaws.com/73586554/
+237139607-d1e6f413-aa2c-4f68-b8ee-08a4361493a0.gif) ---------------------------
+----------------------------------------------------- ### Table of Contents -
+[Quick Start](#quick-start) - [Installation](#installation) - [Prerequisites]
+(#prerequisites) - [Install from source](#install-from-source) - [Install from
+PyPI](#install-from-pypi) - [Implemented Algorithms](#implemented-algorithms) -
+[Examples](#examples) - [Algorithms Registry](#algorithms-registry) -
+[Supported Environments](#supported-environments) - [Try with CLI](#try-with-
+cli) - [Getting Started](#getting-started) - [Important Hints](#important-
+hints) - [Quickstart: Colab on the Cloud](#quickstart-colab-on-the-cloud) -
+[Changelog](#changelog) - [Citing OmniSafe](#citing-omnisafe) - [The OmniSafe
+Team](#the-omnisafe-team) - [License](#license) -------------------------------
+------------------------------------------------- ## Quick Start ###
+Installation #### Prerequisites OmniSafe requires Python 3.8+ and PyTorch
+1.10+. > We support and test for Python 3.8, 3.9, 3.10 on Linux. Meanwhile, we
+also support M1 and M2 versions of macOS. We will accept PRs related to
+Windows, but do not officially support it. #### Install from source ```bash #
+Clone the repo git clone https://github.com/PKU-Alignment/omnisafe.git cd
+omnisafe # Create a conda environment conda env create --file conda-recipe.yaml
+conda activate omnisafe # Install omnisafe pip install -e . ``` #### Install
+from PyPI OmniSafe is hosted in [![PyPI](https://img.shields.io/pypi/v/
+omnisafe?label=pypi&logo=pypi)](https://pypi.org/project/omnisafe) / ![Status]
+(https://img.shields.io/pypi/status/omnisafe?label=status). ```bash pip install
+omnisafe ``` ## Implemented Algorithms LLaatteesstt SSaaffeeRRLL PPaappeerrss - **[AAAI 2023]**
+Augmented Proximal Policy Optimization for Safe Reinforcement Learning (APPO) -
+**[NeurIPS 2022]** [Constrained Update Projection Approach to Safe Policy
+Optimization (CUP)](https://arxiv.org/abs/2209.07089) - **[NeurIPS 2022]**
+[Effects of Safety State Augmentation on Safe Exploration (Simmer)](https://
+arxiv.org/abs/2206.02675) - **[NeurIPS 2022]** [Model-based Safe Deep
+Reinforcement Learning via a Constrained Proximal Policy Optimization
+Algorithm](https://arxiv.org/abs/2210.07573) - **[ICML 2022]** [SautÃ© RL:
+Almost Surely Safe Reinforcement Learning Using State Augmentation (SauteRL)]
+(https://arxiv.org/abs/2202.06558) - **[IJCAI 2022]** [Penalized Proximal
+Policy Optimization for Safe Reinforcement Learning](https://arxiv.org/abs/
+2205.11814) - **[AAAI 2022]** [Conservative and Adaptive Penalty for Model-
+Based Safe Reinforcement Learning (CAP)](https://arxiv.org/abs/2112.07701) LLiisstt
+ooff AAllggoorriitthhmmss OOnn PPoolliiccyy SSaaffeeRRLL - [x] [The Lagrange version of PPO (PPO-Lag)]
+(https://cdn.openai.com/safexp-short.pdf) - [x] [The Lagrange version of TRPO
+(TRPO-Lag)](https://cdn.openai.com/safexp-short.pdf) - [x] **[ICML 2017]**
+[Constrained Policy Optimization (CPO)](https://proceedings.mlr.press/v70/
+achiam17a) - [x] **[ICLR 2019]** [Reward Constrained Policy Optimization
+(RCPO)](https://openreview.net/forum?id=SkfrvsA9FX) - [x] **[ICML 2020]**
+[Responsive Safety in Reinforcement Learning by PID Lagrangian Methods (PID-
+Lag)](https://arxiv.org/abs/2007.03964) - [x] **[NeurIPS 2020]** [First Order
+Constrained Optimization in Policy Space (FOCOPS)](https://arxiv.org/abs/
+2002.06506) - [x] **[AAAI 2020]** [IPO: Interior-point Policy Optimization
+under Constraints (IPO)](https://arxiv.org/abs/1910.09615) - [x] **[ICLR
+2020]** [Projection-Based Constrained Policy Optimization (PCPO)](https://
+openreview.net/forum?id=rke3TJrtPS) - [x] **[ICML 2021]** [CRPO: A New Approach
+for Safe Reinforcement Learning with Convergence Guarantee](https://arxiv.org/
+abs/2011.05869) - [x] **[IJCAI 2022]** [Penalized Proximal Policy Optimization
+for Safe Reinforcement Learning(P3O)](https://arxiv.org/pdf/2205.11814.pdf) OOffff
+PPoolliiccyy SSaaffeeRRLL - **[Preprint 2019]** [The Lagrangian version of DDPG (DDPGLag)]
+(https://cdn.openai.com/safexp-short.pdf) - **[Preprint 2019]** [The Lagrangian
+version of TD3 (TD3Lag)](https://cdn.openai.com/safexp-short.pdf) - **[Preprint
+2019]** [The Lagrangian version of SAC (SACLag)](https://cdn.openai.com/safexp-
+short.pdf) - **[ICML 2020]** [Responsive Safety in Reinforcement Learning by
+PID Lagrangian Methods (DDPGPID)](https://arxiv.org/abs/2007.03964) - **[ICML
+2020]** [Responsive Safety in Reinforcement Learning by PID Lagrangian Methods
+(TD3PID)](https://arxiv.org/abs/2007.03964) - **[ICML 2020]** [Responsive
+Safety in Reinforcement Learning by PID Lagrangian Methods (SACPID)](https://
+arxiv.org/abs/2007.03964) MMooddeell--BBaasseedd SSaaffeeRRLL - [ ] **[NeurIPS 2021]** [Safe
+Reinforcement Learning by Imagining the Near Future (SMBPO)](https://arxiv.org/
+abs/2202.07789) - [x] **[CoRL 2021 (Oral)]** [Learning Off-Policy with Online
+Planning (SafeLOOP)](https://arxiv.org/abs/2008.10066) - [x] **[AAAI 2022]**
+[Conservative and Adaptive Penalty for Model-Based Safe Reinforcement Learning
+(CAP)](https://arxiv.org/abs/2112.07701) - [x] **[NeurIPS 2022]** [Model-based
+Safe Deep Reinforcement Learning via a Constrained Proximal Policy Optimization
+Algorithm](https://arxiv.org/abs/2210.07573) - [ ] **[ICLR 2022]** [Constrained
+Policy Optimization via Bayesian World Models (LA-MBDA)](https://arxiv.org/abs/
+2201.09802) - [x] **[ICML 2022 Workshop]** [Constrained Model-based
 Reinforcement Learning with Robust Cross-Entropy Method (RCE)](https://
-arxiv.org/abs/2010.07968) - [X] **[NeurIPS 2018]** [Constrained Cross-Entropy
+arxiv.org/abs/2010.07968) - [x] **[NeurIPS 2018]** [Constrained Cross-Entropy
 Method for Safe Reinforcement Learning (CCE)](https://proceedings.neurips.cc/
-paper/2018/hash/34ffeb359a192eb8174b6854643cc046-Abstract.html) #### Offline
-Safe - [X] [The Lagrange version of BCQ (BCQ-Lag)](https://arxiv.org/abs/
-1812.02900) - [X] [The Constrained version of CRR (C-CRR)](https://
-proceedings.neurips.cc/paper/2020/hash/588cb956d6bbe67078f29f8de420a13d-
-Abstract.html) - [ ] **[AAAI 2022]** [Constraints Penalized Q-learning for Safe
-Offline Reinforcement Learning CPQ](https://arxiv.org/abs/2107.09003) - [ ] **
-[ICLR 2022 (Spotlight)]** [COptiDICE: Offline Constrained Reinforcement
-Learning via Stationary Distribution Correction Estimation](https://arxiv.org/
-abs/2204.08957?context=cs.AI) - [ ] **[ICML 2022]** [Constrained Offline Policy
-Optimization (COPO)](https://proceedings.mlr.press/v162/polosky22a.html) ####
-Others - [X] [Safe Exploration in Continuous Action Spaces (Safety Layer)]
-(https://arxiv.org/abs/1801.08757) - [ ] **[RA-L 2021]** [Recovery RL: Safe
-Reinforcement Learning with Learned Recovery Zones](https://arxiv.org/abs/
-2010.15920) - [X] **[ICML 2022]** [SautÃ© RL: Almost Surely Safe Reinforcement
-Learning Using State Augmentation (SauteRL)](https://arxiv.org/abs/2202.06558)
-- [X] **[NeurIPS 2022]** [Effects of Safety State Augmentation on Safe
-Exploration](https://arxiv.org/abs/2206.02675) --------------------------------
------------------------------------------------- ## Installation ###
-Prerequisites OmniSafe requires Python 3.8+ and PyTorch 1.10+. > We support and
-test for Python 3.8, 3.9, 3.10 on Linux. Meanwhile, we also support M1 and M2
-versions of macOS. We will accept PRs related to Windows, but do not officially
-support it. #### Install from source ```bash # Clone the repo git clone https:/
-/github.com/OmniSafeAI/omnisafe cd omnisafe # Create a conda environment conda
-env create --file conda-recipe.yaml conda activate omnisafe # Install omnisafe
-pip install -e . ``` #### Install from PyPI OmniSafe is hosted in [![PyPI]
-(https://img.shields.io/pypi/v/omnisafe?label=pypi&logo=pypi)](https://
-pypi.org/project/omnisafe) / ![Status](https://img.shields.io/pypi/status/
-omnisafe?label=status). ```bash pip install omnisafe ``` ### Examples ```bash
-cd examples python train_policy.py --algo PPOLag --env-id SafetyPointGoal1-v0 -
--parallel 1 --total-steps 1024000 --device cpu --vector-env-nums 1 --torch-
-threads 1 ``` **algo:** | Type | Name | | ----------------- | -----------------
------------------------------------------------ | | `Base-On-Policy` |
-`PolicyGradient, PPO`
-`NaturalPG, TRPO` | | `Base-Off-Policy` | `DDPG, TD3, SAC` | | `Naive Lagrange`
-| `RCPO, PPOLag, TRPOLag`
-`DDPGLag, TD3Lag, SACLag` | | `PID Lagrange` | `CPPOPid, TRPOPid` | | `First
-Order` | `FOCOPS, CUP` | | `Second Order` | `SDDPG, CPO, PCPO` | | `Saute RL` |
-`PPOSaute, PPOLagSaute` | | `Simmer RL` | `PPOSimmerQ, PPOSimmerPid`
-`PPOLagSimmerQ, PPOLagSimmerPid` | | `EarlyTerminated` | `PPOEarlyTerminated`
-`PPOLagEarlyTerminated` | | `Model-Based` | `CAP, MBPPOLag, SafeLOOP` | **env-
-id:** Environment id in [Safety Gymnasium](https://www.safety-gymnasium.com/),
-here a list of envs that safety-gymnasium supports.
+paper/2018/hash/34ffeb359a192eb8174b6854643cc046-Abstract.html) OOfffflliinnee SSaaffeeRRLL
+- [x] [The Lagrange version of BCQ (BCQ-Lag)](https://arxiv.org/abs/1812.02900)
+- [x] [The Constrained version of CRR (C-CRR)](https://proceedings.neurips.cc/
+paper/2020/hash/588cb956d6bbe67078f29f8de420a13d-Abstract.html) - [ ] **[AAAI
+2022]** [Constraints Penalized Q-learning for Safe Offline Reinforcement
+Learning CPQ](https://arxiv.org/abs/2107.09003) - [x] **[ICLR 2022
+(Spotlight)]** [COptiDICE: Offline Constrained Reinforcement Learning via
+Stationary Distribution Correction Estimation](https://arxiv.org/abs/
+2204.08957?context=cs.AI) - [ ] **[ICML 2022]** [Constrained Offline Policy
+Optimization (COPO)](https://proceedings.mlr.press/v162/polosky22a.html) OOtthheerrss
+- [ ] **[RA-L 2021]** [Recovery RL: Safe Reinforcement Learning with Learned
+Recovery Zones](https://arxiv.org/abs/2010.15920) - [x] **[ICML 2022]** [SautÃ©
+RL: Almost Surely Safe Reinforcement Learning Using State Augmentation
+(SauteRL)](https://arxiv.org/abs/2202.06558) - [x] **[NeurIPS 2022]** [Effects
+of Safety State Augmentation on Safe Exploration](https://arxiv.org/abs/
+2206.02675) -------------------------------------------------------------------
+------------- ### Examples ```bash cd examples python train_policy.py --algo
+PPOLag --env-id SafetyPointGoal1-v0 --parallel 1 --total-steps 10000000 --
+device cpu --vector-env-nums 1 --torch-threads 1 ``` #### Algorithms Registry
+DDoommaaiinnss               TTyyppeess                AAllggoorriitthhmmss RReeggiissttrryy
+                      Primal Dual          TRPOLag; PPOLag; PDO; RCPO
+                                           TRPOPID; CPPOPID
+On Policy             Convex Optimization  CPO; PCPO; FOCOPS; CUP
+                      Penalty Function     IPO; P3O
+                      Primal               OnCRPO
+Off Policy            Primal-Dual          DDPGLag; TD3Lag; SACLag
+                                           DDPGPID; TD3PID; SACPID
+Model-based           Online Plan          SafeLOOP; CCEPETS; RCEPETS
+                      Pessimistic Estimate CAPPETS
+DICE Based            COptDICE
+                      ET-MDP               PPOEarlyTerminated;
+Other Formulation MDP                      TRPOEarlyTerminated
+                      SauteRL              PPOSaute; TRPOSaute
+                      SimmerRL             PPOSimmerPID; TRPOSimmerPID
+#### Supported Environments Here is a list of environments that [Safety-
+Gymnasium](https://www.safety-gymnasium.com) supports:
  _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
 |_CC_aa_tt_ee_gg_oo_rr_yy_ _ _ _ _ _ _ _|_TT_aa_ss_kk_ _ _ _ _ _ _ _|_AA_gg_ee_nn_tt_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_EE_xx_aa_mm_pp_ll_ee_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |               |_G_o_a_l_[_0_1_2_]_ _ |                        |                       |
 |Safe Navigation|_B_u_t_t_o_n_[_0_1_2_]|Point, Car, Racecar, Ant|SafetyPointGoal1-v0    |
 |               |_P_u_s_h_[_0_1_2_]_ _ |                        |                       |
 |_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_C_i_r_c_l_e_[_0_1_2_]_|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |               |           |HalfCheetah, Hopper,    |SafetyHumanoidVelocity-|
 |Safe Velocity  |Velocity   |Swimmer, Walker2d, Ant, |v1                     |
 |_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _|_H_u_m_a_n_o_i_d_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
-More information about environments, please refer to [Safety Gymnasium](https:/
-/www.safety-gymnasium.com/) **parallel:** `Number of parallels` #### Try with
-CLI **A video example** ![Segmentfault](https://github.com/OmniSafeAI/omnisafe/
-blob/main/images/CLI_example.svg) ```bash pip install omnisafe omnisafe --help
-# Ask for help omnisafe benchmark --help # The benchmark also can be replaced
-with 'eval', 'train', 'train-config' # Quick benchmarking for your research,
-just specify: 1.exp_name, 2.num_pool(how much processes are concurrent), 3.path
-of the config file(refer to omnisafe/examples/benchmarks for format) omnisafe
-benchmark test_benchmark 2 ./saved_source/benchmark_config.yaml # Quick
-evaluating and rendering your trained policy, just specify: 1.path of algorithm
-which you trained omnisafe eval ./saved_source/PPO-{SafetyPointGoal1-v0} --num-
-episode 1 # Quick training some algorithms to validate your thoughts # Note:
-use `key1:key2`, your can select key of hyperparameters which are recursively
-contained, and use `--custom-cfgs`, you can add custom cfgs via CLI omnisafe
-train --algo PPO --total-steps 2048 --vector-env-nums 1 --custom-cfgs
-algo_cfgs:steps_per_epoch --custom-cfgs 1024 # Quick training some algorithms
-via a saved config file, the format is as same as default format omnisafe
-train-config ./saved_source/train_config.yaml ``` -----------------------------
---------------------------------------------------- ## Getting Started ###
-Important Hints - `train_cfgs:torch_threads` is especially important for
-training speed, and is varying with users' machine, this value shouldn't be too
-small or too large. ### Quickstart: Colab on the Cloud Explore OmniSafe easily
-and quickly through a series of colab notebooks: - [Getting Started](https://
-colab.research.google.com/github/OmniSafeAI/omnisafe/blob/main/tutorials/
-English/1.Getting_Started.ipynb) Introduce the basic usage of OmniSafe so that
-users can quickly hand on it. - [CLI Command](https://
-colab.research.google.com/github/OmniSafeAI/omnisafe/blob/main/tutorials/
+For more information about environments, please refer to [Safety-Gymnasium]
+(https://www.safety-gymnasium.com). #### Try with CLI ```bash pip install
+omnisafe omnisafe --help # Ask for help omnisafe benchmark --help # The
+benchmark also can be replaced with 'eval', 'train', 'train-config' # Quick
+benchmarking for your research, just specify: # 1. exp_name # 2. num_pool(how
+much processes are concurrent) # 3. path of the config file (refer to omnisafe/
+examples/benchmarks for format) # Here we provide an exampe in ./tests/
+saved_source. # And you can set your benchmark_config.yaml by following it
+omnisafe benchmark test_benchmark 2 ./tests/saved_source/benchmark_config.yaml
+# Quick evaluating and rendering your trained policy, just specify: # 1. path
+of algorithm which you trained omnisafe eval ./tests/saved_source/PPO-
+{SafetyPointGoal1-v0} --num-episode 1 # Quick training some algorithms to
+validate your thoughts # Note: use `key1:key2`, your can select key of
+hyperparameters which are recursively contained, and use `--custom-cfgs`, you
+can add custom cfgs via CLI omnisafe train --algo PPO --total-steps 2048 --
+vector-env-nums 1 --custom-cfgs algo_cfgs:steps_per_epoch --custom-cfgs 1024 #
+Quick training some algorithms via a saved config file, the format is as same
+as default format omnisafe train-config ./tests/saved_source/train_config.yaml
+``` ---------------------------------------------------------------------------
+----- ## Getting Started ### Important Hints We have provided benchmark results
+for various algorithms, including on-policy, off-policy, model-based, and
+offline approaches, along with parameter tuning analysis. Please refer to the
+following: - [On-Policy](./benchmarks/on-policy/) - [Off-Policy](./benchmarks/
+off-policy/) - [Model-based](./benchmarks/model-based/) - [Offline](./
+benchmarks/offline/) ### Quickstart: Colab on the Cloud Explore OmniSafe easily
+and quickly through a series of Google Colab notebooks: - [Getting Started]
+(https://colab.research.google.com/github/PKU-Alignment/omnisafe/blob/main/
+tutorials/English/1.Getting_Started.ipynb) Introduce the basic usage of
+OmniSafe so that users can quickly hand it. - [CLI Command](https://
+colab.research.google.com/github/PKU-Alignment/omnisafe/blob/main/tutorials/
 English/2.CLI_Command.ipynb) Introduce how to use the CLI tool of OmniSafe. We
 take great pleasure in collaborating with our users to create tutorials in
 various languages. Please refer to our list of currently supported languages.
 If you are interested in translating the tutorial into a new language or
 improving an existing version, kindly submit a PR to us. ----------------------
 ---------------------------------------------------------- ## Changelog See
-[CHANGELOG.md](https://github.com/OmniSafeAI/omnisafe/blob/main/CHANGELOG.md).
-## The OmniSafe Team OmniSafe is mainly developed by the SafeRL research team
-directed by Prof. [Yaodong Yang](https://github.com/orgs/OmniSafeAI/people/PKU-
-YYang). Our SafeRL research team members include [Borong Zhang](https://
-github.com/muchvo), [Jiayi Zhou](https://github.com/Gaiejj), [JTao Dai](https:/
-/github.com/calico-1226), [Weidong Huang](https://github.com/hdadong), [Ruiyang
-Sun](https://github.com/rockmagma02), [Xuehai Pan](https://github.com/
-XuehaiPan) and [Jiaming Ji](https://github.com/zmsn-2077). If you have any
-questions in the process of using omnisafe, don't hesitate to ask your
-questions on [the GitHub issue page](https://github.com/OmniSafeAI/omnisafe/
-issues/new/choose), we will reply to you in 2-3 working days. ## License
-OmniSafe is released under Apache License 2.0.
+[CHANGELOG.md](https://github.com/PKU-Alignment/omnisafe/blob/main/
+CHANGELOG.md). ## Citing OmniSafe If you find OmniSafe useful or use OmniSafe
+in your research, please cite it in your publications. ```bibtex @article
+{omnisafe, title = {OmniSafe: An Infrastructure for Accelerating Safe
+Reinforcement Learning Research}, author = {Jiaming Ji, Jiayi Zhou, Borong
+Zhang, Juntao Dai, Xuehai Pan, Ruiyang Sun, Weidong Huang, Yiran Geng, Mickel
+Liu, Yaodong Yang}, journal = {arXiv preprint arXiv:2305.09304}, year = {2023}
+} ``` ## The OmniSafe Team OmniSafe is mainly developed by the SafeRL research
+team directed by Prof. [Yaodong Yang](https://www.yangyaodong.com/). Our SafeRL
+research team members include [Borong Zhang](https://github.com/muchvo), [Jiayi
+Zhou](https://github.com/Gaiejj), [JTao Dai](https://github.com/calico-1226),
+[Weidong Huang](https://github.com/hdadong), [Ruiyang Sun](https://github.com/
+rockmagma02), [Xuehai Pan](https://github.com/XuehaiPan) and [Jiaming Ji]
+(https://github.com/zmsn-2077). If you have any questions in the process of
+using OmniSafe, don't hesitate to ask your questions on [the GitHub issue page]
+(https://github.com/PKU-Alignment/omnisafe/issues/new/choose), we will reply to
+you in 2-3 working days. ## License OmniSafe is released under Apache License
+2.0.
```

### Comparing `omnisafe-0.4.0/omnisafe.egg-info/SOURCES.txt` & `omnisafe-0.5.0b0/omnisafe.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 omnisafe.egg-info/dependency_links.txt
 omnisafe.egg-info/entry_points.txt
 omnisafe.egg-info/requires.txt
 omnisafe.egg-info/top_level.txt
 omnisafe/adapter/__init__.py
 omnisafe/adapter/early_terminated_adapter.py
 omnisafe/adapter/modelbased_adapter.py
+omnisafe/adapter/offline_adapter.py
 omnisafe/adapter/offpolicy_adapter.py
 omnisafe/adapter/online_adapter.py
 omnisafe/adapter/onpolicy_adapter.py
 omnisafe/adapter/saute_adapter.py
 omnisafe/adapter/simmer_adapter.py
 omnisafe/algorithms/__init__.py
 omnisafe/algorithms/algo_wrapper.py
@@ -40,42 +41,54 @@
 omnisafe/algorithms/model_based/planner/cce.py
 omnisafe/algorithms/model_based/planner/cem.py
 omnisafe/algorithms/model_based/planner/rce.py
 omnisafe/algorithms/model_based/planner/safe_arc.py
 omnisafe/algorithms/off_policy/__init__.py
 omnisafe/algorithms/off_policy/ddpg.py
 omnisafe/algorithms/off_policy/ddpg_lag.py
+omnisafe/algorithms/off_policy/ddpg_pid.py
 omnisafe/algorithms/off_policy/sac.py
 omnisafe/algorithms/off_policy/sac_lag.py
+omnisafe/algorithms/off_policy/sac_pid.py
 omnisafe/algorithms/off_policy/td3.py
 omnisafe/algorithms/off_policy/td3_lag.py
+omnisafe/algorithms/off_policy/td3_pid.py
+omnisafe/algorithms/offline/__init__.py
+omnisafe/algorithms/offline/base.py
+omnisafe/algorithms/offline/bcq.py
+omnisafe/algorithms/offline/bcq_lag.py
+omnisafe/algorithms/offline/c_crr.py
+omnisafe/algorithms/offline/coptidice.py
+omnisafe/algorithms/offline/crr.py
+omnisafe/algorithms/offline/vae_bc.py
 omnisafe/algorithms/on_policy/__init__.py
 omnisafe/algorithms/on_policy/base/__init__.py
 omnisafe/algorithms/on_policy/base/natural_pg.py
 omnisafe/algorithms/on_policy/base/policy_gradient.py
 omnisafe/algorithms/on_policy/base/ppo.py
 omnisafe/algorithms/on_policy/base/trpo.py
 omnisafe/algorithms/on_policy/early_terminated/__init__.py
 omnisafe/algorithms/on_policy/early_terminated/ppo_early_terminated.py
 omnisafe/algorithms/on_policy/early_terminated/trpo_early_terminated.py
 omnisafe/algorithms/on_policy/first_order/__init__.py
 omnisafe/algorithms/on_policy/first_order/cup.py
 omnisafe/algorithms/on_policy/first_order/focops.py
 omnisafe/algorithms/on_policy/naive_lagrange/__init__.py
-omnisafe/algorithms/on_policy/naive_lagrange/crpo.py
 omnisafe/algorithms/on_policy/naive_lagrange/pdo.py
 omnisafe/algorithms/on_policy/naive_lagrange/ppo_lag.py
 omnisafe/algorithms/on_policy/naive_lagrange/rcpo.py
 omnisafe/algorithms/on_policy/naive_lagrange/trpo_lag.py
 omnisafe/algorithms/on_policy/penalty_function/__init__.py
 omnisafe/algorithms/on_policy/penalty_function/ipo.py
 omnisafe/algorithms/on_policy/penalty_function/p3o.py
 omnisafe/algorithms/on_policy/pid_lagrange/__init__.py
 omnisafe/algorithms/on_policy/pid_lagrange/cppo_pid.py
 omnisafe/algorithms/on_policy/pid_lagrange/trpo_pid.py
+omnisafe/algorithms/on_policy/primal/__init__.py
+omnisafe/algorithms/on_policy/primal/crpo.py
 omnisafe/algorithms/on_policy/saute/__init__.py
 omnisafe/algorithms/on_policy/saute/ppo_saute.py
 omnisafe/algorithms/on_policy/saute/trpo_saute.py
 omnisafe/algorithms/on_policy/second_order/__init__.py
 omnisafe/algorithms/on_policy/second_order/cpo.py
 omnisafe/algorithms/on_policy/second_order/pcpo.py
 omnisafe/algorithms/on_policy/simmer/__init__.py
@@ -91,26 +104,38 @@
 omnisafe/common/statistics_tools.py
 omnisafe/common/buffer/__init__.py
 omnisafe/common/buffer/base.py
 omnisafe/common/buffer/offpolicy_buffer.py
 omnisafe/common/buffer/onpolicy_buffer.py
 omnisafe/common/buffer/vector_offpolicy_buffer.py
 omnisafe/common/buffer/vector_onpolicy_buffer.py
+omnisafe/common/offline/__init__.py
+omnisafe/common/offline/data_collector.py
+omnisafe/common/offline/dataset.py
 omnisafe/configs/model-based/CAPPETS.yaml
 omnisafe/configs/model-based/CCEPETS.yaml
 omnisafe/configs/model-based/LOOP.yaml
 omnisafe/configs/model-based/PETS.yaml
 omnisafe/configs/model-based/RCEPETS.yaml
 omnisafe/configs/model-based/SafeLOOP.yaml
 omnisafe/configs/off-policy/DDPG.yaml
 omnisafe/configs/off-policy/DDPGLag.yaml
+omnisafe/configs/off-policy/DDPGPID.yaml
 omnisafe/configs/off-policy/SAC.yaml
 omnisafe/configs/off-policy/SACLag.yaml
+omnisafe/configs/off-policy/SACPID.yaml
 omnisafe/configs/off-policy/TD3.yaml
 omnisafe/configs/off-policy/TD3Lag.yaml
+omnisafe/configs/off-policy/TD3PID.yaml
+omnisafe/configs/offline/BCQ.yaml
+omnisafe/configs/offline/BCQLag.yaml
+omnisafe/configs/offline/CCRR.yaml
+omnisafe/configs/offline/COptiDICE.yaml
+omnisafe/configs/offline/CRR.yaml
+omnisafe/configs/offline/VAEBC.yaml
 omnisafe/configs/on-policy/CPO.yaml
 omnisafe/configs/on-policy/CPPOPID.yaml
 omnisafe/configs/on-policy/CUP.yaml
 omnisafe/configs/on-policy/FOCOPS.yaml
 omnisafe/configs/on-policy/IPO.yaml
 omnisafe/configs/on-policy/NaturalPG.yaml
 omnisafe/configs/on-policy/OnCRPO.yaml
@@ -140,36 +165,42 @@
 omnisafe/models/base.py
 omnisafe/models/actor/__init__.py
 omnisafe/models/actor/actor_builder.py
 omnisafe/models/actor/gaussian_actor.py
 omnisafe/models/actor/gaussian_learning_actor.py
 omnisafe/models/actor/gaussian_sac_actor.py
 omnisafe/models/actor/mlp_actor.py
+omnisafe/models/actor/perturbation_actor.py
+omnisafe/models/actor/vae_actor.py
 omnisafe/models/actor_critic/__init__.py
 omnisafe/models/actor_critic/actor_critic.py
 omnisafe/models/actor_critic/actor_q_critic.py
 omnisafe/models/actor_critic/constraint_actor_critic.py
 omnisafe/models/actor_critic/constraint_actor_q_critic.py
 omnisafe/models/critic/__init__.py
 omnisafe/models/critic/critic_builder.py
 omnisafe/models/critic/q_critic.py
 omnisafe/models/critic/v_critic.py
+omnisafe/models/offline/__init__.py
+omnisafe/models/offline/dice.py
 omnisafe/utils/__init__.py
 omnisafe/utils/command_app.py
 omnisafe/utils/config.py
 omnisafe/utils/distributed.py
 omnisafe/utils/exp_grid_tools.py
 omnisafe/utils/math.py
 omnisafe/utils/model.py
 omnisafe/utils/plotter.py
 omnisafe/utils/schedule.py
 omnisafe/utils/tools.py
 tests/test_buffer.py
 tests/test_cli.py
+tests/test_ensemble.py
 tests/test_env.py
 tests/test_experiment_grid.py
 tests/test_model.py
 tests/test_normalizer.py
+tests/test_offline_data.py
 tests/test_policy.py
 tests/test_registry.py
 tests/test_statistics_tools.py
 tests/test_utils.py
```

### Comparing `omnisafe-0.4.0/pyproject.toml` & `omnisafe-0.5.0b0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -21,34 +21,35 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
-    "safety-gymnasium >= 0.1.0",
+    "safety-gymnasium >= 0.2.0",
     "torch >= 1.10.0",
     "numpy >= 1.20.0",
     "tensorboard >= 2.8.0",
     "wandb >= 0.13.0",
     "pyyaml >= 6.0",
     "moviepy >= 1.0.0",
     "typing-extensions >= 4.0.0",
     "typer[all] >= 0.7.0",
     "seaborn >= 0.12.2",
     "pandas >=  1.5.3",
     "matplotlib >= 3.7.1",
+    "gdown >= 4.6.0"
 ]
 dynamic = ["version", "entry-points"]
 
 [project.urls]
-Homepage = "https://github.com/OmniSafeAI/omnisafe"
-Repository = "https://github.com/OmniSafeAI/omnisafe"
+Homepage = "https://github.com/PKU-Alignment/omnisafe"
+Repository = "https://github.com/PKU-Alignment/omnisafe"
 Documentation = "https://omnisafe.readthedocs.io"
-"Bug Report" = "https://github.com/OmniSafeAI/omnisafe/issues"
+"Bug Report" = "https://github.com/PKU-Alignment/omnisafe/issues"
 
 [project.optional-dependencies]
 lint = [
     "isort >= 5.11.0",
     "black >= 22.6.0",
     "pylint[spelling] >= 2.15.0",
     "mypy >= 0.990",
```

### Comparing `omnisafe-0.4.0/setup.py` & `omnisafe-0.5.0b0/setup.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.4.0/tests/test_buffer.py` & `omnisafe-0.5.0b0/tests/test_buffer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Test Buffers"""
+"""Test Buffers."""
 
 import torch
 from gymnasium.spaces import Box
 
 import helpers
 from omnisafe.common.buffer import (
     OffPolicyBuffer,
```

### Comparing `omnisafe-0.4.0/tests/test_cli.py` & `omnisafe-0.5.0b0/tests/test_cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -106,7 +106,25 @@
             '--compare-num',
             '2',
             '--cost-limit',
             '25',
         ],
     )
     assert result.exit_code == 0, result.output
+
+
+def teardown_module():
+    """teardown_module."""
+    # remove the train_dict folder
+    path = os.path.join(base_path, './train_dict')
+    if os.path.exists(path):
+        os.system('rm -rf ' + path)
+
+    # remove the train folder
+    path = os.path.join(base_path, './train')
+    if os.path.exists(path):
+        os.system('rm -rf ' + path)
+
+    # remove the benchmark folder
+    path = os.path.join(base_path, './benchmark')
+    if os.path.exists(path):
+        os.system('rm -rf ' + path)
```

### Comparing `omnisafe-0.4.0/tests/test_env.py` & `omnisafe-0.5.0b0/tests/test_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Test envs"""
+"""Test envs."""
 
 from gymnasium.spaces import Box
 
 import helpers
 from omnisafe.envs.core import make
```

### Comparing `omnisafe-0.4.0/tests/test_experiment_grid.py` & `omnisafe-0.5.0b0/tests/test_experiment_grid.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Test experiment grid"""
+"""Test experiment grid."""
 
+import os
 
 from omnisafe.common.experiment_grid import ExperimentGrid
 from omnisafe.utils.exp_grid_tools import train
 
 
 def test_experiment_grid():
     """Test experiment grid."""
@@ -42,47 +43,60 @@
     eg.run(train, num_pool=1)
 
     eg.analyze('algo')
     # eg.render(num_episodes=1, render_mode='rgb_array', width=256, height=256)
     eg.evaluate(num_episodes=1)
 
 
-def test_modelbased_experiment_grid():
-    """Test experiment grid."""
-    eg = ExperimentGrid(exp_name='Test_experiment_grid_modelbased')
-
-    # Set the environments.
-    mujoco_envs = ['SafetyPointGoal1-v0-modelbased']
-
-    # Set the algorithms.
-    eg.add('env_id', mujoco_envs)
-
-    eg.add('algo', ['LOOP'])
-    eg.add('train_cfgs:total_steps', [1024])
-    eg.add('train_cfgs:vector_env_nums', [1])
-    eg.add('train_cfgs:torch_threads', [1])
-    eg.add('algo_cfgs:obs_normalize', [False])
-    eg.add('algo_cfgs:steps_per_epoch', [1000])
-    eg.add('algo_cfgs:action_repeat', [10])
-    eg.add('algo_cfgs:update_dynamics_cycle', [2000])
-    eg.add('algo_cfgs:update_policy_cycle', [2000])
-    eg.add('algo_cfgs:update_policy_iters', [1])
-    eg.add('algo_cfgs:start_learning_steps', [3])
-    eg.add('algo_cfgs:policy_batch_size', [1])
-    eg.add('dynamics_cfgs:num_ensemble', [5])
-    eg.add('dynamics_cfgs:batch_size', [1])
-    eg.add('dynamics_cfgs:max_epoch', [1])
-    eg.add('dynamics_cfgs:predict_cost', [False])
-    eg.add('planner_cfgs:plan_horizon', [2])
-    eg.add('planner_cfgs:num_particles', [5])
-    eg.add('planner_cfgs:num_samples', [10])
-    eg.add('planner_cfgs:num_elites', [5])
-    eg.add('evaluation_cfgs:use_eval', [False])
-    eg.add('logger_cfgs:use_wandb', [False])
-    eg.add('seed', [0])
-    # total experiment num must can be divided by num_pool
-    # meanwhile, users should decide this value according to their machine
-    eg.run(train, num_pool=1)
+# def test_modelbased_experiment_grid():
+#     """Test experiment grid."""
+#     eg = ExperimentGrid(exp_name='Test_experiment_grid_modelbased')
+
+#     # Set the environments.
+#     mujoco_envs = ['SafetyPointGoal1-v0-modelbased']
+
+#     # Set the algorithms.
+#     eg.add('env_id', mujoco_envs)
+
+#     eg.add('algo', ['LOOP'])
+#     eg.add('train_cfgs:total_steps', [1024])
+#     eg.add('train_cfgs:vector_env_nums', [1])
+#     eg.add('train_cfgs:torch_threads', [1])
+#     eg.add('algo_cfgs:obs_normalize', [False])
+#     eg.add('algo_cfgs:steps_per_epoch', [1000])
+#     eg.add('algo_cfgs:action_repeat', [10])
+#     eg.add('algo_cfgs:update_dynamics_cycle', [2000])
+#     eg.add('algo_cfgs:update_policy_cycle', [2000])
+#     eg.add('algo_cfgs:update_policy_iters', [1])
+#     eg.add('algo_cfgs:start_learning_steps', [3])
+#     eg.add('algo_cfgs:policy_batch_size', [1])
+#     eg.add('dynamics_cfgs:num_ensemble', [5])
+#     eg.add('dynamics_cfgs:batch_size', [1])
+#     eg.add('dynamics_cfgs:max_epoch', [1])
+#     eg.add('dynamics_cfgs:predict_cost', [False])
+#     eg.add('planner_cfgs:plan_horizon', [2])
+#     eg.add('planner_cfgs:num_particles', [5])
+#     eg.add('planner_cfgs:num_samples', [10])
+#     eg.add('planner_cfgs:num_elites', [5])
+#     eg.add('evaluation_cfgs:use_eval', [False])
+#     eg.add('logger_cfgs:use_wandb', [False])
+#     eg.add('seed', [0])
+#     # total experiment num must can be divided by num_pool
+#     # meanwhile, users should decide this value according to their machine
+#     eg.run(train, num_pool=1)
+
+#     eg.analyze('algo')
+#     # eg.render(num_episodes=1, render_mode='rgb_array', width=256, height=256)
+#     eg.evaluate(num_episodes=1)
+
+
+def teardown_module():
+    """teardown_module."""
+    base_path = os.path.dirname(os.path.abspath(__file__))
+
+    # remove exp-x folder
+    exp_x_path = os.path.join(base_path, 'exp-x')
+    if os.path.exists(exp_x_path):
+        os.system(f'rm -rf {exp_x_path}')
 
-    eg.analyze('algo')
-    # eg.render(num_episodes=1, render_mode='rgb_array', width=256, height=256)
-    eg.evaluate(num_episodes=1)
+    # remove png
+    os.system(f'rm -rf {base_path}/algo--*.png')
```

### Comparing `omnisafe-0.4.0/tests/test_model.py` & `omnisafe-0.5.0b0/tests/test_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Test models"""
+"""Test models."""
 
 import pytest
 import torch
 from gymnasium.spaces import Box, Discrete
 
 import helpers
 from omnisafe.models import ActorBuilder, CriticBuilder
```

### Comparing `omnisafe-0.4.0/tests/test_normalizer.py` & `omnisafe-0.5.0b0/tests/test_normalizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Test normalizer"""
+"""Test normalizer."""
 
 import torch
 
 import helpers
 from omnisafe.common.normalizer import Normalizer
```

### Comparing `omnisafe-0.4.0/tests/test_policy.py` & `omnisafe-0.5.0b0/tests/test_policy.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,48 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Test policy algorithms"""
+"""Test policy algorithms."""
+
+import os
 
 import pytest
 import torch
 
 import helpers
 import omnisafe
 import simple_env  # noqa: F401
 
 
 base_policy = ['PolicyGradient', 'NaturalPG', 'TRPO', 'PPO']
 naive_lagrange_policy = ['PPOLag', 'TRPOLag', 'RCPO', 'OnCRPO', 'PDO']
 first_order_policy = ['CUP', 'FOCOPS']
 second_order_policy = ['CPO', 'PCPO']
 penalty_policy = ['P3O', 'IPO']
-off_policy = ['DDPG', 'TD3', 'DDPGLag', 'TD3Lag']
-sac_policy = ['SAC', 'SACLag']
+off_base = ['DDPG', 'TD3']
+off_lag = ['DDPGLag', 'TD3Lag', 'DDPGPID', 'TD3PID']
+sac_base = ['SAC']
+sac_lag = ['SACLag', 'SACPID']
 saute_policy = ['TRPOSaute', 'PPOSaute']
 simmer_policy = ['TRPOSimmerPID', 'PPOSimmerPID']
 pid_lagrange_policy = ['TRPOPID', 'CPPOPID']
 early_terminated_policy = ['TRPOEarlyTerminated', 'PPOEarlyTerminated']
+offline_policy = ['BCQ', 'BCQLag', 'CRR', 'CCRR', 'VAEBC']
 
-# saute_policy = ['PPOSaute', 'PPOLagSaute']
-# simmer_policy = ['PPOSimmerQ', 'PPOLagSimmerQ', 'PPOSimmerPid', 'PPOLagSimmerPid']
 model_cfgs = {
     'linear_lr_decay': True,
     'actor': {
         'hidden_sizes': [8, 8],
     },
     'critic': {
         'hidden_sizes': [8, 8],
@@ -219,14 +222,15 @@
         'logger_cfgs': {
             'use_wandb': False,
             'save_model_freq': 1,
         },
     }
     agent = omnisafe.Agent(algo, env_id, custom_cfgs=custom_cfgs)
     agent.learn()
+    agent.render()
 
 
 @helpers.parametrize(algo=['LOOP', 'SafeLOOP'])
 def test_loop(algo):
     """Test model_based algorithms."""
     env_id = 'Simple-v0'
 
@@ -242,14 +246,16 @@
             'steps_per_epoch': 100,
             'action_repeat': 1,
             'update_dynamics_cycle': 100,
             'update_policy_cycle': 100,
             'update_policy_iters': 1,
             'start_learning_steps': 3,
             'policy_batch_size': 10,
+            'use_critic_norm': True,
+            'max_grad_norm': True,
         },
         'planner_cfgs': {
             'plan_horizon': 2,
             'num_particles': 5,
             'num_samples': 10,
             'num_elites': 5,
         },
@@ -268,15 +274,15 @@
             'save_model_freq': 1,
         },
     }
     agent = omnisafe.Agent(algo, env_id, custom_cfgs=custom_cfgs)
     agent.learn()
 
 
-@helpers.parametrize(algo=off_policy)
+@helpers.parametrize(algo=off_base)
 def test_off_policy(algo):
     """Test base algorithms."""
     env_id = 'Simple-v0'
     custom_cfgs = {
         'train_cfgs': {
             'total_steps': 200,
             'vector_env_nums': 1,
@@ -297,14 +303,44 @@
         },
         'model_cfgs': model_cfgs,
     }
     agent = omnisafe.Agent(algo, env_id, custom_cfgs=custom_cfgs)
     agent.learn()
 
 
+@helpers.parametrize(algo=off_lag)
+def test_off_lag_policy(algo):
+    """Test base algorithms."""
+    env_id = 'Simple-v0'
+    custom_cfgs = {
+        'train_cfgs': {
+            'total_steps': 200,
+            'vector_env_nums': 1,
+            'torch_threads': 4,
+        },
+        'algo_cfgs': {
+            'steps_per_epoch': 100,
+            'update_cycle': 50,
+            'update_iters': 2,
+            'start_learning_steps': 0,
+            'use_critic_norm': True,
+            'max_grad_norm': True,
+            'obs_normalize': True,
+            'warmup_epochs': 0,
+        },
+        'logger_cfgs': {
+            'use_wandb': False,
+            'save_model_freq': 1,
+        },
+        'model_cfgs': model_cfgs,
+    }
+    agent = omnisafe.Agent(algo, env_id, custom_cfgs=custom_cfgs)
+    agent.learn()
+
+
 auto_alpha = [True, False]
 
 
 @helpers.parametrize(auto_alpha=auto_alpha)
 def test_sac_policy(auto_alpha):
     """Test sac algorithms."""
     env_id = 'Simple-v0'
@@ -331,16 +367,16 @@
     agent = omnisafe.Agent('SAC', env_id, custom_cfgs=custom_cfgs)
     agent.learn()
 
 
 auto_alpha = [True, False]
 
 
-@helpers.parametrize(auto_alpha=auto_alpha)
-def test_sac_lag_policy(auto_alpha):
+@helpers.parametrize(auto_alpha=auto_alpha, algo=sac_lag)
+def test_sac_lag_policy(auto_alpha, algo):
     """Test sac algorithms."""
     env_id = 'Simple-v0'
     custom_cfgs = {
         'train_cfgs': {
             'total_steps': 200,
             'vector_env_nums': 1,
             'torch_threads': 4,
@@ -349,22 +385,23 @@
             'steps_per_epoch': 100,
             'update_cycle': 50,
             'update_iters': 2,
             'start_learning_steps': 0,
             'auto_alpha': auto_alpha,
             'use_critic_norm': True,
             'max_grad_norm': True,
+            'warmup_epochs': 0,
         },
         'logger_cfgs': {
             'use_wandb': False,
             'save_model_freq': 1,
         },
         'model_cfgs': model_cfgs,
     }
-    agent = omnisafe.Agent('SACLag', env_id, custom_cfgs=custom_cfgs)
+    agent = omnisafe.Agent(algo, env_id, custom_cfgs=custom_cfgs)
     agent.learn()
 
 
 @helpers.parametrize(
     algo=(
         base_policy
         + naive_lagrange_policy
@@ -420,14 +457,59 @@
             'diff_norm': True,
         },
     }
     agent = omnisafe.Agent(algo, env_id, custom_cfgs=custom_cfgs)
     agent.learn()
 
 
+@helpers.parametrize(
+    algo=(offline_policy),
+)
+def test_offline(algo):
+    """Test base algorithms."""
+    env_id = 'Simple-v0'
+    dataset = os.path.join(os.path.dirname(__file__), 'saved_source', 'Simple-v0.npz')
+    custom_cfgs = {
+        'train_cfgs': {
+            'total_steps': 4,
+            'torch_threads': 4,
+            'dataset': dataset,
+        },
+        'algo_cfgs': {
+            'batch_size': 10,
+            'steps_per_epoch': 2,
+        },
+    }
+    agent = omnisafe.Agent(algo, env_id, custom_cfgs=custom_cfgs)
+    agent.learn()
+
+
+@helpers.parametrize(
+    fn_type=['softchi', 'chisquare'],
+)
+def test_coptidice(fn_type):
+    """Test coptidice algorithms."""
+    env_id = 'Simple-v0'
+    dataset = os.path.join(os.path.dirname(__file__), 'saved_source', 'Simple-v0.npz')
+    custom_cfgs = {
+        'train_cfgs': {
+            'total_steps': 4,
+            'torch_threads': 4,
+            'dataset': dataset,
+        },
+        'algo_cfgs': {
+            'batch_size': 10,
+            'steps_per_epoch': 2,
+            'fn_type': fn_type,
+        },
+    }
+    agent = omnisafe.Agent('COptiDICE', env_id, custom_cfgs=custom_cfgs)
+    agent.learn()
+
+
 @helpers.parametrize(algo=['PPO', 'SAC', 'PPOLag'])
 def test_workflow_for_training(algo):
     """Test base algorithms."""
     env_id = 'Simple-v0'
     custom_cfgs = {
         'train_cfgs': {
             'total_steps': 200,
@@ -478,190 +560,14 @@
             'exploration_noise_anneal': True,
         },
     }
     agent = omnisafe.Agent('PPO', env_id, custom_cfgs=custom_cfgs)
     agent.learn()
 
 
-# @helpers.parametrize(algo=['PPOLag'])
-# def test_cuda(algo):
-#    """Test std_anealing."""
-#    env_id = 'Simple-v0'
-#    custom_cfgs = {
-#        'train_cfgs': {
-#            'total_steps': 200,
-#            'vector_env_nums': 1,
-#            'torch_threads': 4,
-#            'device': 'cuda:0',
-#        },
-#        'algo_cfgs': {
-#            'steps_per_epoch': 100,
-#            'update_iters': 2,
-#        },
-#        'logger_cfgs': {
-#            'use_wandb': False,
-#            'save_model_freq': 1,
-#        },
-#    }
-#    agent = omnisafe.Agent(algo, env_id, custom_cfgs=custom_cfgs)
-#    agent.learn()
-
-
-# @helpers.parametrize(off_policy_algo=omnisafe.ALGORITHMS['off-policy'])
-# def test_off_policy(off_policy_algo):
-#     """Test off policy algorithms."""
-#     env_id = 'SafetyHumanoidVelocity-v1'
-#     custom_cfgs = {
-#         'epochs': 1,
-#         'steps_per_epoch': 1000,
-#         'update_after': 999,
-#         'update_every': 1,
-#         'use_wandb': False,
-#     }
-#     agent = omnisafe.Agent(off_policy_algo, env_id, custom_cfgs=custom_cfgs, parallel=1)
-#     agent.learn()
-
-
-# @helpers.parametrize(algo=naive_lagrange_policy)
-# def test_naive_lagrange_policy(algo):
-#     """Test naive lagrange algorithms."""
-#     env_id = 'SafetyHumanoidVelocity-v1'
-#     custom_cfgs = {
-#         'epochs': 1,
-#         'steps_per_epoch': 1000,
-#         'pi_iters': 1,
-#         'critic_iters': 1,
-#         'env_cfgs': {'num_envs': 1},
-#         'use_wandb': False,
-#     }
-#     agent = omnisafe.Agent(algo, env_id, custom_cfgs=custom_cfgs, parallel=1)
-#     agent.learn()
-
-
-# @helpers.parametrize(algo=first_order_policy)
-# def test_first_order_policy(algo):
-#     """Test first order algorithms."""
-#     env_id = 'SafetyHumanoidVelocity-v1'
-#     custom_cfgs = {
-#         'epochs': 1,
-#         'steps_per_epoch': 1000,
-#         'pi_iters': 1,
-#         'critic_iters': 1,
-#         'env_cfgs': {'num_envs': 1},
-#         'use_wandb': False,
-#     }
-#     agent = omnisafe.Agent(algo, env_id, custom_cfgs=custom_cfgs, parallel=1)
-#     agent.learn()
-
-
-# @helpers.parametrize(algo=second_order_policy)
-# def test_second_order_policy(algo):
-#     """Test second order algorithms."""
-#     env_id = 'SafetyHumanoidVelocity-v1'
-#     custom_cfgs = {
-#         'epochs': 1,
-#         'steps_per_epoch': 1000,
-#         'pi_iters': 1,
-#         'critic_iters': 1,
-#         'env_cfgs': {'num_envs': 1},
-#         'cost_limit': 0.01,
-#         'use_wandb': False,
-#     }
-#     agent = omnisafe.Agent(algo, env_id, custom_cfgs=custom_cfgs, parallel=1)
-#     agent.learn()
-
-
-# @helpers.parametrize(algo=pid_lagrange_policy)
-# def test_pid_lagrange_policy(algo):
-#     """Test pid lagrange algorithms."""
-#     env_id = 'SafetyHumanoidVelocity-v1'
-#     custom_cfgs = {
-#         'epochs': 1,
-#         'steps_per_epoch': 1000,
-#         'pi_iters': 1,
-#         'critic_iters': 1,
-#         'env_cfgs': {'num_envs': 1},
-#         'use_wandb': False,
-#     }
-#     agent = omnisafe.Agent(algo, env_id, custom_cfgs=custom_cfgs, parallel=1)
-#     agent.learn()
-
-
-# @helpers.parametrize(algo=penalty_policy)
-# def test_penalty_policy(algo):
-#     """Test penalty algorithms."""
-#     env_id = 'SafetyHumanoidVelocity-v1'
-#     custom_cfgs = {
-#         'epochs': 1,
-#         'steps_per_epoch': 1000,
-#         'pi_iters': 1,
-#         'critic_iters': 1,
-#         'env_cfgs': {'num_envs': 1},
-#         'parallel': 2,
-#         'cost_limit': 0.01,
-#         'use_wandb': False,
-#     }
-#     agent = omnisafe.Agent(algo, env_id, custom_cfgs=custom_cfgs, parallel=1)
-#     agent.learn()
-
-
-# @helpers.parametrize(algo=early_terminated_policy)
-# def test_early_terminated_policy(algo):
-#     """Test early terminated algorithms."""
-#     env_id = 'SafetyHumanoidVelocity-v1'
-#     custom_cfgs = {
-#         'epochs': 1,
-#         'steps_per_epoch': 1000,
-#         'pi_iters': 1,
-#         'critic_iters': 1,
-#         'env_cfgs': {'num_envs': 1},
-#         'use_wandb': False,
-#     }
-#     agent = omnisafe.Agent(algo, env_id, custom_cfgs=custom_cfgs, parallel=1)
-#     agent.learn()
-
-
-# @helpers.parametrize(algo=saute_policy)
-# def test_saute_policy(algo):
-#     """Test Saute algorithms."""
-#     env_id = 'SafetyHumanoidVelocity-v1'
-#     custom_cfgs = {
-#         'epochs': 1,
-#         'steps_per_epoch': 1000,
-#         'pi_iters': 1,
-#         'critic_iters': 1,
-#         'env_cfgs': {'num_envs': 1},
-#         'use_wandb': False,
-#     }
-#     agent = omnisafe.Agent(algo, env_id, custom_cfgs=custom_cfgs, parallel=1)
-#     agent.learn()
-
-
-# @helpers.parametrize(algo=simmer_policy)
-# def test_simmer_policy(algo):
-#     """Test Simmer algorithms."""
-#     env_id = 'SafetyHumanoidVelocity-v1'
-#     custom_cfgs = {
-#         'epochs': 1,
-#         'steps_per_epoch': 1000,
-#         'pi_iters': 1,
-#         'critic_iters': 1,
-#         'env_cfgs': {'num_envs': 1},
-#         'use_wandb': False,
-#     }
-#     agent = omnisafe.Agent(algo, env_id, custom_cfgs=custom_cfgs, parallel=1)
-#     agent.learn()
-
-
-# def test_evaluate_saved_policy():
-#     """Test evaluate policy."""
-#     DIR = os.path.join(os.path.dirname(__file__), 'saved_policy')
-#     evaluator = omnisafe.Evaluator()
-#     for algo in os.scandir(DIR):
-#         algo_path = os.path.join(DIR, algo)
-#         for exp in os.scandir(algo_path):
-#             exp_path = os.path.join(algo_path, exp)
-#             for item in os.scandir(os.path.join(exp_path, 'torch_save')):
-#                 if item.is_file() and item.name.split('.')[-1] == 'pt':
-#                     evaluator.load_saved_model(save_dir=exp_path, model_name=item.name)
-#                     evaluator.evaluate(num_episodes=1)
-#                     evaluator.render(num_episode=1, camera_name='track', width=256, height=256)
+def teardown_module():
+    """teardown_module."""
+    # remove runs folder
+    current_path = os.path.dirname(os.path.abspath(__file__))
+    runs_path = os.path.join(current_path, 'runs')
+    if os.path.exists(runs_path):
+        os.system(f'rm -rf {runs_path}')
```

### Comparing `omnisafe-0.4.0/tests/test_registry.py` & `omnisafe-0.5.0b0/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.4.0/tests/test_statistics_tools.py` & `omnisafe-0.5.0b0/tests/test_statistics_tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Test analyzing policies trained by exp-x with OmniSafe."""
 
+import pytest
+
 from omnisafe.common.statistics_tools import StatisticsTools
 
 
 def test_statistics_tools():
     # just fill in the path in which experiment grid runs.
     path = './saved_source/test_statistics_tools'
     st = StatisticsTools()
@@ -25,7 +27,10 @@
     # just fill in the name of the parameter of which value you want to compare.
     # then you can specify the value of the parameter you want to compare,
     # or you can just specify how many values you want to compare in single graph at most,
     # and the function will automatically generate all possible combinations of the graph.
     # but the two mode can not be used at the same time.
     st.draw_graph('algo', None, 1)
     st.draw_graph('algo', ['PolicyGradient'], None)
+    not_a_path = 'not_a_path'
+    with pytest.raises(SystemExit):
+        st.load_source(not_a_path)
```

### Comparing `omnisafe-0.4.0/tests/test_utils.py` & `omnisafe-0.5.0b0/tests/test_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,53 @@
-# Copyright 2022-2023 OmniSafe Team. All Rights Reserved.
+# Copyright 2023 OmniSafe Team. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Test utils"""
+"""Test utils."""
 
 from __future__ import annotations
 
+import os
+
 import pytest
 import torch
 from torch import nn
 from torch.distributions import Normal
 
 import helpers
-from omnisafe.common.experiment_grid import ExperimentGrid
 from omnisafe.typing import Activation, InitFunction
 from omnisafe.utils.config import Config, check_all_configs, get_default_kwargs_yaml
 from omnisafe.utils.distributed import fork
 from omnisafe.utils.exp_grid_tools import train
 from omnisafe.utils.math import (
     SafeTanhTransformer,
     TanhNormal,
     discount_cumsum,
     get_diagonal,
     get_transpose,
 )
 from omnisafe.utils.model import get_activation, initialize_layer
 from omnisafe.utils.schedule import ConstantSchedule, PiecewiseSchedule
-from omnisafe.utils.tools import assert_with_exit, custom_cfgs_to_dict, update_dict
+from omnisafe.utils.tools import (
+    assert_with_exit,
+    custom_cfgs_to_dict,
+    load_yaml,
+    recursive_check_config,
+    update_dict,
+)
 
 
 def test_update_dict():
     d = {'a': 1, 'b': {'c': 2}}
     update_dict(d, {'a': 2, 'b': {'d': 3}, 'e': {'f': 4}})
     assert d == {'a': 2, 'b': {'c': 2, 'd': 3}, 'e': {'f': 4}}
 
@@ -134,22 +141,38 @@
 
 def test_train(
     exp_name='make_test_exp_grid',
     algo='CPO',
     env_id='SafetyHalfCheetahVelocity-v1',
 ):
     """Test train."""
-    eg = ExperimentGrid(exp_name=exp_name)
-    eg.add('algo', [algo])
-    eg.add('env_id', [env_id])
-    eg.add('logger_cfgs:use_wandb', [False])
-    eg.add('algo_cfgs:steps_per_epoch', [512])
-    eg.add('train_cfgs:total_steps', [1024, 2048])
-    eg.add('train_cfgs:vector_env_nums', [1])
-    eg.run(train, num_pool=1, is_test=True)
+    custom_cfgs = {
+        'train_cfgs': {
+            'total_steps': 200,
+            'vector_env_nums': 1,
+            'torch_threads': 4,
+        },
+        'algo_cfgs': {
+            'steps_per_epoch': 100,
+            'update_iters': 2,
+        },
+        'logger_cfgs': {
+            'use_wandb': False,
+            'save_model_freq': 1,
+            'log_dir': 'saved_log',
+        },
+    }
+    train(
+        exp_id=exp_name,
+        algo=algo,
+        env_id=env_id,
+        custom_cfgs=custom_cfgs,
+    )
+    # delete the saved data
+    os.system('rm -rf saved_log')
 
 
 @helpers.parametrize(
     init_function=['kaiming_uniform', 'xavier_normal', 'glorot', 'xavier_uniform', 'orthogonal'],
 )
 def test_initalize(init_function: InitFunction):
     """Test initialize."""
@@ -172,7 +195,37 @@
     constant = ConstantSchedule(1)
     assert constant.value(1) == 1
 
     endpoints = [(0, 0.0), (2, 1.0)]
     piece = PiecewiseSchedule(endpoints, outside_value=0)
     assert piece.value(1) == 0.5
     assert piece.value(100) == 0
+
+
+def teardown_module():
+    """teardown_module."""
+    # remove runs folder
+    current_path = os.path.dirname(os.path.abspath(__file__))
+    runs_path = os.path.join(current_path, 'runs')
+    if os.path.exists(runs_path):
+        os.system(f'rm -rf {runs_path}')
+
+    # remove exp-x folder
+    exp_x_path = os.path.join(current_path, 'exp-x')
+    if os.path.exists(exp_x_path):
+        os.system(f'rm -rf {exp_x_path}')
+
+    # remove png
+    os.system(f'rm -rf {current_path}/algo--*.png')
+
+
+def test_load_yaml():
+    not_a_path = 'not_a_path'
+    with pytest.raises(FileNotFoundError):
+        load_yaml(not_a_path)
+
+
+def test_recursive_check_config():
+    config = {'a': 1, 'b': {'c': 2, 'd': {'e': 3}}, 'not_exist': 1}
+    default_config = {'a': 1, 'b': {'c': 2, 'd': {'e': 3, 'f': 4}}}
+    with pytest.raises(KeyError):
+        recursive_check_config(config, default_config)
```

