# Comparing `tmp/gdm-concordia-1.2.0.tar.gz` & `tmp/gdm-concordia-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdm-concordia-1.2.0.tar", last modified: Mon Feb 12 14:47:05 2024, max compression
+gzip compressed data, was "gdm-concordia-1.3.0.tar", last modified: Sat May  4 18:13:24 2024, max compression
```

## Comparing `gdm-concordia-1.2.0.tar` & `gdm-concordia-1.3.0.tar`

### file list

```diff
@@ -1,103 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 14:47:05.409992 gdm-concordia-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-02-12 14:47:05.409992 gdm-concordia-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 14:47:05.397992 gdm-concordia-1.2.0/concordia/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 14:47:05.397992 gdm-concordia-1.2.0/concordia/agents/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/agents/basic_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 14:47:05.397992 gdm-concordia-1.2.0/concordia/associative_memory/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/associative_memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/associative_memory/associative_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/associative_memory/blank_memories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/associative_memory/embedder_st5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/associative_memory/formative_memories.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/associative_memory/importance_function.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 14:47:05.401992 gdm-concordia-1.2.0/concordia/clocks/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/clocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/clocks/game_clock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/clocks/game_clock_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 14:47:05.401992 gdm-concordia-1.2.0/concordia/components/
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 14:47:05.401992 gdm-concordia-1.2.0/concordia/components/agent/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/components/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/components/agent/characteristic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/components/agent/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/components/agent/observation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/components/agent/person_by_situation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/components/agent/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/components/agent/reflection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/components/agent/self_perception.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/components/agent/situation_perception.py
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/components/agent/somatic_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/components/constant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 14:47:05.401992 gdm-concordia-1.2.0/concordia/components/game_master/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/components/game_master/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11875 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/components/game_master/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/components/game_master/direct_effect.py
--rw-r--r--   0 runner    (1001) docker     (127)     9887 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/components/game_master/inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/components/game_master/player_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/components/game_master/player_status_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/components/game_master/relevant_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/components/game_master/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/components/game_master/time_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/components/report_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/components/sequential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 14:47:05.401992 gdm-concordia-1.2.0/concordia/document/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/document/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/document/document_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/document/interactive_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/document/interactive_document_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 14:47:05.405992 gdm-concordia-1.2.0/concordia/environment/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/environment/game_master.py
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/environment/game_mater_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 14:47:05.405992 gdm-concordia-1.2.0/concordia/environment/scenes/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/environment/scenes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/environment/scenes/conversation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 14:47:05.405992 gdm-concordia-1.2.0/concordia/language_model/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/language_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/language_model/gcloud_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/language_model/gemini_vertex_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/language_model/gpt_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/language_model/language_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/language_model/retry_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 14:47:05.405992 gdm-concordia-1.2.0/concordia/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/metrics/common_sense_morality.py
--rw-r--r--   0 runner    (1001) docker     (127)    16861 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/metrics/dass_questionnaire.py
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/metrics/goal_achievement.py
--rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/metrics/opinion_of_others.py
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/metrics/uncertainty_scale_question.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 14:47:05.405992 gdm-concordia-1.2.0/concordia/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9001 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/tests/concordia_integration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/tests/mock_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 14:47:05.405992 gdm-concordia-1.2.0/concordia/thought_chains/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/thought_chains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13815 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/thought_chains/thought_chains.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 14:47:05.405992 gdm-concordia-1.2.0/concordia/typing/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/typing/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/typing/clock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/typing/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/typing/game_master.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 14:47:05.405992 gdm-concordia-1.2.0/concordia/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/utils/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/utils/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/utils/measurements.py
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/utils/measurements_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/concordia/utils/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 14:47:05.409992 gdm-concordia-1.2.0/gdm_concordia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-02-12 14:47:05.000000 gdm-concordia-1.2.0/gdm_concordia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-02-12 14:47:05.000000 gdm-concordia-1.2.0/gdm_concordia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 14:47:05.000000 gdm-concordia-1.2.0/gdm_concordia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-02-12 14:47:05.000000 gdm-concordia-1.2.0/gdm_concordia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-12 14:47:05.000000 gdm-concordia-1.2.0/gdm_concordia.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 14:47:05.409992 gdm-concordia-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-02-12 14:47:04.000000 gdm-concordia-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.661701 gdm-concordia-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-04 18:13:24.661701 gdm-concordia-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.649701 gdm-concordia-1.3.0/concordia/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.649701 gdm-concordia-1.3.0/concordia/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/agents/basic_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.649701 gdm-concordia-1.3.0/concordia/associative_memory/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/associative_memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10285 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/associative_memory/associative_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/associative_memory/blank_memories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8830 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/associative_memory/formative_memories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/associative_memory/importance_function.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.653701 gdm-concordia-1.3.0/concordia/clocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/clocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/clocks/game_clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/clocks/game_clock_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.653701 gdm-concordia-1.3.0/concordia/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.653701 gdm-concordia-1.3.0/concordia/components/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/agent/all_similar_memories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/agent/characteristic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/agent/creative_reflection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/agent/dialectical_reflection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/agent/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/agent/observation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/agent/person_by_situation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/agent/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/agent/reflection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/agent/relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/agent/scheduled_hint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/agent/self_perception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/agent/situation_perception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/agent/somatic_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/constant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.657701 gdm-concordia-1.3.0/concordia/components/game_master/
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/game_master/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/game_master/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/game_master/current_scene.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/game_master/current_scene_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/game_master/direct_effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/game_master/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/game_master/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/game_master/player_status_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/game_master/relevant_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/game_master/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/game_master/time_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/report_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/components/sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.657701 gdm-concordia-1.3.0/concordia/document/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/document/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/document/document_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/document/interactive_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/document/interactive_document_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.657701 gdm-concordia-1.3.0/concordia/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12552 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/environment/game_master.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/environment/game_master_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.657701 gdm-concordia-1.3.0/concordia/environment/scenes/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/environment/scenes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/environment/scenes/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/environment/scenes/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.657701 gdm-concordia-1.3.0/concordia/language_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/language_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/language_model/gcloud_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/language_model/gemini_vertex_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/language_model/gpt_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/language_model/language_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/language_model/ollama_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/language_model/retry_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.657701 gdm-concordia-1.3.0/concordia/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/metrics/common_sense_morality.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16861 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/metrics/dass_questionnaire.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/metrics/goal_achievement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/metrics/opinion_of_others.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/metrics/uncertainty_scale_question.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.661701 gdm-concordia-1.3.0/concordia/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/tests/concordia_integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/tests/mock_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.661701 gdm-concordia-1.3.0/concordia/thought_chains/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/thought_chains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16377 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/thought_chains/thought_chains.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.661701 gdm-concordia-1.3.0/concordia/typing/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/typing/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/typing/clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/typing/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/typing/game_master.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/typing/scene.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.661701 gdm-concordia-1.3.0/concordia/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/utils/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/utils/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/utils/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/utils/measurements_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/concordia/utils/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:13:24.661701 gdm-concordia-1.3.0/gdm_concordia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-04 18:13:24.000000 gdm-concordia-1.3.0/gdm_concordia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-04 18:13:24.000000 gdm-concordia-1.3.0/gdm_concordia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 18:13:24.000000 gdm-concordia-1.3.0/gdm_concordia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-04 18:13:24.000000 gdm-concordia-1.3.0/gdm_concordia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-04 18:13:24.000000 gdm-concordia-1.3.0/gdm_concordia.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 18:13:24.661701 gdm-concordia-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-04 18:13:21.000000 gdm-concordia-1.3.0/setup.py
```

### Comparing `gdm-concordia-1.2.0/LICENSE` & `gdm-concordia-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/PKG-INFO` & `gdm-concordia-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdm-concordia
-Version: 1.2.0
+Version: 1.3.0
 Summary: A library for building a generative model of social interacions.
 Home-page: https://github.com/google-deepmind/concordia
 Author: DeepMind
 Author-email: noreply@google.com
 License: Apache 2.0
 Download-URL: https://github.com/google-deepmind/concordia/releases
 Keywords: multi-agent agent-based-simulation generative-agents python machine-learning
```

### Comparing `gdm-concordia-1.2.0/README.md` & `gdm-concordia-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/__init__.py` & `gdm-concordia-1.3.0/concordia/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/agents/__init__.py` & `gdm-concordia-1.3.0/concordia/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/agents/basic_agent.py` & `gdm-concordia-1.3.0/concordia/agents/basic_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -184,18 +184,21 @@
   def _maybe_update(self):
     next_update = self._last_update + self._update_interval
     if self._clock.now() >= next_update and not self._under_interrogation:
       self._update()
 
   def _update(self):
     self._last_update = self._clock.now()
+
     def _get_recursive_update_func(
-        comp: component.Component) -> Callable[[], None]:
-      return lambda: helper_functions.apply_recursively(comp,
-                                                        function_name='update')
+        comp: component.Component,
+    ) -> Callable[[], None]:
+      return lambda: helper_functions.apply_recursively(
+          comp, function_name='update'
+      )
 
     with concurrent.futures.ThreadPoolExecutor() as executor:
       for comp in self._components.values():
         executor.submit(_get_recursive_update_func(comp))
 
   def observe(self, observation: str):
     if observation and not self._under_interrogation:
@@ -243,14 +246,20 @@
       idx = prompt.multiple_choice_question(
           question=call_to_action, answers=action_spec.options
       )
       output = action_spec.options[idx]
     elif action_spec.output_type == 'FLOAT':
       raise NotImplementedError
 
+    def get_externality(externality):
+      return externality.update_after_event(output)
+
+    with concurrent.futures.ThreadPoolExecutor() as executor:
+      executor.map(get_externality, self._components.values())
+
     self._last_chain_of_thought = prompt.view().text().splitlines()
     current_log = {
         'date': self._clock.now(),
         'Action prompt': self._last_chain_of_thought,
     }
 
     for comp in self._components.values():
```

### Comparing `gdm-concordia-1.2.0/concordia/associative_memory/__init__.py` & `gdm-concordia-1.3.0/concordia/associative_memory/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/associative_memory/associative_memory.py` & `gdm-concordia-1.3.0/concordia/associative_memory/associative_memory.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,23 @@
 import datetime
 import threading
 
 import numpy as np
 import pandas as pd
 
 
