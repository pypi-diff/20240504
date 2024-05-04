# Comparing `tmp/omnisafe-0.5.0b0.tar.gz` & `tmp/omnisafe-0.5.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnisafe-0.5.0b0.tar", last modified: Thu Jun  1 18:21:46 2023, max compression
+gzip compressed data, was "omnisafe-0.5.1b0.tar", last modified: Sat May  4 08:35:44 2024, max compression
```

## Comparing `omnisafe-0.5.0b0.tar` & `omnisafe-0.5.1b0.tar`

### file list

```diff
@@ -1,245 +1,246 @@
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.641961 omnisafe-0.5.0b0/
--rw-r--r--   0 jiaming    (501) staff       (20)    11375 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/LICENSE
--rw-r--r--   0 jiaming    (501) staff       (20)       43 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/MANIFEST.in
--rw-r--r--   0 jiaming    (501) staff       (20)    19458 2023-06-01 18:21:46.641733 omnisafe-0.5.0b0/PKG-INFO
--rw-r--r--   0 jiaming    (501) staff       (20)    18243 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/README.md
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.613420 omnisafe-0.5.0b0/omnisafe/
--rw-r--r--   0 jiaming    (501) staff       (20)      992 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/__init__.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.615841 omnisafe-0.5.0b0/omnisafe/adapter/
--rw-r--r--   0 jiaming    (501) staff       (20)     1235 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/adapter/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3395 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/adapter/early_terminated_adapter.py
--rw-r--r--   0 jiaming    (501) staff       (20)    15567 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/adapter/modelbased_adapter.py
--rw-r--r--   0 jiaming    (501) staff       (20)     5045 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/adapter/offline_adapter.py
--rw-r--r--   0 jiaming    (501) staff       (20)     7703 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/adapter/offpolicy_adapter.py
--rw-r--r--   0 jiaming    (501) staff       (20)     7691 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/adapter/online_adapter.py
--rw-r--r--   0 jiaming    (501) staff       (20)     6745 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/adapter/onpolicy_adapter.py
--rw-r--r--   0 jiaming    (501) staff       (20)     9709 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/adapter/saute_adapter.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4995 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/adapter/simmer_adapter.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.616594 omnisafe-0.5.0b0/omnisafe/algorithms/
--rw-r--r--   0 jiaming    (501) staff       (20)     2286 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)    10682 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/algo_wrapper.py
--rw-r--r--   0 jiaming    (501) staff       (20)     2567 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/base_algo.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.617226 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/
--rw-r--r--   0 jiaming    (501) staff       (20)     1161 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/__init__.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.617774 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/base/
--rw-r--r--   0 jiaming    (501) staff       (20)      887 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/base/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)    35440 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/base/ensemble.py
--rw-r--r--   0 jiaming    (501) staff       (20)    20235 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/base/loop.py
--rw-r--r--   0 jiaming    (501) staff       (20)    23759 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/base/pets.py
--rw-r--r--   0 jiaming    (501) staff       (20)     6872 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/cap_pets.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4844 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/cce_pets.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.618636 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/planner/
--rw-r--r--   0 jiaming    (501) staff       (20)     1247 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/planner/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)    12841 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/planner/arc.py
--rw-r--r--   0 jiaming    (501) staff       (20)     7115 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/planner/cap.py
--rw-r--r--   0 jiaming    (501) staff       (20)     6158 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/planner/cce.py
--rw-r--r--   0 jiaming    (501) staff       (20)    11612 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/planner/cem.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4953 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/planner/rce.py
--rw-r--r--   0 jiaming    (501) staff       (20)    10712 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/planner/safe_arc.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4852 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/rce_pets.py
--rw-r--r--   0 jiaming    (501) staff       (20)     5305 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/model_based/safeloop.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.620046 omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/
--rw-r--r--   0 jiaming    (501) staff       (20)     1314 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)    23856 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/ddpg.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4108 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/ddpg_lag.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3913 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/ddpg_pid.py
--rw-r--r--   0 jiaming    (501) staff       (20)     8201 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/sac.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4128 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/sac_lag.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4065 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/sac_pid.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4716 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/td3.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3978 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/td3_lag.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3955 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/td3_pid.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.621507 omnisafe-0.5.0b0/omnisafe/algorithms/offline/
--rw-r--r--   0 jiaming    (501) staff       (20)     1089 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/offline/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)     5806 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/offline/base.py
--rw-r--r--   0 jiaming    (501) staff       (20)     8828 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/offline/bcq.py
--rw-r--r--   0 jiaming    (501) staff       (20)     7842 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/offline/bcq_lag.py
--rw-r--r--   0 jiaming    (501) staff       (20)     8291 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/offline/c_crr.py
--rw-r--r--   0 jiaming    (501) staff       (20)    12636 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/offline/coptidice.py
--rw-r--r--   0 jiaming    (501) staff       (20)     8122 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/offline/crr.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3742 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/offline/vae_bc.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.621652 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/
--rw-r--r--   0 jiaming    (501) staff       (20)     1924 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/__init__.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.622443 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/base/
--rw-r--r--   0 jiaming    (501) staff       (20)     1064 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/base/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)     9611 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/base/natural_pg.py
--rw-r--r--   0 jiaming    (501) staff       (20)    25247 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/base/policy_gradient.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3210 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/base/ppo.py
--rw-r--r--   0 jiaming    (501) staff       (20)     9116 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/base/trpo.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.622951 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/early_terminated/
--rw-r--r--   0 jiaming    (501) staff       (20)     1013 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/early_terminated/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)     2462 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/early_terminated/ppo_early_terminated.py
--rw-r--r--   0 jiaming    (501) staff       (20)     2368 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/early_terminated/trpo_early_terminated.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.623450 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/first_order/
--rw-r--r--   0 jiaming    (501) staff       (20)      882 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/first_order/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)     8793 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/first_order/cup.py
--rw-r--r--   0 jiaming    (501) staff       (20)     8476 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/first_order/focops.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.624190 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/naive_lagrange/
--rw-r--r--   0 jiaming    (501) staff       (20)     1060 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/naive_lagrange/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3974 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/naive_lagrange/pdo.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4043 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/naive_lagrange/ppo_lag.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4114 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/naive_lagrange/rcpo.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3958 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/naive_lagrange/trpo_lag.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.624661 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/penalty_function/
--rw-r--r--   0 jiaming    (501) staff       (20)      886 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/penalty_function/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)     2875 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/penalty_function/ipo.py
--rw-r--r--   0 jiaming    (501) staff       (20)     5162 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/penalty_function/p3o.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.625093 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/pid_lagrange/
--rw-r--r--   0 jiaming    (501) staff       (20)      902 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/pid_lagrange/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4110 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/pid_lagrange/cppo_pid.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3958 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/pid_lagrange/trpo_pid.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.625394 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/primal/
--rw-r--r--   0 jiaming    (501) staff       (20)      797 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/primal/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3040 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/primal/crpo.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.625800 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/saute/
--rw-r--r--   0 jiaming    (501) staff       (20)      913 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/saute/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)     2922 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/saute/ppo_saute.py
--rw-r--r--   0 jiaming    (501) staff       (20)     2934 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/saute/trpo_saute.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.626186 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/second_order/
--rw-r--r--   0 jiaming    (501) staff       (20)      879 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/second_order/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)    19058 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/second_order/cpo.py
--rw-r--r--   0 jiaming    (501) staff       (20)     5867 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/second_order/pcpo.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.626550 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/simmer/
--rw-r--r--   0 jiaming    (501) staff       (20)      942 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/simmer/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3211 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/simmer/ppo_simmer_pid.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3223 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/simmer/trpo_simmer_pid.py
--rw-r--r--   0 jiaming    (501) staff       (20)     2220 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/algorithms/registry.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.627572 omnisafe-0.5.0b0/omnisafe/common/
--rw-r--r--   0 jiaming    (501) staff       (20)      918 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/__init__.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.628353 omnisafe-0.5.0b0/omnisafe/common/buffer/
--rw-r--r--   0 jiaming    (501) staff       (20)     1194 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/buffer/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)     5221 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/buffer/base.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4184 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/buffer/offpolicy_buffer.py
--rw-r--r--   0 jiaming    (501) staff       (20)    18534 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/buffer/onpolicy_buffer.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4914 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/buffer/vector_offpolicy_buffer.py
--rw-r--r--   0 jiaming    (501) staff       (20)     5346 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/buffer/vector_onpolicy_buffer.py
--rw-r--r--   0 jiaming    (501) staff       (20)    26545 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/experiment_grid.py
--rw-r--r--   0 jiaming    (501) staff       (20)     5266 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/lagrange.py
--rw-r--r--   0 jiaming    (501) staff       (20)    14965 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/logger.py
--rw-r--r--   0 jiaming    (501) staff       (20)     5837 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/normalizer.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.628737 omnisafe-0.5.0b0/omnisafe/common/offline/
--rw-r--r--   0 jiaming    (501) staff       (20)      893 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/offline/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)     8201 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/offline/data_collector.py
--rw-r--r--   0 jiaming    (501) staff       (20)    18021 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/offline/dataset.py
--rw-r--r--   0 jiaming    (501) staff       (20)     5165 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/pid_lagrange.py
--rw-r--r--   0 jiaming    (501) staff       (20)     7026 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/simmer_agent.py
--rw-r--r--   0 jiaming    (501) staff       (20)    16468 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/common/statistics_tools.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.611028 omnisafe-0.5.0b0/omnisafe/configs/
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.629517 omnisafe-0.5.0b0/omnisafe/configs/model-based/
--rw-r--r--   0 jiaming    (501) staff       (20)     5127 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/model-based/CAPPETS.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     4822 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/model-based/CCEPETS.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     6646 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/model-based/LOOP.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     4656 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/model-based/PETS.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     4825 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/model-based/RCEPETS.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     6757 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/model-based/SafeLOOP.yaml
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.630812 omnisafe-0.5.0b0/omnisafe/configs/off-policy/
--rw-r--r--   0 jiaming    (501) staff       (20)     4361 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/off-policy/DDPG.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     6025 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/off-policy/DDPGLag.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     6434 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/off-policy/DDPGPID.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     4905 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/off-policy/SAC.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     6757 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/off-policy/SACLag.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     6810 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/off-policy/SACPID.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     4457 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/off-policy/TD3.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     6477 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/off-policy/TD3Lag.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     6530 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/off-policy/TD3PID.yaml
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.631587 omnisafe-0.5.0b0/omnisafe/configs/offline/
--rw-r--r--   0 jiaming    (501) staff       (20)     2760 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/offline/BCQ.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3201 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/offline/BCQLag.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3141 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/offline/CCRR.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3371 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/offline/COptiDICE.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     2754 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/offline/CRR.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     2142 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/offline/VAEBC.yaml
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.634587 omnisafe-0.5.0b0/omnisafe/configs/on-policy/
--rw-r--r--   0 jiaming    (501) staff       (20)     3787 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/CPO.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     4349 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/CPPOPID.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3918 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/CUP.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     4088 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/FOCOPS.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3986 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/IPO.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3761 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/NaturalPG.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3613 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/OnCRPO.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3612 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/P3O.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3787 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/PCPO.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3809 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/PDO.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3521 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/PPO.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3582 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/PPOEarlyTerminated.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3841 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/PPOLag.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3762 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/PPOSaute.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     4063 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/PPOSimmerPID.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3490 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/PolicyGradient.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     4050 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/RCPO.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3730 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/TRPO.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3791 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/TRPOEarlyTerminated.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     4050 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/TRPOLag.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     4589 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/TRPOPID.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     3971 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/TRPOSaute.yaml
--rw-r--r--   0 jiaming    (501) staff       (20)     4272 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/configs/on-policy/TRPOSimmerPID.yaml
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.635342 omnisafe-0.5.0b0/omnisafe/envs/
--rw-r--r--   0 jiaming    (501) staff       (20)      980 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/envs/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)    12724 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/envs/core.py
--rw-r--r--   0 jiaming    (501) staff       (20)     6402 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/envs/mujoco_env.py
--rw-r--r--   0 jiaming    (501) staff       (20)     8218 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/envs/safety_gymnasium_env.py
--rw-r--r--   0 jiaming    (501) staff       (20)    20570 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/envs/safety_gymnasium_modelbased.py
--rw-r--r--   0 jiaming    (501) staff       (20)    22475 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/envs/wrapper.py
--rw-r--r--   0 jiaming    (501) staff       (20)    22578 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/evaluator.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.635614 omnisafe-0.5.0b0/omnisafe/models/
--rw-r--r--   0 jiaming    (501) staff       (20)     1731 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/__init__.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.636546 omnisafe-0.5.0b0/omnisafe/models/actor/
--rw-r--r--   0 jiaming    (501) staff       (20)     1207 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/actor/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4928 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/actor/actor_builder.py
--rw-r--r--   0 jiaming    (501) staff       (20)     1407 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/actor/gaussian_actor.py
--rw-r--r--   0 jiaming    (501) staff       (20)     5292 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/actor/gaussian_learning_actor.py
--rw-r--r--   0 jiaming    (501) staff       (20)     6527 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/actor/gaussian_sac_actor.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4531 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/actor/mlp_actor.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4122 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/actor/perturbation_actor.py
--rw-r--r--   0 jiaming    (501) staff       (20)     5516 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/actor/vae_actor.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.637119 omnisafe-0.5.0b0/omnisafe/models/actor_critic/
--rw-r--r--   0 jiaming    (501) staff       (20)     1030 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/actor_critic/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)     7299 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/actor_critic/actor_critic.py
--rw-r--r--   0 jiaming    (501) staff       (20)     7107 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/actor_critic/actor_q_critic.py
--rw-r--r--   0 jiaming    (501) staff       (20)     5177 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/actor_critic/constraint_actor_critic.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4427 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/actor_critic/constraint_actor_q_critic.py
--rw-r--r--   0 jiaming    (501) staff       (20)     8341 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/base.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.637672 omnisafe-0.5.0b0/omnisafe/models/critic/
--rw-r--r--   0 jiaming    (501) staff       (20)      930 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/critic/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4463 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/critic/critic_builder.py
--rw-r--r--   0 jiaming    (501) staff       (20)     5443 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/critic/q_critic.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3217 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/critic/v_critic.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.637942 omnisafe-0.5.0b0/omnisafe/models/offline/
--rw-r--r--   0 jiaming    (501) staff       (20)      776 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/offline/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3265 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/models/offline/dice.py
--rw-r--r--   0 jiaming    (501) staff       (20)     1709 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/typing.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.639521 omnisafe-0.5.0b0/omnisafe/utils/
--rw-r--r--   0 jiaming    (501) staff       (20)      718 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/utils/__init__.py
--rw-r--r--   0 jiaming    (501) staff       (20)    17241 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/utils/command_app.py
--rw-r--r--   0 jiaming    (501) staff       (20)    15410 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/utils/config.py
--rw-r--r--   0 jiaming    (501) staff       (20)    11396 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/utils/distributed.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3305 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/utils/exp_grid_tools.py
--rw-r--r--   0 jiaming    (501) staff       (20)     7276 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/utils/math.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4022 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/utils/model.py
--rw-r--r--   0 jiaming    (501) staff       (20)    16404 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/utils/plotter.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3828 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/utils/schedule.py
--rw-r--r--   0 jiaming    (501) staff       (20)    12016 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/omnisafe/utils/tools.py
--rw-r--r--   0 jiaming    (501) staff       (20)     1833 2023-06-01 18:21:33.000000 omnisafe-0.5.0b0/omnisafe/version.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.614242 omnisafe-0.5.0b0/omnisafe.egg-info/
--rw-r--r--   0 jiaming    (501) staff       (20)    19458 2023-06-01 18:21:46.000000 omnisafe-0.5.0b0/omnisafe.egg-info/PKG-INFO
--rw-r--r--   0 jiaming    (501) staff       (20)     7968 2023-06-01 18:21:46.000000 omnisafe-0.5.0b0/omnisafe.egg-info/SOURCES.txt
--rw-r--r--   0 jiaming    (501) staff       (20)        1 2023-06-01 18:21:46.000000 omnisafe-0.5.0b0/omnisafe.egg-info/dependency_links.txt
--rw-r--r--   0 jiaming    (501) staff       (20)       60 2023-06-01 18:21:46.000000 omnisafe-0.5.0b0/omnisafe.egg-info/entry_points.txt
--rw-r--r--   0 jiaming    (501) staff       (20)      392 2023-06-01 18:21:46.000000 omnisafe-0.5.0b0/omnisafe.egg-info/requires.txt
--rw-r--r--   0 jiaming    (501) staff       (20)        9 2023-06-01 18:21:46.000000 omnisafe-0.5.0b0/omnisafe.egg-info/top_level.txt
--rw-r--r--   0 jiaming    (501) staff       (20)     5348 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/pyproject.toml
--rw-r--r--   0 jiaming    (501) staff       (20)       38 2023-06-01 18:21:46.642014 omnisafe-0.5.0b0/setup.cfg
--rw-r--r--   0 jiaming    (501) staff       (20)      988 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/setup.py
-drwxr-xr-x   0 jiaming    (501) staff       (20)        0 2023-06-01 18:21:46.641420 omnisafe-0.5.0b0/tests/
--rw-r--r--   0 jiaming    (501) staff       (20)    15872 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/tests/test_buffer.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3294 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/tests/test_cli.py
--rw-r--r--   0 jiaming    (501) staff       (20)     2552 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/tests/test_ensemble.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4476 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/tests/test_env.py
--rw-r--r--   0 jiaming    (501) staff       (20)     3735 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/tests/test_experiment_grid.py
--rw-r--r--   0 jiaming    (501) staff       (20)     7110 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/tests/test_model.py
--rw-r--r--   0 jiaming    (501) staff       (20)     1560 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/tests/test_normalizer.py
--rw-r--r--   0 jiaming    (501) staff       (20)     4951 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/tests/test_offline_data.py
--rw-r--r--   0 jiaming    (501) staff       (20)    16357 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/tests/test_policy.py
--rw-r--r--   0 jiaming    (501) staff       (20)     1045 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/tests/test_registry.py
--rw-r--r--   0 jiaming    (501) staff       (20)     1594 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/tests/test_statistics_tools.py
--rw-r--r--   0 jiaming    (501) staff       (20)     7140 2023-06-01 18:20:21.000000 omnisafe-0.5.0b0/tests/test_utils.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.200066 omnisafe-0.5.1b0/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    11375 2023-02-09 04:07:21.000000 omnisafe-0.5.1b0/LICENSE
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)       43 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/MANIFEST.in
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    23065 2024-05-04 08:35:44.199807 omnisafe-0.5.1b0/PKG-INFO
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    20831 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/README.md
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.155121 omnisafe-0.5.1b0/omnisafe/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)      992 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/__init__.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.158016 omnisafe-0.5.1b0/omnisafe/adapter/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     1235 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/adapter/__init__.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3395 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/adapter/early_terminated_adapter.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    15567 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/adapter/modelbased_adapter.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     5349 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/adapter/offline_adapter.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     7813 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/adapter/offpolicy_adapter.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     8885 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/adapter/online_adapter.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     6827 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/adapter/onpolicy_adapter.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    10013 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/adapter/saute_adapter.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     5393 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/adapter/simmer_adapter.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.160130 omnisafe-0.5.1b0/omnisafe/algorithms/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     2286 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/__init__.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    11074 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/algo_wrapper.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     2567 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/base_algo.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.161070 omnisafe-0.5.1b0/omnisafe/algorithms/model_based/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     1161 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/model_based/__init__.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.162871 omnisafe-0.5.1b0/omnisafe/algorithms/model_based/base/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)      887 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/model_based/base/__init__.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    35547 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/model_based/base/ensemble.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    20202 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/model_based/base/loop.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    23755 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/model_based/base/pets.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     6872 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/model_based/cap_pets.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     4844 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/model_based/cce_pets.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.164543 omnisafe-0.5.1b0/omnisafe/algorithms/model_based/planner/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     1247 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/model_based/planner/__init__.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    12823 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/model_based/planner/arc.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     7115 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/model_based/planner/cap.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     6158 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/model_based/planner/cce.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    11600 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/model_based/planner/cem.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     4953 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/model_based/planner/rce.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    10688 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/model_based/planner/safe_arc.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     4852 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/model_based/rce_pets.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     5305 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/model_based/safeloop.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.167479 omnisafe-0.5.1b0/omnisafe/algorithms/off_policy/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     1314 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/off_policy/__init__.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    23909 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/off_policy/ddpg.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     4108 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/off_policy/ddpg_lag.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3913 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/off_policy/ddpg_pid.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     8098 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/off_policy/sac.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     4128 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/off_policy/sac_lag.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     4065 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/off_policy/sac_pid.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     4613 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/off_policy/td3.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3978 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/off_policy/td3_lag.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3955 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/off_policy/td3_pid.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.169986 omnisafe-0.5.1b0/omnisafe/algorithms/offline/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     1089 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/offline/__init__.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     5806 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/offline/base.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     8828 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/offline/bcq.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     7842 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/offline/bcq_lag.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     8291 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/offline/c_crr.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    12636 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/offline/coptidice.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     8122 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/offline/crr.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3732 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/offline/vae_bc.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.170156 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     1924 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/__init__.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.171296 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/base/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     1064 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/base/__init__.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     9611 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/base/natural_pg.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    25512 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/base/policy_gradient.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3210 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/base/ppo.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     9147 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/base/trpo.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.172141 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/early_terminated/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     1013 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/early_terminated/__init__.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     2462 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/early_terminated/ppo_early_terminated.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     2368 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/early_terminated/trpo_early_terminated.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.172633 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/first_order/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)      882 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/first_order/__init__.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     8776 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/first_order/cup.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     8466 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/first_order/focops.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.173376 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/naive_lagrange/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     1060 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/naive_lagrange/__init__.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3974 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/naive_lagrange/pdo.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     4043 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/naive_lagrange/ppo_lag.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     4114 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/naive_lagrange/rcpo.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3958 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/naive_lagrange/trpo_lag.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.173802 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/penalty_function/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)      886 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/penalty_function/__init__.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     2875 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/penalty_function/ipo.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     5162 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/penalty_function/p3o.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.174359 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/pid_lagrange/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)      902 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/pid_lagrange/__init__.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     4110 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/pid_lagrange/cppo_pid.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3958 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/pid_lagrange/trpo_pid.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.174912 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/primal/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)      797 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/primal/__init__.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3216 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/primal/crpo.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.175366 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/saute/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)      913 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/saute/__init__.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     2922 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/saute/ppo_saute.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     2934 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/saute/trpo_saute.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.175878 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/second_order/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)      879 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/second_order/__init__.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    19044 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/second_order/cpo.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     5848 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/second_order/pcpo.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.176345 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/simmer/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)      942 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/simmer/__init__.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3211 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/simmer/ppo_simmer_pid.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3223 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/simmer/trpo_simmer_pid.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     2220 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/algorithms/registry.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.177727 omnisafe-0.5.1b0/omnisafe/common/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)      918 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/common/__init__.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.179248 omnisafe-0.5.1b0/omnisafe/common/buffer/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     1194 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/common/buffer/__init__.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     5221 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/common/buffer/base.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     4184 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/common/buffer/offpolicy_buffer.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    18534 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/common/buffer/onpolicy_buffer.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     4914 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/common/buffer/vector_offpolicy_buffer.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     5346 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/common/buffer/vector_onpolicy_buffer.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    26610 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/common/experiment_grid.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     5266 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/common/lagrange.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    15019 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/common/logger.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     5807 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/common/normalizer.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.179826 omnisafe-0.5.1b0/omnisafe/common/offline/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)      893 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/common/offline/__init__.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     8201 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/common/offline/data_collector.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    18059 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/common/offline/dataset.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     5154 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/common/pid_lagrange.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     7026 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/common/simmer_agent.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    16468 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/common/statistics_tools.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.152674 omnisafe-0.5.1b0/omnisafe/configs/
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.181677 omnisafe-0.5.1b0/omnisafe/configs/model-based/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     5127 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/model-based/CAPPETS.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     4822 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/model-based/CCEPETS.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     6646 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/model-based/LOOP.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     4656 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/model-based/PETS.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     4825 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/model-based/RCEPETS.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     6757 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/model-based/SafeLOOP.yaml
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.183817 omnisafe-0.5.1b0/omnisafe/configs/off-policy/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     4416 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/off-policy/DDPG.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     6080 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/off-policy/DDPGLag.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     6489 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/off-policy/DDPGPID.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     4960 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/off-policy/SAC.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     6812 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/off-policy/SACLag.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     6865 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/off-policy/SACPID.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     4512 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/off-policy/TD3.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     6532 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/off-policy/TD3Lag.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     6585 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/off-policy/TD3PID.yaml
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.184978 omnisafe-0.5.1b0/omnisafe/configs/offline/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     2760 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/offline/BCQ.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3201 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/offline/BCQLag.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3141 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/offline/CCRR.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3371 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/offline/COptiDICE.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     2754 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/offline/CRR.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     2142 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/offline/VAEBC.yaml
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.189106 omnisafe-0.5.1b0/omnisafe/configs/on-policy/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3787 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/on-policy/CPO.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     4349 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/on-policy/CPPOPID.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3918 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/on-policy/CUP.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     4088 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/on-policy/FOCOPS.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3986 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/on-policy/IPO.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3761 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/on-policy/NaturalPG.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3823 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/on-policy/OnCRPO.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3612 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/on-policy/P3O.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3787 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/on-policy/PCPO.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3809 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/on-policy/PDO.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3521 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/on-policy/PPO.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3582 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/on-policy/PPOEarlyTerminated.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3896 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/on-policy/PPOLag.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     5934 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/on-policy/PPOSaute.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     5749 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/on-policy/PPOSimmerPID.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3490 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/on-policy/PolicyGradient.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     4050 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/on-policy/RCPO.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3730 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/on-policy/TRPO.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3791 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/on-policy/TRPOEarlyTerminated.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     4050 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/on-policy/TRPOLag.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     4589 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/on-policy/TRPOPID.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     5379 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/on-policy/TRPOSaute.yaml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     5684 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/configs/on-policy/TRPOSimmerPID.yaml
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.190528 omnisafe-0.5.1b0/omnisafe/envs/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     1027 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/envs/__init__.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    13351 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/envs/core.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     8301 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/envs/custom_env.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     6476 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/envs/mujoco_env.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     9035 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/envs/safety_gymnasium_env.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    20545 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/envs/safety_gymnasium_modelbased.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    22974 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/envs/wrapper.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    22798 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/evaluator.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.190918 omnisafe-0.5.1b0/omnisafe/models/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     1731 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/models/__init__.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.192618 omnisafe-0.5.1b0/omnisafe/models/actor/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     1207 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/models/actor/__init__.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     4895 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/models/actor/actor_builder.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     1407 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/models/actor/gaussian_actor.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     5292 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/models/actor/gaussian_learning_actor.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     6660 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/models/actor/gaussian_sac_actor.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     4531 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/models/actor/mlp_actor.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     4122 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/models/actor/perturbation_actor.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     5516 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/models/actor/vae_actor.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.193353 omnisafe-0.5.1b0/omnisafe/models/actor_critic/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     1030 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/models/actor_critic/__init__.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     7089 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/models/actor_critic/actor_critic.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     6777 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/models/actor_critic/actor_q_critic.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     5177 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/models/actor_critic/constraint_actor_critic.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     4427 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/models/actor_critic/constraint_actor_q_critic.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     8341 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/models/base.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.193900 omnisafe-0.5.1b0/omnisafe/models/critic/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)      930 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/models/critic/__init__.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     4463 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/models/critic/critic_builder.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     5443 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/models/critic/q_critic.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3217 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/models/critic/v_critic.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.194171 omnisafe-0.5.1b0/omnisafe/models/offline/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)      776 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/models/offline/__init__.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3265 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/models/offline/dice.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     1709 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/typing.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.196335 omnisafe-0.5.1b0/omnisafe/utils/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)      718 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/utils/__init__.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    17241 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/utils/command_app.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    15385 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/utils/config.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    12003 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/utils/distributed.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3305 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/utils/exp_grid_tools.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     7319 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/utils/math.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3998 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/utils/model.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    16404 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/utils/plotter.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3780 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/utils/schedule.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    12082 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/omnisafe/utils/tools.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     1833 2024-05-04 08:35:39.000000 omnisafe-0.5.1b0/omnisafe/version.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.198625 omnisafe-0.5.1b0/omnisafe.egg-info/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    23065 2024-05-04 08:35:44.000000 omnisafe-0.5.1b0/omnisafe.egg-info/PKG-INFO
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     7996 2024-05-04 08:35:44.000000 omnisafe-0.5.1b0/omnisafe.egg-info/SOURCES.txt
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)        1 2024-05-04 08:35:44.000000 omnisafe-0.5.1b0/omnisafe.egg-info/dependency_links.txt
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)       60 2024-05-04 08:35:44.000000 omnisafe-0.5.1b0/omnisafe.egg-info/entry_points.txt
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)      392 2024-05-04 08:35:44.000000 omnisafe-0.5.1b0/omnisafe.egg-info/requires.txt
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)        9 2024-05-04 08:35:44.000000 omnisafe-0.5.1b0/omnisafe.egg-info/top_level.txt
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     5347 2024-04-28 17:37:30.000000 omnisafe-0.5.1b0/pyproject.toml
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)       38 2024-05-04 08:35:44.200108 omnisafe-0.5.1b0/setup.cfg
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)      988 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/setup.py
+drwxr-xr-x   0 zhoujiayi   (501) staff       (20)        0 2024-05-04 08:35:44.198425 omnisafe-0.5.1b0/tests/
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    15872 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/tests/test_buffer.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3294 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/tests/test_cli.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     2552 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/tests/test_ensemble.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     4600 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/tests/test_env.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     3735 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/tests/test_experiment_grid.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     7110 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/tests/test_model.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     1560 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/tests/test_normalizer.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     4951 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/tests/test_offline_data.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)    16323 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/tests/test_policy.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     1496 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/tests/test_registry.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     1594 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/tests/test_statistics_tools.py
+-rw-r--r--   0 zhoujiayi   (501) staff       (20)     7140 2024-04-28 17:07:20.000000 omnisafe-0.5.1b0/tests/test_utils.py
```

### Comparing `omnisafe-0.5.0b0/LICENSE` & `omnisafe-0.5.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/PKG-INFO` & `omnisafe-0.5.1b0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnisafe
-Version: 0.5.0b0
+Version: 0.5.1b0
 Summary: A comprehensive and reliable benchmark for safe reinforcement learning.
 Author: OmniSafe Contributors
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://github.com/PKU-Alignment/omnisafe
 Project-URL: Repository, https://github.com/PKU-Alignment/omnisafe
 Project-URL: Documentation, https://omnisafe.readthedocs.io
 Project-URL: Bug Report, https://github.com/PKU-Alignment/omnisafe/issues
@@ -17,17 +17,44 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: safety-gymnasium>=0.2.0
+Requires-Dist: torch>=1.10.0
+Requires-Dist: numpy>=1.20.0
+Requires-Dist: tensorboard>=2.8.0
+Requires-Dist: wandb>=0.13.0
+Requires-Dist: pyyaml>=6.0
+Requires-Dist: moviepy>=1.0.0
+Requires-Dist: typing-extensions>=4.0.0
+Requires-Dist: typer[all]>=0.7.0
+Requires-Dist: seaborn>=0.12.2
+Requires-Dist: pandas==2.0.3
+Requires-Dist: matplotlib>=3.7.1
+Requires-Dist: gdown>=4.6.0
 Provides-Extra: lint
+Requires-Dist: isort>=5.11.0; extra == "lint"
+Requires-Dist: black>=22.6.0; extra == "lint"
+Requires-Dist: pylint[spelling]>=2.15.0; extra == "lint"
+Requires-Dist: mypy>=0.990; extra == "lint"
+Requires-Dist: flake8; extra == "lint"
+Requires-Dist: flake8-bugbear; extra == "lint"
+Requires-Dist: ruff; extra == "lint"
+Requires-Dist: doc8; extra == "lint"
+Requires-Dist: pydocstyle; extra == "lint"
+Requires-Dist: pyenchant; extra == "lint"
+Requires-Dist: pre-commit; extra == "lint"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-xdist; extra == "test"
 
 <!-- markdownlint-disable first-line-h1 -->
 <!-- markdownlint-disable html -->
 
 <div align="center">
   <img src="https://github.com/PKU-Alignment/omnisafe/raw/HEAD/images/logo.png" width="75%"/>
 </div>