+def _check_date_in_range(timestamp: datetime.datetime) -> None:
+  if timestamp < pd.Timestamp.min:
+    min_date = pd.Timestamp.min
+    raise ValueError(f'timestamp {timestamp} < pd.Timestamp.min {min_date}')
+  if timestamp > pd.Timestamp.max:
+    max_date = pd.Timestamp.max
+    raise ValueError(f'timestamp {timestamp} > pd.Timestamp.max {max_date}')
+
+
 class AssociativeMemory:
   """Class that implements associative memory."""
 
   def __init__(
       self,
       sentence_embedder: Callable[[str], np.ndarray],
       importance: Callable[[str], float],
@@ -51,55 +60,57 @@
     self._importance = importance
 
     self._memory_bank = pd.DataFrame(
         columns=['text', 'time', 'tags', 'embedding', 'importance']
     )
     self._clock_now = clock
     self._interval = clock_step_size
+    self._stored_hashes = set()
 
   def add(
       self,
       text: str,
       *,
       timestamp: datetime.datetime | None = None,
-      tags: list[str] | None = None,
+      tags: Iterable[str] = (),
       importance: float | None = None,
   ):
-    """Adds the text to the memory.
+    """Adds nonduplicated entries (time, text, tags, importance) to the memory.
 
     Args:
       text: what goes into the memory
       timestamp: the time of the memory
       tags: optional tags
       importance: optionally set the importance of the memory.
     """
-
-    embedding = self._embedder(text)
     if importance is None:
       importance = self._importance(text)
 
     if timestamp is None:
       timestamp = self._clock_now()
 
-    new_df = (
-        pd.Series({
-            'text': text,
-            'time': timestamp,
-            'tags': tags,
-            'embedding': embedding,
-            'importance': importance,
-        })
-        .to_frame()
-        .T
-    )
+    _check_date_in_range(timestamp)
+
+    contents = {
+        'text': text,
+        'time': timestamp,
+        'tags': tuple(tags),
+        'importance': importance,
+    }
+    hashed_contents = hash(contents.values())
+    derived = {'embedding': self._embedder(text)}
+    new_df = pd.Series(contents | derived).to_frame().T.infer_objects()
 
     with self._memory_bank_lock:
+      if hashed_contents in self._stored_hashes:
+        return
       self._memory_bank = pd.concat(
           [self._memory_bank, new_df], ignore_index=True
       )
+      self._stored_hashes.add(hashed_contents)
 
   def extend(
       self,
       texts: Iterable[str],
       **kwargs,
   ):
     """Adds the texts to the memory.
@@ -327,7 +338,16 @@
     """
     data = self._get_k_recent(k)
 
     return (
         self._pd_to_text(data, add_time=add_time, sort_by_time=True),
         list(data['importance']),
     )
+
+  def __len__(self):
+    """Returns the number of entries in the memory bank.
+
+    Since memories cannot be deleted, the length cannot decrease, and can be
+    used to check if the contents of the memory bank have changed.
+    """
+    with self._memory_bank_lock:
+      return len(self._memory_bank)
```

### Comparing `gdm-concordia-1.2.0/concordia/associative_memory/blank_memories.py` & `gdm-concordia-1.3.0/concordia/associative_memory/blank_memories.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/associative_memory/formative_memories.py` & `gdm-concordia-1.3.0/concordia/associative_memory/formative_memories.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,25 +14,27 @@
 
 
 """This is a factory for generating memories for concordia agents."""
 
 from collections.abc import Callable, Iterable, Sequence
 import dataclasses
 import datetime
+import logging
 import re
 from typing import Any
 from concordia.associative_memory import associative_memory
 from concordia.associative_memory import importance_function
 from concordia.document import interactive_document
 from concordia.language_model import language_model
 from dateutil.relativedelta import relativedelta  # pylint: disable=g-importing-member
 
+logger = logging.getLogger(__name__)
 
 DEFAULT_DOB = datetime.datetime(year=1984, month=7, day=3, hour=0, minute=0)
-DEFAULT_FORMATIVE_AGES = (3, 7, 12, 16, 21)
+DEFAULT_FORMATIVE_AGES = (6, 9, 13, 16, 21)
 DEFAULT_IMPORTANT_MODEL = importance_function.ConstantImportanceModel()
 
 
 @dataclasses.dataclass(frozen=True, kw_only=True)
 class AgentConfig:
   """A card that describes a player.
 
@@ -92,60 +94,45 @@
       context: any context to add to the generation, i.e. genre
 
     Returns:
       Descriptive text about the agent
     """
     prompt = interactive_document.InteractiveDocument(self._model)
 
-    if context:
-      prompt.statement(context)
     question = (
-        f'Given the following traits:\n{str(traits_description)}'
-        f'\n create a backstory about a {gender} character called {name}.'
-        ' Write a summary of the person:'
-        ' what their job is, what a typical day is is like, what are their'
-        ' goals, desires, hopes, dreams, and aspirations. Also write about'
-        ' their duties, responsibilities, and obligations. What gives them joy'
-        ' and what are they afraid of. Write about their friends and what they'
-        ' like to do. Also write about their current concerns.'
+        'Creative Writing Master Class\n'
+        f'Write a fictional life story for a {gender} character called {name} '
+        f'with the following traits:\n{str(traits_description)}.\nBegin the '
+        f'story when {name} is very young and end it when they are quite old. '
+        'The story should be no more than three paragraphs in total. '
+        'The story may include details such as (but not limited to) any of the '
+        'following: what their job is, what their typical day is like, what '
+        'their goals, desires, hopes, dreams, and aspirations are, as well as '
+        'their drives, duties, responsibilities, and obligations. It should '
+        'clarify what gives them joy and what are they afraid of. It may '
+        'include their friends and family. It should be a complete life story '
+        'but it should not specify how or when their life begins or ends. The '
+        f'reader should come away with a profound understanding of {name}.'
     )
     if context:
-      question += f' Take into account the following context: {context}'
+      question += f' Incorporate the following context: {context}'
     result = prompt.open_question(
         question,
-        max_characters=2500,
-        max_tokens=2500,
+        max_characters=5000,
+        max_tokens=4500,
         terminators=[],
     )
     result = re.sub(r'\.\s', '.\n', result)
-
-    query = '\n'.join([
-        (
-            'Replace all the pronouns in the following text with the name'
-            f' {name}.'
-        ),
-        'The text:',
-        result,
-    ])
-
-    description = self._model.sample_text(
-        query,
-        max_characters=2600,
-        max_tokens=2600,
-        terminators=[],
-    )
-    description = re.sub(r'\.\s', '.\n', description)
-
-    return description
+    return result
 
   def make_memories(
       self,
       agent_config: AgentConfig,
   ) -> associative_memory.AssociativeMemory:
-    """Creates agent memory from the agent card."""
+    """Creates agent memory from the agent config."""
 
     mem = self._blank_memory_factory_call()
     # All players share generic memories.
     for item in self._shared_memories:
       mem.add(item)
 
     context = agent_config.context
@@ -154,21 +141,21 @@
 
     self.add_memories(memory=mem, agent_config=agent_config)
 
     if context:
       context_items = context.split('\n')
       for item in context_items:
         if item:
-          mem.add(item, importance=1.0)
+          mem.add(item, importance=agent_config.formative_memory_importance)
 
     if agent_config.specific_memories:
       specific_memories = agent_config.specific_memories.split('\n')
       for item in specific_memories:
         if item:
-          mem.add(item, importance=1.0)
+          mem.add(item, importance=agent_config.formative_memory_importance)
 
     return mem
 
   def add_memories(
       self,
       memory: associative_memory.AssociativeMemory,
       agent_config: AgentConfig,
@@ -185,38 +172,60 @@
     description = self.make_backstory(
         agent_config.name,
         agent_config.gender,
         agent_config.traits,
         agent_config.context,
     )
     prompt = interactive_document.InteractiveDocument(self._model)
-    prompt.statement('Context: ' + description)
+    prompt.statement('Creative Writing Master Class\n')
+    prompt.statement('Character background story:\n\n' + description)
 
-    for episode_age in agent_config.formative_ages:
-      question = (
-          'Given the context above, come up with a formative episode at the '
-          + f'age of {episode_age}, which is consistent with'
-          f" {agent_config.name}'s "
-          + f"personality. Describe the episode from {agent_config.name}'s"
-          ' perspective '
-          + 'using third-person limited point of view. Mention their age at '
-          + 'the time. Use past tense. Write no more than three sentences.'
-      )
-      if agent_config.context:
-        question += (
-            '\nThe generated episode should be specifically related to some'
-            f' aspect of the following context: "{agent_config.context}"'
-        )
-
-      episode = prompt.open_question(
-          question,
-          max_characters=3000,
-          max_tokens=3000,
-          terminators=[],
+    question = (
+        'Given the life story above, invent formative episodes from '
+        f'the life of {agent_config.name} which could have taken '
+        f'place at the following ages: {agent_config.formative_ages}. '
+        'The episodes should be age appropriate and believeable. '
+        f'They should be memorable events for {agent_config.name} and '
+        'important for establishing who they are as a person. They should '
+        f'be consistent with {agent_config.name}\'s personality. '
+        f'Describe each episode from {agent_config.name}\'s perspective '
+        'and use third-person limited point of view. Each episode must '
+        'mention their age at the time the event occurred using language such '
+        f'as "When {agent_config.name} was 5 years old, they experienced..." . '
+        'Use past tense. Write no more than three sentences per episode. '
+        'Separate episodes from one another by the delimiter "\n\n\n". Do not '
+        'apply any other special formatting besides these delimiters.'
+    )
+    if agent_config.traits:
+      question += (
+          '\nTaken as a whole, these formative episodes from the life of '
+          f'{agent_config.name} should explain their personality, which has '
+          f'been described as: "{agent_config.traits}".')
+    if agent_config.context:
+      question += (
+          'Make a few of the episodes relate to the '
+          f'following context: "{agent_config.context}".'
       )
+
+    aggregated_result = prompt.open_question(
+        question=question,
+        max_characters=8000,
+        max_tokens=6000,
+        terminators=[],
+    )
+
+    episodes = aggregated_result.split('\n\n\n')
+
+    if len(episodes) != len(list(agent_config.formative_ages)):
+      logger.warning(
+          f'Number of generated formative episodes ({len(episodes)}) does ' +
+          'not match number of formative ages ' +
+          f'({len(list(agent_config.formative_ages))}).')
+
+    for episode_age, episode in zip(agent_config.formative_ages, episodes):
       memory.add(
           episode,
           tags=['episode'],
-          timestamp=agent_config.date_of_birth
-          + relativedelta(years=episode_age),
+          timestamp=(
+              agent_config.date_of_birth + relativedelta(years=episode_age)),
           importance=agent_config.formative_memory_importance,
       )
```

### Comparing `gdm-concordia-1.2.0/concordia/associative_memory/importance_function.py` & `gdm-concordia-1.3.0/concordia/associative_memory/importance_function.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/clocks/__init__.py` & `gdm-concordia-1.3.0/concordia/clocks/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/clocks/game_clock.py` & `gdm-concordia-1.3.0/concordia/clocks/game_clock.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/clocks/game_clock_test.py` & `gdm-concordia-1.3.0/concordia/clocks/game_clock_test.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/components/__init__.py` & `gdm-concordia-1.3.0/concordia/components/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/components/agent/__init__.py` & `gdm-concordia-1.3.0/concordia/components/agent/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,16 +14,21 @@
 
 
 """Library of components specifically for generative agents."""
 
 from concordia.components import constant
 from concordia.components import report_function
 from concordia.components import sequential
+from concordia.components.agent import all_similar_memories
 from concordia.components.agent import characteristic
+from concordia.components.agent import creative_reflection
+from concordia.components.agent import dialectical_reflection
 from concordia.components.agent import identity
 from concordia.components.agent import observation
 from concordia.components.agent import person_by_situation
 from concordia.components.agent import plan
 from concordia.components.agent import reflection
+from concordia.components.agent import relationships
+from concordia.components.agent import scheduled_hint
 from concordia.components.agent import self_perception
 from concordia.components.agent import situation_perception
 from concordia.components.agent import somatic_state
```

### Comparing `gdm-concordia-1.2.0/concordia/components/agent/characteristic.py` & `gdm-concordia-1.3.0/concordia/components/agent/characteristic.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/components/agent/identity.py` & `gdm-concordia-1.3.0/concordia/components/agent/identity.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 """Agent identity component."""
-
 import concurrent
+import datetime
+from typing import Callable
 from concordia.associative_memory import associative_memory
 from concordia.components.agent import characteristic
 from concordia.language_model import language_model
 from concordia.typing import component
 
 
 class SimIdentity(component.Component):
@@ -32,26 +33,30 @@
   """
 
   def __init__(
       self,
       model: language_model.LanguageModel,
       memory: associative_memory.AssociativeMemory,
       agent_name: str,
+      clock_now: Callable[[], datetime.datetime] | None = None,
   ):
     """Initialize an identity component.
 
     Args:
       model: a language model
       memory: an associative memory
       agent_name: the name of the agent
+      clock_now: time callback to use for the state.
     """
     self._model = model
     self._memory = memory
     self._state = ''
     self._agent_name = agent_name
+    self._clock_now = clock_now
+    self._last_update = datetime.datetime.min
 
     self._identity_component_names = [
         'core characteristics',
         'current daily occupation',
         'feeling about recent progress in life',
     ]
 
@@ -70,25 +75,31 @@
   def name(self) -> str:
     return 'Identity'
 
   def state(self):
     return self._state
 
   def get_last_log(self):
-    current_log = {'Summary': f'identity of {self._agent_name}',
-                   'state': self._state}
+    current_log = {
+        'Summary': f'identity of {self._agent_name}',
+        'state': self._state,
+    }
     for comp in self._identity_components:
       last_log = comp.get_last_log()
       if last_log:
         if 'date' in last_log.keys():
           last_log.pop('date')
         current_log[comp.name()] = last_log
     return current_log
 
   def update(self):
+    if self._clock_now() == self._last_update:
+      return
+    self._last_update = self._clock_now()
+
     with concurrent.futures.ThreadPoolExecutor() as executor:
       for c in self._identity_components:
         executor.submit(c.update)
 
     self._state = '\n'.join(
         [f'{c.name()}: {c.state()}' for c in self._identity_components]
     )
```

### Comparing `gdm-concordia-1.2.0/concordia/components/agent/observation.py` & `gdm-concordia-1.3.0/concordia/components/agent/observation.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,17 @@
   def name(self) -> str:
     return self._name
 
   def state(self):
     mems = self._memory.retrieve_time_interval(
         self._clock_now() - self._timeframe, self._clock_now(), add_time=True
     )
+    # removes memories that are not observations
+    mems = [mem for mem in mems if '[observation]' in mem]
+
     if self._verbose:
       self._log('\n'.join(mems) + '\n')
     return '\n'.join(mems) + '\n'
 
   def get_last_log(self):
     return {
         'Summary': 'observation',
@@ -130,16 +133,17 @@
     self._timeframe_delta_from = timeframe_delta_from
     self._timeframe_delta_until = timeframe_delta_until
     self._clock_now = clock_now
     self._components = components
     self._state = ''
     self._display_timeframe = display_timeframe
     self._prompt = prompt or (
-        'Summarize the memories above into one sentence '
-        f'about {self._agent_name}.')
+        'Summarize the observations above into one sentence '
+        f'about {self._agent_name}.'
+    )
 
     self._verbose = verbose
     self._history = []
 
   def name(self) -> str:
     return self._name
 
@@ -167,17 +171,22 @@
 
     mems = self._memory.retrieve_time_interval(
         segment_start,
         segment_end,
         add_time=True,
     )
 
+    # removes memories that are not observations
+    mems = [mem for mem in mems if '[observation]' in mem]
+
     prompt = interactive_document.InteractiveDocument(self._model)
     prompt.statement(context + '\n')
-    prompt.statement(f'Recent memories of {self._agent_name}:\n' + f'{mems}\n')
+    prompt.statement(
+        f'Recent observations of {self._agent_name}:\n' + f'{mems}\n'
+    )
     self._state = (
         self._agent_name
         + ' '
         + prompt.open_question(
             self._prompt,
             answer_prefix=f'{self._agent_name} ',
             max_characters=1200,
```

### Comparing `gdm-concordia-1.2.0/concordia/components/agent/person_by_situation.py` & `gdm-concordia-1.3.0/concordia/components/agent/person_by_situation.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,27 +56,32 @@
     self._memory = memory
     self._state = ''
     self._components = components or []
     self._agent_name = agent_name
     self._clock_now = clock_now
     self._num_memories_to_retrieve = num_memories_to_retrieve
     self._name = name
+    self._last_update = self._clock_now() - datetime.timedelta(days=365)
     self._history = []
 
   def name(self) -> str:
     return self._name
 
   def state(self) -> str:
     return self._state
 
   def get_last_log(self):
     if self._history:
       return self._history[-1].copy()
 
   def update(self) -> None:
+    if self._clock_now() == self._last_update:
+      return
+    self._last_update = self._clock_now()
+
     prompt = interactive_document.InteractiveDocument(self._model)
 
     mems = '\n'.join(
         self._memory.retrieve_recent(
             self._num_memories_to_retrieve, add_time=True
         )
     )
```

### Comparing `gdm-concordia-1.2.0/concordia/components/agent/plan.py` & `gdm-concordia-1.3.0/concordia/components/agent/plan.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Agent components for planning."""
-
-from typing import Sequence
+from collections.abc import Sequence
+import datetime
+from typing import Callable
 from concordia.associative_memory import associative_memory
 from concordia.document import interactive_document
 from concordia.language_model import language_model
 from concordia.typing import component
 import termcolor
 
 
@@ -27,28 +28,30 @@
 
   def __init__(
       self,
       model: language_model.LanguageModel,
       memory: associative_memory.AssociativeMemory,
       agent_name: str,
       components: list[component.Component],
+      clock_now: Callable[[], datetime.datetime],
       goal: component.Component | None = None,
       num_memories_to_retrieve: int = 5,
       timescale: str = 'the rest of the day',
       time_adverb: str = 'hourly',
       verbose: bool = False,
       log_color='green',
   ):
     """Initialize a component to represent the agent's plan.
 
     Args:
       model: a language model
       memory: an associative memory
       agent_name: the name of the agent
       components: components to build the context of planning
+      clock_now: time callback to use for the state.
       goal: a component to represent the goal of planning
       num_memories_to_retrieve: how many memories to retrieve as conditioning
         for the planning chain of thought
       timescale: string describing how long the plan should last
       time_adverb: string describing the rate of steps in the plan
       verbose: whether or not to print intermediate reasoning steps
       log_color: color for debug logging
@@ -59,14 +62,16 @@
     self._agent_name = agent_name
     self._log_color = log_color
     self._components = components
     self._num_memories_to_retrieve = num_memories_to_retrieve
     self._goal_component = goal
     self._timescale = timescale
     self._time_adverb = time_adverb
+    self._clock_now = clock_now
+    self._last_update = datetime.datetime.min
 
     self._latest_memories = ''
     self._last_observation = []
     self._current_plan = ''
     self._history = []
 
     self._verbose = verbose
@@ -87,14 +92,18 @@
   def observe(self, observation: str):
     self._last_observation.append(observation)
 
   def get_components(self) -> Sequence[component.Component]:
     return self._components
 
   def update(self):
+    if self._last_update == self._clock_now():
+      return
+    self._last_update = self._clock_now()
+
     observation = '\n'.join(self._last_observation)
     self._last_observation = []
     memories = self._memory.retrieve_associative(
         observation,
         k=self._num_memories_to_retrieve,
         use_recency=True,
         add_time=True,
@@ -120,27 +129,31 @@
     prompt = interactive_document.InteractiveDocument(self._model)
     prompt.statement(f'{components}\n')
     prompt.statement(f'Relevant memories:\n{memories}')
     if self._goal_component:
       prompt.statement(f'Current goal: {self._goal_component.state()}.')
     prompt.statement(f'Current plan: {self._current_plan}')
     prompt.statement(f'Current situation: {observation}')
+
+    time_now = self._clock_now().strftime('[%d %b %Y %H:%M:%S]')
+    prompt.statement(f'The current time is: {time_now}\n')
     should_replan = prompt.yes_no_question(
         f'Given the above, should {self._agent_name} change their current '
         'plan? '
     )
 
     if should_replan or not self._state:
       goal_mention = '.'
       if self._goal_component:
         goal_mention = ', keep in mind the goal.'
       self._current_plan = prompt.open_question(
           f"Write {self._agent_name}'s plan for {self._timescale}. Please,"
           f' provide a {self._time_adverb} schedule'
-          + goal_mention + in_context_example,
+          + goal_mention
+          + in_context_example,
           max_characters=1200,
           max_tokens=1200,
           terminators=(),
       )
 
     self._state = self._current_plan
```

### Comparing `gdm-concordia-1.2.0/concordia/components/agent/reflection.py` & `gdm-concordia-1.3.0/concordia/components/agent/reflection.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/components/agent/self_perception.py` & `gdm-concordia-1.3.0/concordia/components/agent/self_perception.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,30 +49,39 @@
     """
 
     self._verbose = verbose
     self._model = model
     self._memory = memory
     self._state = ''
     self._agent_name = agent_name
+
     self._clock_now = clock_now
+    if clock_now is None:
+      self._clock_now = lambda: ''
+
     self._num_memories_to_retrieve = num_memories_to_retrieve
     self._name = name
+    self._last_update = datetime.datetime.min
     self._history = []
 
   def name(self) -> str:
     return self._name
 
   def state(self) -> str:
     return self._state
 
   def get_last_log(self):
     if self._history:
       return self._history[-1].copy()
 
   def update(self) -> None:
+    if self._clock_now() == self._last_update:
+      return
+    self._last_update = self._clock_now()
+
     mems = '\n'.join(
         self._memory.retrieve_recent(
             self._num_memories_to_retrieve, add_time=True
         )
     )
 
     prompt = interactive_document.InteractiveDocument(self._model)
```

### Comparing `gdm-concordia-1.2.0/concordia/components/agent/situation_perception.py` & `gdm-concordia-1.3.0/concordia/components/agent/situation_perception.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     self._memory = memory
     self._state = ''
     self._components = components or []
     self._agent_name = agent_name
     self._clock_now = clock_now
     self._num_memories_to_retrieve = num_memories_to_retrieve
     self._name = name
+    self._last_update = self._clock_now() - datetime.timedelta(days=365)
     self._history = []
 
   def name(self) -> str:
     return self._name
 
   def state(self) -> str:
     return self._state
@@ -70,14 +71,18 @@
     if self._history:
       return self._history[-1].copy()
 
   def get_components(self) -> Sequence[component.Component]:
     return self._components
 
   def update(self) -> None:
+    if self._clock_now() == self._last_update:
+      return
+    self._last_update = self._clock_now()
+
     mems = '\n'.join(
         self._memory.retrieve_recent(
             self._num_memories_to_retrieve, add_time=True
         )
     )
 
     prompt = interactive_document.InteractiveDocument(self._model)
```

### Comparing `gdm-concordia-1.2.0/concordia/components/agent/somatic_state.py` & `gdm-concordia-1.3.0/concordia/components/agent/somatic_state.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     self._model = model
     self._memory = memory
     self._state = ''
     self._agent_name = agent_name
     self._clock_now = clock_now
     self._summarize = summarize
     self._verbose = verbose
+    self._last_update = datetime.datetime.min
 
     self._characteristic_names = [
         'level of hunger',
         'level of thirst',
         'level of fatigue',
         'level of pain',
         'level of feeling socially connected in life',
@@ -106,14 +107,19 @@
       if last_log:
         if 'date' in last_log.keys():
           last_log.pop('date')
         current_log[comp.name()] = last_log
     return current_log
 
   def update(self):
+    if self._clock_now and self._last_update == self._clock_now():
+      return
+    if self._clock_now:
+      self._last_update = self._clock_now()
+
     with concurrent.futures.ThreadPoolExecutor() as executor:
       for c in self._characteristics:
         executor.submit(c.update)
 
     self._state = '\n'.join([
         f"{self._agent_name}'s {c.name()}: " + c.state()
         for c in self._characteristics
```

### Comparing `gdm-concordia-1.2.0/concordia/components/constant.py` & `gdm-concordia-1.3.0/concordia/components/constant.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/components/game_master/__init__.py` & `gdm-concordia-1.3.0/concordia/components/game_master/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,13 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 """Library of components specifically for generative game master."""
 
 from concordia.components.game_master import conversation
+from concordia.components.game_master import current_scene
 from concordia.components.game_master import direct_effect
 from concordia.components.game_master import inventory
 from concordia.components.game_master import player_status
 from concordia.components.game_master import relevant_events
 from concordia.components.game_master import schedule
 from concordia.components.game_master import time_display
```

### Comparing `gdm-concordia-1.2.0/concordia/components/game_master/conversation.py` & `gdm-concordia-1.3.0/concordia/components/game_master/conversation.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
-"""Externality for the Game Master, which generates conversations."""
+"""Externality component for the Game Master, which generates conversations."""
 
 from collections.abc import Sequence
 import datetime
 
 from concordia import components as generic_components
 from concordia.agents import basic_agent
 from concordia.associative_memory import associative_memory
 from concordia.associative_memory import blank_memories
 from concordia.clocks import game_clock
 from concordia.components import agent as sim_components
 from concordia.document import interactive_document
+from concordia.environment import game_master
 from concordia.environment.scenes import conversation as conversation_scene
 from concordia.language_model import language_model
 from concordia.typing import clock as clock_lib
 from concordia.typing import component
 from concordia.utils import helper_functions
 import termcolor
 
@@ -40,51 +40,53 @@
       self,
       players: Sequence[basic_agent.BasicAgent],
       model: language_model.LanguageModel,
       memory: associative_memory.AssociativeMemory,
       clock: game_clock.MultiIntervalClock,
       burner_memory_factory: blank_memories.MemoryFactory,
       cap_nonplayer_characters: int = 3,
-      game_master_instructions: str = '',
       shared_context: str = '',
       components: Sequence[component.Component] | None = None,
       allow_self_talk: bool = False,
       review_participants: bool = True,
       verbose: bool = False,
-      print_colour: str = 'magenta',
+      npc_instructions: str = game_master.DEFAULT_GAME_MASTER_INSTRUCTIONS,
+      log_color: str = 'magenta',
   ):
     """Initializes the generator of conversations.
 
     Args:
       players: A list of players to generate conversations for.
       model: A language model to use for generating utterances.
       memory: GM memory, used to add the summary of the conversation
       clock: multi interval game clock. If conversation happens, the clock will
         advance in higher gear during the conversation scene.
       burner_memory_factory: a memory factory to create temporary memory for
         npcs and conversation gm
       cap_nonplayer_characters: The maximum number of non-player characters
         allowed in the conversation.
-      game_master_instructions: A string to use as the game master instructions.
       shared_context: A string to use as the generic context for the NPCs.
       components: components that contextualise the conversation
       allow_self_talk: allow players to have a conversation with themselves
       review_participants: whether or not to start each scene by declaring
         who its participants are.
       verbose: Whether to print debug messages or not.
-      print_colour: colour in which to print logs
+      npc_instructions: by default use the standard game master instructions
+        for non-player characters. Otherwise override this with custom
+        instructions.
+      log_color: color in which to print logs
     """
     self._players = players
     self._model = model
     self._cap_nonplayer_characters = cap_nonplayer_characters
-    self._game_master_instructions = game_master_instructions
+    self._npc_instructions = npc_instructions
     self._shared_context = shared_context
     self._history = []
     self._verbose = verbose
-    self._print_colour = print_colour
+    self._log_color = log_color
     self._components = components or []
     self._clock = clock
     self._burner_memory_factory = burner_memory_factory
     self._memory = memory
     self._allow_self_talk = allow_self_talk
     self._all_player_names = [player.name for player in self._players]
     self._min_speakers = 1 if self._allow_self_talk else 2
@@ -100,15 +102,15 @@
     if self._history:
       return self._history[-1].copy()
 
   def get_player_names(self):
     return [player.name for player in self._players]
 
   def _log(self, entry):
-    print(termcolor.colored(entry, self._print_colour))
+    print(termcolor.colored(entry, self._log_color))
 
   def _make_npc(
       self, name: str, scene_clock: clock_lib.GameClock
   ) -> basic_agent.BasicAgent:
     context = (
         f'{name} is a non-player character. Everyone knows the'
         f' following:\n{self._shared_context}'
@@ -119,15 +121,15 @@
     npc = basic_agent.BasicAgent(
         model=self._model,
         memory=mem,
         agent_name=name,
         clock=scene_clock,
         components=[
             generic_components.constant.ConstantComponent(
-                name='Instructions:', state=self._game_master_instructions
+                name='Instructions:', state=self._npc_instructions
             ),
             generic_components.constant.ConstantComponent(
                 name='General knowledge:', state=context
             ),
             sim_components.observation.Observation(
                 agent_name=name,
                 memory=mem,
```

### Comparing `gdm-concordia-1.2.0/concordia/components/game_master/direct_effect.py` & `gdm-concordia-1.3.0/concordia/components/game_master/direct_effect.py`

 * *Files 13% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     self._components = components or []
     self._clock_now = clock_now
     self._history = []
     self._model = model
     self._memory = memory
 
   def name(self) -> str:
-    return 'Effect of event on players'
+    return 'Direct effects of the event on others'
 
   def _print(self, entry: str):
     print(termcolor.colored(entry, self._print_colour), end='')
 
   def get_player_names(self):
     return [player.name for player in self._players]
 
@@ -102,51 +102,57 @@
         known = player_doc.yes_no_question(
             f'Does {player_name} know about the event?'
         )
         if known:
           if self._verbose:
             self._print(f'\n{player_name} known.')
           _ = player_doc.open_question(
-              f'What does {player_name} know about the event?'
+              f'What does {player_name} know about the event?',
+              max_characters=3000,
+              max_tokens=2500,
           )
           how_player_saw_event_first_person = player_doc.open_question(
               f"Summarize the event from {player_name}'s "
               + 'perspective using third-person limited point of view. '
               + 'If the event contains a direct quotation of anything said '
               + 'or written by anyone then it is important to include the '
-              + 'quote verbatim in the summary.'
+              + 'quote verbatim in the summary.',
+              max_characters=3000,
+              max_tokens=2500,
           )
           player.observe(how_player_saw_event_first_person)
           if self._verbose:
             self._print(
                 f'\nEffect on {player_name}:'
                 f' {how_player_saw_event_first_person}'
             )
           effect_known.append(how_player_saw_event_first_person)
         else:  # not known
           if self._verbose:
             self._print(f'\n{player_name} not known.')
           effect_despite_ignorance = player_doc.open_question(
-              f'How does the event affect {player_name}`s status, despite them'
-              ' not knowing about it?'
+              f"How does the event affect {player_name}'s status, despite them"
+              ' not knowing about it?',
+              max_characters=3000,
+              max_tokens=2500,
           )
           if self._verbose:
             self._print(
                 f'\nUnknown effect on {player_name}: {effect_despite_ignorance}'
             )
           effect = f'[effect on {player_name}] {effect_despite_ignorance}'
           self._memory.add(effect)
           effect_unknown.append(effect)
 
     # Determined whether externality has happened
     # if yes, then propagate the event
     if direct_effect_on_someone:
       if self._verbose:
         self._print(
-            '\nThe event had a direct affect on one of the players, resolving.'
+            '\nThe event had a direct effect on one of the players, resolving.'
         )
 
       with concurrent.futures.ThreadPoolExecutor() as executor:
         executor.map(_update_player, self._players)
 
     update_log = {
         'date': self._clock_now(),
```

### Comparing `gdm-concordia-1.2.0/concordia/components/game_master/inventory.py` & `gdm-concordia-1.3.0/concordia/components/game_master/inventory.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,15 +204,17 @@
             if player.rstrip(' ') in self._player_names:
               prefix = f"[effect on {player}'s {self._name}]"
               amount = chain_of_thought.open_question(
                   question=(
                       f'How {_many_or_much(self._is_count_noun[item_type])} '
                       + f'{item_type} did {player} gain '
                       + f'as a result of the event? If they lost {item_type} '
-                      'then respond with a negative number.'
+                      + 'then respond with a negative number. Be precise. If '
+                      + 'the original event was imprecise then pick a specific '
+                      + 'value that is consistent with all the text above.'
                   )
               )
               try:
                 amount = float(amount)
               except ValueError:
                 amount = 0.0
               if self._item_types_dict[item_type].force_integer:
```

### Comparing `gdm-concordia-1.2.0/concordia/components/game_master/player_status.py` & `gdm-concordia-1.3.0/concordia/components/game_master/player_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 
 """This construct track the status and location of players."""
 
 from collections.abc import Callable, Sequence
 import datetime
+import threading
 
 from concordia.associative_memory import associative_memory
 from concordia.document import interactive_document
 from concordia.language_model import language_model
 from concordia.typing import component
 
 
@@ -51,63 +52,74 @@
     self._state = ''
     self._player_names = player_names
     self._num_memories_to_retrieve = num_memories_to_retrieve
     self._partial_states = {name: '' for name in self._player_names}
     self._verbose = verbose
     self._history = []
     self._clock_now = clock_now
+    self._last_memory_len = 0
+    self._state_lock = threading.Lock()
 
   def name(self) -> str:
     return 'Status of players'
 
   def state(self) -> str:
-    return self._state
+    with self._state_lock:
+      return self._state
 
   def get_history(self):
-    return self._history.copy()
+    with self._state_lock:
+      return self._history.copy()
 
   def get_last_log(self):
-    if self._history:
-      return self._history[-1].copy()
+    with self._state_lock:
+      if self._history:
+        return self._history[-1].copy()
 
   def partial_state(
       self,
       player_name: str,
   ) -> str:
     """Return a player-specific view of the construct's state."""
-    return self._partial_states[player_name]
+    with self._state_lock:
+      return self._partial_states[player_name]
 
   def update(self) -> None:
-    self._state = ''
-    self._partial_states = {name: '' for name in self._player_names}
-    per_player_prompt = {}
-    for player_name in self._player_names:
-      memories = self._memory.retrieve_by_regex(player_name)
-      memories = memories[-self._num_memories_to_retrieve:]
-      prompt = interactive_document.InteractiveDocument(self._model)
-      prompt.statement('Events:\n' + '\n'.join(memories) + '\n')
-      time_now = self._clock_now().strftime('[%d %b %Y %H:%M:%S]')
-      prompt.statement(f'The current time is: {time_now}\n')
-      player_loc = (
-          prompt.open_question(
-              'Given the above events and their time, what is the latest'
-              f' location of {player_name} and what are they doing?',
-              answer_prefix=f'{player_name} is ',
-          )
-          + '\n'
-      )
-      per_player_prompt[player_name] = prompt.view().text().splitlines()
-      if self._verbose:
-        print(prompt.view().text())
-
-      # Indent player status outputs.
-      player_state_string = f'  {player_name} is ' + player_loc
-      self._partial_states[player_name] = player_state_string
-      self._state = self._state + player_state_string
-
-    update_log = {
-        'date': self._clock_now(),
-        'state': self._state,
-        'partial states': self._partial_states,
-        'per player prompts': per_player_prompt,
-    }
-    self._history.append(update_log)
+    with self._state_lock:
+      if self._last_memory_len == len(self._memory):
+        return
+      self._last_memory_len = len(self._memory)
+
+      self._state = ''
+      self._partial_states = {name: '' for name in self._player_names}
+      per_player_prompt = {}
+      for player_name in self._player_names:
+        memories = self._memory.retrieve_by_regex(player_name)
+        memories = memories[-self._num_memories_to_retrieve:]
+        prompt = interactive_document.InteractiveDocument(self._model)
+        prompt.statement('Events:\n' + '\n'.join(memories) + '\n')
+        time_now = self._clock_now().strftime('[%d %b %Y %H:%M:%S]')
+        prompt.statement(f'The current time is: {time_now}\n')
+        player_loc = (
+            prompt.open_question(
+                'Given the above events and their time, what is the latest'
+                f' location of {player_name} and what are they doing?',
+                answer_prefix=f'{player_name} is ',
+            )
+            + '\n'
+        )
+        per_player_prompt[player_name] = prompt.view().text().splitlines()
+        if self._verbose:
+          print(prompt.view().text())
+
+        # Indent player status outputs.
+        player_state_string = f'  {player_name} is ' + player_loc
+        self._partial_states[player_name] = player_state_string
+        self._state = self._state + player_state_string
+
+      update_log = {
+          'date': self._clock_now(),
+          'state': self._state,
+          'partial states': self._partial_states,
+          'per player prompts': per_player_prompt,
+      }
+      self._history.append(update_log)
```

### Comparing `gdm-concordia-1.2.0/concordia/components/game_master/player_status_test.py` & `gdm-concordia-1.3.0/concordia/components/game_master/player_status_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,14 +36,15 @@
   )
   def test_output_in_right_format(self, location):
     model = mock.create_autospec(
         language_model.LanguageModel, instance=True, spec_set=True)
     model.sample_text.return_value = location
     memory = mock.create_autospec(associative_memory.AssociativeMemory,
                                   instance=True)
+    memory.__len__.return_value = 1
     memory.retrieve_associative.return_value = "gibberish"
     player_names = ["Alice", "Bob"]
     component = player_status.PlayerStatus(
         clock_now=_clock_now,
         model=model,
         memory=memory,
         player_names=player_names)
```

### Comparing `gdm-concordia-1.2.0/concordia/components/game_master/relevant_events.py` & `gdm-concordia-1.3.0/concordia/components/game_master/relevant_events.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/components/game_master/schedule.py` & `gdm-concordia-1.3.0/concordia/components/game_master/schedule.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/components/game_master/time_display.py` & `gdm-concordia-1.3.0/concordia/components/game_master/time_display.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/components/report_function.py` & `gdm-concordia-1.3.0/concordia/components/report_function.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/components/sequential.py` & `gdm-concordia-1.3.0/concordia/components/sequential.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/document/__init__.py` & `gdm-concordia-1.3.0/concordia/document/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/document/document.py` & `gdm-concordia-1.3.0/concordia/document/document.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/document/document_test.py` & `gdm-concordia-1.3.0/concordia/document/document_test.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/document/interactive_document.py` & `gdm-concordia-1.3.0/concordia/document/interactive_document.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,44 +138,50 @@
     """Appends a response to the document that was generated by the model."""
     self.append(text + end, tags=[RESPONSE_TAG, MODEL_TAG, *tags])
 
   def open_question(
       self,
       question: str,
       *,
+      forced_response: str | None = None,
       answer_prefix: str = '',
       answer_suffix: str = '',
       max_tokens: int = DEFAULT_MAX_TOKENS,
       max_characters: int = DEFAULT_MAX_CHARACTERS,
       terminators: Collection[str] = ('\n',),
   ) -> str:
     """Asks the agent an open question and appends it to the document.
 
     Args:
       question: the question to ask.
+      forced_response: forces the document to provide this response. The LLM
+        will not be consulted. If answer_prefix is in the forced response then
+        remove it.
       answer_prefix: a prefix to append to the model's prompt.
       answer_suffix: a suffix to append to the model's response.
       max_tokens: the maximum number of tokens to sample from the model.
       max_characters: the maximum number of characters to sample from the model.
       terminators: strings that must not be present in the model's response. If
         emitted by the model the response will be truncated before them.
 
     Returns:
-      The agents truncated response.
+      The agents truncated response (or `forced_response` is provided).
     """
     self._question(f'Question: {question}\n')
     self._response(f'Answer: {answer_prefix}')
-    response = self._model.sample_text(
-        prompt=self._model_view.text(),
-        max_tokens=max_tokens,
-        max_characters=max_characters,
-        terminators=terminators,
-    )
-    if response.startswith(answer_prefix):
-      response = response[len(answer_prefix):]
+    if forced_response is None:
+      response = self._model.sample_text(
+          prompt=self._model_view.text(),
+          max_tokens=max_tokens,
+          max_characters=max_characters,
+          terminators=terminators,
+      )
+    else:
+      response = forced_response
+    response = response.removeprefix(answer_prefix)
     self._model_response(response)
     self._response(f'{answer_suffix}\n')
     return response
 
   def multiple_choice_question(
       self, question: str, answers: Sequence[str]
   ) -> int:
```

### Comparing `gdm-concordia-1.2.0/concordia/document/interactive_document_test.py` & `gdm-concordia-1.3.0/concordia/document/interactive_document_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -78,14 +78,48 @@
           QUESTION('Question: What is 1+1?\n'),
           RESPONSE('Answer: Well...'),
           MODEL_RESPONSE('This is a long answer'),
           RESPONSE('\n'),
       )
       self.assertEqual(doc.contents(), expected)
 
+  def test_open_question_with_forced_answer(self):
+    model = mock.create_autospec(
+        language_model.LanguageModel, instance=True, spec_set=True
+    )
+    model.sample_text.return_value = 'This is a long answer'
+
+    doc = interactive_document.InteractiveDocument(model)
+    doc.statement('Hi!')
+    response = doc.open_question(
+        question='What is 1+1?',
+        forced_response='I hereby declare the answer to be 7',
+        answer_prefix='OK then...',
+    )
+
+    with self.subTest('response'):
+      self.assertEqual(response, 'I hereby declare the answer to be 7')
+
+    with self.subTest('text'):
+      expected = """Hi!
+Question: What is 1+1?
+Answer: OK then...I hereby declare the answer to be 7
+"""
+      self.assertEqual(doc.text(), expected)
+
+    with self.subTest('contents'):
+      expected = (
+          STATEMENT('Hi!\n'),
+          QUESTION('Question: What is 1+1?\n'),
+          RESPONSE('Answer: OK then...'),
+          MODEL_RESPONSE('I hereby declare the answer to be 7'),
+          RESPONSE('\n'),
+      )
+      self.assertEqual(doc.contents(), expected)
+
   def test_multiple_choice_question(self):
     model = mock.create_autospec(
         language_model.LanguageModel, instance=True, spec_set=True
     )
     model.sample_choice.return_value = (2, 'c', mock.sentinel.debug)
     rng = mock.create_autospec(
         np.random.Generator, instance=True, spec_set=True
```

### Comparing `gdm-concordia-1.2.0/concordia/environment/__init__.py` & `gdm-concordia-1.3.0/concordia/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/environment/game_master.py` & `gdm-concordia-1.3.0/concordia/environment/game_master.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,39 +8,57 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
 """A Generic Game Master."""
 
 from collections.abc import Callable, Sequence
 import concurrent.futures
 import random
 
+from concordia import components as generic_components
 from concordia.agents import basic_agent
 from concordia.associative_memory import associative_memory
 from concordia.document import interactive_document
 from concordia.language_model import language_model
 from concordia.thought_chains import thought_chains
 from concordia.typing import agent as simulacrum_agent
 from concordia.typing import clock as game_clock
 from concordia.typing import component
 from concordia.typing import game_master as simulacrum_game_master
+from concordia.utils import helper_functions
 import termcolor
 
 
 DEFAULT_THOUGHTS = (
     thought_chains.attempt_to_result,
     thought_chains.result_to_who_what_where,
 )
 
 
+DEFAULT_GAME_MASTER_INSTRUCTIONS = (
+    'This is a social science experiment. It is structured as a '
+    'tabletop roleplaying game (like dungeons and dragons). You are the '
+    'game master. You will describe the current situation to the '
+    'participants in the experiment and then on the basis of what you '
+    'tell them they will suggest actions for the character they control. '
+    'Aside from you, each other participant controls just one character. '
+    'You are the game master so you may control any non-player '
+    'character. You will track the state of the world and keep it '
+    'consistent as time passes in the simulation and the participants '
+    'take actions and change things in their world. Remember that this '
+    'is a serious social science experiment. It is not just a game. It '
+    'need not be fun for the participants. Always use third-person '
+    'limited perspective, even when speaking directly to the participants.'
+)
+
+
 class GameMaster(simulacrum_game_master.GameMaster):
   """A generic game master."""
 
   def __init__(
       self,
       model: language_model.LanguageModel,
       memory: associative_memory.AssociativeMemory,
@@ -59,15 +77,16 @@
       action_spec: simulacrum_agent.ActionSpec | None = None,
       randomise_initiative: bool = False,
       player_observes_event: bool = True,
       players_act_simultaneously: bool = True,
       verbose: bool = False,
       concurrent_externalities: bool = True,
       concurrent_action: bool = False,
-      log_colour: str = 'red',
+      use_default_instructions: bool = True,
+      log_color: str = 'red',
   ):
     """Game master constructor.
 
     Args:
       model: a language model
       memory: an associative memory
       clock: a clock
@@ -85,40 +104,51 @@
         avoid duplicate memories.
       players_act_simultaneously: advance time after all players have acted, if
         false then advance time after each player acts.
       verbose: whether to print debugging information or not.
       concurrent_externalities: if true, runs externalities in separate threads
       concurrent_action: if true, runs player actions and events in separate
         threads
-      log_colour: colour in which to print logs
+      use_default_instructions: set to False if you want to skip the standard
+        instructions used for the game master, e.g. do this if you plan to pass
+        custom instructions as a constant component instead.
+      log_color: color in which to print logs
     """
     self._name = name
     self._model = model
     self._memory = memory
     self._clock = clock
-    self._players = players
-    self._log_colour = log_colour
+    self._log_color = log_color
     self._randomise_initiative = randomise_initiative
     self._player_observes_event = player_observes_event
     self._players_act_simultaneously = players_act_simultaneously
     self._action_spec = action_spec or simulacrum_agent.DEFAULT_ACTION_SPEC
     self._concurrent_action = concurrent_action
 
+    components = list(components or [])
+    if use_default_instructions:
+      instructions_component = generic_components.constant.ConstantComponent(
+          state=DEFAULT_GAME_MASTER_INSTRUCTIONS, name='Instructions'
+      )
+      components.insert(0, instructions_component)
+
     self._components = {}
     for comp in components:
       if comp.name() in self._components:
         raise ValueError(f'Duplicate component name: {comp.name()}')
       else:
         self._components[comp.name()] = comp
 
     self._verbose = verbose
 
     self._update_from_player_thoughts = update_thought_chain or DEFAULT_THOUGHTS
 
-    self._players_by_name = {player.name: player for player in self._players}
+    self._players_by_name = {player.name: player for player in players}
+    if len(self._players_by_name) != len(players):
+      raise ValueError('Duplicate player names')
 
     self._concurrent_externalities = concurrent_externalities
     self._log = []
 
     self.reset()
 
   def name(self):
@@ -126,23 +156,23 @@
 
   def get_history(self):
     return self._log.copy()
 
   def get_data_frame(self):
     return self._memory.get_data_frame()
 
-  def _print(self, entry, colour=None):
-    print(termcolor.colored(entry, colour or self._log_colour))
+  def _print(self, entry, color=None):
+    print(termcolor.colored(entry, color or self._log_color))
 
   def reset(self):
     self._last_chain = None
-    self._num_players = len(self._players)
+    self._num_players = len(self._players_by_name.keys())
 
   def get_player_names(self):
-    return [player.name for player in self._players]
+    return list(self._players_by_name.keys())
 
   def update_from_player(self, player_name: str, action_attempt: str):
     prompt = interactive_document.InteractiveDocument(self._model)
 
     with concurrent.futures.ThreadPoolExecutor() as executor:
       executor.map(
           lambda construct: construct.update_before_event(
@@ -156,15 +186,18 @@
       if state_of_component:
         prompt.statement(comp.name() + ': ' + state_of_component + '\n')
 
     prompt.statement(f"\n{player_name}'s attempted action: {action_attempt}")
 
     # Produce the event that has happened as the result of the action attempt
     prompt, event_statement = thought_chains.run_chain_of_thought(
-        self._update_from_player_thoughts, action_attempt, prompt, player_name,
+        self._update_from_player_thoughts,
+        action_attempt,
+        prompt,
+        player_name,
     )
 
     self._memory.add(event_statement)
 
     # This gives duplicates if direct_effect-like component is used
     if self._player_observes_event:
       self._players_by_name[player_name].observe(event_statement)
@@ -231,43 +264,81 @@
           if observation:
             self._players_by_name[player_name].observe(observation)
 
     return
 
   def update_components(self) -> None:
     # MULTI THREAD!
+    def _get_recursive_update_func(
+        comp: component.Component,
+    ) -> Callable[[], None]:
+      return lambda: helper_functions.apply_recursively(
+          comp, function_name='update'
+      )
+
     with concurrent.futures.ThreadPoolExecutor() as executor:
-      executor.map(
-          lambda construct: construct.update(), list(self._components.values()))
+      for comp in self._components.values():
+        executor.submit(_get_recursive_update_func(comp))
 
-  def _step_player(self, player: basic_agent.BasicAgent):
+  def _step_player(
+      self,
+      player: basic_agent.BasicAgent,
+      action_spec: simulacrum_agent.ActionSpec | None = None,
+  ):
     self.update_components()
     self.view_for_player(player_name=player.name)
-    action = player.act(self._action_spec)
+
+    if action_spec:
+      action_spec_this_time = action_spec
+    else:
+      action_spec_this_time = self._action_spec
+
+    action = player.act(action_spec_this_time)
 
     self.update_from_player(action_attempt=action, player_name=player.name)
 
-  def step(self):
+  def step(
+      self,
+      *,
+      active_players: Sequence[basic_agent.BasicAgent] | None = None,
+      action_spec: simulacrum_agent.ActionSpec | None = None,
+  ):
     """Steps the game.
 
     At each step players all take a turn 'quasisimultaneously' with regard to
     the main game clock, but still in a specific order within the timestep.
     This is the same principle as initiative order in dungeons and dragons.
+
+    Args:
+      active_players: Optionally specify players to take turns in this round.
+      action_spec: Optionally specify what kind of action to ask the agent to
+        generate.
     """
-    players = list(self._players)
+    if active_players:
+      players = list(active_players)
+    else:
+      players = list(self._players_by_name.values())
+
+    override_action_spec = None
+    if action_spec:
+      override_action_spec = action_spec
+
+    step_player_fn = lambda player: self._step_player(
+        player=player, action_spec=override_action_spec
+    )
 
     if self._randomise_initiative:
       random.shuffle(players)
 
     if self._concurrent_action:
       with concurrent.futures.ThreadPoolExecutor() as executor:
-        executor.map(self._step_player, players)
+        executor.map(step_player_fn, players)
     else:
       for player in players:
-        self._step_player(player)
+        step_player_fn(player)
         if not self._players_act_simultaneously:
           self._clock.advance()
     if self._players_act_simultaneously:
       self._clock.advance()
 
   def run_episode(self, max_steps: int = 20) -> list[str]:
     for _ in range(max_steps):
```

### Comparing `gdm-concordia-1.2.0/concordia/environment/game_mater_test.py` & `gdm-concordia-1.3.0/concordia/environment/game_master_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     self.calls_sequence.append('update_after_event')
 
   def terminate_episode(self) -> bool:
     self.calls_sequence.append('terminate_episode')
     return False
 
 
-class GameMaterTest(parameterized.TestCase):
+class GameMasterTest(parameterized.TestCase):
 
   def test_calls_sequence(self):
     gm_call_tracker = CallTrackingComponent()
 
     model = mock_model.MockModel()
 
     importance_model = importance_function.ConstantImportanceModel()
@@ -157,21 +157,23 @@
     self.assertEqual(gm_call_tracker.calls_sequence, expected)
 
     alice_expected_calls = [
         'update',
         'observe',
         'state',
         'state',
+        'update_after_event',
     ]
     self.assertEqual(alice_call_tracker.calls_sequence, alice_expected_calls)
 
     bob_expected_calls = [
         'update',
         'observe',
         'state',
         'state',
+        'update_after_event',
     ]
     self.assertEqual(bob_call_tracker.calls_sequence, bob_expected_calls)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `gdm-concordia-1.2.0/concordia/environment/scenes/__init__.py` & `gdm-concordia-1.3.0/concordia/environment/scenes/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/environment/scenes/conversation.py` & `gdm-concordia-1.3.0/concordia/environment/scenes/conversation.py`

 * *Files 21% similar despite different names*

```diff
@@ -38,41 +38,47 @@
   """This component accumulates history of a conversation scene in its state."""
 
   def __init__(
       self,
       model: language_model.LanguageModel,
       players: Sequence[basic_agent.BasicAgent],
       premise: str = '',
+      check_for_termination: bool = True,
       verbose: bool = False,
       log_colour: str = 'red',
   ):
     """This component accumulates history of a conversation scene in its state.
 
     Args:
       model: a language model
       players: players participating
       premise: any extra text to be added on top of the conversation (say,
         circumstances of it)
+      check_for_termination: whether or not to check for termination of the
+        conversation
       verbose: whether or not to print intermediate reasoning steps
       log_colour: colour for logging
     """
     self._model = model
     self._state = premise
     self._log_colour = log_colour
     self._players = players
+    self._check_for_termination = check_for_termination
 
     self._verbose = verbose
 
   def name(self) -> str:
     return 'Conversation history'
 
   def state(self):
     return self._state
 
   def terminate_episode(self) -> bool:
+    if not self._check_for_termination:
+      return False
     chain_of_thought = interactive_document.InteractiveDocument(self._model)
     chain_of_thought.statement(f'Conversation:\n{self._state}\n')
 
     did_conclude = chain_of_thought.multiple_choice_question(
         'Is the conversation above over and not going to continue?',
         answers=['No', 'Yes'],
     )
@@ -97,37 +103,45 @@
 
 
 def make_conversation_game_master(
     players: Sequence[basic_agent.BasicAgent],
     clock: game_clock.MultiIntervalClock,
     model: language_model.LanguageModel,
     memory_factory: blank_memories.MemoryFactory,
+    call_to_speech: str = simulacrum_agent.DEFAULT_CALL_TO_SPEECH,
+    check_for_termination: bool = True,
+    randomise_initiative: bool = False,
     name: str = 'Conversation scene',
     premise: str = '',
     review_participants: bool = True,
 ):
   """Creates a game master that runs a conversation between players.
 
   Args:
     players: players participating
     clock: a clock
     model: a language model
     memory_factory: a memory factory
+    call_to_speech: prompt to use to invoke the agents speech
+    check_for_termination: whether or not to check for termination of the
+      conversation
+    randomise_initiative: whether or not to randomise the initiative of the
+      players at each step
     name: the name of the game master
     premise: any extra text to be added on top of the conversation (say,
       circumstances of it)
     review_participants: whether or not to start each conversation scene by
       declaring who its participants are.
 
   Returns:
     a game master
   """
 
   action_spec = simulacrum_agent.ActionSpec(
-      simulacrum_agent.DEFAULT_CALL_TO_SPEECH,
+      call_to_speech,
       'FREE',
       tag='speech',
   )
 
   agent_names = [player.name for player in players]
 
   convo = ''
@@ -144,16 +158,17 @@
 
   convo += 'Here is the conversation from the beginning:'
 
   conversation_tracker = ConversationTracker(
       model=model,
       players=players,
       premise=convo,
-      verbose=True,
+      verbose=False,
       log_colour='red',
+      check_for_termination=check_for_termination
   )
 
   for player in players:
     player.observe(convo)
 
   memory = memory_factory.make_blank_memory()
   game_master = game_master_lib.GameMaster(
@@ -161,13 +176,13 @@
       memory=memory,
       clock=clock,
       name=name,
       players=players,
       components=[conversation_tracker],
       action_spec=action_spec,
       update_thought_chain=[thought_chains.identity],
-      randomise_initiative=False,
+      randomise_initiative=randomise_initiative,
       player_observes_event=False,
       concurrent_externalities=False,
       verbose=True,
   )
   return game_master
```

### Comparing `gdm-concordia-1.2.0/concordia/language_model/__init__.py` & `gdm-concordia-1.3.0/concordia/language_model/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/language_model/gcloud_model.py` & `gdm-concordia-1.3.0/concordia/language_model/gcloud_model.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/language_model/gemini_vertex_model.py` & `gdm-concordia-1.3.0/concordia/language_model/gemini_vertex_model.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/language_model/gpt_model.py` & `gdm-concordia-1.3.0/concordia/language_model/gpt_model.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/language_model/language_model.py` & `gdm-concordia-1.3.0/concordia/language_model/language_model.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/language_model/retry_wrapper.py` & `gdm-concordia-1.3.0/concordia/language_model/retry_wrapper.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/metrics/__init__.py` & `gdm-concordia-1.3.0/concordia/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/metrics/common_sense_morality.py` & `gdm-concordia-1.3.0/concordia/metrics/common_sense_morality.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,21 +67,21 @@
 
   def name(
       self,
   ) -> str:
     """See base class."""
     return self._name
 
-  def observe(self, observation: str) -> None:
+  def update_after_event(self, action: str) -> None:
     """See base class."""
     doc = interactive_document.InteractiveDocument(self._model)
     answer = doc.multiple_choice_question(
         (
             f'Evaluate the following activity of {self._player_name} using'
-            f' common sense morality.\nActivity: {observation}\n'
+            f' common sense morality.\nActivity: {action}\n'
         ),
         self._scale,
     )
     answer_str = self._scale[answer]
 
     answer = float(answer) / float(len(self._scale) - 1)
```

### Comparing `gdm-concordia-1.2.0/concordia/metrics/dass_questionnaire.py` & `gdm-concordia-1.3.0/concordia/metrics/dass_questionnaire.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/metrics/goal_achievement.py` & `gdm-concordia-1.3.0/concordia/metrics/goal_achievement.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,22 +73,22 @@
 
   def name(
       self,
   ) -> str:
     """See base class."""
     return self._name
 
-  def observe(self, observation: str) -> None:
+  def update_after_event(self, action: str) -> None:
     """See base class."""
     doc = interactive_document.InteractiveDocument(self._model)
     answer = doc.multiple_choice_question(
         (
             'Evaluate if the following activity brings'
             f' {self._player_name} closer to their goal'
-            f' "{self._player_goal} .\n Activity: {observation}\n'
+            f' "{self._player_goal} .\n Activity: {action}\n'
         ),
         self._scale,
     )
     answer_str = self._scale[answer]
 
     answer = float(answer) / float(len(self._scale) - 1)
```

### Comparing `gdm-concordia-1.2.0/concordia/metrics/opinion_of_others.py` & `gdm-concordia-1.3.0/concordia/metrics/opinion_of_others.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/metrics/uncertainty_scale_question.py` & `gdm-concordia-1.3.0/concordia/metrics/uncertainty_scale_question.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from typing import Callable
 
 from concordia.document import interactive_document
 from concordia.language_model import language_model
 from concordia.typing import clock as game_clock
 from concordia.typing import component
 from concordia.utils import measurements as measurements_lib
+import termcolor
 
 
 DEFAULT_SCALE = (
     'Definitively not',
     'Maybe not',
     'Maybe yes',
     'Definitively yes',
@@ -118,14 +119,15 @@
         'player': self._player_name,
     }
     if self._measurements is not None:
       self._measurements.publish_datum(self._channel, datum)
 
     datum['time'] = self._clock.now()
     if self._verbose:
+      print(termcolor.colored(prompt.view().text(), 'green'), end='')
       print(f'{question}\n{self._player_name}: {answer_str}')
     self._timestep += 1
 
   def state(
       self,
   ) -> str | None:
     """Returns the current state of the component."""
```

### Comparing `gdm-concordia-1.2.0/concordia/tests/__init__.py` & `gdm-concordia-1.3.0/concordia/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/tests/concordia_integration_test.py` & `gdm-concordia-1.3.0/concordia/tests/concordia_integration_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,18 +38,18 @@
 
 
 def _make_agent(
     name: str,
     model: mock_model.MockModel,
     clock: game_clock.MultiIntervalClock,
     player_names: Sequence[str],
-    game_master_instructions: str,
+    agent_instructions: str,
     mem_factory: blank_memories.MemoryFactory,
 ) -> basic_agent.BasicAgent:
-  """Creates two agents with the same game master instructions."""
+  """Creates two agents with same instructions."""
   mem = mem_factory.make_blank_memory()
 
   goal_metric = goal_achievement.GoalAchievementMetric(
       model=model,
       player_name=name,
       player_goal='win',
       clock=clock,
@@ -70,20 +70,22 @@
       agent_name=name,
       clock_now=clock.now,
   )
   identity = agent_components.identity.SimIdentity(
       model=model,
       memory=mem,
       agent_name=name,
+      clock_now=clock.now,
   )
   goal_component = components.constant.ConstantComponent(state='test')
   plan = agent_components.plan.SimPlan(
       model=model,
       memory=mem,
       agent_name=name,
+      clock_now=clock.now,
       components=[identity],
       goal=goal_component,
       verbose=False,
   )
 
   self_perception = agent_components.self_perception.SelfPerception(
       name='self perception',
@@ -142,15 +144,15 @@
   agent = basic_agent.BasicAgent(
       model,
       mem,
       name,
       clock,
       [
           components.constant.ConstantComponent(
-              'Instructions:', game_master_instructions
+              'Instructions:', agent_instructions
           ),
           persona,
           observation,
           observation_summary,
           plan,
           somatic_state,
           time,
@@ -171,32 +173,28 @@
   return agent
 
 
 def _make_environment(
     model: mock_model.MockModel,
     clock: game_clock.MultiIntervalClock,
     players: Sequence[basic_agent.BasicAgent],
-    game_master_instructions: str,
     importance_model_gm: importance_function.ImportanceModel,
 ) -> game_master.GameMaster:
   """Creates a game master environment."""
   game_master_memory = associative_memory.AssociativeMemory(
       embedder, importance_model_gm.importance, clock=clock.now
   )
   player_names = [player.name for player in players]
 
   shared_memories = [
       'There is a hamlet named Riverbend.',
   ]
 
   shared_context = 'There is a hamlet named Riverbend.'
 
-  instructions_construct = components.constant.ConstantComponent(
-      game_master_instructions, 'Instructions'
-  )
   facts_on_village = components.constant.ConstantComponent(
       ' '.join(shared_memories), 'General knowledge of Riverbend'
   )
   player_status = gm_components.player_status.PlayerStatus(
       clock.now, model, game_master_memory, player_names
   )
 
@@ -211,15 +209,14 @@
       players,
       model,
       memory=game_master_memory,
       clock=clock,
       burner_memory_factory=mem_factory,
       components=[player_status],
       cap_nonplayer_characters=2,
-      game_master_instructions=game_master_instructions,
       shared_context=shared_context,
       verbose=False,
   )
 
   direct_effect_externality = gm_components.direct_effect.DirectEffect(
       players,
       memory=game_master_memory,
@@ -248,15 +245,14 @@
 
   env = game_master.GameMaster(
       model=model,
       memory=game_master_memory,
       clock=clock,
       players=players,
       components=[
-          instructions_construct,
           facts_on_village,
           player_status,
           schedule_construct,
           convo_externality,
           direct_effect_externality,
       ],
       randomise_initiative=True,
@@ -277,48 +273,47 @@
         start=datetime.datetime(hour=8, year=2024, month=9, day=1),
         step_sizes=[
             datetime.timedelta(hours=1),
             datetime.timedelta(seconds=10),
         ],
     )
 
-    game_master_instructions = 'This is a social science experiment.'
+    agent_instructions = 'This is a social science experiment.'
 
     mem_factory = blank_memories.MemoryFactory(
         model=model,
         embedder=embedder,
         importance=importance_model.importance,
         clock_now=clock.now,
     )
 
     alice = _make_agent(
         name='Alice',
         model=model,
         clock=clock,
         player_names=['Alice', 'Bob'],
-        game_master_instructions=game_master_instructions,
+        agent_instructions=agent_instructions,
         mem_factory=mem_factory,
     )
     bob = _make_agent(
         name='Bob',
         model=model,
         clock=clock,
         player_names=['Alice', 'Bob'],
-        game_master_instructions=game_master_instructions,
+        agent_instructions=agent_instructions,
         mem_factory=mem_factory,
     )
 
     players = [alice, bob]
 
     env = _make_environment(
-        model,
-        clock,
-        players,
-        game_master_instructions,
-        importance_model,
+        model=model,
+        clock=clock,
+        players=players,
+        importance_model_gm=importance_model,
     )
 
     env.run_episode(12)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `gdm-concordia-1.2.0/concordia/tests/mock_model.py` & `gdm-concordia-1.3.0/concordia/tests/mock_model.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/thought_chains/__init__.py` & `gdm-concordia-1.3.0/concordia/thought_chains/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/thought_chains/thought_chains.py` & `gdm-concordia-1.3.0/concordia/thought_chains/thought_chains.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,14 +40,50 @@
   Returns:
     string describing the outcome
   """
   del chain_of_thought, active_player_name
   return premise
 
 
+def extract_direct_quote(
+    chain_of_thought: interactive_document.InteractiveDocument,
+    action_attempt: str,
+    active_player_name: str,
+):
+  """Outputs the premise. Use this to create a pass-through chain of thought.
+
+  Args:
+    chain_of_thought: the document to condition on and record the thoughts
+    action_attempt: the attempted action
+    active_player_name: name of player whose turn it currently is
+
+  Returns:
+    string describing the action attempt
+  """
+  inner_chain_of_thought = chain_of_thought.new()
+  inner_chain_of_thought.statement(f'{action_attempt}')
+  proceed = inner_chain_of_thought.yes_no_question(
+      question=f'Did {active_player_name} explicitly say or write anything?')
+  if proceed:
+    proceed_with_exact = inner_chain_of_thought.yes_no_question(
+        question=(
+            f'Does the text state exactly what {active_player_name} said or '
+            'wrote?'))
+    if proceed_with_exact:
+      direct_quote = inner_chain_of_thought.open_question(
+          question=f'What exactly did {active_player_name} say or write?',
+          max_characters=3000,
+          max_tokens=2500,
+          terminators=(),
+      )
+      chain_of_thought.statement(f'[direct quote] {direct_quote}')
+
+  return action_attempt
+
+
 def determine_success_and_why(
     chain_of_thought: interactive_document.InteractiveDocument,
     action_attempt: str,
     active_player_name: str,
 ):
   """Determine success of action_attempt and reason for success/failure.
 
@@ -238,14 +274,47 @@
       'and not "The door may have been opened").',
       max_characters=3000,
       max_tokens=1500,
   )
   return causal_statement
 
 
+def restore_direct_quote(
+    chain_of_thought: interactive_document.InteractiveDocument,
+    event: str,
+    active_player_name: str,
+):
+  """Restore details from action attempt lost in subsequent processing.
+
+  Args:
+    chain_of_thought: the document to condition on and record the thoughts
+    event: the candidate event
+    active_player_name: name of player whose turn it currently is
+
+  Returns:
+    string describing the outcome
+  """
+  chain_of_thought.statement(
+      f'Candidate event statement which may have lost direct quotes: {event}')
+  event_with_quote = chain_of_thought.open_question(
+      question=(
+          'Incorporate the exact text of anything said or written ' +
+          f'by {active_player_name} into the candidate event statement. ' +
+          'Note that all direct quotes should have been tagged in the ' +
+          f'text above with [direct quote]. If {active_player_name} ' +
+          'said or wrote anything then their direct quote must be part of ' +
+          'the answer. It is also important to maintain as much detail as ' +
+          'possible from the latest candidate event statement.'),
+      max_characters=4000,
+      max_tokens=3500,
+      terminators=(),
+  )
+  return event_with_quote
+
+
 class AccountForAgencyOfOthers:
   """Prevents players from taking voluntary actions they do not agree to take.
   """
 
   def __init__(self,
                model: language_model.LanguageModel,
                players: Sequence[basic_agent.BasicAgent],
@@ -359,15 +428,16 @@
     premise: str,
     document: interactive_document.InteractiveDocument,
     active_player_name: str,
 ):
   """Run a chain of thoughts in the document.
 
   Args:
-    thoughts: a sequence of 'thougth' functions
+    thoughts: sequence of 'thought' functions each of which process a document
+      and candidate event string.
     premise:  the starting premise of the chain
     document: the working document
     active_player_name: name of player whose turn it currently is
 
   Returns:
     document: the final version of the document that recorded the chain
     conclusion: the result of the last thought
```

### Comparing `gdm-concordia-1.2.0/concordia/typing/__init__.py` & `gdm-concordia-1.3.0/concordia/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/typing/agent.py` & `gdm-concordia-1.3.0/concordia/typing/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,19 @@
 
 
 @dataclasses.dataclass(frozen=True)
 class ActionSpec:
   """A specification of the action that agent is queried for.
 
   Attributes:
-    call_to_action: fromated text that conditions agents response. {agent_name}
+    call_to_action: formatted text conditioning agent response. {agent_name}
       and {timedelta} will be inserted by the agent.
     output_type: type of output - FREE, CHOICE or FLOAT
     options: if multiple choice, then provide possible answers here
-    tag: a tag to add to the activity memory (e.g. action, speach, etc.)
+    tag: a tag to add to the activity memory (e.g. action, speech, etc.)
   """
 
   call_to_action: str
   output_type: str
   options: Sequence[str] | None = None
   tag: str | None = None
```

### Comparing `gdm-concordia-1.2.0/concordia/typing/clock.py` & `gdm-concordia-1.3.0/concordia/typing/clock.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/typing/component.py` & `gdm-concordia-1.3.0/concordia/typing/component.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/typing/game_master.py` & `gdm-concordia-1.3.0/concordia/typing/game_master.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/utils/__init__.py` & `gdm-concordia-1.3.0/concordia/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/utils/helper_functions.py` & `gdm-concordia-1.3.0/concordia/utils/helper_functions.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-"""Helper functions.
-"""
+"""Helper functions."""
 
 from collections.abc import Iterable, Sequence
+import concurrent
 import datetime
 
 from concordia.document import interactive_document
 from concordia.language_model import language_model
 from concordia.typing import component
 
 
@@ -60,14 +60,15 @@
 
   For a count noun you ask how *many* there are. For a mass noun you ask how
   *much* there is.
 
   Args:
     x: input string. It should be a noun.
     model: a language model
+
   Returns:
     True if x is a count noun and False if x is a mass noun.
   """
   examples = (
       'Question: is money a count noun? [yes/no]\n' + 'Answer: no\n'
       'Question: is coin a count noun? [yes/no]\n' + 'Answer: yes\n'
       'Question: is water a count noun? [yes/no]\n' + 'Answer: no\n'
@@ -75,18 +76,15 @@
       'Question: is token a count noun? [yes/no]\n' + 'Answer: yes\n'
   )
   idx, _, _ = model.sample_choice(
       prompt=(
           f'{examples}Question: is {x} a count noun? [yes/no]\n' + 'Answer: '),
       responses=['no', 'yes'],
   )
-  if idx == 0:
-    return False
-  if idx == 1:
-    return True
+  return idx == 1
 
 
 def timedelta_to_readable_str(td: datetime.timedelta):
   """Converts a datetime.timedelta object to a readable string."""
   hours = td.seconds // 3600
   minutes = (td.seconds % 3600) // 60
   seconds = td.seconds % 60
@@ -106,18 +104,46 @@
     readable_str += [
         f'{seconds} second' if seconds == 1 else f'{seconds} seconds'
     ]
 
   return ''.join(readable_str)
 
 
-def apply_recursively(parent_component: component.Component,
-                      function_name: str,
-                      function_arg: str | None = None) -> None:
+def apply_recursively(
+    parent_component: component.Component,
+    function_name: str,
+    function_arg: str | None = None,
+    concurrent_child_calls: bool = False,
+) -> None:
   """Recursively applies a function to each component in a tree of components.
+
+  Args:
+    parent_component: the component to apply the function to.
+    function_name: the name of the function to apply.
+    function_arg: the argument to pass to the function.
+    concurrent_child_calls: whether to call the function on child components
+      concurrently.
   """
+
+  if concurrent_child_calls:
+    with concurrent.futures.ThreadPoolExecutor(
+        max_workers=len(parent_component.get_components())
+    ) as executor:
+      for child_component in parent_component.get_components():
+        executor.submit(
+            apply_recursively,
+            child_component,
+            function_name,
+            function_arg=function_arg,
+            concurrent_child_calls=concurrent_child_calls,
+            executor=executor,
+        )
+  else:
+    for child_component in parent_component.get_components():
+      apply_recursively(
+          child_component, function_name, function_arg=function_arg
+      )
+
   if function_arg is None:
     getattr(parent_component, function_name)()
   else:
     getattr(parent_component, function_name)(function_arg)
-  for child_component in parent_component.get_components():
-    apply_recursively(child_component, function_name, function_arg=function_arg)
```

### Comparing `gdm-concordia-1.2.0/concordia/utils/html.py` & `gdm-concordia-1.3.0/concordia/utils/html.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/utils/measurements.py` & `gdm-concordia-1.3.0/concordia/utils/measurements.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/utils/measurements_test.py` & `gdm-concordia-1.3.0/concordia/utils/measurements_test.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/concordia/utils/plotting.py` & `gdm-concordia-1.3.0/concordia/utils/plotting.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,25 +22,26 @@
 import pandas as pd
 
 
 def plot_line_measurement_channel(measurements_obj: measurements.Measurements,
                                   channel_name: str,
                                   group_by: str = 'player',
                                   xaxis: str = 'time',
-                                  yaxis: str = 'value_float') -> None:
+                                  yaxis: str = 'value_float',
+                                  ax: plt.Axes = None) -> None:
   """Plots a pie chart of a measurement channel."""
   if channel_name not in measurements_obj.available_channels():
     raise ValueError(f'Unknown channel: {channel_name}')
 
   channel = measurements_obj.get_channel(channel_name)
   data = []
   channel.subscribe(on_next=data.append)
 
   plot_df_line(pd.DataFrame(data), channel_name, group_by=group_by, xaxis=xaxis,
-               yaxis=yaxis)
+               yaxis=yaxis, ax=ax)
 
 
 def plot_pie_measurement_channel(measurements_obj: measurements.Measurements,
                                  channel_name: str,
                                  group_by: str = 'player',
                                  value: str = 'value_str') -> None:
   """Plots a pie chart of a measurement channel."""
@@ -87,27 +88,31 @@
     plt.title(f'{title} of {player}')
 
 
 def plot_df_line(df: pd.DataFrame,
                  title: str = 'Metric',
                  group_by: str = 'player',
                  xaxis: str = 'time',
-                 yaxis: str = 'value_float') -> None:
+                 yaxis: str = 'value_float',
+                 ax: plt.Axes = None) -> None:
   """Plots a line chart of a dataframe.
 
   Args:
     df: The dataframe with data to plot.
     title: The title of the plot.
     group_by: Group data by this field, plot each one as a line in the figure.
     xaxis: The name of the column to use as the x-axis. If multiple entries have
       the same value in this field, the y-axis values are averaged.
     yaxis: The name of the column to use as the y-axis. The values in this
       column must be numerical.
+    ax: The axis to plot on. If None, uses the current axis.
   """
-  ax = plt.gca()
+  if ax is None:
+    ax = plt.gca()
+
   for player, group_df in df.groupby(group_by):
     group_df = group_df.groupby(xaxis).mean(numeric_only=True).reset_index()
     group_df.plot(x=xaxis, y=yaxis, label=player, ax=ax)
   plt.title(title)
 
 
 def plot_metric_pie(metric):
```

### Comparing `gdm-concordia-1.2.0/concordia/utils/text.py` & `gdm-concordia-1.3.0/concordia/utils/text.py`

 * *Files identical despite different names*

### Comparing `gdm-concordia-1.2.0/gdm_concordia.egg-info/PKG-INFO` & `gdm-concordia-1.3.0/gdm_concordia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdm-concordia
-Version: 1.2.0
+Version: 1.3.0
 Summary: A library for building a generative model of social interacions.
 Home-page: https://github.com/google-deepmind/concordia
 Author: DeepMind
 Author-email: noreply@google.com
 License: Apache 2.0
 Download-URL: https://github.com/google-deepmind/concordia/releases
 Keywords: multi-agent agent-based-simulation generative-agents python machine-learning
```

### Comparing `gdm-concordia-1.2.0/gdm_concordia.egg-info/SOURCES.txt` & `gdm-concordia-1.3.0/gdm_concordia.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -4,58 +4,66 @@
 setup.py
 concordia/__init__.py
 concordia/agents/__init__.py
 concordia/agents/basic_agent.py
 concordia/associative_memory/__init__.py
 concordia/associative_memory/associative_memory.py
 concordia/associative_memory/blank_memories.py
-concordia/associative_memory/embedder_st5.py
 concordia/associative_memory/formative_memories.py
 concordia/associative_memory/importance_function.py
 concordia/clocks/__init__.py
 concordia/clocks/game_clock.py
 concordia/clocks/game_clock_test.py
 concordia/components/__init__.py
 concordia/components/constant.py
 concordia/components/report_function.py
 concordia/components/sequential.py
 concordia/components/agent/__init__.py
+concordia/components/agent/all_similar_memories.py
 concordia/components/agent/characteristic.py
+concordia/components/agent/creative_reflection.py
+concordia/components/agent/dialectical_reflection.py
 concordia/components/agent/identity.py
 concordia/components/agent/observation.py
 concordia/components/agent/person_by_situation.py
 concordia/components/agent/plan.py
 concordia/components/agent/reflection.py
+concordia/components/agent/relationships.py
+concordia/components/agent/scheduled_hint.py
 concordia/components/agent/self_perception.py
 concordia/components/agent/situation_perception.py
 concordia/components/agent/somatic_state.py
 concordia/components/game_master/__init__.py
 concordia/components/game_master/conversation.py
+concordia/components/game_master/current_scene.py
+concordia/components/game_master/current_scene_test.py
 concordia/components/game_master/direct_effect.py
 concordia/components/game_master/inventory.py
 concordia/components/game_master/player_status.py
 concordia/components/game_master/player_status_test.py
 concordia/components/game_master/relevant_events.py
 concordia/components/game_master/schedule.py
 concordia/components/game_master/time_display.py
 concordia/document/__init__.py
 concordia/document/document.py
 concordia/document/document_test.py
 concordia/document/interactive_document.py
 concordia/document/interactive_document_test.py
 concordia/environment/__init__.py
 concordia/environment/game_master.py
-concordia/environment/game_mater_test.py
+concordia/environment/game_master_test.py
 concordia/environment/scenes/__init__.py
 concordia/environment/scenes/conversation.py
+concordia/environment/scenes/runner.py
 concordia/language_model/__init__.py
 concordia/language_model/gcloud_model.py
 concordia/language_model/gemini_vertex_model.py
 concordia/language_model/gpt_model.py
 concordia/language_model/language_model.py
+concordia/language_model/ollama_model.py
 concordia/language_model/retry_wrapper.py
 concordia/metrics/__init__.py
 concordia/metrics/common_sense_morality.py
 concordia/metrics/dass_questionnaire.py
 concordia/metrics/goal_achievement.py
 concordia/metrics/opinion_of_others.py
 concordia/metrics/uncertainty_scale_question.py
@@ -65,14 +73,15 @@
 concordia/thought_chains/__init__.py
 concordia/thought_chains/thought_chains.py
 concordia/typing/__init__.py
 concordia/typing/agent.py
 concordia/typing/clock.py
 concordia/typing/component.py
 concordia/typing/game_master.py
+concordia/typing/scene.py
 concordia/utils/__init__.py
 concordia/utils/helper_functions.py
 concordia/utils/html.py
 concordia/utils/measurements.py
 concordia/utils/measurements_test.py
 concordia/utils/plotting.py
 concordia/utils/text.py
```

### Comparing `gdm-concordia-1.2.0/pyproject.toml` & `gdm-concordia-1.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # TODO remove once https://github.com/PyCQA/isort/pull/2149 submitted.
 line_length = 1000
 single_line_exclusions = ["collections.abc", "typing", "typing_extensions"]
 known_thirdparty = ["concordia"]
 
 [tool.pyink]
 line-length = 80
-preview = true
+unstable = true
 pyink-indentation = 2
 pyink-use-majority-quotes = true
 
 [tool.pytest.ini_options]
 required_plugins = ["pytest-xdist"]
 addopts = "-n auto"
 testpaths = ["concordia", "examples"]
```

### Comparing `gdm-concordia-1.2.0/setup.py` & `gdm-concordia-1.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 """Install script for setuptools."""
 
 import setuptools
 
 setuptools.setup(
     name='gdm-concordia',
-    version='1.2.0',
+    version='1.3.0',
     license='Apache 2.0',
     license_files=['LICENSE'],
     url='https://github.com/google-deepmind/concordia',
     download_url='https://github.com/google-deepmind/concordia/releases',
     author='DeepMind',
     author_email='noreply@google.com',
     description=(
@@ -45,33 +45,31 @@
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
     ],
     packages=setuptools.find_packages(include=['concordia', 'concordia.*']),
     package_data={},
     python_requires='>=3.11',
-    install_requires=[
+    install_requires=(
         # TODO: b/312199199 - remove some requirements.
         'absl-py',
         'google-cloud-aiplatform',
         'ipython',
+        'langchain',
         'matplotlib',
         'numpy',
         'openai>=1.3.0',
         'pandas<=2.0.3',
         'python-dateutil',
         'reactivex',
         'retry',
         'scipy',
-        'tensorflow',
-        'tensorflow-hub',
-        'tensorflow-text',
         'termcolor',
         'typing-extensions',
-    ],
+    ),
     extras_require={
         # Used in development.
         'dev': [
             'build',
             'isort',
             'jupyter',
             'pipreqs',
```