@@ -82,20 +109,22 @@
     - [Prerequisites](#prerequisites)
     - [Install from source](#install-from-source)
     - [Install from PyPI](#install-from-pypi)
 - [Implemented Algorithms](#implemented-algorithms)
   - [Examples](#examples)
     - [Algorithms Registry](#algorithms-registry)
     - [Supported Environments](#supported-environments)
+    - [Customizing your environment](#customizing-your-environment)
     - [Try with CLI](#try-with-cli)
 - [Getting Started](#getting-started)
   - [Important Hints](#important-hints)
   - [Quickstart: Colab on the Cloud](#quickstart-colab-on-the-cloud)
 - [Changelog](#changelog)
 - [Citing OmniSafe](#citing-omnisafe)
+- [Publications using OmniSafe](#publications-using-omnisafe)
 - [The OmniSafe Team](#the-omnisafe-team)
 - [License](#license)
 
 --------------------------------------------------------------------------------
 
 ## Quick Start
 
@@ -313,14 +342,26 @@
     <td>SafetyHumanoidVelocity-v1</td>
   </tr>
 </tbody>
 </table>
 
 For more information about environments, please refer to [Safety-Gymnasium](https://www.safety-gymnasium.com).
 
+#### Customizing your environment
+
+We offer a flexible customized environment interface that allows users to achieve the following **without modifying the OmniSafe source code**:
+
+- Use OmniSafe to train algorithms on customized environments.
+- Create the the environment with specified personalized parameters.
+- Complete the recording of environment-specific information in Logger.
+
+We provide **step-by-step tutorials** on [Environment Customization From Scratch](https://colab.research.google.com/github/PKU-Alignment/omnisafe/blob/main/tutorials/English/3.Environment%20Customization%20from%20Scratch.ipynb) and [Environment Customization From Community](https://colab.research.google.com/github/PKU-Alignment/omnisafe/blob/main/tutorials/English/4.Environment%20Customization%20from%20Community.ipynb) to give you a detailed introduction on how to use this extraordinary feature of OmniSafe.
+
+*Note: If you find trouble customizing your environment, please feel free to open an [issue](https://github.com/PKU-Alignment/omnisafe/issues) or [discussion](https://github.com/PKU-Alignment/omnisafe/discussions). [Pull requests](https://github.com/PKU-Alignment/omnisafe/pulls) are also welcomed if you're willing to contribute the implementation of your environments interface.*
+
 #### Try with CLI
 
 ```bash
 pip install omnisafe
 
 omnisafe --help  # Ask for help
 
@@ -386,14 +427,26 @@
   title   = {OmniSafe: An Infrastructure for Accelerating Safe Reinforcement Learning Research},
   author  = {Jiaming Ji, Jiayi Zhou, Borong Zhang, Juntao Dai, Xuehai Pan, Ruiyang Sun, Weidong Huang, Yiran Geng, Mickel Liu, Yaodong Yang},
   journal = {arXiv preprint arXiv:2305.09304},
   year    = {2023}
 }
 ```
 
+## Publications using OmniSafe
+
+We have compiled a list of papers that use OmniSafe for algorithm implementation or experimentation. If you are willing to include your work in this list, or if you wish to have your implementation officially integrated into OmniSafe, please feel free to [contact us](https://github.com/PKU-Alignment/omnisafe/issues).
+
+| Papers | Publisher|
+|:---:|:---:|
+| [Off-Policy Primal-Dual Safe Reinforcement Learning](https://openreview.net/pdf?id=vy42bYs1Wo) | ICLR 2024 |
+| [Safe Offline Reinforcement Learning with Feasibility-Guided Diffusion Model](https://openreview.net/pdf?id=j5JvZCaDM0) | ICLR 2024 |
+| [Iterative Reachability Estimation for Safe Reinforcement Learning](https://proceedings.neurips.cc/paper_files/paper/2023/file/dca63f2650fe9e88956c1b68440b8ee9-Paper-Conference.pdf) | NeurIPS 2023 |
+| [Balance Reward and Safety Optimization for Safe Reinforcement Learning: A Perspective of Gradient Manipulation](https://ojs.aaai.org/index.php/AAAI/article/view/30102/31944) | AAAI 2024 |
+| [Learning Safety Constraints From Demonstration Using One-Class Decision Trees](https://openreview.net/pdf?id=dxUi16pvub) | AAAI 2024 WorkShops |
+
 ## The OmniSafe Team
 
 OmniSafe is mainly developed by the SafeRL research team directed by Prof. [Yaodong Yang](https://www.yangyaodong.com/).
 Our SafeRL research team members include [Borong Zhang](https://github.com/muchvo), [Jiayi Zhou](https://github.com/Gaiejj), [JTao Dai](https://github.com/calico-1226), [Weidong Huang](https://github.com/hdadong), [Ruiyang Sun](https://github.com/rockmagma02), [Xuehai Pan](https://github.com/XuehaiPan) and [Jiaming Ji](https://github.com/zmsn-2077).
 If you have any questions in the process of using OmniSafe, don't hesitate to ask your questions on [the GitHub issue page](https://github.com/PKU-Alignment/omnisafe/issues/new/choose), we will reply to you in 2-3 working days.
 
 ## License
```

#### html2text {}

```diff
@@ -1,24 +1,37 @@
-Metadata-Version: 2.1 Name: omnisafe Version: 0.5.0b0 Summary: A comprehensive
+Metadata-Version: 2.1 Name: omnisafe Version: 0.5.1b0 Summary: A comprehensive
 and reliable benchmark for safe reinforcement learning. Author: OmniSafe
 Contributors License: Apache License, Version 2.0 Project-URL: Homepage, https:
 //github.com/PKU-Alignment/omnisafe Project-URL: Repository, https://
 github.com/PKU-Alignment/omnisafe Project-URL: Documentation, https://
 omnisafe.readthedocs.io Project-URL: Bug Report, https://github.com/PKU-
 Alignment/omnisafe/issues Keywords: Safe Reinforcement Learning,Reinforcement
 Learning,PyTorch Classifier: Development Status :: 4 - Beta Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Intended Audience :: Science/Research Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Provides-Extra: lint Provides-Extra: test License-
-File: LICENSE
+Content-Type: text/markdown License-File: LICENSE Requires-Dist: safety-
+gymnasium>=0.2.0 Requires-Dist: torch>=1.10.0 Requires-Dist: numpy>=1.20.0
+Requires-Dist: tensorboard>=2.8.0 Requires-Dist: wandb>=0.13.0 Requires-Dist:
+pyyaml>=6.0 Requires-Dist: moviepy>=1.0.0 Requires-Dist: typing-
+extensions>=4.0.0 Requires-Dist: typer[all]>=0.7.0 Requires-Dist:
+seaborn>=0.12.2 Requires-Dist: pandas==2.0.3 Requires-Dist: matplotlib>=3.7.1
+Requires-Dist: gdown>=4.6.0 Provides-Extra: lint Requires-Dist: isort>=5.11.0;
+extra == "lint" Requires-Dist: black>=22.6.0; extra == "lint" Requires-Dist:
+pylint[spelling]>=2.15.0; extra == "lint" Requires-Dist: mypy>=0.990; extra ==
+"lint" Requires-Dist: flake8; extra == "lint" Requires-Dist: flake8-bugbear;
+extra == "lint" Requires-Dist: ruff; extra == "lint" Requires-Dist: doc8; extra
+== "lint" Requires-Dist: pydocstyle; extra == "lint" Requires-Dist: pyenchant;
+extra == "lint" Requires-Dist: pre-commit; extra == "lint" Provides-Extra: test
+Requires-Dist: pytest; extra == "test" Requires-Dist: pytest-cov; extra ==
+"test" Requires-Dist: pytest-xdist; extra == "test"
      [https://github.com/PKU-Alignment/omnisafe/raw/HEAD/images/logo.png]
   [![Organization](https://img.shields.io/badge/Organization-PKU--Alignment-
 blue)](https://github.com/PKU-Alignment) [![PyPI](https://img.shields.io/pypi/
  v/omnisafe?logo=pypi)](https://pypi.org/project/omnisafe) [![tests](https://
      img.shields.io/github/actions/workflow/status/PKU-Alignment/omnisafe/
  test.yml?label=tests&logo=github)](https://github.com/PKU-Alignment/omnisafe/
  tree/HEAD/tests) [![Documentation Status](https://img.shields.io/readthedocs/
@@ -69,75 +82,77 @@
 video](https://github-production-user-asset-6210df.s3.amazonaws.com/73586554/
 237139607-d1e6f413-aa2c-4f68-b8ee-08a4361493a0.gif) ---------------------------
 ----------------------------------------------------- ### Table of Contents -
 [Quick Start](#quick-start) - [Installation](#installation) - [Prerequisites]
 (#prerequisites) - [Install from source](#install-from-source) - [Install from
 PyPI](#install-from-pypi) - [Implemented Algorithms](#implemented-algorithms) -
 [Examples](#examples) - [Algorithms Registry](#algorithms-registry) -
-[Supported Environments](#supported-environments) - [Try with CLI](#try-with-
-cli) - [Getting Started](#getting-started) - [Important Hints](#important-
-hints) - [Quickstart: Colab on the Cloud](#quickstart-colab-on-the-cloud) -
-[Changelog](#changelog) - [Citing OmniSafe](#citing-omnisafe) - [The OmniSafe
-Team](#the-omnisafe-team) - [License](#license) -------------------------------
-------------------------------------------------- ## Quick Start ###
-Installation #### Prerequisites OmniSafe requires Python 3.8+ and PyTorch
-1.10+. > We support and test for Python 3.8, 3.9, 3.10 on Linux. Meanwhile, we
-also support M1 and M2 versions of macOS. We will accept PRs related to
-Windows, but do not officially support it. #### Install from source ```bash #
-Clone the repo git clone https://github.com/PKU-Alignment/omnisafe.git cd
-omnisafe # Create a conda environment conda env create --file conda-recipe.yaml
-conda activate omnisafe # Install omnisafe pip install -e . ``` #### Install
-from PyPI OmniSafe is hosted in [![PyPI](https://img.shields.io/pypi/v/
-omnisafe?label=pypi&logo=pypi)](https://pypi.org/project/omnisafe) / ![Status]
-(https://img.shields.io/pypi/status/omnisafe?label=status). ```bash pip install
-omnisafe ``` ## Implemented Algorithms LLaatteesstt SSaaffeeRRLL PPaappeerrss - **[AAAI 2023]**
-Augmented Proximal Policy Optimization for Safe Reinforcement Learning (APPO) -
-**[NeurIPS 2022]** [Constrained Update Projection Approach to Safe Policy
-Optimization (CUP)](https://arxiv.org/abs/2209.07089) - **[NeurIPS 2022]**
-[Effects of Safety State Augmentation on Safe Exploration (Simmer)](https://
-arxiv.org/abs/2206.02675) - **[NeurIPS 2022]** [Model-based Safe Deep
-Reinforcement Learning via a Constrained Proximal Policy Optimization
-Algorithm](https://arxiv.org/abs/2210.07573) - **[ICML 2022]** [SautÃ© RL:
-Almost Surely Safe Reinforcement Learning Using State Augmentation (SauteRL)]
-(https://arxiv.org/abs/2202.06558) - **[IJCAI 2022]** [Penalized Proximal
-Policy Optimization for Safe Reinforcement Learning](https://arxiv.org/abs/
-2205.11814) - **[AAAI 2022]** [Conservative and Adaptive Penalty for Model-
-Based Safe Reinforcement Learning (CAP)](https://arxiv.org/abs/2112.07701) LLiisstt
-ooff AAllggoorriitthhmmss OOnn PPoolliiccyy SSaaffeeRRLL - [x] [The Lagrange version of PPO (PPO-Lag)]
-(https://cdn.openai.com/safexp-short.pdf) - [x] [The Lagrange version of TRPO
-(TRPO-Lag)](https://cdn.openai.com/safexp-short.pdf) - [x] **[ICML 2017]**
-[Constrained Policy Optimization (CPO)](https://proceedings.mlr.press/v70/
-achiam17a) - [x] **[ICLR 2019]** [Reward Constrained Policy Optimization
-(RCPO)](https://openreview.net/forum?id=SkfrvsA9FX) - [x] **[ICML 2020]**
-[Responsive Safety in Reinforcement Learning by PID Lagrangian Methods (PID-
-Lag)](https://arxiv.org/abs/2007.03964) - [x] **[NeurIPS 2020]** [First Order
-Constrained Optimization in Policy Space (FOCOPS)](https://arxiv.org/abs/
-2002.06506) - [x] **[AAAI 2020]** [IPO: Interior-point Policy Optimization
-under Constraints (IPO)](https://arxiv.org/abs/1910.09615) - [x] **[ICLR
-2020]** [Projection-Based Constrained Policy Optimization (PCPO)](https://
-openreview.net/forum?id=rke3TJrtPS) - [x] **[ICML 2021]** [CRPO: A New Approach
-for Safe Reinforcement Learning with Convergence Guarantee](https://arxiv.org/
-abs/2011.05869) - [x] **[IJCAI 2022]** [Penalized Proximal Policy Optimization
-for Safe Reinforcement Learning(P3O)](https://arxiv.org/pdf/2205.11814.pdf) OOffff
-PPoolliiccyy SSaaffeeRRLL - **[Preprint 2019]** [The Lagrangian version of DDPG (DDPGLag)]
-(https://cdn.openai.com/safexp-short.pdf) - **[Preprint 2019]** [The Lagrangian
-version of TD3 (TD3Lag)](https://cdn.openai.com/safexp-short.pdf) - **[Preprint
-2019]** [The Lagrangian version of SAC (SACLag)](https://cdn.openai.com/safexp-
-short.pdf) - **[ICML 2020]** [Responsive Safety in Reinforcement Learning by
-PID Lagrangian Methods (DDPGPID)](https://arxiv.org/abs/2007.03964) - **[ICML
-2020]** [Responsive Safety in Reinforcement Learning by PID Lagrangian Methods
-(TD3PID)](https://arxiv.org/abs/2007.03964) - **[ICML 2020]** [Responsive
-Safety in Reinforcement Learning by PID Lagrangian Methods (SACPID)](https://
-arxiv.org/abs/2007.03964) MMooddeell--BBaasseedd SSaaffeeRRLL - [ ] **[NeurIPS 2021]** [Safe
-Reinforcement Learning by Imagining the Near Future (SMBPO)](https://arxiv.org/
-abs/2202.07789) - [x] **[CoRL 2021 (Oral)]** [Learning Off-Policy with Online
-Planning (SafeLOOP)](https://arxiv.org/abs/2008.10066) - [x] **[AAAI 2022]**
+[Supported Environments](#supported-environments) - [Customizing your
+environment](#customizing-your-environment) - [Try with CLI](#try-with-cli) -
+[Getting Started](#getting-started) - [Important Hints](#important-hints) -
+[Quickstart: Colab on the Cloud](#quickstart-colab-on-the-cloud) - [Changelog]
+(#changelog) - [Citing OmniSafe](#citing-omnisafe) - [Publications using
+OmniSafe](#publications-using-omnisafe) - [The OmniSafe Team](#the-omnisafe-
+team) - [License](#license) ---------------------------------------------------
+----------------------------- ## Quick Start ### Installation ####
+Prerequisites OmniSafe requires Python 3.8+ and PyTorch 1.10+. > We support and
+test for Python 3.8, 3.9, 3.10 on Linux. Meanwhile, we also support M1 and M2
+versions of macOS. We will accept PRs related to Windows, but do not officially
+support it. #### Install from source ```bash # Clone the repo git clone https:/
+/github.com/PKU-Alignment/omnisafe.git cd omnisafe # Create a conda environment
+conda env create --file conda-recipe.yaml conda activate omnisafe # Install
+omnisafe pip install -e . ``` #### Install from PyPI OmniSafe is hosted in [!
+[PyPI](https://img.shields.io/pypi/v/omnisafe?label=pypi&logo=pypi)](https://
+pypi.org/project/omnisafe) / ![Status](https://img.shields.io/pypi/status/
+omnisafe?label=status). ```bash pip install omnisafe ``` ## Implemented
+Algorithms LLaatteesstt SSaaffeeRRLL PPaappeerrss - **[AAAI 2023]** Augmented Proximal Policy
+Optimization for Safe Reinforcement Learning (APPO) - **[NeurIPS 2022]**
+[Constrained Update Projection Approach to Safe Policy Optimization (CUP)]
+(https://arxiv.org/abs/2209.07089) - **[NeurIPS 2022]** [Effects of Safety
+State Augmentation on Safe Exploration (Simmer)](https://arxiv.org/abs/
+2206.02675) - **[NeurIPS 2022]** [Model-based Safe Deep Reinforcement Learning
+via a Constrained Proximal Policy Optimization Algorithm](https://arxiv.org/
+abs/2210.07573) - **[ICML 2022]** [SautÃ© RL: Almost Surely Safe Reinforcement
+Learning Using State Augmentation (SauteRL)](https://arxiv.org/abs/2202.06558)
+- **[IJCAI 2022]** [Penalized Proximal Policy Optimization for Safe
+Reinforcement Learning](https://arxiv.org/abs/2205.11814) - **[AAAI 2022]**
 [Conservative and Adaptive Penalty for Model-Based Safe Reinforcement Learning
-(CAP)](https://arxiv.org/abs/2112.07701) - [x] **[NeurIPS 2022]** [Model-based
-Safe Deep Reinforcement Learning via a Constrained Proximal Policy Optimization
+(CAP)](https://arxiv.org/abs/2112.07701) LLiisstt ooff AAllggoorriitthhmmss OOnn PPoolliiccyy SSaaffeeRRLL -
+[x] [The Lagrange version of PPO (PPO-Lag)](https://cdn.openai.com/safexp-
+short.pdf) - [x] [The Lagrange version of TRPO (TRPO-Lag)](https://
+cdn.openai.com/safexp-short.pdf) - [x] **[ICML 2017]** [Constrained Policy
+Optimization (CPO)](https://proceedings.mlr.press/v70/achiam17a) - [x] **[ICLR
+2019]** [Reward Constrained Policy Optimization (RCPO)](https://openreview.net/
+forum?id=SkfrvsA9FX) - [x] **[ICML 2020]** [Responsive Safety in Reinforcement
+Learning by PID Lagrangian Methods (PID-Lag)](https://arxiv.org/abs/2007.03964)
+- [x] **[NeurIPS 2020]** [First Order Constrained Optimization in Policy Space
+(FOCOPS)](https://arxiv.org/abs/2002.06506) - [x] **[AAAI 2020]** [IPO:
+Interior-point Policy Optimization under Constraints (IPO)](https://arxiv.org/
+abs/1910.09615) - [x] **[ICLR 2020]** [Projection-Based Constrained Policy
+Optimization (PCPO)](https://openreview.net/forum?id=rke3TJrtPS) - [x] **[ICML
+2021]** [CRPO: A New Approach for Safe Reinforcement Learning with Convergence
+Guarantee](https://arxiv.org/abs/2011.05869) - [x] **[IJCAI 2022]** [Penalized
+Proximal Policy Optimization for Safe Reinforcement Learning(P3O)](https://
+arxiv.org/pdf/2205.11814.pdf) OOffff PPoolliiccyy SSaaffeeRRLL - **[Preprint 2019]** [The
+Lagrangian version of DDPG (DDPGLag)](https://cdn.openai.com/safexp-short.pdf)
+- **[Preprint 2019]** [The Lagrangian version of TD3 (TD3Lag)](https://
+cdn.openai.com/safexp-short.pdf) - **[Preprint 2019]** [The Lagrangian version
+of SAC (SACLag)](https://cdn.openai.com/safexp-short.pdf) - **[ICML 2020]**
+[Responsive Safety in Reinforcement Learning by PID Lagrangian Methods
+(DDPGPID)](https://arxiv.org/abs/2007.03964) - **[ICML 2020]** [Responsive
+Safety in Reinforcement Learning by PID Lagrangian Methods (TD3PID)](https://
+arxiv.org/abs/2007.03964) - **[ICML 2020]** [Responsive Safety in Reinforcement
+Learning by PID Lagrangian Methods (SACPID)](https://arxiv.org/abs/2007.03964)
+MMooddeell--BBaasseedd SSaaffeeRRLL - [ ] **[NeurIPS 2021]** [Safe Reinforcement Learning by
+Imagining the Near Future (SMBPO)](https://arxiv.org/abs/2202.07789) - [x] **
+[CoRL 2021 (Oral)]** [Learning Off-Policy with Online Planning (SafeLOOP)]
+(https://arxiv.org/abs/2008.10066) - [x] **[AAAI 2022]** [Conservative and
+Adaptive Penalty for Model-Based Safe Reinforcement Learning (CAP)](https://
+arxiv.org/abs/2112.07701) - [x] **[NeurIPS 2022]** [Model-based Safe Deep
+Reinforcement Learning via a Constrained Proximal Policy Optimization
 Algorithm](https://arxiv.org/abs/2210.07573) - [ ] **[ICLR 2022]** [Constrained
 Policy Optimization via Bayesian World Models (LA-MBDA)](https://arxiv.org/abs/
 2201.09802) - [x] **[ICML 2022 Workshop]** [Constrained Model-based
 Reinforcement Learning with Robust Cross-Entropy Method (RCE)](https://
 arxiv.org/abs/2010.07968) - [x] **[NeurIPS 2018]** [Constrained Cross-Entropy
 Method for Safe Reinforcement Learning (CCE)](https://proceedings.neurips.cc/
 paper/2018/hash/34ffeb359a192eb8174b6854643cc046-Abstract.html) OOfffflliinnee SSaaffeeRRLL
@@ -182,60 +197,92 @@
 |Safe Navigation|_B_u_t_t_o_n_[_0_1_2_]|Point, Car, Racecar, Ant|SafetyPointGoal1-v0    |
 |               |_P_u_s_h_[_0_1_2_]_ _ |                        |                       |
 |_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_C_i_r_c_l_e_[_0_1_2_]_|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |               |           |HalfCheetah, Hopper,    |SafetyHumanoidVelocity-|
 |Safe Velocity  |Velocity   |Swimmer, Walker2d, Ant, |v1                     |
 |_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _|_H_u_m_a_n_o_i_d_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 For more information about environments, please refer to [Safety-Gymnasium]
-(https://www.safety-gymnasium.com). #### Try with CLI ```bash pip install
-omnisafe omnisafe --help # Ask for help omnisafe benchmark --help # The
-benchmark also can be replaced with 'eval', 'train', 'train-config' # Quick
-benchmarking for your research, just specify: # 1. exp_name # 2. num_pool(how
-much processes are concurrent) # 3. path of the config file (refer to omnisafe/
-examples/benchmarks for format) # Here we provide an exampe in ./tests/
-saved_source. # And you can set your benchmark_config.yaml by following it
-omnisafe benchmark test_benchmark 2 ./tests/saved_source/benchmark_config.yaml
-# Quick evaluating and rendering your trained policy, just specify: # 1. path
-of algorithm which you trained omnisafe eval ./tests/saved_source/PPO-
-{SafetyPointGoal1-v0} --num-episode 1 # Quick training some algorithms to
-validate your thoughts # Note: use `key1:key2`, your can select key of
-hyperparameters which are recursively contained, and use `--custom-cfgs`, you
-can add custom cfgs via CLI omnisafe train --algo PPO --total-steps 2048 --
-vector-env-nums 1 --custom-cfgs algo_cfgs:steps_per_epoch --custom-cfgs 1024 #
-Quick training some algorithms via a saved config file, the format is as same
-as default format omnisafe train-config ./tests/saved_source/train_config.yaml
-``` ---------------------------------------------------------------------------
------ ## Getting Started ### Important Hints We have provided benchmark results
-for various algorithms, including on-policy, off-policy, model-based, and
-offline approaches, along with parameter tuning analysis. Please refer to the
-following: - [On-Policy](./benchmarks/on-policy/) - [Off-Policy](./benchmarks/
-off-policy/) - [Model-based](./benchmarks/model-based/) - [Offline](./
-benchmarks/offline/) ### Quickstart: Colab on the Cloud Explore OmniSafe easily
-and quickly through a series of Google Colab notebooks: - [Getting Started]
+(https://www.safety-gymnasium.com). #### Customizing your environment We offer
+a flexible customized environment interface that allows users to achieve the
+following **without modifying the OmniSafe source code**: - Use OmniSafe to
+train algorithms on customized environments. - Create the the environment with
+specified personalized parameters. - Complete the recording of environment-
+specific information in Logger. We provide **step-by-step tutorials** on
+[Environment Customization From Scratch](https://colab.research.google.com/
+github/PKU-Alignment/omnisafe/blob/main/tutorials/English/
+3.Environment%20Customization%20from%20Scratch.ipynb) and [Environment
+Customization From Community](https://colab.research.google.com/github/PKU-
+Alignment/omnisafe/blob/main/tutorials/English/
+4.Environment%20Customization%20from%20Community.ipynb) to give you a detailed
+introduction on how to use this extraordinary feature of OmniSafe. *Note: If
+you find trouble customizing your environment, please feel free to open an
+[issue](https://github.com/PKU-Alignment/omnisafe/issues) or [discussion]
+(https://github.com/PKU-Alignment/omnisafe/discussions). [Pull requests](https:
+//github.com/PKU-Alignment/omnisafe/pulls) are also welcomed if you're willing
+to contribute the implementation of your environments interface.* #### Try with
+CLI ```bash pip install omnisafe omnisafe --help # Ask for help omnisafe
+benchmark --help # The benchmark also can be replaced with 'eval', 'train',
+'train-config' # Quick benchmarking for your research, just specify: # 1.
+exp_name # 2. num_pool(how much processes are concurrent) # 3. path of the
+config file (refer to omnisafe/examples/benchmarks for format) # Here we
+provide an exampe in ./tests/saved_source. # And you can set your
+benchmark_config.yaml by following it omnisafe benchmark test_benchmark 2 ./
+tests/saved_source/benchmark_config.yaml # Quick evaluating and rendering your
+trained policy, just specify: # 1. path of algorithm which you trained omnisafe
+eval ./tests/saved_source/PPO-{SafetyPointGoal1-v0} --num-episode 1 # Quick
+training some algorithms to validate your thoughts # Note: use `key1:key2`,
+your can select key of hyperparameters which are recursively contained, and use
+`--custom-cfgs`, you can add custom cfgs via CLI omnisafe train --algo PPO --
+total-steps 2048 --vector-env-nums 1 --custom-cfgs algo_cfgs:steps_per_epoch --
+custom-cfgs 1024 # Quick training some algorithms via a saved config file, the
+format is as same as default format omnisafe train-config ./tests/saved_source/
+train_config.yaml ``` ---------------------------------------------------------
+----------------------- ## Getting Started ### Important Hints We have provided
+benchmark results for various algorithms, including on-policy, off-policy,
+model-based, and offline approaches, along with parameter tuning analysis.
+Please refer to the following: - [On-Policy](./benchmarks/on-policy/) - [Off-
+Policy](./benchmarks/off-policy/) - [Model-based](./benchmarks/model-based/) -
+[Offline](./benchmarks/offline/) ### Quickstart: Colab on the Cloud Explore
+OmniSafe easily and quickly through a series of Google Colab notebooks: -
+[Getting Started](https://colab.research.google.com/github/PKU-Alignment/
+omnisafe/blob/main/tutorials/English/1.Getting_Started.ipynb) Introduce the
+basic usage of OmniSafe so that users can quickly hand it. - [CLI Command]
 (https://colab.research.google.com/github/PKU-Alignment/omnisafe/blob/main/
-tutorials/English/1.Getting_Started.ipynb) Introduce the basic usage of
-OmniSafe so that users can quickly hand it. - [CLI Command](https://
-colab.research.google.com/github/PKU-Alignment/omnisafe/blob/main/tutorials/
-English/2.CLI_Command.ipynb) Introduce how to use the CLI tool of OmniSafe. We
-take great pleasure in collaborating with our users to create tutorials in
-various languages. Please refer to our list of currently supported languages.
-If you are interested in translating the tutorial into a new language or
-improving an existing version, kindly submit a PR to us. ----------------------
----------------------------------------------------------- ## Changelog See
-[CHANGELOG.md](https://github.com/PKU-Alignment/omnisafe/blob/main/
-CHANGELOG.md). ## Citing OmniSafe If you find OmniSafe useful or use OmniSafe
-in your research, please cite it in your publications. ```bibtex @article
-{omnisafe, title = {OmniSafe: An Infrastructure for Accelerating Safe
+tutorials/English/2.CLI_Command.ipynb) Introduce how to use the CLI tool of
+OmniSafe. We take great pleasure in collaborating with our users to create
+tutorials in various languages. Please refer to our list of currently supported
+languages. If you are interested in translating the tutorial into a new
+language or improving an existing version, kindly submit a PR to us. ----------
+---------------------------------------------------------------------- ##
+Changelog See [CHANGELOG.md](https://github.com/PKU-Alignment/omnisafe/blob/
+main/CHANGELOG.md). ## Citing OmniSafe If you find OmniSafe useful or use
+OmniSafe in your research, please cite it in your publications. ```bibtex
+@article{omnisafe, title = {OmniSafe: An Infrastructure for Accelerating Safe
 Reinforcement Learning Research}, author = {Jiaming Ji, Jiayi Zhou, Borong
 Zhang, Juntao Dai, Xuehai Pan, Ruiyang Sun, Weidong Huang, Yiran Geng, Mickel
 Liu, Yaodong Yang}, journal = {arXiv preprint arXiv:2305.09304}, year = {2023}
-} ``` ## The OmniSafe Team OmniSafe is mainly developed by the SafeRL research
-team directed by Prof. [Yaodong Yang](https://www.yangyaodong.com/). Our SafeRL
-research team members include [Borong Zhang](https://github.com/muchvo), [Jiayi
-Zhou](https://github.com/Gaiejj), [JTao Dai](https://github.com/calico-1226),
-[Weidong Huang](https://github.com/hdadong), [Ruiyang Sun](https://github.com/
-rockmagma02), [Xuehai Pan](https://github.com/XuehaiPan) and [Jiaming Ji]
-(https://github.com/zmsn-2077). If you have any questions in the process of
-using OmniSafe, don't hesitate to ask your questions on [the GitHub issue page]
-(https://github.com/PKU-Alignment/omnisafe/issues/new/choose), we will reply to
-you in 2-3 working days. ## License OmniSafe is released under Apache License
-2.0.
+} ``` ## Publications using OmniSafe We have compiled a list of papers that use
+OmniSafe for algorithm implementation or experimentation. If you are willing to
+include your work in this list, or if you wish to have your implementation
+officially integrated into OmniSafe, please feel free to [contact us](https://
+github.com/PKU-Alignment/omnisafe/issues). | Papers | Publisher| |:---:|:---:
+| | [Off-Policy Primal-Dual Safe Reinforcement Learning](https://
+openreview.net/pdf?id=vy42bYs1Wo) | ICLR 2024 | | [Safe Offline Reinforcement
+Learning with Feasibility-Guided Diffusion Model](https://openreview.net/
+pdf?id=j5JvZCaDM0) | ICLR 2024 | | [Iterative Reachability Estimation for Safe
+Reinforcement Learning](https://proceedings.neurips.cc/paper_files/paper/2023/
+file/dca63f2650fe9e88956c1b68440b8ee9-Paper-Conference.pdf) | NeurIPS 2023 | |
+[Balance Reward and Safety Optimization for Safe Reinforcement Learning: A
+Perspective of Gradient Manipulation](https://ojs.aaai.org/index.php/AAAI/
+article/view/30102/31944) | AAAI 2024 | | [Learning Safety Constraints From
+Demonstration Using One-Class Decision Trees](https://openreview.net/
+pdf?id=dxUi16pvub) | AAAI 2024 WorkShops | ## The OmniSafe Team OmniSafe is
+mainly developed by the SafeRL research team directed by Prof. [Yaodong Yang]
+(https://www.yangyaodong.com/). Our SafeRL research team members include
+[Borong Zhang](https://github.com/muchvo), [Jiayi Zhou](https://github.com/
+Gaiejj), [JTao Dai](https://github.com/calico-1226), [Weidong Huang](https://
+github.com/hdadong), [Ruiyang Sun](https://github.com/rockmagma02), [Xuehai
+Pan](https://github.com/XuehaiPan) and [Jiaming Ji](https://github.com/zmsn-
+2077). If you have any questions in the process of using OmniSafe, don't
+hesitate to ask your questions on [the GitHub issue page](https://github.com/
+PKU-Alignment/omnisafe/issues/new/choose), we will reply to you in 2-3 working
+days. ## License OmniSafe is released under Apache License 2.0.
```

### Comparing `omnisafe-0.5.0b0/README.md` & `omnisafe-0.5.1b0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -55,20 +55,22 @@
     - [Prerequisites](#prerequisites)
     - [Install from source](#install-from-source)
     - [Install from PyPI](#install-from-pypi)
 - [Implemented Algorithms](#implemented-algorithms)
   - [Examples](#examples)
     - [Algorithms Registry](#algorithms-registry)
     - [Supported Environments](#supported-environments)
+    - [Customizing your environment](#customizing-your-environment)
     - [Try with CLI](#try-with-cli)
 - [Getting Started](#getting-started)
   - [Important Hints](#important-hints)
   - [Quickstart: Colab on the Cloud](#quickstart-colab-on-the-cloud)
 - [Changelog](#changelog)
 - [Citing OmniSafe](#citing-omnisafe)
+- [Publications using OmniSafe](#publications-using-omnisafe)
 - [The OmniSafe Team](#the-omnisafe-team)
 - [License](#license)
 
 --------------------------------------------------------------------------------
 
 ## Quick Start
 
@@ -286,14 +288,26 @@
     <td>SafetyHumanoidVelocity-v1</td>
   </tr>
 </tbody>
 </table>
 
 For more information about environments, please refer to [Safety-Gymnasium](https://www.safety-gymnasium.com).
 
+#### Customizing your environment
+
+We offer a flexible customized environment interface that allows users to achieve the following **without modifying the OmniSafe source code**:
+
+- Use OmniSafe to train algorithms on customized environments.
+- Create the the environment with specified personalized parameters.
+- Complete the recording of environment-specific information in Logger.
+
+We provide **step-by-step tutorials** on [Environment Customization From Scratch](https://colab.research.google.com/github/PKU-Alignment/omnisafe/blob/main/tutorials/English/3.Environment%20Customization%20from%20Scratch.ipynb) and [Environment Customization From Community](https://colab.research.google.com/github/PKU-Alignment/omnisafe/blob/main/tutorials/English/4.Environment%20Customization%20from%20Community.ipynb) to give you a detailed introduction on how to use this extraordinary feature of OmniSafe.
+
+*Note: If you find trouble customizing your environment, please feel free to open an [issue](https://github.com/PKU-Alignment/omnisafe/issues) or [discussion](https://github.com/PKU-Alignment/omnisafe/discussions). [Pull requests](https://github.com/PKU-Alignment/omnisafe/pulls) are also welcomed if you're willing to contribute the implementation of your environments interface.*
+
 #### Try with CLI
 
 ```bash
 pip install omnisafe
 
 omnisafe --help  # Ask for help
 
@@ -359,14 +373,26 @@
   title   = {OmniSafe: An Infrastructure for Accelerating Safe Reinforcement Learning Research},
   author  = {Jiaming Ji, Jiayi Zhou, Borong Zhang, Juntao Dai, Xuehai Pan, Ruiyang Sun, Weidong Huang, Yiran Geng, Mickel Liu, Yaodong Yang},
   journal = {arXiv preprint arXiv:2305.09304},
   year    = {2023}
 }
 ```
 
+## Publications using OmniSafe
+
+We have compiled a list of papers that use OmniSafe for algorithm implementation or experimentation. If you are willing to include your work in this list, or if you wish to have your implementation officially integrated into OmniSafe, please feel free to [contact us](https://github.com/PKU-Alignment/omnisafe/issues).
+
+| Papers | Publisher|
+|:---:|:---:|
+| [Off-Policy Primal-Dual Safe Reinforcement Learning](https://openreview.net/pdf?id=vy42bYs1Wo) | ICLR 2024 |
+| [Safe Offline Reinforcement Learning with Feasibility-Guided Diffusion Model](https://openreview.net/pdf?id=j5JvZCaDM0) | ICLR 2024 |
+| [Iterative Reachability Estimation for Safe Reinforcement Learning](https://proceedings.neurips.cc/paper_files/paper/2023/file/dca63f2650fe9e88956c1b68440b8ee9-Paper-Conference.pdf) | NeurIPS 2023 |
+| [Balance Reward and Safety Optimization for Safe Reinforcement Learning: A Perspective of Gradient Manipulation](https://ojs.aaai.org/index.php/AAAI/article/view/30102/31944) | AAAI 2024 |
+| [Learning Safety Constraints From Demonstration Using One-Class Decision Trees](https://openreview.net/pdf?id=dxUi16pvub) | AAAI 2024 WorkShops |
+
 ## The OmniSafe Team
 
 OmniSafe is mainly developed by the SafeRL research team directed by Prof. [Yaodong Yang](https://www.yangyaodong.com/).
 Our SafeRL research team members include [Borong Zhang](https://github.com/muchvo), [Jiayi Zhou](https://github.com/Gaiejj), [JTao Dai](https://github.com/calico-1226), [Weidong Huang](https://github.com/hdadong), [Ruiyang Sun](https://github.com/rockmagma02), [Xuehai Pan](https://github.com/XuehaiPan) and [Jiaming Ji](https://github.com/zmsn-2077).
 If you have any questions in the process of using OmniSafe, don't hesitate to ask your questions on [the GitHub issue page](https://github.com/PKU-Alignment/omnisafe/issues/new/choose), we will reply to you in 2-3 working days.
 
 ## License
```

#### html2text {}

```diff
@@ -52,75 +52,77 @@
 video](https://github-production-user-asset-6210df.s3.amazonaws.com/73586554/
 237139607-d1e6f413-aa2c-4f68-b8ee-08a4361493a0.gif) ---------------------------
 ----------------------------------------------------- ### Table of Contents -
 [Quick Start](#quick-start) - [Installation](#installation) - [Prerequisites]
 (#prerequisites) - [Install from source](#install-from-source) - [Install from
 PyPI](#install-from-pypi) - [Implemented Algorithms](#implemented-algorithms) -
 [Examples](#examples) - [Algorithms Registry](#algorithms-registry) -
-[Supported Environments](#supported-environments) - [Try with CLI](#try-with-
-cli) - [Getting Started](#getting-started) - [Important Hints](#important-
-hints) - [Quickstart: Colab on the Cloud](#quickstart-colab-on-the-cloud) -
-[Changelog](#changelog) - [Citing OmniSafe](#citing-omnisafe) - [The OmniSafe
-Team](#the-omnisafe-team) - [License](#license) -------------------------------
-------------------------------------------------- ## Quick Start ###
-Installation #### Prerequisites OmniSafe requires Python 3.8+ and PyTorch
-1.10+. > We support and test for Python 3.8, 3.9, 3.10 on Linux. Meanwhile, we
-also support M1 and M2 versions of macOS. We will accept PRs related to
-Windows, but do not officially support it. #### Install from source ```bash #
-Clone the repo git clone https://github.com/PKU-Alignment/omnisafe.git cd
-omnisafe # Create a conda environment conda env create --file conda-recipe.yaml
-conda activate omnisafe # Install omnisafe pip install -e . ``` #### Install
-from PyPI OmniSafe is hosted in [![PyPI](https://img.shields.io/pypi/v/
-omnisafe?label=pypi&logo=pypi)](https://pypi.org/project/omnisafe) / ![Status]
-(https://img.shields.io/pypi/status/omnisafe?label=status). ```bash pip install
-omnisafe ``` ## Implemented Algorithms LLaatteesstt SSaaffeeRRLL PPaappeerrss - **[AAAI 2023]**
-Augmented Proximal Policy Optimization for Safe Reinforcement Learning (APPO) -
-**[NeurIPS 2022]** [Constrained Update Projection Approach to Safe Policy
-Optimization (CUP)](https://arxiv.org/abs/2209.07089) - **[NeurIPS 2022]**
-[Effects of Safety State Augmentation on Safe Exploration (Simmer)](https://
-arxiv.org/abs/2206.02675) - **[NeurIPS 2022]** [Model-based Safe Deep
-Reinforcement Learning via a Constrained Proximal Policy Optimization
-Algorithm](https://arxiv.org/abs/2210.07573) - **[ICML 2022]** [SautÃ© RL:
-Almost Surely Safe Reinforcement Learning Using State Augmentation (SauteRL)]
-(https://arxiv.org/abs/2202.06558) - **[IJCAI 2022]** [Penalized Proximal
-Policy Optimization for Safe Reinforcement Learning](https://arxiv.org/abs/
-2205.11814) - **[AAAI 2022]** [Conservative and Adaptive Penalty for Model-
-Based Safe Reinforcement Learning (CAP)](https://arxiv.org/abs/2112.07701) LLiisstt
-ooff AAllggoorriitthhmmss OOnn PPoolliiccyy SSaaffeeRRLL - [x] [The Lagrange version of PPO (PPO-Lag)]
-(https://cdn.openai.com/safexp-short.pdf) - [x] [The Lagrange version of TRPO
-(TRPO-Lag)](https://cdn.openai.com/safexp-short.pdf) - [x] **[ICML 2017]**
-[Constrained Policy Optimization (CPO)](https://proceedings.mlr.press/v70/
-achiam17a) - [x] **[ICLR 2019]** [Reward Constrained Policy Optimization
-(RCPO)](https://openreview.net/forum?id=SkfrvsA9FX) - [x] **[ICML 2020]**
-[Responsive Safety in Reinforcement Learning by PID Lagrangian Methods (PID-
-Lag)](https://arxiv.org/abs/2007.03964) - [x] **[NeurIPS 2020]** [First Order
-Constrained Optimization in Policy Space (FOCOPS)](https://arxiv.org/abs/
-2002.06506) - [x] **[AAAI 2020]** [IPO: Interior-point Policy Optimization
-under Constraints (IPO)](https://arxiv.org/abs/1910.09615) - [x] **[ICLR
-2020]** [Projection-Based Constrained Policy Optimization (PCPO)](https://
-openreview.net/forum?id=rke3TJrtPS) - [x] **[ICML 2021]** [CRPO: A New Approach
-for Safe Reinforcement Learning with Convergence Guarantee](https://arxiv.org/
-abs/2011.05869) - [x] **[IJCAI 2022]** [Penalized Proximal Policy Optimization
-for Safe Reinforcement Learning(P3O)](https://arxiv.org/pdf/2205.11814.pdf) OOffff
-PPoolliiccyy SSaaffeeRRLL - **[Preprint 2019]** [The Lagrangian version of DDPG (DDPGLag)]
-(https://cdn.openai.com/safexp-short.pdf) - **[Preprint 2019]** [The Lagrangian
-version of TD3 (TD3Lag)](https://cdn.openai.com/safexp-short.pdf) - **[Preprint
-2019]** [The Lagrangian version of SAC (SACLag)](https://cdn.openai.com/safexp-
-short.pdf) - **[ICML 2020]** [Responsive Safety in Reinforcement Learning by
-PID Lagrangian Methods (DDPGPID)](https://arxiv.org/abs/2007.03964) - **[ICML
-2020]** [Responsive Safety in Reinforcement Learning by PID Lagrangian Methods
-(TD3PID)](https://arxiv.org/abs/2007.03964) - **[ICML 2020]** [Responsive
-Safety in Reinforcement Learning by PID Lagrangian Methods (SACPID)](https://
-arxiv.org/abs/2007.03964) MMooddeell--BBaasseedd SSaaffeeRRLL - [ ] **[NeurIPS 2021]** [Safe
-Reinforcement Learning by Imagining the Near Future (SMBPO)](https://arxiv.org/
-abs/2202.07789) - [x] **[CoRL 2021 (Oral)]** [Learning Off-Policy with Online
-Planning (SafeLOOP)](https://arxiv.org/abs/2008.10066) - [x] **[AAAI 2022]**
+[Supported Environments](#supported-environments) - [Customizing your
+environment](#customizing-your-environment) - [Try with CLI](#try-with-cli) -
+[Getting Started](#getting-started) - [Important Hints](#important-hints) -
+[Quickstart: Colab on the Cloud](#quickstart-colab-on-the-cloud) - [Changelog]
+(#changelog) - [Citing OmniSafe](#citing-omnisafe) - [Publications using
+OmniSafe](#publications-using-omnisafe) - [The OmniSafe Team](#the-omnisafe-
+team) - [License](#license) ---------------------------------------------------
+----------------------------- ## Quick Start ### Installation ####
+Prerequisites OmniSafe requires Python 3.8+ and PyTorch 1.10+. > We support and
+test for Python 3.8, 3.9, 3.10 on Linux. Meanwhile, we also support M1 and M2
+versions of macOS. We will accept PRs related to Windows, but do not officially
+support it. #### Install from source ```bash # Clone the repo git clone https:/
+/github.com/PKU-Alignment/omnisafe.git cd omnisafe # Create a conda environment
+conda env create --file conda-recipe.yaml conda activate omnisafe # Install
+omnisafe pip install -e . ``` #### Install from PyPI OmniSafe is hosted in [!
+[PyPI](https://img.shields.io/pypi/v/omnisafe?label=pypi&logo=pypi)](https://
+pypi.org/project/omnisafe) / ![Status](https://img.shields.io/pypi/status/
+omnisafe?label=status). ```bash pip install omnisafe ``` ## Implemented
+Algorithms LLaatteesstt SSaaffeeRRLL PPaappeerrss - **[AAAI 2023]** Augmented Proximal Policy
+Optimization for Safe Reinforcement Learning (APPO) - **[NeurIPS 2022]**
+[Constrained Update Projection Approach to Safe Policy Optimization (CUP)]
+(https://arxiv.org/abs/2209.07089) - **[NeurIPS 2022]** [Effects of Safety
+State Augmentation on Safe Exploration (Simmer)](https://arxiv.org/abs/
+2206.02675) - **[NeurIPS 2022]** [Model-based Safe Deep Reinforcement Learning
+via a Constrained Proximal Policy Optimization Algorithm](https://arxiv.org/
+abs/2210.07573) - **[ICML 2022]** [SautÃ© RL: Almost Surely Safe Reinforcement
+Learning Using State Augmentation (SauteRL)](https://arxiv.org/abs/2202.06558)
+- **[IJCAI 2022]** [Penalized Proximal Policy Optimization for Safe
+Reinforcement Learning](https://arxiv.org/abs/2205.11814) - **[AAAI 2022]**
 [Conservative and Adaptive Penalty for Model-Based Safe Reinforcement Learning
-(CAP)](https://arxiv.org/abs/2112.07701) - [x] **[NeurIPS 2022]** [Model-based
-Safe Deep Reinforcement Learning via a Constrained Proximal Policy Optimization
+(CAP)](https://arxiv.org/abs/2112.07701) LLiisstt ooff AAllggoorriitthhmmss OOnn PPoolliiccyy SSaaffeeRRLL -
+[x] [The Lagrange version of PPO (PPO-Lag)](https://cdn.openai.com/safexp-
+short.pdf) - [x] [The Lagrange version of TRPO (TRPO-Lag)](https://
+cdn.openai.com/safexp-short.pdf) - [x] **[ICML 2017]** [Constrained Policy
+Optimization (CPO)](https://proceedings.mlr.press/v70/achiam17a) - [x] **[ICLR
+2019]** [Reward Constrained Policy Optimization (RCPO)](https://openreview.net/
+forum?id=SkfrvsA9FX) - [x] **[ICML 2020]** [Responsive Safety in Reinforcement
+Learning by PID Lagrangian Methods (PID-Lag)](https://arxiv.org/abs/2007.03964)
+- [x] **[NeurIPS 2020]** [First Order Constrained Optimization in Policy Space
+(FOCOPS)](https://arxiv.org/abs/2002.06506) - [x] **[AAAI 2020]** [IPO:
+Interior-point Policy Optimization under Constraints (IPO)](https://arxiv.org/
+abs/1910.09615) - [x] **[ICLR 2020]** [Projection-Based Constrained Policy
+Optimization (PCPO)](https://openreview.net/forum?id=rke3TJrtPS) - [x] **[ICML
+2021]** [CRPO: A New Approach for Safe Reinforcement Learning with Convergence
+Guarantee](https://arxiv.org/abs/2011.05869) - [x] **[IJCAI 2022]** [Penalized
+Proximal Policy Optimization for Safe Reinforcement Learning(P3O)](https://
+arxiv.org/pdf/2205.11814.pdf) OOffff PPoolliiccyy SSaaffeeRRLL - **[Preprint 2019]** [The
+Lagrangian version of DDPG (DDPGLag)](https://cdn.openai.com/safexp-short.pdf)
+- **[Preprint 2019]** [The Lagrangian version of TD3 (TD3Lag)](https://
+cdn.openai.com/safexp-short.pdf) - **[Preprint 2019]** [The Lagrangian version
+of SAC (SACLag)](https://cdn.openai.com/safexp-short.pdf) - **[ICML 2020]**
+[Responsive Safety in Reinforcement Learning by PID Lagrangian Methods
+(DDPGPID)](https://arxiv.org/abs/2007.03964) - **[ICML 2020]** [Responsive
+Safety in Reinforcement Learning by PID Lagrangian Methods (TD3PID)](https://
+arxiv.org/abs/2007.03964) - **[ICML 2020]** [Responsive Safety in Reinforcement
+Learning by PID Lagrangian Methods (SACPID)](https://arxiv.org/abs/2007.03964)
+MMooddeell--BBaasseedd SSaaffeeRRLL - [ ] **[NeurIPS 2021]** [Safe Reinforcement Learning by
+Imagining the Near Future (SMBPO)](https://arxiv.org/abs/2202.07789) - [x] **
+[CoRL 2021 (Oral)]** [Learning Off-Policy with Online Planning (SafeLOOP)]
+(https://arxiv.org/abs/2008.10066) - [x] **[AAAI 2022]** [Conservative and
+Adaptive Penalty for Model-Based Safe Reinforcement Learning (CAP)](https://
+arxiv.org/abs/2112.07701) - [x] **[NeurIPS 2022]** [Model-based Safe Deep
+Reinforcement Learning via a Constrained Proximal Policy Optimization
 Algorithm](https://arxiv.org/abs/2210.07573) - [ ] **[ICLR 2022]** [Constrained
 Policy Optimization via Bayesian World Models (LA-MBDA)](https://arxiv.org/abs/
 2201.09802) - [x] **[ICML 2022 Workshop]** [Constrained Model-based
 Reinforcement Learning with Robust Cross-Entropy Method (RCE)](https://
 arxiv.org/abs/2010.07968) - [x] **[NeurIPS 2018]** [Constrained Cross-Entropy
 Method for Safe Reinforcement Learning (CCE)](https://proceedings.neurips.cc/
 paper/2018/hash/34ffeb359a192eb8174b6854643cc046-Abstract.html) OOfffflliinnee SSaaffeeRRLL
@@ -165,60 +167,92 @@
 |Safe Navigation|_B_u_t_t_o_n_[_0_1_2_]|Point, Car, Racecar, Ant|SafetyPointGoal1-v0    |
 |               |_P_u_s_h_[_0_1_2_]_ _ |                        |                       |
 |_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_C_i_r_c_l_e_[_0_1_2_]_|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |               |           |HalfCheetah, Hopper,    |SafetyHumanoidVelocity-|
 |Safe Velocity  |Velocity   |Swimmer, Walker2d, Ant, |v1                     |
 |_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _|_H_u_m_a_n_o_i_d_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 For more information about environments, please refer to [Safety-Gymnasium]
-(https://www.safety-gymnasium.com). #### Try with CLI ```bash pip install
-omnisafe omnisafe --help # Ask for help omnisafe benchmark --help # The
-benchmark also can be replaced with 'eval', 'train', 'train-config' # Quick
-benchmarking for your research, just specify: # 1. exp_name # 2. num_pool(how
-much processes are concurrent) # 3. path of the config file (refer to omnisafe/
-examples/benchmarks for format) # Here we provide an exampe in ./tests/
-saved_source. # And you can set your benchmark_config.yaml by following it
-omnisafe benchmark test_benchmark 2 ./tests/saved_source/benchmark_config.yaml
-# Quick evaluating and rendering your trained policy, just specify: # 1. path
-of algorithm which you trained omnisafe eval ./tests/saved_source/PPO-
-{SafetyPointGoal1-v0} --num-episode 1 # Quick training some algorithms to
-validate your thoughts # Note: use `key1:key2`, your can select key of
-hyperparameters which are recursively contained, and use `--custom-cfgs`, you
-can add custom cfgs via CLI omnisafe train --algo PPO --total-steps 2048 --
-vector-env-nums 1 --custom-cfgs algo_cfgs:steps_per_epoch --custom-cfgs 1024 #
-Quick training some algorithms via a saved config file, the format is as same
-as default format omnisafe train-config ./tests/saved_source/train_config.yaml
-``` ---------------------------------------------------------------------------
------ ## Getting Started ### Important Hints We have provided benchmark results
-for various algorithms, including on-policy, off-policy, model-based, and
-offline approaches, along with parameter tuning analysis. Please refer to the
-following: - [On-Policy](./benchmarks/on-policy/) - [Off-Policy](./benchmarks/
-off-policy/) - [Model-based](./benchmarks/model-based/) - [Offline](./
-benchmarks/offline/) ### Quickstart: Colab on the Cloud Explore OmniSafe easily
-and quickly through a series of Google Colab notebooks: - [Getting Started]
+(https://www.safety-gymnasium.com). #### Customizing your environment We offer
+a flexible customized environment interface that allows users to achieve the
+following **without modifying the OmniSafe source code**: - Use OmniSafe to
+train algorithms on customized environments. - Create the the environment with
+specified personalized parameters. - Complete the recording of environment-
+specific information in Logger. We provide **step-by-step tutorials** on
+[Environment Customization From Scratch](https://colab.research.google.com/
+github/PKU-Alignment/omnisafe/blob/main/tutorials/English/
+3.Environment%20Customization%20from%20Scratch.ipynb) and [Environment
+Customization From Community](https://colab.research.google.com/github/PKU-
+Alignment/omnisafe/blob/main/tutorials/English/
+4.Environment%20Customization%20from%20Community.ipynb) to give you a detailed
+introduction on how to use this extraordinary feature of OmniSafe. *Note: If
+you find trouble customizing your environment, please feel free to open an
+[issue](https://github.com/PKU-Alignment/omnisafe/issues) or [discussion]
+(https://github.com/PKU-Alignment/omnisafe/discussions). [Pull requests](https:
+//github.com/PKU-Alignment/omnisafe/pulls) are also welcomed if you're willing
+to contribute the implementation of your environments interface.* #### Try with
+CLI ```bash pip install omnisafe omnisafe --help # Ask for help omnisafe
+benchmark --help # The benchmark also can be replaced with 'eval', 'train',
+'train-config' # Quick benchmarking for your research, just specify: # 1.
+exp_name # 2. num_pool(how much processes are concurrent) # 3. path of the
+config file (refer to omnisafe/examples/benchmarks for format) # Here we
+provide an exampe in ./tests/saved_source. # And you can set your
+benchmark_config.yaml by following it omnisafe benchmark test_benchmark 2 ./
+tests/saved_source/benchmark_config.yaml # Quick evaluating and rendering your
+trained policy, just specify: # 1. path of algorithm which you trained omnisafe
+eval ./tests/saved_source/PPO-{SafetyPointGoal1-v0} --num-episode 1 # Quick
+training some algorithms to validate your thoughts # Note: use `key1:key2`,
+your can select key of hyperparameters which are recursively contained, and use
+`--custom-cfgs`, you can add custom cfgs via CLI omnisafe train --algo PPO --
+total-steps 2048 --vector-env-nums 1 --custom-cfgs algo_cfgs:steps_per_epoch --
+custom-cfgs 1024 # Quick training some algorithms via a saved config file, the
+format is as same as default format omnisafe train-config ./tests/saved_source/
+train_config.yaml ``` ---------------------------------------------------------
+----------------------- ## Getting Started ### Important Hints We have provided
+benchmark results for various algorithms, including on-policy, off-policy,
+model-based, and offline approaches, along with parameter tuning analysis.
+Please refer to the following: - [On-Policy](./benchmarks/on-policy/) - [Off-
+Policy](./benchmarks/off-policy/) - [Model-based](./benchmarks/model-based/) -
+[Offline](./benchmarks/offline/) ### Quickstart: Colab on the Cloud Explore
+OmniSafe easily and quickly through a series of Google Colab notebooks: -
+[Getting Started](https://colab.research.google.com/github/PKU-Alignment/
+omnisafe/blob/main/tutorials/English/1.Getting_Started.ipynb) Introduce the
+basic usage of OmniSafe so that users can quickly hand it. - [CLI Command]
 (https://colab.research.google.com/github/PKU-Alignment/omnisafe/blob/main/
-tutorials/English/1.Getting_Started.ipynb) Introduce the basic usage of
-OmniSafe so that users can quickly hand it. - [CLI Command](https://
-colab.research.google.com/github/PKU-Alignment/omnisafe/blob/main/tutorials/
-English/2.CLI_Command.ipynb) Introduce how to use the CLI tool of OmniSafe. We
-take great pleasure in collaborating with our users to create tutorials in
-various languages. Please refer to our list of currently supported languages.
-If you are interested in translating the tutorial into a new language or
-improving an existing version, kindly submit a PR to us. ----------------------
----------------------------------------------------------- ## Changelog See
-[CHANGELOG.md](https://github.com/PKU-Alignment/omnisafe/blob/main/
-CHANGELOG.md). ## Citing OmniSafe If you find OmniSafe useful or use OmniSafe
-in your research, please cite it in your publications. ```bibtex @article
-{omnisafe, title = {OmniSafe: An Infrastructure for Accelerating Safe
+tutorials/English/2.CLI_Command.ipynb) Introduce how to use the CLI tool of
+OmniSafe. We take great pleasure in collaborating with our users to create
+tutorials in various languages. Please refer to our list of currently supported
+languages. If you are interested in translating the tutorial into a new
+language or improving an existing version, kindly submit a PR to us. ----------
+---------------------------------------------------------------------- ##
+Changelog See [CHANGELOG.md](https://github.com/PKU-Alignment/omnisafe/blob/
+main/CHANGELOG.md). ## Citing OmniSafe If you find OmniSafe useful or use
+OmniSafe in your research, please cite it in your publications. ```bibtex
+@article{omnisafe, title = {OmniSafe: An Infrastructure for Accelerating Safe
 Reinforcement Learning Research}, author = {Jiaming Ji, Jiayi Zhou, Borong
 Zhang, Juntao Dai, Xuehai Pan, Ruiyang Sun, Weidong Huang, Yiran Geng, Mickel
 Liu, Yaodong Yang}, journal = {arXiv preprint arXiv:2305.09304}, year = {2023}
-} ``` ## The OmniSafe Team OmniSafe is mainly developed by the SafeRL research
-team directed by Prof. [Yaodong Yang](https://www.yangyaodong.com/). Our SafeRL
-research team members include [Borong Zhang](https://github.com/muchvo), [Jiayi
-Zhou](https://github.com/Gaiejj), [JTao Dai](https://github.com/calico-1226),
-[Weidong Huang](https://github.com/hdadong), [Ruiyang Sun](https://github.com/
-rockmagma02), [Xuehai Pan](https://github.com/XuehaiPan) and [Jiaming Ji]
-(https://github.com/zmsn-2077). If you have any questions in the process of
-using OmniSafe, don't hesitate to ask your questions on [the GitHub issue page]
-(https://github.com/PKU-Alignment/omnisafe/issues/new/choose), we will reply to
-you in 2-3 working days. ## License OmniSafe is released under Apache License
-2.0.
+} ``` ## Publications using OmniSafe We have compiled a list of papers that use
+OmniSafe for algorithm implementation or experimentation. If you are willing to
+include your work in this list, or if you wish to have your implementation
+officially integrated into OmniSafe, please feel free to [contact us](https://
+github.com/PKU-Alignment/omnisafe/issues). | Papers | Publisher| |:---:|:---:
+| | [Off-Policy Primal-Dual Safe Reinforcement Learning](https://
+openreview.net/pdf?id=vy42bYs1Wo) | ICLR 2024 | | [Safe Offline Reinforcement
+Learning with Feasibility-Guided Diffusion Model](https://openreview.net/
+pdf?id=j5JvZCaDM0) | ICLR 2024 | | [Iterative Reachability Estimation for Safe
+Reinforcement Learning](https://proceedings.neurips.cc/paper_files/paper/2023/
+file/dca63f2650fe9e88956c1b68440b8ee9-Paper-Conference.pdf) | NeurIPS 2023 | |
+[Balance Reward and Safety Optimization for Safe Reinforcement Learning: A
+Perspective of Gradient Manipulation](https://ojs.aaai.org/index.php/AAAI/
+article/view/30102/31944) | AAAI 2024 | | [Learning Safety Constraints From
+Demonstration Using One-Class Decision Trees](https://openreview.net/
+pdf?id=dxUi16pvub) | AAAI 2024 WorkShops | ## The OmniSafe Team OmniSafe is
+mainly developed by the SafeRL research team directed by Prof. [Yaodong Yang]
+(https://www.yangyaodong.com/). Our SafeRL research team members include
+[Borong Zhang](https://github.com/muchvo), [Jiayi Zhou](https://github.com/
+Gaiejj), [JTao Dai](https://github.com/calico-1226), [Weidong Huang](https://
+github.com/hdadong), [Ruiyang Sun](https://github.com/rockmagma02), [Xuehai
+Pan](https://github.com/XuehaiPan) and [Jiaming Ji](https://github.com/zmsn-
+2077). If you have any questions in the process of using OmniSafe, don't
+hesitate to ask your questions on [the GitHub issue page](https://github.com/
+PKU-Alignment/omnisafe/issues/new/choose), we will reply to you in 2-3 working
+days. ## License OmniSafe is released under Apache License 2.0.
```

### Comparing `omnisafe-0.5.0b0/omnisafe/__init__.py` & `omnisafe-0.5.1b0/omnisafe/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/adapter/__init__.py` & `omnisafe-0.5.1b0/omnisafe/adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/adapter/early_terminated_adapter.py` & `omnisafe-0.5.1b0/omnisafe/adapter/early_terminated_adapter.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/adapter/modelbased_adapter.py` & `omnisafe-0.5.1b0/omnisafe/adapter/modelbased_adapter.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/adapter/offline_adapter.py` & `omnisafe-0.5.1b0/omnisafe/adapter/offline_adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -91,22 +91,30 @@
             cost: The amount of cost returned after previous action.
             terminated: Whether the episode has ended.
             truncated: Whether the episode has been truncated due to a time limit.
             info: Some information logged by the environment.
         """
         return self._env.step(actions)
 
-    def reset(self) -> tuple[torch.Tensor, dict[str, Any]]:
+    def reset(
+        self,
+        seed: int | None = None,
+        options: dict[str, Any] | None = None,
+    ) -> tuple[torch.Tensor, dict[str, Any]]:
         """Reset the environment and returns an initial observation.
 
+        Args:
+            seed (int, optional): The random seed. Defaults to None.
+            options (dict[str, Any], optional): The options for the environment. Defaults to None.
+
         Returns:
             observation: The initial observation of the space.
             info: Some information logged by the environment.
         """
-        return self._env.reset()
+        return self._env.reset(seed=seed, options=options)
 
     def evaluate(
         self,
         evaluate_epoisodes: int,
         agent: Actor,
         logger: Logger,
     ) -> None:
```

### Comparing `omnisafe-0.5.0b0/omnisafe/adapter/offpolicy_adapter.py` & `omnisafe-0.5.1b0/omnisafe/adapter/offpolicy_adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -122,26 +122,25 @@
                 and cost critic.
             buffer (VectorOnPolicyBuffer): Vector on-policy buffer.
             logger (Logger): Logger, to log ``EpRet``, ``EpCost``, ``EpLen``.
             use_rand_action (bool): Whether to use random action.
         """
         for _ in range(rollout_step):
             if use_rand_action:
-                act = torch.as_tensor(self._env.sample_action(), dtype=torch.float32).to(
-                    self._device,
-                )
+                act = (torch.rand(self.action_space.shape) * 2 - 1).unsqueeze(0).to(self._device)  # type: ignore
             else:
                 act = agent.step(self._current_obs, deterministic=False)
             next_obs, reward, cost, terminated, truncated, info = self.step(act)
 
             self._log_value(reward=reward, cost=cost, info=info)
             real_next_obs = next_obs.clone()
             for idx, done in enumerate(torch.logical_or(terminated, truncated)):
                 if done:
-                    real_next_obs[idx] = info['final_observation'][idx]
+                    if 'final_observation' in info:
+                        real_next_obs[idx] = info['final_observation'][idx]
                     self._log_metrics(logger, idx)
                     self._reset_log(idx)
 
             buffer.store(
                 obs=self._current_obs,
                 act=act,
                 reward=reward,
@@ -176,14 +175,16 @@
     def _log_metrics(self, logger: Logger, idx: int) -> None:
         """Log metrics, including ``EpRet``, ``EpCost``, ``EpLen``.
 
         Args:
             logger (Logger): Logger, to log ``EpRet``, ``EpCost``, ``EpLen``.
             idx (int): The index of the environment.
         """
+        if hasattr(self._env, 'spec_log'):
+            self._env.spec_log(logger)
         logger.store(
             {
                 'Metrics/EpRet': self._ep_ret[idx],
                 'Metrics/EpCost': self._ep_cost[idx],
                 'Metrics/EpLen': self._ep_len[idx],
             },
         )
```

### Comparing `omnisafe-0.5.0b0/omnisafe/adapter/online_adapter.py` & `omnisafe-0.5.1b0/omnisafe/adapter/online_adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,25 +58,30 @@
     ) -> None:
         """Initialize an instance of :class:`OnlineAdapter`."""
         assert env_id in support_envs(), f'Env {env_id} is not supported.'
 
         self._cfgs: Config = cfgs
         self._device: torch.device = get_device(cfgs.train_cfgs.device)
         self._env_id: str = env_id
-        self._env: CMDP = make(env_id, num_envs=num_envs, device=self._device)
-        self._eval_env: CMDP = make(env_id, num_envs=1, device=self._device)
+
+        env_cfgs = {}
+
+        if hasattr(self._cfgs, 'env_cfgs') and self._cfgs.env_cfgs is not None:
+            env_cfgs = self._cfgs.env_cfgs.todict()
+
+        self._env: CMDP = make(env_id, num_envs=num_envs, device=self._device, **env_cfgs)
+        self._eval_env: CMDP = make(env_id, num_envs=1, device=self._device, **env_cfgs)
 
         self._wrapper(
             obs_normalize=cfgs.algo_cfgs.obs_normalize,
             reward_normalize=cfgs.algo_cfgs.reward_normalize,
             cost_normalize=cfgs.algo_cfgs.cost_normalize,
         )
 
         self._env.set_seed(seed)
-        self._eval_env.set_seed(seed)
 
     def _wrapper(
         self,
         obs_normalize: bool = True,
         reward_normalize: bool = True,
         cost_normalize: bool = True,
     ) -> None:
@@ -106,16 +111,28 @@
 
         Args:
             obs_normalize (bool, optional): Whether to normalize the observation. Defaults to True.
             reward_normalize (bool, optional): Whether to normalize the reward. Defaults to True.
             cost_normalize (bool, optional): Whether to normalize the cost. Defaults to True.
         """
         if self._env.need_time_limit_wrapper:
-            self._env = TimeLimit(self._env, time_limit=1000, device=self._device)
-            self._eval_env = TimeLimit(self._eval_env, time_limit=1000, device=self._device)
+            assert (
+                self._env.max_episode_steps and self._eval_env.max_episode_steps
+            ), 'You must define max_episode_steps as an integer\
+                or cancel the use of the time_limit wrapper.'
+            self._env = TimeLimit(
+                self._env,
+                time_limit=self._env.max_episode_steps,
+                device=self._device,
+            )
+            self._eval_env = TimeLimit(
+                self._eval_env,
+                time_limit=self._eval_env.max_episode_steps,
+                device=self._device,
+            )
         if self._env.need_auto_reset_wrapper:
             self._env = AutoReset(self._env, device=self._device)
             self._eval_env = AutoReset(self._eval_env, device=self._device)
         if obs_normalize:
             self._env = ObsNormalize(self._env, device=self._device)
             self._eval_env = ObsNormalize(self._eval_env, device=self._device)
         if reward_normalize:
@@ -160,28 +177,47 @@
             cost: The amount of cost returned after previous action.
             terminated: Whether the episode has ended.
             truncated: Whether the episode has been truncated due to a time limit.
             info: Some information logged by the environment.
         """
         return self._env.step(action)
 
-    def reset(self) -> tuple[torch.Tensor, dict[str, Any]]:
+    def reset(
+        self,
+        seed: int | None = None,
+        options: dict[str, Any] | None = None,
+    ) -> tuple[torch.Tensor, dict[str, Any]]:
         """Reset the environment and returns an initial observation.
 
+        Args:
+            seed (int, optional): The random seed. Defaults to None.
+            options (dict[str, Any], optional): The options for the environment. Defaults to None.
+
         Returns:
             observation: The initial observation of the space.
             info: Some information logged by the environment.
         """
-        return self._env.reset()
+        return self._env.reset(seed=seed, options=options)
 
     def save(self) -> dict[str, torch.nn.Module]:
         """Save the important components of the environment.
 
         .. note::
             The saved components will be stored in the wrapped environment. If the environment is
             not wrapped, the saved components will be an empty dict. common wrappers are
             ``obs_normalize``, ``reward_normalize``, and ``cost_normalize``.
 
         Returns:
             The saved components of environment, e.g., ``obs_normalizer``.
         """
         return self._env.save()
+
+    def close(self) -> None:
+        """Close the environment after training."""
+        self._env.close()
+
+    @property
+    def env_spec_keys(self) -> list[str]:
+        """Return the environment specification log."""
+        if hasattr(self._env, 'env_spec_log'):
+            return list(self._env.env_spec_log.keys())
+        return []
```

### Comparing `omnisafe-0.5.0b0/omnisafe/adapter/onpolicy_adapter.py` & `omnisafe-0.5.1b0/omnisafe/adapter/onpolicy_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,14 +154,16 @@
     def _log_metrics(self, logger: Logger, idx: int) -> None:
         """Log metrics, including ``EpRet``, ``EpCost``, ``EpLen``.
 
         Args:
             logger (Logger): Logger, to log ``EpRet``, ``EpCost``, ``EpLen``.
             idx (int): The index of the environment.
         """
+        if hasattr(self._env, 'spec_log'):
+            self._env.spec_log(logger)
         logger.store(
             {
                 'Metrics/EpRet': self._ep_ret[idx],
                 'Metrics/EpCost': self._ep_cost[idx],
                 'Metrics/EpLen': self._ep_len[idx],
             },
         )
```

### Comparing `omnisafe-0.5.0b0/omnisafe/adapter/saute_adapter.py` & `omnisafe-0.5.1b0/omnisafe/adapter/saute_adapter.py`

 * *Files 7% similar despite different names*

```diff
@@ -105,25 +105,33 @@
             self._env = ObsNormalize(self._env, device=self._device)
         assert reward_normalize is False, 'Reward normalization is not supported'
         assert cost_normalize is False, 'Cost normalization is not supported'
         self._env = ActionScale(self._env, device=self._device, low=-1.0, high=1.0)
         if self._env.num_envs == 1:
             self._env = Unsqueeze(self._env, device=self._device)
 
-    def reset(self) -> tuple[torch.Tensor, dict[str, Any]]:
+    def reset(
+        self,
+        seed: int | None = None,
+        options: dict[str, Any] | None = None,
+    ) -> tuple[torch.Tensor, dict[str, Any]]:
         """Reset the environment and returns an initial observation.
 
         .. note::
             Additionally, the safety observation will be reset.
 
+        Args:
+            seed (int, optional): The random seed. Defaults to None.
+            options (dict[str, Any], optional): The options for the environment. Defaults to None.
+
         Returns:
             observation: The initial observation of the space.
             info: Some information logged by the environment.
         """
-        obs, info = self._env.reset()
+        obs, info = self._env.reset(seed=seed, options=options)
         self._safety_obs = torch.ones(self._env.num_envs, 1).to(self._device)
         obs = self._augment_obs(obs)
         return obs, info
 
     def step(
         self,
         action: torch.Tensor,
```

### Comparing `omnisafe-0.5.0b0/omnisafe/adapter/simmer_adapter.py` & `omnisafe-0.5.1b0/omnisafe/adapter/simmer_adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,26 +84,34 @@
             shape=(self._env.observation_space.shape[0] + 1,),
         )
         self._controller: BaseSimmerAgent = SimmerPIDAgent(
             cfgs=cfgs.control_cfgs,
             budget_bound=self._upper_budget.cpu(),
         )
 
-    def reset(self) -> tuple[torch.Tensor, dict[str, Any]]:
+    def reset(
+        self,
+        seed: int | None = None,
+        options: dict[str, Any] | None = None,
+    ) -> tuple[torch.Tensor, dict[str, Any]]:
         """Reset the environment and returns an initial observation.
 
         .. note::
             Additionally, the safety observation will be reset. And the safety budget will be reset
             to the value of current ``rel_safety_budget``.
 
+        Args:
+            seed (int, optional): The random seed. Defaults to None.
+            options (dict[str, Any], optional): The options for the environment. Defaults to None.
+
         Returns:
             observation: The initial observation of the space.
             info: Some information logged by the environment.
         """
-        obs, info = self._env.reset()
+        obs, info = self._env.reset(seed=seed, options=options)
         self._safety_obs = self._rel_safety_budget * torch.ones(self._num_envs, 1).to(self._device)
         obs = self._augment_obs(obs)
         return obs, info
 
     def control_budget(self, ep_costs: torch.Tensor) -> None:
         """Control the safety budget.
 
@@ -116,7 +124,8 @@
             / (1 - self._cfgs.algo_cfgs.saute_gamma)
             / self._cfgs.algo_cfgs.max_ep_len
         )
         self._safety_budget = self._controller.act(
             safety_budget=self._safety_budget.cpu(),
             observation=ep_costs.cpu(),
         ).to(self._device)
+        self._rel_safety_budget = (self._safety_budget / self._upper_budget).to(self._device)
```

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/__init__.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/algo_wrapper.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/algo_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,21 +84,23 @@
         Raises:
             AssertionError: If the algorithm name is not in the supported algorithms.
         """
         assert (
             self.algo in ALGORITHMS['all']
         ), f"{self.algo} doesn't exist. Please choose from {ALGORITHMS['all']}."
         self.algo_type = ALGORITHM2TYPE.get(self.algo, '')
-        if self.algo_type in ['model-based', 'offline'] and self.train_terminal_cfgs is not None:
-            assert (
-                self.train_terminal_cfgs['parallel'] == 1
-            ), 'model-based and offline only support parallel==1!'
-            assert (
-                self.train_terminal_cfgs['vector_env_nums'] == 1
-            ), 'model-based and offline only support vector_env_nums==1!'
+        if self.train_terminal_cfgs is not None:
+            if self.algo_type in ['model-based', 'offline']:
+                assert (
+                    self.train_terminal_cfgs['vector_env_nums'] == 1
+                ), 'model-based and offline only support vector_env_nums==1!'
+            if self.algo_type in ['off-policy', 'model-based', 'offline']:
+                assert (
+                    self.train_terminal_cfgs['parallel'] == 1
+                ), 'off-policy, model-based and offline only support parallel==1!'
 
         cfgs = get_default_kwargs_yaml(self.algo, self.env_id, self.algo_type)
 
         # update the cfgs from custom configurations
         if self.custom_cfgs:
             # avoid repeatedly record the env_id and algo
             if 'env_id' in self.custom_cfgs:
@@ -141,26 +143,29 @@
         assert (
             self.env_id in support_envs()
         ), f"{self.env_id} doesn't exist. Please choose from {support_envs()}."
 
     def _init_algo(self) -> None:
         """Initialize the algorithm."""
         check_all_configs(self.cfgs, self.algo_type)
-        device = self.cfgs.train_cfgs.device
-        if device == 'cpu':
-            torch.set_num_threads(self.cfgs.train_cfgs.torch_threads)
-        else:
-            torch.set_num_threads(1)
-            torch.cuda.set_device(self.cfgs.train_cfgs.device)
         if distributed.fork(
             self.cfgs.train_cfgs.parallel,
             device=self.cfgs.train_cfgs.device,
         ):
             # re-launches the current script with workers linked by MPI
             sys.exit()
+        if self.cfgs.train_cfgs.device == 'cpu':
+            torch.set_num_threads(self.cfgs.train_cfgs.torch_threads)
+        else:
+            if self.cfgs.train_cfgs.parallel > 1 and os.getenv('MASTER_ADDR') is not None:
+                ddp_local_rank = int(os.environ['LOCAL_RANK'])
+                self.cfgs.train_cfgs.device = f'cuda:{ddp_local_rank}'
+            torch.set_num_threads(1)
+            torch.cuda.set_device(self.cfgs.train_cfgs.device)
+        os.environ['OMNISAFE_DEVICE'] = self.cfgs.train_cfgs.device
         self.agent: BaseAlgo = registry.get(self.algo)(
             env_id=self.env_id,
             cfgs=self.cfgs,
         )
 
     def learn(self) -> tuple[float, float, float]:
         """Agent learning.
```

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/base_algo.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/base_algo.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/model_based/__init__.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/model_based/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/model_based/base/__init__.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/model_based/base/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/model_based/base/ensemble.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/model_based/base/ensemble.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,15 @@
         input_data (torch.Tensor): The input data.
         index (int): The index of the model to use.
 
     Returns:
         output: The output of the layer.
     """
     if isinstance(layer, EnsembleFC):
+        # pylint: disable-next=not-callable
         output = F.linear(
             input_data,
             torch.transpose(layer.weight[index].squeeze(0), 0, 1),
             layer.bias[index],
         )
 
     else:
@@ -202,16 +203,16 @@
             input_data (torch.Tensor): The input data.
 
         Returns:
             The forward output of the network.
         """
         w_times_x = torch.bmm(input_data, self.weight)
         if self.bias is not None:
-            return torch.add(w_times_x, self.bias[:, None, :])  # w times x + b
-        return w_times_x  # type: ignore
+            w_times_x = torch.add(w_times_x, self.bias[:, None, :])  # w times x + b
+        return w_times_x
 
 
 # pylint: disable-next=too-many-instance-attributes
 class EnsembleModel(nn.Module):
     """Ensemble dynamics model.
 
     A dynamics model with ensemble_size models.
@@ -310,14 +311,15 @@
         self.scaler: StandardScaler = StandardScaler(self._device)
 
     def forward(
         self,
         data: torch.Tensor | np.ndarray,
         ret_log_var: bool = False,
     ) -> tuple[torch.Tensor, torch.Tensor]:
+        # pylint: disable=not-callable
         """Compute next state, reward, cost using all models.
 
         Args:
             data (torch.Tensor): Input data.
             ret_log_var (bool, optional): Whether to return the log variance, defaults to False.
 
         Returns:
@@ -340,14 +342,15 @@
         )
         logvar = self.min_logvar + F.softplus(logvar - self.min_logvar)
         var = torch.exp(logvar)
         if ret_log_var:
             return mean, logvar
         return mean, var
 
+    # pylint: disable=not-callable
     def forward_idx(
         self,
         data: torch.Tensor | np.ndarray,
         idx_model: int,
         ret_log_var: bool = False,
     ) -> tuple[torch.Tensor, torch.Tensor]:
         """Compute next state, reward, cost from an certain model.
```

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/model_based/base/loop.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/model_based/base/loop.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,15 +301,15 @@
             cost (torch.Tensor): The cost signal from the environment.
             terminated (torch.Tensor): The terminated signal from the environment.
             truncated (torch.Tensor): The truncated signal from the environment.
             next_state (torch.Tensor): The next state from the environment.
             info (dict[str, Any]): The information from the environment.
         """
         done = terminated or truncated
-        goal_met = False if 'goal_met' not in info.keys() else info['goal_met']
+        goal_met = info.get('goal_met', False)
         if not done and not goal_met:
             # when goal_met == true:
             # current goal position is not related to the last goal position,
             # this huge transition will confuse the dynamics model.
             self._dynamics_buf.store(
                 obs=state,
                 act=action,
```

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/model_based/base/pets.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/model_based/base/pets.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,15 +329,15 @@
             **{
                 'Loss/DynamicsTrainMseLoss': train_mse_losses.item(),
                 'Loss/DynamicsValMseLoss': val_mse_losses.item(),
             },
         )
 
     def _update_epoch(self) -> None:
-        ...
+        """Update function per epoch."""
 
     def _select_action(  # pylint: disable=unused-argument
         self,
         current_step: int,
         state: torch.Tensor,
     ) -> torch.Tensor:
         """Select action.
@@ -380,15 +380,15 @@
             cost (torch.Tensor): The cost signal from the environment.
             terminated (torch.Tensor): The terminated signal from the environment.
             truncated (torch.Tensor): The truncated signal from the environment.
             next_state (torch.Tensor): The next state from the environment.
             info (dict[str, Any]): The information from the environment.
         """
         done = terminated or truncated
-        goal_met = False if 'goal_met' not in info.keys() else info['goal_met']
+        goal_met = info.get('goal_met', False)
         if not terminated and not truncated and not goal_met:
             # pylint: disable-next=line-too-long
             # if goal_met == true, Current goal position is not related to the last goal position, this huge transition will confuse the dynamics model.
             self._dynamics_buf.store(
                 obs=state,
                 act=action,
                 reward=reward,
```

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/model_based/cap_pets.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/model_based/cap_pets.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/model_based/cce_pets.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/model_based/cce_pets.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/model_based/planner/__init__.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/model_based/planner/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/model_based/planner/arc.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/model_based/planner/arc.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,22 +220,22 @@
         return elite_values, elite_actions, info
 
     @torch.no_grad()
     def _update_mean_var(
         self,
         elite_actions: torch.Tensor,
         elite_values: torch.Tensor,
-        info: dict[str, int | float],
+        info: dict[str, float],
     ) -> tuple[torch.Tensor, torch.Tensor]:  # pylint: disable-next=unused-argument
         """Update the mean and variance of the elite actions.
 
         Args:
             elite_actions (torch.Tensor): The elite actions.
             elite_values (torch.Tensor): The elite values.
-            info (dict[str, int | float]): The dictionary containing the information of the elite values and actions.
+            info (dict[str, float]): The dictionary containing the information of the elite values and actions.
 
         Returns:
             new_mean: The new mean of the elite actions.
             new_var: The new variance of the elite actions.
         """
         assert (
             elite_actions.shape[0] == self._horizon
@@ -257,15 +257,15 @@
             dim=1,
         ) / (score.sum(0) + 1e-9)
         new_var = new_var.clamp_(0, 2)
 
         return new_mean, new_var
 
     @torch.no_grad()
-    def output_action(self, state: torch.Tensor) -> tuple[torch.Tensor, dict[str, int | float]]:
+    def output_action(self, state: torch.Tensor) -> tuple[torch.Tensor, dict[str, float]]:
         """Output the action given the state.
 
         Args:
             state (torch.Tensor): State of the environment.
 
         Returns:
             action: The action of the agent.
```

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/model_based/planner/cap.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/model_based/planner/cap.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/model_based/planner/cce.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/model_based/planner/cce.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/model_based/planner/cem.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/model_based/planner/cem.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,22 +194,22 @@
         return elite_values, elite_actions, info
 
     @torch.no_grad()
     def _update_mean_var(  # pylint: disable=unused-argument
         self,
         elite_actions: torch.Tensor,
         elite_values: torch.Tensor,
-        info: dict[str, int | float],
+        info: dict[str, float],
     ) -> tuple[torch.Tensor, torch.Tensor]:
         """Update the mean and variance of the elite actions.
 
         Args:
             elite_actions (torch.Tensor): The elite actions.
             elite_values (torch.Tensor): The elite values.
-            info (dict[str, int | float]): The dictionary containing the information of the elite values and actions.
+            info (dict[str, float]): The dictionary containing the information of the elite values and actions.
 
         Returns:
             new_mean: The new mean of the elite actions.
             new_var: The new variance of the elite actions.
         """
         assert elite_actions.shape == torch.Size(
             [self._horizon, self._num_elites, *self._action_shape],
```

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/model_based/planner/rce.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/model_based/planner/rce.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/model_based/planner/safe_arc.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/model_based/planner/safe_arc.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,22 +65,22 @@
         self._cost_temperature: float = planner_cfgs.cost_temperature
 
     @torch.no_grad()
     def _update_mean_var(
         self,
         elite_actions: torch.Tensor,
         elite_values: torch.Tensor,
-        info: dict[str, int | float],
+        info: dict[str, float],
     ) -> tuple[torch.Tensor, torch.Tensor]:
         """Update the mean and variance of the elite actions.
 
         Args:
             elite_actions (torch.Tensor): The elite actions.
             elite_values (torch.Tensor): The elite values.
-            info (dict[str, int | float]): The dictionary containing the information of the elite values and actions.
+            info (dict[str, float]): The dictionary containing the information of the elite values and actions.
 
         Returns:
             new_mean: The new mean of the elite actions.
             new_var: The new variance of the elite actions.
         """
         assert (
             elite_actions.shape[0] == self._horizon
@@ -193,15 +193,15 @@
             'Plan/episode_costs_mean': mean_episode_costs.mean().item(),
             'Plan/episode_costs_min': mean_episode_costs.min().item(),
         }
 
         return elite_values, elite_actions, info
 
     @torch.no_grad()
-    def output_action(self, state: torch.Tensor) -> tuple[torch.Tensor, dict[str, int | float]]:
+    def output_action(self, state: torch.Tensor) -> tuple[torch.Tensor, dict[str, float]]:
         """Output the action given the state.
 
         Args:
             state (torch.Tensor): State of the environment.
 
         Returns:
             action: The action of the agent.
@@ -213,15 +213,15 @@
         last_mean = torch.zeros_like(self._action_sequence_mean)
         last_var = self._action_sequence_var.clone()
         last_mean[:-1] = self._action_sequence_mean[1:].clone()
         last_mean[-1] = self._action_sequence_mean[-1].clone()
 
         current_iter = 0
         actions_actor = self._act_from_actor(state)
-        info: dict[str, int | float] = {}
+        info: dict[str, float] = {}
         while current_iter < self._num_iterations and last_var.max() > self._epsilon:
             actions_gauss = self._act_from_last_gaus(last_mean=last_mean, last_var=last_var)
             actions = torch.cat([actions_gauss, actions_actor], dim=1)
             # [horizon, num_sample, action_shape]
             states_repeat, actions_repeat = self._state_action_repeat(state, actions)
             # pylint: disable-next=line-too-long
             # [num_particles * num_samples/num_ensemble, state_shape], [horizon, num_particles * num_samples/num_ensemble, action_shape]
```

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/model_based/rce_pets.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/model_based/rce_pets.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/model_based/safeloop.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/model_based/safeloop.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/__init__.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/off_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/ddpg.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/off_policy/ddpg.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 
 from omnisafe.adapter import OffPolicyAdapter
 from omnisafe.algorithms import registry
 from omnisafe.algorithms.base_algo import BaseAlgo
 from omnisafe.common.buffer import VectorOffPolicyBuffer
 from omnisafe.common.logger import Logger
 from omnisafe.models.actor_critic.constraint_actor_q_critic import ConstraintActorQCritic
-from omnisafe.utils import distributed
 
 
 @registry.register
 # pylint: disable-next=too-many-instance-attributes,too-few-public-methods
 class DDPG(BaseAlgo):
     """The Deep Deterministic Policy Gradient (DDPG) algorithm.
 
@@ -66,28 +65,29 @@
         """
         self._env: OffPolicyAdapter = OffPolicyAdapter(
             self._env_id,
             self._cfgs.train_cfgs.vector_env_nums,
             self._seed,
             self._cfgs,
         )
-        assert (self._cfgs.algo_cfgs.steps_per_epoch) % (
-            distributed.world_size() * self._cfgs.train_cfgs.vector_env_nums
-        ) == 0, 'The number of steps per epoch is not divisible by the number of environments.'
+        assert (
+            self._cfgs.algo_cfgs.steps_per_epoch % self._cfgs.train_cfgs.vector_env_nums == 0
+        ), 'The number of steps per epoch is not divisible by the number of environments.'
 
         assert (
             int(self._cfgs.train_cfgs.total_steps) % self._cfgs.algo_cfgs.steps_per_epoch == 0
         ), 'The total number of steps is not divisible by the number of steps per epoch.'
         self._epochs: int = int(
             self._cfgs.train_cfgs.total_steps // self._cfgs.algo_cfgs.steps_per_epoch,
         )
         self._epoch: int = 0
-        self._steps_per_epoch: int = self._cfgs.algo_cfgs.steps_per_epoch // (
-            distributed.world_size() * self._cfgs.train_cfgs.vector_env_nums
+        self._steps_per_epoch: int = (
+            self._cfgs.algo_cfgs.steps_per_epoch // self._cfgs.train_cfgs.vector_env_nums
         )
+
         self._update_cycle: int = self._cfgs.algo_cfgs.update_cycle
         assert (
             self._steps_per_epoch % self._update_cycle == 0
         ), 'The number of steps per epoch is not divisible by the number of steps per sample.'
         self._samples_per_epoch: int = self._steps_per_epoch // self._update_cycle
         self._update_count: int = 0
 
@@ -196,17 +196,18 @@
         self._logger.setup_torch_saver(what_to_save)
         self._logger.torch_save()
 
         self._logger.register_key('Metrics/EpRet', window_length=50)
         self._logger.register_key('Metrics/EpCost', window_length=50)
         self._logger.register_key('Metrics/EpLen', window_length=50)
 
-        self._logger.register_key('Metrics/TestEpRet', window_length=50)
-        self._logger.register_key('Metrics/TestEpCost', window_length=50)
-        self._logger.register_key('Metrics/TestEpLen', window_length=50)
+        if self._cfgs.train_cfgs.eval_episodes > 0:
+            self._logger.register_key('Metrics/TestEpRet', window_length=50)
+            self._logger.register_key('Metrics/TestEpCost', window_length=50)
+            self._logger.register_key('Metrics/TestEpLen', window_length=50)
 
         self._logger.register_key('Train/Epoch')
         self._logger.register_key('Train/LR')
 
         self._logger.register_key('TotalEnvSteps')
 
         # log information about actor
@@ -223,14 +224,17 @@
 
         self._logger.register_key('Time/Total')
         self._logger.register_key('Time/Rollout')
         self._logger.register_key('Time/Update')
         self._logger.register_key('Time/Evaluate')
         self._logger.register_key('Time/Epoch')
         self._logger.register_key('Time/FPS')
+        # register environment specific keys
+        for env_spec_key in self._env.env_spec_keys:
+            self.logger.register_key(env_spec_key)
 
     def learn(self) -> tuple[float, float, float]:
         """This is main function for algorithm update.
 
         It is divided into the following steps:
 
         - :meth:`rollout`: collect interactive data from environment.
@@ -279,15 +283,15 @@
                 # if we haven't updated the network, log 0 for the loss
                 else:
                     self._log_when_not_update()
                 update_time += time.time() - update_start
 
             eval_start = time.time()
             self._env.eval_policy(
-                episode=1,
+                episode=self._cfgs.train_cfgs.eval_episodes,
                 agent=self._actor_critic,
                 logger=self._logger,
             )
             eval_time = time.time() - eval_start
 
             self._logger.store({'Time/Update': update_time})
             self._logger.store({'Time/Rollout': rollout_time})
@@ -316,14 +320,15 @@
             if (epoch + 1) % self._cfgs.logger_cfgs.save_model_freq == 0:
                 self._logger.torch_save()
 
         ep_ret = self._logger.get_stats('Metrics/EpRet')[0]
         ep_cost = self._logger.get_stats('Metrics/EpCost')[0]
         ep_len = self._logger.get_stats('Metrics/EpLen')[0]
         self._logger.close()
+        self._env.close()
 
         return ep_ret, ep_cost, ep_len
 
     def _update(self) -> None:
         """Update actor, critic.
 
         -  Get the ``data`` from buffer
@@ -416,15 +421,14 @@
         loss.backward()
 
         if self._cfgs.algo_cfgs.max_grad_norm:
             clip_grad_norm_(
                 self._actor_critic.reward_critic.parameters(),
                 self._cfgs.algo_cfgs.max_grad_norm,
             )
-        distributed.avg_grads(self._actor_critic.reward_critic)
         self._actor_critic.reward_critic_optimizer.step()
 
     def _update_cost_critic(
         self,
         obs: torch.Tensor,
         action: torch.Tensor,
         cost: torch.Tensor,
@@ -459,15 +463,14 @@
         loss.backward()
 
         if self._cfgs.algo_cfgs.max_grad_norm:
             clip_grad_norm_(
                 self._actor_critic.cost_critic.parameters(),
                 self._cfgs.algo_cfgs.max_grad_norm,
             )
-        distributed.avg_grads(self._actor_critic.cost_critic)
         self._actor_critic.cost_critic_optimizer.step()
 
         self._logger.store(
             {
                 'Loss/Loss_cost_critic': loss.mean().item(),
                 'Value/cost_critic': q_value_c.mean().item(),
             },
```

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/ddpg_lag.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/off_policy/ddpg_lag.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/ddpg_pid.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/off_policy/ddpg_pid.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/sac.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/off_policy/sac.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 import torch
 from torch import nn, optim
 from torch.nn.utils.clip_grad import clip_grad_norm_
 
 from omnisafe.algorithms import registry
 from omnisafe.algorithms.off_policy.ddpg import DDPG
 from omnisafe.models.actor_critic.constraint_actor_q_critic import ConstraintActorQCritic
-from omnisafe.utils import distributed
 
 
 @registry.register
 # pylint: disable-next=too-many-instance-attributes,too-few-public-methods
 class SAC(DDPG):
     """The Soft Actor-Critic (SAC) algorithm.
 
@@ -138,15 +137,14 @@
         loss.backward()
 
         if self._cfgs.algo_cfgs.max_grad_norm:
             clip_grad_norm_(
                 self._actor_critic.reward_critic.parameters(),
                 self._cfgs.algo_cfgs.max_grad_norm,
             )
-        distributed.avg_grads(self._actor_critic.reward_critic)
         self._actor_critic.reward_critic_optimizer.step()
         self._logger.store(
             {
                 'Loss/Loss_reward_critic': loss.mean().item(),
                 'Value/reward_critic': q1_value_r.mean().item(),
             },
         )
```

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/sac_lag.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/off_policy/sac_lag.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/sac_pid.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/off_policy/sac_pid.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/td3.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/off_policy/td3.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 import torch
 from torch import nn
 from torch.nn.utils.clip_grad import clip_grad_norm_
 
 from omnisafe.algorithms import registry
 from omnisafe.algorithms.off_policy.ddpg import DDPG
 from omnisafe.models.actor_critic.constraint_actor_q_critic import ConstraintActorQCritic
-from omnisafe.utils import distributed
 
 
 @registry.register
 # pylint: disable-next=too-many-instance-attributes,too-few-public-methods
 class TD3(DDPG):
     """The Twin Delayed DDPG (TD3) algorithm.
 
@@ -104,15 +103,14 @@
         loss.backward()
 
         if self._cfgs.algo_cfgs.max_grad_norm:
             clip_grad_norm_(
                 self._actor_critic.reward_critic.parameters(),
                 self._cfgs.algo_cfgs.max_grad_norm,
             )
-        distributed.avg_grads(self._actor_critic.reward_critic)
         self._actor_critic.reward_critic_optimizer.step()
         self._logger.store(
             {
                 'Loss/Loss_reward_critic': loss.mean().item(),
                 'Value/reward_critic': q1_value_r.mean().item(),
             },
         )
```

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/td3_lag.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/off_policy/td3_lag.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/off_policy/td3_pid.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/off_policy/td3_pid.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/offline/__init__.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/offline/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/offline/base.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/offline/base.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/offline/bcq.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/offline/bcq.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/offline/bcq_lag.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/offline/bcq_lag.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/offline/c_crr.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/offline/c_crr.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/offline/coptidice.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/offline/coptidice.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/offline/crr.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/offline/crr.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/offline/vae_bc.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/offline/vae_bc.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 from typing import Any, Dict, Tuple
 
 import torch
 from torch import optim
 
 from omnisafe.algorithms import registry
 from omnisafe.algorithms.offline.base import BaseOffline
+from omnisafe.models.actor import VAE
 from omnisafe.models.actor.actor_builder import ActorBuilder
-from omnisafe.models.actor.vae_actor import VAE
 
 
 @registry.register
 class VAEBC(BaseOffline):
     """Behavior Cloning with Variational Autoencoder.
 
     References:
```

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/__init__.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/base/__init__.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/base/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/base/natural_pg.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/base/natural_pg.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/base/policy_gradient.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/base/policy_gradient.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,14 +218,18 @@
 
         self._logger.register_key('Time/Total')
         self._logger.register_key('Time/Rollout')
         self._logger.register_key('Time/Update')
         self._logger.register_key('Time/Epoch')
         self._logger.register_key('Time/FPS')
 
+        # register environment specific keys
+        for env_spec_key in self._env.env_spec_keys:
+            self.logger.register_key(env_spec_key)
+
     def learn(self) -> tuple[float, float, float]:
         """This is main function for algorithm update.
 
         It is divided into the following steps:
 
         - :meth:`rollout`: collect interactive data from environment.
         - :meth:`update`: perform actor/critic updates.
@@ -264,30 +268,35 @@
             self._logger.store(
                 {
                     'TotalEnvSteps': (epoch + 1) * self._cfgs.algo_cfgs.steps_per_epoch,
                     'Time/FPS': self._cfgs.algo_cfgs.steps_per_epoch / (time.time() - epoch_time),
                     'Time/Total': (time.time() - start_time),
                     'Time/Epoch': (time.time() - epoch_time),
                     'Train/Epoch': epoch,
-                    'Train/LR': 0.0
-                    if self._cfgs.model_cfgs.actor.lr is None
-                    else self._actor_critic.actor_scheduler.get_last_lr()[0],
+                    'Train/LR': (
+                        0.0
+                        if self._cfgs.model_cfgs.actor.lr is None
+                        else self._actor_critic.actor_scheduler.get_last_lr()[0]
+                    ),
                 },
             )
 
             self._logger.dump_tabular()
 
             # save model to disk
-            if (epoch + 1) % self._cfgs.logger_cfgs.save_model_freq == 0:
+            if (epoch + 1) % self._cfgs.logger_cfgs.save_model_freq == 0 or (
+                epoch + 1
+            ) == self._cfgs.train_cfgs.epochs:
                 self._logger.torch_save()
 
         ep_ret = self._logger.get_stats('Metrics/EpRet')[0]
         ep_cost = self._logger.get_stats('Metrics/EpCost')[0]
         ep_len = self._logger.get_stats('Metrics/EpLen')[0]
         self._logger.close()
+        self._env.close()
 
         return ep_ret, ep_cost, ep_len
 
     def _update(self) -> None:
         """Update actor, critic.
 
         -  Get the ``data`` from buffer
@@ -341,15 +350,15 @@
         dataloader = DataLoader(
             dataset=TensorDataset(obs, act, logp, target_value_r, target_value_c, adv_r, adv_c),
             batch_size=self._cfgs.algo_cfgs.batch_size,
             shuffle=True,
         )
 
         update_counts = 0
-        final_kl = torch.ones_like(old_distribution.loc)
+        final_kl = 0.0
 
         for i in track(range(self._cfgs.algo_cfgs.update_iters), description='Updating...'):
             for (
                 obs,
                 act,
                 logp,
                 target_value_r,
@@ -364,22 +373,21 @@
 
             new_distribution = self._actor_critic.actor(original_obs)
 
             kl = (
                 torch.distributions.kl.kl_divergence(old_distribution, new_distribution)
                 .sum(-1, keepdim=True)
                 .mean()
-                .item()
             )
             kl = distributed.dist_avg(kl)
 
-            final_kl = kl
+            final_kl = kl.item()
             update_counts += 1
 
-            if self._cfgs.algo_cfgs.kl_early_stop and kl > self._cfgs.algo_cfgs.target_kl:
+            if self._cfgs.algo_cfgs.kl_early_stop and kl.item() > self._cfgs.algo_cfgs.target_kl:
                 self._logger.log(f'Early stopping at iter {i + 1} due to reaching max kl')
                 break
 
         self._logger.store(
             {
                 'Train/StopIter': update_counts,  # pylint: disable=undefined-loop-variable
                 'Value/Adv': adv_r.mean().item(),
```

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/base/ppo.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/base/ppo.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/base/trpo.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/base/trpo.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         step_direction: torch.Tensor,
         grads: torch.Tensor,
         p_dist: Distribution,
         obs: torch.Tensor,
         act: torch.Tensor,
         logp: torch.Tensor,
         adv: torch.Tensor,
-        loss_before: float,
+        loss_before: torch.Tensor,
         total_steps: int = 15,
         decay: float = 0.8,
     ) -> tuple[torch.Tensor, int]:
         """TRPO performs `line-search <https://en.wikipedia.org/wiki/Line_search>`_ until constraint satisfaction.
 
         .. hint::
             TRPO search around for a satisfied step of policy update to improve loss and reward performance. The search
@@ -106,24 +106,26 @@
             set_param_values_to_model(self._actor_critic.actor, new_theta)
 
             with torch.no_grad():
                 loss = self._loss_pi(obs, act, logp, adv)
                 # compute KL distance between new and old policy
                 q_dist = self._actor_critic.actor(obs)
                 # KL-distance of old p-dist and new q-dist, applied in KLEarlyStopping
-                kl = torch.distributions.kl.kl_divergence(p_dist, q_dist).mean().item()
+                kl = torch.distributions.kl.kl_divergence(p_dist, q_dist).mean()
                 kl = distributed.dist_avg(kl).mean().item()
             # real loss improve: old policy loss - new policy loss
-            loss_improve = loss_before - loss.item()
+            loss_improve = loss_before - loss
             # average processes.... multi-processing style like: mpi_tools.mpi_avg(xxx)
             loss_improve = distributed.dist_avg(loss_improve)
-            self._logger.log(f'Expected Improvement: {expected_improve} Actual: {loss_improve}')
+            self._logger.log(
+                f'Expected Improvement: {expected_improve} Actual: {loss_improve.item()}',
+            )
             if not torch.isfinite(loss):
                 self._logger.log('WARNING: loss_pi not finite')
-            elif loss_improve < 0:
+            elif loss_improve.item() < 0:
                 self._logger.log('INFO: did not improve improve <0')
             elif kl > self._cfgs.algo_cfgs.target_kl:
                 self._logger.log('INFO: violated KL constraint.')
             else:
                 # step only if surrogate is improved and when within trust reg.
                 acceptance_step = step + 1
                 self._logger.log(f'Accept step at i={acceptance_step}')
@@ -172,15 +174,15 @@
             adv_c (torch.Tensor): The cost advantage tensor.
         """
         self._fvp_obs = obs[:: self._cfgs.algo_cfgs.fvp_sample_freq]
         theta_old = get_flat_params_from(self._actor_critic.actor)
         self._actor_critic.actor.zero_grad()
         adv = self._compute_adv_surrogate(adv_r, adv_c)
         loss = self._loss_pi(obs, act, logp, adv)
-        loss_before = distributed.dist_avg(loss).item()
+        loss_before = distributed.dist_avg(loss)
         p_dist = self._actor_critic.actor(obs)
 
         loss.backward()
         distributed.avg_grads(self._actor_critic.actor)
 
         grads = -get_flat_gradients_from(self._actor_critic.actor)
         x = conjugate_gradients(self._fvp, grads, self._cfgs.algo_cfgs.cg_iters)
```

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/early_terminated/__init__.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/early_terminated/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/early_terminated/ppo_early_terminated.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/early_terminated/ppo_early_terminated.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/early_terminated/trpo_early_terminated.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/early_terminated/trpo_early_terminated.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/first_order/__init__.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/first_order/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/first_order/cup.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/first_order/cup.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,19 +180,18 @@
 
             new_distribution = self._actor_critic.actor(original_obs)
 
             kl = (
                 torch.distributions.kl.kl_divergence(old_distribution, new_distribution)
                 .sum(-1, keepdim=True)
                 .mean()
-                .item()
             )
             kl = distributed.dist_avg(kl)
 
-            if self._cfgs.algo_cfgs.kl_early_stop and kl > self._cfgs.algo_cfgs.target_kl:
+            if self._cfgs.algo_cfgs.kl_early_stop and kl.item() > self._cfgs.algo_cfgs.target_kl:
                 final_steps = i + 1
                 self._logger.log(f'Early stopping at iter {i + 1} due to reaching max kl')
                 break
 
         self._logger.store(
             {
                 'Metrics/LagrangeMultiplier': self._lagrange.lagrangian_multiplier.item(),
```

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/first_order/focops.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/first_order/focops.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,20 +208,19 @@
 
             new_distribution = self._actor_critic.actor(original_obs)
 
             kl = (
                 torch.distributions.kl.kl_divergence(old_distribution, new_distribution)
                 .sum(-1, keepdim=True)
                 .mean()
-                .item()
             )
             kl = distributed.dist_avg(kl)
 
-            self._logger.store({'Train/KL': kl})
-            if self._cfgs.algo_cfgs.kl_early_stop and kl > self._cfgs.algo_cfgs.target_kl:
+            self._logger.store({'Train/KL': kl.item()})
+            if self._cfgs.algo_cfgs.kl_early_stop and kl.item() > self._cfgs.algo_cfgs.target_kl:
                 final_steps = i + 1
                 self._logger.log(f'Early stopping at iter {i + 1} due to reaching max kl')
                 break
 
         self._logger.store(
             {
                 'Train/StopIter': final_steps,
```

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/naive_lagrange/__init__.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/naive_lagrange/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/naive_lagrange/pdo.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/naive_lagrange/pdo.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/naive_lagrange/ppo_lag.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/naive_lagrange/ppo_lag.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/naive_lagrange/rcpo.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/naive_lagrange/rcpo.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/naive_lagrange/trpo_lag.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/naive_lagrange/trpo_lag.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/penalty_function/__init__.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/penalty_function/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/penalty_function/ipo.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/penalty_function/ipo.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/penalty_function/p3o.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/penalty_function/p3o.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/pid_lagrange/__init__.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/pid_lagrange/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/pid_lagrange/cppo_pid.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/pid_lagrange/cppo_pid.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/pid_lagrange/trpo_pid.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/pid_lagrange/trpo_pid.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/primal/__init__.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/primal/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/primal/crpo.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/primal/crpo.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 # limitations under the License.
 # ==============================================================================
 """Implementation of the on-policy CRPO algorithm."""
 
 import torch
 
 from omnisafe.algorithms import registry
-from omnisafe.algorithms.on_policy.base.ppo import PPO
+from omnisafe.algorithms.on_policy.base.trpo import TRPO
 from omnisafe.utils.config import Config
 
 
 @registry.register
-class OnCRPO(PPO):
+class OnCRPO(TRPO):
     """The on-policy CRPO algorithm.
 
     References:
         - Title: CRPO: A New Approach for Safe Reinforcement Learning with Convergence Guarantee.
         - Authors: Tengyu Xu, Yingbin Liang, Guanghui Lan.
         - URL: `CRPO <https://arxiv.org/pdf/2011.05869.pdf>`_.
     """
@@ -67,8 +67,14 @@
             The advantage function chosen from reward and cost.
         """
         Jc = self._logger.get_stats('Metrics/EpCost')[0]
         if Jc <= self._cfgs.algo_cfgs.cost_limit + self._cfgs.algo_cfgs.distance:
             self._rew_update += 1
             return adv_r
         self._cost_update += 1
+        self._logger.store(
+            {
+                'Misc/RewUpdate': self._rew_update,
+                'Misc/CostUpdate': self._cost_update,
+            },
+        )
         return -adv_c
```

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/saute/__init__.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/saute/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/saute/ppo_saute.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/saute/ppo_saute.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/saute/trpo_saute.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/saute/trpo_saute.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/second_order/__init__.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/second_order/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/second_order/cpo.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/second_order/cpo.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,16 +60,16 @@
         grads: torch.Tensor,
         p_dist: torch.distributions.Distribution,
         obs: torch.Tensor,
         act: torch.Tensor,
         logp: torch.Tensor,
         adv_r: torch.Tensor,
         adv_c: torch.Tensor,
-        loss_reward_before: float,
-        loss_cost_before: float,
+        loss_reward_before: torch.Tensor,
+        loss_cost_before: torch.Tensor,
         total_steps: int = 15,
         decay: float = 0.8,
         violation_c: int = 0,
         optim_case: int = 0,
     ) -> tuple[torch.Tensor, int]:
         r"""Use line-search to find the step size that satisfies the constraint.
 
@@ -128,17 +128,17 @@
                     continue
                 # loss of cost of policy cost from real/expected reward
                 loss_cost = self._loss_pi_cost(obs=obs, act=act, logp=logp, adv_c=adv_c)
                 # compute KL distance between new and old policy
                 q_dist = self._actor_critic.actor(obs)
                 kl = torch.distributions.kl.kl_divergence(p_dist, q_dist).mean()
             # compute improvement of reward
-            loss_reward_improve = loss_reward_before - loss_reward.item()
+            loss_reward_improve = loss_reward_before - loss_reward
             # compute difference of cost
-            loss_cost_diff = loss_cost.item() - loss_cost_before
+            loss_cost_diff = loss_cost - loss_cost_before
 
             # average across MPI processes...
             kl = distributed.dist_avg(kl)
             # pi_average of torch_kl above
             loss_reward_improve = distributed.dist_avg(loss_reward_improve)
             loss_cost_diff = distributed.dist_avg(loss_cost_diff)
             self._logger.log(
@@ -363,30 +363,30 @@
             adv_r (torch.Tensor): The reward advantage tensor.
             adv_c (torch.Tensor): The cost advantage tensor.
         """
         self._fvp_obs = obs[:: self._cfgs.algo_cfgs.fvp_sample_freq]
         theta_old = get_flat_params_from(self._actor_critic.actor)
         self._actor_critic.actor.zero_grad()
         loss_reward = self._loss_pi(obs, act, logp, adv_r)
-        loss_reward_before = distributed.dist_avg(loss_reward).item()
+        loss_reward_before = distributed.dist_avg(loss_reward)
         p_dist = self._actor_critic.actor(obs)
 
         loss_reward.backward()
         distributed.avg_grads(self._actor_critic.actor)
 
         grads = -get_flat_gradients_from(self._actor_critic.actor)
         x = conjugate_gradients(self._fvp, grads, self._cfgs.algo_cfgs.cg_iters)
         assert torch.isfinite(x).all(), 'x is not finite'
         xHx = x.dot(self._fvp(x))
         assert xHx.item() >= 0, 'xHx is negative'
         alpha = torch.sqrt(2 * self._cfgs.algo_cfgs.target_kl / (xHx + 1e-8))
 
         self._actor_critic.zero_grad()
         loss_cost = self._loss_pi_cost(obs, act, logp, adv_c)
-        loss_cost_before = distributed.dist_avg(loss_cost).item()
+        loss_cost_before = distributed.dist_avg(loss_cost)
 
         loss_cost.backward()
         distributed.avg_grads(self._actor_critic.actor)
 
         b_grads = get_flat_gradients_from(self._actor_critic.actor)
         ep_costs = self._logger.get_stats('Metrics/EpCost')[0] - self._cfgs.algo_cfgs.cost_limit
```

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/second_order/pcpo.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/second_order/pcpo.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             adv_c (torch.Tensor): The cost advantage tensor.
         """
         # pylint: disable=invalid-name
         self._fvp_obs = obs[:: self._cfgs.algo_cfgs.fvp_sample_freq]
         theta_old = get_flat_params_from(self._actor_critic.actor)
         self._actor_critic.actor.zero_grad()
         loss_reward = self._loss_pi(obs, act, logp, adv_r)
-        loss_reward_before = distributed.dist_avg(loss_reward).item()
+        loss_reward_before = distributed.dist_avg(loss_reward)
         p_dist = self._actor_critic.actor(obs)
 
         loss_reward.backward()
         distributed.avg_grads(self._actor_critic.actor)
 
         grads = -get_flat_gradients_from(self._actor_critic.actor)
         x = conjugate_gradients(self._fvp, grads, self._cfgs.algo_cfgs.cg_iters)
@@ -79,15 +79,15 @@
         xHx = x.dot(self._fvp(x))
         H_inv_g = self._fvp(x)
         assert xHx.item() >= 0, 'xHx is negative'
         alpha = torch.sqrt(2 * self._cfgs.algo_cfgs.target_kl / (xHx + 1e-8))
 
         self._actor_critic.zero_grad()
         loss_cost = self._loss_pi_cost(obs, act, logp, adv_c)
-        loss_cost_before = distributed.dist_avg(loss_cost).item()
+        loss_cost_before = distributed.dist_avg(loss_cost)
 
         loss_cost.backward()
         distributed.avg_grads(self._actor_critic.actor)
 
         b_grads = get_flat_gradients_from(self._actor_critic.actor)
         ep_costs = self._logger.get_stats('Metrics/EpCost')[0] - self._cfgs.algo_cfgs.cost_limit
 
@@ -138,15 +138,15 @@
                 'Misc/FinalStepNorm': step_direction.norm().mean().item(),
                 'Misc/xHx': xHx.mean().item(),
                 'Misc/H_inv_g': x.norm().item(),  # H^-1 g
                 'Misc/gradient_norm': torch.norm(grads).mean().item(),
                 'Misc/cost_gradient_norm': torch.norm(b_grads).mean().item(),
                 'Misc/Lambda_star': 1.0,
                 'Misc/Nu_star': 1.0,
-                'Misc/OptimCase': int(1),
+                'Misc/OptimCase': 1,
                 'Misc/A': 1.0,
                 'Misc/B': 1.0,
                 'Misc/q': q.item(),
                 'Misc/r': r.item(),
                 'Misc/s': s.item(),
             },
         )
```

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/simmer/__init__.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/simmer/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/simmer/ppo_simmer_pid.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/simmer/ppo_simmer_pid.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/on_policy/simmer/trpo_simmer_pid.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/on_policy/simmer/trpo_simmer_pid.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/algorithms/registry.py` & `omnisafe-0.5.1b0/omnisafe/algorithms/registry.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/common/__init__.py` & `omnisafe-0.5.1b0/omnisafe/common/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/common/buffer/__init__.py` & `omnisafe-0.5.1b0/omnisafe/common/buffer/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/common/buffer/base.py` & `omnisafe-0.5.1b0/omnisafe/common/buffer/base.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/common/buffer/offpolicy_buffer.py` & `omnisafe-0.5.1b0/omnisafe/common/buffer/offpolicy_buffer.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/common/buffer/onpolicy_buffer.py` & `omnisafe-0.5.1b0/omnisafe/common/buffer/onpolicy_buffer.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/common/buffer/vector_offpolicy_buffer.py` & `omnisafe-0.5.1b0/omnisafe/common/buffer/vector_offpolicy_buffer.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/common/buffer/vector_onpolicy_buffer.py` & `omnisafe-0.5.1b0/omnisafe/common/buffer/vector_onpolicy_buffer.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/common/experiment_grid.py` & `omnisafe-0.5.1b0/omnisafe/common/experiment_grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 """Implementation of the Experiment Grid."""
 
 from __future__ import annotations
 
 import json
+import multiprocessing as mp
 import os
 import string
 from concurrent.futures import ProcessPoolExecutor as Pool
 from copy import deepcopy
 from typing import Any, Callable
 
 import numpy as np
@@ -436,15 +437,15 @@
         line = '=' * self.div_line_width
 
         self._console.print('\nPreparing to run the following experiments...', style='bold green')
         joined_var_names = '\n'.join(var_names)
         announcement = f'\n{joined_var_names}\n\n{line}'
         print(announcement)
 
-        pool = Pool(max_workers=num_pool)
+        pool = Pool(max_workers=num_pool, mp_context=mp.get_context('spawn'))
         # run the variants.
         results = []
         exp_names = []
 
         for idx, var in enumerate(variants):
             self.check_variant_vaild(var)
             print('current_config', var)
```

### Comparing `omnisafe-0.5.0b0/omnisafe/common/lagrange.py` & `omnisafe-0.5.1b0/omnisafe/common/lagrange.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/common/logger.py` & `omnisafe-0.5.1b0/omnisafe/common/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,19 +113,19 @@
             atexit.register(self._output_file.close)
             self.log(f'Logging data to {self._output_file.name}', 'cyan', bold=True)
             self._csv_writer = csv.writer(self._output_file)
 
         self._epoch: int = 0
         self._first_row: bool = True
         self._what_to_save: dict[str, Any] | None = None
-        self._data: dict[str, deque[int | float] | list[int | float]] = {}
+        self._data: dict[str, deque[float] | list[float]] = {}
         self._headers_windows: dict[str, int | None] = {}
         self._headers_minmax: dict[str, bool] = {}
         self._headers_delta: dict[str, bool] = {}
-        self._current_row: dict[str, int | float] = {}
+        self._current_row: dict[str, float] = {}
 
         if config is not None:
             self.save_config(config)
             self._config: Config = config
 
         self._use_tensorboard: bool = use_tensorboard
         self._use_wandb: bool = use_wandb
@@ -253,15 +253,15 @@
     ) -> None:
         """Store the data to the logger.
 
         .. note ::
             The data stored in ``data`` will be updated by ``kwargs``.
 
         Args:
-            data (dict[str, int | float | np.ndarray | torch.Tensor] or None, optional): The data to
+            data (dict[str, float | np.ndarray | torch.Tensor] or None, optional): The data to
                 be stored. Defaults to None.
 
         Keyword Args:
             kwargs (int, float, np.ndarray, or torch.Tensor): The data to be stored.
         """
         if data is not None:
             kwargs.update(data)
@@ -307,15 +307,15 @@
             if self._use_tensorboard:
                 for key, val in self._current_row.items():
                     self._tensorboard_writer.add_scalar(key, val, global_step=self._epoch)
                 self._tensorboard_writer.flush()
 
             if self._use_wandb:
                 wandb.log(self._current_row, step=self._epoch)
-        self._console.print(table)
+            self._console.print(table)
 
     def _update_current_row(self) -> None:
         """Update the current row.
 
         Update the current row with the data stored in the logger.
         """
         for key in self._data:
@@ -336,15 +336,15 @@
             if self._headers_windows[key] is None:
                 self._data[key] = []
 
     def get_stats(
         self,
         key: str,
         min_and_max: bool = False,
-    ) -> tuple[int | float, ...]:
+    ) -> tuple[float, ...]:
         """Get the statistics of the key.
 
         Args:
             key (str): The key to be registered.
             min_and_max (bool, optional): Whether to record the min and max value of the key.
                 Defaults to False.
 
@@ -354,21 +354,21 @@
         assert key in self._current_row, f'Key {key} has not been registered'
         vals = self._data[key]
         if isinstance(vals, deque):
             vals = list(vals)
 
         if min_and_max:
             mean, std, min_val, max_val = dist_statistics_scalar(
-                torch.tensor(vals),
+                torch.tensor(vals).to(os.getenv('OMNISAFE_DEVICE', 'cpu')),
                 with_min_and_max=True,
             )
             return mean.item(), min_val.mean().item(), max_val.mean().item(), std.item()
 
         mean, std = dist_statistics_scalar(  # pylint: disable=unbalanced-tuple-unpacking
-            torch.tensor(vals),
+            torch.tensor(vals).to(os.getenv('OMNISAFE_DEVICE', 'cpu')),
         )
         return (mean.item(),)
 
     @property
     def current_epoch(self) -> int:
         """Return the current epoch."""
         return self._epoch
```

### Comparing `omnisafe-0.5.0b0/omnisafe/common/normalizer.py` & `omnisafe-0.5.1b0/omnisafe/common/normalizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 from __future__ import annotations
 
 from typing import Any, Mapping
 
 import torch
 import torch.nn as nn
-from torch.nn.modules.module import _IncompatibleKeys
 
 
 class Normalizer(nn.Module):
     """Calculate normalized raw_data from running mean and std.
 
     References:
         - Title: Updating Formulae and a Pairwise Algorithm for Computing Sample Variances
@@ -139,20 +138,21 @@
         self._std = torch.sqrt(self._var)
         self._std = torch.max(self._std, 1e-2 * torch.ones_like(self._std))
 
     def load_state_dict(
         self,
         state_dict: Mapping[str, Any],
         strict: bool = True,
-    ) -> _IncompatibleKeys:
+        assign: bool = False,
+    ) -> Any:
         """Load the state_dict to the normalizer.
 
         Args:
             state_dict (Mapping[str, Any]): The state_dict to be loaded.
             strict (bool, optional): Whether to strictly enforce that the keys in :attr:`state_dict`.
                 Defaults to True.
 
         Returns:
             The loaded normalizer.
         """
         self._first = False
-        return super().load_state_dict(state_dict, strict)
+        return super().load_state_dict(state_dict, strict, assign)
```

### Comparing `omnisafe-0.5.0b0/omnisafe/common/offline/__init__.py` & `omnisafe-0.5.1b0/omnisafe/common/offline/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/common/offline/data_collector.py` & `omnisafe-0.5.1b0/omnisafe/common/offline/data_collector.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/common/offline/dataset.py` & `omnisafe-0.5.1b0/omnisafe/common/offline/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 """Offline dataset for offline algorithms."""
 
 from __future__ import annotations
 
 import hashlib
 import os
 from dataclasses import dataclass
+from typing import ClassVar
 
 import gdown
 import numpy as np
 import torch
 from torch.utils.data import Dataset
 
 from omnisafe.typing import DEVICE_CPU
@@ -36,15 +37,15 @@
     sha256sum: str
     episode_length: int | None = None
 
 
 class OfflineDataset(Dataset):
     """A dataset for offline algorithms."""
 
-    _name_to_metadata: dict[str, OfflineMeta] = {
+    _name_to_metadata: ClassVar[dict[str, OfflineMeta]] = {
         'SafetyPointCircle1-v0-mixed-beta0.5': OfflineMeta(
             url='https://drive.google.com/file/d/17q2-T1o01GNM3rBmLP52kRTojYS1ePTX/view?usp=sharing',
             sha256sum='354a762a4fba372c497a0c84e3405863c192406ff754b18eea51a036f47cd5ba',
             episode_length=500,
         ),
         'SafetyPointCircle1-v0-mixed-beta0.25': OfflineMeta(
             url='https://drive.google.com/file/d/1KqDfQ-oxgT4xjM0wu-g-DFWrltSk96kw/view?usp=sharing',
```

### Comparing `omnisafe-0.5.0b0/omnisafe/common/pid_lagrange.py` & `omnisafe-0.5.1b0/omnisafe/common/pid_lagrange.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         diff_norm (bool): Whether to use the diff norm.
         penalty_max (int): The maximum penalty.
         lagrangian_multiplier_init (float): The initial value of the lagrangian multiplier.
         cost_limit (float): The cost limit.
 
     References:
         - Title: Responsive Safety in Reinforcement Learning by PID Lagrangian Methods
-        - Authors: Joshua Achiam, David Held, Aviv Tamar, Pieter Abbeel.
+        - Authors: Adam Stooke, Joshua Achiam, Pieter Abbeel.
         - URL: `PID Lagrange <https://arxiv.org/abs/2007.03964>`_
     """
 
     # pylint: disable-next=too-many-arguments
     def __init__(
         self,
         pid_kp: float,
```

### Comparing `omnisafe-0.5.0b0/omnisafe/common/simmer_agent.py` & `omnisafe-0.5.1b0/omnisafe/common/simmer_agent.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/common/statistics_tools.py` & `omnisafe-0.5.1b0/omnisafe/common/statistics_tools.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/model-based/CAPPETS.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/model-based/CAPPETS.yaml`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/model-based/CCEPETS.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/model-based/CCEPETS.yaml`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/model-based/LOOP.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/model-based/LOOP.yaml`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/model-based/PETS.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/model-based/PETS.yaml`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/model-based/RCEPETS.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/model-based/RCEPETS.yaml`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/model-based/SafeLOOP.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/model-based/SafeLOOP.yaml`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/off-policy/DDPG.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/off-policy/DDPG.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     torch_threads: 16
     # number of vectorized environments
     vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
     total_steps: 1000000
+    # number of evaluate episodes
+    eval_episodes: 1
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
     steps_per_epoch: 2000
     # number of steps per sample
     update_cycle: 1
     # number of iterations to update the policy
```

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/off-policy/DDPGLag.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/off-policy/DDPGLag.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     torch_threads: 16
     # number of vectorized environments
     vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
     total_steps: 1000000
+    # number of evaluate episodes
+    eval_episodes: 1
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
     steps_per_epoch: 2000
     # number of steps per sample
     update_cycle: 1
     # number of iterations to update the policy
```

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/off-policy/DDPGPID.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/off-policy/DDPGPID.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     torch_threads: 16
     # number of vectorized environments
     vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
     total_steps: 1000000
+    # number of evaluate episodes
+    eval_episodes: 1
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
     steps_per_epoch: 2000
     # number of steps per sample
     update_cycle: 1
     # number of iterations to update the policy
```

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/off-policy/SAC.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/off-policy/SAC.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     torch_threads: 16
     # number of vectorized environments
     vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
     total_steps: 1000000
+    # number of evaluate episodes
+    eval_episodes: 1
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
     steps_per_epoch: 2000
     # number of steps per sample
     update_cycle: 1
     # number of iterations to update the policy
```

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/off-policy/SACLag.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/off-policy/SACLag.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     torch_threads: 16
     # number of vectorized environments
     vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
     total_steps: 1000000
+    # number of evaluate episodes
+    eval_episodes: 1
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
     steps_per_epoch: 2000
     # number of steps per sample
     update_cycle: 1
     # number of iterations to update the policy
```

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/off-policy/SACPID.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/off-policy/SACPID.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     torch_threads: 16
     # number of vectorized environments
     vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
     total_steps: 1000000
+    # number of evaluate episodes
+    eval_episodes: 1
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
     steps_per_epoch: 2000
     # number of steps per sample
     update_cycle: 1
     # number of iterations to update the policy
```

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/off-policy/TD3.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/off-policy/TD3.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     torch_threads: 16
     # number of vectorized environments
     vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
     total_steps: 1000000
+    # number of evaluate episodes
+    eval_episodes: 1
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
     steps_per_epoch: 2000
     # number of steps per sample
     update_cycle: 1
     # number of iterations to update the policy
```

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/off-policy/TD3Lag.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/off-policy/TD3Lag.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     torch_threads: 16
     # number of vectorized environments
     vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
     total_steps: 1000000
+    # number of evaluate episodes
+    eval_episodes: 1
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
     steps_per_epoch: 2000
     # number of steps per sample
     update_cycle: 1
     # number of iterations to update the policy
```

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/off-policy/TD3PID.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/off-policy/TD3PID.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     torch_threads: 16
     # number of vectorized environments
     vector_env_nums: 1
     # number of parallel agent, similar to a3c
     parallel: 1
     # total number of steps to train
     total_steps: 1000000
+    # number of evaluate episodes
+    eval_episodes: 1
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
     steps_per_epoch: 2000
     # number of steps per sample
     update_cycle: 1
     # number of iterations to update the policy
```

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/offline/BCQ.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/offline/BCQ.yaml`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/offline/BCQLag.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/offline/BCQLag.yaml`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/offline/CCRR.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/offline/CCRR.yaml`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/offline/COptiDICE.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/offline/COptiDICE.yaml`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/offline/CRR.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/offline/CRR.yaml`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/offline/VAEBC.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/offline/VAEBC.yaml`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/on-policy/CPO.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/on-policy/CPO.yaml`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/on-policy/CPPOPID.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/on-policy/CPPOPID.yaml`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/on-policy/CUP.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/on-policy/CUP.yaml`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/on-policy/FOCOPS.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/on-policy/FOCOPS.yaml`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/on-policy/IPO.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/on-policy/IPO.yaml`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/on-policy/NaturalPG.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/on-policy/NaturalPG.yaml`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/on-policy/OnCRPO.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/on-policy/TRPO.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -29,29 +29,29 @@
     # total number of steps to train
     total_steps: 10000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
     steps_per_epoch: 20000
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
@@ -60,30 +60,32 @@
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
     use_cost: False
-    # the cost limit
-    cost_limit: 25.0
-    # the tolerance of cost limit
-    distance: 2.0
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
@@ -97,28 +99,28 @@
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

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/on-policy/P3O.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/on-policy/P3O.yaml`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/on-policy/PCPO.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/on-policy/PCPO.yaml`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/on-policy/PDO.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/on-policy/PDO.yaml`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/on-policy/PPO.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/on-policy/PPO.yaml`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/on-policy/PPOEarlyTerminated.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/on-policy/PPOEarlyTerminated.yaml`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/on-policy/PPOLag.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/on-policy/PPOLag.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -124,7 +124,9 @@
     cost_limit: 25.0
     # Initial value of lagrangian multiplier
     lagrangian_multiplier_init: 0.001
     # Learning rate of lagrangian multiplier
     lambda_lr: 0.035
     # Type of lagrangian optimizer
     lambda_optimizer: "Adam"
+  # environment specific configurations
+  env_cfgs: {}
```

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/on-policy/PPOSaute.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/on-policy/PolicyGradient.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     # total number of steps to train
     total_steps: 10000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
     steps_per_epoch: 20000
     # number of iterations to update the policy
-    update_iters: 40
+    update_iters: 10
     # batch size for each iteration
     batch_size: 64
     # target kl divergence
     target_kl: 0.02
     # entropy coefficient
     entropy_coef: 0.0
     # normalize reward
@@ -60,34 +60,24 @@
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
     use_cost: False
-    # The safety budget, equal to the cost limit
-    safety_budget: 25.0
-    # The saute gamma
-    saute_gamma: 0.999
-    # The max length of the episode
-    max_ep_len: 1000
-    # The reward when the agent is unsafe
-    unsafe_reward: -1.0
   # logger configurations
   logger_cfgs:
     # use wandb for logging
     use_wandb: False
     # wandb project name
     wandb_project: omnisafe
     # use tensorboard for logging
```

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/on-policy/PPOSimmerPID.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/on-policy/RCPO.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -29,29 +29,29 @@
     # total number of steps to train
     total_steps: 10000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
     steps_per_epoch: 20000
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
@@ -60,36 +60,32 @@
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
-    use_cost: False
-    # The safety budget, equal to the cost limit
-    safety_budget: 25.0
-    # the upper bound of safety budget
-    upper_budget: 25.0
-    # The saute gamma
-    saute_gamma: 0.999
-    # The max length of the episode
-    max_ep_len: 1000
-    # The reward when the agent is unsafe
-    unsafe_reward: -1.0
+    use_cost: True
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
@@ -103,38 +99,38 @@
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
-  # controller configurations
-  control_cfgs:
-    # The Kp of PID controller
-    kp: 1.0
-    # The Ki of PID controller
-    ki: 0.001
-    # The Kd of PID controller
-    kd: 0.01
-    # The polyak coefficient of the target
-    polyak: 0.995
+      lr: 0.001
+  # lagrangian configurations
+  lagrange_cfgs:
+    # Tolerance of constraint violation
+    cost_limit: 25.0
+    # Initial value of lagrangian multiplier
+    lagrangian_multiplier_init: 0.001
+    # Learning rate of lagrangian multiplier
+    lambda_lr: 0.035
+    # Type of lagrangian optimizer
+    lambda_optimizer: "Adam"
```

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/on-policy/PolicyGradient.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/on-policy/TRPOLag.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -31,27 +31,27 @@
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
     steps_per_epoch: 20000
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
@@ -69,15 +69,23 @@
     # standardize reward advantage
     standardized_rew_adv: True
     # standardize cost advantage
     standardized_cost_adv: True
     # penalty coefficient
     penalty_coef: 0.0
     # use cost
-    use_cost: False
+    use_cost: True
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
@@ -91,28 +99,38 @@
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
+  lagrange_cfgs:
+    # Tolerance of constraint violation
+    cost_limit: 25.0
+    # Initial value of lagrangian multiplier
+    lagrangian_multiplier_init: 0.001
+    # Learning rate of lagrangian multiplier
+    lambda_lr: 0.035
+    # Type of lagrangian optimizer
+    lambda_optimizer: "Adam"
```

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/on-policy/RCPO.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/on-policy/TRPOPID.yaml`

 * *Files 13% similar despite different names*

```diff
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
@@ -122,15 +124,29 @@
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # learning rate
       lr: 0.001
   # lagrangian configurations
   lagrange_cfgs:
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
     # Tolerance of constraint violation
     cost_limit: 25.0
+    # The max penalty coefficient
+    penalty_max: 100.0
     # Initial value of lagrangian multiplier
     lagrangian_multiplier_init: 0.001
-    # Learning rate of lagrangian multiplier
-    lambda_lr: 0.035
-    # Type of lagrangian optimizer
-    lambda_optimizer: "Adam"
```

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/on-policy/TRPO.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/on-policy/TRPOEarlyTerminated.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -78,14 +78,16 @@
     cg_damping: 0.1
     # Number of conjugate gradient iterations
     cg_iters: 15
     # Subsampled observation
     fvp_obs: None
     # The sub-sampling rate of the observation
     fvp_sample_freq: 1
+    # Tolerance of constraint violation
+    cost_limit: 25.0
   # logger configurations
   logger_cfgs:
     # use wandb for logging
     use_wandb: False
     # wandb project name
     wandb_project: omnisafe
     # use tensorboard for logging
```

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/on-policy/TRPOEarlyTerminated.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/on-policy/OnCRPO.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -69,25 +69,27 @@
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
     fvp_sample_freq: 1
-    # Tolerance of constraint violation
+    # the cost limit
     cost_limit: 25.0
+    # the tolerance of cost limit
+    distance: 2.0
   # logger configurations
   logger_cfgs:
     # use wandb for logging
     use_wandb: False
     # wandb project name
     wandb_project: omnisafe
     # use tensorboard for logging
```

### Comparing `omnisafe-0.5.0b0/omnisafe/configs/on-policy/TRPOSimmerPID.yaml` & `omnisafe-0.5.1b0/omnisafe/configs/on-policy/PPOSimmerPID.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -29,29 +29,29 @@
     # total number of steps to train
     total_steps: 10000000
   # algorithm configurations
   algo_cfgs:
     # number of steps to update the policy
     steps_per_epoch: 20000
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
@@ -60,32 +60,26 @@
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
     use_cost: False
-    # Damping value for conjugate gradient
-    cg_damping: 0.1
-    # Number of conjugate gradient iterations
-    cg_iters: 15
-    # Subsampled observation
-    fvp_obs: None
-    # The sub-sampling rate of the observation
-    fvp_sample_freq: 1
     # The safety budget, equal to the cost limit
     safety_budget: 25.0
     # the upper bound of safety budget
     upper_budget: 25.0
     # The saute gamma
     saute_gamma: 0.999
     # The max length of the episode
@@ -109,38 +103,106 @@
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
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # out_activation: tanh
       # learning rate
-      lr: ~
+      lr: 0.0003
     critic:
       # hidden layer sizes
       hidden_sizes: [64, 64]
       # activation function
       activation: tanh
       # learning rate
-      lr: 0.001
+      lr: 0.0003
   # controller configurations
   control_cfgs:
     # The Kp of PID controller
-    kp: 1.0
+    kp: 0.0005
     # The Ki of PID controller
-    ki: 0.001
+    ki: 0.00001
     # The Kd of PID controller
-    kd: 0.01
+    kd: 0.0
     # The polyak coefficient of the target
     polyak: 0.995
+
+SafetyCarGoal1-v0:
+  # algorithm configurations
+  algo_cfgs:
+    # number of iterations to update the policy
+    update_iters: 80
+    # normalize observation
+    obs_normalize: False
+    # The saute gamma
+    saute_gamma: 0.9999
+    # The reward when the agent is unsafe
+    unsafe_reward: -0.2
+
+SafetyCarGoal2-v0:
+  # algorithm configurations
+  algo_cfgs:
+    # number of iterations to update the policy
+    update_iters: 80
+    # normalize observation
+    obs_normalize: False
+    # The saute gamma
+    saute_gamma: 0.9999
+    # The reward when the agent is unsafe
+    unsafe_reward: -0.2
+
+SafetyPointCircle1-v0:
+  # algorithm configurations
+  algo_cfgs:
+    # number of iterations to update the policy
+    update_iters: 80
+    # The saute gamma
+    saute_gamma: 0.9999
+    # The reward when the agent is unsafe
+    unsafe_reward: -0.2
+
+SafetyPointCircle2-v0:
+  # algorithm configurations
+  algo_cfgs:
+    # number of iterations to update the policy
+    update_iters: 80
+    # The saute gamma
+    saute_gamma: 0.9999
+    # The reward when the agent is unsafe
+    unsafe_reward: -0.2
+
+SafetyPointGoal1-v0:
+  # algorithm configurations
+  algo_cfgs:
+    # number of iterations to update the policy
+    update_iters: 80
+    # normalize observation
+    obs_normalize: False
+    # The saute gamma
+    saute_gamma: 0.9999
+    # The reward when the agent is unsafe
+    unsafe_reward: -0.2
+
+SafetyPointGoal2-v0:
+  # algorithm configurations
+  algo_cfgs:
+    # number of iterations to update the policy
+    update_iters: 80
+    # normalize observation
+    obs_normalize: False
+    # The saute gamma
+    saute_gamma: 0.9999
+    # The reward when the agent is unsafe
+    unsafe_reward: -0.2
```

### Comparing `omnisafe-0.5.0b0/omnisafe/envs/__init__.py` & `omnisafe-0.5.1b0/omnisafe/envs/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,10 +11,11 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Environment API for OmniSafe."""
 
 from omnisafe.envs.core import CMDP, env_register, make, support_envs
+from omnisafe.envs.custom_env import CustomEnv
 from omnisafe.envs.mujoco_env import MujocoEnv
 from omnisafe.envs.safety_gymnasium_env import SafetyGymnasiumEnv
 from omnisafe.envs.safety_gymnasium_modelbased import SafetyGymnasiumModelBased
```

### Comparing `omnisafe-0.5.0b0/omnisafe/envs/core.py` & `omnisafe-0.5.1b0/omnisafe/envs/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # ==============================================================================
 """The core module of the environment."""
 
 from __future__ import annotations
 
 import inspect
 from abc import ABC, abstractmethod
-from typing import Any
+from typing import Any, ClassVar
 
 import torch
 
 from omnisafe.typing import DEVICE_CPU, OmnisafeSpace
 
 
 __all__ = [
@@ -41,24 +41,25 @@
     environment. The environment should inherit from this class and implement the abstract methods.
 
     Attributes:
         need_time_limit_wrapper (bool): Whether the environment need time limit wrapper.
         need_auto_reset_wrapper (bool): Whether the environment need auto reset wrapper.
     """
 
-    _support_envs: list[str]
     _action_space: OmnisafeSpace
     _observation_space: OmnisafeSpace
     _metadata: dict[str, Any]
 
     _num_envs: int
     _time_limit: int | None = None
     need_time_limit_wrapper: bool
     need_auto_reset_wrapper: bool
 
+    _support_envs: ClassVar[list[str]]
+
     @classmethod
     def support_envs(cls) -> list[str]:
         """The supported environments.
 
         Returns:
             The supported environments.
         """
@@ -78,14 +79,19 @@
 
     @property
     def observation_space(self) -> OmnisafeSpace:
         """The observation space of the environment."""
         return self._observation_space
 
     @property
+    def max_episode_steps(self) -> int | None:
+        """The max steps per episode."""
+        return None
+
+    @property
     def metadata(self) -> dict[str, Any]:
         """The metadata of the environment."""
         return self._metadata
 
     @property
     def num_envs(self) -> int:
         """The number of parallel environments."""
@@ -119,19 +125,24 @@
             cost: The amount of cost returned after previous action.
             terminated: Whether the episode has ended.
             truncated: Whether the episode has been truncated due to a time limit.
             info: Some information logged by the environment.
         """
 
     @abstractmethod
-    def reset(self, seed: int | None = None) -> tuple[torch.Tensor, dict[str, Any]]:
+    def reset(
+        self,
+        seed: int | None = None,
+        options: dict[str, Any] | None = None,
+    ) -> tuple[torch.Tensor, dict[str, Any]]:
         """Reset the environment and returns an initial observation.
 
         Args:
-            seed (int or None): Seed for the environment. Defaults to None.
+            seed (int, optional): The random seed. Defaults to None.
+            options (dict[str, Any], optional): The options for the environment. Defaults to None.
 
         Returns:
             observation: The initial observation of the space.
             info: Some information logged by the environment.
         """
 
     @abstractmethod
@@ -139,22 +150,14 @@
         """Set the seed for this env's random number generator(s).
 
         Args:
             seed (int): The seed to use.
         """
 
     @abstractmethod
-    def sample_action(self) -> torch.Tensor:
-        """Sample an action from the action space.
-
-        Returns:
-            The sampled action.
-        """
-
-    @abstractmethod
     def render(self) -> Any:
         """Compute the render frames as specified by :attr:`render_mode` during the initialization of the environment.
 
         Returns:
             The render frames: we recommend to use `np.ndarray`
                 which could construct video by moviepy.
         """
@@ -232,42 +235,40 @@
             cost: The amount of cost returned after previous action.
             terminated: Whether the episode has ended.
             truncated: Whether the episode has been truncated due to a time limit.
             info: Some information logged by the environment.
         """
         return self._env.step(action)
 
-    def reset(self, seed: int | None = None) -> tuple[torch.Tensor, dict[str, Any]]:
+    def reset(
+        self,
+        seed: int | None = None,
+        options: dict[str, Any] | None = None,
+    ) -> tuple[torch.Tensor, dict[str, Any]]:
         """Reset the environment and returns an initial observation.
 
         Args:
-            seed (int or None): Seed for the environment. Defaults to None.
+            seed (int, optional): The random seed. Defaults to None.
+            options (dict[str, Any], optional): The options for the environment. Defaults to None.
+
 
         Returns:
             observation: The initial observation of the space.
             info: Some information logged by the environment.
         """
-        return self._env.reset(seed)
+        return self._env.reset(seed=seed, options=options)
 
     def set_seed(self, seed: int) -> None:
         """Set the seed for this env's random number generator(s).
 
         Args:
             seed (int): The random seed to use.
         """
         self._env.set_seed(seed)
 
-    def sample_action(self) -> torch.Tensor:
-        """Sample an action from the action space.
-
-        Returns:
-            The sampled action.
-        """
-        return self._env.sample_action()
-
     def render(self) -> Any:
         """Compute the render frames as specified by :attr:`render_mode` during the initialization of the environment.
 
         Returns:
             The render frames: we recommend to use `np.ndarray`
                 which could construct video by moviepy.
         """
@@ -337,14 +338,28 @@
 
         Returns:
             The environment class.
         """
         self._register(env_class)
         return env_class
 
+    def unregister(self, env_class: type[CMDP]) -> type[CMDP]:
+        """Remove the environment from the register.
+
+        Args:
+            env_class (type[CMDP]): The environment class.
+        """
+        class_name = env_class.__name__
+        if class_name not in self._class:
+            print(f'{class_name} has not been registered yet')
+        else:
+            self._class.pop(class_name)
+            self._support_envs.pop(class_name)
+        return env_class
+
     def get_class(self, env_id: str, class_name: str | None) -> type[CMDP]:
         """Get the environment class.
 
         Args:
             env_id (str): The environment id.
             class_name (str or None): The environment class name.
 
@@ -372,14 +387,15 @@
         return list({env_id for env_ids in self._support_envs.values() for env_id in env_ids})
 
 
 ENV_REGISTRY = EnvRegister()
 
 env_register = ENV_REGISTRY.register
 support_envs = ENV_REGISTRY.support_envs
+env_unregister = ENV_REGISTRY.unregister
 
 
 def make(env_id: str, class_name: str | None = None, **kwargs: Any) -> CMDP:
     """Create an environment.
 
     Args:
         env_id (str): The environment id.
```

### Comparing `omnisafe-0.5.0b0/omnisafe/envs/mujoco_env.py` & `omnisafe-0.5.1b0/omnisafe/envs/mujoco_env.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Environments in the Safety Gymnasium."""
+
 from __future__ import annotations
 
-from typing import Any
+from typing import Any, ClassVar
 
 import gymnasium
 import numpy as np
 import torch
 
 from omnisafe.envs.core import CMDP, env_register
 from omnisafe.typing import Box
@@ -30,26 +31,26 @@
     """Gymnasium Mujoco environment.
 
     Attributes:
         need_auto_reset_wrapper (bool): Whether to use auto reset wrapper.
         need_time_limit_wrapper (bool): Whether to use time limit wrapper.
     """
 
-    _support_envs = [
+    need_auto_reset_wrapper = True
+
+    need_time_limit_wrapper = False
+    need_action_repeat_wrapper = True
+    _support_envs: ClassVar[list[str]] = [
         'Ant-v4',
         'Hopper-v4',
         'Walker2d-v4',
         'Humanoid-v4',
         'Swimmer-v4',
         'HalfCheetah-v4',
     ]
-    need_auto_reset_wrapper = False
-
-    need_time_limit_wrapper = False
-    need_action_repeat_wrapper = True
 
     def __init__(
         self,
         env_id: str,
         num_envs: int = 1,
         device: str = 'cpu',
         **kwargs: Any,
@@ -137,47 +138,45 @@
                 info['final_observation'],
                 dtype=torch.float32,
                 device=self._device,
             )
 
         return obs, reward, cost, terminated, truncated, info
 
-    def reset(self, seed: int | None = None) -> tuple[torch.Tensor, dict]:
+    @property
+    def max_episode_steps(self) -> int:
+        """The max steps per episode."""
+        return self._env.env.spec.max_episode_steps  # type: ignore
+
+    def reset(
+        self,
+        seed: int | None = None,
+        options: dict[str, Any] | None = None,
+    ) -> tuple[torch.Tensor, dict]:
         """Reset the environment.
 
         Args:
-            seed (int, optional): Seed to reset the environment. Defaults to None.
+            seed (int, optional): The random seed. Defaults to None.
+            options (dict[str, Any], optional): The options for the environment. Defaults to None.
 
         Returns:
             observation: Agent's observation of the current environment.
             info: Auxiliary diagnostic information (helpful for debugging, and sometimes learning).
         """
-        obs, info = self._env.reset(seed=seed)
+        obs, info = self._env.reset(seed=seed, options=options)
         return torch.as_tensor(obs, dtype=torch.float32, device=self._device), info
 
     def set_seed(self, seed: int) -> None:
         """Set the seed for the environment.
 
         Args:
             seed (int): Seed to set.
         """
         self.reset(seed=seed)
 
-    def sample_action(self) -> torch.Tensor:
-        """Sample a random action.
-
-        Returns:
-            A random action.
-        """
-        return torch.as_tensor(
-            self._env.action_space.sample(),
-            dtype=torch.float32,
-            device=self._device,
-        )
-
     def render(self) -> Any:
         """Render the environment.
 
         Returns:
             Rendered environment.
         """
         return self._env.render()
```

### Comparing `omnisafe-0.5.0b0/omnisafe/envs/safety_gymnasium_env.py` & `omnisafe-0.5.1b0/omnisafe/envs/safety_gymnasium_env.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Environments in the Safety-Gymnasium."""
 
 from __future__ import annotations
 
-from typing import Any
+from typing import Any, ClassVar
 
 import numpy as np
 import safety_gymnasium
 import torch
 
 from omnisafe.envs.core import CMDP, env_register
 from omnisafe.typing import DEVICE_CPU, Box
@@ -47,15 +47,16 @@
     Attributes:
         need_auto_reset_wrapper (bool): Whether to use auto reset wrapper.
         need_time_limit_wrapper (bool): Whether to use time limit wrapper.
     """
 
     need_auto_reset_wrapper: bool = False
     need_time_limit_wrapper: bool = False
-    _support_envs: list[str] = [
+
+    _support_envs: ClassVar[list[str]] = [
         'SafetyPointGoal0-v0',
         'SafetyPointGoal1-v0',
         'SafetyPointGoal2-v0',
         'SafetyPointButton0-v0',
         'SafetyPointButton1-v0',
         'SafetyPointButton2-v0',
         'SafetyPointPush0-v0',
@@ -84,14 +85,38 @@
         'SafetyAntButton2-v0',
         'SafetyAntPush0-v0',
         'SafetyAntPush1-v0',
         'SafetyAntPush2-v0',
         'SafetyAntCircle0-v0',
         'SafetyAntCircle1-v0',
         'SafetyAntCircle2-v0',
+        'SafetyDoggoGoal0-v0',
+        'SafetyDoggoGoal1-v0',
+        'SafetyDoggoGoal2-v0',
+        'SafetyDoggoButton0-v0',
+        'SafetyDoggoButton1-v0',
+        'SafetyDoggoButton2-v0',
+        'SafetyDoggoPush0-v0',
+        'SafetyDoggoPush1-v0',
+        'SafetyDoggoPush2-v0',
+        'SafetyDoggoCircle0-v0',
+        'SafetyDoggoCircle1-v0',
+        'SafetyDoggoCircle2-v0',
+        'SafetyRacecarGoal0-v0',
+        'SafetyRacecarGoal1-v0',
+        'SafetyRacecarGoal2-v0',
+        'SafetyRacecarButton0-v0',
+        'SafetyRacecarButton1-v0',
+        'SafetyRacecarButton2-v0',
+        'SafetyRacecarPush0-v0',
+        'SafetyRacecarPush1-v0',
+        'SafetyRacecarPush2-v0',
+        'SafetyRacecarCircle0-v0',
+        'SafetyRacecarCircle1-v0',
+        'SafetyRacecarCircle2-v0',
         'SafetyHalfCheetahVelocity-v1',
         'SafetyHopperVelocity-v1',
         'SafetySwimmerVelocity-v1',
         'SafetyWalker2dVelocity-v1',
         'SafetyAntVelocity-v1',
         'SafetyHumanoidVelocity-v1',
         'SafetyPointRun0-v0',
@@ -105,14 +130,15 @@
         device: torch.device = DEVICE_CPU,
         **kwargs: Any,
     ) -> None:
         """Initialize an instance of :class:`SafetyGymnasiumEnv`."""
         super().__init__(env_id)
         self._num_envs = num_envs
         self._device = torch.device(device)
+
         if num_envs > 1:
             self._env = safety_gymnasium.vector.make(env_id=env_id, num_envs=num_envs, **kwargs)
             assert isinstance(self._env.single_action_space, Box), 'Only support Box action space.'
             assert isinstance(
                 self._env.single_observation_space,
                 Box,
             ), 'Only support Box observation space.'
@@ -179,48 +205,45 @@
                 info['final_observation'],
                 dtype=torch.float32,
                 device=self._device,
             )
 
         return obs, reward, cost, terminated, truncated, info
 
-    def reset(self, seed: int | None = None) -> tuple[torch.Tensor, dict[str, Any]]:
+    def reset(
+        self,
+        seed: int | None = None,
+        options: dict[str, Any] | None = None,
+    ) -> tuple[torch.Tensor, dict[str, Any]]:
         """Reset the environment.
 
         Args:
-            seed (int or None, optional): Seed to reset the environment.
-                Defaults to None.
+            seed (int, optional): The random seed. Defaults to None.
+            options (dict[str, Any], optional): The options for the environment. Defaults to None.
 
         Returns:
             observation: Agent's observation of the current environment.
             info: Some information logged by the environment.
         """
-        obs, info = self._env.reset(seed=seed)
+        obs, info = self._env.reset(seed=seed, options=options)
         return torch.as_tensor(obs, dtype=torch.float32, device=self._device), info
 
+    @property
+    def max_episode_steps(self) -> int:
+        """The max steps per episode."""
+        return self._env.env.spec.max_episode_steps
+
     def set_seed(self, seed: int) -> None:
         """Set the seed for the environment.
 
         Args:
             seed (int): Seed to set.
         """
         self.reset(seed=seed)
 
-    def sample_action(self) -> torch.Tensor:
-        """Sample a random action.
-
-        Returns:
-            A random action.
-        """
-        return torch.as_tensor(
-            self._env.action_space.sample(),
-            dtype=torch.float32,
-            device=self._device,
-        )
-
     def render(self) -> Any:
         """Compute the render frames as specified by :attr:`render_mode` during the initialization of the environment.
 
         Returns:
             The render frames: we recommend to use `np.ndarray`
                 which could construct video by moviepy.
         """
```

### Comparing `omnisafe-0.5.0b0/omnisafe/envs/safety_gymnasium_modelbased.py` & `omnisafe-0.5.1b0/omnisafe/envs/safety_gymnasium_modelbased.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 """World model of the Safety Gymnasium."""
 
 
 from __future__ import annotations
 
-from typing import Any
+from typing import Any, ClassVar
 
 import gymnasium
 import numpy as np
 import safety_gymnasium
 import torch
 
 from omnisafe.envs.core import CMDP, env_register
@@ -34,24 +34,25 @@
 
     Attributes:
         _support_envs (list[str]): List of supported environments.
         need_auto_reset_wrapper (bool): Whether to use auto reset wrapper.
         need_time_limit_wrapper (bool): Whether to use time limit wrapper.
     """
 
-    _support_envs = [
+    need_auto_reset_wrapper = False
+    need_time_limit_wrapper = False
+
+    _support_envs: ClassVar[list[str]] = [
         'SafetyPointGoal0-v0-modelbased',
         'SafetyPointGoal1-v0-modelbased',
         'SafetyCarGoal0-v0-modelbased',
         'SafetyCarGoal1-v0-modelbased',
         'SafetyAntGoal0-v0-modelbased',
         'SafetyAntGoal1-v0-modelbased',
     ]
-    need_auto_reset_wrapper = False
-    need_time_limit_wrapper = False
 
     def __init__(
         self,
         env_id: str,
         num_envs: int = 1,
         device: str = 'cpu',
         use_lidar: bool = False,
@@ -70,14 +71,15 @@
                 Defaults to ``rgb_array``.
             camera_name (str, optional): The camera name.
             camera_id (int, optional): The camera id.
             width (int, optional): The width of the rendered image. Defaults to 256.
             height (int, optional): The height of the rendered image. Defaults to 256.
         """
         super().__init__(env_id)
+
         self._use_lidar = use_lidar
         if num_envs == 1:
             self._env = safety_gymnasium.make(
                 id=env_id.replace('-modelbased', ''),
                 autoreset=False,
                 **kwargs,
             )
@@ -217,18 +219,17 @@
         hazards_lidar_vec = self._obs_lidar_pseudo(robot_matrix, robot_pos, self.hazards_position)
 
         goal_lidar_vec = self._obs_lidar_pseudo(robot_matrix, robot_pos, [self.goal_position])
         base_state_vec = obs[self.key_to_slice['base_state']]
 
         obs_vec = list(base_state_vec) + list(hazards_lidar_vec) + list(goal_lidar_vec)
 
-        # obs_vec = self.make_observation(obs, lidar_vec)
         obs_vec = np.array(obs_vec)
-        obs_vec = torch.as_tensor(obs_vec, dtype=torch.float32, device=self._device).unsqueeze(0)
-        return obs_vec
+
+        return torch.as_tensor(obs_vec, dtype=torch.float32, device=self._device).unsqueeze(0)
 
     def _ego_xy(
         self,
         robot_matrix: list[list[float]],
         robot_pos: np.ndarray,
         pos: np.ndarray,
     ) -> np.ndarray:
@@ -460,25 +461,36 @@
                 info['final_observation'],
                 dtype=torch.float32,
                 device=self._device,
             )
 
         return obs, reward, cost, terminated, truncated, info
 
-    def reset(self, seed: int | None = None) -> tuple[torch.Tensor, dict[str, Any]]:
+    @property
+    def max_episode_steps(self) -> int:
+        """The max steps per episode."""
+        return self._env.env.spec.max_episode_steps
+
+    def reset(
+        self,
+        seed: int | None = None,
+        options: dict[str, Any] | None = None,
+    ) -> tuple[torch.Tensor, dict[str, Any]]:
         """Reset the environment.
 
         Args:
-            seed (int, optional): Seed to reset the environment. Defaults to None.
+            seed (int, optional): The random seed. Defaults to None.
+            options (dict[str, Any], optional): The options for the environment. Defaults to None.
+
 
         Returns:
             observation: The initial observation of the space.
             info: Some information logged by the environment.
         """
-        obs_original, info = self._env.reset(seed=seed)
+        obs_original, info = self._env.reset(seed=seed, options=options)
         if self._task == 'Goal':
             self.goal_position = self._env.task.goal.pos
             self.robot_position = self._env.task.agent.pos
             self.hazards_position = self._env.task.hazards.pos
             self.goal_distance = self._dist_xy(self.robot_position, self.goal_position)
             coordinate_sensor_obs = self._get_coordinate_sensor()
             flat_coordinate_obs = self._get_flat_coordinate(coordinate_sensor_obs)
@@ -493,26 +505,14 @@
         """Set the seed for the environment.
 
         Args:
             seed (int): Seed to set.
         """
         self.reset(seed=seed)
 
-    def sample_action(self) -> torch.Tensor:
-        """Sample a random action.
-
-        Returns:
-            The sampled action.
-        """
-        return torch.as_tensor(
-            self._env.action_space.sample(),
-            dtype=torch.float32,
-            device=self._device,
-        )
-
     def render(self) -> Any:
         """Render the environment.
 
         Returns:
             The rendered frames, we recommend using `np.ndarray` which could construct video by
             moviepy.
         """
```

### Comparing `omnisafe-0.5.0b0/omnisafe/envs/wrapper.py` & `omnisafe-0.5.1b0/omnisafe/envs/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,29 +48,34 @@
     def __init__(self, env: CMDP, time_limit: int, device: torch.device) -> None:
         """Initialize an instance of :class:`TimeLimit`."""
         super().__init__(env=env, device=device)
         assert self.num_envs == 1, 'TimeLimit only supports single environment'
         self._time: int = 0
         self._time_limit: int = time_limit
 
-    def reset(self, seed: int | None = None) -> tuple[torch.Tensor, dict[str, Any]]:
+    def reset(
+        self,
+        seed: int | None = None,
+        options: dict[str, Any] | None = None,
+    ) -> tuple[torch.Tensor, dict[str, Any]]:
         """Reset the environment.
 
         .. note::
             Additionally, the time step will be reset to 0.
 
         Args:
-            seed (int or None, optional): The seed for the environment. Defaults to None.
+            seed (int, optional): The random seed. Defaults to None.
+            options (dict[str, Any], optional): The options for the environment. Defaults to None.
 
         Returns:
             observation: The initial observation of the space.
             info: Some information logged by the environment.
         """
         self._time = 0
-        return super().reset(seed)
+        return super().reset(seed=seed, options=options)
 
     def step(
         self,
         action: torch.Tensor,
     ) -> tuple[
         torch.Tensor,
         torch.Tensor,
@@ -231,25 +236,30 @@
             info['final_observation'][final_obs_slice] = self._obs_normalizer.normalize(
                 info['final_observation'][final_obs_slice],
             )
         info['original_obs'] = obs
         obs = self._obs_normalizer.normalize(obs)
         return obs, reward, cost, terminated, truncated, info
 
-    def reset(self, seed: int | None = None) -> tuple[torch.Tensor, dict[str, Any]]:
+    def reset(
+        self,
+        seed: int | None = None,
+        options: dict[str, Any] | None = None,
+    ) -> tuple[torch.Tensor, dict[str, Any]]:
         """Reset the environment and returns an initial observation.
 
         Args:
-            seed (int or None, optional): Seed for the environment. Defaults to None.
+            seed (int, optional): The random seed. Defaults to None.
+            options (dict[str, Any], optional): The options for the environment. Defaults to None.
 
         Returns:
             observation: The initial observation of the space.
             info: Some information logged by the environment.
         """
-        obs, info = super().reset(seed)
+        obs, info = super().reset(seed=seed, options=options)
         info['original_obs'] = obs
         obs = self._obs_normalizer.normalize(obs)
         return obs, info
 
     def save(self) -> dict[str, torch.nn.Module]:
         """Save the observation normalizer.
 
@@ -428,16 +438,16 @@
         high (int or float): The upper bound of the action space.
     """
 
     def __init__(
         self,
         env: CMDP,
         device: torch.device,
-        low: int | float,
-        high: int | float,
+        low: float,
+        high: float,
     ) -> None:
         """Initialize an instance of :class:`ActionScale`."""
         super().__init__(env=env, device=device)
         assert isinstance(self.action_space, spaces.Box), 'Action space must be Box'
 
         self._old_min_action: torch.Tensor = torch.tensor(
             self.action_space.low,
@@ -496,14 +506,15 @@
             terminated: Whether the episode has ended.
             truncated: Whether the episode has been truncated due to a time limit.
             info: Some information logged by the environment.
         """
         action = self._old_min_action + (self._old_max_action - self._old_min_action) * (
             action - self._min_action
         ) / (self._max_action - self._min_action)
+
         return super().step(action)
 
 
 class ActionRepeat(Wrapper):
     """Repeat action given times.
 
     Example:
@@ -610,27 +621,32 @@
         )
         for k, v in info.items():
             if isinstance(v, torch.Tensor):
                 info[k] = v.unsqueeze(0)
 
         return obs, reward, cost, terminated, truncated, info
 
-    def reset(self, seed: int | None = None) -> tuple[torch.Tensor, dict[str, Any]]:
+    def reset(
+        self,
+        seed: int | None = None,
+        options: dict[str, Any] | None = None,
+    ) -> tuple[torch.Tensor, dict[str, Any]]:
         """Reset the environment and returns a new observation.
 
         .. note::
             The vector information will be unsqueezed to (1, dim) for agent training.
 
         Args:
-            seed (int or None, optional): Set the seed for the environment. Defaults to None.
+            seed (int, optional): The random seed. Defaults to None.
+            options (dict[str, Any], optional): The options for the environment. Defaults to None.
 
         Returns:
             observation: The initial observation of the space.
             info: Some information logged by the environment.
         """
-        obs, info = super().reset(seed)
+        obs, info = super().reset(seed=seed, options=options)
         obs = obs.unsqueeze(0)
         for k, v in info.items():
             if isinstance(v, torch.Tensor):
                 info[k] = v.unsqueeze(0)
 
         return obs, info
```

### Comparing `omnisafe-0.5.0b0/omnisafe/evaluator.py` & `omnisafe-0.5.1b0/omnisafe/evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,32 +50,29 @@
     Args:
         env (CMDP or None, optional): The environment. Defaults to None.
         actor (Actor or None, optional): The actor. Defaults to None.
         render_mode (str, optional): The render mode. Defaults to 'rgb_array'.
     """
 
     _cfgs: Config
+    _dict_cfgs: dict[str, Any]
     _save_dir: str
     _model_name: str
     _cost_count: torch.Tensor
 
     # pylint: disable-next=too-many-arguments
     def __init__(
         self,
         env: CMDP | None = None,
         actor: Actor | None = None,
         actor_critic: ConstraintActorCritic | ConstraintActorQCritic | None = None,
         dynamics: EnsembleDynamicsModel | None = None,
-        planner: CEMPlanner
-        | ARCPlanner
-        | SafeARCPlanner
-        | CCEPlanner
-        | CAPPlanner
-        | RCEPlanner
-        | None = None,
+        planner: (
+            CEMPlanner | ARCPlanner | SafeARCPlanner | CCEPlanner | CAPPlanner | RCEPlanner | None
+        ) = None,
         render_mode: str = 'rgb_array',
     ) -> None:
         """Initialize an instance of :class:`Evaluator`."""
         self._env: CMDP | None = env
         self._actor: Actor | None = actor
         self._actor_critic: ConstraintActorCritic | ConstraintActorQCritic | None = actor_critic
         self._dynamics: EnsembleDynamicsModel | None = dynamics
@@ -115,14 +112,15 @@
         try:
             with open(cfg_path, encoding='utf-8') as file:
                 kwargs = json.load(file)
         except FileNotFoundError as error:
             raise FileNotFoundError(
                 f'The config file is not found in the save directory{save_dir}.',
             ) from error
+        self._dict_cfgs = kwargs
         self._cfgs = Config.dict2config(kwargs)
 
     # pylint: disable-next=too-many-branches
     def __load_model_and_env(
         self,
         save_dir: str,
         model_name: str,
@@ -327,14 +325,16 @@
             'num_envs': 1,
             'render_mode': self._render_mode,
             'camera_id': camera_id,
             'camera_name': camera_name,
             'width': width,
             'height': height,
         }
+        if self._dict_cfgs.get('env_cfgs') is not None:
+            env_kwargs.update(self._dict_cfgs['env_cfgs'])
 
         self.__load_model_and_env(save_dir, model_name, env_kwargs)
 
     def evaluate(
         self,
         num_episodes: int = 10,
         cost_criteria: float = 1.0,
@@ -411,14 +411,16 @@
             print(f'Episode length: {length}')
 
         print(self._dividing_line)
         print('Evaluation results:')
         print(f'Average episode reward: {np.mean(a=episode_rewards)}')
         print(f'Average episode cost: {np.mean(a=episode_costs)}')
         print(f'Average episode length: {np.mean(a=episode_lengths)}')
+
+        self._env.close()
         return (
             episode_rewards,
             episode_costs,
         )
 
     @property
     def fps(self) -> int:
@@ -429,15 +431,15 @@
             AtrributeError: If the fps is not found.
         """
         assert (
             self._env is not None
         ), 'The environment must be provided or created before getting the fps.'
         try:
             fps = self._env.metadata['render_fps']
-        except AttributeError:
+        except (AttributeError, KeyError):
             fps = 30
             warnings.warn('The fps is not found, use 30 as default.', stacklevel=2)
 
         return fps
 
     def render(  # pylint: disable=too-many-locals,too-many-arguments,too-many-branches,too-many-statements
         self,
@@ -548,7 +550,8 @@
                 print(f'Episode length: {length}', file=f)
         with open(result_path, 'a+', encoding='utf-8') as f:
             print(self._dividing_line)
             print('Evaluation results:', file=f)
             print(f'Average episode reward: {np.mean(episode_rewards)}', file=f)
             print(f'Average episode cost: {np.mean(episode_costs)}', file=f)
             print(f'Average episode length: {np.mean(episode_lengths)}', file=f)
+        self._env.close()
```

### Comparing `omnisafe-0.5.0b0/omnisafe/models/__init__.py` & `omnisafe-0.5.1b0/omnisafe/models/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/models/actor/__init__.py` & `omnisafe-0.5.1b0/omnisafe/models/actor/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/models/actor/actor_builder.py` & `omnisafe-0.5.1b0/omnisafe/models/actor/actor_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from __future__ import annotations
 
 from omnisafe.models.actor.gaussian_learning_actor import GaussianLearningActor
 from omnisafe.models.actor.gaussian_sac_actor import GaussianSACActor
 from omnisafe.models.actor.mlp_actor import MLPActor
 from omnisafe.models.actor.perturbation_actor import PerturbationActor
 from omnisafe.models.actor.vae_actor import VAE
+from omnisafe.models.base import Actor
 from omnisafe.typing import Activation, ActorType, InitFunction, OmnisafeSpace
 
 
 # pylint: disable-next=too-few-public-methods
 class ActorBuilder:
     """Class for building actor networks.
 
@@ -52,15 +53,15 @@
         self._activation: Activation = activation
         self._hidden_sizes: list[int] = hidden_sizes
 
     # pylint: disable-next=too-many-return-statements
     def build_actor(
         self,
         actor_type: ActorType,
-    ) -> GaussianLearningActor | GaussianSACActor | MLPActor | VAE | PerturbationActor:
+    ) -> Actor:
         """Build actor network.
 
         Currently, we support the following actor types:
             - ``gaussian_learning``: Gaussian actor with learnable standard deviation parameters.
             - ``gaussian_sac``: Gaussian actor with learnable standard deviation network.
             - ``mlp``: Multi-layer perceptron actor, used in ``DDPG`` and ``TD3``.
```

### Comparing `omnisafe-0.5.0b0/omnisafe/models/actor/gaussian_actor.py` & `omnisafe-0.5.1b0/omnisafe/models/actor/gaussian_actor.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/models/actor/gaussian_learning_actor.py` & `omnisafe-0.5.1b0/omnisafe/models/actor/gaussian_learning_actor.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/models/actor/gaussian_sac_actor.py` & `omnisafe-0.5.1b0/omnisafe/models/actor/gaussian_sac_actor.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,15 @@
             The current distribution.
         """
         self._current_dist = self._distribution(obs)
         self._after_inference = True
         return TanhNormal(self._current_dist.mean, self._current_dist.stddev)
 
     def log_prob(self, act: torch.Tensor) -> torch.Tensor:
+        # pylint: disable=not-callable
         r"""Compute the log probability of the action given the current distribution.
 
         .. warning::
             You must call :meth:`forward` or :meth:`predict` before calling this method.
 
         .. note::
             In this method, we will regularize the log probability of the action. The regularization
@@ -150,17 +151,21 @@
         if self._current_raw_action is not None:
             logp = self._current_dist.log_prob(self._current_raw_action).sum(axis=-1)
             logp -= (
                 2
                 * (
                     self._log2
                     - self._current_raw_action
-                    - nn.functional.softplus(-2 * self._current_raw_action)
+                    - nn.functional.softplus(
+                        -2 * self._current_raw_action,
+                    )
                 )
-            ).sum(axis=-1)
+            ).sum(
+                axis=-1,
+            )  # type: ignore
             self._current_raw_action = None
         else:
             logp = (
                 TanhNormal(self._current_dist.mean, self._current_dist.stddev)
                 .log_prob(act)
                 .sum(axis=-1)
             )
```

### Comparing `omnisafe-0.5.0b0/omnisafe/models/actor/mlp_actor.py` & `omnisafe-0.5.1b0/omnisafe/models/actor/mlp_actor.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/models/actor/perturbation_actor.py` & `omnisafe-0.5.1b0/omnisafe/models/actor/perturbation_actor.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/models/actor/vae_actor.py` & `omnisafe-0.5.1b0/omnisafe/models/actor/vae_actor.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/models/actor_critic/__init__.py` & `omnisafe-0.5.1b0/omnisafe/models/actor_critic/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/models/actor_critic/actor_critic.py` & `omnisafe-0.5.1b0/omnisafe/models/actor_critic/actor_critic.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,23 +16,17 @@
 
 from __future__ import annotations
 
 import torch
 from torch import nn, optim
 from torch.optim.lr_scheduler import ConstantLR, LinearLR
 
-from omnisafe.models.actor import (
-    VAE,
-    GaussianLearningActor,
-    GaussianSACActor,
-    MLPActor,
-    PerturbationActor,
-)
+from omnisafe.models.actor import GaussianLearningActor
 from omnisafe.models.actor.actor_builder import ActorBuilder
-from omnisafe.models.base import Critic
+from omnisafe.models.base import Actor, Critic
 from omnisafe.models.critic.critic_builder import CriticBuilder
 from omnisafe.typing import OmnisafeSpace
 from omnisafe.utils.config import ModelConfig
 from omnisafe.utils.schedule import PiecewiseSchedule, Schedule
 
 
 class ActorCritic(nn.Module):
@@ -69,15 +63,15 @@
         act_space: OmnisafeSpace,
         model_cfgs: ModelConfig,
         epochs: int,
     ) -> None:
         """Initialize an instance of :class:`ActorCritic`."""
         super().__init__()
 
-        self.actor: GaussianLearningActor | GaussianSACActor | MLPActor | VAE | PerturbationActor = ActorBuilder(
+        self.actor: Actor = ActorBuilder(
             obs_space=obs_space,
             act_space=act_space,
             hidden_sizes=model_cfgs.actor.hidden_sizes,
             activation=model_cfgs.actor.activation,
             weight_initialization_mode=model_cfgs.weight_initialization_mode,
         ).build_actor(
             actor_type=model_cfgs.actor_type,
@@ -106,22 +100,20 @@
             self.actor_scheduler: LinearLR | ConstantLR
             if model_cfgs.linear_lr_decay:
                 self.actor_scheduler = LinearLR(
                     self.actor_optimizer,
                     start_factor=1.0,
                     end_factor=0.0,
                     total_iters=epochs,
-                    verbose=True,
                 )
             else:
                 self.actor_scheduler = ConstantLR(
                     self.actor_optimizer,
                     factor=1.0,
                     total_iters=epochs,
-                    verbose=True,
                 )
 
     def step(
         self,
         obs: torch.Tensor,
         deterministic: bool = False,
     ) -> tuple[torch.Tensor, ...]:
```

### Comparing `omnisafe-0.5.0b0/omnisafe/models/actor_critic/actor_q_critic.py` & `omnisafe-0.5.1b0/omnisafe/models/actor_critic/actor_q_critic.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,23 +18,16 @@
 
 from copy import deepcopy
 
 import torch
 from torch import nn, optim
 from torch.optim.lr_scheduler import ConstantLR, LinearLR
 
-from omnisafe.models.actor import (
-    VAE,
-    GaussianLearningActor,
-    GaussianSACActor,
-    MLPActor,
-    PerturbationActor,
-)
 from omnisafe.models.actor.actor_builder import ActorBuilder
-from omnisafe.models.base import Critic
+from omnisafe.models.base import Actor, Critic
 from omnisafe.models.critic.critic_builder import CriticBuilder
 from omnisafe.typing import OmnisafeSpace
 from omnisafe.utils.config import ModelConfig
 
 
 class ActorQCritic(nn.Module):
     """Class for ActorQCritic.
@@ -72,15 +65,15 @@
         act_space: OmnisafeSpace,
         model_cfgs: ModelConfig,
         epochs: int,
     ) -> None:
         """Initialize an instance of :class:`ActorQCritic`."""
         super().__init__()
 
-        self.actor: GaussianLearningActor | GaussianSACActor | MLPActor | VAE | PerturbationActor = ActorBuilder(
+        self.actor: Actor = ActorBuilder(
             obs_space=obs_space,
             act_space=act_space,
             hidden_sizes=model_cfgs.actor.hidden_sizes,
             activation=model_cfgs.actor.activation,
             weight_initialization_mode=model_cfgs.weight_initialization_mode,
         ).build_actor(
             actor_type=model_cfgs.actor_type,
@@ -93,15 +86,15 @@
             weight_initialization_mode=model_cfgs.weight_initialization_mode,
             num_critics=model_cfgs.critic.num_critics,
             use_obs_encoder=False,
         ).build_critic(critic_type='q')
         self.target_reward_critic: Critic = deepcopy(self.reward_critic)
         for param in self.target_reward_critic.parameters():
             param.requires_grad = False
-        self.target_actor: GaussianLearningActor | GaussianSACActor | MLPActor | VAE | PerturbationActor = deepcopy(
+        self.target_actor: Actor = deepcopy(
             self.actor,
         )
         for param in self.target_actor.parameters():
             param.requires_grad = False
         self.add_module('actor', self.actor)
         self.add_module('reward_critic', self.reward_critic)
 
@@ -118,22 +111,20 @@
         self.actor_scheduler: LinearLR | ConstantLR
         if model_cfgs.linear_lr_decay:
             self.actor_scheduler = LinearLR(
                 self.actor_optimizer,
                 start_factor=1.0,
                 end_factor=0.0,
                 total_iters=epochs,
-                verbose=True,
             )
         else:
             self.actor_scheduler = ConstantLR(
                 self.actor_optimizer,
                 factor=1.0,
                 total_iters=epochs,
-                verbose=True,
             )
 
     def step(self, obs: torch.Tensor, deterministic: bool = False) -> torch.Tensor:
         """Choose the action based on the observation. used in rollout without gradient.
 
         Args:
             obs (torch.tensor): The observation from environments.
```

### Comparing `omnisafe-0.5.0b0/omnisafe/models/actor_critic/constraint_actor_critic.py` & `omnisafe-0.5.1b0/omnisafe/models/actor_critic/constraint_actor_critic.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/models/actor_critic/constraint_actor_q_critic.py` & `omnisafe-0.5.1b0/omnisafe/models/actor_critic/constraint_actor_q_critic.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/models/base.py` & `omnisafe-0.5.1b0/omnisafe/models/base.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/models/critic/__init__.py` & `omnisafe-0.5.1b0/omnisafe/models/critic/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/models/critic/critic_builder.py` & `omnisafe-0.5.1b0/omnisafe/models/critic/critic_builder.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/models/critic/q_critic.py` & `omnisafe-0.5.1b0/omnisafe/models/critic/q_critic.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/models/critic/v_critic.py` & `omnisafe-0.5.1b0/omnisafe/models/critic/v_critic.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/models/offline/__init__.py` & `omnisafe-0.5.1b0/omnisafe/models/offline/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/models/offline/dice.py` & `omnisafe-0.5.1b0/omnisafe/models/offline/dice.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/typing.py` & `omnisafe-0.5.1b0/omnisafe/typing.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/utils/__init__.py` & `omnisafe-0.5.1b0/omnisafe/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/utils/command_app.py` & `omnisafe-0.5.1b0/omnisafe/utils/command_app.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/utils/config.py` & `omnisafe-0.5.1b0/omnisafe/utils/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,15 +241,15 @@
         The default kwargs.
     """
     path = os.path.dirname(os.path.abspath(__file__))
     cfg_path = os.path.join(path, '..', 'configs', algo_type, f'{algo}.yaml')
     print(f'Loading {algo}.yaml from {cfg_path}')
     kwargs = load_yaml(cfg_path)
     default_kwargs = kwargs['defaults']
-    env_spec_kwargs = kwargs[env_id] if env_id in kwargs else None
+    env_spec_kwargs = kwargs.get(env_id)
 
     default_kwargs = Config.dict2config(default_kwargs)
 
     if env_spec_kwargs is not None:
         default_kwargs.recurisve_update(env_spec_kwargs)
 
     return default_kwargs
@@ -343,15 +343,15 @@
         assert isinstance(configs.obs_normalize, bool), 'obs_normalize must be bool'
         assert isinstance(configs.kl_early_stop, bool), 'kl_early_stop must be bool'
         assert isinstance(configs.use_max_grad_norm, bool), 'use_max_grad_norm must be bool'
         assert isinstance(configs.use_critic_norm, bool), 'use_critic_norm must be bool'
         assert isinstance(configs.max_grad_norm, float) and isinstance(
             configs.critic_norm_coef,
             float,
-        ), 'norm must be bool'
+        ), 'norm must be float'
         assert (
             isinstance(configs.gamma, float) and configs.gamma >= 0.0 and configs.gamma <= 1.0
         ), 'gamma must be float, and it values must be [0.0, 1.0]'
         assert (
             isinstance(configs.cost_gamma, float)
             and configs.cost_gamma >= 0.0
             and configs.cost_gamma <= 1.0
```

### Comparing `omnisafe-0.5.0b0/omnisafe/utils/distributed.py` & `omnisafe-0.5.1b0/omnisafe/utils/distributed.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,26 @@
     backend = 'gloo' if device == 'cpu' else 'nccl'
     if os.getenv('MASTER_ADDR') is not None and os.getenv('IN_DIST') is None:
         dist.init_process_group(backend=backend)
         os.environ['IN_DIST'] = '1'
     # check if MPI is already setup..
     if parallel > 1 and os.getenv('MASTER_ADDR') is None:
         # MPI is not yet set up: quit parent process and start N child processes
-        os.environ['USE_DISTRIBUTED'] = '1'
+        if device != 'cpu':
+            initial_device = int(device.split(':')[-1])
+            os.environ['USE_DISTRIBUTED'] = '1'
+            if os.getenv('CUDA_VISIBLE_DEVICES') is None:
+                os.environ['CUDA_VISIBLE_DEVICES'] = ','.join(
+                    str(initial_device + i) for i in range(parallel)
+                )
+            num_gpu = int((len(os.environ['CUDA_VISIBLE_DEVICES']) + 1) / 2)
+            assert (
+                num_gpu >= parallel
+            ), f'Please make sure you have enough available GPUs to run Parallel {parallel}, \
+                current available Devices are {num_gpu}.'
         env = os.environ.copy()
         env.update(MKL_NUM_THREADS='1', OMP_NUM_THREADS='1', IN_MPI='1')
         args = [
             'torchrun',
             '--rdzv_backend',
             'c10d',
             '--rdzv_endpoint',
@@ -241,15 +252,15 @@
     if world_size() > 1:
         for parameter in module.parameters():
             param_tensor = parameter.data
             avg_param_tensor = dist_avg(param_tensor)
             param_tensor[:] = avg_param_tensor[:]
 
 
-def dist_avg(value: np.ndarray | torch.Tensor | int | float) -> torch.Tensor:
+def dist_avg(value: np.ndarray | torch.Tensor | float) -> torch.Tensor:
     """Average a tensor over distributed processes.
 
     Examples:
         >>> # In process 0
         >>> x = torch.tensor(1.0)
         >>> # In process 1
         >>> x = torch.tensor(2.0)
@@ -261,15 +272,15 @@
 
     Returns:
         Averaged tensor.
     """
     return dist_sum(value) / world_size()
 
 
-def dist_max(value: np.ndarray | torch.Tensor | int | float) -> torch.Tensor:
+def dist_max(value: np.ndarray | torch.Tensor | float) -> torch.Tensor:
     """Determine global maximum of tensor over distributed processes.
 
     Examples:
         >>> # In process 0
         >>> x = torch.tensor(1.0)
         >>> # In process 1
         >>> x = torch.tensor(2.0)
@@ -281,15 +292,15 @@
 
     Returns:
         Maximum tensor.
     """
     return dist_op(value, ReduceOp.MAX)
 
 
-def dist_min(value: np.ndarray | torch.Tensor | int | float) -> torch.Tensor:
+def dist_min(value: np.ndarray | torch.Tensor | float) -> torch.Tensor:
     """Determine global minimum of tensor over distributed processes.
 
     Examples:
         >>> # In process 0
         >>> x = torch.tensor(1.0)
         >>> # In process 1
         >>> x = torch.tensor(2.0)
@@ -301,15 +312,15 @@
 
     Returns:
         Minimum tensor.
     """
     return dist_op(value, ReduceOp.MIN)
 
 
-def dist_sum(value: np.ndarray | torch.Tensor | int | float) -> torch.Tensor:
+def dist_sum(value: np.ndarray | torch.Tensor | float) -> torch.Tensor:
     """Sum a tensor over distributed processes.
 
     Examples:
         >>> # In process 0
         >>> x = torch.tensor(1.0)
         >>> # In process 1
         >>> x = torch.tensor(2.0)
@@ -321,15 +332,15 @@
 
     Returns:
         Summed tensor.
     """
     return dist_op(value, ReduceOp.SUM)
 
 
-def dist_op(value: np.ndarray | torch.Tensor | int | float, operation: Any) -> torch.Tensor:
+def dist_op(value: np.ndarray | torch.Tensor | float, operation: Any) -> torch.Tensor:
     """Multi-processing operation.
 
     .. note::
         The operation can be ``ReduceOp.SUM``, ``ReduceOp.MAX``, ``ReduceOp.MIN``. corresponding to
         :meth:`dist_sum`, :meth:`dist_max`, :meth:`dist_min`, respectively.
 
     Args:
@@ -365,15 +376,15 @@
         value (torch.Tensor): Value to be operated.
         with_min_and_max (bool, optional): whether to return min and max. Defaults to False.
 
     Returns:
         A tuple of the [mean, std] or [mean, std, min, max] of the input tensor.
     """
     global_sum = dist_sum(torch.sum(value))
-    global_n = dist_sum(len(value))
+    global_n = dist_sum(torch.tensor(len(value)).to(os.getenv('OMNISAFE_DEVICE', 'cpu')))
     mean = global_sum / global_n
 
     global_sum_sq = dist_sum(torch.sum((value - mean) ** 2))
     # compute global std
     std = torch.sqrt(global_sum_sq / global_n)
     if with_min_and_max:
         global_min = dist_min(value)
```

### Comparing `omnisafe-0.5.0b0/omnisafe/utils/exp_grid_tools.py` & `omnisafe-0.5.1b0/omnisafe/utils/exp_grid_tools.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/utils/math.py` & `omnisafe-0.5.1b0/omnisafe/utils/math.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,20 +167,22 @@
         tensor([-0.7616])
 
     Args:
         loc (float or Tensor): The mean of the underlying normal distribution.
         scale (float or Tensor): The standard deviation of the underlying normal distribution.
     """
 
-    arg_constraints = {'loc': constraints.real, 'scale': constraints.positive}
-
     def __init__(self, loc: torch.Tensor, scale: torch.Tensor) -> None:
         """Initialize an instance of :class:`TanhNormal`."""
         base_dist = Normal(loc, scale)
         super().__init__(base_dist, SafeTanhTransformer())
+        self.arg_constraints = {
+            'loc': constraints.real,
+            'scale': constraints.positive,
+        }
 
     def expand(self, batch_shape: tuple[int, ...], instance: Any | None = None) -> TanhNormal:
         """Expand the distribution."""
         new = self._get_checked_instance(TanhNormal, instance)
         return super().expand(batch_shape, new)
 
     @property
```

### Comparing `omnisafe-0.5.0b0/omnisafe/utils/model.py` & `omnisafe-0.5.1b0/omnisafe/utils/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         nn.init.orthogonal_(layer.weight, gain=np.sqrt(2))
     else:
         raise TypeError(f'Invalid initialization function: {init_function}')
 
 
 def get_activation(
     activation: Activation,
-) -> type[nn.Identity] | type[nn.ReLU] | type[nn.Sigmoid] | type[nn.Softplus] | type[nn.Tanh]:
+) -> type[nn.Identity | nn.ReLU | nn.Sigmoid | nn.Softplus | nn.Tanh]:
     """Get the activation function.
 
     The ``activation`` can be chosen from: ``identity``, ``relu``, ``sigmoid``, ``softplus``,
     ``tanh``.
 
     Args:
         activation (Activation): The activation function.
```

### Comparing `omnisafe-0.5.0b0/omnisafe/utils/plotter.py` & `omnisafe-0.5.1b0/omnisafe/utils/plotter.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/omnisafe/utils/schedule.py` & `omnisafe-0.5.1b0/omnisafe/utils/schedule.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     return left + alpha * (right - left)
 
 
 class Schedule(ABC):
     """Schedule for a value based on the step."""
 
     @abstractmethod
-    def value(self, time: int | float) -> int | float:
+    def value(self, time: float) -> float:
         """Value at time t."""
 
 
 # pylint: disable=too-few-public-methods
 class PiecewiseSchedule(Schedule):
     """Piece-wise schedule for a value based on the step, from OpenAI baselines.
 
@@ -46,24 +46,24 @@
         outside_value (int or float): Value to use if `t` is before the first time in `endpoints` or
             after the last one.
     """
 
     def __init__(
         self,
         endpoints: list[tuple[int, float]],
-        outside_value: int | float,
+        outside_value: float,
     ) -> None:
         """Initialize an instance of :class:`PiecewiseSchedule`."""
         idxes = [e[0] for e in endpoints]
         assert idxes == sorted(idxes)
         self._interpolation: Callable[[float, float, float], float] = _linear_interpolation
-        self._outside_value: int | float = outside_value
+        self._outside_value: float = outside_value
         self._endpoints: list[tuple[int, float]] = endpoints
 
-    def value(self, time: int | float) -> int | float:
+    def value(self, time: float) -> float:
         """Value at time t.
 
         Args:
             time (int or float): Current time step.
 
         Returns:
             The interpolation value at time t or outside_value if t is before the first time in
@@ -85,15 +85,15 @@
 class ConstantSchedule(Schedule):
     """Constant schedule for a value."""
 
     def __init__(self, value: float) -> None:
         """Initialize an instance of :class:`ConstantSchedule`."""
         self._v: float = value
 
-    def value(self, time: int | float) -> int | float:  # pylint: disable=unused-argument
+    def value(self, time: float) -> float:  # pylint: disable=unused-argument
         """Value at time t.
 
         Args:
             time (int or float): Current time step.
 
         Returns:
             The interpolation value at time t or outside_value if t is before the first time in
```

### Comparing `omnisafe-0.5.0b0/omnisafe/utils/tools.py` & `omnisafe-0.5.1b0/omnisafe/utils/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,17 +267,19 @@
 
     Raises:
         AssertionError: If the type of the value is not the same as the default value.
         KeyError: If the key is not in default_config.
     """
     assert isinstance(config, dict), 'custom_cfgs must be a dict!'
     for key in config:
-        if key not in default_config.keys() and key not in exclude_keys:
+        if key not in default_config and key not in exclude_keys:
             raise KeyError(f'Invalid key: {key}')
-        if isinstance(config[key], dict):
+        if config[key] is None:
+            return
+        if isinstance(config[key], dict) and key != 'env_cfgs':
             recursive_check_config(config[key], default_config[key])
 
 
 def assert_with_exit(condition: bool, msg: str) -> None:
     """Assert with message.
 
     Examples:
```

### Comparing `omnisafe-0.5.0b0/omnisafe/version.py` & `omnisafe-0.5.1b0/omnisafe/version.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """OmniSafe: A comprehensive and reliable benchmark for safe reinforcement learning."""
 
-__version__ = '0.5.0b0'
+__version__ = '0.5.1b0'
 __license__ = 'Apache License, Version 2.0'
 __author__ = 'OmniSafe Contributors'
 __release__ = True
 
 if not __release__:
     import os
     import subprocess
```

### Comparing `omnisafe-0.5.0b0/omnisafe.egg-info/PKG-INFO` & `omnisafe-0.5.1b0/omnisafe.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnisafe
-Version: 0.5.0b0
+Version: 0.5.1b0
 Summary: A comprehensive and reliable benchmark for safe reinforcement learning.
 Author: OmniSafe Contributors
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://github.com/PKU-Alignment/omnisafe
 Project-URL: Repository, https://github.com/PKU-Alignment/omnisafe
 Project-URL: Documentation, https://omnisafe.readthedocs.io
 Project-URL: Bug Report, https://github.com/PKU-Alignment/omnisafe/issues
@@ -17,17 +17,44 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: safety-gymnasium>=0.2.0
+Requires-Dist: torch>=1.10.0
+Requires-Dist: numpy>=1.20.0
+Requires-Dist: tensorboard>=2.8.0
+Requires-Dist: wandb>=0.13.0
+Requires-Dist: pyyaml>=6.0
+Requires-Dist: moviepy>=1.0.0
+Requires-Dist: typing-extensions>=4.0.0
+Requires-Dist: typer[all]>=0.7.0
+Requires-Dist: seaborn>=0.12.2
+Requires-Dist: pandas==2.0.3
+Requires-Dist: matplotlib>=3.7.1
+Requires-Dist: gdown>=4.6.0
 Provides-Extra: lint
+Requires-Dist: isort>=5.11.0; extra == "lint"
+Requires-Dist: black>=22.6.0; extra == "lint"
+Requires-Dist: pylint[spelling]>=2.15.0; extra == "lint"
+Requires-Dist: mypy>=0.990; extra == "lint"
+Requires-Dist: flake8; extra == "lint"
+Requires-Dist: flake8-bugbear; extra == "lint"
+Requires-Dist: ruff; extra == "lint"
+Requires-Dist: doc8; extra == "lint"
+Requires-Dist: pydocstyle; extra == "lint"
+Requires-Dist: pyenchant; extra == "lint"
+Requires-Dist: pre-commit; extra == "lint"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-xdist; extra == "test"
 
 <!-- markdownlint-disable first-line-h1 -->
 <!-- markdownlint-disable html -->
 
 <div align="center">
   <img src="https://github.com/PKU-Alignment/omnisafe/raw/HEAD/images/logo.png" width="75%"/>
 </div>
@@ -82,20 +109,22 @@
     - [Prerequisites](#prerequisites)
     - [Install from source](#install-from-source)
     - [Install from PyPI](#install-from-pypi)
 - [Implemented Algorithms](#implemented-algorithms)
   - [Examples](#examples)
     - [Algorithms Registry](#algorithms-registry)
     - [Supported Environments](#supported-environments)
+    - [Customizing your environment](#customizing-your-environment)
     - [Try with CLI](#try-with-cli)
 - [Getting Started](#getting-started)
   - [Important Hints](#important-hints)
   - [Quickstart: Colab on the Cloud](#quickstart-colab-on-the-cloud)
 - [Changelog](#changelog)
 - [Citing OmniSafe](#citing-omnisafe)
+- [Publications using OmniSafe](#publications-using-omnisafe)
 - [The OmniSafe Team](#the-omnisafe-team)
 - [License](#license)
 
 --------------------------------------------------------------------------------
 
 ## Quick Start
 
@@ -313,14 +342,26 @@
     <td>SafetyHumanoidVelocity-v1</td>
   </tr>
 </tbody>
 </table>
 
 For more information about environments, please refer to [Safety-Gymnasium](https://www.safety-gymnasium.com).
 
+#### Customizing your environment
+
+We offer a flexible customized environment interface that allows users to achieve the following **without modifying the OmniSafe source code**:
+
+- Use OmniSafe to train algorithms on customized environments.
+- Create the the environment with specified personalized parameters.
+- Complete the recording of environment-specific information in Logger.
+
+We provide **step-by-step tutorials** on [Environment Customization From Scratch](https://colab.research.google.com/github/PKU-Alignment/omnisafe/blob/main/tutorials/English/3.Environment%20Customization%20from%20Scratch.ipynb) and [Environment Customization From Community](https://colab.research.google.com/github/PKU-Alignment/omnisafe/blob/main/tutorials/English/4.Environment%20Customization%20from%20Community.ipynb) to give you a detailed introduction on how to use this extraordinary feature of OmniSafe.
+
+*Note: If you find trouble customizing your environment, please feel free to open an [issue](https://github.com/PKU-Alignment/omnisafe/issues) or [discussion](https://github.com/PKU-Alignment/omnisafe/discussions). [Pull requests](https://github.com/PKU-Alignment/omnisafe/pulls) are also welcomed if you're willing to contribute the implementation of your environments interface.*
+
 #### Try with CLI
 
 ```bash
 pip install omnisafe
 
 omnisafe --help  # Ask for help
 
@@ -386,14 +427,26 @@
   title   = {OmniSafe: An Infrastructure for Accelerating Safe Reinforcement Learning Research},
   author  = {Jiaming Ji, Jiayi Zhou, Borong Zhang, Juntao Dai, Xuehai Pan, Ruiyang Sun, Weidong Huang, Yiran Geng, Mickel Liu, Yaodong Yang},
   journal = {arXiv preprint arXiv:2305.09304},
   year    = {2023}
 }
 ```
 
+## Publications using OmniSafe
+
+We have compiled a list of papers that use OmniSafe for algorithm implementation or experimentation. If you are willing to include your work in this list, or if you wish to have your implementation officially integrated into OmniSafe, please feel free to [contact us](https://github.com/PKU-Alignment/omnisafe/issues).
+
+| Papers | Publisher|
+|:---:|:---:|
+| [Off-Policy Primal-Dual Safe Reinforcement Learning](https://openreview.net/pdf?id=vy42bYs1Wo) | ICLR 2024 |
+| [Safe Offline Reinforcement Learning with Feasibility-Guided Diffusion Model](https://openreview.net/pdf?id=j5JvZCaDM0) | ICLR 2024 |
+| [Iterative Reachability Estimation for Safe Reinforcement Learning](https://proceedings.neurips.cc/paper_files/paper/2023/file/dca63f2650fe9e88956c1b68440b8ee9-Paper-Conference.pdf) | NeurIPS 2023 |
+| [Balance Reward and Safety Optimization for Safe Reinforcement Learning: A Perspective of Gradient Manipulation](https://ojs.aaai.org/index.php/AAAI/article/view/30102/31944) | AAAI 2024 |
+| [Learning Safety Constraints From Demonstration Using One-Class Decision Trees](https://openreview.net/pdf?id=dxUi16pvub) | AAAI 2024 WorkShops |
+
 ## The OmniSafe Team
 
 OmniSafe is mainly developed by the SafeRL research team directed by Prof. [Yaodong Yang](https://www.yangyaodong.com/).
 Our SafeRL research team members include [Borong Zhang](https://github.com/muchvo), [Jiayi Zhou](https://github.com/Gaiejj), [JTao Dai](https://github.com/calico-1226), [Weidong Huang](https://github.com/hdadong), [Ruiyang Sun](https://github.com/rockmagma02), [Xuehai Pan](https://github.com/XuehaiPan) and [Jiaming Ji](https://github.com/zmsn-2077).
 If you have any questions in the process of using OmniSafe, don't hesitate to ask your questions on [the GitHub issue page](https://github.com/PKU-Alignment/omnisafe/issues/new/choose), we will reply to you in 2-3 working days.
 
 ## License
```

#### html2text {}

```diff
@@ -1,24 +1,37 @@
-Metadata-Version: 2.1 Name: omnisafe Version: 0.5.0b0 Summary: A comprehensive
+Metadata-Version: 2.1 Name: omnisafe Version: 0.5.1b0 Summary: A comprehensive
 and reliable benchmark for safe reinforcement learning. Author: OmniSafe
 Contributors License: Apache License, Version 2.0 Project-URL: Homepage, https:
 //github.com/PKU-Alignment/omnisafe Project-URL: Repository, https://
 github.com/PKU-Alignment/omnisafe Project-URL: Documentation, https://
 omnisafe.readthedocs.io Project-URL: Bug Report, https://github.com/PKU-
 Alignment/omnisafe/issues Keywords: Safe Reinforcement Learning,Reinforcement
 Learning,PyTorch Classifier: Development Status :: 4 - Beta Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Intended Audience :: Science/Research Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Provides-Extra: lint Provides-Extra: test License-
-File: LICENSE
+Content-Type: text/markdown License-File: LICENSE Requires-Dist: safety-
+gymnasium>=0.2.0 Requires-Dist: torch>=1.10.0 Requires-Dist: numpy>=1.20.0
+Requires-Dist: tensorboard>=2.8.0 Requires-Dist: wandb>=0.13.0 Requires-Dist:
+pyyaml>=6.0 Requires-Dist: moviepy>=1.0.0 Requires-Dist: typing-
+extensions>=4.0.0 Requires-Dist: typer[all]>=0.7.0 Requires-Dist:
+seaborn>=0.12.2 Requires-Dist: pandas==2.0.3 Requires-Dist: matplotlib>=3.7.1
+Requires-Dist: gdown>=4.6.0 Provides-Extra: lint Requires-Dist: isort>=5.11.0;
+extra == "lint" Requires-Dist: black>=22.6.0; extra == "lint" Requires-Dist:
+pylint[spelling]>=2.15.0; extra == "lint" Requires-Dist: mypy>=0.990; extra ==
+"lint" Requires-Dist: flake8; extra == "lint" Requires-Dist: flake8-bugbear;
+extra == "lint" Requires-Dist: ruff; extra == "lint" Requires-Dist: doc8; extra
+== "lint" Requires-Dist: pydocstyle; extra == "lint" Requires-Dist: pyenchant;
+extra == "lint" Requires-Dist: pre-commit; extra == "lint" Provides-Extra: test
+Requires-Dist: pytest; extra == "test" Requires-Dist: pytest-cov; extra ==
+"test" Requires-Dist: pytest-xdist; extra == "test"
      [https://github.com/PKU-Alignment/omnisafe/raw/HEAD/images/logo.png]
   [![Organization](https://img.shields.io/badge/Organization-PKU--Alignment-
 blue)](https://github.com/PKU-Alignment) [![PyPI](https://img.shields.io/pypi/
  v/omnisafe?logo=pypi)](https://pypi.org/project/omnisafe) [![tests](https://
      img.shields.io/github/actions/workflow/status/PKU-Alignment/omnisafe/
  test.yml?label=tests&logo=github)](https://github.com/PKU-Alignment/omnisafe/
  tree/HEAD/tests) [![Documentation Status](https://img.shields.io/readthedocs/
@@ -69,75 +82,77 @@
 video](https://github-production-user-asset-6210df.s3.amazonaws.com/73586554/
 237139607-d1e6f413-aa2c-4f68-b8ee-08a4361493a0.gif) ---------------------------
 ----------------------------------------------------- ### Table of Contents -
 [Quick Start](#quick-start) - [Installation](#installation) - [Prerequisites]
 (#prerequisites) - [Install from source](#install-from-source) - [Install from
 PyPI](#install-from-pypi) - [Implemented Algorithms](#implemented-algorithms) -
 [Examples](#examples) - [Algorithms Registry](#algorithms-registry) -
-[Supported Environments](#supported-environments) - [Try with CLI](#try-with-
-cli) - [Getting Started](#getting-started) - [Important Hints](#important-
-hints) - [Quickstart: Colab on the Cloud](#quickstart-colab-on-the-cloud) -
-[Changelog](#changelog) - [Citing OmniSafe](#citing-omnisafe) - [The OmniSafe
-Team](#the-omnisafe-team) - [License](#license) -------------------------------
-------------------------------------------------- ## Quick Start ###
-Installation #### Prerequisites OmniSafe requires Python 3.8+ and PyTorch
-1.10+. > We support and test for Python 3.8, 3.9, 3.10 on Linux. Meanwhile, we
-also support M1 and M2 versions of macOS. We will accept PRs related to
-Windows, but do not officially support it. #### Install from source ```bash #
-Clone the repo git clone https://github.com/PKU-Alignment/omnisafe.git cd
-omnisafe # Create a conda environment conda env create --file conda-recipe.yaml
-conda activate omnisafe # Install omnisafe pip install -e . ``` #### Install
-from PyPI OmniSafe is hosted in [![PyPI](https://img.shields.io/pypi/v/
-omnisafe?label=pypi&logo=pypi)](https://pypi.org/project/omnisafe) / ![Status]
-(https://img.shields.io/pypi/status/omnisafe?label=status). ```bash pip install
-omnisafe ``` ## Implemented Algorithms LLaatteesstt SSaaffeeRRLL PPaappeerrss - **[AAAI 2023]**
-Augmented Proximal Policy Optimization for Safe Reinforcement Learning (APPO) -
-**[NeurIPS 2022]** [Constrained Update Projection Approach to Safe Policy
-Optimization (CUP)](https://arxiv.org/abs/2209.07089) - **[NeurIPS 2022]**
-[Effects of Safety State Augmentation on Safe Exploration (Simmer)](https://
-arxiv.org/abs/2206.02675) - **[NeurIPS 2022]** [Model-based Safe Deep
-Reinforcement Learning via a Constrained Proximal Policy Optimization
-Algorithm](https://arxiv.org/abs/2210.07573) - **[ICML 2022]** [SautÃ© RL:
-Almost Surely Safe Reinforcement Learning Using State Augmentation (SauteRL)]
-(https://arxiv.org/abs/2202.06558) - **[IJCAI 2022]** [Penalized Proximal
-Policy Optimization for Safe Reinforcement Learning](https://arxiv.org/abs/
-2205.11814) - **[AAAI 2022]** [Conservative and Adaptive Penalty for Model-
-Based Safe Reinforcement Learning (CAP)](https://arxiv.org/abs/2112.07701) LLiisstt
-ooff AAllggoorriitthhmmss OOnn PPoolliiccyy SSaaffeeRRLL - [x] [The Lagrange version of PPO (PPO-Lag)]
-(https://cdn.openai.com/safexp-short.pdf) - [x] [The Lagrange version of TRPO
-(TRPO-Lag)](https://cdn.openai.com/safexp-short.pdf) - [x] **[ICML 2017]**
-[Constrained Policy Optimization (CPO)](https://proceedings.mlr.press/v70/
-achiam17a) - [x] **[ICLR 2019]** [Reward Constrained Policy Optimization
-(RCPO)](https://openreview.net/forum?id=SkfrvsA9FX) - [x] **[ICML 2020]**
-[Responsive Safety in Reinforcement Learning by PID Lagrangian Methods (PID-
-Lag)](https://arxiv.org/abs/2007.03964) - [x] **[NeurIPS 2020]** [First Order
-Constrained Optimization in Policy Space (FOCOPS)](https://arxiv.org/abs/
-2002.06506) - [x] **[AAAI 2020]** [IPO: Interior-point Policy Optimization
-under Constraints (IPO)](https://arxiv.org/abs/1910.09615) - [x] **[ICLR
-2020]** [Projection-Based Constrained Policy Optimization (PCPO)](https://
-openreview.net/forum?id=rke3TJrtPS) - [x] **[ICML 2021]** [CRPO: A New Approach
-for Safe Reinforcement Learning with Convergence Guarantee](https://arxiv.org/
-abs/2011.05869) - [x] **[IJCAI 2022]** [Penalized Proximal Policy Optimization
-for Safe Reinforcement Learning(P3O)](https://arxiv.org/pdf/2205.11814.pdf) OOffff
-PPoolliiccyy SSaaffeeRRLL - **[Preprint 2019]** [The Lagrangian version of DDPG (DDPGLag)]
-(https://cdn.openai.com/safexp-short.pdf) - **[Preprint 2019]** [The Lagrangian
-version of TD3 (TD3Lag)](https://cdn.openai.com/safexp-short.pdf) - **[Preprint
-2019]** [The Lagrangian version of SAC (SACLag)](https://cdn.openai.com/safexp-
-short.pdf) - **[ICML 2020]** [Responsive Safety in Reinforcement Learning by
-PID Lagrangian Methods (DDPGPID)](https://arxiv.org/abs/2007.03964) - **[ICML
-2020]** [Responsive Safety in Reinforcement Learning by PID Lagrangian Methods
-(TD3PID)](https://arxiv.org/abs/2007.03964) - **[ICML 2020]** [Responsive
-Safety in Reinforcement Learning by PID Lagrangian Methods (SACPID)](https://
-arxiv.org/abs/2007.03964) MMooddeell--BBaasseedd SSaaffeeRRLL - [ ] **[NeurIPS 2021]** [Safe
-Reinforcement Learning by Imagining the Near Future (SMBPO)](https://arxiv.org/
-abs/2202.07789) - [x] **[CoRL 2021 (Oral)]** [Learning Off-Policy with Online
-Planning (SafeLOOP)](https://arxiv.org/abs/2008.10066) - [x] **[AAAI 2022]**
+[Supported Environments](#supported-environments) - [Customizing your
+environment](#customizing-your-environment) - [Try with CLI](#try-with-cli) -
+[Getting Started](#getting-started) - [Important Hints](#important-hints) -
+[Quickstart: Colab on the Cloud](#quickstart-colab-on-the-cloud) - [Changelog]
+(#changelog) - [Citing OmniSafe](#citing-omnisafe) - [Publications using
+OmniSafe](#publications-using-omnisafe) - [The OmniSafe Team](#the-omnisafe-
+team) - [License](#license) ---------------------------------------------------
+----------------------------- ## Quick Start ### Installation ####
+Prerequisites OmniSafe requires Python 3.8+ and PyTorch 1.10+. > We support and
+test for Python 3.8, 3.9, 3.10 on Linux. Meanwhile, we also support M1 and M2
+versions of macOS. We will accept PRs related to Windows, but do not officially
+support it. #### Install from source ```bash # Clone the repo git clone https:/
+/github.com/PKU-Alignment/omnisafe.git cd omnisafe # Create a conda environment
+conda env create --file conda-recipe.yaml conda activate omnisafe # Install
+omnisafe pip install -e . ``` #### Install from PyPI OmniSafe is hosted in [!
+[PyPI](https://img.shields.io/pypi/v/omnisafe?label=pypi&logo=pypi)](https://
+pypi.org/project/omnisafe) / ![Status](https://img.shields.io/pypi/status/
+omnisafe?label=status). ```bash pip install omnisafe ``` ## Implemented
+Algorithms LLaatteesstt SSaaffeeRRLL PPaappeerrss - **[AAAI 2023]** Augmented Proximal Policy
+Optimization for Safe Reinforcement Learning (APPO) - **[NeurIPS 2022]**
+[Constrained Update Projection Approach to Safe Policy Optimization (CUP)]
+(https://arxiv.org/abs/2209.07089) - **[NeurIPS 2022]** [Effects of Safety
+State Augmentation on Safe Exploration (Simmer)](https://arxiv.org/abs/
+2206.02675) - **[NeurIPS 2022]** [Model-based Safe Deep Reinforcement Learning
+via a Constrained Proximal Policy Optimization Algorithm](https://arxiv.org/
+abs/2210.07573) - **[ICML 2022]** [SautÃ© RL: Almost Surely Safe Reinforcement
+Learning Using State Augmentation (SauteRL)](https://arxiv.org/abs/2202.06558)
+- **[IJCAI 2022]** [Penalized Proximal Policy Optimization for Safe
+Reinforcement Learning](https://arxiv.org/abs/2205.11814) - **[AAAI 2022]**
 [Conservative and Adaptive Penalty for Model-Based Safe Reinforcement Learning
-(CAP)](https://arxiv.org/abs/2112.07701) - [x] **[NeurIPS 2022]** [Model-based
-Safe Deep Reinforcement Learning via a Constrained Proximal Policy Optimization
+(CAP)](https://arxiv.org/abs/2112.07701) LLiisstt ooff AAllggoorriitthhmmss OOnn PPoolliiccyy SSaaffeeRRLL -
+[x] [The Lagrange version of PPO (PPO-Lag)](https://cdn.openai.com/safexp-
+short.pdf) - [x] [The Lagrange version of TRPO (TRPO-Lag)](https://
+cdn.openai.com/safexp-short.pdf) - [x] **[ICML 2017]** [Constrained Policy
+Optimization (CPO)](https://proceedings.mlr.press/v70/achiam17a) - [x] **[ICLR
+2019]** [Reward Constrained Policy Optimization (RCPO)](https://openreview.net/
+forum?id=SkfrvsA9FX) - [x] **[ICML 2020]** [Responsive Safety in Reinforcement
+Learning by PID Lagrangian Methods (PID-Lag)](https://arxiv.org/abs/2007.03964)
+- [x] **[NeurIPS 2020]** [First Order Constrained Optimization in Policy Space
+(FOCOPS)](https://arxiv.org/abs/2002.06506) - [x] **[AAAI 2020]** [IPO:
+Interior-point Policy Optimization under Constraints (IPO)](https://arxiv.org/
+abs/1910.09615) - [x] **[ICLR 2020]** [Projection-Based Constrained Policy
+Optimization (PCPO)](https://openreview.net/forum?id=rke3TJrtPS) - [x] **[ICML
+2021]** [CRPO: A New Approach for Safe Reinforcement Learning with Convergence
+Guarantee](https://arxiv.org/abs/2011.05869) - [x] **[IJCAI 2022]** [Penalized
+Proximal Policy Optimization for Safe Reinforcement Learning(P3O)](https://
+arxiv.org/pdf/2205.11814.pdf) OOffff PPoolliiccyy SSaaffeeRRLL - **[Preprint 2019]** [The
+Lagrangian version of DDPG (DDPGLag)](https://cdn.openai.com/safexp-short.pdf)
+- **[Preprint 2019]** [The Lagrangian version of TD3 (TD3Lag)](https://
+cdn.openai.com/safexp-short.pdf) - **[Preprint 2019]** [The Lagrangian version
+of SAC (SACLag)](https://cdn.openai.com/safexp-short.pdf) - **[ICML 2020]**
+[Responsive Safety in Reinforcement Learning by PID Lagrangian Methods
+(DDPGPID)](https://arxiv.org/abs/2007.03964) - **[ICML 2020]** [Responsive
+Safety in Reinforcement Learning by PID Lagrangian Methods (TD3PID)](https://
+arxiv.org/abs/2007.03964) - **[ICML 2020]** [Responsive Safety in Reinforcement
+Learning by PID Lagrangian Methods (SACPID)](https://arxiv.org/abs/2007.03964)
+MMooddeell--BBaasseedd SSaaffeeRRLL - [ ] **[NeurIPS 2021]** [Safe Reinforcement Learning by
+Imagining the Near Future (SMBPO)](https://arxiv.org/abs/2202.07789) - [x] **
+[CoRL 2021 (Oral)]** [Learning Off-Policy with Online Planning (SafeLOOP)]
+(https://arxiv.org/abs/2008.10066) - [x] **[AAAI 2022]** [Conservative and
+Adaptive Penalty for Model-Based Safe Reinforcement Learning (CAP)](https://
+arxiv.org/abs/2112.07701) - [x] **[NeurIPS 2022]** [Model-based Safe Deep
+Reinforcement Learning via a Constrained Proximal Policy Optimization
 Algorithm](https://arxiv.org/abs/2210.07573) - [ ] **[ICLR 2022]** [Constrained
 Policy Optimization via Bayesian World Models (LA-MBDA)](https://arxiv.org/abs/
 2201.09802) - [x] **[ICML 2022 Workshop]** [Constrained Model-based
 Reinforcement Learning with Robust Cross-Entropy Method (RCE)](https://
 arxiv.org/abs/2010.07968) - [x] **[NeurIPS 2018]** [Constrained Cross-Entropy
 Method for Safe Reinforcement Learning (CCE)](https://proceedings.neurips.cc/
 paper/2018/hash/34ffeb359a192eb8174b6854643cc046-Abstract.html) OOfffflliinnee SSaaffeeRRLL
@@ -182,60 +197,92 @@
 |Safe Navigation|_B_u_t_t_o_n_[_0_1_2_]|Point, Car, Racecar, Ant|SafetyPointGoal1-v0    |
 |               |_P_u_s_h_[_0_1_2_]_ _ |                        |                       |
 |_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_C_i_r_c_l_e_[_0_1_2_]_|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |               |           |HalfCheetah, Hopper,    |SafetyHumanoidVelocity-|
 |Safe Velocity  |Velocity   |Swimmer, Walker2d, Ant, |v1                     |
 |_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _|_H_u_m_a_n_o_i_d_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 For more information about environments, please refer to [Safety-Gymnasium]
-(https://www.safety-gymnasium.com). #### Try with CLI ```bash pip install
-omnisafe omnisafe --help # Ask for help omnisafe benchmark --help # The
-benchmark also can be replaced with 'eval', 'train', 'train-config' # Quick
-benchmarking for your research, just specify: # 1. exp_name # 2. num_pool(how
-much processes are concurrent) # 3. path of the config file (refer to omnisafe/
-examples/benchmarks for format) # Here we provide an exampe in ./tests/
-saved_source. # And you can set your benchmark_config.yaml by following it
-omnisafe benchmark test_benchmark 2 ./tests/saved_source/benchmark_config.yaml
-# Quick evaluating and rendering your trained policy, just specify: # 1. path
-of algorithm which you trained omnisafe eval ./tests/saved_source/PPO-
-{SafetyPointGoal1-v0} --num-episode 1 # Quick training some algorithms to
-validate your thoughts # Note: use `key1:key2`, your can select key of
-hyperparameters which are recursively contained, and use `--custom-cfgs`, you
-can add custom cfgs via CLI omnisafe train --algo PPO --total-steps 2048 --
-vector-env-nums 1 --custom-cfgs algo_cfgs:steps_per_epoch --custom-cfgs 1024 #
-Quick training some algorithms via a saved config file, the format is as same
-as default format omnisafe train-config ./tests/saved_source/train_config.yaml
-``` ---------------------------------------------------------------------------
------ ## Getting Started ### Important Hints We have provided benchmark results
-for various algorithms, including on-policy, off-policy, model-based, and
-offline approaches, along with parameter tuning analysis. Please refer to the
-following: - [On-Policy](./benchmarks/on-policy/) - [Off-Policy](./benchmarks/
-off-policy/) - [Model-based](./benchmarks/model-based/) - [Offline](./
-benchmarks/offline/) ### Quickstart: Colab on the Cloud Explore OmniSafe easily
-and quickly through a series of Google Colab notebooks: - [Getting Started]
+(https://www.safety-gymnasium.com). #### Customizing your environment We offer
+a flexible customized environment interface that allows users to achieve the
+following **without modifying the OmniSafe source code**: - Use OmniSafe to
+train algorithms on customized environments. - Create the the environment with
+specified personalized parameters. - Complete the recording of environment-
+specific information in Logger. We provide **step-by-step tutorials** on
+[Environment Customization From Scratch](https://colab.research.google.com/
+github/PKU-Alignment/omnisafe/blob/main/tutorials/English/
+3.Environment%20Customization%20from%20Scratch.ipynb) and [Environment
+Customization From Community](https://colab.research.google.com/github/PKU-
+Alignment/omnisafe/blob/main/tutorials/English/
+4.Environment%20Customization%20from%20Community.ipynb) to give you a detailed
+introduction on how to use this extraordinary feature of OmniSafe. *Note: If
+you find trouble customizing your environment, please feel free to open an
+[issue](https://github.com/PKU-Alignment/omnisafe/issues) or [discussion]
+(https://github.com/PKU-Alignment/omnisafe/discussions). [Pull requests](https:
+//github.com/PKU-Alignment/omnisafe/pulls) are also welcomed if you're willing
+to contribute the implementation of your environments interface.* #### Try with
+CLI ```bash pip install omnisafe omnisafe --help # Ask for help omnisafe
+benchmark --help # The benchmark also can be replaced with 'eval', 'train',
+'train-config' # Quick benchmarking for your research, just specify: # 1.
+exp_name # 2. num_pool(how much processes are concurrent) # 3. path of the
+config file (refer to omnisafe/examples/benchmarks for format) # Here we
+provide an exampe in ./tests/saved_source. # And you can set your
+benchmark_config.yaml by following it omnisafe benchmark test_benchmark 2 ./
+tests/saved_source/benchmark_config.yaml # Quick evaluating and rendering your
+trained policy, just specify: # 1. path of algorithm which you trained omnisafe
+eval ./tests/saved_source/PPO-{SafetyPointGoal1-v0} --num-episode 1 # Quick
+training some algorithms to validate your thoughts # Note: use `key1:key2`,
+your can select key of hyperparameters which are recursively contained, and use
+`--custom-cfgs`, you can add custom cfgs via CLI omnisafe train --algo PPO --
+total-steps 2048 --vector-env-nums 1 --custom-cfgs algo_cfgs:steps_per_epoch --
+custom-cfgs 1024 # Quick training some algorithms via a saved config file, the
+format is as same as default format omnisafe train-config ./tests/saved_source/
+train_config.yaml ``` ---------------------------------------------------------
+----------------------- ## Getting Started ### Important Hints We have provided
+benchmark results for various algorithms, including on-policy, off-policy,
+model-based, and offline approaches, along with parameter tuning analysis.
+Please refer to the following: - [On-Policy](./benchmarks/on-policy/) - [Off-
+Policy](./benchmarks/off-policy/) - [Model-based](./benchmarks/model-based/) -
+[Offline](./benchmarks/offline/) ### Quickstart: Colab on the Cloud Explore
+OmniSafe easily and quickly through a series of Google Colab notebooks: -
+[Getting Started](https://colab.research.google.com/github/PKU-Alignment/
+omnisafe/blob/main/tutorials/English/1.Getting_Started.ipynb) Introduce the
+basic usage of OmniSafe so that users can quickly hand it. - [CLI Command]
 (https://colab.research.google.com/github/PKU-Alignment/omnisafe/blob/main/
-tutorials/English/1.Getting_Started.ipynb) Introduce the basic usage of
-OmniSafe so that users can quickly hand it. - [CLI Command](https://
-colab.research.google.com/github/PKU-Alignment/omnisafe/blob/main/tutorials/
-English/2.CLI_Command.ipynb) Introduce how to use the CLI tool of OmniSafe. We
-take great pleasure in collaborating with our users to create tutorials in
-various languages. Please refer to our list of currently supported languages.
-If you are interested in translating the tutorial into a new language or
-improving an existing version, kindly submit a PR to us. ----------------------
----------------------------------------------------------- ## Changelog See
-[CHANGELOG.md](https://github.com/PKU-Alignment/omnisafe/blob/main/
-CHANGELOG.md). ## Citing OmniSafe If you find OmniSafe useful or use OmniSafe
-in your research, please cite it in your publications. ```bibtex @article
-{omnisafe, title = {OmniSafe: An Infrastructure for Accelerating Safe
+tutorials/English/2.CLI_Command.ipynb) Introduce how to use the CLI tool of
+OmniSafe. We take great pleasure in collaborating with our users to create
+tutorials in various languages. Please refer to our list of currently supported
+languages. If you are interested in translating the tutorial into a new
+language or improving an existing version, kindly submit a PR to us. ----------
+---------------------------------------------------------------------- ##
+Changelog See [CHANGELOG.md](https://github.com/PKU-Alignment/omnisafe/blob/
+main/CHANGELOG.md). ## Citing OmniSafe If you find OmniSafe useful or use
+OmniSafe in your research, please cite it in your publications. ```bibtex
+@article{omnisafe, title = {OmniSafe: An Infrastructure for Accelerating Safe
 Reinforcement Learning Research}, author = {Jiaming Ji, Jiayi Zhou, Borong
 Zhang, Juntao Dai, Xuehai Pan, Ruiyang Sun, Weidong Huang, Yiran Geng, Mickel
 Liu, Yaodong Yang}, journal = {arXiv preprint arXiv:2305.09304}, year = {2023}
-} ``` ## The OmniSafe Team OmniSafe is mainly developed by the SafeRL research
-team directed by Prof. [Yaodong Yang](https://www.yangyaodong.com/). Our SafeRL
-research team members include [Borong Zhang](https://github.com/muchvo), [Jiayi
-Zhou](https://github.com/Gaiejj), [JTao Dai](https://github.com/calico-1226),
-[Weidong Huang](https://github.com/hdadong), [Ruiyang Sun](https://github.com/
-rockmagma02), [Xuehai Pan](https://github.com/XuehaiPan) and [Jiaming Ji]
-(https://github.com/zmsn-2077). If you have any questions in the process of
-using OmniSafe, don't hesitate to ask your questions on [the GitHub issue page]
-(https://github.com/PKU-Alignment/omnisafe/issues/new/choose), we will reply to
-you in 2-3 working days. ## License OmniSafe is released under Apache License
-2.0.
+} ``` ## Publications using OmniSafe We have compiled a list of papers that use
+OmniSafe for algorithm implementation or experimentation. If you are willing to
+include your work in this list, or if you wish to have your implementation
+officially integrated into OmniSafe, please feel free to [contact us](https://
+github.com/PKU-Alignment/omnisafe/issues). | Papers | Publisher| |:---:|:---:
+| | [Off-Policy Primal-Dual Safe Reinforcement Learning](https://
+openreview.net/pdf?id=vy42bYs1Wo) | ICLR 2024 | | [Safe Offline Reinforcement
+Learning with Feasibility-Guided Diffusion Model](https://openreview.net/
+pdf?id=j5JvZCaDM0) | ICLR 2024 | | [Iterative Reachability Estimation for Safe
+Reinforcement Learning](https://proceedings.neurips.cc/paper_files/paper/2023/
+file/dca63f2650fe9e88956c1b68440b8ee9-Paper-Conference.pdf) | NeurIPS 2023 | |
+[Balance Reward and Safety Optimization for Safe Reinforcement Learning: A
+Perspective of Gradient Manipulation](https://ojs.aaai.org/index.php/AAAI/
+article/view/30102/31944) | AAAI 2024 | | [Learning Safety Constraints From
+Demonstration Using One-Class Decision Trees](https://openreview.net/
+pdf?id=dxUi16pvub) | AAAI 2024 WorkShops | ## The OmniSafe Team OmniSafe is
+mainly developed by the SafeRL research team directed by Prof. [Yaodong Yang]
+(https://www.yangyaodong.com/). Our SafeRL research team members include
+[Borong Zhang](https://github.com/muchvo), [Jiayi Zhou](https://github.com/
+Gaiejj), [JTao Dai](https://github.com/calico-1226), [Weidong Huang](https://
+github.com/hdadong), [Ruiyang Sun](https://github.com/rockmagma02), [Xuehai
+Pan](https://github.com/XuehaiPan) and [Jiaming Ji](https://github.com/zmsn-
+2077). If you have any questions in the process of using OmniSafe, don't
+hesitate to ask your questions on [the GitHub issue page](https://github.com/
+PKU-Alignment/omnisafe/issues/new/choose), we will reply to you in 2-3 working
+days. ## License OmniSafe is released under Apache License 2.0.
```

### Comparing `omnisafe-0.5.0b0/omnisafe.egg-info/SOURCES.txt` & `omnisafe-0.5.1b0/omnisafe.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -153,14 +153,15 @@
 omnisafe/configs/on-policy/TRPOEarlyTerminated.yaml
 omnisafe/configs/on-policy/TRPOLag.yaml
 omnisafe/configs/on-policy/TRPOPID.yaml
 omnisafe/configs/on-policy/TRPOSaute.yaml
 omnisafe/configs/on-policy/TRPOSimmerPID.yaml
 omnisafe/envs/__init__.py
 omnisafe/envs/core.py
+omnisafe/envs/custom_env.py
 omnisafe/envs/mujoco_env.py
 omnisafe/envs/safety_gymnasium_env.py
 omnisafe/envs/safety_gymnasium_modelbased.py
 omnisafe/envs/wrapper.py
 omnisafe/models/__init__.py
 omnisafe/models/base.py
 omnisafe/models/actor/__init__.py
```

### Comparing `omnisafe-0.5.0b0/pyproject.toml` & `omnisafe-0.5.1b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "tensorboard >= 2.8.0",
     "wandb >= 0.13.0",
     "pyyaml >= 6.0",
     "moviepy >= 1.0.0",
     "typing-extensions >= 4.0.0",
     "typer[all] >= 0.7.0",
     "seaborn >= 0.12.2",
-    "pandas >=  1.5.3",
+    "pandas == 2.0.3",
     "matplotlib >= 3.7.1",
     "gdown >= 4.6.0"
 ]
 dynamic = ["version", "entry-points"]
 
 [project.urls]
 Homepage = "https://github.com/PKU-Alignment/omnisafe"
```

### Comparing `omnisafe-0.5.0b0/setup.py` & `omnisafe-0.5.1b0/setup.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/tests/test_buffer.py` & `omnisafe-0.5.1b0/tests/test_buffer.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/tests/test_cli.py` & `omnisafe-0.5.1b0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/tests/test_ensemble.py` & `omnisafe-0.5.1b0/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/tests/test_env.py` & `omnisafe-0.5.1b0/tests/test_env.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Test envs."""
 
+import torch
 from gymnasium.spaces import Box
 
 import helpers
 from omnisafe.envs.core import make
 
 
 @helpers.parametrize(
@@ -37,15 +38,15 @@
     env.set_seed(0)
     obs, _ = env.reset()
     if num_envs > 1:
         assert obs.shape == (num_envs, obs_space.shape[0])
     else:
         assert obs.shape == (obs_space.shape[0],)
 
-    act = env.sample_action()
+    act = torch.zeros(env.action_space.shape, dtype=torch.float32)
     if num_envs > 1:
         act = act.repeat(num_envs, 1)
 
     obs, reward, cost, terminated, truncated, info = env.step(act)
 
     if num_envs > 1:
         assert obs.shape == (num_envs, obs_space.shape[0])
@@ -89,15 +90,15 @@
     obs, _ = env.reset()
     # env.render()
     if num_envs > 1:
         assert obs.shape == (num_envs, obs_space.shape[0])
     else:
         assert obs.shape == (obs_space.shape[0],)
 
-    act = env.sample_action()
+    act = torch.zeros(env.action_space.shape, dtype=torch.float32)
     if num_envs > 1:
         act = act.repeat(num_envs, 1)
 
     obs, reward, cost, terminated, truncated, info = env.step(act)
 
     assert obs.shape == (obs_space.shape[0],)
     assert reward.shape == ()
@@ -131,15 +132,15 @@
     # env.render()
 
     if num_envs > 1:
         assert obs.shape == (num_envs, obs_space.shape[0])
     else:
         assert obs.shape == (obs_space.shape[0],)
 
-    act = env.sample_action()
+    act = torch.zeros(env.action_space.shape, dtype=torch.float32)
     if num_envs > 1:
         act = act.repeat(num_envs, 1)
 
     obs, reward, cost, terminated, truncated, info = env.step(act)
 
     assert obs.shape == (obs_space.shape[0],)
     assert reward.shape == ()
```

### Comparing `omnisafe-0.5.0b0/tests/test_experiment_grid.py` & `omnisafe-0.5.1b0/tests/test_experiment_grid.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/tests/test_model.py` & `omnisafe-0.5.1b0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/tests/test_normalizer.py` & `omnisafe-0.5.1b0/tests/test_normalizer.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/tests/test_offline_data.py` & `omnisafe-0.5.1b0/tests/test_offline_data.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/tests/test_policy.py` & `omnisafe-0.5.1b0/tests/test_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 }
 
 optim_case = [0, 1, 2, 3, 4]
 
 
 @helpers.parametrize(optim_case=optim_case)
 def test_cpo(optim_case):
-    agent = omnisafe.Agent('CPO', 'Simple-v0', custom_cfgs={})
+    agent = omnisafe.Agent('CPO', 'Test-v0', custom_cfgs={})
     b_grads = torch.Tensor([1])
     ep_costs = torch.Tensor([-1])
     r = torch.Tensor([0])
     q = torch.Tensor([0])
     s = torch.Tensor([1])
     p = torch.Tensor([1])
     xHx = torch.Tensor([1])
@@ -109,15 +109,15 @@
         loss_reward_before=loss_reward_before,
         loss_cost_before=loss_cost_before,
     )
 
 
 def test_assertion_error():
     """Test base algorithms."""
-    env_id = 'Simple-v0'
+    env_id = 'Test-v0'
     custom_cfgs = {
         'train_cfgs': {
             'total_steps': 200,
             'vector_env_nums': 1,
             'torch_threads': 4,
         },
         'algo_cfgs': {
@@ -159,15 +159,15 @@
     with pytest.raises(AssertionError):
         custom_cfgs = [1, 2, 3]
         agent = omnisafe.Agent('PPO', env_id, custom_cfgs=custom_cfgs)
 
 
 def test_render():
     """Test render image"""
-    env_id = 'Simple-v0'
+    env_id = 'Test-v0'
     custom_cfgs = {
         'train_cfgs': {
             'total_steps': 200,
             'vector_env_nums': 1,
             'torch_threads': 4,
         },
         'algo_cfgs': {
@@ -184,15 +184,15 @@
     agent.learn()
     agent.render(num_episodes=1, render_mode='rgb_array')
 
 
 @helpers.parametrize(algo=['PETS', 'CCEPETS', 'CAPPETS', 'RCEPETS'])
 def test_cem_based(algo):
     """Test model_based algorithms."""
-    env_id = 'Simple-v0'
+    env_id = 'Test-v0'
 
     custom_cfgs = {
         'train_cfgs': {
             'total_steps': 200,
             'vector_env_nums': 1,
             'torch_threads': 4,
         },
@@ -228,15 +228,15 @@
     agent.learn()
     agent.render()
 
 
 @helpers.parametrize(algo=['LOOP', 'SafeLOOP'])
 def test_loop(algo):
     """Test model_based algorithms."""
-    env_id = 'Simple-v0'
+    env_id = 'Test-v0'
 
     custom_cfgs = {
         'train_cfgs': {
             'total_steps': 200,
             'vector_env_nums': 1,
             'torch_threads': 4,
         },
@@ -277,15 +277,15 @@
     agent = omnisafe.Agent(algo, env_id, custom_cfgs=custom_cfgs)
     agent.learn()
 
 
 @helpers.parametrize(algo=off_base)
 def test_off_policy(algo):
     """Test base algorithms."""
-    env_id = 'Simple-v0'
+    env_id = 'Test-v0'
     custom_cfgs = {
         'train_cfgs': {
             'total_steps': 200,
             'vector_env_nums': 1,
             'torch_threads': 4,
         },
         'algo_cfgs': {
@@ -306,15 +306,15 @@
     agent = omnisafe.Agent(algo, env_id, custom_cfgs=custom_cfgs)
     agent.learn()
 
 
 @helpers.parametrize(algo=off_lag)
 def test_off_lag_policy(algo):
     """Test base algorithms."""
-    env_id = 'Simple-v0'
+    env_id = 'Test-v0'
     custom_cfgs = {
         'train_cfgs': {
             'total_steps': 200,
             'vector_env_nums': 1,
             'torch_threads': 4,
         },
         'algo_cfgs': {
@@ -339,15 +339,15 @@
 
 auto_alpha = [True, False]
 
 
 @helpers.parametrize(auto_alpha=auto_alpha)
 def test_sac_policy(auto_alpha):
     """Test sac algorithms."""
-    env_id = 'Simple-v0'
+    env_id = 'Test-v0'
     custom_cfgs = {
         'train_cfgs': {
             'total_steps': 200,
             'vector_env_nums': 1,
             'torch_threads': 4,
         },
         'algo_cfgs': {
@@ -370,15 +370,15 @@
 
 auto_alpha = [True, False]
 
 
 @helpers.parametrize(auto_alpha=auto_alpha, algo=sac_lag)
 def test_sac_lag_policy(auto_alpha, algo):
     """Test sac algorithms."""
-    env_id = 'Simple-v0'
+    env_id = 'Test-v0'
     custom_cfgs = {
         'train_cfgs': {
             'total_steps': 200,
             'vector_env_nums': 1,
             'torch_threads': 4,
         },
         'algo_cfgs': {
@@ -411,15 +411,15 @@
         + saute_policy
         + simmer_policy
         + early_terminated_policy
     ),
 )
 def test_on_policy(algo):
     """Test base algorithms."""
-    env_id = 'Simple-v0'
+    env_id = 'Test-v0'
     custom_cfgs = {
         'train_cfgs': {
             'total_steps': 200,
             'vector_env_nums': 1,
             'torch_threads': 4,
         },
         'algo_cfgs': {
@@ -434,15 +434,15 @@
     agent = omnisafe.Agent(algo, env_id, custom_cfgs=custom_cfgs)
     agent.learn()
 
 
 @helpers.parametrize(algo=pid_lagrange_policy)
 def test_pid(algo):
     """Test pid algorithms."""
-    env_id = 'Simple-v0'
+    env_id = 'Test-v0'
     custom_cfgs = {
         'train_cfgs': {
             'total_steps': 200,
             'vector_env_nums': 1,
             'torch_threads': 4,
         },
         'algo_cfgs': {
@@ -462,16 +462,16 @@
 
 
 @helpers.parametrize(
     algo=(offline_policy),
 )
 def test_offline(algo):
     """Test base algorithms."""
-    env_id = 'Simple-v0'
-    dataset = os.path.join(os.path.dirname(__file__), 'saved_source', 'Simple-v0.npz')
+    env_id = 'Test-v0'
+    dataset = os.path.join(os.path.dirname(__file__), 'saved_source', 'Test-v0.npz')
     custom_cfgs = {
         'train_cfgs': {
             'total_steps': 4,
             'torch_threads': 4,
             'dataset': dataset,
         },
         'algo_cfgs': {
@@ -484,16 +484,16 @@
 
 
 @helpers.parametrize(
     fn_type=['softchi', 'chisquare'],
 )
 def test_coptidice(fn_type):
     """Test coptidice algorithms."""
-    env_id = 'Simple-v0'
-    dataset = os.path.join(os.path.dirname(__file__), 'saved_source', 'Simple-v0.npz')
+    env_id = 'Test-v0'
+    dataset = os.path.join(os.path.dirname(__file__), 'saved_source', 'Test-v0.npz')
     custom_cfgs = {
         'train_cfgs': {
             'total_steps': 4,
             'torch_threads': 4,
             'dataset': dataset,
         },
         'algo_cfgs': {
@@ -505,15 +505,15 @@
     agent = omnisafe.Agent('COptiDICE', env_id, custom_cfgs=custom_cfgs)
     agent.learn()
 
 
 @helpers.parametrize(algo=['PPO', 'SAC', 'PPOLag'])
 def test_workflow_for_training(algo):
     """Test base algorithms."""
-    env_id = 'Simple-v0'
+    env_id = 'Test-v0'
     custom_cfgs = {
         'train_cfgs': {
             'total_steps': 200,
             'vector_env_nums': 1,
             'torch_threads': 4,
         },
         'algo_cfgs': {
@@ -532,15 +532,15 @@
     agent.plot(smooth=2)
     # agent.render(num_episodes=1, render_mode='rgb_array', width=1, height=1)
     agent.evaluate(num_episodes=1)
 
 
 def test_std_anealing():
     """Test std_anealing."""
-    env_id = 'Simple-v0'
+    env_id = 'Test-v0'
     custom_cfgs = {
         'train_cfgs': {
             'total_steps': 200,
             'vector_env_nums': 1,
         },
         'algo_cfgs': {
             'steps_per_epoch': 100,
```

### Comparing `omnisafe-0.5.0b0/tests/test_registry.py` & `omnisafe-0.5.1b0/tests/test_registry.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,21 +13,40 @@
 # limitations under the License.
 # ==============================================================================
 """Test registry."""
 
 import pytest
 
 from omnisafe.algorithms.registry import Registry
+from omnisafe.envs.core import CMDP, env_register, env_unregister
 
 
 class TestRegistry:
     name: str = 'test'
     idx: int = 0
 
 
 def test_with_error() -> None:
     registry = Registry('test')
     TestRegistry()
     with pytest.raises(TypeError):
         registry.register('test')
     with pytest.raises(KeyError):
         registry.get('test')
+    with pytest.raises(TypeError):
+
+        @env_register
+        class TestEnv:
+            name: str = 'test'
+            idx: int = 0
+
+    with pytest.raises(ValueError):
+
+        @env_register
+        class CustomEnv(CMDP):
+            pass
+
+    @env_register
+    @env_unregister
+    @env_unregister
+    class CustomEnv(CMDP):  # noqa
+        _support_envs = ['Simple-v0']  # noqa
```

### Comparing `omnisafe-0.5.0b0/tests/test_statistics_tools.py` & `omnisafe-0.5.1b0/tests/test_statistics_tools.py`

 * *Files identical despite different names*

### Comparing `omnisafe-0.5.0b0/tests/test_utils.py` & `omnisafe-0.5.1b0/tests/test_utils.py`

 * *Files identical despite different names*

