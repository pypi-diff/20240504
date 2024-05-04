# Comparing `tmp/pref_voting-1.2.0.tar.gz` & `tmp/pref_voting-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pref_voting-1.2.0.tar", max compression
+gzip compressed data, was "pref_voting-1.3.0.tar", max compression
```

## Comparing `pref_voting-1.2.0.tar` & `pref_voting-1.3.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1085 2024-03-19 19:26:58.359673 pref_voting-1.2.0/LICENSE
--rw-r--r--   0        0        0     1770 2024-04-24 21:45:43.110237 pref_voting-1.2.0/README.md
--rw-r--r--   0        0        0       22 2024-04-30 01:55:59.429329 pref_voting-1.2.0/pref_voting/__init__.py
--rw-r--r--   0        0        0    18867 2023-11-14 11:21:19.592605 pref_voting-1.2.0/pref_voting/analysis.py
--rw-r--r--   0        0        0     1270 2023-11-14 11:21:20.178458 pref_voting-1.2.0/pref_voting/axiom.py
--rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-1.2.0/pref_voting/axiom_helpers.py
--rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-1.2.0/pref_voting/axioms.py
--rw-r--r--   0        0        0    33205 2024-04-09 01:59:48.226095 pref_voting-1.2.0/pref_voting/c1_methods.py
--rw-r--r--   0        0        0    15161 2024-03-15 20:53:44.539281 pref_voting-1.2.0/pref_voting/combined_methods.py
--rw-r--r--   0        0        0    12827 2024-04-30 00:43:54.579498 pref_voting-1.2.0/pref_voting/dominance_axioms.py
--rw-r--r--   0        0        0    24283 2024-04-24 20:51:32.848337 pref_voting-1.2.0/pref_voting/generate_profiles.py
--rw-r--r--   0        0        0     7648 2023-09-26 23:38:41.018490 pref_voting-1.2.0/pref_voting/generate_spatial_profiles.py
--rw-r--r--   0        0        0     6181 2023-11-14 11:21:22.463664 pref_voting-1.2.0/pref_voting/generate_utility_profiles.py
--rw-r--r--   0        0        0    12781 2024-01-20 19:48:28.167312 pref_voting-1.2.0/pref_voting/generate_weighted_majority_graphs.py
--rw-r--r--   0        0        0     8796 2024-03-02 21:50:31.229821 pref_voting-1.2.0/pref_voting/grade_methods.py
--rw-r--r--   0        0        0    15536 2024-02-19 21:31:17.860108 pref_voting-1.2.0/pref_voting/grade_profiles.py
--rw-r--r--   0        0        0     8068 2024-04-19 01:31:48.812126 pref_voting-1.2.0/pref_voting/helper.py
--rw-r--r--   0        0        0    12710 2023-10-25 22:23:58.100791 pref_voting-1.2.0/pref_voting/invariance_axioms.py
--rw-r--r--   0        0        0        0 2024-03-17 12:02:53.705325 pref_voting-1.2.0/pref_voting/io/__init__.py
--rw-r--r--   0        0        0    17327 2024-04-15 10:20:24.422714 pref_voting-1.2.0/pref_voting/io/readers.py
--rw-r--r--   0        0        0     9283 2024-04-15 10:10:45.393951 pref_voting-1.2.0/pref_voting/io/writers.py
--rw-r--r--   0        0        0    93528 2024-04-30 00:49:36.509648 pref_voting-1.2.0/pref_voting/iterative_methods.py
--rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-1.2.0/pref_voting/maj_graph_ex1.png
--rw-r--r--   0        0        0    22586 2024-04-15 17:48:22.507316 pref_voting-1.2.0/pref_voting/mappings.py
--rw-r--r--   0        0        0    72109 2024-04-28 20:01:53.768039 pref_voting-1.2.0/pref_voting/margin_based_methods.py
--rw-r--r--   0        0        0    70814 2024-04-27 22:10:28.624211 pref_voting-1.2.0/pref_voting/margin_based_methods_old.py
--rw-r--r--   0        0        0    39807 2024-04-15 09:43:01.243011 pref_voting-1.2.0/pref_voting/monotonicity_axioms.py
--rw-r--r--   0        0        0    24548 2024-03-16 15:19:40.029463 pref_voting-1.2.0/pref_voting/other_methods.py
--rw-r--r--   0        0        0     2994 2024-04-15 22:33:37.313589 pref_voting-1.2.0/pref_voting/prob_voting_method.py
--rw-r--r--   0        0        0     4338 2024-04-15 22:36:04.584538 pref_voting-1.2.0/pref_voting/probabilistic_methods.py
--rw-r--r--   0        0        0    30126 2024-03-21 11:19:48.716586 pref_voting-1.2.0/pref_voting/profiles.py
--rw-r--r--   0        0        0    31608 2024-03-19 11:44:23.373414 pref_voting-1.2.0/pref_voting/profiles_with_ties.py
--rw-r--r--   0        0        0    13859 2024-03-03 16:50:37.545900 pref_voting-1.2.0/pref_voting/rankings.py
--rw-r--r--   0        0        0    22528 2024-04-30 01:19:53.430327 pref_voting-1.2.0/pref_voting/scoring_methods.py
--rw-r--r--   0        0        0     1891 2024-04-15 22:36:47.601045 pref_voting-1.2.0/pref_voting/social_welfare_function.py
--rw-r--r--   0        0        0      362 2024-02-16 02:11:21.780066 pref_voting-1.2.0/pref_voting/social_welfare_functions.py
--rw-r--r--   0        0        0     7395 2024-03-19 17:48:42.747157 pref_voting-1.2.0/pref_voting/spatial_profiles.py
--rw-r--r--   0        0        0    15790 2024-04-30 00:43:41.503635 pref_voting-1.2.0/pref_voting/strategic_axioms.py
--rw-r--r--   0        0        0     7833 2024-04-30 00:43:41.503770 pref_voting-1.2.0/pref_voting/swf_axioms.py
--rw-r--r--   0        0        0        0 2023-12-03 11:15:38.617857 pref_voting-1.2.0/pref_voting/tests/__init__.py
--rw-r--r--   0        0        0      745 2024-04-28 20:04:29.865701 pref_voting-1.2.0/pref_voting/tests/conftest.py
--rw-r--r--   0        0        0     5690 2024-04-28 20:01:53.768645 pref_voting-1.2.0/pref_voting/tests/test_c1_methods.py
--rw-r--r--   0        0        0     3092 2024-04-28 20:01:53.768816 pref_voting-1.2.0/pref_voting/tests/test_combined_methods.py
--rw-r--r--   0        0        0    12962 2024-04-24 20:08:43.229903 pref_voting-1.2.0/pref_voting/tests/test_generate_profiles.py
--rw-r--r--   0        0        0     2504 2024-03-19 18:59:44.204010 pref_voting-1.2.0/pref_voting/tests/test_generate_spatial_profile.py
--rw-r--r--   0        0        0    15002 2024-04-15 10:21:41.931501 pref_voting-1.2.0/pref_voting/tests/test_io.py
--rw-r--r--   0        0        0    11606 2024-04-28 20:41:27.682198 pref_voting-1.2.0/pref_voting/tests/test_iterative_methods.py
--rw-r--r--   0        0        0    11912 2024-03-16 21:03:40.865827 pref_voting-1.2.0/pref_voting/tests/test_majority_graph.py
--rw-r--r--   0        0        0     6284 2024-04-15 17:49:58.759298 pref_voting-1.2.0/pref_voting/tests/test_mapping.py
--rw-r--r--   0        0        0    10335 2024-04-28 12:01:51.077156 pref_voting-1.2.0/pref_voting/tests/test_margin_based_methods.py
--rw-r--r--   0        0        0     7778 2024-04-08 19:41:37.247861 pref_voting-1.2.0/pref_voting/tests/test_margin_graph.py
--rw-r--r--   0        0        0     3722 2024-03-17 11:44:20.741638 pref_voting-1.2.0/pref_voting/tests/test_other_methods.py
--rw-r--r--   0        0        0     1815 2024-04-15 22:34:08.166452 pref_voting-1.2.0/pref_voting/tests/test_prob_voting_method.py
--rw-r--r--   0        0        0    11558 2024-03-19 11:40:09.393149 pref_voting-1.2.0/pref_voting/tests/test_profile.py
--rw-r--r--   0        0        0    20184 2024-04-08 19:41:37.248346 pref_voting-1.2.0/pref_voting/tests/test_profile_with_ties.py
--rw-r--r--   0        0        0     8964 2024-03-17 10:17:34.347218 pref_voting-1.2.0/pref_voting/tests/test_ranking.py
--rw-r--r--   0        0        0     6234 2024-04-28 20:40:55.278187 pref_voting-1.2.0/pref_voting/tests/test_scoring_rules.py
--rw-r--r--   0        0        0     1531 2024-04-15 14:32:09.859043 pref_voting-1.2.0/pref_voting/tests/test_social_welfare_functions.py
--rw-r--r--   0        0        0     5459 2024-04-08 19:41:37.248846 pref_voting-1.2.0/pref_voting/tests/test_spatial_profile.py
--rw-r--r--   0        0        0     2429 2024-04-08 19:41:37.249181 pref_voting-1.2.0/pref_voting/tests/test_support_graph.py
--rw-r--r--   0        0        0     3808 2024-04-15 19:15:01.227825 pref_voting-1.2.0/pref_voting/tests/test_utility_function.py
--rw-r--r--   0        0        0     1943 2024-03-19 18:31:19.950002 pref_voting-1.2.0/pref_voting/tests/test_utility_functions.py
--rw-r--r--   0        0        0     1585 2024-04-08 19:41:37.249465 pref_voting-1.2.0/pref_voting/tests/test_voting_method.py
--rw-r--r--   0        0        0     3963 2024-04-08 22:35:46.799439 pref_voting-1.2.0/pref_voting/utility_functions.py
--rw-r--r--   0        0        0     7245 2024-02-16 01:32:30.000312 pref_voting-1.2.0/pref_voting/utility_methods.py
--rw-r--r--   0        0        0    12673 2024-02-19 23:28:54.492364 pref_voting-1.2.0/pref_voting/utility_profiles.py
--rw-r--r--   0        0        0    18724 2023-12-05 16:58:20.198435 pref_voting-1.2.0/pref_voting/variable_candidate_axioms.py
--rw-r--r--   0        0        0    91126 2024-04-28 20:01:53.769602 pref_voting-1.2.0/pref_voting/variable_voter_axioms.py
--rw-r--r--   0        0        0     6148 2024-04-30 01:20:56.462342 pref_voting-1.2.0/pref_voting/voting_method.py
--rw-r--r--   0        0        0     1341 2024-04-30 00:59:45.610622 pref_voting-1.2.0/pref_voting/voting_method_properties.py
--rw-r--r--   0        0        0      372 2023-11-14 00:06:58.907333 pref_voting-1.2.0/pref_voting/voting_methods.py
--rw-r--r--   0        0        0     2563 2024-04-30 01:26:13.410155 pref_voting-1.2.0/pref_voting/voting_methods_registry.py
--rw-r--r--   0        0        0    57320 2024-04-08 19:41:37.250216 pref_voting-1.2.0/pref_voting/weighted_majority_graphs.py
--rw-r--r--   0        0        0      760 2024-04-30 01:55:59.427023 pref_voting-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2855 1970-01-01 00:00:00.000000 pref_voting-1.2.0/setup.py
--rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 pref_voting-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-03-19 19:26:58.359673 pref_voting-1.3.0/LICENSE
+-rw-r--r--   0        0        0     1770 2024-04-24 21:45:43.110237 pref_voting-1.3.0/README.md
+-rw-r--r--   0        0        0       22 2024-05-04 21:41:10.493296 pref_voting-1.3.0/pref_voting/__init__.py
+-rw-r--r--   0        0        0    18867 2023-11-14 11:21:19.592605 pref_voting-1.3.0/pref_voting/analysis.py
+-rw-r--r--   0        0        0     1270 2023-11-14 11:21:20.178458 pref_voting-1.3.0/pref_voting/axiom.py
+-rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-1.3.0/pref_voting/axiom_helpers.py
+-rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-1.3.0/pref_voting/axioms.py
+-rw-r--r--   0        0        0    36802 2024-05-04 20:01:37.592836 pref_voting-1.3.0/pref_voting/c1_methods.py
+-rw-r--r--   0        0        0    17576 2024-05-04 20:17:22.935128 pref_voting-1.3.0/pref_voting/combined_methods.py
+-rw-r--r--   0        0        0    12837 2024-05-03 10:23:29.480445 pref_voting-1.3.0/pref_voting/dominance_axioms.py
+-rw-r--r--   0        0        0    24283 2024-04-24 20:51:32.848337 pref_voting-1.3.0/pref_voting/generate_profiles.py
+-rw-r--r--   0        0        0     7648 2023-09-26 23:38:41.018490 pref_voting-1.3.0/pref_voting/generate_spatial_profiles.py
+-rw-r--r--   0        0        0     6181 2023-11-14 11:21:22.463664 pref_voting-1.3.0/pref_voting/generate_utility_profiles.py
+-rw-r--r--   0        0        0    12781 2024-01-20 19:48:28.167312 pref_voting-1.3.0/pref_voting/generate_weighted_majority_graphs.py
+-rw-r--r--   0        0        0     8796 2024-03-02 21:50:31.229821 pref_voting-1.3.0/pref_voting/grade_methods.py
+-rw-r--r--   0        0        0    15536 2024-02-19 21:31:17.860108 pref_voting-1.3.0/pref_voting/grade_profiles.py
+-rw-r--r--   0        0        0     8068 2024-04-19 01:31:48.812126 pref_voting-1.3.0/pref_voting/helper.py
+-rw-r--r--   0        0        0    12710 2023-10-25 22:23:58.100791 pref_voting-1.3.0/pref_voting/invariance_axioms.py
+-rw-r--r--   0        0        0        0 2024-03-17 12:02:53.705325 pref_voting-1.3.0/pref_voting/io/__init__.py
+-rw-r--r--   0        0        0    17327 2024-04-15 10:20:24.422714 pref_voting-1.3.0/pref_voting/io/readers.py
+-rw-r--r--   0        0        0     9283 2024-04-15 10:10:45.393951 pref_voting-1.3.0/pref_voting/io/writers.py
+-rw-r--r--   0        0        0    98984 2024-05-04 20:01:36.763021 pref_voting-1.3.0/pref_voting/iterative_methods.py
+-rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-1.3.0/pref_voting/maj_graph_ex1.png
+-rw-r--r--   0        0        0    22586 2024-04-15 17:48:22.507316 pref_voting-1.3.0/pref_voting/mappings.py
+-rw-r--r--   0        0        0    75213 2024-05-04 20:04:04.180220 pref_voting-1.3.0/pref_voting/margin_based_methods.py
+-rw-r--r--   0        0        0    70814 2024-04-27 22:10:28.624211 pref_voting-1.3.0/pref_voting/margin_based_methods_old.py
+-rw-r--r--   0        0        0    39807 2024-04-15 09:43:01.243011 pref_voting-1.3.0/pref_voting/monotonicity_axioms.py
+-rw-r--r--   0        0        0    30057 2024-05-04 20:35:29.533768 pref_voting-1.3.0/pref_voting/other_methods.py
+-rw-r--r--   0        0        0     2994 2024-04-15 22:33:37.313589 pref_voting-1.3.0/pref_voting/prob_voting_method.py
+-rw-r--r--   0        0        0     4338 2024-04-15 22:36:04.584538 pref_voting-1.3.0/pref_voting/probabilistic_methods.py
+-rw-r--r--   0        0        0    30126 2024-03-21 11:19:48.716586 pref_voting-1.3.0/pref_voting/profiles.py
+-rw-r--r--   0        0        0    31608 2024-03-19 11:44:23.373414 pref_voting-1.3.0/pref_voting/profiles_with_ties.py
+-rw-r--r--   0        0        0    13859 2024-03-03 16:50:37.545900 pref_voting-1.3.0/pref_voting/rankings.py
+-rw-r--r--   0        0        0    22958 2024-05-04 20:03:48.499502 pref_voting-1.3.0/pref_voting/scoring_methods.py
+-rw-r--r--   0        0        0     1891 2024-04-15 22:36:47.601045 pref_voting-1.3.0/pref_voting/social_welfare_function.py
+-rw-r--r--   0        0        0      362 2024-02-16 02:11:21.780066 pref_voting-1.3.0/pref_voting/social_welfare_functions.py
+-rw-r--r--   0        0        0     7395 2024-03-19 17:48:42.747157 pref_voting-1.3.0/pref_voting/spatial_profiles.py
+-rw-r--r--   0        0        0    15790 2024-04-30 00:43:41.503635 pref_voting-1.3.0/pref_voting/strategic_axioms.py
+-rw-r--r--   0        0        0     7881 2024-05-01 10:27:56.905820 pref_voting-1.3.0/pref_voting/swf_axioms.py
+-rw-r--r--   0        0        0        0 2023-12-03 11:15:38.617857 pref_voting-1.3.0/pref_voting/tests/__init__.py
+-rw-r--r--   0        0        0      745 2024-04-28 20:04:29.865701 pref_voting-1.3.0/pref_voting/tests/conftest.py
+-rw-r--r--   0        0        0     5690 2024-04-28 20:01:53.768645 pref_voting-1.3.0/pref_voting/tests/test_c1_methods.py
+-rw-r--r--   0        0        0     3092 2024-04-28 20:01:53.768816 pref_voting-1.3.0/pref_voting/tests/test_combined_methods.py
+-rw-r--r--   0        0        0    12962 2024-04-24 20:08:43.229903 pref_voting-1.3.0/pref_voting/tests/test_generate_profiles.py
+-rw-r--r--   0        0        0     2504 2024-03-19 18:59:44.204010 pref_voting-1.3.0/pref_voting/tests/test_generate_spatial_profile.py
+-rw-r--r--   0        0        0    15002 2024-04-15 10:21:41.931501 pref_voting-1.3.0/pref_voting/tests/test_io.py
+-rw-r--r--   0        0        0    11606 2024-04-28 20:41:27.682198 pref_voting-1.3.0/pref_voting/tests/test_iterative_methods.py
+-rw-r--r--   0        0        0    11912 2024-03-16 21:03:40.865827 pref_voting-1.3.0/pref_voting/tests/test_majority_graph.py
+-rw-r--r--   0        0        0     6284 2024-04-15 17:49:58.759298 pref_voting-1.3.0/pref_voting/tests/test_mapping.py
+-rw-r--r--   0        0        0    10335 2024-04-28 12:01:51.077156 pref_voting-1.3.0/pref_voting/tests/test_margin_based_methods.py
+-rw-r--r--   0        0        0     7778 2024-04-08 19:41:37.247861 pref_voting-1.3.0/pref_voting/tests/test_margin_graph.py
+-rw-r--r--   0        0        0     3722 2024-03-17 11:44:20.741638 pref_voting-1.3.0/pref_voting/tests/test_other_methods.py
+-rw-r--r--   0        0        0     1815 2024-04-15 22:34:08.166452 pref_voting-1.3.0/pref_voting/tests/test_prob_voting_method.py
+-rw-r--r--   0        0        0    11558 2024-03-19 11:40:09.393149 pref_voting-1.3.0/pref_voting/tests/test_profile.py
+-rw-r--r--   0        0        0    20184 2024-04-08 19:41:37.248346 pref_voting-1.3.0/pref_voting/tests/test_profile_with_ties.py
+-rw-r--r--   0        0        0     8964 2024-03-17 10:17:34.347218 pref_voting-1.3.0/pref_voting/tests/test_ranking.py
+-rw-r--r--   0        0        0     6234 2024-04-28 20:40:55.278187 pref_voting-1.3.0/pref_voting/tests/test_scoring_rules.py
+-rw-r--r--   0        0        0     1531 2024-04-15 14:32:09.859043 pref_voting-1.3.0/pref_voting/tests/test_social_welfare_functions.py
+-rw-r--r--   0        0        0     5459 2024-04-08 19:41:37.248846 pref_voting-1.3.0/pref_voting/tests/test_spatial_profile.py
+-rw-r--r--   0        0        0     2429 2024-04-08 19:41:37.249181 pref_voting-1.3.0/pref_voting/tests/test_support_graph.py
+-rw-r--r--   0        0        0     3808 2024-04-15 19:15:01.227825 pref_voting-1.3.0/pref_voting/tests/test_utility_function.py
+-rw-r--r--   0        0        0     1943 2024-03-19 18:31:19.950002 pref_voting-1.3.0/pref_voting/tests/test_utility_functions.py
+-rw-r--r--   0        0        0     1585 2024-04-08 19:41:37.249465 pref_voting-1.3.0/pref_voting/tests/test_voting_method.py
+-rw-r--r--   0        0        0     3963 2024-04-08 22:35:46.799439 pref_voting-1.3.0/pref_voting/utility_functions.py
+-rw-r--r--   0        0        0     7245 2024-02-16 01:32:30.000312 pref_voting-1.3.0/pref_voting/utility_methods.py
+-rw-r--r--   0        0        0    12673 2024-02-19 23:28:54.492364 pref_voting-1.3.0/pref_voting/utility_profiles.py
+-rw-r--r--   0        0        0    18724 2023-12-05 16:58:20.198435 pref_voting-1.3.0/pref_voting/variable_candidate_axioms.py
+-rw-r--r--   0        0        0    91144 2024-05-03 10:23:29.483544 pref_voting-1.3.0/pref_voting/variable_voter_axioms.py
+-rw-r--r--   0        0        0     6148 2024-04-30 01:20:56.462342 pref_voting-1.3.0/pref_voting/voting_method.py
+-rw-r--r--   0        0        0     1341 2024-04-30 00:59:45.610622 pref_voting-1.3.0/pref_voting/voting_method_properties.py
+-rw-r--r--   0        0        0      254 2024-05-04 20:05:10.058403 pref_voting-1.3.0/pref_voting/voting_methods.py
+-rw-r--r--   0        0        0     4679 2024-05-04 21:29:02.086406 pref_voting-1.3.0/pref_voting/voting_methods_registry.py
+-rw-r--r--   0        0        0    57320 2024-04-08 19:41:37.250216 pref_voting-1.3.0/pref_voting/weighted_majority_graphs.py
+-rw-r--r--   0        0        0      760 2024-05-04 21:41:10.492260 pref_voting-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2855 1970-01-01 00:00:00.000000 pref_voting-1.3.0/setup.py
+-rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 pref_voting-1.3.0/PKG-INFO
```

### Comparing `pref_voting-1.2.0/LICENSE` & `pref_voting-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/README.md` & `pref_voting-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/analysis.py` & `pref_voting-1.3.0/pref_voting/analysis.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/axiom.py` & `pref_voting-1.3.0/pref_voting/axiom.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/c1_methods.py` & `pref_voting-1.3.0/pref_voting/c1_methods.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,16 +14,23 @@
 from pref_voting.rankings import Ranking, break_ties_alphabetically
 from pref_voting.social_welfare_function import swf
 import copy
 import math
 from itertools import product, permutations, combinations, chain
 import networkx as nx
 import matplotlib.pyplot as plt
+from pref_voting.voting_method_properties import VotingMethodProperties, ElectionTypes
 
-@vm(name = "Condorcet")
+condorcet_properties = VotingMethodProperties(
+    condorcet_winner=True,
+    condorcet_loser=False,
+    pareto_dominance=False,)
+@vm(name = "Condorcet",
+    properties = condorcet_properties,
+    input_types = [ElectionTypes.PROFILE, ElectionTypes.PROFILE_WITH_TIES, ElectionTypes.MAJORITY_GRAPH, ElectionTypes.MARGIN_GRAPH])
 def condorcet(edata, curr_cands = None):
     """
     Return the Condorcet winner if one exists, otherwise return all the candidates.  A Condorcet winner is a candidate :math:`c` that is majority preferred to every other candidate. 
 
     Args:
         edata (Profile, ProfileWithTies, MajorityGraph, MarginGraph): Any election data that has a `condorcet_winner` method. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
@@ -61,16 +68,21 @@
     """
    
     candidates = edata.candidates if curr_cands is None else curr_cands
     cond_winner = edata.condorcet_winner(curr_cands = curr_cands)
     
     return [cond_winner] if cond_winner is not None else sorted(candidates)
 
-
-@vm(name = "Copeland")
+copeland_properties = VotingMethodProperties(
+    condorcet_winner=True,
+    condorcet_loser=True,
+    pareto_dominance=True,)
+@vm(name = "Copeland",
+    properties = copeland_properties,
+    input_types = [ElectionTypes.PROFILE, ElectionTypes.PROFILE_WITH_TIES, ElectionTypes.MAJORITY_GRAPH, ElectionTypes.MARGIN_GRAPH])
 def copeland(edata, curr_cands = None):
     """The Copeland score for c is the number of candidates that c is majority preferred to minus the number of candidates majority preferred to c.  The Copeland winners are the candidates with the maximum Copeland score in the profile restricted to ``curr_cands``. 
 
     Args:
         edata (Profile, ProfileWithTies, MajorityGraph, MarginGraph): Any election data that has a `copeland_scores` method. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
@@ -142,15 +154,22 @@
     copeland_ranking.normalize_ranks()
 
     if tie_breaking == "alphabetic":
         copeland_ranking = break_ties_alphabetically(copeland_ranking)
 
     return copeland_ranking
 
-@vm(name = "Llull")
+
+llull_properties = VotingMethodProperties(
+    condorcet_winner=True,
+    condorcet_loser=True,
+    pareto_dominance=True,)
+@vm(name = "Llull",
+    properties = llull_properties,
+    input_types = [ElectionTypes.PROFILE, ElectionTypes.PROFILE_WITH_TIES, ElectionTypes.MAJORITY_GRAPH, ElectionTypes.MARGIN_GRAPH])
 def llull(edata, curr_cands = None):
     """The Llull score for a candidate :math:`c` is the number of candidates that :math:`c` is weakly majority preferred to.  This is equivalent to calculating the Copeland scores for a candidate :math:`c` with 1 point for each candidate that :math:`c` is majority preferred to, 1/2 point for each candidate that :math:`c` is tied with, and 0 points for each candidate that is majority preferred to :math:`c`.  The Llull winners are the candidates with the maximum Llull score in the profile restricted to ``curr_cands``. 
 
     Args:
         edata (Profile, ProfileWithTies, MajorityGraph, MarginGraph): Any election data that has a `copeland_scores` method. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
@@ -201,16 +220,21 @@
 
 def right_covers(dom, c1, c2):
     # right covers: c1 right covers c2 when all the candidates that c2  majority preferrs are majority
     # preferred by c1
       
     return dom[c2].issubset(dom[c1])
 
-
-@vm(name = "Uncovered Set")
+uc_gill_properties = VotingMethodProperties(
+    condorcet_winner=True,
+    condorcet_loser=True,
+    pareto_dominance=True,)
+@vm(name = "Uncovered Set",
+    properties = uc_gill_properties,
+    input_types = [ElectionTypes.PROFILE, ElectionTypes.PROFILE_WITH_TIES, ElectionTypes.MAJORITY_GRAPH, ElectionTypes.MARGIN_GRAPH])
 def uc_gill(edata, curr_cands = None): 
     """Uncovered Set (Gillies version):  Given candidates :math:`a` and :math:`b`, say that :math:`a` defeats :math:`b` in the election if :math:`a` is majority preferred to :math:`b` and :math:`a` left covers :math:`b`: i.e., for all :math:`c`, if :math:`c` is majority preferred to :math:`a`,  then :math:`c` majority preferred to :math:`b`. The winners are the set of candidates who are undefeated in the election restricted to ``curr_cands``. 
     
     Args:
         edata (Profile, ProfileWithTies, MajorityGraph, MarginGraph): Any election data that has a `dominators` method. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
@@ -293,16 +317,21 @@
         for c2 in edata.dominators(c1, curr_cands = curr_cands): # consider only c2 predecessors
             if c1 != c2:
                 # check if c2 left covers  c1 
                 if left_covers(dom, c2, c1):
                     defeat.add_edge(c2, c1)
     return defeat
 
-
-@vm(name = "Uncovered Set - Fishburn")
+uc_fish_properties = VotingMethodProperties(
+    condorcet_winner=True,
+    condorcet_loser=True,
+    pareto_dominance=True,)
+@vm(name = "Uncovered Set - Fishburn",
+    properties = uc_fish_properties,
+    input_types = [ElectionTypes.PROFILE, ElectionTypes.PROFILE_WITH_TIES, ElectionTypes.MAJORITY_GRAPH, ElectionTypes.MARGIN_GRAPH])
 def uc_fish(edata, curr_cands = None): 
     """Uncovered Set (Fishburn version):  Given candidates :math:`a` and :math:`b`, say that :math:`a` defeats :math:`b` in the election :math:`a` left covers :math:`b`: i.e., for all :math:`c`, if :math:`c` is majority preferred to :math:`a`,  then :math:`c` majority preferred to :math:`b`. The winners are the set of candidates who are undefeated in the election restricted to ``curr_cands``. 
     
     Args:
         edata (Profile, ProfileWithTies, MajorityGraph, MarginGraph): Any election data that has a `dominators` method. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
@@ -384,16 +413,21 @@
         for c2 in candidates:
             if c1 != c2:
                 # check if c2 left covers  c1 but c1 does not left cover c2
                 if left_covers(dom, c2, c1)  and not left_covers(dom, c1, c2):
                     defeat.add_edge(c2, c1)
     return defeat
 
-
-@vm(name = "Uncovered Set - Bordes")
+uc_bordes_properties = VotingMethodProperties(
+    condorcet_winner=True,
+    condorcet_loser=True,
+    pareto_dominance=True,)
+@vm(name = "Uncovered Set - Bordes",
+    properties = uc_fish_properties,
+    input_types = [ElectionTypes.PROFILE, ElectionTypes.PROFILE_WITH_TIES, ElectionTypes.MAJORITY_GRAPH, ElectionTypes.MARGIN_GRAPH])
 def uc_bordes(edata, curr_cands = None): 
     """Uncovered Set (Bordes version):  Given candidates :math:`a` and :math:`b`, say that :math:`a` Bordes covers :math:`b` if :math:`a` is majority preferred to :math:`b` and for all :math:`c`, if :math:`c` is majority preferred or tied with :math:`a`, then :math:`c` is majority preferred to or tied with :math:`b`. The winners are the set of candidates who are not Bordes covered in the election restricted to ``curr_cands``. 
     
     Args:
         edata (Profile, ProfileWithTies, MajorityGraph, MarginGraph): Any election data that has  `dominators` and `majority_prefers` methods. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
@@ -442,15 +476,21 @@
                 # check if c2 left covers  c1 
                 if left_covers(dom, c2, c1):
                     is_in_ucs = False
         if is_in_ucs:
             uc_set.append(c1)
     return list(sorted(uc_set))  
 
-@vm(name = "Uncovered Set - McKelvey")
+uc_mckelvey_properties = VotingMethodProperties(
+    condorcet_winner=True,
+    condorcet_loser=True,
+    pareto_dominance=True,)
+@vm(name = "Uncovered Set - McKelvey",
+    properties = uc_fish_properties,
+    input_types = [ElectionTypes.PROFILE, ElectionTypes.PROFILE_WITH_TIES, ElectionTypes.MAJORITY_GRAPH, ElectionTypes.MARGIN_GRAPH])
 def uc_mckelvey(edata, curr_cands = None): 
     """Uncovered Set (McKelvey version):  Given candidates :math:`a` and :math:`b`, say that  :math:`a` McKelvey covers :math:`b` if a Gillies covers :math:`b` and :math:`a` Bordes covers :math:`b`. The winners are the set of candidates who are not McKelvey covered in the election restricted to ``curr_cands``. 
     
     Args:
         edata (Profile, ProfileWithTies, MajorityGraph, MarginGraph): Any election data that has  `dominators` and `majority_prefers` methods. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
@@ -458,16 +498,15 @@
         A sorted list of candidates
 
     .. seealso::
 
         :func:`pref_voting.c1_methods.uc_gill`, :func:`pref_voting.c1_methods.uc_fish`, :func:`pref_voting.c1_methods.uc_bordes`
 
     :Example: 
-        
-        
+         
     .. plot::  margin_graphs_examples/mg_ex_uncovered_sets.py
         :context: reset  
         :include-source: True
 
 
     .. code-block:: 
 
@@ -498,15 +537,21 @@
                 # check if c2 left covers  c1 
                 if left_covers(strict_dom, c2, c1) and left_covers(weak_dom, c2, c1):
                     is_in_ucs = False
         if is_in_ucs:
             uc_set.append(c1)
     return list(sorted(uc_set))      
 
-@vm(name = "Top Cycle")
+top_cycle_properties = VotingMethodProperties(
+    condorcet_winner=True,
+    condorcet_loser=True,
+    pareto_dominance=True,)
+@vm(name = "Top Cycle",
+    properties = top_cycle_properties,
+    input_types = [ElectionTypes.PROFILE, ElectionTypes.PROFILE_WITH_TIES, ElectionTypes.MAJORITY_GRAPH, ElectionTypes.MARGIN_GRAPH])
 def top_cycle(edata, curr_cands = None):
     """The smallest set of candidates such that every candidate inside the set is majority preferred to every candidate outside the set.  
     
     Args:
         edata (Profile, ProfileWithTies, MajorityGraph, MarginGraph): Any election data that has a `majority_prefers` method. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
@@ -554,16 +599,19 @@
     min_indegree = min([max([wmg.in_degree(n) for n in comp]) for comp in scc])
     smith = [comp for comp in scc if max([wmg.in_degree(n) for n in comp]) == min_indegree][0]
     return sorted(list(smith))
 
 # Create some aliases for Top Cycle
 top_cycle.set_name("GETCHA")
 getcha = copy.deepcopy(top_cycle)
+getcha.skip_registration = True
+
 top_cycle.set_name("Smith Set")
 smith_set = copy.deepcopy(top_cycle)
+smith_set.skip_registration = True
 
 # reset the name Top Cycle
 top_cycle.set_name("Top Cycle")
 
 def top_cycle_defeat(edata, curr_cands = None):
     """Return the defeat relation associated with the Top Cycle voting method. 
     
@@ -590,16 +638,21 @@
     candidates = edata.candidates if curr_cands is None else curr_cands
     smith_set = top_cycle(edata, curr_cands = candidates)
     
     defeat.add_nodes_from(candidates)
     defeat.add_edges_from([(a, b) for a in candidates for b in candidates if a != b and a in smith_set and b not in smith_set])
     return defeat
 
-
-@vm(name = "GOCHA")
+gocha_properties = VotingMethodProperties(
+    condorcet_winner=True,
+    condorcet_loser=True,
+    pareto_dominance=True,)
+@vm(name = "GOCHA",
+    properties = gocha_properties,
+    input_types = [ElectionTypes.PROFILE, ElectionTypes.PROFILE_WITH_TIES, ElectionTypes.MAJORITY_GRAPH, ElectionTypes.MARGIN_GRAPH])
 def gocha(edata, curr_cands = None):
     """The GOCHA set (also known as the Schwartz set) is the set of all candidates x such that if y can reach x in the transitive closer of the majority relation, then x can reach y in the transitive closer of the majority relation.
       
     Args:
         edata (Profile, ProfileWithTies, MajorityGraph, MarginGraph): Any election data that has a `majority_prefers` method. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
@@ -646,14 +699,15 @@
                     for c1 in ssc for c2 in transitive_closure.nodes if c2 not in ssc]):
             schwartz =  schwartz.union(ssc)
     return sorted(list(schwartz))
 
 # Create some aliases for GOCHA
 gocha.set_name("Schwartz Set")
 schwartz_set = copy.deepcopy(gocha)
+schwartz_set.skip_registration = True
 
 # reset the name GETCHA
 gocha.set_name("GOCHA")
 
 
 ## Banks
 #
@@ -669,15 +723,21 @@
                 return False
     return True
 
 def is_subsequence(x, y):
     it = iter(y)
     return all(any(c == ch for c in it) for ch in x)
 
-@vm(name = "Banks")
+banks_properties = VotingMethodProperties(
+    condorcet_winner=True,
+    condorcet_loser=True,
+    pareto_dominance=True,)
+@vm(name = "Banks",
+    properties = banks_properties,
+    input_types = [ElectionTypes.PROFILE, ElectionTypes.PROFILE_WITH_TIES, ElectionTypes.MAJORITY_GRAPH, ElectionTypes.MARGIN_GRAPH])
 def banks(edata, curr_cands = None): 
     """ Say that a *chain* in majority graph is a subset of candidates that is linearly ordered by the majority relation. Then a candidate :math:`a` if :math:`a` is the maximum element with respect to the majority relation of some maximal chain in the majority graph.
 
     Args:
         edata (Profile, ProfileWithTies, MarginGraph): Any election data that has a `margin` method. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
@@ -850,16 +910,21 @@
         if dist < min_dist: 
             min_dist = dist
             rankings = [lin_order]
         elif dist == min_dist: 
             rankings.append(lin_order)
     return rankings, min_dist
 
-        
-@vm(name = "Slater")
+slater_properties = VotingMethodProperties(
+    condorcet_winner=True,
+    condorcet_loser=True,
+    pareto_dominance=True,)
+@vm(name = "Slater",
+    properties = slater_properties,
+    input_types = [ElectionTypes.PROFILE, ElectionTypes.PROFILE_WITH_TIES, ElectionTypes.MAJORITY_GRAPH, ElectionTypes.MARGIN_GRAPH])
 def slater(edata, curr_cands = None): 
     """A Slater ranking is a linear order :math:`R` of the candidates that minimizes the number of edges in the majority graph we have to turn around before we obtain :math:`R`.   A candidate is a Slater winner if the candidate is the top element of some Slater ranking.
 
     Args:
         edata (Profile, ProfileWithTies, MarginGraph): Any election data that has a `margin` method. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
@@ -892,44 +957,35 @@
         slater.display(mg)
 
     """    
     rankings, dist = slater_rankings(edata, curr_cands = curr_cands)
     
     return sorted(list(set([r[0] for r in rankings])))
 
-
-@vm(name="Bipartisan Set")
+bipartisan_properties = VotingMethodProperties(
+    condorcet_winner=True,
+    condorcet_loser=True,
+    pareto_dominance=True,)
+@vm(name = "Bipartisan Set",
+    properties = bipartisan_properties,
+    input_types = [ElectionTypes.PROFILE, ElectionTypes.PROFILE_WITH_TIES, ElectionTypes.MAJORITY_GRAPH, ElectionTypes.MARGIN_GRAPH])
 def bipartisan(edata, curr_cands = None, threshold = 0.0000001): 
     """The Bipartisan Set is the support of the (chosen) C1 maximal lottery.
 
     Args:
         edata (Profile, ProfileWithTies, MajorityGraph, MarginGraph): Any election data that has a `margin_matrix` attribute.
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
     Returns:
         A sorted list of candidates.
     """
 
     ml = c1_maximal_lottery(edata, curr_cands=curr_cands)
     return sorted([c for c in ml.keys() if  ml[c] > threshold])
 
-
-c1_vms = [
-    banks,
-    condorcet,
-    copeland,
-    llull,
-    uc_gill,
-    uc_fish,
-    uc_bordes,
-    uc_mckelvey,
-    top_cycle,
-    gocha,
-]
-
 c1_swf = [
     copeland_ranking
 ]
 
 defeat_methods = [
     top_cycle_defeat,
     uc_gill_defeat,
```

### Comparing `pref_voting-1.2.0/pref_voting/dominance_axioms.py` & `pref_voting-1.3.0/pref_voting/dominance_axioms.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,15 @@
         Result of the test (bool): Returns True if there is a violation and False otherwise. 
 
     """
 
     s_set = smith_set(edata)
     ws = vm(edata)
 
-    winners_not_in_smith = [w not in s_set for w in ws]
+    winners_not_in_smith = [w for w in ws if w not in s_set]
     if len(winners_not_in_smith) > 0: 
         if verbose:
             if type(edata) == Profile or type(edata) == ProfileWithTies: 
                 edata.display_margin_graph()
             else: 
                 edata.display()
             print(f"The winners that are not in the Smith set: {list_to_string(winners_not_in_smith, edata.cmap)}.")
@@ -255,15 +255,15 @@
         Result of the test (bool): Returns True if there is a violation and False otherwise. 
 
     """
 
     s_set = smith_set(edata)
     ws = vm(edata)
 
-    winners_not_in_smith = [w not in s_set for w in ws]
+    winners_not_in_smith = [w for w in ws if w not in s_set]
     if len(winners_not_in_smith) > 0: 
         if verbose:
             if type(edata) == Profile or type(edata) == ProfileWithTies: 
                 edata.display_margin_graph()
             else: 
                 edata.display()
             print(f"The winners that are not in the Smith set: {list_to_string(winners_not_in_smith, edata.cmap)}.")
```

### Comparing `pref_voting-1.2.0/pref_voting/generate_profiles.py` & `pref_voting-1.3.0/pref_voting/generate_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/generate_spatial_profiles.py` & `pref_voting-1.3.0/pref_voting/generate_spatial_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/generate_utility_profiles.py` & `pref_voting-1.3.0/pref_voting/generate_utility_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/generate_weighted_majority_graphs.py` & `pref_voting-1.3.0/pref_voting/generate_weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/grade_methods.py` & `pref_voting-1.3.0/pref_voting/grade_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/grade_profiles.py` & `pref_voting-1.3.0/pref_voting/grade_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/helper.py` & `pref_voting-1.3.0/pref_voting/helper.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/invariance_axioms.py` & `pref_voting-1.3.0/pref_voting/invariance_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/io/readers.py` & `pref_voting-1.3.0/pref_voting/io/readers.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/io/writers.py` & `pref_voting-1.3.0/pref_voting/io/writers.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/iterative_methods.py` & `pref_voting-1.3.0/pref_voting/iterative_methods.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from pref_voting.margin_based_methods import split_cycle, minimax_scores
 from pref_voting.c1_methods import top_cycle, gocha
 from pref_voting.rankings import Ranking
 from pref_voting.social_welfare_function import swf
 import copy
 from itertools import permutations, product
 import numpy as np
+from pref_voting.voting_method_properties import VotingMethodProperties, ElectionTypes
+
 
 def _instant_runoff_basic(profile,curr_cands = None):
     "The basic implementation of instant runoff"
     # need the total number of all candidates in a profile to check when all candidates have been removed   
     num_cands = profile.num_cands 
     
     candidates = profile.candidates if curr_cands is None else curr_cands
@@ -61,15 +63,22 @@
 
     if len(lowest_first_place_votes) == len(candidates):
         return sorted(lowest_first_place_votes)
     
     else:
         return _instant_runoff_recursive(profile, [c for c in candidates if c not in lowest_first_place_votes])
 
-@vm(name = "Instant Runoff")
+irv_properties = VotingMethodProperties(
+    condorcet_winner=False, 
+    condorcet_loser=False,
+    pareto_dominance=True, 
+    )
+@vm(name = "Instant Runoff",
+    properties=irv_properties,
+    input_types=[ElectionTypes.PROFILE])
 def instant_runoff(profile, curr_cands = None, algorithm = "basic"):
     """
     If there is a majority winner then that candidate is the winner. If there is no majority winner, then remove all candidates that are ranked first by the fewest number of voters. Continue removing candidates with the fewest number first-place votes until there is a candidate with a majority of first place votes.  
     
     .. important::
         If there is more than one candidate with the fewest number of first-place votes, then *all* such candidates are removed from the profile. 
     
@@ -152,15 +161,22 @@
         rec_ranking = instant_runoff_ranking(profile, [c for c in candidates if c not in lowest_first_place_votes])
         max_rank = max(rec_ranking.ranks)
         rec_ranking_dict = rec_ranking.rmap
         ranking = Ranking({c: rec_ranking_dict[c] if not isin(lowest_first_place_votes,c) else max_rank+1 for c in candidates})
 
         return ranking
 
-@vm(name = "Instant Runoff TB")
+irv_tb_properties = VotingMethodProperties(
+    condorcet_winner=False, 
+    condorcet_loser=None,
+    pareto_dominance=True, 
+    )
+@vm(name = "Instant Runoff TB",
+    properties=irv_tb_properties,
+    input_types=[ElectionTypes.PROFILE])
 def instant_runoff_tb(profile, curr_cands = None, tie_breaker = None):
     """Instant Runoff (``instant_runoff``) with tie breaking:  If there is  more than one candidate with the fewest number of first-place votes, then remove the candidate with lowest in the tie_breaker ranking from the profile.
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
         tie_breaker (List[int]): A list of the candidates in the profile to be used as a tiebreaker.
@@ -220,16 +236,22 @@
             winners = sorted(lowest_first_place_votes)
         else:
             winners = [c for c in candidates 
                        if not isin(cands_to_ignore,c) and _num_rank_first(rs, rcounts, cands_to_ignore, c) >= strict_maj_size]
      
     return sorted(winners)
 
-
-@vm(name = "Instant Runoff PUT")
+irv_put_properties = VotingMethodProperties(
+    condorcet_winner=False, 
+    condorcet_loser=None,
+    pareto_dominance=True, 
+    )
+@vm(name = "Instant Runoff PUT",
+    properties=irv_put_properties,
+    input_types=[ElectionTypes.PROFILE])
 def instant_runoff_put(profile, curr_cands = None):
     """
     Instant Runoff (:func:`instant_runoff`) with parallel universe tie-breaking (PUT), defined recursively: if there is a candidate with a strict majority of first-place votes, that candidate is the IRV-PUT winner; otherwise a candidate x is an IRV-PUT winner if there is some candidate y with a minimal number of first-place votes such that after removing y from the profile, x is an IRV-PUT winner.
     
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
@@ -384,16 +406,22 @@
             winners = sorted(lowest_first_place_votes)
         else:
             winners = [c for c in candidates 
                        if not isin(cands_to_ignore,c) and _num_rank_first(rs, rcounts, cands_to_ignore, c) >= strict_maj_size]
      
     return sorted(winners), elims_list
 
-
-@vm(name="Instant Runoff")
+irv_truncated_lo_properties = VotingMethodProperties(
+    condorcet_winner=False, 
+    condorcet_loser=False,
+    pareto_dominance=None, 
+    )
+@vm(name="Instant Runoff",
+    properties=irv_truncated_lo_properties,
+    input_types=[ElectionTypes.TRUNCATED_LINEAR_PROFILE])
 def instant_runoff_for_truncated_linear_orders(profile, curr_cands = None, threshold = None, hide_warnings = True): 
     """
     Instant Runoff for Truncated Linear Orders.  Iteratively remove the candidates with the fewest number of first place votes, until there is a candidate with more than the threshold number of first-place votes. 
     If a threshold is not set, then it is strictly more than half of the non-empty ballots. 
     
     Args:
         profile (ProfileWithTies): An anonymous profile with no ties in the ballots (note that ProfileWithTies allows for truncated linear orders).
@@ -476,15 +504,22 @@
         
     pl_scores = reduced_prof.plurality_scores()
     
     max_pl_score = max(pl_scores.values())
     
     return sorted([c for c in pl_scores.keys() if pl_scores[c] == max_pl_score])
 
-@vm(name="Bottom-Two-Runoff Instant Runoff")
+bottom_two_runoff_properties = VotingMethodProperties(
+    condorcet_winner=True, 
+    condorcet_loser=False,
+    pareto_dominance=True, 
+    )
+@vm(name="Bottom-Two-Runoff Instant Runoff",
+    properties=bottom_two_runoff_properties,
+    input_types=[ElectionTypes.PROFILE])
 def bottom_two_runoff_instant_runoff(profile, curr_cands = None):
     """Find the two candidates with the lowest two plurality scores, remove the one who loses head-to-head to the other, and repeat until a single candidate remains. 
     
     If there is a tie for lowest or second lowest plurality score, consider all head-to-head matches between a candidate with lowest and a candidate with second lowest plurality score, and remove all the losers of the head-to-head matches, unless this would remove all candidates.
 
     .. note:: 
         BTR-IRV is a Condorcet consistent voting method, i.e., if a Condorcet winner exists, then BTR-IRV will elect the Condorcet winner. 
@@ -526,15 +561,22 @@
                     cands_to_remove.append(c2)
     
     if len(set(cands_to_remove)) == len(candidates):
         return candidates
     else:
         return bottom_two_runoff_instant_runoff(profile, [cand for cand in candidates if cand not in set(cands_to_remove)])
 
-@vm(name="Bottom-Two-Runoff Instant Runoff PUT")
+bottom_two_runoff_put_properties = VotingMethodProperties(
+    condorcet_winner=None, 
+    condorcet_loser=False,
+    pareto_dominance=None, 
+    )
+@vm(name="Bottom-Two-Runoff Instant Runoff PUT",
+    properties=bottom_two_runoff_put_properties,
+    input_types=[ElectionTypes.PROFILE])
 def bottom_two_runoff_instant_runoff_put(profile, curr_cands = None):
     """Find the two candidates with the lowest two plurality scores, remove the one who loses head-to-head to the other, and repeat until a single candidate remains. Parallel-universe tiebreaking is used to break ties for lowest or second lowest plurality scores. 
 
     .. note:: 
         BTR-IRV is a Condorcet consistent voting method, i.e., if a Condorcet winner exists, then BTR-IRV will elect the Condorcet winner. 
 
     Args:
@@ -569,15 +611,23 @@
                 else:
                     additional_winners = bottom_two_runoff_instant_runoff_put(profile, curr_cands = [c for c in candidates if not c == c2])
                 
                 winners = winners + additional_winners
     
     return sorted(set(winners))
     
-@vm(name = "PluralityWRunoff PUT")
+
+pl_w_runoff_properties = VotingMethodProperties(
+    condorcet_winner=False, 
+    condorcet_loser=True,
+    pareto_dominance=None, 
+    )
+@vm(name = "PluralityWRunoff PUT",
+    properties=pl_w_runoff_properties,
+    input_types=[ElectionTypes.PROFILE])
 def plurality_with_runoff_put(profile, curr_cands = None):
     """If there is a majority winner then that candidate is the Plurality with Runoff winner. Otherwise hold a runoff between the top two candidates: the candidate with the most first place votes and the candidate with the 2nd most first place votes (or perhaps tied for the most first place votes). In the case of multiple candidates tied for the most or 2nd most first place votes, use parallel-universe tiebreaking: a candidate is a Plurality with Runoff winner if it is a winner in some runoff as described. If the candidates are all tied for the most first place votes, then all candidates are winners.
         
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
@@ -676,15 +726,22 @@
             winners.append(c2)
         elif profile.margin(c1,c2) == 0:
             winners.append(c1)
             winners.append(c2)
     
     return sorted(list(set(winners))), list(all_runoff_pairs)
 
-@vm(name = "Coombs")
+coombs_properties = VotingMethodProperties(
+    condorcet_winner=False, 
+    condorcet_loser=True,
+    pareto_dominance=True, 
+    )
+@vm(name = "Coombs",
+    properties=coombs_properties,
+    input_types=[ElectionTypes.PROFILE])
 def coombs(profile, curr_cands = None):
     """If there is a majority winner then that candidate is the Coombs winner.   If there is no majority winner, then remove all candidates that are ranked last by the greatest number of voters.  Continue removing candidates with the most last-place votes until there is a candidate with a majority of first place votes.  
     
     .. important::
         If there is  more than one candidate with the largest number of last-place votes, then *all* such candidates are removed from the profile. 
     
     Args:
@@ -741,16 +798,22 @@
             winners = list(greatest_last_place_votes)
         else:
             winners = [c for c in candidates 
                        if not isin(cands_to_ignore,c) and _num_rank_first(rs, rcounts, cands_to_ignore, c) >= strict_maj_size]
 
     return sorted(winners)
 
-
-@vm(name = "Coombs TB")
+coombs_tb_properties = VotingMethodProperties(
+    condorcet_winner=False, 
+    condorcet_loser=None,
+    pareto_dominance=True, 
+    )
+@vm(name = "Coombs TB",
+    properties=coombs_tb_properties,
+    input_types=[ElectionTypes.PROFILE])
 def coombs_tb(profile, curr_cands = None, tie_breaker=None):
     """
     Coombs with a fixed tie-breaking rule: The tie-breaking rule is any linear order (i.e., list) of the candidates.  The default rule is to order the candidates as follows: 0,....,num_cands-1.
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
@@ -812,15 +875,22 @@
             winners = list(greatest_last_place_votes)
         else:
             winners = [c for c in candidates 
                        if not isin(cands_to_ignore,c) and _num_rank_first(rs, rcounts, cands_to_ignore, c) >= strict_maj_size]
 
     return sorted(winners)
 
-@vm(name = "Coombs PUT")
+coombs_put_properties = VotingMethodProperties(
+    condorcet_winner=False, 
+    condorcet_loser=None,
+    pareto_dominance=True, 
+    )
+@vm(name = "Coombs PUT",
+    properties=coombs_put_properties,
+    input_types=[ElectionTypes.PROFILE])
 def coombs_put(profile, curr_cands = None):
     """Coombs with parallel universe tie-breaking (PUT), defined recursively: if there is a candidate with a strict majority of first-place votes, that candidate is the Coombs-PUT winner; otherwise a candidate x is a Coombs-PUT winner if there is some candidate y with a maximal number of last-place votes such that after removing y from the profile, x is a Coombs-PUT winner.
     
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
@@ -944,15 +1014,22 @@
             winners = list(greatest_last_place_votes)
         else:
             winners = [c for c in candidates 
                        if not isin(cands_to_ignore,c) and _num_rank_first(rs, rcounts, cands_to_ignore, c) >= strict_maj_size]
 
     return sorted(winners), elims_list
 
-@vm(name = "Baldwin")
+baldwin_properties = VotingMethodProperties(
+    condorcet_winner=True, 
+    condorcet_loser=True,
+    pareto_dominance=True, 
+    )
+@vm(name = "Baldwin",
+    properties=baldwin_properties,
+    input_types=[ElectionTypes.PROFILE])
 def baldwin(profile, curr_cands = None):
     """Iteratively remove all candidates with the lowest Borda score until a single candidate remains.  If, at any stage, all  candidates have the same Borda score,  then all (remaining) candidates are winners.
 
     .. note:: 
         Baldwin is a Condorcet consistent voting method, i.e., if a Condorcet winner exists, then Baldwin will elect the Condorcet winner. 
 
     Args:
@@ -1011,15 +1088,22 @@
             winners = sorted(last_place_borda_scores)
         elif num_cands - cands_to_ignore.shape[0] ==  1: # only one candidate remains
             winners = sorted([c for c in candidates if c not in cands_to_ignore])
         else: 
             updated_rankings = _find_updated_profile(rankings, cands_to_ignore, num_cands)
     return sorted(winners)
 
-@vm(name = "Baldwin TB")
+baldwin_tb_properties = VotingMethodProperties(
+    condorcet_winner=True, 
+    condorcet_loser=True,
+    pareto_dominance=True, 
+    )
+@vm(name = "Baldwin TB",
+    properties=coombs_tb_properties,
+    input_types=[ElectionTypes.PROFILE])
 def baldwin_tb(profile, curr_cands = None, tie_breaker=None):
     """
     Baldwin with a fixed tie-breaking rule: The tie-breaking rule is any linear order (i.e., list) of the candidates.  The default rule is to order the candidates as follows: 0,....,num_cands-1.
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
@@ -1094,15 +1178,22 @@
             winners = sorted(last_place_borda_scores)
         elif num_cands - cands_to_ignore.shape[0] ==  1: # only one candidate remains
             winners = sorted([c for c in candidates if c not in cands_to_ignore])
         else: 
             updated_rankings = _find_updated_profile(rankings, cands_to_ignore, num_cands)
     return sorted(winners)
 
-@vm(name = "Baldwin PUT")
+baldwin_put_properties = VotingMethodProperties(
+    condorcet_winner=True, 
+    condorcet_loser=True,
+    pareto_dominance=True, 
+    )
+@vm(name = "Baldwin PUT",
+    properties=baldwin_put_properties,
+    input_types=[ElectionTypes.PROFILE])
 def baldwin_put(profile, curr_cands=None):
     """Baldwin with parallel universe tie-breaking (PUT), defined recursively: if there is a single candidate in the profile, that candidate wins; otherwise a candidate x is a Baldwin-PUT winner if there is some candidate y with a minimal Borda score such that after removing y from the profile, x is a Baldwin-PUT winner.
     
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
@@ -1234,15 +1325,22 @@
             winners = sorted(last_place_borda_scores)
         elif num_cands - cands_to_ignore.shape[0] ==  1: # only one candidate remains
             winners = sorted([c for c in candidates if c not in cands_to_ignore])
         else: 
             updated_rankings = _find_updated_profile(rankings, cands_to_ignore, num_cands)
     return sorted(winners), elims_list
 
-@vm(name = "Strict Nanson")
+strict_nanson_properties = VotingMethodProperties(
+    condorcet_winner=True, 
+    condorcet_loser=True,
+    pareto_dominance=True, 
+    )
+@vm(name = "Strict Nanson",
+    properties=strict_nanson_properties,
+    input_types=[ElectionTypes.PROFILE])
 def strict_nanson(profile, curr_cands = None):
     """Iteratively remove all candidates with the  Borda score strictly below the average Borda score until one candidate remains.  If, at any stage, all  candidates have the same Borda score, then all (remaining) candidates are winners.
 
     .. note:: 
         
         Strict Nanson is a Condorcet consistent voting method, i.e., if a Condorcet winner exists, then Strict Nanson will elect the Condorcet winner. 
 
@@ -1377,16 +1475,22 @@
         if (len(below_borda_avg_candidates) == 0) or ((all_num_cands - cands_to_ignore.shape[0]) == 1):
             winners = sorted([c for c in candidates if c not in cands_to_ignore])
         else:
             updated_rankings = _find_updated_profile(rankings, cands_to_ignore, num_cands)
             
     return winners, elim_list
 
-
-@vm(name = "Weak Nanson")
+weak_nanson_properties = VotingMethodProperties(
+    condorcet_winner=True, 
+    condorcet_loser=True,
+    pareto_dominance=True, 
+    )
+@vm(name = "Weak Nanson",
+    properties=weak_nanson_properties,
+    input_types=[ElectionTypes.PROFILE])
 def weak_nanson(profile, curr_cands = None):
     """Iteratively remove all candidates with Borda score less than or equal the average Borda score until one candidate remains.  If, at any stage, all  candidates have the same Borda score, then all (remaining) candidates are winners.
 
     .. note:: 
 
         Weak Nanson is a Condorcet consistent voting method, i.e.,  if a Condorcet winner exists, then Weak Nanson will elect the Condorcet winner. 
 
@@ -1543,15 +1647,22 @@
             winners = [c for c in candidates if not isin(cands_to_ignore, c)]
         else:
             updated_rankings = _find_updated_profile(rankings, cands_to_ignore, num_cands)
             
     return winners, elim_list
 
 
-@vm(name = "Iterated Removal Condorcet Loser")
+it_condorcet_loser_properties = VotingMethodProperties(
+    condorcet_winner=False, 
+    condorcet_loser=True,
+    pareto_dominance=False, 
+    )
+@vm(name = "Iterated Removal Condorcet Loser",
+    properties=it_condorcet_loser_properties,
+    input_types=[ElectionTypes.PROFILE, ElectionTypes.PROFILE_WITH_TIES, ElectionTypes.MAJORITY_GRAPH, ElectionTypes.MARGIN_GRAPH])
 def iterated_removal_cl(edata, curr_cands = None):
     """
     Iteratively remove candidates that are Condorcet losers until there are no Condorcet losers.   A candidate :math:`c` is a **Condorcet loser** when every other candidate is majority preferred to :math:`c`. 
 
     Args:
         edata (Profile, ProfileWithTies, MajorityGraph, MarginGraph): Any election data that has a `condorcet_loser` method. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
@@ -1639,15 +1750,22 @@
     worst_m_score = min([m_scores[c] for c in curr_cands])
     worst_losers = [c for c in curr_cands if m_scores[c] == worst_m_score]
     if len(worst_losers) == len(curr_cands):
         return curr_cands
     else:
         return [c for c in curr_cands if c not in worst_losers]
 
-@vm(name = "Raynaud")
+raynaud_properties = VotingMethodProperties(
+    condorcet_winner=True, 
+    condorcet_loser=False,
+    pareto_dominance=True, 
+    )
+@vm(name = "Raynaud",
+    properties=raynaud_properties,
+    input_types=[ElectionTypes.PROFILE, ElectionTypes.PROFILE_WITH_TIES, ElectionTypes.MARGIN_GRAPH])
 def raynaud(edata, curr_cands=None, score_method = "margins"):
     """Iteratively remove the candidate(s) whose worst loss is biggest, unless all candidates have the same worst loss. See https://electowiki.org/wiki/Raynaud.
     
     Args:
         edata (Profile, ProfileWithTies, MarginGraph): Any election data that has a `margin` method. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``.
         score_method (str, optional): Options include "margins" (the default), "winning" assigns to each candidate :math:`c` the maximum support of a candidate majority preferred to :math:`c`,  and "pairwise_opposition" assigns to each candidate :math:`c` the maximum support of any candidate over :math:`c`.   These scores only lead to different results on non-linear profiles. 
@@ -1658,15 +1776,22 @@
     candidates = edata.candidates if curr_cands is None else curr_cands
     new_cands = _remove_worst_losers(edata,candidates,score_method)
     while not new_cands == candidates:
         candidates = new_cands
         new_cands = _remove_worst_losers(edata,candidates,score_method)
     return sorted(candidates)
 
-@vm(name = "Benham")
+benham_properties = VotingMethodProperties(
+    condorcet_winner=True, 
+    condorcet_loser=False,
+    pareto_dominance=True, 
+    )
+@vm(name = "Benham",
+    properties=benham_properties,
+    input_types=[ElectionTypes.PROFILE])
 def benham(profile, curr_cands = None):
     """
     As long as the profile has no Condorcet winner, eliminate the candidate with the lowest plurality score.
     
     .. important::
         If there is  more than one candidate with the fewest number of first-place votes, then *all* such candidates are removed from the profile. 
     
@@ -1710,16 +1835,22 @@
         else:
             cw = profile.condorcet_winner([c for c in profile.candidates if not isin(cands_to_ignore, c)])
             if cw is not None: 
                 winners = [cw]
 
     return sorted(winners)
 
-
-@vm(name = "Benham TB")
+benham_tb_properties = VotingMethodProperties(
+    condorcet_winner=True, 
+    condorcet_loser=None,
+    pareto_dominance=True, 
+    )
+@vm(name = "Benham TB",
+    properties=benham_tb_properties,
+    input_types=[ElectionTypes.PROFILE])
 def benham_tb(profile, curr_cands = None, tie_breaker = None):
     """Benham (``benham``) with tie breaking:  If there is  more than one candidate with the fewest number of first-place votes, then remove the candidate with lowest in the tie_breaker ranking from the profile.
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
         tie_breaker (List[int]): A list of the candidates in the profile to be used as a tiebreaker.
@@ -1762,15 +1893,22 @@
         else:
             cw = profile.condorcet_winner(curr_cands = [c for c in profile.candidates if not isin(cands_to_ignore, c)])
             if cw is not None: 
                 winners = [cw]
     return sorted(winners)
 
 
-@vm(name = "Benham PUT")
+benham_tb_properties = VotingMethodProperties(
+    condorcet_winner=True, 
+    condorcet_loser=None,
+    pareto_dominance=True, 
+    )
+@vm(name = "Benham PUT",
+    properties=benham_tb_properties,
+    input_types=[ElectionTypes.PROFILE])
 def benham_put(profile, curr_cands = None):
     """Benham (:func:`benham`) with parallel universe tie-breaking (PUT), defined recursively: if there is a Condorcet winner, that candidate is the Benham-PUT winner; otherwise a candidate x is a Benham-PUT winner if there is some candidate y with minimal plurality score such that after removing y from the profile, x is a Benham-PUT winner.
     
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
@@ -1850,16 +1988,31 @@
             return vm_ws
             
         else:
             return _ta(profile, curr_cands = [c for c in candidates if not c in cands_to_remove])
 
     return VotingMethod(_ta, name=f"Tideman Alternative {vm.name}")
 
+ta_smith_properties = VotingMethodProperties(
+    condorcet_winner=True,
+    condorcet_loser=True,
+    pareto_dominance=True,
+)
 tideman_alternative_smith = tideman_alternative(top_cycle)
+tideman_alternative_smith.properties = ta_smith_properties
+tideman_alternative_smith.input_types = [ElectionTypes.PROFILE]
+
+ta_schwartz_properties = VotingMethodProperties(
+    condorcet_winner=True,
+    condorcet_loser=True,
+    pareto_dominance=True,
+)
 tideman_alternative_schwartz = tideman_alternative(gocha)
+tideman_alternative_schwartz.properties = ta_schwartz_properties
+tideman_alternative_schwartz.input_types = [ElectionTypes.PROFILE]
 
 def tideman_alternative_put(vm):
     """Given a voting method vm, returns a voting method that restricts the profile to the set of vm winners, then eliminates the candidate with the fewest first-place votes, and then repeats until there is only one vm winner. Parallel-universe tiebreaking is used when there are multiple candidates with the fewest first-place votes.
 
     Args:
         vm (VotingMethod): A voting method.
 
@@ -1887,18 +2040,42 @@
                 additional_winners = _ta(profile, curr_cands = [c for c in candidates if not c == cand_to_remove])
                 winners = winners + additional_winners
 
         return sorted(set(winners))
 
     return VotingMethod(_ta, name=f"Tideman Alternative {vm.name} PUT")
 
+
+ta_smith_put_properties = VotingMethodProperties(
+    condorcet_winner=True,
+    condorcet_loser=True,
+    pareto_dominance=True,
+)
 tideman_alternative_smith_put = tideman_alternative_put(top_cycle)
+tideman_alternative_smith_put.properties = ta_smith_put_properties
+tideman_alternative_smith_put.input_types = [ElectionTypes.PROFILE]
+
+ta_schwartz_put_properties = VotingMethodProperties(
+    condorcet_winner=True,
+    condorcet_loser=True,
+    pareto_dominance=True,
+)
 tideman_alternative_schwartz_put = tideman_alternative_put(gocha)
+tideman_alternative_schwartz_put.properties = ta_schwartz_put_properties
+tideman_alternative_schwartz_put.input_types = [ElectionTypes.PROFILE]
+
 
-@vm(name = "Woodall")
+woodall_properties = VotingMethodProperties(
+    condorcet_winner=True,
+    condorcet_loser=True,
+    pareto_dominance=True,
+)
+@vm(name = "Woodall",
+    properties=woodall_properties,
+    input_types=[ElectionTypes.PROFILE])
 def woodall(profile, curr_cands = None):
     """
     If there is a single member of the Smith Set (i.e., a Condorcet winner) then that candidate is the winner.  If there the Smith Set contains more than one candidate, then remove all candidates that are ranked first by the fewest number of voters.  Continue removing candidates with the fewest number first-place votes until there is a single member of the originally Smith Set remaining.  
     
     .. important::
         If there is  more than one candidate with the fewest number of first-place votes, then *all* such candidates are removed from the profile. 
     
@@ -1951,15 +2128,22 @@
         if len(new_remaining_cands_in_smith_set) == 1:
             winners = new_remaining_cands_in_smith_set 
      
         cands_to_ignore = new_cands_to_ignore
 
     return sorted(winners)
 
-@vm(name = "Knockout Voting")
+knockout_properties = VotingMethodProperties(
+    condorcet_winner=None,
+    condorcet_loser=None,
+    pareto_dominance=None,
+)
+@vm(name = "Knockout Voting",
+    properties=knockout_properties,
+    input_types=[ElectionTypes.PROFILE])
 def knockout(profile, curr_cands=None):
     """Find the two candidates in curr_cands with the lowest and second lowest Borda scores among any candidates in curr_cands. Then remove from curr_cands whichever one loses to the other in a head-to-head majority comparison. Repeat this process, always using the original Borda score (i.e., the Borda scores calculated with respect to all candidates in the profile, not with respect to curr_cands as for Baldwin and Nanson) until only one candidate remains in curr_cands. Parallel universe tie-breaking (PUT) is used when there are ties in lowest or second lowest Borda scores.
 
     .. note::
         Proposed by Edward B. Foley (with unspecified handling of ties in Borda scores, so PUT is used here as an example).
     
     Args:
@@ -2015,43 +2199,14 @@
             if profile.margin(cand_with_lowest_borda_score, c2) > 0:
                 new_winners = knockout(profile, curr_cands = [c for c in candidates if not c == c2])
                 winners = winners + new_winners
 
     return sorted(set(winners))
 
     
-iterated_vms = [
-    instant_runoff,
-    instant_runoff_tb,
-    instant_runoff_put,
-    #hare,
-    #ranked_choice,
-    bottom_two_runoff_instant_runoff,
-    bottom_two_runoff_instant_runoff_put,
-    benham,
-    benham_put,
-    benham_tb,
-    plurality_with_runoff_put,
-    coombs,
-    coombs_tb,
-    coombs_put,
-    baldwin,
-    baldwin_tb,
-    baldwin_put,
-    strict_nanson,
-    weak_nanson,
-    iterated_removal_cl,
-    raynaud,
-    tideman_alternative_smith,
-    tideman_alternative_smith_put,
-    tideman_alternative_schwartz,
-    tideman_alternative_schwartz_put,
-    woodall,
-    knockout
-]
 
 iterated_vms_with_explanation = [
     instant_runoff_with_explanation,
     coombs_with_explanation,
     plurality_with_runoff_put_with_explanation,
     baldwin_with_explanation,
     strict_nanson_with_explanation,
```

### Comparing `pref_voting-1.2.0/pref_voting/maj_graph_ex1.png` & `pref_voting-1.3.0/pref_voting/maj_graph_ex1.png`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/mappings.py` & `pref_voting-1.3.0/pref_voting/mappings.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/margin_based_methods.py` & `pref_voting-1.3.0/pref_voting/margin_based_methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,4476 +32,4670 @@
 000001f0: 6572 2069 6d70 6f72 7420 6765 745f 6d67  er import get_mg
 00000200: 2c20 5350 4f0a 696d 706f 7274 206d 6174  , SPO.import mat
 00000210: 680a 6672 6f6d 2069 7465 7274 6f6f 6c73  h.from itertools
 00000220: 2069 6d70 6f72 7420 7072 6f64 7563 742c   import product,
 00000230: 2070 6572 6d75 7461 7469 6f6e 732c 2063   permutations, c
 00000240: 6f6d 6269 6e61 7469 6f6e 732c 2063 6861  ombinations, cha
 00000250: 696e 0a69 6d70 6f72 7420 6e65 7477 6f72  in.import networ
-00000260: 6b78 2061 7320 6e78 0a0a 4076 6d28 6e61  kx as nx..@vm(na
-00000270: 6d65 203d 2022 4d69 6e69 6d61 7822 290a  me = "Minimax").
-00000280: 6465 6620 6d69 6e69 6d61 7828 6564 6174  def minimax(edat
-00000290: 612c 2063 7572 725f 6361 6e64 7320 3d20  a, curr_cands = 
-000002a0: 4e6f 6e65 2c20 7374 7265 6e67 7468 5f66  None, strength_f
-000002b0: 756e 6374 696f 6e20 3d20 4e6f 6e65 293a  unction = None):
-000002c0: 2020 200a 2020 2020 2222 220a 2020 2020     .    """.    
-000002d0: 5468 6520 4d69 6e69 6d61 7820 7769 6e6e  The Minimax winn
-000002e0: 6572 7320 6172 6520 7468 6520 6361 6e64  ers are the cand
-000002f0: 6964 6174 6573 2077 6974 6820 7468 6520  idates with the 
-00000300: 736d 616c 6c65 7374 206d 6178 696d 756d  smallest maximum
-00000310: 2070 6169 7277 6973 6520 6c6f 7373 2e20   pairwise loss. 
-00000320: 2054 6861 7420 6973 2c20 666f 7220 6561   That is, for ea
-00000330: 6368 2063 616e 6469 6461 7465 203a 6d61  ch candidate :ma
-00000340: 7468 3a60 6160 2c20 6669 6e64 2074 6865  th:`a`, find the
-00000350: 2062 6967 6765 7374 206d 6172 6769 6e20   biggest margin 
-00000360: 6f66 2061 2063 616e 6469 6461 7465 203a  of a candidate :
-00000370: 6d61 7468 3a60 6260 206f 7665 7220 3a6d  math:`b` over :m
-00000380: 6174 683a 6061 602c 2074 6865 6e20 656c  ath:`a`, then el
-00000390: 6563 7420 7468 6520 6361 6e64 6964 6174  ect the candidat
-000003a0: 6528 7329 2077 6974 6820 7468 6520 736d  e(s) with the sm
-000003b0: 616c 6c65 7374 2073 7563 6820 6c6f 7373  allest such loss
-000003c0: 2e20 416c 736f 206b 6e6f 776e 2061 7320  . Also known as 
-000003d0: 7468 6520 5369 6d70 736f 6e2d 4b72 616d  the Simpson-Kram
-000003e0: 6572 2052 756c 652e 0a20 2020 200a 2020  er Rule..    .  
-000003f0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00000400: 6564 6174 6120 2850 726f 6669 6c65 2c20  edata (Profile, 
-00000410: 5072 6f66 696c 6557 6974 6854 6965 732c  ProfileWithTies,
-00000420: 204d 6172 6769 6e47 7261 7068 293a 2041   MarginGraph): A
-00000430: 6e79 2065 6c65 6374 696f 6e20 6461 7461  ny election data
-00000440: 2074 6861 7420 6861 7320 6120 606d 6172   that has a `mar
-00000450: 6769 6e60 206d 6574 686f 642e 200a 2020  gin` method. .  
-00000460: 2020 2020 2020 6375 7272 5f63 616e 6473        curr_cands
-00000470: 2028 4c69 7374 5b69 6e74 5d2c 206f 7074   (List[int], opt
-00000480: 696f 6e61 6c29 3a20 4966 2073 6574 2c20  ional): If set, 
-00000490: 7468 656e 2066 696e 6420 7468 6520 7769  then find the wi
-000004a0: 6e6e 6572 7320 666f 7220 7468 6520 7072  nners for the pr
-000004b0: 6f66 696c 6520 7265 7374 7269 6374 6564  ofile restricted
-000004c0: 2074 6f20 7468 6520 6361 6e64 6964 6174   to the candidat
-000004d0: 6573 2069 6e20 6060 6375 7272 5f63 616e  es in ``curr_can
-000004e0: 6473 6060 0a0a 2020 2020 5265 7475 726e  ds``..    Return
-000004f0: 733a 200a 2020 2020 2020 2020 4120 736f  s: .        A so
-00000500: 7274 6564 206c 6973 7420 6f66 2063 616e  rted list of can
-00000510: 6469 6461 7465 730a 0a20 2020 202e 2e20  didates..    .. 
-00000520: 7365 6561 6c73 6f3a 3a0a 0a20 2020 2020  seealso::..     
-00000530: 2020 203a 6d65 7468 3a60 7072 6566 5f76     :meth:`pref_v
-00000540: 6f74 696e 672e 6d61 7267 696e 5f62 6173  oting.margin_bas
-00000550: 6564 5f6d 6574 686f 6473 2e6d 696e 696d  ed_methods.minim
-00000560: 6178 5f73 636f 7265 7360 0a0a 2020 2020  ax_scores`..    
-00000570: 3a45 7861 6d70 6c65 3a20 0a0a 2020 2020  :Example: ..    
-00000580: 2e2e 2070 6c6f 743a 3a20 206d 6172 6769  .. plot::  margi
-00000590: 6e5f 6772 6170 6873 5f65 7861 6d70 6c65  n_graphs_example
-000005a0: 732f 6d67 5f65 785f 6d69 6e69 6d61 782e  s/mg_ex_minimax.
-000005b0: 7079 0a20 2020 2020 2020 203a 636f 6e74  py.        :cont
-000005c0: 6578 743a 2072 6573 6574 2020 0a20 2020  ext: reset  .   
-000005d0: 2020 2020 203a 696e 636c 7564 652d 736f       :include-so
-000005e0: 7572 6365 3a20 5472 7565 0a0a 0a20 2020  urce: True...   
-000005f0: 202e 2e20 636f 6465 2d62 6c6f 636b 3a3a   .. code-block::
-00000600: 200a 0a20 2020 2020 2020 2066 726f 6d20   ..        from 
-00000610: 7072 6566 5f76 6f74 696e 672e 6d61 7267  pref_voting.marg
-00000620: 696e 5f62 6173 6564 5f6d 6574 686f 6473  in_based_methods
-00000630: 2069 6d70 6f72 7420 6d69 6e69 6d61 780a   import minimax.
-00000640: 0a20 2020 2020 2020 206d 696e 696d 6178  .        minimax
-00000650: 2e64 6973 706c 6179 2870 726f 6629 0a0a  .display(prof)..
-00000660: 0a20 2020 202e 2e20 6578 6563 5f63 6f64  .    .. exec_cod
-00000670: 653a 3a20 0a20 2020 2020 2020 203a 6869  e:: .        :hi
-00000680: 6465 5f63 6f64 653a 0a0a 2020 2020 2020  de_code:..      
-00000690: 2020 6672 6f6d 2070 7265 665f 766f 7469    from pref_voti
-000006a0: 6e67 2e70 726f 6669 6c65 7320 696d 706f  ng.profiles impo
-000006b0: 7274 2050 726f 6669 6c65 0a20 2020 2020  rt Profile.     
-000006c0: 2020 2066 726f 6d20 7072 6566 5f76 6f74     from pref_vot
-000006d0: 696e 672e 6d61 7267 696e 5f62 6173 6564  ing.margin_based
-000006e0: 5f6d 6574 686f 6473 2069 6d70 6f72 7420  _methods import 
-000006f0: 6d69 6e69 6d61 780a 2020 2020 2020 2020  minimax.        
-00000700: 0a20 2020 2020 2020 2070 726f 6620 3d20  .        prof = 
-00000710: 5072 6f66 696c 6528 5b5b 332c 2030 2c20  Profile([[3, 0, 
-00000720: 312c 2032 5d2c 205b 312c 2033 2c20 322c  1, 2], [1, 3, 2,
-00000730: 2030 5d2c 205b 312c 2033 2c20 302c 2032   0], [1, 3, 0, 2
-00000740: 5d2c 205b 312c 2032 2c20 302c 2033 5d2c  ], [1, 2, 0, 3],
-00000750: 205b 332c 2032 2c20 302c 2031 5d2c 205b   [3, 2, 0, 1], [
-00000760: 302c 2032 2c20 312c 2033 5d5d 2c20 5b31  0, 2, 1, 3]], [1
-00000770: 2c20 312c 2031 2c20 312c 2032 2c20 315d  , 1, 1, 1, 2, 1]
-00000780: 290a 0a20 2020 2020 2020 206d 696e 696d  )..        minim
-00000790: 6178 2e64 6973 706c 6179 2870 726f 6629  ax.display(prof)
-000007a0: 0a0a 2020 2020 2222 220a 0a20 2020 2063  ..    """..    c
-000007b0: 616e 6469 6461 7465 7320 3d20 6564 6174  andidates = edat
-000007c0: 612e 6361 6e64 6964 6174 6573 2069 6620  a.candidates if 
-000007d0: 6375 7272 5f63 616e 6473 2069 7320 4e6f  curr_cands is No
-000007e0: 6e65 2065 6c73 6520 6375 7272 5f63 616e  ne else curr_can
-000007f0: 6473 2020 2020 0a20 2020 2073 7472 656e  ds    .    stren
-00000800: 6774 685f 6675 6e63 7469 6f6e 203d 2065  gth_function = e
-00000810: 6461 7461 2e6d 6172 6769 6e20 6966 2073  data.margin if s
-00000820: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-00000830: 2069 7320 4e6f 6e65 2065 6c73 6520 7374   is None else st
-00000840: 7265 6e67 7468 5f66 756e 6374 696f 6e0a  rength_function.
-00000850: 0a20 2020 2073 636f 7265 7320 3d20 7b63  .    scores = {c
-00000860: 3a20 6d61 7828 5b73 7472 656e 6774 685f  : max([strength_
-00000870: 6675 6e63 7469 6f6e 285f 632c 2063 2920  function(_c, c) 
-00000880: 666f 7220 5f63 2069 6e20 6564 6174 612e  for _c in edata.
-00000890: 646f 6d69 6e61 746f 7273 2863 2920 6966  dominators(c) if
-000008a0: 205f 6320 696e 2063 616e 6469 6461 7465   _c in candidate
-000008b0: 735d 2920 6966 2061 6e79 285b 5f63 2069  s]) if any([_c i
-000008c0: 6e20 6564 6174 612e 646f 6d69 6e61 746f  n edata.dominato
-000008d0: 7273 2863 2920 666f 7220 5f63 2069 6e20  rs(c) for _c in 
-000008e0: 6361 6e64 6964 6174 6573 5d29 2065 6c73  candidates]) els
-000008f0: 6520 3020 0a20 2020 2020 2020 2020 2020  e 0 .           
-00000900: 2020 2066 6f72 2063 2069 6e20 6361 6e64     for c in cand
-00000910: 6964 6174 6573 7d0a 2020 2020 6d69 6e5f  idates}.    min_
-00000920: 7363 6f72 6520 3d20 6d69 6e28 7363 6f72  score = min(scor
-00000930: 6573 2e76 616c 7565 7328 2929 0a20 2020  es.values()).   
-00000940: 2072 6574 7572 6e20 736f 7274 6564 285b   return sorted([
-00000950: 6320 666f 7220 6320 696e 2063 616e 6469  c for c in candi
-00000960: 6461 7465 7320 6966 2073 636f 7265 735b  dates if scores[
-00000970: 635d 203d 3d20 6d69 6e5f 7363 6f72 655d  c] == min_score]
-00000980: 290a 0a0a 6465 6620 6d69 6e69 6d61 785f  )...def minimax_
-00000990: 7363 6f72 6573 2865 6461 7461 2c20 6375  scores(edata, cu
-000009a0: 7272 5f63 616e 6473 203d 204e 6f6e 652c  rr_cands = None,
-000009b0: 2073 636f 7265 5f6d 6574 686f 643d 226d   score_method="m
-000009c0: 6172 6769 6e73 2229 3a0a 2020 2020 2222  argins"):.    ""
-000009d0: 2252 6574 7572 6e20 7468 6520 6d69 6e69  "Return the mini
-000009e0: 6d61 7820 7363 6f72 6573 2066 6f72 2065  max scores for e
-000009f0: 6163 6820 6361 6e64 6964 6174 652c 2077  ach candidate, w
-00000a00: 6865 7265 2074 6865 206d 696e 696d 6178  here the minimax
-00000a10: 2073 636f 7265 2066 6f72 203a 6d61 7468   score for :math
-00000a20: 3a60 6360 2069 7320 2d31 202a 2074 6865  :`c` is -1 * the
-00000a30: 206d 6178 696d 756d 2070 6169 7277 6973   maximum pairwis
-00000a40: 6520 6d61 6a6f 7269 7479 206c 6f73 732e  e majority loss.
-00000a50: 200a 0a20 2020 2041 7267 733a 0a20 2020   ..    Args:.   
-00000a60: 2020 2020 2065 6461 7461 2028 5072 6f66       edata (Prof
-00000a70: 696c 652c 2050 726f 6669 6c65 5769 7468  ile, ProfileWith
-00000a80: 5469 6573 2c20 4d61 7267 696e 4772 6170  Ties, MarginGrap
-00000a90: 6829 3a20 416e 7920 656c 6563 7469 6f6e  h): Any election
-00000aa0: 2064 6174 6120 7468 6174 2068 6173 2061   data that has a
-00000ab0: 2060 6d61 7267 696e 6020 6d65 7468 6f64   `margin` method
-00000ac0: 2e20 0a20 2020 2020 2020 2063 7572 725f  . .        curr_
-00000ad0: 6361 6e64 7320 284c 6973 745b 696e 745d  cands (List[int]
-00000ae0: 2c20 6f70 7469 6f6e 616c 293a 2049 6620  , optional): If 
-00000af0: 7365 742c 2074 6865 6e20 6669 6e64 2074  set, then find t
-00000b00: 6865 2077 696e 6e65 7273 2066 6f72 2074  he winners for t
-00000b10: 6865 2070 726f 6669 6c65 2072 6573 7472  he profile restr
-00000b20: 6963 7465 6420 746f 2074 6865 2063 616e  icted to the can
-00000b30: 6469 6461 7465 7320 696e 2060 6063 7572  didates in ``cur
-00000b40: 725f 6361 6e64 7360 600a 2020 2020 2020  r_cands``.      
-00000b50: 2020 7363 6f72 655f 6d65 7468 6f64 2028    score_method (
-00000b60: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
-00000b70: 4f70 7469 6f6e 7320 696e 636c 7564 6520  Options include 
-00000b80: 226d 6172 6769 6e73 2220 2874 6865 2064  "margins" (the d
-00000b90: 6566 6175 6c74 292c 2022 7769 6e6e 696e  efault), "winnin
-00000ba0: 6722 2061 7373 6967 6e73 2074 6f20 6561  g" assigns to ea
-00000bb0: 6368 2063 616e 6469 6461 7465 203a 6d61  ch candidate :ma
-00000bc0: 7468 3a60 6360 2074 6865 206d 6178 696d  th:`c` the maxim
-00000bd0: 756d 2073 7570 706f 7274 206f 6620 6120  um support of a 
-00000be0: 6361 6e64 6964 6174 6520 6d61 6a6f 7269  candidate majori
-00000bf0: 7479 2070 7265 6665 7272 6564 2074 6f20  ty preferred to 
-00000c00: 3a6d 6174 683a 6063 602c 2020 616e 6420  :math:`c`,  and 
-00000c10: 2270 6169 7277 6973 655f 6f70 706f 7369  "pairwise_opposi
-00000c20: 7469 6f6e 2220 6173 7369 676e 7320 746f  tion" assigns to
-00000c30: 2065 6163 6820 6361 6e64 6964 6174 6520   each candidate 
-00000c40: 3a6d 6174 683a 6063 6020 7468 6520 6d61  :math:`c` the ma
-00000c50: 7869 6d75 6d20 7375 7070 6f72 7420 6f66  ximum support of
-00000c60: 2061 6e79 2063 616e 6469 6461 7465 206f   any candidate o
-00000c70: 7665 7220 3a6d 6174 683a 6063 602e 2020  ver :math:`c`.  
-00000c80: 2054 6865 7365 2073 636f 7265 7320 6f6e   These scores on
-00000c90: 6c79 206c 6561 6420 746f 2064 6966 6665  ly lead to diffe
-00000ca0: 7265 6e74 2072 6573 756c 7473 206f 6e20  rent results on 
-00000cb0: 6e6f 6e2d 6c69 6e65 6172 2070 726f 6669  non-linear profi
-00000cc0: 6c65 732e 200a 0a20 2020 2052 6574 7572  les. ..    Retur
-00000cd0: 6e73 3a20 0a20 2020 2020 2020 2041 2064  ns: .        A d
-00000ce0: 6963 7469 6f6e 6172 7920 6173 736f 6369  ictionary associ
-00000cf0: 6174 696e 6720 6561 6368 2063 616e 6469  ating each candi
-00000d00: 6461 7465 2077 6974 6820 6974 7320 6d69  date with its mi
-00000d10: 6e69 6d61 7820 7363 6f72 652e 0a0a 2020  nimax score...  
-00000d20: 2020 2e2e 2073 6565 616c 736f 3a3a 0a0a    .. seealso::..
-00000d30: 2020 2020 2020 2020 3a6d 6574 683a 6070          :meth:`p
-00000d40: 7265 665f 766f 7469 6e67 2e6d 6172 6769  ref_voting.margi
-00000d50: 6e5f 6261 7365 645f 6d65 7468 6f64 732e  n_based_methods.
-00000d60: 6d69 6e69 6d61 7860 0a0a 2020 2020 3a45  minimax`..    :E
-00000d70: 7861 6d70 6c65 3a20 0a0a 2020 2020 2e2e  xample: ..    ..
-00000d80: 2070 6c6f 743a 3a20 206d 6172 6769 6e5f   plot::  margin_
-00000d90: 6772 6170 6873 5f65 7861 6d70 6c65 732f  graphs_examples/
-00000da0: 6d67 5f65 785f 6d69 6e69 6d61 782e 7079  mg_ex_minimax.py
-00000db0: 0a20 2020 2020 2020 203a 636f 6e74 6578  .        :contex
-00000dc0: 743a 2072 6573 6574 2020 0a20 2020 2020  t: reset  .     
-00000dd0: 2020 203a 696e 636c 7564 652d 736f 7572     :include-sour
-00000de0: 6365 3a20 5472 7565 0a0a 0a20 2020 202e  ce: True...    .
-00000df0: 2e20 636f 6465 2d62 6c6f 636b 3a3a 200a  . code-block:: .
-00000e00: 0a20 2020 2020 2020 2066 726f 6d20 7072  .        from pr
-00000e10: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
-00000e20: 5f62 6173 6564 5f6d 6574 686f 6473 2069  _based_methods i
-00000e30: 6d70 6f72 7420 6d69 6e69 6d61 785f 7363  mport minimax_sc
-00000e40: 6f72 6573 2c20 6d69 6e69 6d61 780a 0a20  ores, minimax.. 
-00000e50: 2020 2020 2020 206d 696e 696d 6178 2e64         minimax.d
-00000e60: 6973 706c 6179 2870 726f 6629 0a20 2020  isplay(prof).   
-00000e70: 2020 2020 2070 7269 6e74 286d 696e 696d       print(minim
-00000e80: 6178 5f73 636f 7265 7328 7072 6f66 2929  ax_scores(prof))
-00000e90: 0a0a 0a20 2020 202e 2e20 6578 6563 5f63  ...    .. exec_c
-00000ea0: 6f64 653a 3a20 0a20 2020 2020 2020 203a  ode:: .        :
-00000eb0: 6869 6465 5f63 6f64 653a 0a0a 2020 2020  hide_code:..    
-00000ec0: 2020 2020 6672 6f6d 2070 7265 665f 766f      from pref_vo
-00000ed0: 7469 6e67 2e70 726f 6669 6c65 7320 696d  ting.profiles im
-00000ee0: 706f 7274 2050 726f 6669 6c65 0a20 2020  port Profile.   
-00000ef0: 2020 2020 2066 726f 6d20 7072 6566 5f76       from pref_v
-00000f00: 6f74 696e 672e 6d61 7267 696e 5f62 6173  oting.margin_bas
-00000f10: 6564 5f6d 6574 686f 6473 2069 6d70 6f72  ed_methods impor
-00000f20: 7420 6d69 6e69 6d61 782c 206d 696e 696d  t minimax, minim
-00000f30: 6178 5f73 636f 7265 730a 2020 2020 2020  ax_scores.      
-00000f40: 2020 0a20 2020 2020 2020 2070 726f 6620    .        prof 
-00000f50: 3d20 5072 6f66 696c 6528 5b5b 332c 2030  = Profile([[3, 0
-00000f60: 2c20 312c 2032 5d2c 205b 312c 2033 2c20  , 1, 2], [1, 3, 
-00000f70: 322c 2030 5d2c 205b 312c 2033 2c20 302c  2, 0], [1, 3, 0,
-00000f80: 2032 5d2c 205b 312c 2032 2c20 302c 2033   2], [1, 2, 0, 3
-00000f90: 5d2c 205b 332c 2032 2c20 302c 2031 5d2c  ], [3, 2, 0, 1],
-00000fa0: 205b 302c 2032 2c20 312c 2033 5d5d 2c20   [0, 2, 1, 3]], 
-00000fb0: 5b31 2c20 312c 2031 2c20 312c 2032 2c20  [1, 1, 1, 1, 2, 
-00000fc0: 315d 290a 0a20 2020 2020 2020 206d 696e  1])..        min
-00000fd0: 696d 6178 2e64 6973 706c 6179 2870 726f  imax.display(pro
-00000fe0: 6629 0a20 2020 2020 2020 2070 7269 6e74  f).        print
-00000ff0: 286d 696e 696d 6178 5f73 636f 7265 7328  (minimax_scores(
-00001000: 7072 6f66 2929 0a0a 2020 2020 2222 220a  prof))..    """.
-00001010: 2020 2020 0a20 2020 2063 616e 6469 6461      .    candida
-00001020: 7465 7320 3d20 6564 6174 612e 6361 6e64  tes = edata.cand
-00001030: 6964 6174 6573 2069 6620 6375 7272 5f63  idates if curr_c
-00001040: 616e 6473 2069 7320 4e6f 6e65 2065 6c73  ands is None els
-00001050: 6520 6375 7272 5f63 616e 6473 0a0a 2020  e curr_cands..  
-00001060: 2020 6966 206c 656e 2863 616e 6469 6461    if len(candida
-00001070: 7465 7329 203d 3d20 313a 0a20 2020 2020  tes) == 1:.     
-00001080: 2020 2072 6574 7572 6e20 7b63 3a20 3020     return {c: 0 
-00001090: 666f 7220 6320 696e 2063 616e 6469 6461  for c in candida
-000010a0: 7465 737d 0a20 2020 200a 2020 2020 2320  tes}.    .    # 
-000010b0: 7468 6572 6520 6172 6520 6469 6666 6572  there are differ
-000010c0: 656e 7420 7363 6f72 696e 6720 6675 6e63  ent scoring func
-000010d0: 7469 6f6e 7320 7468 6174 2063 616e 2062  tions that can b
-000010e0: 6520 7573 6564 2074 6f20 6d65 6173 7572  e used to measur
-000010f0: 6520 7468 6520 776f 7273 6520 6c6f 7373  e the worse loss
-00001100: 2066 6f72 2065 6163 6820 0a20 2020 2023   for each .    #
-00001110: 2063 616e 6469 6461 7465 2e20 5468 6573   candidate. Thes
-00001120: 6520 616c 6c20 7072 6f64 7563 6520 7468  e all produce th
-00001130: 6520 7361 6d65 2073 6574 206f 6620 7769  e same set of wi
-00001140: 6e6e 6572 7320 7768 656e 2076 6f74 6572  nners when voter
-00001150: 7320 7375 626d 6974 206c 696e 6561 7220  s submit linear 
-00001160: 6f72 6465 7273 2e20 0a20 2020 2073 636f  orders. .    sco
-00001170: 7265 5f66 756e 6374 696f 6e73 203d 207b  re_functions = {
-00001180: 0a20 2020 2020 2020 2022 7769 6e6e 696e  .        "winnin
-00001190: 6722 3a20 6c61 6d62 6461 2063 732c 2063  g": lambda cs, c
-000011a0: 3a20 6d61 7828 5b65 6461 7461 2e73 7570  : max([edata.sup
-000011b0: 706f 7274 285f 632c 6329 2066 6f72 205f  port(_c,c) for _
-000011c0: 6320 696e 2063 735d 2920 6966 206c 656e  c in cs]) if len
-000011d0: 2863 7329 203e 2030 2065 6c73 6520 302c  (cs) > 0 else 0,
-000011e0: 0a20 2020 2020 2020 2022 6d61 7267 696e  .        "margin
-000011f0: 7322 3a20 6c61 6d62 6461 2063 732c 2063  s": lambda cs, c
-00001200: 3a20 6d61 7828 5b65 6461 7461 2e6d 6172  : max([edata.mar
-00001210: 6769 6e28 5f63 2c63 2920 666f 7220 5f63  gin(_c,c) for _c
-00001220: 2069 6e20 6373 5d29 2069 6620 6c65 6e28   in cs]) if len(
-00001230: 6373 2920 3e20 3020 656c 7365 2030 2c0a  cs) > 0 else 0,.
-00001240: 2020 2020 2020 2020 2270 6169 7277 6973          "pairwis
-00001250: 655f 6f70 706f 7369 7469 6f6e 223a 206c  e_opposition": l
-00001260: 616d 6264 6120 6373 2c20 633a 206d 6178  ambda cs, c: max
-00001270: 285b 6564 6174 612e 7375 7070 6f72 7428  ([edata.support(
-00001280: 5f63 2c63 2920 666f 7220 5f63 2069 6e20  _c,c) for _c in 
-00001290: 6373 5d29 0a20 2020 207d 200a 2020 2020  cs]).    } .    
-000012a0: 0a20 2020 2063 616e 6473 203d 207b 0a20  .    cands = {. 
-000012b0: 2020 2020 2020 2022 7769 6e6e 696e 6722         "winning"
-000012c0: 3a20 6c61 6d62 6461 2063 3a20 6564 6174  : lambda c: edat
-000012d0: 612e 646f 6d69 6e61 746f 7273 2863 2c20  a.dominators(c, 
-000012e0: 6375 7272 5f63 616e 6473 203d 2063 7572  curr_cands = cur
-000012f0: 725f 6361 6e64 7329 2c0a 2020 2020 2020  r_cands),.      
-00001300: 2020 226d 6172 6769 6e73 223a 206c 616d    "margins": lam
-00001310: 6264 6120 633a 2065 6461 7461 2e64 6f6d  bda c: edata.dom
-00001320: 696e 6174 6f72 7328 632c 2063 7572 725f  inators(c, curr_
-00001330: 6361 6e64 7320 3d20 6375 7272 5f63 616e  cands = curr_can
-00001340: 6473 292c 0a20 2020 2020 2020 2022 7061  ds),.        "pa
-00001350: 6972 7769 7365 5f6f 7070 6f73 6974 696f  irwise_oppositio
-00001360: 6e22 3a20 6c61 6d62 6461 2063 3a20 5b5f  n": lambda c: [_
-00001370: 6320 666f 7220 5f63 2069 6e20 6361 6e64  c for _c in cand
-00001380: 6964 6174 6573 2069 6620 5f63 2021 3d20  idates if _c != 
-00001390: 635d 0a20 2020 207d 200a 0a20 2020 2072  c].    } ..    r
-000013a0: 6574 7572 6e20 7b63 3a20 2d31 202a 2073  eturn {c: -1 * s
-000013b0: 636f 7265 5f66 756e 6374 696f 6e73 5b73  core_functions[s
-000013c0: 636f 7265 5f6d 6574 686f 645d 2863 616e  core_method](can
-000013d0: 6473 5b73 636f 7265 5f6d 6574 686f 645d  ds[score_method]
-000013e0: 2863 292c 2063 2920 666f 7220 6320 696e  (c), c) for c in
-000013f0: 2063 616e 6469 6461 7465 737d 0a0a 0a64   candidates}...d
-00001400: 6566 206d 6178 696d 616c 5f65 6c65 6d65  ef maximal_eleme
-00001410: 6e74 7328 6729 3a20 0a20 2020 2022 2222  nts(g): .    """
-00001420: 7265 7475 726e 2074 6865 206e 6f64 6573  return the nodes
-00001430: 2069 6e20 6720 7769 7468 206e 6f20 696e   in g with no in
-00001440: 636f 6d69 6e67 2061 7272 6f77 732e 2222  coming arrows.""
-00001450: 220a 2020 2020 7265 7475 726e 205b 6e20  ".    return [n 
-00001460: 666f 7220 6e20 696e 2067 2e6e 6f64 6573  for n in g.nodes
-00001470: 2069 6620 672e 696e 5f64 6567 7265 6528   if g.in_degree(
-00001480: 6e29 203d 3d20 305d 0a0a 0a64 6566 205f  n) == 0]...def _
-00001490: 6265 6174 5f70 6174 685f 6261 7369 6328  beat_path_basic(
-000014a0: 6564 6174 612c 200a 2020 2020 2020 2020  edata, .        
-000014b0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-000014c0: 725f 6361 6e64 7320 3d20 4e6f 6e65 2c20  r_cands = None, 
-000014d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000014e0: 2020 2020 2020 7374 7265 6e67 7468 5f66        strength_f
-000014f0: 756e 6374 696f 6e20 3d20 4e6f 6e65 293a  unction = None):
-00001500: 200a 2020 2020 2222 2241 6e20 696d 706c   .    """An impl
-00001510: 656d 656e 7461 7469 6f6e 206f 6620 7468  ementation of th
-00001520: 6520 4265 6174 2050 6174 6820 6d65 7468  e Beat Path meth
-00001530: 6f64 2074 6861 7420 7573 6573 2061 2062  od that uses a b
-00001540: 6173 6963 2061 6c67 6f72 6974 686d 2e20  asic algorithm. 
-00001550: 2054 6869 7320 6973 206e 6f74 2065 6666   This is not eff
-00001560: 6963 6965 6e74 2066 6f72 206c 6172 6765  icient for large
-00001570: 2067 7261 7068 732e 0a20 2020 200a 2020   graphs..    .  
-00001580: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00001590: 6564 6174 6120 2850 726f 6669 6c65 2c20  edata (Profile, 
-000015a0: 5072 6f66 696c 6557 6974 6854 6965 732c  ProfileWithTies,
-000015b0: 204d 6172 6769 6e47 7261 7068 293a 2041   MarginGraph): A
-000015c0: 6e79 2065 6c65 6374 696f 6e20 6461 7461  ny election data
-000015d0: 2074 6861 7420 6861 7320 6120 606d 6172   that has a `mar
-000015e0: 6769 6e60 206d 6574 686f 642e 200a 2020  gin` method. .  
-000015f0: 2020 2020 2020 6375 7272 5f63 616e 6473        curr_cands
-00001600: 2028 4c69 7374 5b69 6e74 5d2c 206f 7074   (List[int], opt
-00001610: 696f 6e61 6c29 3a20 4966 2073 6574 2c20  ional): If set, 
-00001620: 7468 656e 2066 696e 6420 7468 6520 7769  then find the wi
-00001630: 6e6e 6572 7320 666f 7220 7468 6520 7072  nners for the pr
-00001640: 6f66 696c 6520 7265 7374 7269 6374 6564  ofile restricted
-00001650: 2074 6f20 7468 6520 6361 6e64 6964 6174   to the candidat
-00001660: 6573 2069 6e20 6060 6375 7272 5f63 616e  es in ``curr_can
-00001670: 6473 6060 0a20 2020 2020 2020 2073 7472  ds``.        str
-00001680: 656e 6774 685f 6675 6e63 7469 6f6e 2028  ength_function (
-00001690: 6675 6e63 7469 6f6e 2c20 6f70 7469 6f6e  function, option
-000016a0: 616c 293a 2054 6865 2073 7472 656e 6774  al): The strengt
-000016b0: 6820 6675 6e63 7469 6f6e 2074 6f20 6265  h function to be
-000016c0: 2075 7365 6420 746f 2063 616c 6375 6c61   used to calcula
-000016d0: 7465 2074 6865 2073 7472 656e 6774 6820  te the strength 
-000016e0: 6f66 2061 2070 6174 682e 2020 2054 6865  of a path.   The
-000016f0: 2064 6566 6175 6c74 2069 7320 7468 6520   default is the 
-00001700: 6d61 7267 696e 206d 6574 686f 6420 6f66  margin method of
-00001710: 2060 6065 6461 7461 6060 2e20 2020 5468   ``edata``.   Th
-00001720: 6973 206f 6e6c 7920 6d61 7474 6572 7320  is only matters 
-00001730: 7768 656e 2074 6865 2062 616c 6c6f 7473  when the ballots
-00001740: 2061 7265 206e 6f74 206c 696e 6561 7220   are not linear 
-00001750: 6f72 6465 7273 2e20 0a0a 2020 2020 5265  orders. ..    Re
-00001760: 7475 726e 733a 200a 2020 2020 2020 2020  turns: .        
-00001770: 4120 736f 7274 6564 206c 6973 7420 6f66  A sorted list of
-00001780: 2063 616e 6469 6461 7465 732e 200a 0a20   candidates. .. 
-00001790: 2020 2022 2222 0a20 2020 200a 2020 2020     """.    .    
-000017a0: 6361 6e64 6964 6174 6573 203d 2065 6461  candidates = eda
-000017b0: 7461 2e63 616e 6469 6461 7465 7320 6966  ta.candidates if
-000017c0: 2063 7572 725f 6361 6e64 7320 6973 204e   curr_cands is N
-000017d0: 6f6e 6520 656c 7365 2063 7572 725f 6361  one else curr_ca
-000017e0: 6e64 7320 2020 200a 2020 2020 7374 7265  nds    .    stre
-000017f0: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
-00001800: 6564 6174 612e 6d61 7267 696e 2069 6620  edata.margin if 
-00001810: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-00001820: 6e20 6973 204e 6f6e 6520 656c 7365 2073  n is None else s
-00001830: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-00001840: 0a20 2020 200a 2020 2020 6d67 203d 2067  .    .    mg = g
-00001850: 6574 5f6d 6728 6564 6174 612c 2063 7572  et_mg(edata, cur
-00001860: 725f 6361 6e64 7320 3d20 6375 7272 5f63  r_cands = curr_c
-00001870: 616e 6473 290a 2020 2020 0a20 2020 2062  ands).    .    b
-00001880: 6561 745f 7061 7468 735f 7765 6967 6874  eat_paths_weight
-00001890: 7320 3d20 7b63 3a20 7b63 323a 3020 666f  s = {c: {c2:0 fo
-000018a0: 7220 6332 2069 6e20 6361 6e64 6964 6174  r c2 in candidat
-000018b0: 6573 2069 6620 6332 2021 3d20 637d 2066  es if c2 != c} f
-000018c0: 6f72 2063 2069 6e20 6361 6e64 6964 6174  or c in candidat
-000018d0: 6573 7d0a 2020 2020 666f 7220 6320 696e  es}.    for c in
-000018e0: 2063 616e 6469 6461 7465 733a 200a 2020   candidates: .  
-000018f0: 2020 2020 2020 666f 7220 6f74 6865 725f        for other_
-00001900: 6320 696e 2062 6561 745f 7061 7468 735f  c in beat_paths_
-00001910: 7765 6967 6874 735b 635d 2e6b 6579 7328  weights[c].keys(
-00001920: 293a 0a20 2020 2020 2020 2020 2020 2061  ):.            a
-00001930: 6c6c 5f70 6174 6873 203d 2020 6c69 7374  ll_paths =  list
-00001940: 286e 782e 616c 6c5f 7369 6d70 6c65 5f70  (nx.all_simple_p
-00001950: 6174 6873 286d 672c 2063 2c20 6f74 6865  aths(mg, c, othe
-00001960: 725f 6329 290a 2020 2020 2020 2020 2020  r_c)).          
-00001970: 2020 6966 206c 656e 2861 6c6c 5f70 6174    if len(all_pat
-00001980: 6873 2920 3e20 303a 0a20 2020 2020 2020  hs) > 0:.       
-00001990: 2020 2020 2020 2020 2062 6561 745f 7061           beat_pa
-000019a0: 7468 735f 7765 6967 6874 735b 635d 5b6f  ths_weights[c][o
-000019b0: 7468 6572 5f63 5d20 3d20 6d61 7828 5b6d  ther_c] = max([m
-000019c0: 696e 285b 7374 7265 6e67 7468 5f66 756e  in([strength_fun
-000019d0: 6374 696f 6e28 705b 695d 2c20 705b 692b  ction(p[i], p[i+
-000019e0: 315d 2920 0a20 2020 2020 2020 2020 2020  1]) .           
-000019f0: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-00001a00: 6e67 6528 302c 6c65 6e28 7029 2d31 295d  nge(0,len(p)-1)]
-00001a10: 2920 0a20 2020 2020 2020 2020 2020 2020  ) .             
-00001a20: 2020 2066 6f72 2070 2069 6e20 616c 6c5f     for p in all_
-00001a30: 7061 7468 735d 290a 2020 2020 0a20 2020  paths]).    .   
-00001a40: 2077 696e 6e65 7273 203d 206c 6973 7428   winners = list(
-00001a50: 290a 2020 2020 666f 7220 6320 696e 2063  ).    for c in c
-00001a60: 616e 6469 6461 7465 733a 200a 2020 2020  andidates: .    
-00001a70: 2020 2020 6966 2061 6c6c 285b 6265 6174      if all([beat
-00001a80: 5f70 6174 6873 5f77 6569 6768 7473 5b63  _paths_weights[c
-00001a90: 5d5b 6332 5d20 3e3d 2062 6561 745f 7061  ][c2] >= beat_pa
-00001aa0: 7468 735f 7765 6967 6874 735b 6332 5d5b  ths_weights[c2][
-00001ab0: 635d 2066 6f72 2063 3220 696e 2063 616e  c] for c2 in can
-00001ac0: 6469 6461 7465 7320 2069 6620 6332 2021  didates  if c2 !
-00001ad0: 3d20 635d 293a 0a20 2020 2020 2020 2020  = c]):.         
-00001ae0: 2020 2077 696e 6e65 7273 2e61 7070 656e     winners.appen
-00001af0: 6428 6329 0a20 2020 2072 6574 7572 6e20  d(c).    return 
-00001b00: 736f 7274 6564 286c 6973 7428 7769 6e6e  sorted(list(winn
-00001b10: 6572 7329 290a 0a0a 6465 6620 5f62 6561  ers))...def _bea
-00001b20: 745f 7061 7468 5f66 6c6f 7964 5f77 6172  t_path_floyd_war
-00001b30: 7368 616c 6c28 0a20 2020 2020 2020 2065  shall(.        e
-00001b40: 6461 7461 2c20 0a20 2020 2020 2020 2063  data, .        c
-00001b50: 7572 725f 6361 6e64 7320 3d20 4e6f 6e65  urr_cands = None
-00001b60: 2c20 0a20 2020 2020 2020 2073 7472 656e  , .        stren
-00001b70: 6774 685f 6675 6e63 7469 6f6e 203d 204e  gth_function = N
-00001b80: 6f6e 6529 3a20 2020 0a20 2020 2022 2222  one):   .    """
-00001b90: 416e 2069 6d70 6c65 6d65 6e74 6174 696f  An implementatio
-00001ba0: 6e20 6f66 2042 6561 7420 5061 7468 2075  n of Beat Path u
-00001bb0: 7369 6e67 2061 2076 6172 6961 7469 6f6e  sing a variation
-00001bc0: 206f 6620 7468 6520 466c 6f79 642d 5761   of the Floyd-Wa
-00001bd0: 7273 6861 6c6c 2041 6c67 6f72 6974 686d  rshall Algorithm
-00001be0: 0a20 2020 2053 6565 2068 7474 7073 3a2f  .    See https:/
-00001bf0: 2f65 6e2e 7769 6b69 7065 6469 612e 6f72  /en.wikipedia.or
-00001c00: 672f 7769 6b69 2f53 6368 756c 7a65 5f6d  g/wiki/Schulze_m
-00001c10: 6574 686f 6423 496d 706c 656d 656e 7461  ethod#Implementa
-00001c20: 7469 6f6e 290a 200a 2020 2020 4172 6773  tion). .    Args
-00001c30: 3a0a 2020 2020 2020 2020 6564 6174 6120  :.        edata 
-00001c40: 2850 726f 6669 6c65 2c20 5072 6f66 696c  (Profile, Profil
-00001c50: 6557 6974 6854 6965 732c 204d 6172 6769  eWithTies, Margi
-00001c60: 6e47 7261 7068 293a 2041 6e79 2065 6c65  nGraph): Any ele
-00001c70: 6374 696f 6e20 6461 7461 2074 6861 7420  ction data that 
-00001c80: 6861 7320 6120 606d 6172 6769 6e60 206d  has a `margin` m
-00001c90: 6574 686f 642e 200a 2020 2020 2020 2020  ethod. .        
-00001ca0: 6375 7272 5f63 616e 6473 2028 4c69 7374  curr_cands (List
-00001cb0: 5b69 6e74 5d2c 206f 7074 696f 6e61 6c29  [int], optional)
-00001cc0: 3a20 4966 2073 6574 2c20 7468 656e 2066  : If set, then f
-00001cd0: 696e 6420 7468 6520 7769 6e6e 6572 7320  ind the winners 
-00001ce0: 666f 7220 7468 6520 7072 6f66 696c 6520  for the profile 
-00001cf0: 7265 7374 7269 6374 6564 2074 6f20 7468  restricted to th
-00001d00: 6520 6361 6e64 6964 6174 6573 2069 6e20  e candidates in 
-00001d10: 6060 6375 7272 5f63 616e 6473 6060 0a20  ``curr_cands``. 
-00001d20: 2020 2020 2020 2073 7472 656e 6774 685f         strength_
-00001d30: 6675 6e63 7469 6f6e 2028 6675 6e63 7469  function (functi
-00001d40: 6f6e 2c20 6f70 7469 6f6e 616c 293a 2054  on, optional): T
-00001d50: 6865 2073 7472 656e 6774 6820 6675 6e63  he strength func
-00001d60: 7469 6f6e 2074 6f20 6265 2075 7365 6420  tion to be used 
-00001d70: 746f 2063 616c 6375 6c61 7465 2074 6865  to calculate the
-00001d80: 2073 7472 656e 6774 6820 6f66 2061 2070   strength of a p
-00001d90: 6174 682e 2020 2054 6865 2064 6566 6175  ath.   The defau
-00001da0: 6c74 2069 7320 7468 6520 6d61 7267 696e  lt is the margin
-00001db0: 206d 6574 686f 6420 6f66 2060 6065 6461   method of ``eda
-00001dc0: 7461 6060 2e20 2020 5468 6973 206f 6e6c  ta``.   This onl
-00001dd0: 7920 6d61 7474 6572 7320 7768 656e 2074  y matters when t
-00001de0: 6865 2062 616c 6c6f 7473 2061 7265 206e  he ballots are n
-00001df0: 6f74 206c 696e 6561 7220 6f72 6465 7273  ot linear orders
-00001e00: 2e20 0a0a 2020 2020 5265 7475 726e 733a  . ..    Returns:
-00001e10: 200a 2020 2020 2020 2020 4120 736f 7274   .        A sort
-00001e20: 6564 206c 6973 7420 6f66 2063 616e 6469  ed list of candi
-00001e30: 6461 7465 732e 200a 0a20 2020 2022 2222  dates. ..    """
-00001e40: 0a0a 2020 2020 6361 6e64 6964 6174 6573  ..    candidates
-00001e50: 203d 2065 6461 7461 2e63 616e 6469 6461   = edata.candida
-00001e60: 7465 7320 6966 2063 7572 725f 6361 6e64  tes if curr_cand
-00001e70: 7320 6973 204e 6f6e 6520 656c 7365 2063  s is None else c
-00001e80: 7572 725f 6361 6e64 7320 2020 200a 2020  urr_cands    .  
+00000260: 6b78 2061 7320 6e78 0a66 726f 6d20 7072  kx as nx.from pr
+00000270: 6566 5f76 6f74 696e 672e 766f 7469 6e67  ef_voting.voting
+00000280: 5f6d 6574 686f 645f 7072 6f70 6572 7469  _method_properti
+00000290: 6573 2069 6d70 6f72 7420 566f 7469 6e67  es import Voting
+000002a0: 4d65 7468 6f64 5072 6f70 6572 7469 6573  MethodProperties
+000002b0: 2c20 456c 6563 7469 6f6e 5479 7065 730a  , ElectionTypes.
+000002c0: 0a6d 696e 696d 6178 5f70 726f 7065 7274  .minimax_propert
+000002d0: 6965 7320 3d20 566f 7469 6e67 4d65 7468  ies = VotingMeth
+000002e0: 6f64 5072 6f70 6572 7469 6573 280a 2020  odProperties(.  
+000002f0: 2020 636f 6e64 6f72 6365 745f 7769 6e6e    condorcet_winn
+00000300: 6572 3d54 7275 652c 200a 2020 2020 636f  er=True, .    co
+00000310: 6e64 6f72 6365 745f 6c6f 7365 723d 4661  ndorcet_loser=Fa
+00000320: 6c73 652c 0a20 2020 2070 6172 6574 6f5f  lse,.    pareto_
+00000330: 646f 6d69 6e61 6e63 653d 5472 7565 2c20  dominance=True, 
+00000340: 0a20 2020 2029 0a40 766d 286e 616d 6520  .    ).@vm(name 
+00000350: 3d20 224d 696e 696d 6178 222c 0a20 2020  = "Minimax",.   
+00000360: 2070 726f 7065 7274 6965 733d 6d69 6e69   properties=mini
+00000370: 6d61 785f 7072 6f70 6572 7469 6573 2c0a  max_properties,.
+00000380: 2020 2020 696e 7075 745f 7479 7065 733d      input_types=
+00000390: 5b45 6c65 6374 696f 6e54 7970 6573 2e50  [ElectionTypes.P
+000003a0: 524f 4649 4c45 2c20 456c 6563 7469 6f6e  ROFILE, Election
+000003b0: 5479 7065 732e 5052 4f46 494c 455f 5749  Types.PROFILE_WI
+000003c0: 5448 5f54 4945 532c 2045 6c65 6374 696f  TH_TIES, Electio
+000003d0: 6e54 7970 6573 2e4d 4152 4749 4e5f 4752  nTypes.MARGIN_GR
+000003e0: 4150 485d 0a20 2020 2029 0a64 6566 206d  APH].    ).def m
+000003f0: 696e 696d 6178 2865 6461 7461 2c20 6375  inimax(edata, cu
+00000400: 7272 5f63 616e 6473 203d 204e 6f6e 652c  rr_cands = None,
+00000410: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+00000420: 6f6e 203d 204e 6f6e 6529 3a20 2020 0a20  on = None):   . 
+00000430: 2020 2022 2222 0a20 2020 2054 6865 204d     """.    The M
+00000440: 696e 696d 6178 2077 696e 6e65 7273 2061  inimax winners a
+00000450: 7265 2074 6865 2063 616e 6469 6461 7465  re the candidate
+00000460: 7320 7769 7468 2074 6865 2073 6d61 6c6c  s with the small
+00000470: 6573 7420 6d61 7869 6d75 6d20 7061 6972  est maximum pair
+00000480: 7769 7365 206c 6f73 732e 2020 5468 6174  wise loss.  That
+00000490: 2069 732c 2066 6f72 2065 6163 6820 6361   is, for each ca
+000004a0: 6e64 6964 6174 6520 3a6d 6174 683a 6061  ndidate :math:`a
+000004b0: 602c 2066 696e 6420 7468 6520 6269 6767  `, find the bigg
+000004c0: 6573 7420 6d61 7267 696e 206f 6620 6120  est margin of a 
+000004d0: 6361 6e64 6964 6174 6520 3a6d 6174 683a  candidate :math:
+000004e0: 6062 6020 6f76 6572 203a 6d61 7468 3a60  `b` over :math:`
+000004f0: 6160 2c20 7468 656e 2065 6c65 6374 2074  a`, then elect t
+00000500: 6865 2063 616e 6469 6461 7465 2873 2920  he candidate(s) 
+00000510: 7769 7468 2074 6865 2073 6d61 6c6c 6573  with the smalles
+00000520: 7420 7375 6368 206c 6f73 732e 2041 6c73  t such loss. Als
+00000530: 6f20 6b6e 6f77 6e20 6173 2074 6865 2053  o known as the S
+00000540: 696d 7073 6f6e 2d4b 7261 6d65 7220 5275  impson-Kramer Ru
+00000550: 6c65 2e0a 2020 2020 0a20 2020 2041 7267  le..    .    Arg
+00000560: 733a 0a20 2020 2020 2020 2065 6461 7461  s:.        edata
+00000570: 2028 5072 6f66 696c 652c 2050 726f 6669   (Profile, Profi
+00000580: 6c65 5769 7468 5469 6573 2c20 4d61 7267  leWithTies, Marg
+00000590: 696e 4772 6170 6829 3a20 416e 7920 656c  inGraph): Any el
+000005a0: 6563 7469 6f6e 2064 6174 6120 7468 6174  ection data that
+000005b0: 2068 6173 2061 2060 6d61 7267 696e 6020   has a `margin` 
+000005c0: 6d65 7468 6f64 2e20 0a20 2020 2020 2020  method. .       
+000005d0: 2063 7572 725f 6361 6e64 7320 284c 6973   curr_cands (Lis
+000005e0: 745b 696e 745d 2c20 6f70 7469 6f6e 616c  t[int], optional
+000005f0: 293a 2049 6620 7365 742c 2074 6865 6e20  ): If set, then 
+00000600: 6669 6e64 2074 6865 2077 696e 6e65 7273  find the winners
+00000610: 2066 6f72 2074 6865 2070 726f 6669 6c65   for the profile
+00000620: 2072 6573 7472 6963 7465 6420 746f 2074   restricted to t
+00000630: 6865 2063 616e 6469 6461 7465 7320 696e  he candidates in
+00000640: 2060 6063 7572 725f 6361 6e64 7360 600a   ``curr_cands``.
+00000650: 0a20 2020 2052 6574 7572 6e73 3a20 0a20  .    Returns: . 
+00000660: 2020 2020 2020 2041 2073 6f72 7465 6420         A sorted 
+00000670: 6c69 7374 206f 6620 6361 6e64 6964 6174  list of candidat
+00000680: 6573 0a0a 2020 2020 2e2e 2073 6565 616c  es..    .. seeal
+00000690: 736f 3a3a 0a0a 2020 2020 2020 2020 3a6d  so::..        :m
+000006a0: 6574 683a 6070 7265 665f 766f 7469 6e67  eth:`pref_voting
+000006b0: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
+000006c0: 7468 6f64 732e 6d69 6e69 6d61 785f 7363  thods.minimax_sc
+000006d0: 6f72 6573 600a 0a20 2020 203a 4578 616d  ores`..    :Exam
+000006e0: 706c 653a 200a 0a20 2020 202e 2e20 706c  ple: ..    .. pl
+000006f0: 6f74 3a3a 2020 6d61 7267 696e 5f67 7261  ot::  margin_gra
+00000700: 7068 735f 6578 616d 706c 6573 2f6d 675f  phs_examples/mg_
+00000710: 6578 5f6d 696e 696d 6178 2e70 790a 2020  ex_minimax.py.  
+00000720: 2020 2020 2020 3a63 6f6e 7465 7874 3a20        :context: 
+00000730: 7265 7365 7420 200a 2020 2020 2020 2020  reset  .        
+00000740: 3a69 6e63 6c75 6465 2d73 6f75 7263 653a  :include-source:
+00000750: 2054 7275 650a 0a0a 2020 2020 2e2e 2063   True...    .. c
+00000760: 6f64 652d 626c 6f63 6b3a 3a20 0a0a 2020  ode-block:: ..  
+00000770: 2020 2020 2020 6672 6f6d 2070 7265 665f        from pref_
+00000780: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
+00000790: 7365 645f 6d65 7468 6f64 7320 696d 706f  sed_methods impo
+000007a0: 7274 206d 696e 696d 6178 0a0a 2020 2020  rt minimax..    
+000007b0: 2020 2020 6d69 6e69 6d61 782e 6469 7370      minimax.disp
+000007c0: 6c61 7928 7072 6f66 290a 0a0a 2020 2020  lay(prof)...    
+000007d0: 2e2e 2065 7865 635f 636f 6465 3a3a 200a  .. exec_code:: .
+000007e0: 2020 2020 2020 2020 3a68 6964 655f 636f          :hide_co
+000007f0: 6465 3a0a 0a20 2020 2020 2020 2066 726f  de:..        fro
+00000800: 6d20 7072 6566 5f76 6f74 696e 672e 7072  m pref_voting.pr
+00000810: 6f66 696c 6573 2069 6d70 6f72 7420 5072  ofiles import Pr
+00000820: 6f66 696c 650a 2020 2020 2020 2020 6672  ofile.        fr
+00000830: 6f6d 2070 7265 665f 766f 7469 6e67 2e6d  om pref_voting.m
+00000840: 6172 6769 6e5f 6261 7365 645f 6d65 7468  argin_based_meth
+00000850: 6f64 7320 696d 706f 7274 206d 696e 696d  ods import minim
+00000860: 6178 0a20 2020 2020 2020 200a 2020 2020  ax.        .    
+00000870: 2020 2020 7072 6f66 203d 2050 726f 6669      prof = Profi
+00000880: 6c65 285b 5b33 2c20 302c 2031 2c20 325d  le([[3, 0, 1, 2]
+00000890: 2c20 5b31 2c20 332c 2032 2c20 305d 2c20  , [1, 3, 2, 0], 
+000008a0: 5b31 2c20 332c 2030 2c20 325d 2c20 5b31  [1, 3, 0, 2], [1
+000008b0: 2c20 322c 2030 2c20 335d 2c20 5b33 2c20  , 2, 0, 3], [3, 
+000008c0: 322c 2030 2c20 315d 2c20 5b30 2c20 322c  2, 0, 1], [0, 2,
+000008d0: 2031 2c20 335d 5d2c 205b 312c 2031 2c20   1, 3]], [1, 1, 
+000008e0: 312c 2031 2c20 322c 2031 5d29 0a0a 2020  1, 1, 2, 1])..  
+000008f0: 2020 2020 2020 6d69 6e69 6d61 782e 6469        minimax.di
+00000900: 7370 6c61 7928 7072 6f66 290a 0a20 2020  splay(prof)..   
+00000910: 2022 2222 0a0a 2020 2020 6361 6e64 6964   """..    candid
+00000920: 6174 6573 203d 2065 6461 7461 2e63 616e  ates = edata.can
+00000930: 6469 6461 7465 7320 6966 2063 7572 725f  didates if curr_
+00000940: 6361 6e64 7320 6973 204e 6f6e 6520 656c  cands is None el
+00000950: 7365 2063 7572 725f 6361 6e64 7320 2020  se curr_cands   
+00000960: 200a 2020 2020 7374 7265 6e67 7468 5f66   .    strength_f
+00000970: 756e 6374 696f 6e20 3d20 6564 6174 612e  unction = edata.
+00000980: 6d61 7267 696e 2069 6620 7374 7265 6e67  margin if streng
+00000990: 7468 5f66 756e 6374 696f 6e20 6973 204e  th_function is N
+000009a0: 6f6e 6520 656c 7365 2073 7472 656e 6774  one else strengt
+000009b0: 685f 6675 6e63 7469 6f6e 0a0a 2020 2020  h_function..    
+000009c0: 7363 6f72 6573 203d 207b 633a 206d 6178  scores = {c: max
+000009d0: 285b 7374 7265 6e67 7468 5f66 756e 6374  ([strength_funct
+000009e0: 696f 6e28 5f63 2c20 6329 2066 6f72 205f  ion(_c, c) for _
+000009f0: 6320 696e 2065 6461 7461 2e64 6f6d 696e  c in edata.domin
+00000a00: 6174 6f72 7328 6329 2069 6620 5f63 2069  ators(c) if _c i
+00000a10: 6e20 6361 6e64 6964 6174 6573 5d29 2069  n candidates]) i
+00000a20: 6620 616e 7928 5b5f 6320 696e 2065 6461  f any([_c in eda
+00000a30: 7461 2e64 6f6d 696e 6174 6f72 7328 6329  ta.dominators(c)
+00000a40: 2066 6f72 205f 6320 696e 2063 616e 6469   for _c in candi
+00000a50: 6461 7465 735d 2920 656c 7365 2030 200a  dates]) else 0 .
+00000a60: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00000a70: 7220 6320 696e 2063 616e 6469 6461 7465  r c in candidate
+00000a80: 737d 0a20 2020 206d 696e 5f73 636f 7265  s}.    min_score
+00000a90: 203d 206d 696e 2873 636f 7265 732e 7661   = min(scores.va
+00000aa0: 6c75 6573 2829 290a 2020 2020 7265 7475  lues()).    retu
+00000ab0: 726e 2073 6f72 7465 6428 5b63 2066 6f72  rn sorted([c for
+00000ac0: 2063 2069 6e20 6361 6e64 6964 6174 6573   c in candidates
+00000ad0: 2069 6620 7363 6f72 6573 5b63 5d20 3d3d   if scores[c] ==
+00000ae0: 206d 696e 5f73 636f 7265 5d29 0a0a 0a64   min_score])...d
+00000af0: 6566 206d 696e 696d 6178 5f73 636f 7265  ef minimax_score
+00000b00: 7328 6564 6174 612c 2063 7572 725f 6361  s(edata, curr_ca
+00000b10: 6e64 7320 3d20 4e6f 6e65 2c20 7363 6f72  nds = None, scor
+00000b20: 655f 6d65 7468 6f64 3d22 6d61 7267 696e  e_method="margin
+00000b30: 7322 293a 0a20 2020 2022 2222 5265 7475  s"):.    """Retu
+00000b40: 726e 2074 6865 206d 696e 696d 6178 2073  rn the minimax s
+00000b50: 636f 7265 7320 666f 7220 6561 6368 2063  cores for each c
+00000b60: 616e 6469 6461 7465 2c20 7768 6572 6520  andidate, where 
+00000b70: 7468 6520 6d69 6e69 6d61 7820 7363 6f72  the minimax scor
+00000b80: 6520 666f 7220 3a6d 6174 683a 6063 6020  e for :math:`c` 
+00000b90: 6973 202d 3120 2a20 7468 6520 6d61 7869  is -1 * the maxi
+00000ba0: 6d75 6d20 7061 6972 7769 7365 206d 616a  mum pairwise maj
+00000bb0: 6f72 6974 7920 6c6f 7373 2e20 0a0a 2020  ority loss. ..  
+00000bc0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00000bd0: 6564 6174 6120 2850 726f 6669 6c65 2c20  edata (Profile, 
+00000be0: 5072 6f66 696c 6557 6974 6854 6965 732c  ProfileWithTies,
+00000bf0: 204d 6172 6769 6e47 7261 7068 293a 2041   MarginGraph): A
+00000c00: 6e79 2065 6c65 6374 696f 6e20 6461 7461  ny election data
+00000c10: 2074 6861 7420 6861 7320 6120 606d 6172   that has a `mar
+00000c20: 6769 6e60 206d 6574 686f 642e 200a 2020  gin` method. .  
+00000c30: 2020 2020 2020 6375 7272 5f63 616e 6473        curr_cands
+00000c40: 2028 4c69 7374 5b69 6e74 5d2c 206f 7074   (List[int], opt
+00000c50: 696f 6e61 6c29 3a20 4966 2073 6574 2c20  ional): If set, 
+00000c60: 7468 656e 2066 696e 6420 7468 6520 7769  then find the wi
+00000c70: 6e6e 6572 7320 666f 7220 7468 6520 7072  nners for the pr
+00000c80: 6f66 696c 6520 7265 7374 7269 6374 6564  ofile restricted
+00000c90: 2074 6f20 7468 6520 6361 6e64 6964 6174   to the candidat
+00000ca0: 6573 2069 6e20 6060 6375 7272 5f63 616e  es in ``curr_can
+00000cb0: 6473 6060 0a20 2020 2020 2020 2073 636f  ds``.        sco
+00000cc0: 7265 5f6d 6574 686f 6420 2873 7472 2c20  re_method (str, 
+00000cd0: 6f70 7469 6f6e 616c 293a 204f 7074 696f  optional): Optio
+00000ce0: 6e73 2069 6e63 6c75 6465 2022 6d61 7267  ns include "marg
+00000cf0: 696e 7322 2028 7468 6520 6465 6661 756c  ins" (the defaul
+00000d00: 7429 2c20 2277 696e 6e69 6e67 2220 6173  t), "winning" as
+00000d10: 7369 676e 7320 746f 2065 6163 6820 6361  signs to each ca
+00000d20: 6e64 6964 6174 6520 3a6d 6174 683a 6063  ndidate :math:`c
+00000d30: 6020 7468 6520 6d61 7869 6d75 6d20 7375  ` the maximum su
+00000d40: 7070 6f72 7420 6f66 2061 2063 616e 6469  pport of a candi
+00000d50: 6461 7465 206d 616a 6f72 6974 7920 7072  date majority pr
+00000d60: 6566 6572 7265 6420 746f 203a 6d61 7468  eferred to :math
+00000d70: 3a60 6360 2c20 2061 6e64 2022 7061 6972  :`c`,  and "pair
+00000d80: 7769 7365 5f6f 7070 6f73 6974 696f 6e22  wise_opposition"
+00000d90: 2061 7373 6967 6e73 2074 6f20 6561 6368   assigns to each
+00000da0: 2063 616e 6469 6461 7465 203a 6d61 7468   candidate :math
+00000db0: 3a60 6360 2074 6865 206d 6178 696d 756d  :`c` the maximum
+00000dc0: 2073 7570 706f 7274 206f 6620 616e 7920   support of any 
+00000dd0: 6361 6e64 6964 6174 6520 6f76 6572 203a  candidate over :
+00000de0: 6d61 7468 3a60 6360 2e20 2020 5468 6573  math:`c`.   Thes
+00000df0: 6520 7363 6f72 6573 206f 6e6c 7920 6c65  e scores only le
+00000e00: 6164 2074 6f20 6469 6666 6572 656e 7420  ad to different 
+00000e10: 7265 7375 6c74 7320 6f6e 206e 6f6e 2d6c  results on non-l
+00000e20: 696e 6561 7220 7072 6f66 696c 6573 2e20  inear profiles. 
+00000e30: 0a0a 2020 2020 5265 7475 726e 733a 200a  ..    Returns: .
+00000e40: 2020 2020 2020 2020 4120 6469 6374 696f          A dictio
+00000e50: 6e61 7279 2061 7373 6f63 6961 7469 6e67  nary associating
+00000e60: 2065 6163 6820 6361 6e64 6964 6174 6520   each candidate 
+00000e70: 7769 7468 2069 7473 206d 696e 696d 6178  with its minimax
+00000e80: 2073 636f 7265 2e0a 0a20 2020 202e 2e20   score...    .. 
+00000e90: 7365 6561 6c73 6f3a 3a0a 0a20 2020 2020  seealso::..     
+00000ea0: 2020 203a 6d65 7468 3a60 7072 6566 5f76     :meth:`pref_v
+00000eb0: 6f74 696e 672e 6d61 7267 696e 5f62 6173  oting.margin_bas
+00000ec0: 6564 5f6d 6574 686f 6473 2e6d 696e 696d  ed_methods.minim
+00000ed0: 6178 600a 0a20 2020 203a 4578 616d 706c  ax`..    :Exampl
+00000ee0: 653a 200a 0a20 2020 202e 2e20 706c 6f74  e: ..    .. plot
+00000ef0: 3a3a 2020 6d61 7267 696e 5f67 7261 7068  ::  margin_graph
+00000f00: 735f 6578 616d 706c 6573 2f6d 675f 6578  s_examples/mg_ex
+00000f10: 5f6d 696e 696d 6178 2e70 790a 2020 2020  _minimax.py.    
+00000f20: 2020 2020 3a63 6f6e 7465 7874 3a20 7265      :context: re
+00000f30: 7365 7420 200a 2020 2020 2020 2020 3a69  set  .        :i
+00000f40: 6e63 6c75 6465 2d73 6f75 7263 653a 2054  nclude-source: T
+00000f50: 7275 650a 0a0a 2020 2020 2e2e 2063 6f64  rue...    .. cod
+00000f60: 652d 626c 6f63 6b3a 3a20 0a0a 2020 2020  e-block:: ..    
+00000f70: 2020 2020 6672 6f6d 2070 7265 665f 766f      from pref_vo
+00000f80: 7469 6e67 2e6d 6172 6769 6e5f 6261 7365  ting.margin_base
+00000f90: 645f 6d65 7468 6f64 7320 696d 706f 7274  d_methods import
+00000fa0: 206d 696e 696d 6178 5f73 636f 7265 732c   minimax_scores,
+00000fb0: 206d 696e 696d 6178 0a0a 2020 2020 2020   minimax..      
+00000fc0: 2020 6d69 6e69 6d61 782e 6469 7370 6c61    minimax.displa
+00000fd0: 7928 7072 6f66 290a 2020 2020 2020 2020  y(prof).        
+00000fe0: 7072 696e 7428 6d69 6e69 6d61 785f 7363  print(minimax_sc
+00000ff0: 6f72 6573 2870 726f 6629 290a 0a0a 2020  ores(prof))...  
+00001000: 2020 2e2e 2065 7865 635f 636f 6465 3a3a    .. exec_code::
+00001010: 200a 2020 2020 2020 2020 3a68 6964 655f   .        :hide_
+00001020: 636f 6465 3a0a 0a20 2020 2020 2020 2066  code:..        f
+00001030: 726f 6d20 7072 6566 5f76 6f74 696e 672e  rom pref_voting.
+00001040: 7072 6f66 696c 6573 2069 6d70 6f72 7420  profiles import 
+00001050: 5072 6f66 696c 650a 2020 2020 2020 2020  Profile.        
+00001060: 6672 6f6d 2070 7265 665f 766f 7469 6e67  from pref_voting
+00001070: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
+00001080: 7468 6f64 7320 696d 706f 7274 206d 696e  thods import min
+00001090: 696d 6178 2c20 6d69 6e69 6d61 785f 7363  imax, minimax_sc
+000010a0: 6f72 6573 0a20 2020 2020 2020 200a 2020  ores.        .  
+000010b0: 2020 2020 2020 7072 6f66 203d 2050 726f        prof = Pro
+000010c0: 6669 6c65 285b 5b33 2c20 302c 2031 2c20  file([[3, 0, 1, 
+000010d0: 325d 2c20 5b31 2c20 332c 2032 2c20 305d  2], [1, 3, 2, 0]
+000010e0: 2c20 5b31 2c20 332c 2030 2c20 325d 2c20  , [1, 3, 0, 2], 
+000010f0: 5b31 2c20 322c 2030 2c20 335d 2c20 5b33  [1, 2, 0, 3], [3
+00001100: 2c20 322c 2030 2c20 315d 2c20 5b30 2c20  , 2, 0, 1], [0, 
+00001110: 322c 2031 2c20 335d 5d2c 205b 312c 2031  2, 1, 3]], [1, 1
+00001120: 2c20 312c 2031 2c20 322c 2031 5d29 0a0a  , 1, 1, 2, 1])..
+00001130: 2020 2020 2020 2020 6d69 6e69 6d61 782e          minimax.
+00001140: 6469 7370 6c61 7928 7072 6f66 290a 2020  display(prof).  
+00001150: 2020 2020 2020 7072 696e 7428 6d69 6e69        print(mini
+00001160: 6d61 785f 7363 6f72 6573 2870 726f 6629  max_scores(prof)
+00001170: 290a 0a20 2020 2022 2222 0a20 2020 200a  )..    """.    .
+00001180: 2020 2020 6361 6e64 6964 6174 6573 203d      candidates =
+00001190: 2065 6461 7461 2e63 616e 6469 6461 7465   edata.candidate
+000011a0: 7320 6966 2063 7572 725f 6361 6e64 7320  s if curr_cands 
+000011b0: 6973 204e 6f6e 6520 656c 7365 2063 7572  is None else cur
+000011c0: 725f 6361 6e64 730a 0a20 2020 2069 6620  r_cands..    if 
+000011d0: 6c65 6e28 6361 6e64 6964 6174 6573 2920  len(candidates) 
+000011e0: 3d3d 2031 3a0a 2020 2020 2020 2020 7265  == 1:.        re
+000011f0: 7475 726e 207b 633a 2030 2066 6f72 2063  turn {c: 0 for c
+00001200: 2069 6e20 6361 6e64 6964 6174 6573 7d0a   in candidates}.
+00001210: 2020 2020 0a20 2020 2023 2074 6865 7265      .    # there
+00001220: 2061 7265 2064 6966 6665 7265 6e74 2073   are different s
+00001230: 636f 7269 6e67 2066 756e 6374 696f 6e73  coring functions
+00001240: 2074 6861 7420 6361 6e20 6265 2075 7365   that can be use
+00001250: 6420 746f 206d 6561 7375 7265 2074 6865  d to measure the
+00001260: 2077 6f72 7365 206c 6f73 7320 666f 7220   worse loss for 
+00001270: 6561 6368 200a 2020 2020 2320 6361 6e64  each .    # cand
+00001280: 6964 6174 652e 2054 6865 7365 2061 6c6c  idate. These all
+00001290: 2070 726f 6475 6365 2074 6865 2073 616d   produce the sam
+000012a0: 6520 7365 7420 6f66 2077 696e 6e65 7273  e set of winners
+000012b0: 2077 6865 6e20 766f 7465 7273 2073 7562   when voters sub
+000012c0: 6d69 7420 6c69 6e65 6172 206f 7264 6572  mit linear order
+000012d0: 732e 200a 2020 2020 7363 6f72 655f 6675  s. .    score_fu
+000012e0: 6e63 7469 6f6e 7320 3d20 7b0a 2020 2020  nctions = {.    
+000012f0: 2020 2020 2277 696e 6e69 6e67 223a 206c      "winning": l
+00001300: 616d 6264 6120 6373 2c20 633a 206d 6178  ambda cs, c: max
+00001310: 285b 6564 6174 612e 7375 7070 6f72 7428  ([edata.support(
+00001320: 5f63 2c63 2920 666f 7220 5f63 2069 6e20  _c,c) for _c in 
+00001330: 6373 5d29 2069 6620 6c65 6e28 6373 2920  cs]) if len(cs) 
+00001340: 3e20 3020 656c 7365 2030 2c0a 2020 2020  > 0 else 0,.    
+00001350: 2020 2020 226d 6172 6769 6e73 223a 206c      "margins": l
+00001360: 616d 6264 6120 6373 2c20 633a 206d 6178  ambda cs, c: max
+00001370: 285b 6564 6174 612e 6d61 7267 696e 285f  ([edata.margin(_
+00001380: 632c 6329 2066 6f72 205f 6320 696e 2063  c,c) for _c in c
+00001390: 735d 2920 6966 206c 656e 2863 7329 203e  s]) if len(cs) >
+000013a0: 2030 2065 6c73 6520 302c 0a20 2020 2020   0 else 0,.     
+000013b0: 2020 2022 7061 6972 7769 7365 5f6f 7070     "pairwise_opp
+000013c0: 6f73 6974 696f 6e22 3a20 6c61 6d62 6461  osition": lambda
+000013d0: 2063 732c 2063 3a20 6d61 7828 5b65 6461   cs, c: max([eda
+000013e0: 7461 2e73 7570 706f 7274 285f 632c 6329  ta.support(_c,c)
+000013f0: 2066 6f72 205f 6320 696e 2063 735d 290a   for _c in cs]).
+00001400: 2020 2020 7d20 0a20 2020 200a 2020 2020      } .    .    
+00001410: 6361 6e64 7320 3d20 7b0a 2020 2020 2020  cands = {.      
+00001420: 2020 2277 696e 6e69 6e67 223a 206c 616d    "winning": lam
+00001430: 6264 6120 633a 2065 6461 7461 2e64 6f6d  bda c: edata.dom
+00001440: 696e 6174 6f72 7328 632c 2063 7572 725f  inators(c, curr_
+00001450: 6361 6e64 7320 3d20 6375 7272 5f63 616e  cands = curr_can
+00001460: 6473 292c 0a20 2020 2020 2020 2022 6d61  ds),.        "ma
+00001470: 7267 696e 7322 3a20 6c61 6d62 6461 2063  rgins": lambda c
+00001480: 3a20 6564 6174 612e 646f 6d69 6e61 746f  : edata.dominato
+00001490: 7273 2863 2c20 6375 7272 5f63 616e 6473  rs(c, curr_cands
+000014a0: 203d 2063 7572 725f 6361 6e64 7329 2c0a   = curr_cands),.
+000014b0: 2020 2020 2020 2020 2270 6169 7277 6973          "pairwis
+000014c0: 655f 6f70 706f 7369 7469 6f6e 223a 206c  e_opposition": l
+000014d0: 616d 6264 6120 633a 205b 5f63 2066 6f72  ambda c: [_c for
+000014e0: 205f 6320 696e 2063 616e 6469 6461 7465   _c in candidate
+000014f0: 7320 6966 205f 6320 213d 2063 5d0a 2020  s if _c != c].  
+00001500: 2020 7d20 0a0a 2020 2020 7265 7475 726e    } ..    return
+00001510: 207b 633a 202d 3120 2a20 7363 6f72 655f   {c: -1 * score_
+00001520: 6675 6e63 7469 6f6e 735b 7363 6f72 655f  functions[score_
+00001530: 6d65 7468 6f64 5d28 6361 6e64 735b 7363  method](cands[sc
+00001540: 6f72 655f 6d65 7468 6f64 5d28 6329 2c20  ore_method](c), 
+00001550: 6329 2066 6f72 2063 2069 6e20 6361 6e64  c) for c in cand
+00001560: 6964 6174 6573 7d0a 0a0a 6465 6620 6d61  idates}...def ma
+00001570: 7869 6d61 6c5f 656c 656d 656e 7473 2867  ximal_elements(g
+00001580: 293a 200a 2020 2020 2222 2272 6574 7572  ): .    """retur
+00001590: 6e20 7468 6520 6e6f 6465 7320 696e 2067  n the nodes in g
+000015a0: 2077 6974 6820 6e6f 2069 6e63 6f6d 696e   with no incomin
+000015b0: 6720 6172 726f 7773 2e22 2222 0a20 2020  g arrows.""".   
+000015c0: 2072 6574 7572 6e20 5b6e 2066 6f72 206e   return [n for n
+000015d0: 2069 6e20 672e 6e6f 6465 7320 6966 2067   in g.nodes if g
+000015e0: 2e69 6e5f 6465 6772 6565 286e 2920 3d3d  .in_degree(n) ==
+000015f0: 2030 5d0a 0a0a 6465 6620 5f62 6561 745f   0]...def _beat_
+00001600: 7061 7468 5f62 6173 6963 2865 6461 7461  path_basic(edata
+00001610: 2c20 0a20 2020 2020 2020 2020 2020 2020  , .             
+00001620: 2020 2020 2020 2020 6375 7272 5f63 616e          curr_can
+00001630: 6473 203d 204e 6f6e 652c 200a 2020 2020  ds = None, .    
+00001640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001650: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+00001660: 6f6e 203d 204e 6f6e 6529 3a20 0a20 2020  on = None): .   
+00001670: 2022 2222 416e 2069 6d70 6c65 6d65 6e74   """An implement
+00001680: 6174 696f 6e20 6f66 2074 6865 2042 6561  ation of the Bea
+00001690: 7420 5061 7468 206d 6574 686f 6420 7468  t Path method th
+000016a0: 6174 2075 7365 7320 6120 6261 7369 6320  at uses a basic 
+000016b0: 616c 676f 7269 7468 6d2e 2020 5468 6973  algorithm.  This
+000016c0: 2069 7320 6e6f 7420 6566 6669 6369 656e   is not efficien
+000016d0: 7420 666f 7220 6c61 7267 6520 6772 6170  t for large grap
+000016e0: 6873 2e0a 2020 2020 0a20 2020 2041 7267  hs..    .    Arg
+000016f0: 733a 0a20 2020 2020 2020 2065 6461 7461  s:.        edata
+00001700: 2028 5072 6f66 696c 652c 2050 726f 6669   (Profile, Profi
+00001710: 6c65 5769 7468 5469 6573 2c20 4d61 7267  leWithTies, Marg
+00001720: 696e 4772 6170 6829 3a20 416e 7920 656c  inGraph): Any el
+00001730: 6563 7469 6f6e 2064 6174 6120 7468 6174  ection data that
+00001740: 2068 6173 2061 2060 6d61 7267 696e 6020   has a `margin` 
+00001750: 6d65 7468 6f64 2e20 0a20 2020 2020 2020  method. .       
+00001760: 2063 7572 725f 6361 6e64 7320 284c 6973   curr_cands (Lis
+00001770: 745b 696e 745d 2c20 6f70 7469 6f6e 616c  t[int], optional
+00001780: 293a 2049 6620 7365 742c 2074 6865 6e20  ): If set, then 
+00001790: 6669 6e64 2074 6865 2077 696e 6e65 7273  find the winners
+000017a0: 2066 6f72 2074 6865 2070 726f 6669 6c65   for the profile
+000017b0: 2072 6573 7472 6963 7465 6420 746f 2074   restricted to t
+000017c0: 6865 2063 616e 6469 6461 7465 7320 696e  he candidates in
+000017d0: 2060 6063 7572 725f 6361 6e64 7360 600a   ``curr_cands``.
+000017e0: 2020 2020 2020 2020 7374 7265 6e67 7468          strength
+000017f0: 5f66 756e 6374 696f 6e20 2866 756e 6374  _function (funct
+00001800: 696f 6e2c 206f 7074 696f 6e61 6c29 3a20  ion, optional): 
+00001810: 5468 6520 7374 7265 6e67 7468 2066 756e  The strength fun
+00001820: 6374 696f 6e20 746f 2062 6520 7573 6564  ction to be used
+00001830: 2074 6f20 6361 6c63 756c 6174 6520 7468   to calculate th
+00001840: 6520 7374 7265 6e67 7468 206f 6620 6120  e strength of a 
+00001850: 7061 7468 2e20 2020 5468 6520 6465 6661  path.   The defa
+00001860: 756c 7420 6973 2074 6865 206d 6172 6769  ult is the margi
+00001870: 6e20 6d65 7468 6f64 206f 6620 6060 6564  n method of ``ed
+00001880: 6174 6160 602e 2020 2054 6869 7320 6f6e  ata``.   This on
+00001890: 6c79 206d 6174 7465 7273 2077 6865 6e20  ly matters when 
+000018a0: 7468 6520 6261 6c6c 6f74 7320 6172 6520  the ballots are 
+000018b0: 6e6f 7420 6c69 6e65 6172 206f 7264 6572  not linear order
+000018c0: 732e 200a 0a20 2020 2052 6574 7572 6e73  s. ..    Returns
+000018d0: 3a20 0a20 2020 2020 2020 2041 2073 6f72  : .        A sor
+000018e0: 7465 6420 6c69 7374 206f 6620 6361 6e64  ted list of cand
+000018f0: 6964 6174 6573 2e20 0a0a 2020 2020 2222  idates. ..    ""
+00001900: 220a 2020 2020 0a20 2020 2063 616e 6469  ".    .    candi
+00001910: 6461 7465 7320 3d20 6564 6174 612e 6361  dates = edata.ca
+00001920: 6e64 6964 6174 6573 2069 6620 6375 7272  ndidates if curr
+00001930: 5f63 616e 6473 2069 7320 4e6f 6e65 2065  _cands is None e
+00001940: 6c73 6520 6375 7272 5f63 616e 6473 2020  lse curr_cands  
+00001950: 2020 0a20 2020 2073 7472 656e 6774 685f    .    strength_
+00001960: 6675 6e63 7469 6f6e 203d 2065 6461 7461  function = edata
+00001970: 2e6d 6172 6769 6e20 6966 2073 7472 656e  .margin if stren
+00001980: 6774 685f 6675 6e63 7469 6f6e 2069 7320  gth_function is 
+00001990: 4e6f 6e65 2065 6c73 6520 7374 7265 6e67  None else streng
+000019a0: 7468 5f66 756e 6374 696f 6e0a 2020 2020  th_function.    
+000019b0: 0a20 2020 206d 6720 3d20 6765 745f 6d67  .    mg = get_mg
+000019c0: 2865 6461 7461 2c20 6375 7272 5f63 616e  (edata, curr_can
+000019d0: 6473 203d 2063 7572 725f 6361 6e64 7329  ds = curr_cands)
+000019e0: 0a20 2020 200a 2020 2020 6265 6174 5f70  .    .    beat_p
+000019f0: 6174 6873 5f77 6569 6768 7473 203d 207b  aths_weights = {
+00001a00: 633a 207b 6332 3a30 2066 6f72 2063 3220  c: {c2:0 for c2 
+00001a10: 696e 2063 616e 6469 6461 7465 7320 6966  in candidates if
+00001a20: 2063 3220 213d 2063 7d20 666f 7220 6320   c2 != c} for c 
+00001a30: 696e 2063 616e 6469 6461 7465 737d 0a20  in candidates}. 
+00001a40: 2020 2066 6f72 2063 2069 6e20 6361 6e64     for c in cand
+00001a50: 6964 6174 6573 3a20 0a20 2020 2020 2020  idates: .       
+00001a60: 2066 6f72 206f 7468 6572 5f63 2069 6e20   for other_c in 
+00001a70: 6265 6174 5f70 6174 6873 5f77 6569 6768  beat_paths_weigh
+00001a80: 7473 5b63 5d2e 6b65 7973 2829 3a0a 2020  ts[c].keys():.  
+00001a90: 2020 2020 2020 2020 2020 616c 6c5f 7061            all_pa
+00001aa0: 7468 7320 3d20 206c 6973 7428 6e78 2e61  ths =  list(nx.a
+00001ab0: 6c6c 5f73 696d 706c 655f 7061 7468 7328  ll_simple_paths(
+00001ac0: 6d67 2c20 632c 206f 7468 6572 5f63 2929  mg, c, other_c))
+00001ad0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00001ae0: 6c65 6e28 616c 6c5f 7061 7468 7329 203e  len(all_paths) >
+00001af0: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+00001b00: 2020 2020 6265 6174 5f70 6174 6873 5f77      beat_paths_w
+00001b10: 6569 6768 7473 5b63 5d5b 6f74 6865 725f  eights[c][other_
+00001b20: 635d 203d 206d 6178 285b 6d69 6e28 5b73  c] = max([min([s
+00001b30: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+00001b40: 2870 5b69 5d2c 2070 5b69 2b31 5d29 200a  (p[i], p[i+1]) .
+00001b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b60: 666f 7220 6920 696e 2072 616e 6765 2830  for i in range(0
+00001b70: 2c6c 656e 2870 292d 3129 5d29 200a 2020  ,len(p)-1)]) .  
+00001b80: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00001b90: 7220 7020 696e 2061 6c6c 5f70 6174 6873  r p in all_paths
+00001ba0: 5d29 0a20 2020 200a 2020 2020 7769 6e6e  ]).    .    winn
+00001bb0: 6572 7320 3d20 6c69 7374 2829 0a20 2020  ers = list().   
+00001bc0: 2066 6f72 2063 2069 6e20 6361 6e64 6964   for c in candid
+00001bd0: 6174 6573 3a20 0a20 2020 2020 2020 2069  ates: .        i
+00001be0: 6620 616c 6c28 5b62 6561 745f 7061 7468  f all([beat_path
+00001bf0: 735f 7765 6967 6874 735b 635d 5b63 325d  s_weights[c][c2]
+00001c00: 203e 3d20 6265 6174 5f70 6174 6873 5f77   >= beat_paths_w
+00001c10: 6569 6768 7473 5b63 325d 5b63 5d20 666f  eights[c2][c] fo
+00001c20: 7220 6332 2069 6e20 6361 6e64 6964 6174  r c2 in candidat
+00001c30: 6573 2020 6966 2063 3220 213d 2063 5d29  es  if c2 != c])
+00001c40: 3a0a 2020 2020 2020 2020 2020 2020 7769  :.            wi
+00001c50: 6e6e 6572 732e 6170 7065 6e64 2863 290a  nners.append(c).
+00001c60: 2020 2020 7265 7475 726e 2073 6f72 7465      return sorte
+00001c70: 6428 6c69 7374 2877 696e 6e65 7273 2929  d(list(winners))
+00001c80: 0a0a 0a64 6566 205f 6265 6174 5f70 6174  ...def _beat_pat
+00001c90: 685f 666c 6f79 645f 7761 7273 6861 6c6c  h_floyd_warshall
+00001ca0: 280a 2020 2020 2020 2020 6564 6174 612c  (.        edata,
+00001cb0: 200a 2020 2020 2020 2020 6375 7272 5f63   .        curr_c
+00001cc0: 616e 6473 203d 204e 6f6e 652c 200a 2020  ands = None, .  
+00001cd0: 2020 2020 2020 7374 7265 6e67 7468 5f66        strength_f
+00001ce0: 756e 6374 696f 6e20 3d20 4e6f 6e65 293a  unction = None):
+00001cf0: 2020 200a 2020 2020 2222 2241 6e20 696d     .    """An im
+00001d00: 706c 656d 656e 7461 7469 6f6e 206f 6620  plementation of 
+00001d10: 4265 6174 2050 6174 6820 7573 696e 6720  Beat Path using 
+00001d20: 6120 7661 7269 6174 696f 6e20 6f66 2074  a variation of t
+00001d30: 6865 2046 6c6f 7964 2d57 6172 7368 616c  he Floyd-Warshal
+00001d40: 6c20 416c 676f 7269 7468 6d0a 2020 2020  l Algorithm.    
+00001d50: 5365 6520 6874 7470 733a 2f2f 656e 2e77  See https://en.w
+00001d60: 696b 6970 6564 6961 2e6f 7267 2f77 696b  ikipedia.org/wik
+00001d70: 692f 5363 6875 6c7a 655f 6d65 7468 6f64  i/Schulze_method
+00001d80: 2349 6d70 6c65 6d65 6e74 6174 696f 6e29  #Implementation)
+00001d90: 0a20 0a20 2020 2041 7267 733a 0a20 2020  . .    Args:.   
+00001da0: 2020 2020 2065 6461 7461 2028 5072 6f66       edata (Prof
+00001db0: 696c 652c 2050 726f 6669 6c65 5769 7468  ile, ProfileWith
+00001dc0: 5469 6573 2c20 4d61 7267 696e 4772 6170  Ties, MarginGrap
+00001dd0: 6829 3a20 416e 7920 656c 6563 7469 6f6e  h): Any election
+00001de0: 2064 6174 6120 7468 6174 2068 6173 2061   data that has a
+00001df0: 2060 6d61 7267 696e 6020 6d65 7468 6f64   `margin` method
+00001e00: 2e20 0a20 2020 2020 2020 2063 7572 725f  . .        curr_
+00001e10: 6361 6e64 7320 284c 6973 745b 696e 745d  cands (List[int]
+00001e20: 2c20 6f70 7469 6f6e 616c 293a 2049 6620  , optional): If 
+00001e30: 7365 742c 2074 6865 6e20 6669 6e64 2074  set, then find t
+00001e40: 6865 2077 696e 6e65 7273 2066 6f72 2074  he winners for t
+00001e50: 6865 2070 726f 6669 6c65 2072 6573 7472  he profile restr
+00001e60: 6963 7465 6420 746f 2074 6865 2063 616e  icted to the can
+00001e70: 6469 6461 7465 7320 696e 2060 6063 7572  didates in ``cur
+00001e80: 725f 6361 6e64 7360 600a 2020 2020 2020  r_cands``.      
 00001e90: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
-00001ea0: 696f 6e20 3d20 6564 6174 612e 6d61 7267  ion = edata.marg
-00001eb0: 696e 2069 6620 7374 7265 6e67 7468 5f66  in if strength_f
-00001ec0: 756e 6374 696f 6e20 6973 204e 6f6e 6520  unction is None 
-00001ed0: 656c 7365 2073 7472 656e 6774 685f 6675  else strength_fu
-00001ee0: 6e63 7469 6f6e 0a20 2020 2020 2020 200a  nction.        .
-00001ef0: 2020 2020 735f 6d61 7472 6978 203d 205b      s_matrix = [
-00001f00: 5b2d 6e70 2e69 6e66 2066 6f72 205f 2069  [-np.inf for _ i
-00001f10: 6e20 6361 6e64 6964 6174 6573 5d20 666f  n candidates] fo
-00001f20: 7220 5f20 696e 2063 616e 6469 6461 7465  r _ in candidate
-00001f30: 735d 0a20 2020 2066 6f72 2063 315f 6964  s].    for c1_id
-00001f40: 782c 2063 3120 696e 2065 6e75 6d65 7261  x, c1 in enumera
-00001f50: 7465 2863 616e 6469 6461 7465 7329 3a0a  te(candidates):.
-00001f60: 2020 2020 2020 2020 666f 7220 6332 5f69          for c2_i
-00001f70: 6478 2c20 6332 2069 6e20 656e 756d 6572  dx, c2 in enumer
-00001f80: 6174 6528 6361 6e64 6964 6174 6573 293a  ate(candidates):
-00001f90: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00001fa0: 2865 6461 7461 2e6d 616a 6f72 6974 795f  (edata.majority_
-00001fb0: 7072 6566 6572 7328 6331 2c20 6332 2920  prefers(c1, c2) 
-00001fc0: 6f72 2063 3120 3d3d 2063 3229 3a0a 2020  or c1 == c2):.  
-00001fd0: 2020 2020 2020 2020 2020 2020 2020 735f                s_
-00001fe0: 6d61 7472 6978 5b63 315f 6964 785d 5b63  matrix[c1_idx][c
-00001ff0: 325f 6964 785d 203d 2073 7472 656e 6774  2_idx] = strengt
-00002000: 685f 6675 6e63 7469 6f6e 2863 312c 2063  h_function(c1, c
-00002010: 3229 200a 2020 2020 7374 7265 6e67 7468  2) .    strength
-00002020: 203d 206c 6973 7428 6d61 7028 6c61 6d62   = list(map(lamb
-00002030: 6461 2069 203a 206c 6973 7428 6d61 7028  da i : list(map(
-00002040: 6c61 6d62 6461 206a 203a 206a 202c 2069  lambda j : j , i
-00002050: 2929 202c 2073 5f6d 6174 7269 7829 290a  )) , s_matrix)).
-00002060: 2020 2020 666f 7220 695f 6964 782c 2069      for i_idx, i
-00002070: 2069 6e20 656e 756d 6572 6174 6528 6361   in enumerate(ca
-00002080: 6e64 6964 6174 6573 293a 2020 2020 2020  ndidates):      
-00002090: 2020 200a 2020 2020 2020 2020 666f 7220     .        for 
-000020a0: 6a5f 6964 782c 206a 2069 6e20 656e 756d  j_idx, j in enum
-000020b0: 6572 6174 6528 6361 6e64 6964 6174 6573  erate(candidates
-000020c0: 293a 200a 2020 2020 2020 2020 2020 2020  ): .            
-000020d0: 6966 2069 213d 206a 3a0a 2020 2020 2020  if i!= j:.      
-000020e0: 2020 2020 2020 2020 2020 666f 7220 6b5f            for k_
-000020f0: 6964 782c 206b 2069 6e20 656e 756d 6572  idx, k in enumer
-00002100: 6174 6528 6361 6e64 6964 6174 6573 293a  ate(candidates):
-00002110: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-00002120: 2020 2020 2020 6966 2069 213d 206b 2061        if i!= k a
-00002130: 6e64 206a 2021 3d20 6b3a 0a20 2020 2020  nd j != k:.     
-00002140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002150: 2020 2073 7472 656e 6774 685b 6a5f 6964     strength[j_id
-00002160: 785d 5b6b 5f69 6478 5d20 3d20 6d61 7828  x][k_idx] = max(
-00002170: 7374 7265 6e67 7468 5b6a 5f69 6478 5d5b  strength[j_idx][
-00002180: 6b5f 6964 785d 2c20 6d69 6e28 7374 7265  k_idx], min(stre
-00002190: 6e67 7468 5b6a 5f69 6478 5d5b 695f 6964  ngth[j_idx][i_id
-000021a0: 785d 2c73 7472 656e 6774 685b 695f 6964  x],strength[i_id
-000021b0: 785d 5b6b 5f69 6478 5d29 290a 2020 2020  x][k_idx])).    
-000021c0: 7769 6e6e 6572 7320 3d20 7b69 3a54 7275  winners = {i:Tru
-000021d0: 6520 666f 7220 6920 696e 2063 616e 6469  e for i in candi
-000021e0: 6461 7465 737d 0a20 2020 2066 6f72 2069  dates}.    for i
-000021f0: 5f69 6478 2c20 6920 696e 2065 6e75 6d65  _idx, i in enume
-00002200: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
-00002210: 3a20 0a20 2020 2020 2020 2066 6f72 206a  : .        for j
-00002220: 5f69 6478 2c20 6a20 696e 2065 6e75 6d65  _idx, j in enume
-00002230: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
-00002240: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00002250: 2069 213d 6a3a 0a20 2020 2020 2020 2020   i!=j:.         
-00002260: 2020 2020 2020 2069 6620 7374 7265 6e67         if streng
-00002270: 7468 5b6a 5f69 6478 5d5b 695f 6964 785d  th[j_idx][i_idx]
-00002280: 203e 2073 7472 656e 6774 685b 695f 6964   > strength[i_id
-00002290: 785d 5b6a 5f69 6478 5d3a 0a20 2020 2020  x][j_idx]:.     
-000022a0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-000022b0: 696e 6e65 7273 5b69 5d20 3d20 4661 6c73  inners[i] = Fals
-000022c0: 650a 2020 2020 7265 7475 726e 2073 6f72  e.    return sor
-000022d0: 7465 6428 5b63 2066 6f72 2063 2069 6e20  ted([c for c in 
-000022e0: 6361 6e64 6964 6174 6573 2069 6620 7769  candidates if wi
-000022f0: 6e6e 6572 735b 635d 5d29 0a0a 4076 6d28  nners[c]])..@vm(
-00002300: 6e61 6d65 3d22 4265 6174 2050 6174 6822  name="Beat Path"
-00002310: 290a 6465 6620 6265 6174 5f70 6174 6828  ).def beat_path(
-00002320: 0a20 2020 2065 6461 7461 2c20 0a20 2020  .    edata, .   
-00002330: 2063 7572 725f 6361 6e64 7320 3d20 4e6f   curr_cands = No
-00002340: 6e65 2c20 0a20 2020 2073 7472 656e 6774  ne, .    strengt
-00002350: 685f 6675 6e63 7469 6f6e 203d 204e 6f6e  h_function = Non
-00002360: 652c 200a 2020 2020 616c 676f 7269 7468  e, .    algorith
-00002370: 6d20 3d20 2766 6c6f 7964 5f77 6172 7368  m = 'floyd_warsh
-00002380: 616c 6c27 293a 2020 0a0a 2020 2020 2222  all'):  ..    ""
-00002390: 2246 6f72 2063 616e 6469 6461 7465 7320  "For candidates 
-000023a0: 3a6d 6174 683a 6061 6020 616e 6420 3a6d  :math:`a` and :m
-000023b0: 6174 683a 6062 602c 2061 202a 2a70 6174  ath:`b`, a **pat
-000023c0: 682a 2a20 6672 6f6d 203a 6d61 7468 3a60  h** from :math:`
-000023d0: 6160 2074 6f20 3a6d 6174 683a 6062 6020  a` to :math:`b` 
-000023e0: 6973 2061 2073 6571 7565 6e63 6520 0a20  is a sequence . 
-000023f0: 2020 203a 6d61 7468 3a60 785f 312c 205c     :math:`x_1, \
-00002400: 6c64 6f74 732c 2078 5f6e 6020 6f66 2064  ldots, x_n` of d
-00002410: 6973 7469 6e63 7420 6361 6e64 6964 6174  istinct candidat
-00002420: 6573 2020 7769 7468 2020 3a6d 6174 683a  es  with  :math:
-00002430: 6078 5f31 3d61 6020 616e 6420 3a6d 6174  `x_1=a` and :mat
-00002440: 683a 6078 5f6e 3d62 6020 7375 6368 2074  h:`x_n=b` such t
-00002450: 6861 7420 0a20 2020 2066 6f72 203a 6d61  hat .    for :ma
-00002460: 7468 3a60 315c 6c65 7120 6b5c 6c65 7120  th:`1\leq k\leq 
-00002470: 6e2d 3160 2c20 3a6d 6174 683a 6078 5f6b  n-1`, :math:`x_k
-00002480: 6020 6973 206d 616a 6f72 6974 7920 7072  ` is majority pr
-00002490: 6566 6572 7265 6420 746f 203a 6d61 7468  eferred to :math
-000024a0: 3a60 785f 7b6b 2b31 7d60 2e20 2054 6865  :`x_{k+1}`.  The
-000024b0: 202a 2a73 7472 656e 6774 6820 6f66 2061   **strength of a
-000024c0: 2070 6174 682a 2a0a 2020 2020 6973 2074   path**.    is t
-000024d0: 6865 206d 696e 696d 616c 206d 6172 6769  he minimal margi
-000024e0: 6e20 616c 6f6e 6720 7468 6174 2070 6174  n along that pat
-000024f0: 682e 2020 5361 7920 7468 6174 203a 6d61  h.  Say that :ma
-00002500: 7468 3a60 6160 2064 6566 6561 7473 203a  th:`a` defeats :
-00002510: 6d61 7468 3a60 6260 2061 6363 6f72 6469  math:`b` accordi
-00002520: 6e67 2074 6f20 4265 6174 2050 6174 6820  ng to Beat Path 
-00002530: 6966 2074 6865 2074 6865 2073 7472 656e  if the the stren
-00002540: 6774 6820 6f66 2074 6865 2073 7472 6f6e  gth of the stron
-00002550: 6765 7374 2070 6174 6820 6672 6f6d 203a  gest path from :
-00002560: 6d61 7468 3a60 6160 2074 6f20 3a6d 6174  math:`a` to :mat
-00002570: 683a 6062 6020 6973 2067 7265 6174 6572  h:`b` is greater
-00002580: 2074 6861 6e20 7468 6520 7374 7265 6e67   than the streng
-00002590: 7468 206f 6620 7468 6520 7374 726f 6e67  th of the strong
-000025a0: 6573 7420 7061 7468 2066 726f 6d20 3a6d  est path from :m
-000025b0: 6174 683a 6062 6020 746f 203a 6d61 7468  ath:`b` to :math
-000025c0: 3a60 6160 2e20 5468 656e 2c20 7468 6520  :`a`. Then, the 
-000025d0: 6361 6e64 6964 6174 6573 2074 6861 7420  candidates that 
-000025e0: 6172 6520 756e 6465 6665 6174 6564 2061  are undefeated a
-000025f0: 6363 6f72 6469 6e67 2074 6f20 4265 6174  ccording to Beat
-00002600: 2050 6174 6820 6172 6520 7468 6520 7769   Path are the wi
-00002610: 6e6e 6572 732e 2020 416c 736f 206b 6e6f  nners.  Also kno
-00002620: 776e 2061 7320 7468 6520 5363 6875 6c7a  wn as the Schulz
-00002630: 6520 5275 6c65 2e20 0a0a 2020 2020 4172  e Rule. ..    Ar
-00002640: 6773 3a0a 2020 2020 2020 2020 6564 6174  gs:.        edat
-00002650: 6120 2850 726f 6669 6c65 2c20 5072 6f66  a (Profile, Prof
-00002660: 696c 6557 6974 6854 6965 732c 204d 6172  ileWithTies, Mar
-00002670: 6769 6e47 7261 7068 293a 2041 6e79 2065  ginGraph): Any e
-00002680: 6c65 6374 696f 6e20 6461 7461 2074 6861  lection data tha
-00002690: 7420 6861 7320 6120 606d 6172 6769 6e60  t has a `margin`
-000026a0: 206d 6574 686f 642e 200a 2020 2020 2020   method. .      
-000026b0: 2020 6375 7272 5f63 616e 6473 2028 4c69    curr_cands (Li
-000026c0: 7374 5b69 6e74 5d2c 206f 7074 696f 6e61  st[int], optiona
-000026d0: 6c29 3a20 4966 2073 6574 2c20 7468 656e  l): If set, then
-000026e0: 2066 696e 6420 7468 6520 7769 6e6e 6572   find the winner
-000026f0: 7320 666f 7220 7468 6520 7072 6f66 696c  s for the profil
-00002700: 6520 7265 7374 7269 6374 6564 2074 6f20  e restricted to 
-00002710: 7468 6520 6361 6e64 6964 6174 6573 2069  the candidates i
-00002720: 6e20 6060 6375 7272 5f63 616e 6473 6060  n ``curr_cands``
-00002730: 0a20 2020 2020 2020 2073 7472 656e 6774  .        strengt
-00002740: 685f 6675 6e63 7469 6f6e 2028 6675 6e63  h_function (func
-00002750: 7469 6f6e 2c20 6f70 7469 6f6e 616c 293a  tion, optional):
-00002760: 2054 6865 2073 7472 656e 6774 6820 6675   The strength fu
-00002770: 6e63 7469 6f6e 2074 6f20 6265 2075 7365  nction to be use
-00002780: 6420 746f 2063 616c 6375 6c61 7465 2074  d to calculate t
-00002790: 6865 2073 7472 656e 6774 6820 6f66 2061  he strength of a
-000027a0: 2070 6174 682e 2020 2054 6865 2064 6566   path.   The def
-000027b0: 6175 6c74 2069 7320 7468 6520 6d61 7267  ault is the marg
-000027c0: 696e 206d 6574 686f 6420 6f66 2060 6065  in method of ``e
-000027d0: 6461 7461 6060 2e20 2020 5468 6973 206f  data``.   This o
-000027e0: 6e6c 7920 6d61 7474 6572 7320 7768 656e  nly matters when
-000027f0: 2074 6865 2062 616c 6c6f 7473 2061 7265   the ballots are
-00002800: 206e 6f74 206c 696e 6561 7220 6f72 6465   not linear orde
-00002810: 7273 2e20 0a20 2020 2020 2020 2061 6c67  rs. .        alg
-00002820: 6f72 6974 686d 2028 7374 7229 3a20 5370  orithm (str): Sp
-00002830: 6563 6966 7920 7768 6963 6820 616c 676f  ecify which algo
-00002840: 7269 7468 6d20 746f 2075 7365 2e20 204f  rithm to use.  O
-00002850: 7074 696f 6e73 2061 7265 2027 666c 6f79  ptions are 'floy
-00002860: 645f 7761 7273 6861 6c6c 2720 2874 6865  d_warshall' (the
-00002870: 2064 6566 6175 6c74 2920 616e 6420 2762   default) and 'b
-00002880: 6173 6963 272e 0a0a 2020 2020 5265 7475  asic'...    Retu
-00002890: 726e 733a 200a 2020 2020 2020 2020 4120  rns: .        A 
-000028a0: 736f 7274 6564 206c 6973 7420 6f66 2063  sorted list of c
-000028b0: 616e 6469 6461 7465 732e 200a 0a20 2020  andidates. ..   
-000028c0: 202e 2e20 7365 6561 6c73 6f3a 3a0a 0a20   .. seealso::.. 
-000028d0: 2020 2020 2020 203a 6d65 7468 3a60 7072         :meth:`pr
-000028e0: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
-000028f0: 5f62 6173 6564 5f6d 6574 686f 6473 2e62  _based_methods.b
-00002900: 6561 745f 7061 7468 5f64 6566 6561 7460  eat_path_defeat`
-00002910: 0a0a 2020 2020 3a45 7861 6d70 6c65 3a20  ..    :Example: 
-00002920: 0a0a 2020 2020 2e2e 2070 6c6f 743a 3a20  ..    .. plot:: 
-00002930: 206d 6172 6769 6e5f 6772 6170 6873 5f65   margin_graphs_e
-00002940: 7861 6d70 6c65 732f 6d67 5f65 785f 6270  xamples/mg_ex_bp
-00002950: 5f72 702e 7079 0a20 2020 2020 2020 203a  _rp.py.        :
-00002960: 636f 6e74 6578 743a 2072 6573 6574 2020  context: reset  
-00002970: 0a20 2020 2020 2020 203a 696e 636c 7564  .        :includ
-00002980: 652d 736f 7572 6365 3a20 5472 7565 0a0a  e-source: True..
-00002990: 0a20 2020 202e 2e20 636f 6465 2d62 6c6f  .    .. code-blo
-000029a0: 636b 3a3a 200a 0a20 2020 2020 2020 2066  ck:: ..        f
-000029b0: 726f 6d20 7072 6566 5f76 6f74 696e 672e  rom pref_voting.
-000029c0: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
-000029d0: 686f 6473 2069 6d70 6f72 7420 6265 6174  hods import beat
-000029e0: 5f70 6174 680a 0a20 2020 2020 2020 2062  _path..        b
-000029f0: 6561 745f 7061 7468 2e64 6973 706c 6179  eat_path.display
-00002a00: 286d 6729 0a0a 0a20 2020 202e 2e20 6578  (mg)...    .. ex
-00002a10: 6563 5f63 6f64 653a 3a20 0a20 2020 2020  ec_code:: .     
-00002a20: 2020 203a 6869 6465 5f63 6f64 653a 0a0a     :hide_code:..
-00002a30: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
-00002a40: 665f 766f 7469 6e67 2e77 6569 6768 7465  f_voting.weighte
-00002a50: 645f 6d61 6a6f 7269 7479 5f67 7261 7068  d_majority_graph
-00002a60: 7320 696d 706f 7274 204d 6172 6769 6e47  s import MarginG
-00002a70: 7261 7068 0a20 2020 2020 2020 2066 726f  raph.        fro
-00002a80: 6d20 7072 6566 5f76 6f74 696e 672e 6d61  m pref_voting.ma
-00002a90: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
-00002aa0: 6473 2069 6d70 6f72 7420 6265 6174 5f70  ds import beat_p
-00002ab0: 6174 680a 2020 2020 2020 2020 0a20 2020  ath.        .   
-00002ac0: 2020 2020 206d 6720 3d20 4d61 7267 696e       mg = Margin
-00002ad0: 4772 6170 6828 5b30 2c20 312c 2032 2c20  Graph([0, 1, 2, 
-00002ae0: 335d 2c20 5b28 302c 2032 2c20 3329 2c20  3], [(0, 2, 3), 
-00002af0: 2831 2c20 302c 2035 292c 2028 322c 2031  (1, 0, 5), (2, 1
-00002b00: 2c20 3529 2c20 2832 2c20 332c 2031 292c  , 5), (2, 3, 1),
-00002b10: 2028 332c 2030 2c20 3329 2c20 2833 2c20   (3, 0, 3), (3, 
-00002b20: 312c 2031 295d 290a 2020 2020 2020 2020  1, 1)]).        
-00002b30: 0a20 2020 2020 2020 2062 6561 745f 7061  .        beat_pa
-00002b40: 7468 2e64 6973 706c 6179 286d 6729 0a20  th.display(mg). 
-00002b50: 2020 2020 2020 2062 6561 745f 7061 7468         beat_path
-00002b60: 2e64 6973 706c 6179 286d 672c 2061 6c67  .display(mg, alg
-00002b70: 6f72 6974 686d 3d27 666c 6f79 645f 7761  orithm='floyd_wa
-00002b80: 7273 6861 6c6c 2729 200a 2020 2020 2020  rshall') .      
-00002b90: 2020 6265 6174 5f70 6174 682e 6469 7370    beat_path.disp
-00002ba0: 6c61 7928 6d67 2c20 616c 676f 7269 7468  lay(mg, algorith
-00002bb0: 6d3d 2762 6173 6963 2729 0a20 2020 2022  m='basic').    "
-00002bc0: 2222 0a0a 2020 2020 6966 2061 6c67 6f72  ""..    if algor
-00002bd0: 6974 686d 203d 3d20 2766 6c6f 7964 5f77  ithm == 'floyd_w
-00002be0: 6172 7368 616c 6c27 3a0a 2020 2020 2020  arshall':.      
-00002bf0: 2020 7265 7475 726e 205f 6265 6174 5f70    return _beat_p
-00002c00: 6174 685f 666c 6f79 645f 7761 7273 6861  ath_floyd_warsha
-00002c10: 6c6c 2865 6461 7461 2c20 6375 7272 5f63  ll(edata, curr_c
-00002c20: 616e 6473 203d 2063 7572 725f 6361 6e64  ands = curr_cand
-00002c30: 732c 2073 7472 656e 6774 685f 6675 6e63  s, strength_func
-00002c40: 7469 6f6e 203d 2073 7472 656e 6774 685f  tion = strength_
-00002c50: 6675 6e63 7469 6f6e 290a 2020 2020 656c  function).    el
-00002c60: 6966 2061 6c67 6f72 6974 686d 203d 3d20  if algorithm == 
-00002c70: 2762 6173 6963 273a 0a20 2020 2020 2020  'basic':.       
-00002c80: 2072 6574 7572 6e20 5f62 6561 745f 7061   return _beat_pa
-00002c90: 7468 5f62 6173 6963 2865 6461 7461 2c20  th_basic(edata, 
-00002ca0: 6375 7272 5f63 616e 6473 203d 2063 7572  curr_cands = cur
-00002cb0: 725f 6361 6e64 732c 2073 7472 656e 6774  r_cands, strengt
-00002cc0: 685f 6675 6e63 7469 6f6e 203d 2073 7472  h_function = str
-00002cd0: 656e 6774 685f 6675 6e63 7469 6f6e 290a  ength_function).
-00002ce0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00002cf0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-00002d00: 6f72 2822 496e 7661 6c69 6420 616c 676f  or("Invalid algo
-00002d10: 7269 7468 6d20 7370 6563 6966 6965 642e  rithm specified.
-00002d20: 2229 0a0a 6465 6620 6265 6174 5f70 6174  ")..def beat_pat
-00002d30: 685f 6465 6665 6174 2865 6461 7461 2c20  h_defeat(edata, 
-00002d40: 6375 7272 5f63 616e 6473 203d 204e 6f6e  curr_cands = Non
-00002d50: 652c 2073 7472 656e 6774 685f 6675 6e63  e, strength_func
-00002d60: 7469 6f6e 203d 204e 6f6e 6529 3a20 2020  tion = None):   
-00002d70: 0a20 2020 2022 2222 5265 7475 726e 7320  .    """Returns 
-00002d80: 7468 6520 6465 6665 6174 2072 656c 6174  the defeat relat
-00002d90: 696f 6e20 666f 7220 4265 6174 2050 6174  ion for Beat Pat
-00002da0: 682e 200a 2020 2020 0a20 2020 2041 7267  h. .    .    Arg
-00002db0: 733a 0a20 2020 2020 2020 2065 6461 7461  s:.        edata
-00002dc0: 2028 5072 6f66 696c 652c 2050 726f 6669   (Profile, Profi
-00002dd0: 6c65 5769 7468 5469 6573 2c20 4d61 7267  leWithTies, Marg
-00002de0: 696e 4772 6170 6829 3a20 416e 7920 656c  inGraph): Any el
-00002df0: 6563 7469 6f6e 2064 6174 6120 7468 6174  ection data that
-00002e00: 2068 6173 2061 2060 6d61 7267 696e 6020   has a `margin` 
-00002e10: 6d65 7468 6f64 2e20 0a20 2020 2020 2020  method. .       
-00002e20: 2063 7572 725f 6361 6e64 7320 284c 6973   curr_cands (Lis
-00002e30: 745b 696e 745d 2c20 6f70 7469 6f6e 616c  t[int], optional
-00002e40: 293a 2049 6620 7365 742c 2074 6865 6e20  ): If set, then 
-00002e50: 6669 6e64 2074 6865 2077 696e 6e65 7273  find the winners
-00002e60: 2066 6f72 2074 6865 2070 726f 6669 6c65   for the profile
-00002e70: 2072 6573 7472 6963 7465 6420 746f 2074   restricted to t
-00002e80: 6865 2063 616e 6469 6461 7465 7320 696e  he candidates in
-00002e90: 2060 6063 7572 725f 6361 6e64 7360 600a   ``curr_cands``.
-00002ea0: 2020 2020 2020 2020 7374 7265 6e67 7468          strength
-00002eb0: 5f66 756e 6374 696f 6e20 2866 756e 6374  _function (funct
-00002ec0: 696f 6e2c 206f 7074 696f 6e61 6c29 3a20  ion, optional): 
-00002ed0: 5468 6520 7374 7265 6e67 7468 2066 756e  The strength fun
-00002ee0: 6374 696f 6e20 746f 2062 6520 7573 6564  ction to be used
-00002ef0: 2074 6f20 6361 6c63 756c 6174 6520 7468   to calculate th
-00002f00: 6520 7374 7265 6e67 7468 206f 6620 6120  e strength of a 
-00002f10: 7061 7468 2e20 2020 5468 6520 6465 6661  path.   The defa
-00002f20: 756c 7420 6973 2074 6865 206d 6172 6769  ult is the margi
-00002f30: 6e20 6d65 7468 6f64 206f 6620 6060 6564  n method of ``ed
-00002f40: 6174 6160 602e 2020 2054 6869 7320 6f6e  ata``.   This on
-00002f50: 6c79 206d 6174 7465 7273 2077 6865 6e20  ly matters when 
-00002f60: 7468 6520 6261 6c6c 6f74 7320 6172 6520  the ballots are 
-00002f70: 6e6f 7420 6c69 6e65 6172 206f 7264 6572  not linear order
-00002f80: 732e 200a 0a20 2020 2052 6574 7572 6e73  s. ..    Returns
-00002f90: 3a20 0a20 2020 2020 2020 2041 206e 6574  : .        A net
-00002fa0: 776f 726b 7820 4469 4772 6170 6820 7265  workx DiGraph re
-00002fb0: 7072 6573 656e 7469 6e67 2074 6865 2042  presenting the B
-00002fc0: 6561 7420 5061 7468 2064 6566 6561 7420  eat Path defeat 
-00002fd0: 7265 6c61 7469 6f6e 2e20 0a0a 2020 2020  relation. ..    
-00002fe0: 2e2e 2073 6565 616c 736f 3a3a 0a0a 2020  .. seealso::..  
-00002ff0: 2020 2020 2020 3a6d 6574 683a 6070 7265        :meth:`pre
-00003000: 665f 766f 7469 6e67 2e6d 6172 6769 6e5f  f_voting.margin_
-00003010: 6261 7365 645f 6d65 7468 6f64 732e 6265  based_methods.be
-00003020: 6174 5f70 6174 6860 2c20 3a6d 6574 683a  at_path`, :meth:
-00003030: 6070 7265 665f 766f 7469 6e67 2e6d 6172  `pref_voting.mar
-00003040: 6769 6e5f 6261 7365 645f 6d65 7468 6f64  gin_based_method
-00003050: 732e 6265 6174 5f70 6174 685f 466c 6f79  s.beat_path_Floy
-00003060: 645f 5761 7273 6861 6c6c 600a 0a20 2020  d_Warshall`..   
-00003070: 203a 4578 616d 706c 653a 200a 0a20 2020   :Example: ..   
-00003080: 202e 2e20 706c 6f74 3a3a 2020 6d61 7267   .. plot::  marg
-00003090: 696e 5f67 7261 7068 735f 6578 616d 706c  in_graphs_exampl
-000030a0: 6573 2f6d 675f 6578 5f62 705f 6465 6665  es/mg_ex_bp_defe
-000030b0: 6174 2e70 790a 2020 2020 2020 2020 3a63  at.py.        :c
-000030c0: 6f6e 7465 7874 3a20 7265 7365 7420 200a  ontext: reset  .
-000030d0: 2020 2020 2020 2020 3a69 6e63 6c75 6465          :include
-000030e0: 2d73 6f75 7263 653a 2054 7275 650a 0a20  -source: True.. 
-000030f0: 2020 2022 2222 0a0a 2020 2020 6361 6e64     """..    cand
-00003100: 6964 6174 6573 203d 2065 6461 7461 2e63  idates = edata.c
-00003110: 616e 6469 6461 7465 7320 6966 2063 7572  andidates if cur
-00003120: 725f 6361 6e64 7320 6973 204e 6f6e 6520  r_cands is None 
-00003130: 656c 7365 2063 7572 725f 6361 6e64 7320  else curr_cands 
-00003140: 2020 200a 2020 2020 7374 7265 6e67 7468     .    strength
-00003150: 5f66 756e 6374 696f 6e20 3d20 6564 6174  _function = edat
-00003160: 612e 6d61 7267 696e 2069 6620 7374 7265  a.margin if stre
-00003170: 6e67 7468 5f66 756e 6374 696f 6e20 6973  ngth_function is
-00003180: 204e 6f6e 6520 656c 7365 2073 7472 656e   None else stren
-00003190: 6774 685f 6675 6e63 7469 6f6e 0a20 2020  gth_function.   
-000031a0: 2020 2020 200a 2020 2020 735f 6d61 7472       .    s_matr
-000031b0: 6978 203d 205b 5b2d 6e70 2e69 6e66 2066  ix = [[-np.inf f
-000031c0: 6f72 205f 2069 6e20 6361 6e64 6964 6174  or _ in candidat
-000031d0: 6573 5d20 666f 7220 5f20 696e 2063 616e  es] for _ in can
-000031e0: 6469 6461 7465 735d 0a20 2020 2066 6f72  didates].    for
-000031f0: 2063 315f 6964 782c 2063 3120 696e 2065   c1_idx, c1 in e
-00003200: 6e75 6d65 7261 7465 2863 616e 6469 6461  numerate(candida
-00003210: 7465 7329 3a0a 2020 2020 2020 2020 666f  tes):.        fo
-00003220: 7220 6332 5f69 6478 2c20 6332 2069 6e20  r c2_idx, c2 in 
-00003230: 656e 756d 6572 6174 6528 6361 6e64 6964  enumerate(candid
-00003240: 6174 6573 293a 0a20 2020 2020 2020 2020  ates):.         
-00003250: 2020 2069 6620 2865 6461 7461 2e6d 616a     if (edata.maj
-00003260: 6f72 6974 795f 7072 6566 6572 7328 6331  ority_prefers(c1
-00003270: 2c20 6332 2920 6f72 2063 3120 3d3d 2063  , c2) or c1 == c
-00003280: 3229 3a0a 2020 2020 2020 2020 2020 2020  2):.            
-00003290: 2020 2020 735f 6d61 7472 6978 5b63 315f      s_matrix[c1_
-000032a0: 6964 785d 5b63 325f 6964 785d 203d 2073  idx][c2_idx] = s
-000032b0: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-000032c0: 2863 312c 2063 3229 200a 2020 2020 7374  (c1, c2) .    st
-000032d0: 7265 6e67 7468 203d 206c 6973 7428 6d61  rength = list(ma
-000032e0: 7028 6c61 6d62 6461 2069 203a 206c 6973  p(lambda i : lis
-000032f0: 7428 6d61 7028 6c61 6d62 6461 206a 203a  t(map(lambda j :
-00003300: 206a 202c 2069 2929 202c 2073 5f6d 6174   j , i)) , s_mat
-00003310: 7269 7829 290a 2020 2020 666f 7220 695f  rix)).    for i_
-00003320: 6964 782c 2069 2069 6e20 656e 756d 6572  idx, i in enumer
-00003330: 6174 6528 6361 6e64 6964 6174 6573 293a  ate(candidates):
-00003340: 2020 2020 2020 2020 200a 2020 2020 2020           .      
-00003350: 2020 666f 7220 6a5f 6964 782c 206a 2069    for j_idx, j i
-00003360: 6e20 656e 756d 6572 6174 6528 6361 6e64  n enumerate(cand
-00003370: 6964 6174 6573 293a 200a 2020 2020 2020  idates): .      
-00003380: 2020 2020 2020 6966 2069 213d 206a 3a0a        if i!= j:.
-00003390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033a0: 666f 7220 6b5f 6964 782c 206b 2069 6e20  for k_idx, k in 
-000033b0: 656e 756d 6572 6174 6528 6361 6e64 6964  enumerate(candid
-000033c0: 6174 6573 293a 200a 2020 2020 2020 2020  ates): .        
-000033d0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-000033e0: 213d 206b 2061 6e64 206a 2021 3d20 6b3a  != k and j != k:
-000033f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003400: 2020 2020 2020 2020 2073 7472 656e 6774           strengt
-00003410: 685b 6a5f 6964 785d 5b6b 5f69 6478 5d20  h[j_idx][k_idx] 
-00003420: 3d20 6d61 7828 7374 7265 6e67 7468 5b6a  = max(strength[j
-00003430: 5f69 6478 5d5b 6b5f 6964 785d 2c20 6d69  _idx][k_idx], mi
-00003440: 6e28 7374 7265 6e67 7468 5b6a 5f69 6478  n(strength[j_idx
-00003450: 5d5b 695f 6964 785d 2c73 7472 656e 6774  ][i_idx],strengt
-00003460: 685b 695f 6964 785d 5b6b 5f69 6478 5d29  h[i_idx][k_idx])
-00003470: 290a 0a20 2020 2064 6566 6561 745f 6772  )..    defeat_gr
-00003480: 6170 6820 3d20 6e78 2e44 6947 7261 7068  aph = nx.DiGraph
-00003490: 2829 0a20 2020 2064 6566 6561 745f 6772  ().    defeat_gr
-000034a0: 6170 682e 6164 645f 6e6f 6465 735f 6672  aph.add_nodes_fr
-000034b0: 6f6d 2863 616e 6469 6461 7465 7329 0a20  om(candidates). 
-000034c0: 2020 200a 2020 2020 666f 7220 695f 6964     .    for i_id
-000034d0: 782c 2069 2069 6e20 656e 756d 6572 6174  x, i in enumerat
-000034e0: 6528 6361 6e64 6964 6174 6573 293a 200a  e(candidates): .
-000034f0: 2020 2020 2020 2020 666f 7220 6a5f 6964          for j_id
-00003500: 782c 206a 2069 6e20 656e 756d 6572 6174  x, j in enumerat
-00003510: 6528 6361 6e64 6964 6174 6573 293a 0a20  e(candidates):. 
-00003520: 2020 2020 2020 2020 2020 2069 6620 6921             if i!
-00003530: 3d6a 3a0a 2020 2020 2020 2020 2020 2020  =j:.            
-00003540: 2020 2020 6966 2073 7472 656e 6774 685b      if strength[
-00003550: 6a5f 6964 785d 5b69 5f69 6478 5d20 3e20  j_idx][i_idx] > 
-00003560: 7374 7265 6e67 7468 5b69 5f69 6478 5d5b  strength[i_idx][
-00003570: 6a5f 6964 785d 3a0a 2020 2020 2020 2020  j_idx]:.        
-00003580: 2020 2020 2020 2020 2020 2020 6465 6665              defe
-00003590: 6174 5f67 7261 7068 2e61 6464 5f77 6569  at_graph.add_wei
-000035a0: 6768 7465 645f 6564 6765 735f 6672 6f6d  ghted_edges_from
-000035b0: 285b 286a 2c69 2c73 5f6d 6174 7269 785b  ([(j,i,s_matrix[
-000035c0: 6a5f 6964 785d 5b69 5f69 6478 5d29 5d29  j_idx][i_idx])])
-000035d0: 0a0a 2020 2020 7265 7475 726e 2064 6566  ..    return def
-000035e0: 6561 745f 6772 6170 680a 0a0a 0a64 6566  eat_graph....def
-000035f0: 2068 6173 5f73 7472 6f6e 675f 7061 7468   has_strong_path
-00003600: 2841 2c20 736f 7572 6365 2c20 7461 7267  (A, source, targ
-00003610: 6574 2c20 6b29 3a0a 2020 2020 2222 2247  et, k):.    """G
-00003620: 6976 656e 2061 2073 7175 6172 6520 6d61  iven a square ma
-00003630: 7472 6978 2041 2c20 7265 7475 726e 2054  trix A, return T
-00003640: 7275 6520 6966 2074 6865 7265 2069 7320  rue if there is 
-00003650: 6120 7061 7468 2066 726f 6d20 736f 7572  a path from sour
-00003660: 6365 2074 6f20 7461 7267 6574 2069 6e20  ce to target in 
-00003670: 7468 6520 6173 736f 6369 6174 6564 2064  the associated d
-00003680: 6972 6563 7465 6420 6772 6170 6820 2020  irected graph   
-00003690: 2020 7768 6572 6520 6561 6368 2065 6467    where each edg
-000036a0: 6520 6861 7320 6120 7765 6967 6874 2067  e has a weight g
-000036b0: 7265 6174 6572 2074 6861 6e20 6f72 2065  reater than or e
-000036c0: 7175 616c 2074 6f20 6b2c 2061 6e64 2046  qual to k, and F
-000036d0: 616c 7365 206f 7468 6572 7769 7365 2e22  alse otherwise."
-000036e0: 2222 0a20 2020 200a 2020 2020 6e20 3d20  "".    .    n = 
-000036f0: 412e 7368 6170 655b 305d 2023 2061 7373  A.shape[0] # ass
-00003700: 756d 6520 4120 6973 2061 2073 7175 6172  ume A is a squar
-00003710: 6520 6d61 7472 6978 0a20 2020 2076 6973  e matrix.    vis
-00003720: 6974 6564 203d 206e 702e 7a65 726f 7328  ited = np.zeros(
-00003730: 6e2c 2064 7479 7065 3d62 6f6f 6c29 0a0a  n, dtype=bool)..
-00003740: 2020 2020 6465 6620 6466 7328 6e6f 6465      def dfs(node
-00003750: 293a 0a20 2020 2020 2020 2069 6620 6e6f  ):.        if no
-00003760: 6465 203d 3d20 7461 7267 6574 3a0a 2020  de == target:.  
-00003770: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00003780: 2054 7275 650a 2020 2020 2020 2020 7669   True.        vi
-00003790: 7369 7465 645b 6e6f 6465 5d20 3d20 5472  sited[node] = Tr
-000037a0: 7565 0a20 2020 2020 2020 2066 6f72 206e  ue.        for n
-000037b0: 6569 6768 626f 722c 2077 6569 6768 7420  eighbor, weight 
-000037c0: 696e 2065 6e75 6d65 7261 7465 2841 5b6e  in enumerate(A[n
-000037d0: 6f64 652c 203a 5d29 3a0a 2020 2020 2020  ode, :]):.      
-000037e0: 2020 2020 2020 6966 2041 5b6e 6f64 655d        if A[node]
-000037f0: 5b6e 6569 6768 626f 725d 203e 2041 5b6e  [neighbor] > A[n
-00003800: 6569 6768 626f 725d 5b6e 6f64 655d 2061  eighbor][node] a
-00003810: 6e64 2077 6569 6768 7420 3e3d 206b 2061  nd weight >= k a
-00003820: 6e64 206e 6f74 2076 6973 6974 6564 5b6e  nd not visited[n
-00003830: 6569 6768 626f 725d 3a0a 2020 2020 2020  eighbor]:.      
-00003840: 2020 2020 2020 2020 2020 6966 2064 6673            if dfs
-00003850: 286e 6569 6768 626f 7229 3a0a 2020 2020  (neighbor):.    
-00003860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003870: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
-00003880: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-00003890: 0a0a 2020 2020 7265 7475 726e 2064 6673  ..    return dfs
-000038a0: 2873 6f75 7263 6529 0a0a 6465 6620 5f73  (source)..def _s
-000038b0: 706c 6974 5f63 7963 6c65 5f62 6173 6963  plit_cycle_basic
-000038c0: 280a 2020 2020 2020 2020 6564 6174 612c  (.        edata,
-000038d0: 200a 2020 2020 2020 2020 6375 7272 5f63   .        curr_c
-000038e0: 616e 6473 203d 204e 6f6e 652c 200a 2020  ands = None, .  
-000038f0: 2020 2020 2020 7374 7265 6e67 7468 5f66        strength_f
-00003900: 756e 6374 696f 6e20 3d20 4e6f 6e65 293a  unction = None):
-00003910: 0a20 2020 2022 2222 416e 2069 6d70 6c65  .    """An imple
-00003920: 6d65 6e74 6174 696f 6e20 6f66 2053 706c  mentation of Spl
-00003930: 6974 2043 7963 6c65 2062 6173 6564 206f  it Cycle based o
-00003940: 6e20 7468 6520 6d61 7468 656d 6174 6963  n the mathematic
-00003950: 616c 2064 6566 696e 6974 696f 6e2e 2020  al definition.  
-00003960: 5468 6973 2069 7320 6d6f 7265 2065 6666  This is more eff
-00003970: 6963 6965 6e74 2074 6861 6e20 7468 6520  icient than the 
-00003980: 666c 6f79 645f 7761 7273 6861 6c6c 2069  floyd_warshall i
-00003990: 6d70 6c65 6d65 6e74 6174 696f 6e2e 200a  mplementation. .
-000039a0: 2020 2020 2222 220a 2020 2020 7374 7265      """.    stre
-000039b0: 6e67 7468 5f6d 6174 7269 782c 2063 616e  ngth_matrix, can
-000039c0: 645f 746f 5f63 696e 6465 7820 3d20 6564  d_to_cindex = ed
-000039d0: 6174 612e 7374 7265 6e67 7468 5f6d 6174  ata.strength_mat
-000039e0: 7269 7828 6375 7272 5f63 616e 6473 203d  rix(curr_cands =
-000039f0: 2063 7572 725f 6361 6e64 732c 2073 7472   curr_cands, str
-00003a00: 656e 6774 685f 6675 6e63 7469 6f6e 3d73  ength_function=s
-00003a10: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-00003a20: 290a 0a20 2020 2063 616e 6469 6461 7465  )..    candidate
-00003a30: 7320 3d20 6564 6174 612e 6361 6e64 6964  s = edata.candid
-00003a40: 6174 6573 2069 6620 6375 7272 5f63 616e  ates if curr_can
-00003a50: 6473 2069 7320 4e6f 6e65 2065 6c73 6520  ds is None else 
-00003a60: 6375 7272 5f63 616e 6473 2020 0a0a 2020  curr_cands  ..  
-00003a70: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
-00003a80: 696f 6e20 3d20 6564 6174 612e 6d61 7267  ion = edata.marg
-00003a90: 696e 2069 6620 7374 7265 6e67 7468 5f66  in if strength_f
-00003aa0: 756e 6374 696f 6e20 6973 204e 6f6e 6520  unction is None 
-00003ab0: 656c 7365 2073 7472 656e 6774 685f 6675  else strength_fu
-00003ac0: 6e63 7469 6f6e 200a 0a20 2020 2070 6f74  nction ..    pot
-00003ad0: 656e 7469 616c 5f77 696e 6e65 7273 203d  ential_winners =
-00003ae0: 2073 6574 2863 616e 6469 6461 7465 7329   set(candidates)
-00003af0: 0a0a 2020 2020 666f 7220 6120 696e 2063  ..    for a in c
-00003b00: 616e 6469 6461 7465 733a 0a20 2020 2020  andidates:.     
-00003b10: 2020 2066 6f72 2062 2069 6e20 6361 6e64     for b in cand
-00003b20: 6964 6174 6573 3a0a 2020 2020 2020 2020  idates:.        
-00003b30: 2020 2020 6966 2073 7472 656e 6774 685f      if strength_
-00003b40: 6675 6e63 7469 6f6e 2862 2c20 6129 203e  function(b, a) >
-00003b50: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-00003b60: 6f6e 2861 2c20 6229 2061 6e64 206e 6f74  on(a, b) and not
-00003b70: 2068 6173 5f73 7472 6f6e 675f 7061 7468   has_strong_path
-00003b80: 2873 7472 656e 6774 685f 6d61 7472 6978  (strength_matrix
-00003b90: 2c20 6361 6e64 5f74 6f5f 6369 6e64 6578  , cand_to_cindex
-00003ba0: 2861 292c 2063 616e 645f 746f 5f63 696e  (a), cand_to_cin
-00003bb0: 6465 7828 6229 2c20 7374 7265 6e67 7468  dex(b), strength
-00003bc0: 5f66 756e 6374 696f 6e28 622c 6129 293a  _function(b,a)):
-00003bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003be0: 2070 6f74 656e 7469 616c 5f77 696e 6e65   potential_winne
-00003bf0: 7273 2e64 6973 6361 7264 2861 290a 2020  rs.discard(a).  
-00003c00: 2020 2020 2020 2020 2020 2020 2020 6272                br
-00003c10: 6561 6b0a 0a20 2020 2072 6574 7572 6e20  eak..    return 
-00003c20: 736f 7274 6564 2870 6f74 656e 7469 616c  sorted(potential
-00003c30: 5f77 696e 6e65 7273 290a 0a64 6566 205f  _winners)..def _
-00003c40: 7370 6c69 745f 6379 636c 655f 666c 6f79  split_cycle_floy
-00003c50: 645f 7761 7273 6861 6c6c 280a 2020 2020  d_warshall(.    
-00003c60: 2020 2020 6564 6174 612c 200a 2020 2020      edata, .    
-00003c70: 2020 2020 6375 7272 5f63 616e 6473 203d      curr_cands =
-00003c80: 204e 6f6e 652c 200a 2020 2020 2020 2020   None, .        
-00003c90: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-00003ca0: 6e20 3d20 4e6f 6e65 293a 2020 200a 2020  n = None):   .  
-00003cb0: 2020 2222 2241 6e20 696d 706c 656d 656e    """An implemen
-00003cc0: 7461 7469 6f6e 206f 6620 5370 6c69 7420  tation of Split 
-00003cd0: 4379 636c 6520 6261 7365 6420 6f6e 2074  Cycle based on t
-00003ce0: 6865 2046 6c6f 7964 2d57 6172 7368 616c  he Floyd-Warshal
-00003cf0: 6c20 416c 676f 7269 7468 6d2e 200a 0a20  l Algorithm. .. 
-00003d00: 2020 2053 6565 2068 7474 7073 3a2f 2f67     See https://g
-00003d10: 6974 6875 622e 636f 6d2f 6570 6163 7569  ithub.com/epacui
-00003d20: 742f 7370 6c69 7463 7963 6c65 2061 6e64  t/splitcycle and
-00003d30: 2074 6865 2070 6170 6572 2068 7474 7073   the paper https
-00003d40: 3a2f 2f61 7278 6976 2e6f 7267 2f61 6273  ://arxiv.org/abs
-00003d50: 2f32 3030 342e 3032 3335 3020 666f 7220  /2004.02350 for 
-00003d60: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
-00003d70: 2e20 0a0a 2020 2020 2222 220a 0a20 2020  . ..    """..   
-00003d80: 2063 616e 6469 6461 7465 7320 3d20 6564   candidates = ed
-00003d90: 6174 612e 6361 6e64 6964 6174 6573 2069  ata.candidates i
-00003da0: 6620 6375 7272 5f63 616e 6473 2069 7320  f curr_cands is 
-00003db0: 4e6f 6e65 2065 6c73 6520 6375 7272 5f63  None else curr_c
-00003dc0: 616e 6473 2020 2020 0a20 2020 2073 7472  ands    .    str
-00003dd0: 656e 6774 685f 6675 6e63 7469 6f6e 203d  ength_function =
-00003de0: 2065 6461 7461 2e6d 6172 6769 6e20 6966   edata.margin if
-00003df0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-00003e00: 6f6e 2069 7320 4e6f 6e65 2065 6c73 6520  on is None else 
-00003e10: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-00003e20: 6e20 0a20 0a20 2020 2077 6561 6b5f 636f  n . .    weak_co
-00003e30: 6e64 6f72 6365 745f 7769 6e6e 6572 7320  ndorcet_winners 
-00003e40: 3d20 7b63 3a54 7275 6520 666f 7220 6320  = {c:True for c 
-00003e50: 696e 2063 616e 6469 6461 7465 737d 0a20  in candidates}. 
-00003e60: 2020 2073 5f6d 6174 7269 7820 3d20 5b5b     s_matrix = [[
-00003e70: 2d6e 702e 696e 6620 666f 7220 5f20 696e  -np.inf for _ in
-00003e80: 2063 616e 6469 6461 7465 735d 2066 6f72   candidates] for
-00003e90: 205f 2069 6e20 6361 6e64 6964 6174 6573   _ in candidates
-00003ea0: 5d0a 2020 2020 0a20 2020 2023 2069 6e69  ].    .    # ini
-00003eb0: 7469 616c 697a 6520 7468 6520 735f 6d61  tialize the s_ma
-00003ec0: 7472 6978 0a20 2020 2066 6f72 2063 315f  trix.    for c1_
-00003ed0: 6964 782c 2063 3120 696e 2065 6e75 6d65  idx, c1 in enume
-00003ee0: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
-00003ef0: 3a0a 2020 2020 2020 2020 666f 7220 6332  :.        for c2
-00003f00: 5f69 6478 2c20 6332 2069 6e20 656e 756d  _idx, c2 in enum
-00003f10: 6572 6174 6528 6361 6e64 6964 6174 6573  erate(candidates
-00003f20: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
-00003f30: 6620 2865 6461 7461 2e6d 616a 6f72 6974  f (edata.majorit
-00003f40: 795f 7072 6566 6572 7328 6331 2c20 6332  y_prefers(c1, c2
-00003f50: 2920 6f72 2063 3120 3d3d 2063 3229 3a0a  ) or c1 == c2):.
-00003f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f70: 735f 6d61 7472 6978 5b63 315f 6964 785d  s_matrix[c1_idx]
-00003f80: 5b63 325f 6964 785d 203d 2073 7472 656e  [c2_idx] = stren
-00003f90: 6774 685f 6675 6e63 7469 6f6e 2863 312c  gth_function(c1,
-00003fa0: 2063 3229 200a 2020 2020 2020 2020 2020   c2) .          
-00003fb0: 2020 2020 2020 7765 616b 5f63 6f6e 646f        weak_condo
-00003fc0: 7263 6574 5f77 696e 6e65 7273 5b63 325d  rcet_winners[c2]
-00003fd0: 203d 2077 6561 6b5f 636f 6e64 6f72 6365   = weak_condorce
-00003fe0: 745f 7769 6e6e 6572 735b 6332 5d20 616e  t_winners[c2] an
-00003ff0: 6420 2863 3120 3d3d 2063 3229 2023 2057  d (c1 == c2) # W
-00004000: 6561 6b20 436f 6e64 6f72 6365 7420 7769  eak Condorcet wi
-00004010: 6e6e 6572 7320 6172 6520 5370 6c69 7420  nners are Split 
-00004020: 4379 636c 6520 7769 6e6e 6572 730a 2020  Cycle winners.  
-00004030: 2020 0a20 2020 2073 7472 656e 6774 6820    .    strength 
-00004040: 3d20 6c69 7374 286d 6170 286c 616d 6264  = list(map(lambd
-00004050: 6120 6920 3a20 6c69 7374 286d 6170 286c  a i : list(map(l
-00004060: 616d 6264 6120 6a20 3a20 6a20 2c20 6929  ambda j : j , i)
-00004070: 2920 2c20 735f 6d61 7472 6978 2929 0a20  ) , s_matrix)). 
-00004080: 2020 2066 6f72 2069 5f69 6478 2c20 6920     for i_idx, i 
-00004090: 696e 2065 6e75 6d65 7261 7465 2863 616e  in enumerate(can
-000040a0: 6469 6461 7465 7329 3a20 0a20 2020 2020  didates): .     
-000040b0: 2020 2066 6f72 206a 5f69 6478 2c20 6a20     for j_idx, j 
-000040c0: 696e 2065 6e75 6d65 7261 7465 2863 616e  in enumerate(can
-000040d0: 6469 6461 7465 7329 3a0a 2020 2020 2020  didates):.      
-000040e0: 2020 2020 2020 6966 2069 213d 206a 3a0a        if i!= j:.
-000040f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004100: 6966 206e 6f74 2077 6561 6b5f 636f 6e64  if not weak_cond
-00004110: 6f72 6365 745f 7769 6e6e 6572 735b 6a5d  orcet_winners[j]
-00004120: 3a20 2320 7765 616b 2043 6f6e 646f 7263  : # weak Condorc
-00004130: 6574 2077 696e 6e65 7273 2061 7265 2053  et winners are S
-00004140: 706c 6974 2043 7963 6c65 2077 696e 6e65  plit Cycle winne
-00004150: 7273 0a20 2020 2020 2020 2020 2020 2020  rs.             
-00004160: 2020 2020 2020 2066 6f72 206b 5f69 6478         for k_idx
-00004170: 2c20 6b20 696e 2065 6e75 6d65 7261 7465  , k in enumerate
-00004180: 2863 616e 6469 6461 7465 7329 3a20 0a20  (candidates): . 
-00004190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041a0: 2020 2020 2020 2069 6620 6920 213d 206b         if i != k
-000041b0: 2061 6e64 206a 2021 3d20 6b3a 0a20 2020   and j != k:.   
-000041c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041d0: 2020 2020 2020 2020 2073 7472 656e 6774           strengt
-000041e0: 685b 6a5f 6964 785d 5b6b 5f69 6478 5d20  h[j_idx][k_idx] 
-000041f0: 3d20 6d61 7828 7374 7265 6e67 7468 5b6a  = max(strength[j
-00004200: 5f69 6478 5d5b 6b5f 6964 785d 2c20 6d69  _idx][k_idx], mi
-00004210: 6e28 7374 7265 6e67 7468 5b6a 5f69 6478  n(strength[j_idx
-00004220: 5d5b 695f 6964 785d 2c73 7472 656e 6774  ][i_idx],strengt
-00004230: 685b 695f 6964 785d 5b6b 5f69 6478 5d29  h[i_idx][k_idx])
-00004240: 290a 2020 2020 7769 6e6e 6572 7320 3d20  ).    winners = 
-00004250: 7b69 3a54 7275 6520 666f 7220 6920 696e  {i:True for i in
-00004260: 2063 616e 6469 6461 7465 737d 0a20 2020   candidates}.   
-00004270: 2066 6f72 2069 5f69 6478 2c20 6920 696e   for i_idx, i in
-00004280: 2065 6e75 6d65 7261 7465 2863 616e 6469   enumerate(candi
-00004290: 6461 7465 7329 3a0a 2020 2020 2020 2020  dates):.        
-000042a0: 666f 7220 6a5f 6964 782c 206a 2069 6e20  for j_idx, j in 
-000042b0: 656e 756d 6572 6174 6528 6361 6e64 6964  enumerate(candid
-000042c0: 6174 6573 293a 0a20 2020 2020 2020 2020  ates):.         
-000042d0: 2020 2069 6620 6920 213d 206a 3a0a 2020     if i != j:.  
-000042e0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000042f0: 2073 5f6d 6174 7269 785b 6a5f 6964 785d   s_matrix[j_idx]
-00004300: 5b69 5f69 6478 5d20 3e20 7374 7265 6e67  [i_idx] > streng
-00004310: 7468 5b69 5f69 6478 5d5b 6a5f 6964 785d  th[i_idx][j_idx]
-00004320: 3a20 2320 7468 6520 6d61 696e 2064 6966  : # the main dif
-00004330: 6665 7265 6e63 6520 7769 7468 2042 6561  ference with Bea
-00004340: 7420 5061 7468 0a20 2020 2020 2020 2020  t Path.         
-00004350: 2020 2020 2020 2020 2020 2077 696e 6e65             winne
-00004360: 7273 5b69 5d20 3d20 4661 6c73 650a 2020  rs[i] = False.  
-00004370: 2020 7265 7475 726e 2073 6f72 7465 6428    return sorted(
-00004380: 5b63 2066 6f72 2063 2069 6e20 6361 6e64  [c for c in cand
-00004390: 6964 6174 6573 2069 6620 7769 6e6e 6572  idates if winner
-000043a0: 735b 635d 5d29 0a0a 4076 6d28 6e61 6d65  s[c]])..@vm(name
-000043b0: 3d22 5370 6c69 7420 4379 636c 6522 290a  ="Split Cycle").
-000043c0: 6465 6620 7370 6c69 745f 6379 636c 6528  def split_cycle(
-000043d0: 0a20 2020 2065 6461 7461 2c20 0a20 2020  .    edata, .   
-000043e0: 2063 7572 725f 6361 6e64 733d 4e6f 6e65   curr_cands=None
-000043f0: 2c20 0a20 2020 2073 7472 656e 6774 685f  , .    strength_
-00004400: 6675 6e63 7469 6f6e 3d4e 6f6e 652c 0a20  function=None,. 
-00004410: 2020 2061 6c67 6f72 6974 686d 3d27 6261     algorithm='ba
-00004420: 7369 6327 293a 0a0a 2020 2020 2222 2241  sic'):..    """A
-00004430: 202a 2a6d 616a 6f72 6974 7920 6379 636c   **majority cycl
-00004440: 652a 2a20 6973 2061 2073 6571 7565 6e63  e** is a sequenc
-00004450: 6520 3a6d 6174 683a 6078 5f31 2c20 5c6c  e :math:`x_1, \l
-00004460: 646f 7473 202c 785f 6e60 206f 6620 6469  dots ,x_n` of di
-00004470: 7374 696e 6374 2063 616e 6469 6461 7465  stinct candidate
-00004480: 7320 7769 7468 203a 6d61 7468 3a60 785f  s with :math:`x_
-00004490: 313d 785f 6e60 2073 7563 6820 7468 6174  1=x_n` such that
-000044a0: 2066 6f72 203a 6d61 7468 3a60 3120 5c6c   for :math:`1 \l
-000044b0: 6571 206b 205c 6c65 7120 6e2d 3160 2c20  eq k \leq n-1`, 
-000044c0: 203a 6d61 7468 3a60 785f 6b60 2069 7320   :math:`x_k` is 
-000044d0: 6d61 6a6f 7269 7479 2070 7265 6665 7272  majority preferr
-000044e0: 6564 2074 6f20 3a6d 6174 683a 6078 5f7b  ed to :math:`x_{
-000044f0: 6b2b 317d 602e 2020 5468 6520 5370 6c69  k+1}`.  The Spli
-00004500: 7420 4379 636c 6520 7769 6e6e 6572 7320  t Cycle winners 
-00004510: 6172 6520 6465 7465 726d 696e 6564 2061  are determined a
-00004520: 7320 666f 6c6c 6f77 733a 2020 0a20 2020  s follows:  .   
-00004530: 200a 2020 2020 4966 2063 616e 6469 6461   .    If candida
-00004540: 7465 2078 2068 6173 2061 2070 6f73 6974  te x has a posit
-00004550: 6976 6520 6d61 7267 696e 206f 7665 7220  ive margin over 
-00004560: 7920 616e 6420 2878 2c79 2920 6973 206e  y and (x,y) is n
-00004570: 6f74 2074 6865 2077 6561 6b65 7374 2065  ot the weakest e
-00004580: 6467 6520 696e 2061 2063 7963 6c65 2c20  dge in a cycle, 
-00004590: 7468 656e 2078 2064 6566 6561 7473 2079  then x defeats y
-000045a0: 2e20 4571 7569 7661 6c65 6e74 6c79 2c20  . Equivalently, 
-000045b0: 6966 2078 2068 6173 2061 2070 6f73 6974  if x has a posit
-000045c0: 6976 6520 6d61 7267 696e 206f 7665 7220  ive margin over 
-000045d0: 7920 616e 6420 7468 6572 6520 6973 206e  y and there is n
-000045e0: 6f20 7061 7468 2066 726f 6d20 7920 6261  o path from y ba
-000045f0: 636b 2074 6f20 7820 6f66 2073 7472 656e  ck to x of stren
-00004600: 6774 6820 6174 206c 6561 7374 2074 6865  gth at least the
-00004610: 206d 6172 6769 6e20 6f66 2078 206f 7665   margin of x ove
-00004620: 7220 792c 2074 6865 6e20 7820 6465 6665  r y, then x defe
-00004630: 6174 7320 792e 200a 2020 2020 0a20 2020  ats y. .    .   
-00004640: 2054 6865 2063 616e 6469 6461 7465 7320   The candidates 
-00004650: 7468 6174 2061 7265 2075 6e64 6566 6561  that are undefea
-00004660: 7465 6420 6172 6520 7468 6520 5370 6c69  ted are the Spli
-00004670: 7420 4379 636c 6520 7769 6e6e 6572 732e  t Cycle winners.
-00004680: 0a0a 2020 2020 5365 6520 6874 7470 733a  ..    See https:
-00004690: 2f2f 6769 7468 7562 2e63 6f6d 2f65 7061  //github.com/epa
-000046a0: 6375 6974 2f73 706c 6974 6379 636c 6520  cuit/splitcycle 
-000046b0: 616e 6420 7468 6520 7061 7065 7220 6874  and the paper ht
-000046c0: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
-000046d0: 6162 732f 3230 3034 2e30 3233 3530 2066  abs/2004.02350 f
-000046e0: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
-000046f0: 696f 6e2e 200a 0a20 2020 2041 7267 733a  ion. ..    Args:
-00004700: 0a20 2020 2020 2020 2065 6461 7461 2028  .        edata (
-00004710: 5072 6f66 696c 652c 2050 726f 6669 6c65  Profile, Profile
-00004720: 5769 7468 5469 6573 2c20 4d61 7267 696e  WithTies, Margin
-00004730: 4772 6170 6829 3a20 416e 7920 656c 6563  Graph): Any elec
-00004740: 7469 6f6e 2064 6174 6120 7468 6174 2068  tion data that h
-00004750: 6173 2061 2060 6d61 7267 696e 6020 6d65  as a `margin` me
-00004760: 7468 6f64 2e20 0a20 2020 2020 2020 2063  thod. .        c
-00004770: 7572 725f 6361 6e64 7320 284c 6973 745b  urr_cands (List[
-00004780: 696e 745d 2c20 6f70 7469 6f6e 616c 293a  int], optional):
-00004790: 2049 6620 7365 742c 2074 6865 6e20 6669   If set, then fi
-000047a0: 6e64 2074 6865 2077 696e 6e65 7273 2066  nd the winners f
-000047b0: 6f72 2074 6865 2070 726f 6669 6c65 2072  or the profile r
-000047c0: 6573 7472 6963 7465 6420 746f 2074 6865  estricted to the
-000047d0: 2063 616e 6469 6461 7465 7320 696e 2060   candidates in `
-000047e0: 6063 7572 725f 6361 6e64 7360 600a 2020  `curr_cands``.  
-000047f0: 2020 2020 2020 7374 7265 6e67 7468 5f66        strength_f
-00004800: 756e 6374 696f 6e20 2866 756e 6374 696f  unction (functio
-00004810: 6e2c 206f 7074 696f 6e61 6c29 3a20 5468  n, optional): Th
-00004820: 6520 7374 7265 6e67 7468 2066 756e 6374  e strength funct
-00004830: 696f 6e20 746f 2062 6520 7573 6564 2074  ion to be used t
-00004840: 6f20 6361 6c63 756c 6174 6520 7468 6520  o calculate the 
-00004850: 7374 7265 6e67 7468 206f 6620 6120 7061  strength of a pa
-00004860: 7468 2e20 2020 5468 6520 6465 6661 756c  th.   The defaul
-00004870: 7420 6973 2074 6865 206d 6172 6769 6e20  t is the margin 
-00004880: 6d65 7468 6f64 206f 6620 6060 6564 6174  method of ``edat
-00004890: 6160 602e 2020 2054 6869 7320 6f6e 6c79  a``.   This only
-000048a0: 206d 6174 7465 7273 2077 6865 6e20 7468   matters when th
-000048b0: 6520 6261 6c6c 6f74 7320 6172 6520 6e6f  e ballots are no
-000048c0: 7420 6c69 6e65 6172 206f 7264 6572 732e  t linear orders.
-000048d0: 200a 2020 2020 2020 2020 616c 676f 7269   .        algori
-000048e0: 7468 6d20 2873 7472 293a 2053 7065 6369  thm (str): Speci
-000048f0: 6679 2077 6869 6368 2061 6c67 6f72 6974  fy which algorit
-00004900: 686d 2074 6f20 7573 652e 2020 4f70 7469  hm to use.  Opti
-00004910: 6f6e 7320 6172 6520 2762 6173 6963 2720  ons are 'basic' 
-00004920: 2874 6865 2064 6566 6175 6c74 2920 616e  (the default) an
-00004930: 6420 2766 6c6f 7964 5f77 6172 7368 616c  d 'floyd_warshal
-00004940: 6c27 2e0a 0a20 2020 2052 6574 7572 6e73  l'...    Returns
-00004950: 3a20 0a20 2020 2020 2020 2041 2073 6f72  : .        A sor
-00004960: 7465 6420 6c69 7374 206f 6620 6361 6e64  ted list of cand
-00004970: 6964 6174 6573 2e20 0a0a 2020 2020 2e2e  idates. ..    ..
-00004980: 2073 6565 616c 736f 3a3a 0a0a 2020 2020   seealso::..    
-00004990: 2020 2020 3a6d 6574 683a 6070 7265 665f      :meth:`pref_
-000049a0: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
-000049b0: 7365 645f 6d65 7468 6f64 732e 7370 6c69  sed_methods.spli
-000049c0: 745f 6379 636c 655f 6465 6665 6174 600a  t_cycle_defeat`.
-000049d0: 0a20 2020 203a 4578 616d 706c 653a 200a  .    :Example: .
-000049e0: 0a20 2020 202e 2e20 706c 6f74 3a3a 2020  .    .. plot::  
-000049f0: 6d61 7267 696e 5f67 7261 7068 735f 6578  margin_graphs_ex
-00004a00: 616d 706c 6573 2f6d 675f 6578 5f62 705f  amples/mg_ex_bp_
-00004a10: 7270 2e70 790a 2020 2020 2020 2020 3a63  rp.py.        :c
-00004a20: 6f6e 7465 7874 3a20 7265 7365 7420 200a  ontext: reset  .
-00004a30: 2020 2020 2020 2020 3a69 6e63 6c75 6465          :include
-00004a40: 2d73 6f75 7263 653a 2054 7275 650a 0a20  -source: True.. 
-00004a50: 2020 202e 2e20 636f 6465 2d62 6c6f 636b     .. code-block
-00004a60: 3a3a 200a 0a20 2020 2020 2020 2066 726f  :: ..        fro
-00004a70: 6d20 7072 6566 5f76 6f74 696e 672e 6d61  m pref_voting.ma
-00004a80: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
-00004a90: 6473 2069 6d70 6f72 7420 7370 6c69 745f  ds import split_
-00004aa0: 6379 636c 650a 0a20 2020 2020 2020 2073  cycle..        s
-00004ab0: 706c 6974 5f63 7963 6c65 2e64 6973 706c  plit_cycle.displ
-00004ac0: 6179 286d 6729 0a0a 0a20 2020 202e 2e20  ay(mg)...    .. 
-00004ad0: 6578 6563 5f63 6f64 653a 3a20 0a20 2020  exec_code:: .   
-00004ae0: 2020 2020 203a 6869 6465 5f63 6f64 653a       :hide_code:
-00004af0: 0a0a 2020 2020 2020 2020 6672 6f6d 2070  ..        from p
-00004b00: 7265 665f 766f 7469 6e67 2e77 6569 6768  ref_voting.weigh
-00004b10: 7465 645f 6d61 6a6f 7269 7479 5f67 7261  ted_majority_gra
-00004b20: 7068 7320 696d 706f 7274 204d 6172 6769  phs import Margi
-00004b30: 6e47 7261 7068 0a20 2020 2020 2020 2066  nGraph.        f
-00004b40: 726f 6d20 7072 6566 5f76 6f74 696e 672e  rom pref_voting.
-00004b50: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
-00004b60: 686f 6473 2069 6d70 6f72 7420 7370 6c69  hods import spli
-00004b70: 745f 6379 636c 650a 2020 2020 2020 2020  t_cycle.        
-00004b80: 0a20 2020 2020 2020 206d 6720 3d20 4d61  .        mg = Ma
-00004b90: 7267 696e 4772 6170 6828 5b30 2c20 312c  rginGraph([0, 1,
-00004ba0: 2032 2c20 335d 2c20 5b28 302c 2032 2c20   2, 3], [(0, 2, 
-00004bb0: 3329 2c20 2831 2c20 302c 2035 292c 2028  3), (1, 0, 5), (
-00004bc0: 322c 2031 2c20 3529 2c20 2832 2c20 332c  2, 1, 5), (2, 3,
-00004bd0: 2031 292c 2028 332c 2030 2c20 3329 2c20   1), (3, 0, 3), 
-00004be0: 2833 2c20 312c 2031 295d 290a 2020 2020  (3, 1, 1)]).    
-00004bf0: 2020 2020 0a20 2020 2020 2020 2073 706c      .        spl
-00004c00: 6974 5f63 7963 6c65 2e64 6973 706c 6179  it_cycle.display
-00004c10: 286d 6729 0a20 2020 2020 2020 2073 706c  (mg).        spl
-00004c20: 6974 5f63 7963 6c65 2e64 6973 706c 6179  it_cycle.display
-00004c30: 286d 672c 2061 6c67 6f72 6974 686d 3d27  (mg, algorithm='
-00004c40: 6261 7369 6327 290a 2020 2020 2020 2020  basic').        
-00004c50: 7370 6c69 745f 6379 636c 652e 6469 7370  split_cycle.disp
-00004c60: 6c61 7928 6d67 2c20 616c 676f 7269 7468  lay(mg, algorith
-00004c70: 6d3d 2766 6c6f 7964 5f77 6172 7368 616c  m='floyd_warshal
-00004c80: 6c27 290a 2020 2020 2222 220a 2020 2020  l').    """.    
-00004c90: 0a20 2020 2069 6620 616c 676f 7269 7468  .    if algorith
-00004ca0: 6d20 3d3d 2027 6261 7369 6327 3a0a 2020  m == 'basic':.  
-00004cb0: 2020 2020 2020 7265 7475 726e 205f 7370        return _sp
-00004cc0: 6c69 745f 6379 636c 655f 6261 7369 6328  lit_cycle_basic(
-00004cd0: 6564 6174 612c 2063 7572 725f 6361 6e64  edata, curr_cand
-00004ce0: 7320 3d20 6375 7272 5f63 616e 6473 2c20  s = curr_cands, 
-00004cf0: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-00004d00: 6e20 3d20 7374 7265 6e67 7468 5f66 756e  n = strength_fun
-00004d10: 6374 696f 6e29 0a20 2020 2065 6c69 6620  ction).    elif 
-00004d20: 616c 676f 7269 7468 6d20 3d3d 2027 666c  algorithm == 'fl
-00004d30: 6f79 645f 7761 7273 6861 6c6c 273a 0a20  oyd_warshall':. 
-00004d40: 2020 2020 2020 2072 6574 7572 6e20 5f73         return _s
-00004d50: 706c 6974 5f63 7963 6c65 5f66 6c6f 7964  plit_cycle_floyd
-00004d60: 5f77 6172 7368 616c 6c28 6564 6174 612c  _warshall(edata,
-00004d70: 2063 7572 725f 6361 6e64 7320 3d20 6375   curr_cands = cu
-00004d80: 7272 5f63 616e 6473 2c20 7374 7265 6e67  rr_cands, streng
-00004d90: 7468 5f66 756e 6374 696f 6e20 3d20 7374  th_function = st
-00004da0: 7265 6e67 7468 5f66 756e 6374 696f 6e29  rength_function)
-00004db0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-00004dc0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-00004dd0: 726f 7228 2249 6e76 616c 6964 2061 6c67  ror("Invalid alg
-00004de0: 6f72 6974 686d 2073 7065 6369 6669 6564  orithm specified
-00004df0: 2e22 290a 0a0a 6465 6620 7370 6c69 745f  .")...def split_
-00004e00: 6379 636c 655f 6465 6665 6174 2865 6461  cycle_defeat(eda
-00004e10: 7461 2c20 6375 7272 5f63 616e 6473 203d  ta, curr_cands =
-00004e20: 204e 6f6e 652c 2073 7472 656e 6774 685f   None, strength_
-00004e30: 6675 6e63 7469 6f6e 203d 204e 6f6e 6529  function = None)
-00004e40: 3a20 2020 0a20 2020 2022 2222 0a20 2020  :   .    """.   
-00004e50: 2052 6574 7572 6e73 2074 6865 2053 706c   Returns the Spl
-00004e60: 6974 2043 7963 6c65 2064 6566 6561 7420  it Cycle defeat 
-00004e70: 7265 6c61 7469 6f6e 2e20 0a0a 2020 2020  relation. ..    
-00004e80: 5365 6520 6874 7470 733a 2f2f 6172 7869  See https://arxi
-00004e90: 762e 6f72 672f 6162 732f 3230 3038 2e30  v.org/abs/2008.0
-00004ea0: 3834 3531 2066 6f72 2061 6e20 6578 7465  8451 for an exte
-00004eb0: 6e64 6564 2064 6973 6375 7373 696f 6e20  nded discussion 
-00004ec0: 6f66 2074 6869 7320 6e6f 7469 6f6e 206f  of this notion o
-00004ed0: 6620 6465 6665 6174 2069 6e20 616e 2065  f defeat in an e
-00004ee0: 6c65 6374 696f 6e2e 200a 0a20 2020 2041  lection. ..    A
-00004ef0: 7267 733a 0a20 2020 2020 2020 2065 6461  rgs:.        eda
-00004f00: 7461 2028 5072 6f66 696c 652c 2050 726f  ta (Profile, Pro
-00004f10: 6669 6c65 5769 7468 5469 6573 2c20 4d61  fileWithTies, Ma
-00004f20: 7267 696e 4772 6170 6829 3a20 416e 7920  rginGraph): Any 
-00004f30: 656c 6563 7469 6f6e 2064 6174 6120 7468  election data th
-00004f40: 6174 2068 6173 2061 2060 6d61 7267 696e  at has a `margin
-00004f50: 6020 6d65 7468 6f64 2e20 0a20 2020 2020  ` method. .     
-00004f60: 2020 2063 7572 725f 6361 6e64 7320 284c     curr_cands (L
-00004f70: 6973 745b 696e 745d 2c20 6f70 7469 6f6e  ist[int], option
-00004f80: 616c 293a 2049 6620 7365 742c 2074 6865  al): If set, the
-00004f90: 6e20 6669 6e64 2074 6865 2077 696e 6e65  n find the winne
-00004fa0: 7273 2066 6f72 2074 6865 2070 726f 6669  rs for the profi
-00004fb0: 6c65 2072 6573 7472 6963 7465 6420 746f  le restricted to
-00004fc0: 2074 6865 2063 616e 6469 6461 7465 7320   the candidates 
-00004fd0: 696e 2060 6063 7572 725f 6361 6e64 7360  in ``curr_cands`
-00004fe0: 600a 0a20 2020 2052 6574 7572 6e73 3a20  `..    Returns: 
-00004ff0: 0a20 2020 2020 2020 2041 206e 6574 776f  .        A netwo
-00005000: 726b 7820 4469 4772 6170 6820 7265 7072  rkx DiGraph repr
-00005010: 6573 656e 7469 6e67 2074 6865 2053 706c  esenting the Spl
-00005020: 6974 2043 7963 6c65 2064 6566 6561 7420  it Cycle defeat 
-00005030: 7265 6c61 7469 6f6e 2e20 0a0a 2020 2020  relation. ..    
-00005040: 2e2e 2073 6565 616c 736f 3a3a 0a0a 2020  .. seealso::..  
-00005050: 2020 2020 2020 3a6d 6574 683a 6070 7265        :meth:`pre
-00005060: 665f 766f 7469 6e67 2e6d 6172 6769 6e5f  f_voting.margin_
-00005070: 6261 7365 645f 6d65 7468 6f64 732e 7370  based_methods.sp
-00005080: 6c69 745f 6379 636c 6560 2c20 3a6d 6574  lit_cycle`, :met
-00005090: 683a 6070 7265 665f 766f 7469 6e67 2e6d  h:`pref_voting.m
-000050a0: 6172 6769 6e5f 6261 7365 645f 6d65 7468  argin_based_meth
-000050b0: 6f64 732e 7370 6c69 745f 6379 636c 655f  ods.split_cycle_
-000050c0: 466c 6f79 645f 5761 7273 6861 6c6c 600a  Floyd_Warshall`.
-000050d0: 0a20 2020 203a 4578 616d 706c 653a 200a  .    :Example: .
-000050e0: 0a20 2020 202e 2e20 706c 6f74 3a3a 2020  .    .. plot::  
-000050f0: 6d61 7267 696e 5f67 7261 7068 735f 6578  margin_graphs_ex
-00005100: 616d 706c 6573 2f6d 675f 6578 5f73 635f  amples/mg_ex_sc_
-00005110: 6465 6665 6174 2e70 790a 2020 2020 2020  defeat.py.      
-00005120: 2020 3a63 6f6e 7465 7874 3a20 7265 7365    :context: rese
-00005130: 7420 200a 2020 2020 2020 2020 3a69 6e63  t  .        :inc
-00005140: 6c75 6465 2d73 6f75 7263 653a 2054 7275  lude-source: Tru
-00005150: 650a 0a20 2020 2022 2222 0a0a 2020 2020  e..    """..    
-00005160: 6361 6e64 6964 6174 6573 203d 2065 6461  candidates = eda
-00005170: 7461 2e63 616e 6469 6461 7465 7320 6966  ta.candidates if
-00005180: 2063 7572 725f 6361 6e64 7320 6973 204e   curr_cands is N
-00005190: 6f6e 6520 656c 7365 2063 7572 725f 6361  one else curr_ca
-000051a0: 6e64 7320 2020 200a 2020 2020 7374 7265  nds    .    stre
-000051b0: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
-000051c0: 6564 6174 612e 6d61 7267 696e 2069 6620  edata.margin if 
-000051d0: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-000051e0: 6e20 6973 204e 6f6e 6520 656c 7365 2073  n is None else s
-000051f0: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-00005200: 200a 200a 2020 2020 7765 616b 5f63 6f6e   . .    weak_con
-00005210: 646f 7263 6574 5f77 696e 6e65 7273 203d  dorcet_winners =
-00005220: 207b 633a 5472 7565 2066 6f72 2063 2069   {c:True for c i
-00005230: 6e20 6361 6e64 6964 6174 6573 7d0a 2020  n candidates}.  
-00005240: 2020 735f 6d61 7472 6978 203d 205b 5b2d    s_matrix = [[-
-00005250: 6e70 2e69 6e66 2066 6f72 205f 2069 6e20  np.inf for _ in 
-00005260: 6361 6e64 6964 6174 6573 5d20 666f 7220  candidates] for 
-00005270: 5f20 696e 2063 616e 6469 6461 7465 735d  _ in candidates]
-00005280: 0a20 2020 200a 2020 2020 2320 696e 6974  .    .    # init
-00005290: 6961 6c69 7a65 2074 6865 2073 5f6d 6174  ialize the s_mat
-000052a0: 7269 780a 2020 2020 666f 7220 6331 5f69  rix.    for c1_i
-000052b0: 6478 2c20 6331 2069 6e20 656e 756d 6572  dx, c1 in enumer
-000052c0: 6174 6528 6361 6e64 6964 6174 6573 293a  ate(candidates):
-000052d0: 0a20 2020 2020 2020 2066 6f72 2063 325f  .        for c2_
-000052e0: 6964 782c 2063 3220 696e 2065 6e75 6d65  idx, c2 in enume
-000052f0: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
-00005300: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00005310: 2028 6564 6174 612e 6d61 6a6f 7269 7479   (edata.majority
-00005320: 5f70 7265 6665 7273 2863 312c 2063 3229  _prefers(c1, c2)
-00005330: 206f 7220 6331 203d 3d20 6332 293a 0a20   or c1 == c2):. 
-00005340: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00005350: 5f6d 6174 7269 785b 6331 5f69 6478 5d5b  _matrix[c1_idx][
-00005360: 6332 5f69 6478 5d20 3d20 7374 7265 6e67  c2_idx] = streng
-00005370: 7468 5f66 756e 6374 696f 6e28 6331 2c20  th_function(c1, 
-00005380: 6332 2920 0a20 2020 2020 2020 2020 2020  c2) .           
-00005390: 2020 2020 2077 6561 6b5f 636f 6e64 6f72       weak_condor
-000053a0: 6365 745f 7769 6e6e 6572 735b 6332 5d20  cet_winners[c2] 
-000053b0: 3d20 7765 616b 5f63 6f6e 646f 7263 6574  = weak_condorcet
-000053c0: 5f77 696e 6e65 7273 5b63 325d 2061 6e64  _winners[c2] and
-000053d0: 2028 6331 203d 3d20 6332 2920 2320 7765   (c1 == c2) # we
-000053e0: 616b 2043 6f6e 646f 7263 6574 2077 696e  ak Condorcet win
-000053f0: 6e65 7273 2061 7265 2053 706c 6974 2043  ners are Split C
-00005400: 7963 6c65 2077 696e 6e65 7273 0a20 2020  ycle winners.   
-00005410: 200a 2020 2020 7374 7265 6e67 7468 203d   .    strength =
-00005420: 206c 6973 7428 6d61 7028 6c61 6d62 6461   list(map(lambda
-00005430: 2069 203a 206c 6973 7428 6d61 7028 6c61   i : list(map(la
-00005440: 6d62 6461 206a 203a 206a 202c 2069 2929  mbda j : j , i))
-00005450: 202c 2073 5f6d 6174 7269 7829 290a 2020   , s_matrix)).  
-00005460: 2020 666f 7220 695f 6964 782c 2069 2069    for i_idx, i i
-00005470: 6e20 656e 756d 6572 6174 6528 6361 6e64  n enumerate(cand
-00005480: 6964 6174 6573 293a 200a 2020 2020 2020  idates): .      
-00005490: 2020 666f 7220 6a5f 6964 782c 206a 2069    for j_idx, j i
-000054a0: 6e20 656e 756d 6572 6174 6528 6361 6e64  n enumerate(cand
-000054b0: 6964 6174 6573 293a 0a20 2020 2020 2020  idates):.       
-000054c0: 2020 2020 2069 6620 6921 3d20 6a3a 0a20       if i!= j:. 
-000054d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000054e0: 6620 6e6f 7420 7765 616b 5f63 6f6e 646f  f not weak_condo
-000054f0: 7263 6574 5f77 696e 6e65 7273 5b6a 5d3a  rcet_winners[j]:
-00005500: 2023 2077 6561 6b20 436f 6e64 6f72 6365   # weak Condorce
-00005510: 7420 7769 6e6e 6572 7320 6172 6520 5370  t winners are Sp
-00005520: 6c69 7420 4379 636c 6520 7769 6e6e 6572  lit Cycle winner
-00005530: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00005540: 2020 2020 2020 666f 7220 6b5f 6964 782c        for k_idx,
-00005550: 206b 2069 6e20 656e 756d 6572 6174 6528   k in enumerate(
-00005560: 6361 6e64 6964 6174 6573 293a 200a 2020  candidates): .  
-00005570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005580: 2020 2020 2020 6966 2069 2021 3d20 6b20        if i != k 
-00005590: 616e 6420 6a20 213d 206b 3a0a 2020 2020  and j != k:.    
-000055a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055b0: 2020 2020 2020 2020 7374 7265 6e67 7468          strength
-000055c0: 5b6a 5f69 6478 5d5b 6b5f 6964 785d 203d  [j_idx][k_idx] =
-000055d0: 206d 6178 2873 7472 656e 6774 685b 6a5f   max(strength[j_
-000055e0: 6964 785d 5b6b 5f69 6478 5d2c 206d 696e  idx][k_idx], min
-000055f0: 2873 7472 656e 6774 685b 6a5f 6964 785d  (strength[j_idx]
-00005600: 5b69 5f69 6478 5d2c 7374 7265 6e67 7468  [i_idx],strength
-00005610: 5b69 5f69 6478 5d5b 6b5f 6964 785d 2929  [i_idx][k_idx]))
-00005620: 0a20 0a20 2020 2064 6566 6561 745f 6772  . .    defeat_gr
-00005630: 6170 6820 3d20 6e78 2e44 6947 7261 7068  aph = nx.DiGraph
-00005640: 2829 0a20 2020 2064 6566 6561 745f 6772  ().    defeat_gr
-00005650: 6170 682e 6164 645f 6e6f 6465 735f 6672  aph.add_nodes_fr
-00005660: 6f6d 2863 616e 6469 6461 7465 7329 0a0a  om(candidates)..
-00005670: 2020 2020 666f 7220 695f 6964 782c 2069      for i_idx, i
-00005680: 2069 6e20 656e 756d 6572 6174 6528 6361   in enumerate(ca
-00005690: 6e64 6964 6174 6573 293a 0a20 2020 2020  ndidates):.     
-000056a0: 2020 2066 6f72 206a 5f69 6478 2c20 6a20     for j_idx, j 
-000056b0: 696e 2065 6e75 6d65 7261 7465 2863 616e  in enumerate(can
-000056c0: 6469 6461 7465 7329 3a0a 2020 2020 2020  didates):.      
-000056d0: 2020 2020 2020 6966 2069 2021 3d20 6a3a        if i != j:
-000056e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000056f0: 2069 6620 735f 6d61 7472 6978 5b6a 5f69   if s_matrix[j_i
-00005700: 6478 5d5b 695f 6964 785d 203e 2073 7472  dx][i_idx] > str
-00005710: 656e 6774 685b 695f 6964 785d 5b6a 5f69  ength[i_idx][j_i
-00005720: 6478 5d3a 2023 2074 6865 206d 6169 6e20  dx]: # the main 
-00005730: 6469 6666 6572 656e 6365 2077 6974 6820  difference with 
-00005740: 4265 6174 2050 6174 680a 2020 2020 2020  Beat Path.      
-00005750: 2020 2020 2020 2020 2020 2020 2020 6465                de
-00005760: 6665 6174 5f67 7261 7068 2e61 6464 5f77  feat_graph.add_w
-00005770: 6569 6768 7465 645f 6564 6765 735f 6672  eighted_edges_fr
-00005780: 6f6d 285b 286a 2c69 2c73 5f6d 6174 7269  om([(j,i,s_matri
-00005790: 785b 6a5f 6964 785d 5b69 5f69 6478 5d29  x[j_idx][i_idx])
-000057a0: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-000057b0: 2020 200a 2020 2020 7265 7475 726e 2064     .    return d
-000057c0: 6566 6561 745f 6772 6170 680a 0a0a 2320  efeat_graph...# 
-000057d0: 666c 6174 7465 6e20 6120 3264 206c 6973  flatten a 2d lis
-000057e0: 7420 2d20 7475 726e 2061 2032 6420 6c69  t - turn a 2d li
-000057f0: 7374 2069 6e74 6f20 6120 7369 6e67 6c65  st into a single
-00005800: 206c 6973 7420 6f66 2069 7465 6d73 0a66   list of items.f
-00005810: 6c61 7474 656e 203d 206c 616d 6264 6120  latten = lambda 
-00005820: 6c3a 205b 6974 656d 2066 6f72 2073 7562  l: [item for sub
-00005830: 6c69 7374 2069 6e20 6c20 666f 7220 6974  list in l for it
-00005840: 656d 2069 6e20 7375 626c 6973 745d 0a0a  em in sublist]..
-00005850: 6465 6620 646f 6573 5f63 7265 6174 655f  def does_create_
-00005860: 6379 636c 6528 672c 2065 6467 6529 3a0a  cycle(g, edge):.
-00005870: 2020 2020 2727 2772 6574 7572 6e20 5472      '''return Tr
-00005880: 7565 2069 6620 6164 6469 6e67 2074 6865  ue if adding the
-00005890: 2065 6467 6520 746f 2067 2063 7265 6174   edge to g creat
-000058a0: 6520 6120 6379 636c 652e 0a20 2020 2069  e a cycle..    i
-000058b0: 7420 6973 2061 7373 756d 6564 2074 6861  t is assumed tha
-000058c0: 7420 6564 6765 2069 7320 616c 7265 6164  t edge is alread
-000058d0: 7920 696e 2067 2727 270a 2020 2020 736f  y in g'''.    so
-000058e0: 7572 6365 203d 2065 6467 655b 305d 0a20  urce = edge[0]. 
-000058f0: 2020 2074 6172 6765 7420 3d20 6564 6765     target = edge
-00005900: 5b31 5d0a 2020 2020 666f 7220 6e20 696e  [1].    for n in
-00005910: 2067 2e70 7265 6465 6365 7373 6f72 7328   g.predecessors(
-00005920: 736f 7572 6365 293a 0a20 2020 2020 2020  source):.       
-00005930: 2069 6620 6e78 2e68 6173 5f70 6174 6828   if nx.has_path(
-00005940: 672c 2074 6172 6765 742c 206e 293a 200a  g, target, n): .
-00005950: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00005960: 726e 2054 7275 650a 2020 2020 7265 7475  rn True.    retu
-00005970: 726e 2046 616c 7365 0a0a 0a0a 6465 6620  rn False....def 
-00005980: 706f 7765 7273 6574 2869 7465 7261 626c  powerset(iterabl
-00005990: 6529 3a0a 2020 2020 2222 220a 2020 2020  e):.    """.    
-000059a0: 5265 7475 726e 2074 6865 2070 6f77 6572  Return the power
-000059b0: 7365 7420 6f66 2060 6069 7465 7261 626c  set of ``iterabl
-000059c0: 6560 600a 0a20 2020 2070 6f77 6572 7365  e``..    powerse
-000059d0: 7428 5b31 2c32 2c33 5d29 202d 2d3e 2028  t([1,2,3]) --> (
-000059e0: 2920 2831 2c29 2028 322c 2920 2833 2c29  ) (1,) (2,) (3,)
-000059f0: 2028 312c 3229 2028 312c 3329 2028 322c   (1,2) (1,3) (2,
-00005a00: 3329 2028 312c 322c 3329 0a20 2020 2022  3) (1,2,3).    "
-00005a10: 2222 0a20 2020 2073 203d 206c 6973 7428  "".    s = list(
-00005a20: 6974 6572 6162 6c65 290a 2020 2020 7265  iterable).    re
-00005a30: 7475 726e 2063 6861 696e 2e66 726f 6d5f  turn chain.from_
-00005a40: 6974 6572 6162 6c65 2863 6f6d 6269 6e61  iterable(combina
-00005a50: 7469 6f6e 7328 732c 2072 2920 666f 7220  tions(s, r) for 
-00005a60: 7220 696e 2072 616e 6765 286c 656e 2873  r in range(len(s
-00005a70: 292b 3129 290a 0a0a 6465 6620 6973 5f73  )+1))...def is_s
-00005a80: 7461 636b 2865 6461 7461 2c20 6361 6e64  tack(edata, cand
-00005a90: 5f6c 6973 742c 2063 7572 725f 6361 6e64  _list, curr_cand
-00005aa0: 733d 4e6f 6e65 293a 200a 2020 2020 2222  s=None): .    ""
-00005ab0: 220a 2020 2020 4120 2a2a 7374 6163 6b2a  ".    A **stack*
-00005ac0: 2a20 6973 2061 206c 696e 6561 7220 6f72  * is a linear or
-00005ad0: 6465 7220 3a6d 6174 683a 604c 6020 6f6e  der :math:`L` on
-00005ae0: 2074 6865 2063 616e 6469 6461 7465 2073   the candidate s
-00005af0: 7563 6820 7468 6174 2066 6f72 2061 6c6c  uch that for all
-00005b00: 2063 616e 6469 6461 7465 7320 3a6d 6174   candidates :mat
-00005b10: 683a 6061 6020 616e 6420 3a6d 6174 683a  h:`a` and :math:
-00005b20: 6062 602c 2069 6620 3a6d 6174 683a 6061  `b`, if :math:`a
-00005b30: 4c62 602c 2074 6865 6e20 7468 6572 6520  Lb`, then there 
-00005b40: 6172 6520 6469 7374 696e 6374 2063 616e  are distinct can
-00005b50: 6469 6461 7465 7320 3a6d 6174 683a 6078  didates :math:`x
-00005b60: 5f31 2c5c 646f 7473 2c78 5f6e 6020 7769  _1,\dots,x_n` wi
-00005b70: 7468 203a 6d61 7468 3a60 785f 313d 6160  th :math:`x_1=a`
-00005b80: 2061 6e64 203a 6d61 7468 3a60 785f 6e3d   and :math:`x_n=
-00005b90: 6260 2073 7563 6820 7468 6174 203a 6d61  b` such that :ma
-00005ba0: 7468 3a60 785f 6920 4c20 785f 7b69 2b31  th:`x_i L x_{i+1
-00005bb0: 7d60 2061 6e64 2066 6f72 2061 6c6c 203a  }` and for all :
-00005bc0: 6d61 7468 3a60 695c 696e 205c 7b31 2c5c  math:`i\in \{1,\
-00005bd0: 646f 7473 2c20 6e2d 315c 7d60 2c20 7468  dots, n-1\}`, th
-00005be0: 6520 6d61 7267 696e 206f 6620 3a6d 6174  e margin of :mat
-00005bf0: 683a 6078 5f31 6020 6f76 6572 203a 6d61  h:`x_1` over :ma
-00005c00: 7468 3a60 785f 7b69 2b31 7d60 2069 7320  th:`x_{i+1}` is 
-00005c10: 6772 6561 7465 7220 7468 616e 206f 7220  greater than or 
-00005c20: 6571 7561 6c20 746f 2074 6865 206d 6172  equal to the mar
-00005c30: 6769 6e20 6f66 203a 6d61 7468 3a60 6260  gin of :math:`b`
-00005c40: 206f 7665 7220 3a6d 6174 683a 6061 602e   over :math:`a`.
-00005c50: 0a0a 2020 2020 5468 6973 2064 6566 696e  ..    This defin
-00005c60: 6974 696f 6e20 6973 2064 7565 2074 6f20  ition is due to 
-00005c70: 5a61 7669 7374 2061 6e64 2054 6964 656d  Zavist and Tidem
-00005c80: 616e 2031 3938 392c 2061 6e64 2069 7320  an 1989, and is 
-00005c90: 7573 6564 2061 7320 616e 2061 6c74 6572  used as an alter
-00005ca0: 6e61 7469 7665 2063 6861 7261 6374 6572  native character
-00005cb0: 697a 6174 696f 6e20 6f66 2052 616e 6b65  ization of Ranke
-00005cc0: 6420 5061 6972 733a 203a 6d61 7468 3a60  d Pairs: :math:`
-00005cd0: 6160 2069 7320 6120 5261 6e6b 6564 2050  a` is a Ranked P
-00005ce0: 6169 7273 2077 696e 6e65 7220 6966 2061  airs winner if a
-00005cf0: 6e64 206f 6e6c 7920 6966 203a 6d61 7468  nd only if :math
-00005d00: 3a60 6160 2069 7320 7468 6520 6d61 7869  :`a` is the maxi
-00005d10: 6d75 6d20 656c 656d 656e 7420 6f66 2073  mum element of s
-00005d20: 6f6d 6520 7374 6163 6b2e 200a 0a20 2020  ome stack. ..   
-00005d30: 2041 7267 733a 0a20 2020 2020 2020 2065   Args:.        e
-00005d40: 6461 7461 2028 5072 6f66 696c 652c 2050  data (Profile, P
-00005d50: 726f 6669 6c65 5769 7468 5469 6573 2c20  rofileWithTies, 
-00005d60: 4d61 7267 696e 4772 6170 6829 3a20 416e  MarginGraph): An
-00005d70: 7920 656c 6563 7469 6f6e 2064 6174 6120  y election data 
-00005d80: 7468 6174 2068 6173 2061 2060 6d61 7267  that has a `marg
-00005d90: 696e 6020 6d65 7468 6f64 2e20 0a20 2020  in` method. .   
-00005da0: 2020 2020 2063 616e 645f 6c69 7374 2028       cand_list (
-00005db0: 6c69 7374 293a 2054 6865 206c 6973 7420  list): The list 
-00005dc0: 6f66 2063 616e 6469 6461 7465 7320 7468  of candidates th
-00005dd0: 6174 206d 6179 2062 6520 6120 7374 6163  at may be a stac
-00005de0: 6b0a 2020 2020 2020 2020 6375 7272 5f63  k.        curr_c
-00005df0: 616e 6473 2028 4c69 7374 5b69 6e74 5d2c  ands (List[int],
-00005e00: 206f 7074 696f 6e61 6c29 3a20 4966 2073   optional): If s
-00005e10: 6574 2c20 7468 656e 2066 696e 6420 7468  et, then find th
-00005e20: 6520 7769 6e6e 6572 7320 666f 7220 7468  e winners for th
-00005e30: 6520 7072 6f66 696c 6520 7265 7374 7269  e profile restri
-00005e40: 6374 6564 2074 6f20 7468 6520 6361 6e64  cted to the cand
-00005e50: 6964 6174 6573 2069 6e20 6060 6375 7272  idates in ``curr
-00005e60: 5f63 616e 6473 6060 0a0a 2020 2020 5265  _cands``..    Re
-00005e70: 7475 726e 733a 200a 2020 2020 2020 2020  turns: .        
-00005e80: 5472 7565 2069 6620 6060 6361 6e64 5f6c  True if ``cand_l
-00005e90: 6973 7460 6020 6973 2061 2073 7461 636b  ist`` is a stack
-00005ea0: 2061 6e64 2046 616c 7365 206f 7468 6572   and False other
-00005eb0: 7769 7365 0a0a 2020 2020 3a45 7861 6d70  wise..    :Examp
-00005ec0: 6c65 3a20 0a20 2020 200a 2020 2020 2e2e  le: .    .    ..
-00005ed0: 2070 6c6f 743a 3a20 206d 6172 6769 6e5f   plot::  margin_
-00005ee0: 6772 6170 6873 5f65 7861 6d70 6c65 732f  graphs_examples/
-00005ef0: 6d67 5f65 785f 7270 5f73 7461 636b 732e  mg_ex_rp_stacks.
-00005f00: 7079 0a20 2020 2020 2020 203a 636f 6e74  py.        :cont
-00005f10: 6578 743a 2072 6573 6574 2020 0a20 2020  ext: reset  .   
-00005f20: 2020 2020 203a 696e 636c 7564 652d 736f       :include-so
-00005f30: 7572 6365 3a20 5472 7565 0a0a 0a20 2020  urce: True...   
-00005f40: 202e 2e20 6578 6563 5f63 6f64 653a 3a0a   .. exec_code::.
-00005f50: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00005f60: 2066 726f 6d20 7072 6566 5f76 6f74 696e   from pref_votin
-00005f70: 672e 7765 6967 6874 6564 5f6d 616a 6f72  g.weighted_major
-00005f80: 6974 795f 6772 6170 6873 2069 6d70 6f72  ity_graphs impor
-00005f90: 7420 4d61 7267 696e 4772 6170 680a 2020  t MarginGraph.  
-00005fa0: 2020 2020 2020 6672 6f6d 2070 7265 665f        from pref_
-00005fb0: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
-00005fc0: 7365 645f 6d65 7468 6f64 7320 696d 706f  sed_methods impo
-00005fd0: 7274 2069 735f 7374 6163 6b0a 2020 2020  rt is_stack.    
-00005fe0: 2020 2020 6672 6f6d 2069 7465 7274 6f6f      from itertoo
-00005ff0: 6c73 2069 6d70 6f72 7420 7065 726d 7574  ls import permut
-00006000: 6174 696f 6e73 0a20 2020 2020 2020 200a  ations.        .
-00006010: 2020 2020 2020 2020 6d67 203d 204d 6172          mg = Mar
-00006020: 6769 6e47 7261 7068 285b 302c 2031 2c20  ginGraph([0, 1, 
-00006030: 325d 2c20 5b28 302c 2031 2c20 3229 2c20  2], [(0, 1, 2), 
-00006040: 2831 2c20 322c 2034 292c 2028 322c 2030  (1, 2, 4), (2, 0
-00006050: 2c20 3229 5d29 0a20 2020 2020 2020 200a  , 2)]).        .
-00006060: 2020 2020 2020 2020 666f 7220 636c 6973          for clis
-00006070: 7420 696e 2070 6572 6d75 7461 7469 6f6e  t in permutation
-00006080: 7328 6d67 2e63 616e 6469 6461 7465 7329  s(mg.candidates)
-00006090: 3a20 0a20 2020 2020 2020 2020 2020 2070  : .            p
-000060a0: 7269 6e74 2866 227b 636c 6973 747d 207b  rint(f"{clist} {
-000060b0: 2769 7327 2069 6620 6973 5f73 7461 636b  'is' if is_stack
-000060c0: 286d 672c 2063 6c69 7374 2920 656c 7365  (mg, clist) else
-000060d0: 2027 6973 206e 6f74 277d 2061 2073 7461   'is not'} a sta
-000060e0: 636b 2229 0a20 2020 2020 2020 2020 2020  ck").           
-000060f0: 200a 2020 2020 2222 220a 2020 2020 0a20   .    """.    . 
-00006100: 2020 2063 616e 6469 6461 7465 7320 3d20     candidates = 
-00006110: 6375 7272 5f63 616e 6473 2069 6620 6375  curr_cands if cu
-00006120: 7272 5f63 616e 6473 2069 7320 6e6f 7420  rr_cands is not 
-00006130: 4e6f 6e65 2065 6c73 6520 6564 6174 612e  None else edata.
-00006140: 6361 6e64 6964 6174 6573 0a20 2020 2063  candidates.    c
-00006150: 616e 645f 7061 6972 7320 3d20 5b28 612c  and_pairs = [(a,
-00006160: 2062 2920 6966 2063 616e 645f 6c69 7374   b) if cand_list
-00006170: 2e69 6e64 6578 2861 2920 3c20 6361 6e64  .index(a) < cand
-00006180: 5f6c 6973 742e 696e 6465 7828 6229 2065  _list.index(b) e
-00006190: 6c73 6520 2862 2c20 6129 2066 6f72 2061  lse (b, a) for a
-000061a0: 2c20 6220 696e 2063 6f6d 6269 6e61 7469  , b in combinati
-000061b0: 6f6e 7328 6361 6e64 6964 6174 6573 2c20  ons(candidates, 
-000061c0: 3229 5d0a 2020 2020 2020 2020 0a20 2020  2)].        .   
-000061d0: 2066 6f72 2061 2c20 6220 696e 2063 616e   for a, b in can
-000061e0: 645f 7061 6972 733a 0a20 2020 2020 2020  d_pairs:.       
-000061f0: 206f 7468 6572 5f63 616e 6473 203d 205b   other_cands = [
-00006200: 6320 666f 7220 6320 696e 2063 616e 6469  c for c in candi
-00006210: 6461 7465 7320 6966 2063 2021 3d20 6120  dates if c != a 
-00006220: 616e 6420 6320 213d 2062 5d0a 2020 2020  and c != b].    
-00006230: 2020 2020 666f 756e 645f 7061 7468 203d      found_path =
-00006240: 2046 616c 7365 0a20 2020 2020 2020 200a   False.        .
-00006250: 2020 2020 2020 2020 7375 626c 6973 7420          sublist 
-00006260: 3d20 6361 6e64 5f6c 6973 745b 6361 6e64  = cand_list[cand
-00006270: 5f6c 6973 742e 696e 6465 7828 6129 202b  _list.index(a) +
-00006280: 2031 3a63 616e 645f 6c69 7374 2e69 6e64   1:cand_list.ind
-00006290: 6578 2862 295d 0a20 2020 2020 2020 200a  ex(b)].        .
-000062a0: 2020 2020 2020 2020 666f 7220 696e 6469          for indi
-000062b0: 6365 7320 696e 2070 6f77 6572 7365 7428  ces in powerset(
-000062c0: 7261 6e67 6528 6c65 6e28 7375 626c 6973  range(len(sublis
-000062d0: 7429 2929 3a20 0a20 2020 2020 2020 2020  t))): .         
-000062e0: 2020 200a 2020 2020 2020 2020 2020 2020     .            
-000062f0: 7061 7468 203d 205b 615d 202b 205b 7375  path = [a] + [su
-00006300: 626c 6973 745b 695d 2066 6f72 2069 2069  blist[i] for i i
-00006310: 6e20 736f 7274 6564 2869 6e64 6963 6573  n sorted(indices
-00006320: 295d 202b 205b 625d 0a20 2020 2020 2020  )] + [b].       
-00006330: 2020 2020 206d 6172 6769 6e73 203d 205b       margins = [
-00006340: 6564 6174 612e 6d61 7267 696e 2878 692c  edata.margin(xi,
-00006350: 2070 6174 685b 6920 2b20 315d 2920 666f   path[i + 1]) fo
-00006360: 7220 692c 2078 6920 696e 2065 6e75 6d65  r i, xi in enume
-00006370: 7261 7465 2870 6174 685b 303a 2d31 5d29  rate(path[0:-1])
-00006380: 5d0a 2020 2020 2020 2020 2020 2020 6966  ].            if
-00006390: 2061 6c6c 285b 6361 6e64 5f6c 6973 742e   all([cand_list.
-000063a0: 696e 6465 7828 7869 2920 3c20 6361 6e64  index(xi) < cand
-000063b0: 5f6c 6973 742e 696e 6465 7828 7061 7468  _list.index(path
-000063c0: 5b69 2b31 5d29 2066 6f72 2069 2c20 7869  [i+1]) for i, xi
-000063d0: 2069 6e20 656e 756d 6572 6174 6528 7061   in enumerate(pa
-000063e0: 7468 5b30 3a2d 315d 295d 2920 616e 6420  th[0:-1])]) and 
-000063f0: 616c 6c28 5b6d 203e 3d20 6564 6174 612e  all([m >= edata.
-00006400: 6d61 7267 696e 2862 2c20 6129 2066 6f72  margin(b, a) for
-00006410: 206d 2069 6e20 6d61 7267 696e 735d 293a   m in margins]):
-00006420: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-00006430: 2020 666f 756e 645f 7061 7468 203d 2054    found_path = T
-00006440: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
-00006450: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
-00006460: 2020 6966 206e 6f74 2066 6f75 6e64 5f70    if not found_p
-00006470: 6174 683a 200a 2020 2020 2020 2020 2020  ath: .          
-00006480: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
-00006490: 2020 2072 6574 7572 6e20 5472 7565 0a0a     return True..
-000064a0: 6465 6620 5f72 616e 6b65 645f 7061 6972  def _ranked_pair
-000064b0: 735f 6672 6f6d 5f73 7461 636b 7328 6564  s_from_stacks(ed
-000064c0: 6174 612c 2063 7572 725f 6361 6e64 7320  ata, curr_cands 
-000064d0: 3d20 4e6f 6e65 293a 200a 2020 2020 2222  = None): .    ""
-000064e0: 2246 696e 6420 7468 6520 5261 6e6b 6564  "Find the Ranked
-000064f0: 2050 6169 7273 2077 696e 6e65 7273 2062   Pairs winners b
-00006500: 7920 6974 6572 6174 696e 6720 6f76 6572  y iterating over
-00006510: 2061 6c6c 2070 6572 6d75 7461 7469 6f6e   all permutation
-00006520: 7320 6f66 2063 616e 6469 6461 7465 7320  s of candidates 
-00006530: 2872 6573 7472 6963 7465 6420 746f 2060  (restricted to `
-00006540: 6063 7572 725f 6361 6e64 7360 6020 6966  `curr_cands`` if
-00006550: 206e 6f74 204e 6f6e 6529 2c20 616e 6420   not None), and 
-00006560: 6368 6563 6b69 6e67 2069 6620 7468 6520  checking if the 
-00006570: 6c69 7374 2069 7320 6120 7374 6163 6b2e  list is a stack.
-00006580: 200a 0a20 2020 2041 7267 733a 0a20 2020   ..    Args:.   
-00006590: 2020 2020 2065 6461 7461 2028 5072 6f66       edata (Prof
-000065a0: 696c 652c 2050 726f 6669 6c65 5769 7468  ile, ProfileWith
-000065b0: 5469 6573 2c20 4d61 7267 696e 4772 6170  Ties, MarginGrap
-000065c0: 6829 3a20 416e 7920 656c 6563 7469 6f6e  h): Any election
-000065d0: 2064 6174 6120 7468 6174 2068 6173 2061   data that has a
-000065e0: 2060 6d61 7267 696e 6020 6d65 7468 6f64   `margin` method
-000065f0: 2e20 0a20 2020 2020 2020 2063 7572 725f  . .        curr_
-00006600: 6361 6e64 7320 284c 6973 745b 696e 745d  cands (List[int]
-00006610: 2c20 6f70 7469 6f6e 616c 293a 2049 6620  , optional): If 
-00006620: 7365 742c 2074 6865 6e20 6669 6e64 2074  set, then find t
-00006630: 6865 2077 696e 6e65 7273 2066 6f72 2074  he winners for t
-00006640: 6865 2070 726f 6669 6c65 2072 6573 7472  he profile restr
-00006650: 6963 7465 6420 746f 2074 6865 2063 616e  icted to the can
-00006660: 6469 6461 7465 7320 696e 2060 6063 7572  didates in ``cur
-00006670: 725f 6361 6e64 7360 600a 0a20 2020 2052  r_cands``..    R
-00006680: 6574 7572 6e73 3a20 0a20 2020 2020 2020  eturns: .       
-00006690: 2041 2073 6f72 7465 6420 6c69 7374 206f   A sorted list o
-000066a0: 6620 6361 6e64 6964 6174 6573 2e20 0a0a  f candidates. ..
-000066b0: 2020 2020 2e2e 2073 6565 616c 736f 3a3a      .. seealso::
-000066c0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000066d0: 2020 3a6d 6574 683a 6070 7265 665f 766f    :meth:`pref_vo
-000066e0: 7469 6e67 2e6d 6172 6769 6e5f 6261 7365  ting.margin_base
-000066f0: 645f 6d65 7468 6f64 732e 6973 5f73 7461  d_methods.is_sta
-00006700: 636b 600a 0a0a 2020 2020 2222 2220 2020  ck`...    """   
-00006710: 200a 0a20 2020 2063 616e 6469 6461 7465   ..    candidate
-00006720: 7320 3d20 6375 7272 5f63 616e 6473 2069  s = curr_cands i
-00006730: 6620 6375 7272 5f63 616e 6473 2069 7320  f curr_cands is 
-00006740: 6e6f 7420 4e6f 6e65 2065 6c73 6520 6564  not None else ed
-00006750: 6174 612e 6361 6e64 6964 6174 6573 0a20  ata.candidates. 
-00006760: 2020 2077 696e 6e65 7273 203d 206c 6973     winners = lis
-00006770: 7428 290a 2020 2020 666f 7220 636c 6973  t().    for clis
-00006780: 7420 696e 2070 6572 6d75 7461 7469 6f6e  t in permutation
-00006790: 7328 6361 6e64 6964 6174 6573 293a 200a  s(candidates): .
-000067a0: 2020 2020 2020 2020 6973 7374 6163 6b20          isstack 
-000067b0: 3d20 6973 5f73 7461 636b 2865 6461 7461  = is_stack(edata
-000067c0: 2c20 636c 6973 742c 2063 7572 725f 6361  , clist, curr_ca
-000067d0: 6e64 7320 3d20 6375 7272 5f63 616e 6473  nds = curr_cands
-000067e0: 290a 2020 2020 2020 2020 6966 2069 7373  ).        if iss
-000067f0: 7461 636b 3a20 0a20 2020 2020 2020 2020  tack: .         
-00006800: 2020 2077 696e 6e65 7273 2e61 7070 656e     winners.appen
-00006810: 6428 636c 6973 745b 305d 290a 2020 2020  d(clist[0]).    
-00006820: 2020 2020 2020 2020 0a20 2020 2072 6574          .    ret
-00006830: 7572 6e20 736f 7274 6564 286c 6973 7428  urn sorted(list(
-00006840: 7365 7428 7769 6e6e 6572 7329 2929 0a0a  set(winners)))..
-00006850: 6465 6620 5f72 616e 6b65 645f 7061 6972  def _ranked_pair
-00006860: 735f 6261 7369 6328 0a20 2020 2065 6461  s_basic(.    eda
-00006870: 7461 2c20 0a20 2020 2063 7572 725f 6361  ta, .    curr_ca
-00006880: 6e64 7320 3d20 4e6f 6e65 2c20 0a20 2020  nds = None, .   
-00006890: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-000068a0: 6f6e 203d 204e 6f6e 6529 3a20 2020 0a20  on = None):   . 
-000068b0: 2020 2022 2222 416e 2069 6d70 6c65 6d65     """An impleme
-000068c0: 6e74 6174 696f 6e20 6f66 2052 616e 6b65  ntation of Ranke
-000068d0: 6420 5061 6972 7320 7468 6174 2075 7365  d Pairs that use
-000068e0: 7320 6120 6261 7369 6320 616c 676f 7269  s a basic algori
-000068f0: 7468 6d2e 200a 0a20 2020 2041 7267 733a  thm. ..    Args:
-00006900: 0a20 2020 2020 2020 2065 6461 7461 2028  .        edata (
-00006910: 5072 6f66 696c 652c 2050 726f 6669 6c65  Profile, Profile
-00006920: 5769 7468 5469 6573 2c20 4d61 7267 696e  WithTies, Margin
-00006930: 4772 6170 6829 3a20 416e 7920 656c 6563  Graph): Any elec
-00006940: 7469 6f6e 2064 6174 6120 7468 6174 2068  tion data that h
-00006950: 6173 2061 2060 6d61 7267 696e 6020 6d65  as a `margin` me
-00006960: 7468 6f64 2e20 0a20 2020 2020 2020 2063  thod. .        c
-00006970: 7572 725f 6361 6e64 7320 284c 6973 745b  urr_cands (List[
-00006980: 696e 745d 2c20 6f70 7469 6f6e 616c 293a  int], optional):
-00006990: 2049 6620 7365 742c 2074 6865 6e20 6669   If set, then fi
-000069a0: 6e64 2074 6865 2077 696e 6e65 7273 2066  nd the winners f
-000069b0: 6f72 2074 6865 2070 726f 6669 6c65 2072  or the profile r
-000069c0: 6573 7472 6963 7465 6420 746f 2074 6865  estricted to the
-000069d0: 2063 616e 6469 6461 7465 7320 696e 2060   candidates in `
-000069e0: 6063 7572 725f 6361 6e64 7360 600a 0a20  `curr_cands``.. 
-000069f0: 2020 2052 6574 7572 6e73 3a20 0a20 2020     Returns: .   
-00006a00: 2020 2020 2041 2073 6f72 7465 6420 6c69       A sorted li
-00006a10: 7374 206f 6620 6361 6e64 6964 6174 6573  st of candidates
-00006a20: 2e20 0a0a 2020 2020 2222 220a 2020 2020  . ..    """.    
-00006a30: 6361 6e64 6964 6174 6573 203d 2065 6461  candidates = eda
-00006a40: 7461 2e63 616e 6469 6461 7465 7320 6966  ta.candidates if
-00006a50: 2063 7572 725f 6361 6e64 7320 6973 204e   curr_cands is N
-00006a60: 6f6e 6520 656c 7365 2063 7572 725f 6361  one else curr_ca
-00006a70: 6e64 7320 0a20 2020 2063 6964 785f 746f  nds .    cidx_to
-00006a80: 5f63 616e 6420 3d20 7b63 6964 783a 2063  _cand = {cidx: c
-00006a90: 2066 6f72 2063 6964 782c 2063 2069 6e20   for cidx, c in 
-00006aa0: 656e 756d 6572 6174 6528 6361 6e64 6964  enumerate(candid
-00006ab0: 6174 6573 297d 2020 0a20 2020 2063 616e  ates)}  .    can
-00006ac0: 645f 746f 5f63 6964 7820 3d20 7b63 3a20  d_to_cidx = {c: 
-00006ad0: 6369 6478 2066 6f72 2063 6964 782c 2063  cidx for cidx, c
-00006ae0: 2069 6e20 656e 756d 6572 6174 6528 6361   in enumerate(ca
-00006af0: 6e64 6964 6174 6573 297d 2020 0a20 2020  ndidates)}  .   
-00006b00: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-00006b10: 6f6e 203d 2065 6461 7461 2e6d 6172 6769  on = edata.margi
-00006b20: 6e20 6966 2073 7472 656e 6774 685f 6675  n if strength_fu
-00006b30: 6e63 7469 6f6e 2069 7320 4e6f 6e65 2065  nction is None e
-00006b40: 6c73 6520 7374 7265 6e67 7468 5f66 756e  lse strength_fun
-00006b50: 6374 696f 6e20 2020 200a 0a20 2020 2063  ction    ..    c
-00006b60: 7720 3d20 6564 6174 612e 636f 6e64 6f72  w = edata.condor
-00006b70: 6365 745f 7769 6e6e 6572 2863 7572 725f  cet_winner(curr_
-00006b80: 6361 6e64 733d 6375 7272 5f63 616e 6473  cands=curr_cands
-00006b90: 290a 2020 2020 2320 5261 6e6b 6564 2050  ).    # Ranked P
-00006ba0: 6169 7273 2069 7320 436f 6e64 6f72 6365  airs is Condorce
-00006bb0: 7420 636f 6e73 6973 7465 6e74 2c20 736f  t consistent, so
-00006bc0: 2073 696d 706c 7920 7265 7475 726e 2074   simply return t
-00006bd0: 6865 2043 6f6e 646f 7263 6574 2077 696e  he Condorcet win
-00006be0: 6e65 7220 6966 2065 7869 7374 730a 2020  ner if exists.  
-00006bf0: 2020 6966 2063 7720 6973 206e 6f74 204e    if cw is not N
-00006c00: 6f6e 653a 200a 2020 2020 2020 2020 7769  one: .        wi
-00006c10: 6e6e 6572 7320 3d20 5b63 775d 0a20 2020  nners = [cw].   
-00006c20: 2065 6c73 653a 0a20 2020 2020 2020 2077   else:.        w
-00006c30: 5f65 6467 6573 203d 205b 2863 312c 2063  _edges = [(c1, c
-00006c40: 322c 2073 7472 656e 6774 685f 6675 6e63  2, strength_func
-00006c50: 7469 6f6e 2863 312c 2063 3229 2920 666f  tion(c1, c2)) fo
-00006c60: 7220 6331 2069 6e20 6361 6e64 6964 6174  r c1 in candidat
-00006c70: 6573 2066 6f72 2063 3220 696e 2063 616e  es for c2 in can
-00006c80: 6469 6461 7465 7320 0a20 2020 2020 2020  didates .       
-00006c90: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00006ca0: 3120 213d 2063 3220 616e 6420 2865 6461  1 != c2 and (eda
-00006cb0: 7461 2e6d 616a 6f72 6974 795f 7072 6566  ta.majority_pref
-00006cc0: 6572 7328 6331 2c20 6332 2920 6f72 2065  ers(c1, c2) or e
-00006cd0: 6461 7461 2e69 735f 7469 6564 2863 312c  data.is_tied(c1,
-00006ce0: 2063 3229 295d 0a20 2020 2020 2020 2077   c2))].        w
-00006cf0: 696e 6e65 7273 203d 206c 6973 7428 2920  inners = list() 
-00006d00: 2020 0a20 2020 2020 2020 2069 6620 6c65    .        if le
-00006d10: 6e28 775f 6564 6765 7329 203e 2030 3a20  n(w_edges) > 0: 
-00006d20: 2020 2020 2020 2020 200a 2020 2020 2020           .      
-00006d30: 2020 2020 2020 7374 7265 6e67 7468 7320        strengths 
-00006d40: 3d20 736f 7274 6564 286c 6973 7428 7365  = sorted(list(se
-00006d50: 7428 5b65 5b32 5d20 666f 7220 6520 696e  t([e[2] for e in
-00006d60: 2077 5f65 6467 6573 5d29 292c 2072 6576   w_edges])), rev
-00006d70: 6572 7365 3d54 7275 6529 0a20 2020 2020  erse=True).     
-00006d80: 2020 2020 2020 2073 6f72 7465 645f 6564         sorted_ed
-00006d90: 6765 7320 3d20 5b5b 6520 666f 7220 6520  ges = [[e for e 
-00006da0: 696e 2077 5f65 6467 6573 2069 6620 655b  in w_edges if e[
-00006db0: 325d 203d 3d20 735d 2066 6f72 2073 2069  2] == s] for s i
-00006dc0: 6e20 7374 7265 6e67 7468 735d 0a20 2020  n strengths].   
-00006dd0: 2020 2020 2020 2020 2074 6273 203d 2070           tbs = p
-00006de0: 726f 6475 6374 282a 5b70 6572 6d75 7461  roduct(*[permuta
-00006df0: 7469 6f6e 7328 6564 6765 7329 2066 6f72  tions(edges) for
-00006e00: 2065 6467 6573 2069 6e20 736f 7274 6564   edges in sorted
-00006e10: 5f65 6467 6573 5d29 0a20 2020 2020 2020  _edges]).       
-00006e20: 2020 2020 2066 6f72 2074 6220 696e 2074       for tb in t
-00006e30: 6273 3a0a 2020 2020 2020 2020 2020 2020  bs:.            
-00006e40: 2020 2020 6564 6765 7320 3d20 666c 6174      edges = flat
-00006e50: 7465 6e28 7462 290a 2020 2020 2020 2020  ten(tb).        
-00006e60: 2020 2020 2020 2020 7270 5f64 6566 6561          rp_defea
-00006e70: 7420 3d20 5350 4f28 6c65 6e28 6361 6e64  t = SPO(len(cand
-00006e80: 6964 6174 6573 2929 0a20 2020 2020 2020  idates)).       
-00006e90: 2020 2020 2020 2020 2066 6f72 2065 302c           for e0,
-00006ea0: 6531 2c73 2069 6e20 6564 6765 733a 200a  e1,s in edges: .
-00006eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ec0: 2020 2020 6966 206e 6f74 2072 705f 6465      if not rp_de
-00006ed0: 6665 6174 2e50 5b63 616e 645f 746f 5f63  feat.P[cand_to_c
-00006ee0: 6964 785b 6531 5d5d 5b63 616e 645f 746f  idx[e1]][cand_to
-00006ef0: 5f63 6964 785b 6530 5d5d 3a0a 2020 2020  _cidx[e0]]:.    
-00006f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f10: 2020 2020 7270 5f64 6566 6561 742e 6164      rp_defeat.ad
-00006f20: 6428 6361 6e64 5f74 6f5f 6369 6478 5b65  d(cand_to_cidx[e
-00006f30: 305d 2c63 616e 645f 746f 5f63 6964 785b  0],cand_to_cidx[
-00006f40: 6531 5d29 0a20 2020 2020 2020 2020 2020  e1]).           
-00006f50: 2020 2020 2077 696e 6e65 7273 2e61 7070       winners.app
-00006f60: 656e 6428 6369 6478 5f74 6f5f 6361 6e64  end(cidx_to_cand
-00006f70: 5b72 705f 6465 6665 6174 2e69 6e69 7469  [rp_defeat.initi
-00006f80: 616c 5f65 6c65 6d65 6e74 7328 295b 305d  al_elements()[0]
-00006f90: 5d29 0a20 2020 2020 2020 2065 6c73 653a  ]).        else:
-00006fa0: 200a 2020 2020 2020 2020 2020 2020 7769   .            wi
-00006fb0: 6e6e 6572 7320 3d20 6361 6e64 6964 6174  nners = candidat
-00006fc0: 6573 0a20 2020 2072 6574 7572 6e20 736f  es.    return so
-00006fd0: 7274 6564 286c 6973 7428 7365 7428 7769  rted(list(set(wi
-00006fe0: 6e6e 6572 7329 2929 0a0a 0a40 766d 286e  nners)))...@vm(n
-00006ff0: 616d 653d 2252 616e 6b65 6420 5061 6972  ame="Ranked Pair
-00007000: 7322 290a 6465 6620 7261 6e6b 6564 5f70  s").def ranked_p
-00007010: 6169 7273 280a 2020 2020 6564 6174 612c  airs(.    edata,
-00007020: 200a 2020 2020 6375 7272 5f63 616e 6473   .    curr_cands
-00007030: 3d4e 6f6e 652c 200a 2020 2020 7374 7265  =None, .    stre
-00007040: 6e67 7468 5f66 756e 6374 696f 6e3d 4e6f  ngth_function=No
-00007050: 6e65 2c20 0a20 2020 2061 6c67 6f72 6974  ne, .    algorit
-00007060: 686d 3d27 6261 7369 6327 293a 2020 200a  hm='basic'):   .
-00007070: 2020 2020 2222 220a 2020 2020 4f72 6465      """.    Orde
-00007080: 7220 7468 6520 6564 6765 7320 696e 2074  r the edges in t
-00007090: 6865 206d 6172 6769 6e20 6772 6170 6820  he margin graph 
-000070a0: 6672 6f6d 206c 6172 6765 7374 2074 6f20  from largest to 
-000070b0: 736d 616c 6c65 7374 2061 6e64 206c 6f63  smallest and loc
-000070c0: 6b20 7468 656d 2069 6e20 696e 2074 6861  k them in in tha
-000070d0: 7420 6f72 6465 722c 2073 6b69 7070 696e  t order, skippin
-000070e0: 6720 6564 6765 7320 7468 6174 2063 7265  g edges that cre
-000070f0: 6174 6520 6120 6379 636c 652e 2020 4966  ate a cycle.  If
-00007100: 2074 6865 7265 2061 7265 2074 6965 7320   there are ties 
-00007110: 696e 2074 6865 206d 6172 6769 6e73 2c20  in the margins, 
-00007120: 6272 6561 6b20 7468 6520 7469 6573 2075  break the ties u
-00007130: 7369 6e67 2061 2074 6965 2d62 7265 616b  sing a tie-break
-00007140: 696e 6720 7275 6c65 3a20 6120 6c69 6e65  ing rule: a line
-00007150: 6172 206f 7264 6572 696e 6720 6f76 6572  ar ordering over
-00007160: 2074 6865 2065 6467 6573 2e20 2020 4120   the edges.   A 
-00007170: 6361 6e64 6964 6174 6520 6973 2061 2052  candidate is a R
-00007180: 616e 6b65 6420 5061 6972 7320 7769 6e6e  anked Pairs winn
-00007190: 6572 2069 6620 6974 2077 696e 7320 6163  er if it wins ac
-000071a0: 636f 7264 696e 6720 746f 2073 6f6d 6520  cording to some 
-000071b0: 7469 652d 6272 6561 6b69 6e67 2072 756c  tie-breaking rul
-000071c0: 652e 2041 6c73 6f20 6b6e 6f77 6e20 6173  e. Also known as
-000071d0: 2054 6964 656d 616e 2773 2052 756c 652e   Tideman's Rule.
-000071e0: 0a0a 2020 2020 2e2e 2077 6172 6e69 6e67  ..    .. warning
-000071f0: 3a3a 200a 2020 2020 2020 2020 5468 6973  :: .        This
-00007200: 206d 6574 686f 6420 6361 6e20 7461 6b65   method can take
-00007210: 2061 2076 6572 7920 6c6f 6e67 2074 696d   a very long tim
-00007220: 6520 746f 2066 696e 6420 7769 6e6e 6572  e to find winner
-00007230: 732e 200a 2020 2020 2020 2020 0a20 2020  s. .        .   
-00007240: 2041 7267 733a 0a20 2020 2020 2020 2065   Args:.        e
-00007250: 6461 7461 2028 5072 6f66 696c 652c 2050  data (Profile, P
-00007260: 726f 6669 6c65 5769 7468 5469 6573 2c20  rofileWithTies, 
-00007270: 4d61 7267 696e 4772 6170 6829 3a20 416e  MarginGraph): An
-00007280: 7920 656c 6563 7469 6f6e 2064 6174 6120  y election data 
-00007290: 7468 6174 2068 6173 2061 2060 6d61 7267  that has a `marg
-000072a0: 696e 6020 6d65 7468 6f64 2e20 0a20 2020  in` method. .   
-000072b0: 2020 2020 2063 7572 725f 6361 6e64 7320       curr_cands 
-000072c0: 284c 6973 745b 696e 745d 2c20 6f70 7469  (List[int], opti
-000072d0: 6f6e 616c 293a 2049 6620 7365 742c 2074  onal): If set, t
-000072e0: 6865 6e20 6669 6e64 2074 6865 2077 696e  hen find the win
-000072f0: 6e65 7273 2066 6f72 2074 6865 2070 726f  ners for the pro
-00007300: 6669 6c65 2072 6573 7472 6963 7465 6420  file restricted 
-00007310: 746f 2074 6865 2063 616e 6469 6461 7465  to the candidate
-00007320: 7320 696e 2060 6063 7572 725f 6361 6e64  s in ``curr_cand
-00007330: 7360 600a 2020 2020 2020 2020 7374 7265  s``.        stre
-00007340: 6e67 7468 5f66 756e 6374 696f 6e20 2866  ngth_function (f
-00007350: 756e 6374 696f 6e2c 206f 7074 696f 6e61  unction, optiona
-00007360: 6c29 3a20 5468 6520 7374 7265 6e67 7468  l): The strength
-00007370: 2066 756e 6374 696f 6e20 746f 2062 6520   function to be 
-00007380: 7573 6564 2074 6f20 6361 6c63 756c 6174  used to calculat
-00007390: 6520 7468 6520 7374 7265 6e67 7468 206f  e the strength o
-000073a0: 6620 6120 7061 7468 2e20 2020 5468 6520  f a path.   The 
-000073b0: 6465 6661 756c 7420 6973 2074 6865 206d  default is the m
-000073c0: 6172 6769 6e20 6d65 7468 6f64 206f 6620  argin method of 
-000073d0: 6060 6564 6174 6160 602e 2020 2054 6869  ``edata``.   Thi
-000073e0: 7320 6f6e 6c79 206d 6174 7465 7273 2077  s only matters w
-000073f0: 6865 6e20 7468 6520 6261 6c6c 6f74 7320  hen the ballots 
-00007400: 6172 6520 6e6f 7420 6c69 6e65 6172 206f  are not linear o
-00007410: 7264 6572 732e 200a 2020 2020 2020 2020  rders. .        
-00007420: 616c 676f 7269 7468 6d20 2873 7472 2c20  algorithm (str, 
-00007430: 6f70 7469 6f6e 616c 293a 2053 7065 6369  optional): Speci
-00007440: 6679 2077 6869 6368 2061 6c67 6f72 6974  fy which algorit
-00007450: 686d 2074 6f20 7573 652e 2020 4f70 7469  hm to use.  Opti
-00007460: 6f6e 7320 6172 6520 2762 6173 6963 2720  ons are 'basic' 
-00007470: 2874 6865 2064 6566 6175 6c74 2920 616e  (the default) an
-00007480: 6420 2766 726f 6d5f 7374 6163 6b73 272e  d 'from_stacks'.
-00007490: 0a0a 2020 2020 5265 7475 726e 733a 200a  ..    Returns: .
-000074a0: 2020 2020 2020 2020 4120 736f 7274 6564          A sorted
-000074b0: 206c 6973 7420 6f66 2063 616e 6469 6461   list of candida
-000074c0: 7465 732e 200a 0a20 2020 202e 2e20 7365  tes. ..    .. se
-000074d0: 6561 6c73 6f3a 3a0a 0a20 2020 2020 2020  ealso::..       
-000074e0: 203a 6d65 7468 3a60 7072 6566 5f76 6f74   :meth:`pref_vot
-000074f0: 696e 672e 6d61 7267 696e 5f62 6173 6564  ing.margin_based
-00007500: 5f6d 6574 686f 6473 2e72 616e 6b65 645f  _methods.ranked_
-00007510: 7061 6972 735f 7769 7468 5f74 6573 7460  pairs_with_test`
-00007520: 2c20 3a6d 6574 683a 6070 7265 665f 766f  , :meth:`pref_vo
-00007530: 7469 6e67 2e6d 6172 6769 6e5f 6261 7365  ting.margin_base
-00007540: 645f 6d65 7468 6f64 732e 7261 6e6b 6564  d_methods.ranked
-00007550: 5f70 6169 7273 5f7a 7460 2c20 3a6d 6574  _pairs_zt`, :met
-00007560: 683a 6070 7265 665f 766f 7469 6e67 2e6d  h:`pref_voting.m
-00007570: 6172 6769 6e5f 6261 7365 645f 6d65 7468  argin_based_meth
-00007580: 6f64 732e 7261 6e6b 6564 5f70 6169 7273  ods.ranked_pairs
-00007590: 5f64 6566 6561 7473 600a 0a20 2020 203a  _defeats`..    :
-000075a0: 4578 616d 706c 653a 200a 0a20 2020 202e  Example: ..    .
-000075b0: 2e20 706c 6f74 3a3a 2020 6d61 7267 696e  . plot::  margin
-000075c0: 5f67 7261 7068 735f 6578 616d 706c 6573  _graphs_examples
-000075d0: 2f6d 675f 6578 5f62 705f 7270 2e70 790a  /mg_ex_bp_rp.py.
-000075e0: 2020 2020 2020 2020 3a63 6f6e 7465 7874          :context
-000075f0: 3a20 7265 7365 7420 200a 2020 2020 2020  : reset  .      
-00007600: 2020 3a69 6e63 6c75 6465 2d73 6f75 7263    :include-sourc
-00007610: 653a 2054 7275 650a 0a0a 2020 2020 2e2e  e: True...    ..
-00007620: 2063 6f64 652d 626c 6f63 6b3a 3a20 0a0a   code-block:: ..
-00007630: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
-00007640: 665f 766f 7469 6e67 2e6d 6172 6769 6e5f  f_voting.margin_
-00007650: 6261 7365 645f 6d65 7468 6f64 7320 696d  based_methods im
-00007660: 706f 7274 2072 616e 6b65 645f 7061 6972  port ranked_pair
-00007670: 730a 0a20 2020 2020 2020 2072 616e 6b65  s..        ranke
-00007680: 645f 7061 6972 732e 6469 7370 6c61 7928  d_pairs.display(
-00007690: 6d67 290a 2020 2020 2020 2020 7261 6e6b  mg).        rank
-000076a0: 6564 5f70 6169 7273 2e64 6973 706c 6179  ed_pairs.display
-000076b0: 286d 672c 2061 6c67 6f72 6974 686d 3d27  (mg, algorithm='
-000076c0: 6261 7369 6327 2920 0a20 2020 2020 2020  basic') .       
-000076d0: 2072 616e 6b65 645f 7061 6972 732e 6469   ranked_pairs.di
-000076e0: 7370 6c61 7928 6d67 2c20 616c 676f 7269  splay(mg, algori
-000076f0: 7468 6d3d 2766 726f 6d5f 7374 6163 6b73  thm='from_stacks
-00007700: 2729 2020 2020 0a0a 0a20 2020 202e 2e20  ')    ...    .. 
-00007710: 6578 6563 5f63 6f64 653a 3a20 0a20 2020  exec_code:: .   
-00007720: 2020 2020 203a 6869 6465 5f63 6f64 653a       :hide_code:
-00007730: 0a0a 2020 2020 2020 2020 6672 6f6d 2070  ..        from p
-00007740: 7265 665f 766f 7469 6e67 2e77 6569 6768  ref_voting.weigh
-00007750: 7465 645f 6d61 6a6f 7269 7479 5f67 7261  ted_majority_gra
-00007760: 7068 7320 696d 706f 7274 204d 6172 6769  phs import Margi
-00007770: 6e47 7261 7068 0a20 2020 2020 2020 2066  nGraph.        f
-00007780: 726f 6d20 7072 6566 5f76 6f74 696e 672e  rom pref_voting.
-00007790: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
-000077a0: 686f 6473 2069 6d70 6f72 7420 7261 6e6b  hods import rank
-000077b0: 6564 5f70 6169 7273 0a20 2020 2020 2020  ed_pairs.       
-000077c0: 200a 2020 2020 2020 2020 6d67 203d 204d   .        mg = M
-000077d0: 6172 6769 6e47 7261 7068 285b 302c 2031  arginGraph([0, 1
-000077e0: 2c20 322c 2033 5d2c 205b 2830 2c20 322c  , 2, 3], [(0, 2,
-000077f0: 2033 292c 2028 312c 2030 2c20 3529 2c20   3), (1, 0, 5), 
-00007800: 2832 2c20 312c 2035 292c 2028 322c 2033  (2, 1, 5), (2, 3
-00007810: 2c20 3129 2c20 2833 2c20 302c 2033 292c  , 1), (3, 0, 3),
-00007820: 2028 332c 2031 2c20 3129 5d29 0a20 2020   (3, 1, 1)]).   
-00007830: 2020 2020 200a 2020 2020 2020 2020 7261       .        ra
-00007840: 6e6b 6564 5f70 6169 7273 2e64 6973 706c  nked_pairs.displ
-00007850: 6179 286d 6729 0a20 2020 2020 2020 2072  ay(mg).        r
-00007860: 616e 6b65 645f 7061 6972 732e 6469 7370  anked_pairs.disp
-00007870: 6c61 7928 6d67 2c20 616c 676f 7269 7468  lay(mg, algorith
-00007880: 6d3d 2762 6173 6963 2729 0a20 2020 2020  m='basic').     
-00007890: 2020 2072 616e 6b65 645f 7061 6972 732e     ranked_pairs.
-000078a0: 6469 7370 6c61 7928 6d67 2c20 616c 676f  display(mg, algo
-000078b0: 7269 7468 6d3d 2766 726f 6d5f 7374 6163  rithm='from_stac
-000078c0: 6b73 2729 0a0a 2020 2020 2222 220a 0a20  ks')..    """.. 
-000078d0: 2020 2069 6620 616c 676f 7269 7468 6d20     if algorithm 
-000078e0: 3d3d 2027 6261 7369 6327 3a0a 2020 2020  == 'basic':.    
-000078f0: 2020 2020 7265 7475 726e 205f 7261 6e6b      return _rank
-00007900: 6564 5f70 6169 7273 5f62 6173 6963 2865  ed_pairs_basic(e
-00007910: 6461 7461 2c20 6375 7272 5f63 616e 6473  data, curr_cands
-00007920: 203d 2063 7572 725f 6361 6e64 732c 2073   = curr_cands, s
-00007930: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-00007940: 203d 2073 7472 656e 6774 685f 6675 6e63   = strength_func
-00007950: 7469 6f6e 290a 2020 2020 656c 6966 2061  tion).    elif a
-00007960: 6c67 6f72 6974 686d 203d 3d20 2766 726f  lgorithm == 'fro
-00007970: 6d5f 7374 6163 6b73 273a 0a20 2020 2020  m_stacks':.     
-00007980: 2020 2072 6574 7572 6e20 5f72 616e 6b65     return _ranke
-00007990: 645f 7061 6972 735f 6672 6f6d 5f73 7461  d_pairs_from_sta
-000079a0: 636b 7328 6564 6174 612c 2063 7572 725f  cks(edata, curr_
-000079b0: 6361 6e64 7320 3d20 6375 7272 5f63 616e  cands = curr_can
-000079c0: 6473 290a 2020 2020 656c 7365 3a0a 2020  ds).    else:.  
-000079d0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-000079e0: 6545 7272 6f72 2822 496e 7661 6c69 6420  eError("Invalid 
-000079f0: 616c 676f 7269 7468 6d20 7370 6563 6966  algorithm specif
-00007a00: 6965 642e 2229 0a0a 0a40 766d 286e 616d  ied.")...@vm(nam
-00007a10: 653d 2252 616e 6b65 6420 5061 6972 7322  e="Ranked Pairs"
-00007a20: 290a 6465 6620 7261 6e6b 6564 5f70 6169  ).def ranked_pai
-00007a30: 7273 5f77 6974 685f 7465 7374 280a 2020  rs_with_test(.  
-00007a40: 2020 6564 6174 612c 200a 2020 2020 6375    edata, .    cu
-00007a50: 7272 5f63 616e 6473 3d4e 6f6e 652c 200a  rr_cands=None, .
-00007a60: 2020 2020 7374 7265 6e67 7468 5f66 756e      strength_fun
-00007a70: 6374 696f 6e3d 4e6f 6e65 293a 2020 200a  ction=None):   .
-00007a80: 2020 2020 2222 2246 696e 6420 7468 6520      """Find the 
-00007a90: 5261 6e6b 6564 2050 6169 7273 2077 696e  Ranked Pairs win
-00007aa0: 6e65 7273 2c20 6275 7420 696e 636c 7564  ners, but includ
-00007ab0: 6520 6120 7465 7374 2074 6f20 6465 7465  e a test to dete
-00007ac0: 726d 696e 6564 2069 6620 6974 2077 696c  rmined if it wil
-00007ad0: 6c20 7461 6b65 2074 6f6f 206c 6f6e 6720  l take too long 
-00007ae0: 746f 2063 6f6d 7075 7465 2074 6865 2052  to compute the R
-00007af0: 616e 6b65 6420 5061 6972 7320 7769 6e6e  anked Pairs winn
-00007b00: 6572 732e 2049 6620 7468 6520 6361 6c63  ers. If the calc
-00007b10: 756c 6174 696f 6e20 6f66 2074 6865 2077  ulation of the w
-00007b20: 696e 6e65 7273 2077 696c 6c20 7461 6b65  inners will take
-00007b30: 2074 6f6f 206c 6f6e 672c 2072 6574 7572   too long, retur
-00007b40: 6e20 4e6f 6e65 2e0a 0a20 2020 202e 2e20  n None...    .. 
-00007b50: 696d 706f 7274 616e 743a 3a0a 2020 2020  important::.    
-00007b60: 2020 2020 5468 6973 2076 6f74 696e 6720      This voting 
-00007b70: 6d65 7468 6f64 2074 6861 7420 6d69 6768  method that migh
-00007b80: 7420 7265 7475 726e 204e 6f6e 6520 7261  t return None ra
-00007b90: 7468 6572 2074 6861 6e20 6120 6c69 7374  ther than a list
-00007ba0: 206f 6620 6361 6e64 6964 6174 6573 2e20   of candidates. 
-00007bb0: 200a 0a20 2020 2041 7267 733a 0a20 2020   ..    Args:.   
-00007bc0: 2020 2020 2065 6461 7461 2028 5072 6f66       edata (Prof
-00007bd0: 696c 652c 2050 726f 6669 6c65 5769 7468  ile, ProfileWith
-00007be0: 5469 6573 2c20 4d61 7267 696e 4772 6170  Ties, MarginGrap
-00007bf0: 6829 3a20 416e 7920 656c 6563 7469 6f6e  h): Any election
-00007c00: 2064 6174 6120 7468 6174 2068 6173 2061   data that has a
-00007c10: 2060 6d61 7267 696e 6020 6d65 7468 6f64   `margin` method
-00007c20: 2e20 0a20 2020 2020 2020 2063 7572 725f  . .        curr_
-00007c30: 6361 6e64 7320 284c 6973 745b 696e 745d  cands (List[int]
-00007c40: 2c20 6f70 7469 6f6e 616c 293a 2049 6620  , optional): If 
-00007c50: 7365 742c 2074 6865 6e20 6669 6e64 2074  set, then find t
-00007c60: 6865 2077 696e 6e65 7273 2066 6f72 2074  he winners for t
-00007c70: 6865 2070 726f 6669 6c65 2072 6573 7472  he profile restr
-00007c80: 6963 7465 6420 746f 2074 6865 2063 616e  icted to the can
-00007c90: 6469 6461 7465 7320 696e 2060 6063 7572  didates in ``cur
-00007ca0: 725f 6361 6e64 7360 600a 2020 2020 2020  r_cands``.      
-00007cb0: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
-00007cc0: 696f 6e20 2866 756e 6374 696f 6e2c 206f  ion (function, o
-00007cd0: 7074 696f 6e61 6c29 3a20 5468 6520 7374  ptional): The st
-00007ce0: 7265 6e67 7468 2066 756e 6374 696f 6e20  rength function 
-00007cf0: 746f 2062 6520 7573 6564 2074 6f20 6361  to be used to ca
-00007d00: 6c63 756c 6174 6520 7468 6520 7374 7265  lculate the stre
-00007d10: 6e67 7468 206f 6620 6120 7061 7468 2e20  ngth of a path. 
-00007d20: 2020 5468 6520 6465 6661 756c 7420 6973    The default is
-00007d30: 2074 6865 206d 6172 6769 6e20 6d65 7468   the margin meth
-00007d40: 6f64 206f 6620 6060 6564 6174 6160 602e  od of ``edata``.
-00007d50: 2020 2054 6869 7320 6f6e 6c79 206d 6174     This only mat
-00007d60: 7465 7273 2077 6865 6e20 7468 6520 6261  ters when the ba
-00007d70: 6c6c 6f74 7320 6172 6520 6e6f 7420 6c69  llots are not li
-00007d80: 6e65 6172 206f 7264 6572 732e 200a 0a20  near orders. .. 
-00007d90: 2020 2052 6574 7572 6e73 3a20 0a20 2020     Returns: .   
-00007da0: 2020 2020 2041 2073 6f72 7465 6420 6c69       A sorted li
-00007db0: 7374 206f 6620 6361 6e64 6964 6174 6573  st of candidates
-00007dc0: 2e20 0a0a 2020 2020 2e2e 2073 6565 616c  . ..    .. seeal
-00007dd0: 736f 3a3a 0a0a 2020 2020 2020 2020 3a6d  so::..        :m
-00007de0: 6574 683a 6070 7265 665f 766f 7469 6e67  eth:`pref_voting
-00007df0: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
-00007e00: 7468 6f64 732e 7261 6e6b 6564 5f70 6169  thods.ranked_pai
-00007e10: 7273 5f77 6974 685f 7465 7374 602c 203a  rs_with_test`, :
-00007e20: 6d65 7468 3a60 7072 6566 5f76 6f74 696e  meth:`pref_votin
-00007e30: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
-00007e40: 6574 686f 6473 2e72 616e 6b65 645f 7061  ethods.ranked_pa
-00007e50: 6972 735f 7a74 602c 203a 6d65 7468 3a60  irs_zt`, :meth:`
-00007e60: 7072 6566 5f76 6f74 696e 672e 6d61 7267  pref_voting.marg
-00007e70: 696e 5f62 6173 6564 5f6d 6574 686f 6473  in_based_methods
-00007e80: 2e72 616e 6b65 645f 7061 6972 735f 6465  .ranked_pairs_de
-00007e90: 6665 6174 7360 0a0a 2020 2020 3a45 7861  feats`..    :Exa
-00007ea0: 6d70 6c65 3a20 0a0a 2020 2020 2e2e 2070  mple: ..    .. p
-00007eb0: 6c6f 743a 3a20 206d 6172 6769 6e5f 6772  lot::  margin_gr
-00007ec0: 6170 6873 5f65 7861 6d70 6c65 732f 6d67  aphs_examples/mg
-00007ed0: 5f65 785f 7270 5f77 6974 685f 7465 7374  _ex_rp_with_test
-00007ee0: 2e70 790a 2020 2020 2020 2020 3a63 6f6e  .py.        :con
-00007ef0: 7465 7874 3a20 7265 7365 7420 200a 2020  text: reset  .  
-00007f00: 2020 2020 2020 3a69 6e63 6c75 6465 2d73        :include-s
-00007f10: 6f75 7263 653a 2054 7275 650a 0a0a 2020  ource: True...  
-00007f20: 2020 2e2e 2063 6f64 652d 626c 6f63 6b3a    .. code-block:
-00007f30: 3a20 0a0a 2020 2020 2020 2020 6672 6f6d  : ..        from
-00007f40: 2070 7265 665f 766f 7469 6e67 2e6d 6172   pref_voting.mar
-00007f50: 6769 6e5f 6261 7365 645f 6d65 7468 6f64  gin_based_method
-00007f60: 7320 696d 706f 7274 2072 616e 6b65 645f  s import ranked_
-00007f70: 7061 6972 735f 7769 7468 5f74 6573 740a  pairs_with_test.
-00007f80: 0a20 2020 2020 2020 2072 616e 6b65 645f  .        ranked_
-00007f90: 7061 6972 735f 7769 7468 5f74 6573 742e  pairs_with_test.
-00007fa0: 6469 7370 6c61 7928 6d67 290a 0a0a 2020  display(mg)...  
-00007fb0: 2020 2e2e 2065 7865 635f 636f 6465 3a3a    .. exec_code::
-00007fc0: 200a 2020 2020 2020 2020 3a68 6964 655f   .        :hide_
-00007fd0: 636f 6465 3a0a 0a20 2020 2020 2020 2066  code:..        f
-00007fe0: 726f 6d20 7072 6566 5f76 6f74 696e 672e  rom pref_voting.
-00007ff0: 7765 6967 6874 6564 5f6d 616a 6f72 6974  weighted_majorit
-00008000: 795f 6772 6170 6873 2069 6d70 6f72 7420  y_graphs import 
-00008010: 4d61 7267 696e 4772 6170 680a 2020 2020  MarginGraph.    
-00008020: 2020 2020 6672 6f6d 2070 7265 665f 766f      from pref_vo
-00008030: 7469 6e67 2e6d 6172 6769 6e5f 6261 7365  ting.margin_base
-00008040: 645f 6d65 7468 6f64 7320 696d 706f 7274  d_methods import
-00008050: 2072 616e 6b65 645f 7061 6972 735f 7769   ranked_pairs_wi
-00008060: 7468 5f74 6573 740a 2020 2020 2020 2020  th_test.        
-00008070: 0a20 2020 2020 2020 206d 6720 3d20 4d61  .        mg = Ma
-00008080: 7267 696e 4772 6170 6828 5b30 2c20 312c  rginGraph([0, 1,
-00008090: 2032 2c20 335d 2c20 5b28 312c 2032 2c20   2, 3], [(1, 2, 
-000080a0: 3229 2c20 2831 2c20 332c 2032 292c 2028  2), (1, 3, 2), (
-000080b0: 322c 2030 2c20 3229 5d29 0a20 2020 2020  2, 0, 2)]).     
-000080c0: 2020 200a 2020 2020 2020 2020 7261 6e6b     .        rank
-000080d0: 6564 5f70 6169 7273 5f77 6974 685f 7465  ed_pairs_with_te
-000080e0: 7374 2e64 6973 706c 6179 286d 6729 0a0a  st.display(mg)..
-000080f0: 0a20 2020 2022 2222 2020 2020 0a20 2020  .    """    .   
-00008100: 2063 616e 6469 6461 7465 7320 3d20 6564   candidates = ed
-00008110: 6174 612e 6361 6e64 6964 6174 6573 2069  ata.candidates i
-00008120: 6620 6375 7272 5f63 616e 6473 2069 7320  f curr_cands is 
-00008130: 4e6f 6e65 2065 6c73 6520 6375 7272 5f63  None else curr_c
-00008140: 616e 6473 2020 2020 0a20 2020 2063 6964  ands    .    cid
-00008150: 785f 746f 5f63 616e 6420 3d20 7b63 6964  x_to_cand = {cid
-00008160: 783a 2063 2066 6f72 2063 6964 782c 2063  x: c for cidx, c
-00008170: 2069 6e20 656e 756d 6572 6174 6528 6361   in enumerate(ca
-00008180: 6e64 6964 6174 6573 297d 2020 0a20 2020  ndidates)}  .   
-00008190: 2063 616e 645f 746f 5f63 6964 7820 3d20   cand_to_cidx = 
-000081a0: 7b63 3a20 6369 6478 2066 6f72 2063 6964  {c: cidx for cid
-000081b0: 782c 2063 2069 6e20 656e 756d 6572 6174  x, c in enumerat
-000081c0: 6528 6361 6e64 6964 6174 6573 297d 2020  e(candidates)}  
-000081d0: 0a20 2020 200a 2020 2020 7374 7265 6e67  .    .    streng
-000081e0: 7468 5f66 756e 6374 696f 6e20 3d20 6564  th_function = ed
-000081f0: 6174 612e 6d61 7267 696e 2069 6620 7374  ata.margin if st
-00008200: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
-00008210: 6973 204e 6f6e 6520 656c 7365 2073 7472  is None else str
-00008220: 656e 6774 685f 6675 6e63 7469 6f6e 2020  ength_function  
-00008230: 200a 0a20 2020 2063 7720 3d20 6564 6174   ..    cw = edat
-00008240: 612e 636f 6e64 6f72 6365 745f 7769 6e6e  a.condorcet_winn
-00008250: 6572 2863 7572 725f 6361 6e64 7320 3d20  er(curr_cands = 
-00008260: 6375 7272 5f63 616e 6473 290a 2020 2020  curr_cands).    
-00008270: 2320 5261 6e6b 6564 2050 6169 7273 2069  # Ranked Pairs i
-00008280: 7320 436f 6e64 6f72 6365 7420 636f 6e73  s Condorcet cons
-00008290: 6973 7465 6e74 2c20 736f 2073 696d 706c  istent, so simpl
-000082a0: 7920 7265 7475 726e 2074 6865 2043 6f6e  y return the Con
-000082b0: 646f 7263 6574 2077 696e 6e65 7220 6966  dorcet winner if
-000082c0: 2065 7869 7374 730a 2020 2020 6966 2063   exists.    if c
-000082d0: 7720 6973 206e 6f74 204e 6f6e 653a 200a  w is not None: .
-000082e0: 2020 2020 2020 2020 7769 6e6e 6572 7320          winners 
-000082f0: 3d20 5b63 775d 0a20 2020 2065 6c73 653a  = [cw].    else:
-00008300: 0a20 2020 2020 2020 2077 5f65 6467 6573  .        w_edges
-00008310: 203d 205b 2863 312c 2063 322c 2073 7472   = [(c1, c2, str
-00008320: 656e 6774 685f 6675 6e63 7469 6f6e 2863  ength_function(c
-00008330: 312c 2063 3229 2920 666f 7220 6331 2069  1, c2)) for c1 i
-00008340: 6e20 6361 6e64 6964 6174 6573 2066 6f72  n candidates for
-00008350: 2063 3220 696e 2063 616e 6469 6461 7465   c2 in candidate
-00008360: 7320 0a20 2020 2020 2020 2020 2020 2020  s .             
-00008370: 2020 2020 2020 6966 2063 3120 213d 2063        if c1 != c
-00008380: 3220 616e 6420 2865 6461 7461 2e6d 616a  2 and (edata.maj
-00008390: 6f72 6974 795f 7072 6566 6572 7328 6331  ority_prefers(c1
-000083a0: 2c20 6332 2920 6f72 2065 6461 7461 2e69  , c2) or edata.i
-000083b0: 735f 7469 6564 2863 312c 2063 3229 295d  s_tied(c1, c2))]
-000083c0: 0a20 2020 2020 2020 2077 696e 6e65 7273  .        winners
-000083d0: 203d 206c 6973 7428 2920 2020 2020 2020   = list()       
-000083e0: 2020 2020 200a 2020 2020 2020 2020 7374       .        st
-000083f0: 7265 6e67 7468 7320 3d20 736f 7274 6564  rengths = sorted
-00008400: 286c 6973 7428 7365 7428 5b65 5b32 5d20  (list(set([e[2] 
-00008410: 666f 7220 6520 696e 2077 5f65 6467 6573  for e in w_edges
-00008420: 5d29 292c 2072 6576 6572 7365 3d54 7275  ])), reverse=Tru
-00008430: 6529 0a20 2020 2020 2020 2073 6f72 7465  e).        sorte
-00008440: 645f 6564 6765 7320 3d20 5b5b 6520 666f  d_edges = [[e fo
-00008450: 7220 6520 696e 2077 5f65 6467 6573 2069  r e in w_edges i
-00008460: 6620 655b 325d 203d 3d20 735d 2066 6f72  f e[2] == s] for
-00008470: 2073 2069 6e20 7374 7265 6e67 7468 735d   s in strengths]
-00008480: 0a20 2020 2020 2020 2069 6620 6e70 2e70  .        if np.p
-00008490: 726f 6428 5b6d 6174 682e 6661 6374 6f72  rod([math.factor
-000084a0: 6961 6c28 6c65 6e28 6573 2929 2066 6f72  ial(len(es)) for
-000084b0: 2065 7320 696e 2073 6f72 7465 645f 6564   es in sorted_ed
-000084c0: 6765 735d 2920 3e20 3330 3030 3a20 0a20  ges]) > 3000: . 
-000084d0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000084e0: 6e20 4e6f 6e65 0a20 2020 2020 2020 2065  n None.        e
-000084f0: 6c73 653a 200a 2020 2020 2020 2020 2020  lse: .          
-00008500: 2020 7462 7320 3d20 7072 6f64 7563 7428    tbs = product(
-00008510: 2a5b 7065 726d 7574 6174 696f 6e73 2865  *[permutations(e
-00008520: 6467 6573 2920 666f 7220 6564 6765 7320  dges) for edges 
-00008530: 696e 2073 6f72 7465 645f 6564 6765 735d  in sorted_edges]
-00008540: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
-00008550: 7220 7462 2069 6e20 7462 733a 0a20 2020  r tb in tbs:.   
-00008560: 2020 2020 2020 2020 2020 2020 2065 6467               edg
-00008570: 6573 203d 2066 6c61 7474 656e 2874 6229  es = flatten(tb)
-00008580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008590: 2072 705f 6465 6665 6174 203d 2053 504f   rp_defeat = SPO
-000085a0: 286c 656e 2863 616e 6469 6461 7465 7329  (len(candidates)
-000085b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000085c0: 2020 666f 7220 6530 2c65 312c 7320 696e    for e0,e1,s in
-000085d0: 2065 6467 6573 3a20 0a20 2020 2020 2020   edges: .       
-000085e0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000085f0: 6e6f 7420 7270 5f64 6566 6561 742e 505b  not rp_defeat.P[
-00008600: 6361 6e64 5f74 6f5f 6369 6478 5b65 315d  cand_to_cidx[e1]
-00008610: 5d5b 6361 6e64 5f74 6f5f 6369 6478 5b65  ][cand_to_cidx[e
-00008620: 305d 5d3a 0a20 2020 2020 2020 2020 2020  0]]:.           
-00008630: 2020 2020 2020 2020 2020 2020 2072 705f               rp_
-00008640: 6465 6665 6174 2e61 6464 2863 616e 645f  defeat.add(cand_
-00008650: 746f 5f63 6964 785b 6530 5d2c 6361 6e64  to_cidx[e0],cand
-00008660: 5f74 6f5f 6369 6478 5b65 315d 290a 2020  _to_cidx[e1]).  
-00008670: 2020 2020 2020 2020 2020 2020 2020 7769                wi
-00008680: 6e6e 6572 732e 6170 7065 6e64 2863 6964  nners.append(cid
-00008690: 785f 746f 5f63 616e 645b 7270 5f64 6566  x_to_cand[rp_def
-000086a0: 6561 742e 696e 6974 6961 6c5f 656c 656d  eat.initial_elem
-000086b0: 656e 7473 2829 5b30 5d5d 290a 2020 2020  ents()[0]]).    
-000086c0: 7265 7475 726e 2073 6f72 7465 6428 6c69  return sorted(li
-000086d0: 7374 2873 6574 2877 696e 6e65 7273 2929  st(set(winners))
-000086e0: 290a 0a64 6566 2072 616e 6b65 645f 7061  )..def ranked_pa
-000086f0: 6972 735f 6465 6665 6174 7328 6564 6174  irs_defeats(edat
-00008700: 612c 2063 7572 725f 6361 6e64 7320 3d20  a, curr_cands = 
-00008710: 4e6f 6e65 2c20 7374 7265 6e67 7468 5f66  None, strength_f
-00008720: 756e 6374 696f 6e20 3d20 4e6f 6e65 293a  unction = None):
-00008730: 2020 200a 2020 2020 2222 220a 2020 2020     .    """.    
-00008740: 5265 7475 726e 7320 7468 6520 5261 6e6b  Returns the Rank
-00008750: 6564 2050 6169 7273 2064 6566 6561 7420  ed Pairs defeat 
-00008760: 7265 6c61 7469 6f6e 7320 7072 6f64 7563  relations produc
-00008770: 6564 2062 7920 7468 6520 5261 6e6b 6564  ed by the Ranked
-00008780: 2050 6169 7273 2061 6c67 6f72 6974 686d   Pairs algorithm
-00008790: 2e20 0a0a 2020 2020 2e2e 2069 6d70 6f72  . ..    .. impor
-000087a0: 7461 6e74 3a3a 0a20 2020 2020 2020 2055  tant::.        U
-000087b0: 6e6c 696b 6520 7468 6520 6f74 6865 7220  nlike the other 
-000087c0: 6675 6e63 7469 6f6e 7320 7468 6174 2072  functions that r
-000087d0: 6574 7572 6e20 6120 7369 6e67 6c65 2064  eturn a single d
-000087e0: 6566 6561 7420 7265 6c61 7469 6f6e 2c20  efeat relation, 
-000087f0: 7468 6973 2072 6574 7572 6e73 2061 206c  this returns a l
-00008800: 6973 7420 6f66 2064 6566 6561 7420 7265  ist of defeat re
-00008810: 6c61 7469 6f6e 732e 200a 2020 2020 2020  lations. .      
-00008820: 2020 0a20 2020 2041 7267 733a 0a20 2020    .    Args:.   
-00008830: 2020 2020 2065 6461 7461 2028 5072 6f66       edata (Prof
-00008840: 696c 652c 2050 726f 6669 6c65 5769 7468  ile, ProfileWith
-00008850: 5469 6573 2c20 4d61 7267 696e 4772 6170  Ties, MarginGrap
-00008860: 6829 3a20 416e 7920 656c 6563 7469 6f6e  h): Any election
-00008870: 2064 6174 6120 7468 6174 2068 6173 2061   data that has a
-00008880: 2060 6d61 7267 696e 6020 6d65 7468 6f64   `margin` method
-00008890: 2e20 0a20 2020 2020 2020 2063 7572 725f  . .        curr_
-000088a0: 6361 6e64 7320 284c 6973 745b 696e 745d  cands (List[int]
-000088b0: 2c20 6f70 7469 6f6e 616c 293a 2049 6620  , optional): If 
-000088c0: 7365 742c 2074 6865 6e20 6669 6e64 2074  set, then find t
-000088d0: 6865 2077 696e 6e65 7273 2066 6f72 2074  he winners for t
-000088e0: 6865 2070 726f 6669 6c65 2072 6573 7472  he profile restr
-000088f0: 6963 7465 6420 746f 2074 6865 2063 616e  icted to the can
-00008900: 6469 6461 7465 7320 696e 2060 6063 7572  didates in ``cur
-00008910: 725f 6361 6e64 7360 600a 2020 2020 2020  r_cands``.      
-00008920: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
-00008930: 696f 6e20 2866 756e 6374 696f 6e2c 206f  ion (function, o
-00008940: 7074 696f 6e61 6c29 3a20 5468 6520 7374  ptional): The st
-00008950: 7265 6e67 7468 2066 756e 6374 696f 6e20  rength function 
-00008960: 746f 2062 6520 7573 6564 2074 6f20 6361  to be used to ca
-00008970: 6c63 756c 6174 6520 7468 6520 7374 7265  lculate the stre
-00008980: 6e67 7468 206f 6620 6120 7061 7468 2e20  ngth of a path. 
-00008990: 2020 5468 6520 6465 6661 756c 7420 6973    The default is
-000089a0: 2074 6865 206d 6172 6769 6e20 6d65 7468   the margin meth
-000089b0: 6f64 206f 6620 6060 6564 6174 6160 602e  od of ``edata``.
-000089c0: 2020 2054 6869 7320 6f6e 6c79 206d 6174     This only mat
-000089d0: 7465 7273 2077 6865 6e20 7468 6520 6261  ters when the ba
-000089e0: 6c6c 6f74 7320 6172 6520 6e6f 7420 6c69  llots are not li
-000089f0: 6e65 6172 206f 7264 6572 732e 200a 0a20  near orders. .. 
-00008a00: 2020 2052 6574 7572 6e73 3a20 0a20 2020     Returns: .   
-00008a10: 2020 2020 2041 206e 6574 776f 726b 7820       A networkx 
-00008a20: 4469 4772 6170 6820 7265 7072 6573 656e  DiGraph represen
-00008a30: 7469 6e67 2074 6865 2052 616e 6b65 6420  ting the Ranked 
-00008a40: 5061 6972 7320 6465 6665 6174 2072 656c  Pairs defeat rel
-00008a50: 6174 696f 6e2e 200a 0a20 2020 202e 2e20  ation. ..    .. 
-00008a60: 7365 6561 6c73 6f3a 3a0a 0a20 2020 2020  seealso::..     
-00008a70: 2020 203a 6d65 7468 3a60 7072 6566 5f76     :meth:`pref_v
-00008a80: 6f74 696e 672e 6d61 7267 696e 5f62 6173  oting.margin_bas
-00008a90: 6564 5f6d 6574 686f 6473 2e72 616e 6b65  ed_methods.ranke
-00008aa0: 645f 7061 6972 7360 2c20 3a6d 6574 683a  d_pairs`, :meth:
-00008ab0: 6070 7265 665f 766f 7469 6e67 2e6d 6172  `pref_voting.mar
-00008ac0: 6769 6e5f 6261 7365 645f 6d65 7468 6f64  gin_based_method
-00008ad0: 732e 7261 6e6b 6564 5f70 6169 7273 5f77  s.ranked_pairs_w
-00008ae0: 6974 685f 7465 7374 600a 0a20 2020 203a  ith_test`..    :
-00008af0: 4578 616d 706c 653a 200a 0a20 2020 202e  Example: ..    .
-00008b00: 2e20 706c 6f74 3a3a 2020 6d61 7267 696e  . plot::  margin
-00008b10: 5f67 7261 7068 735f 6578 616d 706c 6573  _graphs_examples
-00008b20: 2f6d 675f 6578 5f72 705f 6465 6665 6174  /mg_ex_rp_defeat
-00008b30: 732e 7079 0a20 2020 2020 2020 203a 636f  s.py.        :co
-00008b40: 6e74 6578 743a 2072 6573 6574 2020 0a20  ntext: reset  . 
-00008b50: 2020 2020 2020 203a 696e 636c 7564 652d         :include-
-00008b60: 736f 7572 6365 3a20 5472 7565 0a0a 2020  source: True..  
-00008b70: 2020 2e2e 2065 7865 635f 636f 6465 3a3a    .. exec_code::
-00008b80: 0a0a 0a20 2020 2020 2020 2066 726f 6d20  ...        from 
-00008b90: 7072 6566 5f76 6f74 696e 672e 7765 6967  pref_voting.weig
-00008ba0: 6874 6564 5f6d 616a 6f72 6974 795f 6772  hted_majority_gr
-00008bb0: 6170 6873 2069 6d70 6f72 7420 4d61 7267  aphs import Marg
-00008bc0: 696e 4772 6170 680a 2020 2020 2020 2020  inGraph.        
-00008bd0: 6672 6f6d 2070 7265 665f 766f 7469 6e67  from pref_voting
-00008be0: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
-00008bf0: 7468 6f64 7320 696d 706f 7274 2072 616e  thods import ran
-00008c00: 6b65 645f 7061 6972 735f 6465 6665 6174  ked_pairs_defeat
-00008c10: 730a 0a20 2020 2020 2020 206d 6720 3d20  s..        mg = 
-00008c20: 4d61 7267 696e 4772 6170 6828 5b30 2c20  MarginGraph([0, 
-00008c30: 312c 2032 2c20 335d 2c20 5b28 302c 2031  1, 2, 3], [(0, 1
-00008c40: 2c20 3130 292c 2028 302c 2032 2c20 3229  , 10), (0, 2, 2)
-00008c50: 2c20 2831 2c20 332c 2034 292c 2028 322c  , (1, 3, 4), (2,
-00008c60: 2031 2c20 3629 2c20 2832 2c20 332c 2038   1, 6), (2, 3, 8
-00008c70: 292c 2028 332c 2030 2c20 3429 5d29 0a20  ), (3, 0, 4)]). 
-00008c80: 2020 2020 2020 2072 705f 6465 6665 6174         rp_defeat
-00008c90: 7320 3d20 7261 6e6b 6564 5f70 6169 7273  s = ranked_pairs
-00008ca0: 5f64 6566 6561 7473 286d 6729 0a0a 2020  _defeats(mg)..  
-00008cb0: 2020 2020 2020 666f 7220 7270 6420 696e        for rpd in
-00008cc0: 2072 705f 6465 6665 6174 733a 200a 2020   rp_defeats: .  
-00008cd0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00008ce0: 7270 642e 6564 6765 7329 0a0a 2020 2020  rpd.edges)..    
-00008cf0: 2222 220a 2020 2020 0a20 2020 2063 616e  """.    .    can
-00008d00: 6469 6461 7465 7320 3d20 6564 6174 612e  didates = edata.
-00008d10: 6361 6e64 6964 6174 6573 2069 6620 6375  candidates if cu
-00008d20: 7272 5f63 616e 6473 2069 7320 4e6f 6e65  rr_cands is None
-00008d30: 2065 6c73 6520 6375 7272 5f63 616e 6473   else curr_cands
-00008d40: 2020 2020 0a20 2020 2073 7472 656e 6774      .    strengt
-00008d50: 685f 6675 6e63 7469 6f6e 203d 2065 6461  h_function = eda
-00008d60: 7461 2e6d 6172 6769 6e20 6966 2073 7472  ta.margin if str
-00008d70: 656e 6774 685f 6675 6e63 7469 6f6e 2069  ength_function i
-00008d80: 7320 4e6f 6e65 2065 6c73 6520 7374 7265  s None else stre
-00008d90: 6e67 7468 5f66 756e 6374 696f 6e20 2020  ngth_function   
-00008da0: 200a 0a20 2020 2077 5f65 6467 6573 203d   ..    w_edges =
-00008db0: 205b 2863 312c 2063 322c 2073 7472 656e   [(c1, c2, stren
-00008dc0: 6774 685f 6675 6e63 7469 6f6e 2863 312c  gth_function(c1,
-00008dd0: 2063 3229 2920 666f 7220 6331 2069 6e20   c2)) for c1 in 
-00008de0: 6361 6e64 6964 6174 6573 2066 6f72 2063  candidates for c
-00008df0: 3220 696e 2063 616e 6469 6461 7465 7320  2 in candidates 
-00008e00: 6966 2063 3120 213d 2063 3220 616e 6420  if c1 != c2 and 
-00008e10: 2865 6461 7461 2e6d 616a 6f72 6974 795f  (edata.majority_
-00008e20: 7072 6566 6572 7328 6331 2c20 6332 2920  prefers(c1, c2) 
-00008e30: 6f72 2065 6461 7461 2e69 735f 7469 6564  or edata.is_tied
-00008e40: 2863 312c 2063 3229 295d 0a20 2020 2077  (c1, c2))].    w
-00008e50: 696e 6e65 7273 203d 206c 6973 7428 2920  inners = list() 
-00008e60: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-00008e70: 7374 7265 6e67 7468 7320 3d20 736f 7274  strengths = sort
-00008e80: 6564 286c 6973 7428 7365 7428 5b65 5b32  ed(list(set([e[2
-00008e90: 5d20 666f 7220 6520 696e 2077 5f65 6467  ] for e in w_edg
-00008ea0: 6573 5d29 292c 2072 6576 6572 7365 3d54  es])), reverse=T
-00008eb0: 7275 6529 0a20 2020 2073 6f72 7465 645f  rue).    sorted_
-00008ec0: 6564 6765 7320 3d20 5b5b 6520 666f 7220  edges = [[e for 
-00008ed0: 6520 696e 2077 5f65 6467 6573 2069 6620  e in w_edges if 
-00008ee0: 655b 325d 203d 3d20 735d 2066 6f72 2073  e[2] == s] for s
-00008ef0: 2069 6e20 7374 7265 6e67 7468 735d 0a20   in strengths]. 
-00008f00: 2020 2074 6273 203d 2070 726f 6475 6374     tbs = product
-00008f10: 282a 5b70 6572 6d75 7461 7469 6f6e 7328  (*[permutations(
-00008f20: 6564 6765 7329 2066 6f72 2065 6467 6573  edges) for edges
-00008f30: 2069 6e20 736f 7274 6564 5f65 6467 6573   in sorted_edges
-00008f40: 5d29 0a20 2020 2072 705f 6465 6665 6174  ]).    rp_defeat
-00008f50: 7320 3d20 6c69 7374 2829 0a20 2020 2066  s = list().    f
-00008f60: 6f72 2074 6220 696e 2074 6273 3a0a 2020  or tb in tbs:.  
-00008f70: 2020 2020 2020 6564 6765 7320 3d20 666c        edges = fl
-00008f80: 6174 7465 6e28 7462 290a 2020 2020 2020  atten(tb).      
-00008f90: 2020 7270 5f64 6566 6561 7420 3d20 6e78    rp_defeat = nx
-00008fa0: 2e44 6947 7261 7068 2829 200a 2020 2020  .DiGraph() .    
-00008fb0: 2020 2020 666f 7220 6520 696e 2065 6467      for e in edg
-00008fc0: 6573 3a20 0a20 2020 2020 2020 2020 2020  es: .           
-00008fd0: 2072 705f 6465 6665 6174 2e61 6464 5f65   rp_defeat.add_e
-00008fe0: 6467 6528 655b 305d 2c20 655b 315d 2c20  dge(e[0], e[1], 
-00008ff0: 7765 6967 6874 3d65 5b32 5d29 0a20 2020  weight=e[2]).   
-00009000: 2020 2020 2020 2020 2069 6620 646f 6573           if does
-00009010: 5f63 7265 6174 655f 6379 636c 6528 7270  _create_cycle(rp
-00009020: 5f64 6566 6561 742c 2065 293a 0a20 2020  _defeat, e):.   
-00009030: 2020 2020 2020 2020 2020 2020 2072 705f               rp_
-00009040: 6465 6665 6174 2e72 656d 6f76 655f 6564  defeat.remove_ed
-00009050: 6765 2865 5b30 5d2c 2065 5b31 5d29 0a20  ge(e[0], e[1]). 
-00009060: 2020 2020 2020 2072 705f 6465 6665 6174         rp_defeat
-00009070: 732e 6170 7065 6e64 2872 705f 6465 6665  s.append(rp_defe
-00009080: 6174 290a 2020 2020 2020 2020 7769 6e6e  at).        winn
-00009090: 6572 732e 6170 7065 6e64 286d 6178 696d  ers.append(maxim
-000090a0: 616c 5f65 6c65 6d65 6e74 7328 7270 5f64  al_elements(rp_d
-000090b0: 6566 6561 7429 5b30 5d29 0a20 2020 2072  efeat)[0]).    r
-000090c0: 6574 7572 6e20 7270 5f64 6566 6561 7473  eturn rp_defeats
-000090d0: 0a0a 0a40 766d 286e 616d 653d 2252 616e  ...@vm(name="Ran
-000090e0: 6b65 6420 5061 6972 7320 5442 2229 0a64  ked Pairs TB").d
-000090f0: 6566 2072 616e 6b65 645f 7061 6972 735f  ef ranked_pairs_
-00009100: 7462 280a 2020 2020 6564 6174 612c 200a  tb(.    edata, .
-00009110: 2020 2020 6375 7272 5f63 616e 6473 203d      curr_cands =
-00009120: 204e 6f6e 652c 200a 2020 2020 7469 655f   None, .    tie_
-00009130: 6272 6561 6b65 7220 3d20 4e6f 6e65 2c20  breaker = None, 
-00009140: 0a20 2020 2073 7472 656e 6774 685f 6675  .    strength_fu
-00009150: 6e63 7469 6f6e 203d 204e 6f6e 6529 3a20  nction = None): 
-00009160: 2020 0a20 2020 2022 2222 0a20 2020 2052    .    """.    R
-00009170: 616e 6b65 6420 5061 6972 7320 7769 7468  anked Pairs with
-00009180: 2061 2066 6978 6564 206c 696e 6561 7220   a fixed linear 
-00009190: 6f72 6465 7220 6f6e 2074 6865 2063 616e  order on the can
-000091a0: 6469 6461 7465 7320 746f 2062 7265 616b  didates to break
-000091b0: 2061 6e79 2074 6965 7320 696e 2074 6865   any ties in the
-000091c0: 206d 6172 6769 6e73 2e20 2020 0a20 2020   margins.   .   
-000091d0: 2053 696e 6365 2074 6865 2074 6965 5f62   Since the tie_b
-000091e0: 7265 616b 6572 2069 7320 6120 6c69 6e65  reaker is a line
-000091f0: 6172 206f 7264 6572 2c20 7468 6973 206d  ar order, this m
-00009200: 6574 686f 6420 6973 2072 6573 6f6c 7574  ethod is resolut
-00009210: 652e 2020 200a 0a20 2020 2041 7267 733a  e.   ..    Args:
-00009220: 0a20 2020 2020 2020 2065 6461 7461 2028  .        edata (
-00009230: 5072 6f66 696c 652c 2050 726f 6669 6c65  Profile, Profile
-00009240: 5769 7468 5469 6573 2c20 4d61 7267 696e  WithTies, Margin
-00009250: 4772 6170 6829 3a20 416e 7920 656c 6563  Graph): Any elec
-00009260: 7469 6f6e 2064 6174 6120 7468 6174 2068  tion data that h
-00009270: 6173 2061 2060 6d61 7267 696e 6020 6d65  as a `margin` me
-00009280: 7468 6f64 2e20 0a20 2020 2020 2020 2063  thod. .        c
-00009290: 7572 725f 6361 6e64 7320 284c 6973 745b  urr_cands (List[
-000092a0: 696e 745d 2c20 6f70 7469 6f6e 616c 293a  int], optional):
-000092b0: 2049 6620 7365 742c 2074 6865 6e20 6669   If set, then fi
-000092c0: 6e64 2074 6865 2077 696e 6e65 7273 2066  nd the winners f
-000092d0: 6f72 2074 6865 2070 726f 6669 6c65 2072  or the profile r
-000092e0: 6573 7472 6963 7465 6420 746f 2074 6865  estricted to the
-000092f0: 2063 616e 6469 6461 7465 7320 696e 2060   candidates in `
-00009300: 6063 7572 725f 6361 6e64 7360 600a 2020  `curr_cands``.  
-00009310: 2020 2020 2020 7374 7265 6e67 7468 5f66        strength_f
-00009320: 756e 6374 696f 6e20 2866 756e 6374 696f  unction (functio
-00009330: 6e2c 206f 7074 696f 6e61 6c29 3a20 5468  n, optional): Th
-00009340: 6520 7374 7265 6e67 7468 2066 756e 6374  e strength funct
-00009350: 696f 6e20 746f 2062 6520 7573 6564 2074  ion to be used t
-00009360: 6f20 6361 6c63 756c 6174 6520 7468 6520  o calculate the 
-00009370: 7374 7265 6e67 7468 206f 6620 6120 7061  strength of a pa
-00009380: 7468 2e20 2020 5468 6520 6465 6661 756c  th.   The defaul
-00009390: 7420 6973 2074 6865 206d 6172 6769 6e20  t is the margin 
-000093a0: 6d65 7468 6f64 206f 6620 6060 6564 6174  method of ``edat
-000093b0: 6160 602e 2020 2054 6869 7320 6f6e 6c79  a``.   This only
-000093c0: 206d 6174 7465 7273 2077 6865 6e20 7468   matters when th
-000093d0: 6520 6261 6c6c 6f74 7320 6172 6520 6e6f  e ballots are no
-000093e0: 7420 6c69 6e65 6172 206f 7264 6572 732e  t linear orders.
-000093f0: 200a 0a20 2020 2052 6574 7572 6e73 3a20   ..    Returns: 
-00009400: 0a20 2020 2020 2020 2041 2073 6f72 7465  .        A sorte
-00009410: 6420 6c69 7374 206f 6620 6361 6e64 6964  d list of candid
-00009420: 6174 6573 2e20 0a0a 2020 2020 2e2e 2073  ates. ..    .. s
-00009430: 6565 616c 736f 3a3a 0a0a 2020 2020 2020  eealso::..      
-00009440: 2020 3a6d 6574 683a 6070 7265 665f 766f    :meth:`pref_vo
-00009450: 7469 6e67 2e6d 6172 6769 6e5f 6261 7365  ting.margin_base
-00009460: 645f 6d65 7468 6f64 732e 7261 6e6b 6564  d_methods.ranked
-00009470: 5f70 6169 7273 602c 203a 6d65 7468 3a60  _pairs`, :meth:`
-00009480: 7072 6566 5f76 6f74 696e 672e 6d61 7267  pref_voting.marg
-00009490: 696e 5f62 6173 6564 5f6d 6574 686f 6473  in_based_methods
-000094a0: 2e72 616e 6b65 645f 7061 6972 735f 7769  .ranked_pairs_wi
-000094b0: 7468 5f74 6573 7460 0a0a 2020 2020 2e2e  th_test`..    ..
-000094c0: 2065 7865 635f 636f 6465 3a3a 0a0a 2020   exec_code::..  
-000094d0: 2020 2020 2020 6672 6f6d 2070 7265 665f        from pref_
-000094e0: 766f 7469 6e67 2e70 726f 6669 6c65 7320  voting.profiles 
-000094f0: 696d 706f 7274 2050 726f 6669 6c65 0a20  import Profile. 
-00009500: 2020 2020 2020 2066 726f 6d20 7072 6566         from pref
-00009510: 5f76 6f74 696e 672e 6d61 7267 696e 5f62  _voting.margin_b
-00009520: 6173 6564 5f6d 6574 686f 6473 2069 6d70  ased_methods imp
-00009530: 6f72 7420 7261 6e6b 6564 5f70 6169 7273  ort ranked_pairs
-00009540: 5f74 622c 2072 616e 6b65 645f 7061 6972  _tb, ranked_pair
-00009550: 735f 7a74 0a0a 2020 2020 2020 2020 7072  s_zt..        pr
-00009560: 6f66 203d 2050 726f 6669 6c65 285b 5b32  of = Profile([[2
-00009570: 2c20 332c 2031 2c20 305d 2c20 5b30 2c20  , 3, 1, 0], [0, 
-00009580: 332c 2031 2c20 325d 2c20 5b31 2c20 332c  3, 1, 2], [1, 3,
-00009590: 2032 2c20 305d 2c20 5b32 2c20 312c 2033   2, 0], [2, 1, 3
-000095a0: 2c20 305d 5d2c 205b 312c 2031 2c20 312c  , 0]], [1, 1, 1,
-000095b0: 2031 5d29 0a0a 2020 2020 2020 2020 7072   1])..        pr
-000095c0: 6f66 2e64 6973 706c 6179 2829 0a0a 2020  of.display()..  
-000095d0: 2020 2020 2020 7261 6e6b 6564 5f70 6169        ranked_pai
-000095e0: 7273 5f74 622e 6469 7370 6c61 7928 7072  rs_tb.display(pr
-000095f0: 6f66 290a 2020 2020 2020 2020 7261 6e6b  of).        rank
-00009600: 6564 5f70 6169 7273 5f74 622e 6469 7370  ed_pairs_tb.disp
-00009610: 6c61 7928 7072 6f66 2c20 7469 655f 6272  lay(prof, tie_br
-00009620: 6561 6b65 7220 3d20 5b33 2c20 322c 2031  eaker = [3, 2, 1
-00009630: 2c20 305d 290a 2020 2020 2020 2020 7261  , 0]).        ra
-00009640: 6e6b 6564 5f70 6169 7273 5f7a 742e 6469  nked_pairs_zt.di
-00009650: 7370 6c61 7928 7072 6f66 290a 0a20 2020  splay(prof)..   
-00009660: 2022 2222 0a0a 2020 2020 6361 6e64 6964   """..    candid
-00009670: 6174 6573 203d 2065 6461 7461 2e63 616e  ates = edata.can
-00009680: 6469 6461 7465 7320 6966 2063 7572 725f  didates if curr_
-00009690: 6361 6e64 7320 6973 204e 6f6e 6520 656c  cands is None el
-000096a0: 7365 2063 7572 725f 6361 6e64 7320 2020  se curr_cands   
-000096b0: 200a 2020 2020 6369 6478 5f74 6f5f 6361   .    cidx_to_ca
-000096c0: 6e64 203d 207b 6369 6478 3a20 6320 666f  nd = {cidx: c fo
-000096d0: 7220 6369 6478 2c20 6320 696e 2065 6e75  r cidx, c in enu
-000096e0: 6d65 7261 7465 2863 616e 6469 6461 7465  merate(candidate
-000096f0: 7329 7d20 200a 2020 2020 6361 6e64 5f74  s)}  .    cand_t
-00009700: 6f5f 6369 6478 203d 207b 633a 2063 6964  o_cidx = {c: cid
-00009710: 7820 666f 7220 6369 6478 2c20 6320 696e  x for cidx, c in
-00009720: 2065 6e75 6d65 7261 7465 2863 616e 6469   enumerate(candi
-00009730: 6461 7465 7329 7d20 200a 0a20 2020 2073  dates)}  ..    s
-00009740: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-00009750: 203d 2065 6461 7461 2e6d 6172 6769 6e20   = edata.margin 
-00009760: 6966 2073 7472 656e 6774 685f 6675 6e63  if strength_func
-00009770: 7469 6f6e 2069 7320 4e6f 6e65 2065 6c73  tion is None els
-00009780: 6520 7374 7265 6e67 7468 5f66 756e 6374  e strength_funct
-00009790: 696f 6e0a 2020 2020 0a20 2020 2074 625f  ion.    .    tb_
-000097a0: 7261 6e6b 696e 6720 3d20 7469 655f 6272  ranking = tie_br
-000097b0: 6561 6b65 7220 6966 2074 6965 5f62 7265  eaker if tie_bre
-000097c0: 616b 6572 2069 7320 6e6f 7420 4e6f 6e65  aker is not None
-000097d0: 2065 6c73 6520 736f 7274 6564 286c 6973   else sorted(lis
-000097e0: 7428 6361 6e64 6964 6174 6573 2929 0a0a  t(candidates))..
-000097f0: 2020 2020 6377 203d 2065 6461 7461 2e63      cw = edata.c
-00009800: 6f6e 646f 7263 6574 5f77 696e 6e65 7228  ondorcet_winner(
-00009810: 6375 7272 5f63 616e 6473 3d63 7572 725f  curr_cands=curr_
-00009820: 6361 6e64 7329 0a20 2020 2023 2052 616e  cands).    # Ran
-00009830: 6b65 6420 5061 6972 7320 6973 2043 6f6e  ked Pairs is Con
-00009840: 646f 7263 6574 2063 6f6e 7369 7374 656e  dorcet consisten
-00009850: 742c 2073 6f20 7369 6d70 6c79 2072 6574  t, so simply ret
-00009860: 7572 6e20 7468 6520 436f 6e64 6f72 6365  urn the Condorce
-00009870: 7420 7769 6e6e 6572 2069 6620 6578 6973  t winner if exis
-00009880: 7473 0a20 2020 2069 6620 6377 2069 7320  ts.    if cw is 
-00009890: 6e6f 7420 4e6f 6e65 3a20 0a20 2020 2020  not None: .     
-000098a0: 2020 2077 696e 6e65 7273 203d 205b 6377     winners = [cw
-000098b0: 5d0a 2020 2020 656c 7365 3a0a 2020 2020  ].    else:.    
-000098c0: 2020 2020 775f 6564 6765 7320 3d20 5b28      w_edges = [(
-000098d0: 6331 2c20 6332 2c20 7374 7265 6e67 7468  c1, c2, strength
-000098e0: 5f66 756e 6374 696f 6e28 6331 2c20 6332  _function(c1, c2
-000098f0: 2929 2066 6f72 2063 3120 696e 2063 616e  )) for c1 in can
-00009900: 6469 6461 7465 7320 666f 7220 6332 2069  didates for c2 i
-00009910: 6e20 6361 6e64 6964 6174 6573 200a 2020  n candidates .  
-00009920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009930: 2069 6620 6331 2021 3d20 6332 2061 6e64   if c1 != c2 and
-00009940: 2028 6564 6174 612e 6d61 6a6f 7269 7479   (edata.majority
-00009950: 5f70 7265 6665 7273 2863 312c 2063 3229  _prefers(c1, c2)
-00009960: 206f 7220 6564 6174 612e 6973 5f74 6965   or edata.is_tie
-00009970: 6428 6331 2c20 6332 2929 5d0a 2020 2020  d(c1, c2))].    
-00009980: 2020 2020 7769 6e6e 6572 7320 3d20 6c69      winners = li
-00009990: 7374 2829 2020 2020 2020 2020 2020 2020  st()            
-000099a0: 0a20 2020 2020 2020 2073 7472 656e 6774  .        strengt
-000099b0: 6873 203d 2073 6f72 7465 6428 6c69 7374  hs = sorted(list
-000099c0: 2873 6574 285b 655b 325d 2066 6f72 2065  (set([e[2] for e
-000099d0: 2069 6e20 775f 6564 6765 735d 2929 2c20   in w_edges])), 
-000099e0: 7265 7665 7273 653d 5472 7565 290a 2020  reverse=True).  
-000099f0: 2020 2020 2020 0a20 2020 2020 2020 2072        .        r
-00009a00: 705f 6465 6665 6174 203d 2053 504f 286c  p_defeat = SPO(l
-00009a10: 656e 2863 616e 6469 6461 7465 7329 290a  en(candidates)).
-00009a20: 0a20 2020 2020 2020 2066 6f72 2073 2069  .        for s i
-00009a30: 6e20 7374 7265 6e67 7468 733a 200a 2020  n strengths: .  
-00009a40: 2020 2020 2020 2020 2020 6564 6765 7320            edges 
-00009a50: 3d20 5b65 2066 6f72 2065 2069 6e20 775f  = [e for e in w_
-00009a60: 6564 6765 7320 6966 2065 5b32 5d20 3d3d  edges if e[2] ==
-00009a70: 2073 5d0a 2020 2020 2020 2020 2020 2020   s].            
-00009a80: 0a20 2020 2020 2020 2020 2020 2023 2062  .            # b
-00009a90: 7265 616b 2074 6965 7320 7573 696e 6720  reak ties using 
-00009aa0: 7468 6520 6c65 7869 636f 6772 6170 6869  the lexicographi
-00009ab0: 6320 6f72 6465 7269 6e67 206f 6e20 7475  c ordering on tu
-00009ac0: 706c 6573 2067 6976 656e 2074 625f 7261  ples given tb_ra
-00009ad0: 6e6b 696e 670a 2020 2020 2020 2020 2020  nking.          
-00009ae0: 2020 736f 7274 6564 5f65 6467 6573 203d    sorted_edges =
-00009af0: 2073 6f72 7465 6428 6564 6765 732c 206b   sorted(edges, k
-00009b00: 6579 203d 206c 616d 6264 6120 653a 2028  ey = lambda e: (
-00009b10: 7462 5f72 616e 6b69 6e67 2e69 6e64 6578  tb_ranking.index
-00009b20: 2865 5b30 5d29 2c20 7462 5f72 616e 6b69  (e[0]), tb_ranki
-00009b30: 6e67 2e69 6e64 6578 2865 5b31 5d29 292c  ng.index(e[1])),
-00009b40: 2072 6576 6572 7365 3d46 616c 7365 290a   reverse=False).
-00009b50: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00009b60: 6530 2c65 312c 7320 696e 2065 6467 6573  e0,e1,s in edges
-00009b70: 3a20 0a20 2020 2020 2020 2020 2020 2020  : .             
-00009b80: 2020 2069 6620 6e6f 7420 7270 5f64 6566     if not rp_def
-00009b90: 6561 742e 505b 6361 6e64 5f74 6f5f 6369  eat.P[cand_to_ci
-00009ba0: 6478 5b65 315d 5d5b 6361 6e64 5f74 6f5f  dx[e1]][cand_to_
-00009bb0: 6369 6478 5b65 305d 5d3a 0a20 2020 2020  cidx[e0]]:.     
-00009bc0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00009bd0: 705f 6465 6665 6174 2e61 6464 2863 616e  p_defeat.add(can
-00009be0: 645f 746f 5f63 6964 785b 6530 5d2c 6361  d_to_cidx[e0],ca
-00009bf0: 6e64 5f74 6f5f 6369 6478 5b65 315d 290a  nd_to_cidx[e1]).
-00009c00: 2020 2020 2020 2020 2020 2020 7769 6e6e              winn
-00009c10: 6572 732e 6170 7065 6e64 2863 6964 785f  ers.append(cidx_
-00009c20: 746f 5f63 616e 645b 7270 5f64 6566 6561  to_cand[rp_defea
-00009c30: 742e 696e 6974 6961 6c5f 656c 656d 656e  t.initial_elemen
-00009c40: 7473 2829 5b30 5d5d 290a 0a20 2020 2072  ts()[0]])..    r
-00009c50: 6574 7572 6e20 736f 7274 6564 286c 6973  eturn sorted(lis
-00009c60: 7428 7365 7428 7769 6e6e 6572 7329 2929  t(set(winners)))
-00009c70: 0a0a 0a40 766d 286e 616d 653d 2252 616e  ...@vm(name="Ran
-00009c80: 6b65 6420 5061 6972 7320 5a54 2229 0a64  ked Pairs ZT").d
-00009c90: 6566 2072 616e 6b65 645f 7061 6972 735f  ef ranked_pairs_
-00009ca0: 7a74 280a 2020 2020 7072 6f66 696c 652c  zt(.    profile,
-00009cb0: 200a 2020 2020 6375 7272 5f63 616e 6473   .    curr_cands
-00009cc0: 203d 204e 6f6e 652c 200a 2020 2020 7374   = None, .    st
-00009cd0: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
-00009ce0: 3d20 4e6f 6e65 293a 2020 200a 2020 2020  = None):   .    
-00009cf0: 2222 2252 616e 6b65 6420 7061 6972 7320  """Ranked pairs 
-00009d00: 7768 6572 6520 6120 6669 7865 6420 766f  where a fixed vo
-00009d10: 7465 7220 6272 6561 6b73 2061 6e79 2074  ter breaks any t
-00009d20: 6965 7320 696e 2074 6865 206d 6172 6769  ies in the margi
-00009d30: 6e73 2e20 2049 7420 6973 2061 6c77 6179  ns.  It is alway
-00009d40: 7320 7468 6520 766f 7465 7220 696e 2070  s the voter in p
-00009d50: 6f73 6974 696f 6e20 3020 7468 6174 2062  osition 0 that b
-00009d60: 7265 616b 7320 7468 6520 7469 6573 2e20  reaks the ties. 
-00009d70: 2053 696e 6365 2076 6f74 6572 7320 6861   Since voters ha
-00009d80: 7665 2073 7472 6963 7420 7072 6566 6572  ve strict prefer
-00009d90: 656e 6365 732c 2074 6869 7320 6d65 7468  ences, this meth
-00009da0: 6f64 2069 7320 7265 736f 6c75 7465 2e20  od is resolute. 
-00009db0: 2054 6869 7320 6973 206b 6e6f 776e 2061   This is known a
-00009dc0: 7320 5261 6e6b 6564 2050 6169 7273 205a  s Ranked Pairs Z
-00009dd0: 542c 2066 6f72 205a 6176 6973 7420 5469  T, for Zavist Ti
-00009de0: 6465 6d61 6e2e 0a0a 2020 2020 4172 6773  deman...    Args
-00009df0: 3a0a 2020 2020 2020 2020 6564 6174 6120  :.        edata 
-00009e00: 2850 726f 6669 6c65 293a 2041 2070 726f  (Profile): A pro
-00009e10: 6669 6c65 206f 6620 6c69 6e65 6172 206f  file of linear o
-00009e20: 7264 6572 730a 2020 2020 2020 2020 6375  rders.        cu
-00009e30: 7272 5f63 616e 6473 2028 4c69 7374 5b69  rr_cands (List[i
-00009e40: 6e74 5d2c 206f 7074 696f 6e61 6c29 3a20  nt], optional): 
-00009e50: 4966 2073 6574 2c20 7468 656e 2066 696e  If set, then fin
-00009e60: 6420 7468 6520 7769 6e6e 6572 7320 666f  d the winners fo
-00009e70: 7220 7468 6520 7072 6f66 696c 6520 7265  r the profile re
-00009e80: 7374 7269 6374 6564 2074 6f20 7468 6520  stricted to the 
-00009e90: 6361 6e64 6964 6174 6573 2069 6e20 6060  candidates in ``
-00009ea0: 6375 7272 5f63 616e 6473 6060 0a0a 2020  curr_cands``..  
-00009eb0: 2020 5265 7475 726e 733a 200a 2020 2020    Returns: .    
-00009ec0: 2020 2020 4120 736f 7274 6564 206c 6973      A sorted lis
-00009ed0: 7420 6f66 2063 616e 6469 6461 7465 732e  t of candidates.
-00009ee0: 200a 0a20 2020 202e 2e20 7365 6561 6c73   ..    .. seeals
-00009ef0: 6f3a 3a0a 0a20 2020 2020 2020 203a 6d65  o::..        :me
-00009f00: 7468 3a60 7072 6566 5f76 6f74 696e 672e  th:`pref_voting.
-00009f10: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
-00009f20: 686f 6473 2e72 616e 6b65 645f 7061 6972  hods.ranked_pair
-00009f30: 7360 2c20 3a6d 6574 683a 6070 7265 665f  s`, :meth:`pref_
-00009f40: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
-00009f50: 7365 645f 6d65 7468 6f64 732e 7261 6e6b  sed_methods.rank
-00009f60: 6564 5f70 6169 7273 5f77 6974 685f 7465  ed_pairs_with_te
-00009f70: 7374 600a 0a20 2020 202e 2e20 6578 6563  st`..    .. exec
-00009f80: 5f63 6f64 653a 3a0a 0a20 2020 2020 2020  _code::..       
-00009f90: 2066 726f 6d20 7072 6566 5f76 6f74 696e   from pref_votin
-00009fa0: 672e 7072 6f66 696c 6573 2069 6d70 6f72  g.profiles impor
-00009fb0: 7420 5072 6f66 696c 650a 2020 2020 2020  t Profile.      
-00009fc0: 2020 6672 6f6d 2070 7265 665f 766f 7469    from pref_voti
-00009fd0: 6e67 2e6d 6172 6769 6e5f 6261 7365 645f  ng.margin_based_
-00009fe0: 6d65 7468 6f64 7320 696d 706f 7274 2072  methods import r
-00009ff0: 616e 6b65 645f 7061 6972 735f 7462 2c20  anked_pairs_tb, 
-0000a000: 7261 6e6b 6564 5f70 6169 7273 5f7a 740a  ranked_pairs_zt.
-0000a010: 0a20 2020 2020 2020 2070 726f 6620 3d20  .        prof = 
-0000a020: 5072 6f66 696c 6528 5b5b 322c 2033 2c20  Profile([[2, 3, 
-0000a030: 312c 2030 5d2c 205b 302c 2033 2c20 312c  1, 0], [0, 3, 1,
-0000a040: 2032 5d2c 205b 312c 2033 2c20 322c 2030   2], [1, 3, 2, 0
-0000a050: 5d2c 205b 322c 2031 2c20 332c 2030 5d5d  ], [2, 1, 3, 0]]
-0000a060: 2c20 5b31 2c20 312c 2031 2c20 315d 290a  , [1, 1, 1, 1]).
-0000a070: 0a20 2020 2020 2020 2070 726f 662e 6469  .        prof.di
-0000a080: 7370 6c61 7928 290a 0a20 2020 2020 2020  splay()..       
-0000a090: 2072 616e 6b65 645f 7061 6972 735f 7462   ranked_pairs_tb
-0000a0a0: 2e64 6973 706c 6179 2870 726f 6629 0a20  .display(prof). 
-0000a0b0: 2020 2020 2020 2072 616e 6b65 645f 7061         ranked_pa
-0000a0c0: 6972 735f 7462 2e64 6973 706c 6179 2870  irs_tb.display(p
-0000a0d0: 726f 662c 2074 6965 5f62 7265 616b 6572  rof, tie_breaker
-0000a0e0: 203d 205b 332c 2032 2c20 312c 2030 5d29   = [3, 2, 1, 0])
-0000a0f0: 0a20 2020 2020 2020 2072 616e 6b65 645f  .        ranked_
-0000a100: 7061 6972 735f 7a74 2e64 6973 706c 6179  pairs_zt.display
-0000a110: 2870 726f 6629 0a0a 2020 2020 0a20 2020  (prof)..    .   
-0000a120: 2022 2222 0a20 2020 2063 616e 6469 6461   """.    candida
-0000a130: 7465 7320 3d20 7072 6f66 696c 652e 6361  tes = profile.ca
-0000a140: 6e64 6964 6174 6573 2069 6620 6375 7272  ndidates if curr
-0000a150: 5f63 616e 6473 2069 7320 4e6f 6e65 2065  _cands is None e
-0000a160: 6c73 6520 6375 7272 5f63 616e 6473 2020  lse curr_cands  
-0000a170: 2020 0a20 2020 200a 2020 2020 2320 7468    .    .    # th
-0000a180: 6520 7469 652d 6272 6561 6b65 7220 6973  e tie-breaker is
-0000a190: 2061 6c77 6179 7320 7468 6520 6669 7273   always the firs
-0000a1a0: 7420 766f 7465 722e 200a 2020 2020 7462  t voter. .    tb
-0000a1b0: 5f72 616e 6b69 6e67 203d 2074 7570 6c65  _ranking = tuple
-0000a1c0: 285b 6320 666f 7220 6320 696e 206c 6973  ([c for c in lis
-0000a1d0: 7428 7072 6f66 696c 652e 5f72 616e 6b69  t(profile._ranki
-0000a1e0: 6e67 735b 305d 2920 6966 2063 2069 6e20  ngs[0]) if c in 
-0000a1f0: 6361 6e64 6964 6174 6573 5d29 0a20 2020  candidates]).   
-0000a200: 200a 2020 2020 7265 7475 726e 2072 616e   .    return ran
-0000a210: 6b65 645f 7061 6972 735f 7462 2870 726f  ked_pairs_tb(pro
-0000a220: 6669 6c65 2c20 6375 7272 5f63 616e 6473  file, curr_cands
-0000a230: 203d 2063 7572 725f 6361 6e64 732c 2074   = curr_cands, t
-0000a240: 6965 5f62 7265 616b 6572 203d 2074 625f  ie_breaker = tb_
-0000a250: 7261 6e6b 696e 672c 2073 7472 656e 6774  ranking, strengt
-0000a260: 685f 6675 6e63 7469 6f6e 203d 2073 7472  h_function = str
-0000a270: 656e 6774 685f 6675 6e63 7469 6f6e 290a  ength_function).
-0000a280: 0a0a 4076 6d28 6e61 6d65 3d22 5269 7665  ..@vm(name="Rive
-0000a290: 7222 290a 6465 6620 7269 7665 7228 6564  r").def river(ed
-0000a2a0: 6174 612c 2063 7572 725f 6361 6e64 7320  ata, curr_cands 
-0000a2b0: 3d20 4e6f 6e65 2c20 7374 7265 6e67 7468  = None, strength
-0000a2c0: 5f66 756e 6374 696f 6e20 3d20 4e6f 6e65  _function = None
-0000a2d0: 293a 2020 200a 2020 2020 2222 220a 2020  ):   .    """.  
-0000a2e0: 2020 4f72 6465 7220 7468 6520 6564 6765    Order the edge
-0000a2f0: 7320 696e 2074 6865 2077 6561 6b20 6d61  s in the weak ma
-0000a300: 7267 696e 2067 7261 7068 2066 726f 6d20  rgin graph from 
-0000a310: 6c61 7267 6573 7420 746f 2073 6d61 6c6c  largest to small
-0000a320: 6573 7420 616e 6420 6c6f 636b 2074 6865  est and lock the
-0000a330: 6d20 696e 2069 6e20 7468 6174 206f 7264  m in in that ord
-0000a340: 6572 2c20 736b 6970 7069 6e67 2065 6467  er, skipping edg
-0000a350: 6573 2074 6861 7420 6372 6561 7465 2061  es that create a
-0000a360: 2063 7963 6c65 202a 616e 6420 6564 6765   cycle *and edge
-0000a370: 7320 696e 2077 6869 6368 2074 6865 7265  s in which there
-0000a380: 2069 7320 616c 7265 6164 7920 616e 2065   is already an e
-0000a390: 6467 6520 706f 696e 7469 6e67 2074 6f20  dge pointing to 
-0000a3a0: 7468 6520 7461 7267 6574 2a2e 2020 4272  the target*.  Br
-0000a3b0: 6561 6b20 7469 6573 2075 7369 6e67 2061  eak ties using a
-0000a3c0: 2074 6965 2d62 7265 616b 696e 6720 206c   tie-breaking  l
-0000a3d0: 696e 6561 7220 6f72 6465 7269 6e67 206f  inear ordering o
-0000a3e0: 7665 7220 7468 6520 6564 6765 732e 2020  ver the edges.  
-0000a3f0: 4120 6361 6e64 6964 6174 6520 6973 2061  A candidate is a
-0000a400: 2052 6976 6572 2077 696e 6e65 7220 6966   River winner if
-0000a410: 2069 7420 7769 6e73 2061 6363 6f72 6469   it wins accordi
-0000a420: 6e67 2074 6f20 736f 6d65 2074 6965 2d62  ng to some tie-b
-0000a430: 7265 616b 696e 6720 7275 6c65 2e20 5365  reaking rule. Se
-0000a440: 6520 6874 7470 733a 2f2f 656c 6563 746f  e https://electo
-0000a450: 7769 6b69 2e6f 7267 2f77 696b 692f 5269  wiki.org/wiki/Ri
-0000a460: 7665 722e 0a0a 2020 2020 4172 6773 3a0a  ver...    Args:.
-0000a470: 2020 2020 2020 2020 6564 6174 6120 2850          edata (P
-0000a480: 726f 6669 6c65 2c20 5072 6f66 696c 6557  rofile, ProfileW
-0000a490: 6974 6854 6965 732c 204d 6172 6769 6e47  ithTies, MarginG
-0000a4a0: 7261 7068 293a 2041 6e79 2065 6c65 6374  raph): Any elect
-0000a4b0: 696f 6e20 6461 7461 2074 6861 7420 6861  ion data that ha
-0000a4c0: 7320 6120 606d 6172 6769 6e60 206d 6574  s a `margin` met
-0000a4d0: 686f 642e 200a 2020 2020 2020 2020 6375  hod. .        cu
-0000a4e0: 7272 5f63 616e 6473 2028 4c69 7374 5b69  rr_cands (List[i
-0000a4f0: 6e74 5d2c 206f 7074 696f 6e61 6c29 3a20  nt], optional): 
-0000a500: 4966 2073 6574 2c20 7468 656e 2066 696e  If set, then fin
-0000a510: 6420 7468 6520 7769 6e6e 6572 7320 666f  d the winners fo
-0000a520: 7220 7468 6520 7072 6f66 696c 6520 7265  r the profile re
-0000a530: 7374 7269 6374 6564 2074 6f20 7468 6520  stricted to the 
-0000a540: 6361 6e64 6964 6174 6573 2069 6e20 6060  candidates in ``
-0000a550: 6375 7272 5f63 616e 6473 6060 0a20 2020  curr_cands``.   
-0000a560: 2020 2020 2073 7472 656e 6774 685f 6675       strength_fu
-0000a570: 6e63 7469 6f6e 2028 6675 6e63 7469 6f6e  nction (function
-0000a580: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
-0000a590: 2073 7472 656e 6774 6820 6675 6e63 7469   strength functi
-0000a5a0: 6f6e 2074 6f20 6265 2075 7365 6420 746f  on to be used to
-0000a5b0: 2063 616c 6375 6c61 7465 2074 6865 2073   calculate the s
-0000a5c0: 7472 656e 6774 6820 6f66 2061 2070 6174  trength of a pat
-0000a5d0: 682e 2020 2054 6865 2064 6566 6175 6c74  h.   The default
-0000a5e0: 2069 7320 7468 6520 6d61 7267 696e 206d   is the margin m
-0000a5f0: 6574 686f 6420 6f66 2060 6065 6461 7461  ethod of ``edata
-0000a600: 6060 2e20 2020 5468 6973 206f 6e6c 7920  ``.   This only 
-0000a610: 6d61 7474 6572 7320 7768 656e 2074 6865  matters when the
-0000a620: 2062 616c 6c6f 7473 2061 7265 206e 6f74   ballots are not
-0000a630: 206c 696e 6561 7220 6f72 6465 7273 2e20   linear orders. 
-0000a640: 0a0a 2020 2020 5265 7475 726e 733a 200a  ..    Returns: .
-0000a650: 2020 2020 2020 2020 4120 736f 7274 6564          A sorted
-0000a660: 206c 6973 7420 6f66 2063 616e 6469 6461   list of candida
-0000a670: 7465 732e 200a 0a20 2020 203a 4578 616d  tes. ..    :Exam
-0000a680: 706c 653a 200a 0a20 2020 202e 2e20 6578  ple: ..    .. ex
-0000a690: 6563 5f63 6f64 653a 3a20 0a0a 2020 2020  ec_code:: ..    
-0000a6a0: 2020 2020 6672 6f6d 2070 7265 665f 766f      from pref_vo
-0000a6b0: 7469 6e67 2e77 6569 6768 7465 645f 6d61  ting.weighted_ma
-0000a6c0: 6a6f 7269 7479 5f67 7261 7068 7320 696d  jority_graphs im
-0000a6d0: 706f 7274 204d 6172 6769 6e47 7261 7068  port MarginGraph
-0000a6e0: 0a20 2020 2020 2020 2066 726f 6d20 7072  .        from pr
-0000a6f0: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
-0000a700: 5f62 6173 6564 5f6d 6574 686f 6473 2069  _based_methods i
-0000a710: 6d70 6f72 7420 7269 7665 722c 2072 616e  mport river, ran
-0000a720: 6b65 645f 7061 6972 730a 2020 2020 2020  ked_pairs.      
-0000a730: 2020 0a20 2020 2020 2020 206d 6720 3d20    .        mg = 
-0000a740: 4d61 7267 696e 4772 6170 6828 5b30 2c20  MarginGraph([0, 
-0000a750: 312c 2032 2c20 335d 2c20 5b28 302c 2032  1, 2, 3], [(0, 2
-0000a760: 2c20 3229 2c20 2830 2c20 332c 2038 292c  , 2), (0, 3, 8),
-0000a770: 2028 312c 2030 2c20 3132 292c 2028 322c   (1, 0, 12), (2,
-0000a780: 2033 2c20 3132 292c 2028 332c 2031 2c20   3, 12), (3, 1, 
-0000a790: 3629 5d29 0a0a 2020 2020 2020 2020 7261  6)])..        ra
-0000a7a0: 6e6b 6564 5f70 6169 7273 2e64 6973 706c  nked_pairs.displ
-0000a7b0: 6179 286d 6729 0a20 2020 2020 2020 2072  ay(mg).        r
-0000a7c0: 6976 6572 2e64 6973 706c 6179 286d 6729  iver.display(mg)
-0000a7d0: 0a0a 2020 2020 2222 220a 2020 2020 6361  ..    """.    ca
-0000a7e0: 6e64 6964 6174 6573 203d 2065 6461 7461  ndidates = edata
-0000a7f0: 2e63 616e 6469 6461 7465 7320 6966 2063  .candidates if c
-0000a800: 7572 725f 6361 6e64 7320 6973 204e 6f6e  urr_cands is Non
-0000a810: 6520 656c 7365 2063 7572 725f 6361 6e64  e else curr_cand
-0000a820: 7320 2020 200a 2020 2020 6369 6478 5f74  s    .    cidx_t
-0000a830: 6f5f 6361 6e64 203d 207b 6369 6478 3a20  o_cand = {cidx: 
-0000a840: 6320 666f 7220 6369 6478 2c20 6320 696e  c for cidx, c in
-0000a850: 2065 6e75 6d65 7261 7465 2863 616e 6469   enumerate(candi
-0000a860: 6461 7465 7329 7d20 200a 2020 2020 6361  dates)}  .    ca
-0000a870: 6e64 5f74 6f5f 6369 6478 203d 207b 633a  nd_to_cidx = {c:
-0000a880: 2063 6964 7820 666f 7220 6369 6478 2c20   cidx for cidx, 
-0000a890: 6320 696e 2065 6e75 6d65 7261 7465 2863  c in enumerate(c
-0000a8a0: 616e 6469 6461 7465 7329 7d20 200a 0a20  andidates)}  .. 
-0000a8b0: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
-0000a8c0: 7469 6f6e 203d 2065 6461 7461 2e6d 6172  tion = edata.mar
-0000a8d0: 6769 6e20 6966 2073 7472 656e 6774 685f  gin if strength_
-0000a8e0: 6675 6e63 7469 6f6e 2069 7320 4e6f 6e65  function is None
-0000a8f0: 2065 6c73 6520 7374 7265 6e67 7468 5f66   else strength_f
-0000a900: 756e 6374 696f 6e20 2020 200a 0a20 2020  unction    ..   
-0000a910: 2063 7720 3d20 6564 6174 612e 636f 6e64   cw = edata.cond
-0000a920: 6f72 6365 745f 7769 6e6e 6572 2863 7572  orcet_winner(cur
-0000a930: 725f 6361 6e64 733d 6375 7272 5f63 616e  r_cands=curr_can
-0000a940: 6473 290a 2020 2020 2320 5261 6e6b 6564  ds).    # Ranked
-0000a950: 2050 6169 7273 2069 7320 436f 6e64 6f72   Pairs is Condor
-0000a960: 6365 7420 636f 6e73 6973 7465 6e74 2c20  cet consistent, 
-0000a970: 736f 2073 696d 706c 7920 7265 7475 726e  so simply return
-0000a980: 2074 6865 2043 6f6e 646f 7263 6574 2077   the Condorcet w
-0000a990: 696e 6e65 7220 6966 2065 7869 7374 730a  inner if exists.
-0000a9a0: 2020 2020 6966 2063 7720 6973 206e 6f74      if cw is not
-0000a9b0: 204e 6f6e 653a 200a 2020 2020 2020 2020   None: .        
-0000a9c0: 7769 6e6e 6572 7320 3d20 5b63 775d 0a20  winners = [cw]. 
-0000a9d0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000a9e0: 2077 5f65 6467 6573 203d 205b 2863 312c   w_edges = [(c1,
-0000a9f0: 2063 322c 2073 7472 656e 6774 685f 6675   c2, strength_fu
-0000aa00: 6e63 7469 6f6e 2863 312c 2063 3229 2920  nction(c1, c2)) 
-0000aa10: 666f 7220 6331 2069 6e20 6361 6e64 6964  for c1 in candid
-0000aa20: 6174 6573 2066 6f72 2063 3220 696e 2063  ates for c2 in c
-0000aa30: 616e 6469 6461 7465 7320 0a20 2020 2020  andidates .     
-0000aa40: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000aa50: 2063 3120 213d 2063 3220 616e 6420 2865   c1 != c2 and (e
-0000aa60: 6461 7461 2e6d 616a 6f72 6974 795f 7072  data.majority_pr
-0000aa70: 6566 6572 7328 6331 2c20 6332 2920 6f72  efers(c1, c2) or
-0000aa80: 2065 6461 7461 2e69 735f 7469 6564 2863   edata.is_tied(c
-0000aa90: 312c 2063 3229 295d 0a20 2020 2020 2020  1, c2))].       
-0000aaa0: 2077 696e 6e65 7273 203d 206c 6973 7428   winners = list(
-0000aab0: 2920 2020 2020 2020 2020 2020 200a 2020  )            .  
-0000aac0: 2020 2020 2020 7374 7265 6e67 7468 7320        strengths 
-0000aad0: 3d20 736f 7274 6564 286c 6973 7428 7365  = sorted(list(se
-0000aae0: 7428 5b65 5b32 5d20 666f 7220 6520 696e  t([e[2] for e in
-0000aaf0: 2077 5f65 6467 6573 5d29 292c 2072 6576   w_edges])), rev
-0000ab00: 6572 7365 3d54 7275 6529 0a20 2020 2020  erse=True).     
-0000ab10: 2020 2073 6f72 7465 645f 6564 6765 7320     sorted_edges 
-0000ab20: 3d20 5b5b 6520 666f 7220 6520 696e 2077  = [[e for e in w
-0000ab30: 5f65 6467 6573 2069 6620 655b 325d 203d  _edges if e[2] =
-0000ab40: 3d20 735d 2066 6f72 2073 2069 6e20 7374  = s] for s in st
-0000ab50: 7265 6e67 7468 735d 0a20 2020 2020 2020  rengths].       
-0000ab60: 2074 6273 203d 2070 726f 6475 6374 282a   tbs = product(*
-0000ab70: 5b70 6572 6d75 7461 7469 6f6e 7328 6564  [permutations(ed
-0000ab80: 6765 7329 2066 6f72 2065 6467 6573 2069  ges) for edges i
-0000ab90: 6e20 736f 7274 6564 5f65 6467 6573 5d29  n sorted_edges])
-0000aba0: 0a20 2020 2020 2020 2066 6f72 2074 6220  .        for tb 
-0000abb0: 696e 2074 6273 3a0a 2020 2020 2020 2020  in tbs:.        
-0000abc0: 2020 2020 6564 6765 7320 3d20 666c 6174      edges = flat
-0000abd0: 7465 6e28 7462 290a 2020 2020 2020 2020  ten(tb).        
-0000abe0: 2020 2020 7276 5f64 6566 6561 7420 3d20      rv_defeat = 
-0000abf0: 5350 4f28 6c65 6e28 6361 6e64 6964 6174  SPO(len(candidat
-0000ac00: 6573 2929 0a20 2020 2020 2020 2020 2020  es)).           
-0000ac10: 2066 6f72 2065 302c 6531 2c73 2069 6e20   for e0,e1,s in 
-0000ac20: 6564 6765 733a 200a 2020 2020 2020 2020  edges: .        
-0000ac30: 2020 2020 2020 2020 6966 206e 6f74 2072          if not r
-0000ac40: 765f 6465 6665 6174 2e50 5b63 616e 645f  v_defeat.P[cand_
-0000ac50: 746f 5f63 6964 785b 6531 5d5d 5b63 616e  to_cidx[e1]][can
-0000ac60: 645f 746f 5f63 6964 785b 6530 5d5d 2061  d_to_cidx[e0]] a
-0000ac70: 6e64 206c 656e 2872 765f 6465 6665 6174  nd len(rv_defeat
-0000ac80: 2e70 7265 6473 5b63 616e 645f 746f 5f63  .preds[cand_to_c
-0000ac90: 6964 785b 6531 5d5d 2920 3d3d 2030 3a0a  idx[e1]]) == 0:.
-0000aca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000acb0: 2020 2020 7276 5f64 6566 6561 742e 6164      rv_defeat.ad
-0000acc0: 6428 6361 6e64 5f74 6f5f 6369 6478 5b65  d(cand_to_cidx[e
-0000acd0: 305d 2c63 616e 645f 746f 5f63 6964 785b  0],cand_to_cidx[
-0000ace0: 6531 5d29 0a20 2020 2020 2020 2020 2020  e1]).           
-0000acf0: 2077 696e 6e65 7273 2e61 7070 656e 6428   winners.append(
-0000ad00: 6369 6478 5f74 6f5f 6361 6e64 5b72 765f  cidx_to_cand[rv_
-0000ad10: 6465 6665 6174 2e69 6e69 7469 616c 5f65  defeat.initial_e
-0000ad20: 6c65 6d65 6e74 7328 295b 305d 5d29 0a0a  lements()[0]])..
-0000ad30: 2020 2020 7265 7475 726e 2073 6f72 7465      return sorte
-0000ad40: 6428 6c69 7374 2873 6574 2877 696e 6e65  d(list(set(winne
-0000ad50: 7273 2929 290a 0a64 6566 2072 6976 6572  rs)))..def river
-0000ad60: 5f64 6566 6561 7473 2865 6461 7461 2c20  _defeats(edata, 
-0000ad70: 6375 7272 5f63 616e 6473 203d 204e 6f6e  curr_cands = Non
-0000ad80: 652c 2073 7472 656e 6774 685f 6675 6e63  e, strength_func
-0000ad90: 7469 6f6e 203d 204e 6f6e 6529 3a0a 2020  tion = None):.  
-0000ada0: 2020 2222 220a 2020 2020 5265 7475 726e    """.    Return
-0000adb0: 7320 7468 6520 5269 7665 7220 6465 6665  s the River defe
-0000adc0: 6174 2072 656c 6174 696f 6e73 2070 726f  at relations pro
-0000add0: 6475 6365 6420 6279 2074 6865 2052 6976  duced by the Riv
-0000ade0: 6572 2061 6c67 6f72 6974 686d 2e0a 0a20  er algorithm... 
-0000adf0: 2020 202e 2e20 696d 706f 7274 616e 743a     .. important:
-0000ae00: 3a0a 2020 2020 2020 2020 556e 6c69 6b65  :.        Unlike
-0000ae10: 2074 6865 206f 7468 6572 2066 756e 6374   the other funct
-0000ae20: 696f 6e73 2074 6861 7420 7265 7475 726e  ions that return
-0000ae30: 2061 2073 696e 676c 6520 6465 6665 6174   a single defeat
-0000ae40: 2072 656c 6174 696f 6e2c 2074 6869 7320   relation, this 
-0000ae50: 7265 7475 726e 7320 6120 6c69 7374 206f  returns a list o
-0000ae60: 6620 6465 6665 6174 2072 656c 6174 696f  f defeat relatio
-0000ae70: 6e73 2e20 0a20 2020 2020 2020 200a 2020  ns. .        .  
-0000ae80: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-0000ae90: 6564 6174 6120 2850 726f 6669 6c65 2c20  edata (Profile, 
-0000aea0: 5072 6f66 696c 6557 6974 6854 6965 732c  ProfileWithTies,
-0000aeb0: 204d 6172 6769 6e47 7261 7068 293a 2041   MarginGraph): A
-0000aec0: 6e79 2065 6c65 6374 696f 6e20 6461 7461  ny election data
-0000aed0: 2074 6861 7420 6861 7320 6120 606d 6172   that has a `mar
-0000aee0: 6769 6e60 206d 6574 686f 642e 200a 2020  gin` method. .  
-0000aef0: 2020 2020 2020 6375 7272 5f63 616e 6473        curr_cands
-0000af00: 2028 4c69 7374 5b69 6e74 5d2c 206f 7074   (List[int], opt
-0000af10: 696f 6e61 6c29 3a20 4966 2073 6574 2c20  ional): If set, 
-0000af20: 7468 656e 2066 696e 6420 7468 6520 7769  then find the wi
-0000af30: 6e6e 6572 7320 666f 7220 7468 6520 7072  nners for the pr
-0000af40: 6f66 696c 6520 7265 7374 7269 6374 6564  ofile restricted
-0000af50: 2074 6f20 7468 6520 6361 6e64 6964 6174   to the candidat
-0000af60: 6573 2069 6e20 6060 6375 7272 5f63 616e  es in ``curr_can
-0000af70: 6473 6060 0a20 2020 2020 2020 2073 7472  ds``.        str
-0000af80: 656e 6774 685f 6675 6e63 7469 6f6e 2028  ength_function (
-0000af90: 6675 6e63 7469 6f6e 2c20 6f70 7469 6f6e  function, option
-0000afa0: 616c 293a 2054 6865 2073 7472 656e 6774  al): The strengt
-0000afb0: 6820 6675 6e63 7469 6f6e 2074 6f20 6265  h function to be
-0000afc0: 2075 7365 6420 746f 2063 616c 6375 6c61   used to calcula
-0000afd0: 7465 2074 6865 2073 7472 656e 6774 6820  te the strength 
-0000afe0: 6f66 2061 2070 6174 682e 2020 2054 6865  of a path.   The
-0000aff0: 2064 6566 6175 6c74 2069 7320 7468 6520   default is the 
-0000b000: 6d61 7267 696e 206d 6574 686f 6420 6f66  margin method of
-0000b010: 2060 6065 6461 7461 6060 2e20 2020 5468   ``edata``.   Th
-0000b020: 6973 206f 6e6c 7920 6d61 7474 6572 7320  is only matters 
-0000b030: 7768 656e 2074 6865 2062 616c 6c6f 7473  when the ballots
-0000b040: 2061 7265 206e 6f74 206c 696e 6561 7220   are not linear 
-0000b050: 6f72 6465 7273 2e20 0a0a 2020 2020 5265  orders. ..    Re
-0000b060: 7475 726e 733a 200a 2020 2020 2020 2020  turns: .        
-0000b070: 4120 6e65 7477 6f72 6b78 2044 6947 7261  A networkx DiGra
-0000b080: 7068 2072 6570 7265 7365 6e74 696e 6720  ph representing 
-0000b090: 7468 6520 5269 7665 7220 6465 6665 6174  the River defeat
-0000b0a0: 2072 656c 6174 696f 6e2e 200a 2020 2020   relation. .    
-0000b0b0: 2222 220a 0a20 2020 2063 616e 6469 6461  """..    candida
-0000b0c0: 7465 7320 3d20 6564 6174 612e 6361 6e64  tes = edata.cand
-0000b0d0: 6964 6174 6573 2069 6620 6375 7272 5f63  idates if curr_c
-0000b0e0: 616e 6473 2069 7320 4e6f 6e65 2065 6c73  ands is None els
-0000b0f0: 6520 6375 7272 5f63 616e 6473 2020 2020  e curr_cands    
-0000b100: 0a20 2020 2073 7472 656e 6774 685f 6675  .    strength_fu
-0000b110: 6e63 7469 6f6e 203d 2065 6461 7461 2e6d  nction = edata.m
-0000b120: 6172 6769 6e20 6966 2073 7472 656e 6774  argin if strengt
-0000b130: 685f 6675 6e63 7469 6f6e 2069 7320 4e6f  h_function is No
-0000b140: 6e65 2065 6c73 6520 7374 7265 6e67 7468  ne else strength
-0000b150: 5f66 756e 6374 696f 6e20 2020 200a 0a20  _function    .. 
-0000b160: 2020 2077 5f65 6467 6573 203d 205b 2863     w_edges = [(c
-0000b170: 312c 2063 322c 2073 7472 656e 6774 685f  1, c2, strength_
-0000b180: 6675 6e63 7469 6f6e 2863 312c 2063 3229  function(c1, c2)
-0000b190: 2920 666f 7220 6331 2069 6e20 6361 6e64  ) for c1 in cand
-0000b1a0: 6964 6174 6573 2066 6f72 2063 3220 696e  idates for c2 in
-0000b1b0: 2063 616e 6469 6461 7465 7320 6966 2063   candidates if c
-0000b1c0: 3120 213d 2063 3220 616e 6420 2865 6461  1 != c2 and (eda
-0000b1d0: 7461 2e6d 616a 6f72 6974 795f 7072 6566  ta.majority_pref
-0000b1e0: 6572 7328 6331 2c20 6332 2920 6f72 2065  ers(c1, c2) or e
-0000b1f0: 6461 7461 2e69 735f 7469 6564 2863 312c  data.is_tied(c1,
-0000b200: 2063 3229 295d 0a0a 2020 2020 7374 7265   c2))]..    stre
-0000b210: 6e67 7468 7320 3d20 736f 7274 6564 286c  ngths = sorted(l
-0000b220: 6973 7428 7365 7428 5b65 5b32 5d20 666f  ist(set([e[2] fo
-0000b230: 7220 6520 696e 2077 5f65 6467 6573 5d29  r e in w_edges])
-0000b240: 292c 2072 6576 6572 7365 3d54 7275 6529  ), reverse=True)
-0000b250: 0a20 2020 2073 6f72 7465 645f 6564 6765  .    sorted_edge
-0000b260: 7320 3d20 5b5b 6520 666f 7220 6520 696e  s = [[e for e in
-0000b270: 2077 5f65 6467 6573 2069 6620 655b 325d   w_edges if e[2]
-0000b280: 203d 3d20 735d 2066 6f72 2073 2069 6e20   == s] for s in 
-0000b290: 7374 7265 6e67 7468 735d 0a20 2020 2074  strengths].    t
-0000b2a0: 6273 203d 2070 726f 6475 6374 282a 5b70  bs = product(*[p
-0000b2b0: 6572 6d75 7461 7469 6f6e 7328 6564 6765  ermutations(edge
-0000b2c0: 7329 2066 6f72 2065 6467 6573 2069 6e20  s) for edges in 
-0000b2d0: 736f 7274 6564 5f65 6467 6573 5d29 0a0a  sorted_edges])..
-0000b2e0: 2020 2020 7269 7665 725f 6465 6665 6174      river_defeat
-0000b2f0: 7320 3d20 6c69 7374 2829 0a20 2020 2066  s = list().    f
-0000b300: 6f72 2074 6220 696e 2074 6273 3a0a 2020  or tb in tbs:.  
-0000b310: 2020 2020 2020 6564 6765 7320 3d20 666c        edges = fl
-0000b320: 6174 7465 6e28 7462 290a 2020 2020 2020  atten(tb).      
-0000b330: 2020 7269 7665 725f 6465 6665 6174 203d    river_defeat =
-0000b340: 206e 782e 4469 4772 6170 6828 2920 0a20   nx.DiGraph() . 
-0000b350: 2020 2020 2020 2066 6f72 2065 2069 6e20         for e in 
-0000b360: 6564 6765 733a 200a 2020 2020 2020 2020  edges: .        
-0000b370: 2020 2020 6966 2065 5b31 5d20 6e6f 7420      if e[1] not 
-0000b380: 696e 2072 6976 6572 5f64 6566 6561 742e  in river_defeat.
-0000b390: 6e6f 6465 7320 6f72 206c 656e 286c 6973  nodes or len(lis
-0000b3a0: 7428 7269 7665 725f 6465 6665 6174 2e69  t(river_defeat.i
-0000b3b0: 6e5f 6564 6765 7328 655b 315d 2929 2920  n_edges(e[1]))) 
-0000b3c0: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
-0000b3d0: 2020 2020 2020 7269 7665 725f 6465 6665        river_defe
-0000b3e0: 6174 2e61 6464 5f65 6467 6528 655b 305d  at.add_edge(e[0]
-0000b3f0: 2c20 655b 315d 2c20 7765 6967 6874 3d65  , e[1], weight=e
-0000b400: 5b32 5d29 0a20 2020 2020 2020 2020 2020  [2]).           
-0000b410: 2020 2020 2069 6620 646f 6573 5f63 7265       if does_cre
-0000b420: 6174 655f 6379 636c 6528 7269 7665 725f  ate_cycle(river_
-0000b430: 6465 6665 6174 2c20 6529 3a0a 2020 2020  defeat, e):.    
-0000b440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b450: 7269 7665 725f 6465 6665 6174 2e72 656d  river_defeat.rem
-0000b460: 6f76 655f 6564 6765 2865 5b30 5d2c 2065  ove_edge(e[0], e
-0000b470: 5b31 5d29 0a20 2020 2020 2020 2020 2020  [1]).           
-0000b480: 200a 2020 2020 2020 2020 7269 7665 725f   .        river_
-0000b490: 6465 6665 6174 732e 6170 7065 6e64 2872  defeats.append(r
-0000b4a0: 6976 6572 5f64 6566 6561 7429 0a0a 2020  iver_defeat)..  
-0000b4b0: 2020 7265 7475 726e 2072 6976 6572 5f64    return river_d
-0000b4c0: 6566 6561 7473 0a0a 4076 6d28 6e61 6d65  efeats..@vm(name
-0000b4d0: 3d22 5269 7665 7222 290a 6465 6620 7269  ="River").def ri
-0000b4e0: 7665 725f 7769 7468 5f74 6573 7428 6564  ver_with_test(ed
-0000b4f0: 6174 612c 2063 7572 725f 6361 6e64 7320  ata, curr_cands 
-0000b500: 3d20 4e6f 6e65 2c20 7374 7265 6e67 7468  = None, strength
-0000b510: 5f66 756e 6374 696f 6e20 3d20 4e6f 6e65  _function = None
-0000b520: 293a 2020 200a 2020 2020 2222 2246 696e  ):   .    """Fin
-0000b530: 6420 7468 6520 5269 7665 7220 7769 6e6e  d the River winn
-0000b540: 6572 7320 7769 7468 2061 2074 6573 7420  ers with a test 
-0000b550: 746f 2064 6574 6572 6d69 6e65 6420 6966  to determined if
-0000b560: 2069 7420 7769 6c6c 2074 616b 6520 746f   it will take to
-0000b570: 6f20 6c6f 6e67 2074 6f20 636f 6d70 7574  o long to comput
-0000b580: 6520 7468 6520 5269 7665 7220 7769 6e6e  e the River winn
-0000b590: 6572 732e 2049 6620 7468 6520 6361 6c63  ers. If the calc
-0000b5a0: 756c 6174 696f 6e20 6f66 2074 6865 2077  ulation of the w
-0000b5b0: 696e 6e65 7273 2077 696c 6c20 7461 6b65  inners will take
-0000b5c0: 2074 6f6f 206c 6f6e 672c 2072 6574 7572   too long, retur
-0000b5d0: 6e20 4e6f 6e65 2e20 0a20 2020 2020 2020  n None. .       
-0000b5e0: 200a 2020 2020 2e2e 2069 6d70 6f72 7461   .    .. importa
-0000b5f0: 6e74 3a3a 0a20 2020 2020 2020 2054 6869  nt::.        Thi
-0000b600: 7320 766f 7469 6e67 206d 6574 686f 6420  s voting method 
-0000b610: 7468 6174 206d 6967 6874 2072 6574 7572  that might retur
-0000b620: 6e20 4e6f 6e65 2072 6174 6865 7220 7468  n None rather th
-0000b630: 616e 2061 206c 6973 7420 6f66 2063 616e  an a list of can
-0000b640: 6469 6461 7465 732e 2020 0a0a 2020 2020  didates.  ..    
-0000b650: 4172 6773 3a0a 2020 2020 2020 2020 6564  Args:.        ed
-0000b660: 6174 6120 2850 726f 6669 6c65 2c20 5072  ata (Profile, Pr
-0000b670: 6f66 696c 6557 6974 6854 6965 732c 204d  ofileWithTies, M
-0000b680: 6172 6769 6e47 7261 7068 293a 2041 6e79  arginGraph): Any
-0000b690: 2065 6c65 6374 696f 6e20 6461 7461 2074   election data t
-0000b6a0: 6861 7420 6861 7320 6120 606d 6172 6769  hat has a `margi
-0000b6b0: 6e60 206d 6574 686f 642e 200a 2020 2020  n` method. .    
-0000b6c0: 2020 2020 6375 7272 5f63 616e 6473 2028      curr_cands (
-0000b6d0: 4c69 7374 5b69 6e74 5d2c 206f 7074 696f  List[int], optio
-0000b6e0: 6e61 6c29 3a20 4966 2073 6574 2c20 7468  nal): If set, th
-0000b6f0: 656e 2066 696e 6420 7468 6520 7769 6e6e  en find the winn
-0000b700: 6572 7320 666f 7220 7468 6520 7072 6f66  ers for the prof
-0000b710: 696c 6520 7265 7374 7269 6374 6564 2074  ile restricted t
-0000b720: 6f20 7468 6520 6361 6e64 6964 6174 6573  o the candidates
-0000b730: 2069 6e20 6060 6375 7272 5f63 616e 6473   in ``curr_cands
-0000b740: 6060 0a20 2020 2020 2020 2073 7472 656e  ``.        stren
-0000b750: 6774 685f 6675 6e63 7469 6f6e 2028 6675  gth_function (fu
-0000b760: 6e63 7469 6f6e 2c20 6f70 7469 6f6e 616c  nction, optional
-0000b770: 293a 2054 6865 2073 7472 656e 6774 6820  ): The strength 
-0000b780: 6675 6e63 7469 6f6e 2074 6f20 6265 2075  function to be u
-0000b790: 7365 6420 746f 2063 616c 6375 6c61 7465  sed to calculate
-0000b7a0: 2074 6865 2073 7472 656e 6774 6820 6f66   the strength of
-0000b7b0: 2061 2070 6174 682e 2020 2054 6865 2064   a path.   The d
-0000b7c0: 6566 6175 6c74 2069 7320 7468 6520 6d61  efault is the ma
-0000b7d0: 7267 696e 206d 6574 686f 6420 6f66 2060  rgin method of `
-0000b7e0: 6065 6461 7461 6060 2e20 2020 5468 6973  `edata``.   This
-0000b7f0: 206f 6e6c 7920 6d61 7474 6572 7320 7768   only matters wh
-0000b800: 656e 2074 6865 2062 616c 6c6f 7473 2061  en the ballots a
-0000b810: 7265 206e 6f74 206c 696e 6561 7220 6f72  re not linear or
-0000b820: 6465 7273 2e20 0a0a 2020 2020 5265 7475  ders. ..    Retu
-0000b830: 726e 733a 200a 2020 2020 2020 2020 4120  rns: .        A 
-0000b840: 736f 7274 6564 206c 6973 7420 6f66 2063  sorted list of c
-0000b850: 616e 6469 6461 7465 732e 200a 0a20 2020  andidates. ..   
-0000b860: 202e 2e20 7365 6561 6c73 6f3a 3a0a 0a20   .. seealso::.. 
-0000b870: 2020 2020 2020 203a 6d65 7468 3a60 7072         :meth:`pr
-0000b880: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
-0000b890: 5f62 6173 6564 5f6d 6574 686f 6473 2e72  _based_methods.r
-0000b8a0: 616e 6b65 645f 7061 6972 735f 7769 7468  anked_pairs_with
-0000b8b0: 5f74 6573 7460 2c20 3a6d 6574 683a 6070  _test`, :meth:`p
-0000b8c0: 7265 665f 766f 7469 6e67 2e6d 6172 6769  ref_voting.margi
-0000b8d0: 6e5f 6261 7365 645f 6d65 7468 6f64 732e  n_based_methods.
-0000b8e0: 7269 7665 7260 0a0a 2020 2020 2222 220a  river`..    """.
-0000b8f0: 2020 2020 6361 6e64 6964 6174 6573 203d      candidates =
-0000b900: 2065 6461 7461 2e63 616e 6469 6461 7465   edata.candidate
-0000b910: 7320 6966 2063 7572 725f 6361 6e64 7320  s if curr_cands 
-0000b920: 6973 204e 6f6e 6520 656c 7365 2063 7572  is None else cur
-0000b930: 725f 6361 6e64 7320 2020 200a 2020 2020  r_cands    .    
-0000b940: 6369 6478 5f74 6f5f 6361 6e64 203d 207b  cidx_to_cand = {
-0000b950: 6369 6478 3a20 6320 666f 7220 6369 6478  cidx: c for cidx
-0000b960: 2c20 6320 696e 2065 6e75 6d65 7261 7465  , c in enumerate
-0000b970: 2863 616e 6469 6461 7465 7329 7d20 200a  (candidates)}  .
-0000b980: 2020 2020 6361 6e64 5f74 6f5f 6369 6478      cand_to_cidx
-0000b990: 203d 207b 633a 2063 6964 7820 666f 7220   = {c: cidx for 
-0000b9a0: 6369 6478 2c20 6320 696e 2065 6e75 6d65  cidx, c in enume
-0000b9b0: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
-0000b9c0: 7d20 200a 0a20 2020 2073 7472 656e 6774  }  ..    strengt
-0000b9d0: 685f 6675 6e63 7469 6f6e 203d 2065 6461  h_function = eda
-0000b9e0: 7461 2e6d 6172 6769 6e20 6966 2073 7472  ta.margin if str
-0000b9f0: 656e 6774 685f 6675 6e63 7469 6f6e 2069  ength_function i
-0000ba00: 7320 4e6f 6e65 2065 6c73 6520 7374 7265  s None else stre
-0000ba10: 6e67 7468 5f66 756e 6374 696f 6e20 2020  ngth_function   
-0000ba20: 200a 0a20 2020 2063 7720 3d20 6564 6174   ..    cw = edat
-0000ba30: 612e 636f 6e64 6f72 6365 745f 7769 6e6e  a.condorcet_winn
-0000ba40: 6572 2863 7572 725f 6361 6e64 733d 6375  er(curr_cands=cu
-0000ba50: 7272 5f63 616e 6473 290a 2020 2020 2320  rr_cands).    # 
-0000ba60: 5261 6e6b 6564 2050 6169 7273 2069 7320  Ranked Pairs is 
-0000ba70: 436f 6e64 6f72 6365 7420 636f 6e73 6973  Condorcet consis
-0000ba80: 7465 6e74 2c20 736f 2073 696d 706c 7920  tent, so simply 
-0000ba90: 7265 7475 726e 2074 6865 2043 6f6e 646f  return the Condo
-0000baa0: 7263 6574 2077 696e 6e65 7220 6966 2065  rcet winner if e
-0000bab0: 7869 7374 730a 2020 2020 6966 2063 7720  xists.    if cw 
-0000bac0: 6973 206e 6f74 204e 6f6e 653a 200a 2020  is not None: .  
-0000bad0: 2020 2020 2020 7769 6e6e 6572 7320 3d20        winners = 
-0000bae0: 5b63 775d 0a20 2020 2065 6c73 653a 0a20  [cw].    else:. 
-0000baf0: 2020 2020 2020 2077 5f65 6467 6573 203d         w_edges =
-0000bb00: 205b 2863 312c 2063 322c 2073 7472 656e   [(c1, c2, stren
-0000bb10: 6774 685f 6675 6e63 7469 6f6e 2863 312c  gth_function(c1,
-0000bb20: 2063 3229 2920 666f 7220 6331 2069 6e20   c2)) for c1 in 
-0000bb30: 6361 6e64 6964 6174 6573 2066 6f72 2063  candidates for c
-0000bb40: 3220 696e 2063 616e 6469 6461 7465 7320  2 in candidates 
-0000bb50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bb60: 2020 2020 6966 2063 3120 213d 2063 3220      if c1 != c2 
-0000bb70: 616e 6420 2865 6461 7461 2e6d 616a 6f72  and (edata.major
-0000bb80: 6974 795f 7072 6566 6572 7328 6331 2c20  ity_prefers(c1, 
-0000bb90: 6332 2920 6f72 2065 6461 7461 2e69 735f  c2) or edata.is_
-0000bba0: 7469 6564 2863 312c 2063 3229 295d 0a20  tied(c1, c2))]. 
-0000bbb0: 2020 2020 2020 2077 696e 6e65 7273 203d         winners =
-0000bbc0: 206c 6973 7428 2920 2020 2020 2020 2020   list()         
-0000bbd0: 2020 200a 2020 2020 2020 2020 7374 7265     .        stre
-0000bbe0: 6e67 7468 7320 3d20 736f 7274 6564 286c  ngths = sorted(l
-0000bbf0: 6973 7428 7365 7428 5b65 5b32 5d20 666f  ist(set([e[2] fo
-0000bc00: 7220 6520 696e 2077 5f65 6467 6573 5d29  r e in w_edges])
-0000bc10: 292c 2072 6576 6572 7365 3d54 7275 6529  ), reverse=True)
-0000bc20: 0a20 2020 2020 2020 2073 6f72 7465 645f  .        sorted_
-0000bc30: 6564 6765 7320 3d20 5b5b 6520 666f 7220  edges = [[e for 
-0000bc40: 6520 696e 2077 5f65 6467 6573 2069 6620  e in w_edges if 
-0000bc50: 655b 325d 203d 3d20 735d 2066 6f72 2073  e[2] == s] for s
-0000bc60: 2069 6e20 7374 7265 6e67 7468 735d 0a20   in strengths]. 
-0000bc70: 2020 2020 2020 2069 6620 6e70 2e70 726f         if np.pro
-0000bc80: 6428 5b6d 6174 682e 6661 6374 6f72 6961  d([math.factoria
-0000bc90: 6c28 6c65 6e28 6573 2929 2066 6f72 2065  l(len(es)) for e
-0000bca0: 7320 696e 2073 6f72 7465 645f 6564 6765  s in sorted_edge
-0000bcb0: 735d 2920 3e20 3330 3030 3a20 0a20 2020  s]) > 3000: .   
-0000bcc0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000bcd0: 4e6f 6e65 0a20 2020 2020 2020 2065 6c73  None.        els
-0000bce0: 653a 200a 2020 2020 2020 2020 2020 2020  e: .            
-0000bcf0: 7462 7320 3d20 7072 6f64 7563 7428 2a5b  tbs = product(*[
-0000bd00: 7065 726d 7574 6174 696f 6e73 2865 6467  permutations(edg
-0000bd10: 6573 2920 666f 7220 6564 6765 7320 696e  es) for edges in
-0000bd20: 2073 6f72 7465 645f 6564 6765 735d 290a   sorted_edges]).
-0000bd30: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000bd40: 7462 2069 6e20 7462 733a 0a20 2020 2020  tb in tbs:.     
-0000bd50: 2020 2020 2020 2020 2020 2065 6467 6573             edges
-0000bd60: 203d 2066 6c61 7474 656e 2874 6229 0a20   = flatten(tb). 
-0000bd70: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000bd80: 765f 6465 6665 6174 203d 2053 504f 286c  v_defeat = SPO(l
-0000bd90: 656e 2863 616e 6469 6461 7465 7329 290a  en(candidates)).
-0000bda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bdb0: 666f 7220 6530 2c65 312c 7320 696e 2065  for e0,e1,s in e
-0000bdc0: 6467 6573 3a20 0a20 2020 2020 2020 2020  dges: .         
-0000bdd0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-0000bde0: 7420 7276 5f64 6566 6561 742e 505b 6361  t rv_defeat.P[ca
-0000bdf0: 6e64 5f74 6f5f 6369 6478 5b65 315d 5d5b  nd_to_cidx[e1]][
-0000be00: 6361 6e64 5f74 6f5f 6369 6478 5b65 305d  cand_to_cidx[e0]
-0000be10: 5d20 616e 6420 6c65 6e28 7276 5f64 6566  ] and len(rv_def
-0000be20: 6561 742e 7072 6564 735b 6361 6e64 5f74  eat.preds[cand_t
-0000be30: 6f5f 6369 6478 5b65 315d 5d29 203d 3d20  o_cidx[e1]]) == 
-0000be40: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
-0000be50: 2020 2020 2020 2020 2020 2072 765f 6465             rv_de
-0000be60: 6665 6174 2e61 6464 2863 616e 645f 746f  feat.add(cand_to
-0000be70: 5f63 6964 785b 6530 5d2c 6361 6e64 5f74  _cidx[e0],cand_t
-0000be80: 6f5f 6369 6478 5b65 315d 290a 2020 2020  o_cidx[e1]).    
-0000be90: 2020 2020 2020 2020 2020 2020 7769 6e6e              winn
-0000bea0: 6572 732e 6170 7065 6e64 2863 6964 785f  ers.append(cidx_
-0000beb0: 746f 5f63 616e 645b 7276 5f64 6566 6561  to_cand[rv_defea
-0000bec0: 742e 696e 6974 6961 6c5f 656c 656d 656e  t.initial_elemen
-0000bed0: 7473 2829 5b30 5d5d 290a 2020 2020 7265  ts()[0]]).    re
-0000bee0: 7475 726e 2073 6f72 7465 6428 6c69 7374  turn sorted(list
-0000bef0: 2873 6574 2877 696e 6e65 7273 2929 290a  (set(winners))).
-0000bf00: 0a40 766d 286e 616d 653d 2252 6976 6572  .@vm(name="River
-0000bf10: 2054 4222 290a 6465 6620 7269 7665 725f   TB").def river_
-0000bf20: 7462 2865 6461 7461 2c20 6375 7272 5f63  tb(edata, curr_c
-0000bf30: 616e 6473 203d 204e 6f6e 652c 2074 6965  ands = None, tie
-0000bf40: 5f62 7265 616b 6572 203d 204e 6f6e 652c  _breaker = None,
-0000bf50: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-0000bf60: 6f6e 203d 204e 6f6e 6529 3a20 2020 0a20  on = None):   . 
-0000bf70: 2020 2022 2222 0a20 2020 2052 6976 6572     """.    River
-0000bf80: 2077 6974 6820 6120 6669 7865 6420 6c69   with a fixed li
-0000bf90: 6e65 6172 206f 7264 6572 206f 6e20 7468  near order on th
-0000bfa0: 6520 6361 6e64 6964 6174 6573 2074 6f20  e candidates to 
-0000bfb0: 6272 6561 6b20 616e 7920 7469 6573 2069  break any ties i
-0000bfc0: 6e20 7468 6520 6d61 7267 696e 732e 2020  n the margins.  
-0000bfd0: 5369 6e63 6520 7468 6520 7469 655f 6272  Since the tie_br
-0000bfe0: 6561 6b65 7220 6973 2061 206c 696e 6561  eaker is a linea
-0000bff0: 7220 6f72 6465 722c 2074 6869 7320 6d65  r order, this me
-0000c000: 7468 6f64 2069 7320 7265 736f 6c75 7465  thod is resolute
-0000c010: 2e20 2020 0a0a 2020 2020 4172 6773 3a0a  .   ..    Args:.
-0000c020: 2020 2020 2020 2020 6564 6174 6120 2850          edata (P
-0000c030: 726f 6669 6c65 2c20 5072 6f66 696c 6557  rofile, ProfileW
-0000c040: 6974 6854 6965 732c 204d 6172 6769 6e47  ithTies, MarginG
-0000c050: 7261 7068 293a 2041 6e79 2065 6c65 6374  raph): Any elect
-0000c060: 696f 6e20 6461 7461 2074 6861 7420 6861  ion data that ha
-0000c070: 7320 6120 606d 6172 6769 6e60 206d 6574  s a `margin` met
-0000c080: 686f 642e 200a 2020 2020 2020 2020 6375  hod. .        cu
-0000c090: 7272 5f63 616e 6473 2028 4c69 7374 5b69  rr_cands (List[i
-0000c0a0: 6e74 5d2c 206f 7074 696f 6e61 6c29 3a20  nt], optional): 
-0000c0b0: 4966 2073 6574 2c20 7468 656e 2066 696e  If set, then fin
-0000c0c0: 6420 7468 6520 7769 6e6e 6572 7320 666f  d the winners fo
-0000c0d0: 7220 7468 6520 7072 6f66 696c 6520 7265  r the profile re
-0000c0e0: 7374 7269 6374 6564 2074 6f20 7468 6520  stricted to the 
-0000c0f0: 6361 6e64 6964 6174 6573 2069 6e20 6060  candidates in ``
-0000c100: 6375 7272 5f63 616e 6473 6060 0a20 2020  curr_cands``.   
-0000c110: 2020 2020 2074 6965 5f62 7265 616b 6572       tie_breaker
-0000c120: 2028 4c69 7374 5b69 6e74 5d2c 206f 7074   (List[int], opt
-0000c130: 696f 6e61 6c29 3a20 4120 6c69 6e65 6172  ional): A linear
-0000c140: 206f 7264 6572 206f 6e20 7468 6520 6361   order on the ca
-0000c150: 6e64 6964 6174 6573 2e20 2049 6620 6e6f  ndidates.  If no
-0000c160: 7420 7365 742c 2074 6865 6e20 7468 6520  t set, then the 
-0000c170: 6361 6e64 6964 6174 6573 2061 7265 2073  candidates are s
-0000c180: 6f72 7465 6420 696e 2061 7363 656e 6469  orted in ascendi
-0000c190: 6e67 206f 7264 6572 2e0a 2020 2020 2020  ng order..      
-0000c1a0: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
-0000c1b0: 696f 6e20 2866 756e 6374 696f 6e2c 206f  ion (function, o
-0000c1c0: 7074 696f 6e61 6c29 3a20 5468 6520 7374  ptional): The st
-0000c1d0: 7265 6e67 7468 2066 756e 6374 696f 6e20  rength function 
-0000c1e0: 746f 2062 6520 7573 6564 2074 6f20 6361  to be used to ca
-0000c1f0: 6c63 756c 6174 6520 7468 6520 7374 7265  lculate the stre
-0000c200: 6e67 7468 206f 6620 6120 7061 7468 2e20  ngth of a path. 
-0000c210: 2020 5468 6520 6465 6661 756c 7420 6973    The default is
-0000c220: 2074 6865 206d 6172 6769 6e20 6d65 7468   the margin meth
-0000c230: 6f64 206f 6620 6060 6564 6174 6160 602e  od of ``edata``.
-0000c240: 2020 2054 6869 7320 6f6e 6c79 206d 6174     This only mat
-0000c250: 7465 7273 2077 6865 6e20 7468 6520 6261  ters when the ba
-0000c260: 6c6c 6f74 7320 6172 6520 6e6f 7420 6c69  llots are not li
-0000c270: 6e65 6172 206f 7264 6572 732e 200a 0a20  near orders. .. 
-0000c280: 2020 2052 6574 7572 6e73 3a20 0a20 2020     Returns: .   
-0000c290: 2020 2020 2041 2073 6f72 7465 6420 6c69       A sorted li
-0000c2a0: 7374 206f 6620 6361 6e64 6964 6174 6573  st of candidates
-0000c2b0: 2e20 0a0a 2020 2020 2222 220a 2020 2020  . ..    """.    
-0000c2c0: 6361 6e64 6964 6174 6573 203d 2065 6461  candidates = eda
-0000c2d0: 7461 2e63 616e 6469 6461 7465 7320 6966  ta.candidates if
-0000c2e0: 2063 7572 725f 6361 6e64 7320 6973 204e   curr_cands is N
-0000c2f0: 6f6e 6520 656c 7365 2063 7572 725f 6361  one else curr_ca
-0000c300: 6e64 7320 2020 200a 2020 2020 6369 6478  nds    .    cidx
-0000c310: 5f74 6f5f 6361 6e64 203d 207b 6369 6478  _to_cand = {cidx
-0000c320: 3a20 6320 666f 7220 6369 6478 2c20 6320  : c for cidx, c 
-0000c330: 696e 2065 6e75 6d65 7261 7465 2863 616e  in enumerate(can
-0000c340: 6469 6461 7465 7329 7d20 200a 2020 2020  didates)}  .    
-0000c350: 6361 6e64 5f74 6f5f 6369 6478 203d 207b  cand_to_cidx = {
-0000c360: 633a 2063 6964 7820 666f 7220 6369 6478  c: cidx for cidx
-0000c370: 2c20 6320 696e 2065 6e75 6d65 7261 7465  , c in enumerate
-0000c380: 2863 616e 6469 6461 7465 7329 7d20 200a  (candidates)}  .
-0000c390: 2020 2020 7374 7265 6e67 7468 5f66 756e      strength_fun
-0000c3a0: 6374 696f 6e20 3d20 6564 6174 612e 6d61  ction = edata.ma
-0000c3b0: 7267 696e 2069 6620 7374 7265 6e67 7468  rgin if strength
-0000c3c0: 5f66 756e 6374 696f 6e20 6973 204e 6f6e  _function is Non
-0000c3d0: 6520 656c 7365 2073 7472 656e 6774 685f  e else strength_
-0000c3e0: 6675 6e63 7469 6f6e 2020 2020 0a0a 2020  function    ..  
-0000c3f0: 2020 7462 5f72 616e 6b69 6e67 203d 2074    tb_ranking = t
-0000c400: 6965 5f62 7265 616b 6572 2069 6620 7469  ie_breaker if ti
-0000c410: 655f 6272 6561 6b65 7220 6973 206e 6f74  e_breaker is not
-0000c420: 204e 6f6e 6520 656c 7365 2073 6f72 7465   None else sorte
-0000c430: 6428 6c69 7374 2863 616e 6469 6461 7465  d(list(candidate
-0000c440: 7329 290a 0a20 2020 2063 7720 3d20 6564  s))..    cw = ed
-0000c450: 6174 612e 636f 6e64 6f72 6365 745f 7769  ata.condorcet_wi
-0000c460: 6e6e 6572 2863 7572 725f 6361 6e64 733d  nner(curr_cands=
-0000c470: 6375 7272 5f63 616e 6473 290a 2020 2020  curr_cands).    
-0000c480: 2320 5269 7665 7220 6973 2043 6f6e 646f  # River is Condo
-0000c490: 7263 6574 2063 6f6e 7369 7374 656e 742c  rcet consistent,
-0000c4a0: 2073 6f20 7369 6d70 6c79 2072 6574 7572   so simply retur
-0000c4b0: 6e20 7468 6520 436f 6e64 6f72 6365 7420  n the Condorcet 
-0000c4c0: 7769 6e6e 6572 2069 6620 6578 6973 7473  winner if exists
-0000c4d0: 0a20 2020 2069 6620 6377 2069 7320 6e6f  .    if cw is no
-0000c4e0: 7420 4e6f 6e65 3a20 0a20 2020 2020 2020  t None: .       
-0000c4f0: 2077 696e 6e65 7273 203d 205b 6377 5d0a   winners = [cw].
-0000c500: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000c510: 2020 775f 6564 6765 7320 3d20 5b28 6331    w_edges = [(c1
-0000c520: 2c20 6332 2c20 7374 7265 6e67 7468 5f66  , c2, strength_f
-0000c530: 756e 6374 696f 6e28 6331 2c20 6332 2929  unction(c1, c2))
-0000c540: 2066 6f72 2063 3120 696e 2063 616e 6469   for c1 in candi
-0000c550: 6461 7465 7320 666f 7220 6332 2069 6e20  dates for c2 in 
-0000c560: 6361 6e64 6964 6174 6573 2069 6620 6331  candidates if c1
-0000c570: 2021 3d20 6332 2061 6e64 2028 6564 6174   != c2 and (edat
-0000c580: 612e 6d61 6a6f 7269 7479 5f70 7265 6665  a.majority_prefe
-0000c590: 7273 2863 312c 2063 3229 206f 7220 6564  rs(c1, c2) or ed
-0000c5a0: 6174 612e 6973 5f74 6965 6428 6331 2c20  ata.is_tied(c1, 
-0000c5b0: 6332 2929 5d0a 2020 2020 2020 2020 7769  c2))].        wi
-0000c5c0: 6e6e 6572 7320 3d20 6c69 7374 2829 2020  nners = list()  
-0000c5d0: 0a20 2020 2020 2020 2073 7472 656e 6774  .        strengt
-0000c5e0: 6873 203d 2073 6f72 7465 6428 6c69 7374  hs = sorted(list
-0000c5f0: 2873 6574 285b 655b 325d 2066 6f72 2065  (set([e[2] for e
-0000c600: 2069 6e20 775f 6564 6765 735d 2929 2c20   in w_edges])), 
-0000c610: 7265 7665 7273 653d 5472 7565 290a 0a20  reverse=True).. 
-0000c620: 2020 2020 2020 2072 765f 6465 6665 6174         rv_defeat
-0000c630: 203d 2053 504f 286c 656e 2863 616e 6469   = SPO(len(candi
-0000c640: 6461 7465 7329 290a 0a20 2020 2020 2020  dates))..       
-0000c650: 2066 6f72 2073 2069 6e20 7374 7265 6e67   for s in streng
-0000c660: 7468 733a 200a 2020 2020 2020 2020 2020  ths: .          
-0000c670: 2020 6564 6765 7320 3d20 5b65 2066 6f72    edges = [e for
-0000c680: 2065 2069 6e20 775f 6564 6765 7320 6966   e in w_edges if
-0000c690: 2065 5b32 5d20 3d3d 2073 5d0a 2020 2020   e[2] == s].    
-0000c6a0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-0000c6b0: 2020 2020 2023 2062 7265 616b 2074 6965       # break tie
-0000c6c0: 7320 7573 696e 6720 7468 6520 6c65 7869  s using the lexi
-0000c6d0: 636f 6772 6170 6869 6320 6f72 6465 7269  cographic orderi
-0000c6e0: 6e67 206f 6e20 7475 706c 6573 2067 6976  ng on tuples giv
-0000c6f0: 656e 2074 625f 7261 6e6b 696e 670a 2020  en tb_ranking.  
-0000c700: 2020 2020 2020 2020 2020 736f 7274 6564            sorted
-0000c710: 5f65 6467 6573 203d 2073 6f72 7465 6428  _edges = sorted(
-0000c720: 6564 6765 732c 206b 6579 203d 206c 616d  edges, key = lam
-0000c730: 6264 6120 653a 2028 7462 5f72 616e 6b69  bda e: (tb_ranki
-0000c740: 6e67 2e69 6e64 6578 2865 5b30 5d29 2c20  ng.index(e[0]), 
-0000c750: 7462 5f72 616e 6b69 6e67 2e69 6e64 6578  tb_ranking.index
-0000c760: 2865 5b31 5d29 292c 2072 6576 6572 7365  (e[1])), reverse
-0000c770: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
-0000c780: 2020 2020 666f 7220 6530 2c65 312c 7320      for e0,e1,s 
-0000c790: 696e 2073 6f72 7465 645f 6564 6765 733a  in sorted_edges:
-0000c7a0: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-0000c7b0: 2020 6966 206e 6f74 2072 765f 6465 6665    if not rv_defe
-0000c7c0: 6174 2e50 5b63 616e 645f 746f 5f63 6964  at.P[cand_to_cid
-0000c7d0: 785b 6531 5d5d 5b63 616e 645f 746f 5f63  x[e1]][cand_to_c
-0000c7e0: 6964 785b 6530 5d5d 2061 6e64 206c 656e  idx[e0]] and len
-0000c7f0: 2872 765f 6465 6665 6174 2e70 7265 6473  (rv_defeat.preds
-0000c800: 5b63 616e 645f 746f 5f63 6964 785b 6531  [cand_to_cidx[e1
-0000c810: 5d5d 2920 3d3d 2030 3a0a 2020 2020 2020  ]]) == 0:.      
-0000c820: 2020 2020 2020 2020 2020 2020 2020 7276                rv
-0000c830: 5f64 6566 6561 742e 6164 6428 6361 6e64  _defeat.add(cand
-0000c840: 5f74 6f5f 6369 6478 5b65 305d 2c63 616e  _to_cidx[e0],can
-0000c850: 645f 746f 5f63 6964 785b 6531 5d29 0a20  d_to_cidx[e1]). 
-0000c860: 2020 2020 2020 2020 2020 2077 696e 6e65             winne
-0000c870: 7273 2e61 7070 656e 6428 6369 6478 5f74  rs.append(cidx_t
-0000c880: 6f5f 6361 6e64 5b72 765f 6465 6665 6174  o_cand[rv_defeat
-0000c890: 2e69 6e69 7469 616c 5f65 6c65 6d65 6e74  .initial_element
-0000c8a0: 7328 295b 305d 5d29 0a20 2020 2072 6574  s()[0]]).    ret
-0000c8b0: 7572 6e20 736f 7274 6564 286c 6973 7428  urn sorted(list(
-0000c8c0: 7365 7428 7769 6e6e 6572 7329 2929 0a0a  set(winners)))..
-0000c8d0: 0a40 766d 286e 616d 653d 2252 6976 6572  .@vm(name="River
-0000c8e0: 205a 5422 290a 6465 6620 7269 7665 725f   ZT").def river_
-0000c8f0: 7a74 2870 726f 6669 6c65 2c20 6375 7272  zt(profile, curr
-0000c900: 5f63 616e 6473 203d 204e 6f6e 652c 2073  _cands = None, s
-0000c910: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-0000c920: 203d 204e 6f6e 6529 3a20 2020 0a20 2020   = None):   .   
-0000c930: 2022 2222 5269 7665 7220 7768 6572 6520   """River where 
-0000c940: 6120 6669 7865 6420 766f 7465 7220 6272  a fixed voter br
-0000c950: 6561 6b73 2061 6e79 2074 6965 7320 696e  eaks any ties in
-0000c960: 2074 6865 206d 6172 6769 6e73 2e20 2049   the margins.  I
-0000c970: 7420 6973 2061 6c77 6179 7320 7468 6520  t is always the 
-0000c980: 766f 7465 7220 696e 2070 6f73 6974 696f  voter in positio
-0000c990: 6e20 3020 7468 6174 2062 7265 616b 7320  n 0 that breaks 
-0000c9a0: 7468 6520 7469 6573 2e20 2053 696e 6365  the ties.  Since
-0000c9b0: 2076 6f74 6572 7320 6861 7665 2073 7472   voters have str
-0000c9c0: 6963 7420 7072 6566 6572 656e 6365 732c  ict preferences,
-0000c9d0: 2074 6869 7320 6d65 7468 6f64 2069 7320   this method is 
-0000c9e0: 7265 736f 6c75 7465 2e20 200a 0a20 2020  resolute.  ..   
-0000c9f0: 2041 7267 733a 0a20 2020 2020 2020 2065   Args:.        e
-0000ca00: 6461 7461 2028 5072 6f66 696c 6529 3a20  data (Profile): 
-0000ca10: 4120 7072 6f66 696c 6520 6f66 206c 696e  A profile of lin
-0000ca20: 6561 7220 6f72 6465 7273 0a20 2020 2020  ear orders.     
-0000ca30: 2020 2063 7572 725f 6361 6e64 7320 284c     curr_cands (L
-0000ca40: 6973 745b 696e 745d 2c20 6f70 7469 6f6e  ist[int], option
-0000ca50: 616c 293a 2049 6620 7365 742c 2074 6865  al): If set, the
-0000ca60: 6e20 6669 6e64 2074 6865 2077 696e 6e65  n find the winne
-0000ca70: 7273 2066 6f72 2074 6865 2070 726f 6669  rs for the profi
-0000ca80: 6c65 2072 6573 7472 6963 7465 6420 746f  le restricted to
-0000ca90: 2074 6865 2063 616e 6469 6461 7465 7320   the candidates 
-0000caa0: 696e 2060 6063 7572 725f 6361 6e64 7360  in ``curr_cands`
-0000cab0: 600a 0a20 2020 2052 6574 7572 6e73 3a20  `..    Returns: 
-0000cac0: 0a20 2020 2020 2020 2041 2073 6f72 7465  .        A sorte
-0000cad0: 6420 6c69 7374 206f 6620 6361 6e64 6964  d list of candid
-0000cae0: 6174 6573 2e20 0a0a 2020 2020 2e2e 2073  ates. ..    .. s
-0000caf0: 6565 616c 736f 3a3a 0a0a 2020 2020 2020  eealso::..      
-0000cb00: 2020 3a6d 6574 683a 6070 7265 665f 766f    :meth:`pref_vo
-0000cb10: 7469 6e67 2e6d 6172 6769 6e5f 6261 7365  ting.margin_base
-0000cb20: 645f 6d65 7468 6f64 732e 7269 7665 7260  d_methods.river`
-0000cb30: 2c20 3a6d 6574 683a 6070 7265 665f 766f  , :meth:`pref_vo
-0000cb40: 7469 6e67 2e6d 6172 6769 6e5f 6261 7365  ting.margin_base
-0000cb50: 645f 6d65 7468 6f64 732e 7269 7665 725f  d_methods.river_
-0000cb60: 7769 7468 5f74 6573 7460 2c20 3a6d 6574  with_test`, :met
-0000cb70: 683a 6070 7265 665f 766f 7469 6e67 2e6d  h:`pref_voting.m
-0000cb80: 6172 6769 6e5f 6261 7365 645f 6d65 7468  argin_based_meth
-0000cb90: 6f64 732e 7261 6e6b 6564 5f70 6169 7273  ods.ranked_pairs
-0000cba0: 600a 0a20 2020 200a 2020 2020 2222 220a  `..    .    """.
-0000cbb0: 2020 2020 6361 6e64 6964 6174 6573 203d      candidates =
-0000cbc0: 2070 726f 6669 6c65 2e63 616e 6469 6461   profile.candida
-0000cbd0: 7465 7320 6966 2063 7572 725f 6361 6e64  tes if curr_cand
-0000cbe0: 7320 6973 204e 6f6e 6520 656c 7365 2063  s is None else c
-0000cbf0: 7572 725f 6361 6e64 7320 2020 200a 2020  urr_cands    .  
-0000cc00: 2020 0a20 2020 2023 2074 6865 2074 6965    .    # the tie
-0000cc10: 2d62 7265 616b 6572 2069 7320 616c 7761  -breaker is alwa
-0000cc20: 7973 2074 6865 2066 6972 7374 2076 6f74  ys the first vot
-0000cc30: 6572 2e20 0a20 2020 2074 625f 7261 6e6b  er. .    tb_rank
-0000cc40: 696e 6720 3d20 7475 706c 6528 5b63 2066  ing = tuple([c f
-0000cc50: 6f72 2063 2069 6e20 6c69 7374 2870 726f  or c in list(pro
-0000cc60: 6669 6c65 2e5f 7261 6e6b 696e 6773 5b30  file._rankings[0
-0000cc70: 5d29 2069 6620 6320 696e 2063 616e 6469  ]) if c in candi
-0000cc80: 6461 7465 735d 290a 2020 2020 0a20 2020  dates]).    .   
-0000cc90: 2072 6574 7572 6e20 7269 7665 725f 7462   return river_tb
-0000cca0: 2870 726f 6669 6c65 2c20 6375 7272 5f63  (profile, curr_c
-0000ccb0: 616e 6473 203d 2063 7572 725f 6361 6e64  ands = curr_cand
-0000ccc0: 732c 2074 6965 5f62 7265 616b 6572 203d  s, tie_breaker =
-0000ccd0: 2074 625f 7261 6e6b 696e 672c 2073 7472   tb_ranking, str
-0000cce0: 656e 6774 685f 6675 6e63 7469 6f6e 203d  ength_function =
-0000ccf0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-0000cd00: 6f6e 290a 2020 2020 0a0a 2320 5369 6d70  on).    ..# Simp
-0000cd10: 6c65 2053 7461 626c 6520 566f 7469 6e67  le Stable Voting
-0000cd20: 200a 6465 6620 5f73 696d 706c 655f 7374   .def _simple_st
-0000cd30: 6162 6c65 5f76 6f74 696e 6728 6375 7272  able_voting(curr
-0000cd40: 5f63 616e 6473 2c20 0a20 2020 2020 2020  _cands, .       
-0000cd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd60: 2020 2073 6f72 7465 645f 6d61 7463 6865     sorted_matche
-0000cd70: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-0000cd80: 2020 2020 2020 2020 2020 2020 206d 656d               mem
-0000cd90: 5f73 765f 7769 6e6e 6572 7329 3a0a 2020  _sv_winners):.  
-0000cda0: 2020 2727 270a 2020 2020 4465 7465 726d    '''.    Determ
-0000cdb0: 696e 6520 7468 6520 5369 6d70 6c65 2053  ine the Simple S
-0000cdc0: 7461 626c 6520 566f 7469 6e67 2077 696e  table Voting win
-0000cdd0: 6e65 7273 2077 6869 6c65 206b 6565 7069  ners while keepi
-0000cde0: 6e67 2074 7261 636b 200a 2020 2020 6f66  ng track .    of
-0000cdf0: 2074 6865 2077 696e 6e65 7273 2069 6e20   the winners in 
-0000ce00: 616e 7920 7375 6270 726f 6669 6c65 7320  any subprofiles 
-0000ce10: 6368 6563 6b65 6420 6475 7269 6e67 2063  checked during c
-0000ce20: 6f6d 7075 7461 7469 6f6e 2e20 0a20 2020  omputation. .   
-0000ce30: 2027 2727 0a20 2020 200a 2020 2020 7376   '''.    .    sv
-0000ce40: 5f77 696e 6e65 7273 203d 206c 6973 7428  _winners = list(
-0000ce50: 290a 2020 2020 2020 2020 0a20 2020 2069  ).        .    i
-0000ce60: 6620 6c65 6e28 6375 7272 5f63 616e 6473  f len(curr_cands
-0000ce70: 2920 3d3d 2031 3a20 0a20 2020 2020 2020  ) == 1: .       
-0000ce80: 206d 656d 5f73 765f 7769 6e6e 6572 735b   mem_sv_winners[
-0000ce90: 7475 706c 6528 6375 7272 5f63 616e 6473  tuple(curr_cands
-0000cea0: 295d 203d 2063 7572 725f 6361 6e64 730a  )] = curr_cands.
-0000ceb0: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-0000cec0: 7572 725f 6361 6e64 732c 206d 656d 5f73  urr_cands, mem_s
-0000ced0: 765f 7769 6e6e 6572 730a 2020 2020 0a20  v_winners.    . 
-0000cee0: 2020 206d 6172 6769 6e5f 7769 746e 6573     margin_witnes
-0000cef0: 7369 6e67 5f77 696e 203d 202d 6d61 7468  sing_win = -math
-0000cf00: 2e69 6e66 0a0a 2020 2020 666f 7220 612c  .inf..    for a,
-0000cf10: 2062 2c20 7320 696e 2073 6f72 7465 645f   b, s in sorted_
-0000cf20: 6d61 7463 6865 733a 0a20 2020 2020 2020  matches:.       
-0000cf30: 2069 6620 7320 3c20 6d61 7267 696e 5f77   if s < margin_w
-0000cf40: 6974 6e65 7373 696e 675f 7769 6e3a 200a  itnessing_win: .
-0000cf50: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-0000cf60: 6b0a 2020 2020 2020 2020 6966 2061 206e  k.        if a n
-0000cf70: 6f74 2069 6e20 7376 5f77 696e 6e65 7273  ot in sv_winners
-0000cf80: 3a20 0a20 2020 2020 2020 2020 2020 2063  : .            c
-0000cf90: 616e 6473 5f6d 696e 7573 5f62 203d 205b  ands_minus_b = [
-0000cfa0: 6320 666f 7220 6320 696e 2063 7572 725f  c for c in curr_
-0000cfb0: 6361 6e64 7320 6966 2063 2021 3d20 625d  cands if c != b]
-0000cfc0: 0a20 2020 2020 2020 2020 2020 2063 616e  .            can
-0000cfd0: 6473 5f6d 696e 7573 5f62 5f6b 6579 203d  ds_minus_b_key =
-0000cfe0: 2074 7570 6c65 2873 6f72 7465 6428 6361   tuple(sorted(ca
-0000cff0: 6e64 735f 6d69 6e75 735f 6229 290a 2020  nds_minus_b)).  
-0000d000: 2020 2020 2020 2020 2020 6966 2063 616e            if can
-0000d010: 6473 5f6d 696e 7573 5f62 5f6b 6579 206e  ds_minus_b_key n
-0000d020: 6f74 2069 6e20 6d65 6d5f 7376 5f77 696e  ot in mem_sv_win
-0000d030: 6e65 7273 2e6b 6579 7328 293a 200a 2020  ners.keys(): .  
-0000d040: 2020 2020 2020 2020 2020 2020 2020 7773                ws
-0000d050: 2c20 6d65 6d5f 7376 5f77 696e 6e65 7273  , mem_sv_winners
-0000d060: 203d 205f 7369 6d70 6c65 5f73 7461 626c   = _simple_stabl
-0000d070: 655f 766f 7469 6e67 2863 7572 725f 6361  e_voting(curr_ca
-0000d080: 6e64 7320 3d20 6361 6e64 735f 6d69 6e75  nds = cands_minu
-0000d090: 735f 622c 0a20 2020 2020 2020 2020 2020  s_b,.           
-0000d0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ea0: 696f 6e20 2866 756e 6374 696f 6e2c 206f  ion (function, o
+00001eb0: 7074 696f 6e61 6c29 3a20 5468 6520 7374  ptional): The st
+00001ec0: 7265 6e67 7468 2066 756e 6374 696f 6e20  rength function 
+00001ed0: 746f 2062 6520 7573 6564 2074 6f20 6361  to be used to ca
+00001ee0: 6c63 756c 6174 6520 7468 6520 7374 7265  lculate the stre
+00001ef0: 6e67 7468 206f 6620 6120 7061 7468 2e20  ngth of a path. 
+00001f00: 2020 5468 6520 6465 6661 756c 7420 6973    The default is
+00001f10: 2074 6865 206d 6172 6769 6e20 6d65 7468   the margin meth
+00001f20: 6f64 206f 6620 6060 6564 6174 6160 602e  od of ``edata``.
+00001f30: 2020 2054 6869 7320 6f6e 6c79 206d 6174     This only mat
+00001f40: 7465 7273 2077 6865 6e20 7468 6520 6261  ters when the ba
+00001f50: 6c6c 6f74 7320 6172 6520 6e6f 7420 6c69  llots are not li
+00001f60: 6e65 6172 206f 7264 6572 732e 200a 0a20  near orders. .. 
+00001f70: 2020 2052 6574 7572 6e73 3a20 0a20 2020     Returns: .   
+00001f80: 2020 2020 2041 2073 6f72 7465 6420 6c69       A sorted li
+00001f90: 7374 206f 6620 6361 6e64 6964 6174 6573  st of candidates
+00001fa0: 2e20 0a0a 2020 2020 2222 220a 0a20 2020  . ..    """..   
+00001fb0: 2063 616e 6469 6461 7465 7320 3d20 6564   candidates = ed
+00001fc0: 6174 612e 6361 6e64 6964 6174 6573 2069  ata.candidates i
+00001fd0: 6620 6375 7272 5f63 616e 6473 2069 7320  f curr_cands is 
+00001fe0: 4e6f 6e65 2065 6c73 6520 6375 7272 5f63  None else curr_c
+00001ff0: 616e 6473 2020 2020 0a20 2020 2073 7472  ands    .    str
+00002000: 656e 6774 685f 6675 6e63 7469 6f6e 203d  ength_function =
+00002010: 2065 6461 7461 2e6d 6172 6769 6e20 6966   edata.margin if
+00002020: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+00002030: 6f6e 2069 7320 4e6f 6e65 2065 6c73 6520  on is None else 
+00002040: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+00002050: 6e0a 2020 2020 2020 2020 0a20 2020 2073  n.        .    s
+00002060: 5f6d 6174 7269 7820 3d20 5b5b 2d6e 702e  _matrix = [[-np.
+00002070: 696e 6620 666f 7220 5f20 696e 2063 616e  inf for _ in can
+00002080: 6469 6461 7465 735d 2066 6f72 205f 2069  didates] for _ i
+00002090: 6e20 6361 6e64 6964 6174 6573 5d0a 2020  n candidates].  
+000020a0: 2020 666f 7220 6331 5f69 6478 2c20 6331    for c1_idx, c1
+000020b0: 2069 6e20 656e 756d 6572 6174 6528 6361   in enumerate(ca
+000020c0: 6e64 6964 6174 6573 293a 0a20 2020 2020  ndidates):.     
+000020d0: 2020 2066 6f72 2063 325f 6964 782c 2063     for c2_idx, c
+000020e0: 3220 696e 2065 6e75 6d65 7261 7465 2863  2 in enumerate(c
+000020f0: 616e 6469 6461 7465 7329 3a0a 2020 2020  andidates):.    
+00002100: 2020 2020 2020 2020 6966 2028 6564 6174          if (edat
+00002110: 612e 6d61 6a6f 7269 7479 5f70 7265 6665  a.majority_prefe
+00002120: 7273 2863 312c 2063 3229 206f 7220 6331  rs(c1, c2) or c1
+00002130: 203d 3d20 6332 293a 0a20 2020 2020 2020   == c2):.       
+00002140: 2020 2020 2020 2020 2073 5f6d 6174 7269           s_matri
+00002150: 785b 6331 5f69 6478 5d5b 6332 5f69 6478  x[c1_idx][c2_idx
+00002160: 5d20 3d20 7374 7265 6e67 7468 5f66 756e  ] = strength_fun
+00002170: 6374 696f 6e28 6331 2c20 6332 2920 0a20  ction(c1, c2) . 
+00002180: 2020 2073 7472 656e 6774 6820 3d20 6c69     strength = li
+00002190: 7374 286d 6170 286c 616d 6264 6120 6920  st(map(lambda i 
+000021a0: 3a20 6c69 7374 286d 6170 286c 616d 6264  : list(map(lambd
+000021b0: 6120 6a20 3a20 6a20 2c20 6929 2920 2c20  a j : j , i)) , 
+000021c0: 735f 6d61 7472 6978 2929 0a20 2020 2066  s_matrix)).    f
+000021d0: 6f72 2069 5f69 6478 2c20 6920 696e 2065  or i_idx, i in e
+000021e0: 6e75 6d65 7261 7465 2863 616e 6469 6461  numerate(candida
+000021f0: 7465 7329 3a20 2020 2020 2020 2020 0a20  tes):         . 
+00002200: 2020 2020 2020 2066 6f72 206a 5f69 6478         for j_idx
+00002210: 2c20 6a20 696e 2065 6e75 6d65 7261 7465  , j in enumerate
+00002220: 2863 616e 6469 6461 7465 7329 3a20 0a20  (candidates): . 
+00002230: 2020 2020 2020 2020 2020 2069 6620 6921             if i!
+00002240: 3d20 6a3a 0a20 2020 2020 2020 2020 2020  = j:.           
+00002250: 2020 2020 2066 6f72 206b 5f69 6478 2c20       for k_idx, 
+00002260: 6b20 696e 2065 6e75 6d65 7261 7465 2863  k in enumerate(c
+00002270: 616e 6469 6461 7465 7329 3a20 0a20 2020  andidates): .   
+00002280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002290: 2069 6620 6921 3d20 6b20 616e 6420 6a20   if i!= k and j 
+000022a0: 213d 206b 3a0a 2020 2020 2020 2020 2020  != k:.          
+000022b0: 2020 2020 2020 2020 2020 2020 2020 7374                st
+000022c0: 7265 6e67 7468 5b6a 5f69 6478 5d5b 6b5f  rength[j_idx][k_
+000022d0: 6964 785d 203d 206d 6178 2873 7472 656e  idx] = max(stren
+000022e0: 6774 685b 6a5f 6964 785d 5b6b 5f69 6478  gth[j_idx][k_idx
+000022f0: 5d2c 206d 696e 2873 7472 656e 6774 685b  ], min(strength[
+00002300: 6a5f 6964 785d 5b69 5f69 6478 5d2c 7374  j_idx][i_idx],st
+00002310: 7265 6e67 7468 5b69 5f69 6478 5d5b 6b5f  rength[i_idx][k_
+00002320: 6964 785d 2929 0a20 2020 2077 696e 6e65  idx])).    winne
+00002330: 7273 203d 207b 693a 5472 7565 2066 6f72  rs = {i:True for
+00002340: 2069 2069 6e20 6361 6e64 6964 6174 6573   i in candidates
+00002350: 7d0a 2020 2020 666f 7220 695f 6964 782c  }.    for i_idx,
+00002360: 2069 2069 6e20 656e 756d 6572 6174 6528   i in enumerate(
+00002370: 6361 6e64 6964 6174 6573 293a 200a 2020  candidates): .  
+00002380: 2020 2020 2020 666f 7220 6a5f 6964 782c        for j_idx,
+00002390: 206a 2069 6e20 656e 756d 6572 6174 6528   j in enumerate(
+000023a0: 6361 6e64 6964 6174 6573 293a 0a20 2020  candidates):.   
+000023b0: 2020 2020 2020 2020 2069 6620 6921 3d6a           if i!=j
+000023c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000023d0: 2020 6966 2073 7472 656e 6774 685b 6a5f    if strength[j_
+000023e0: 6964 785d 5b69 5f69 6478 5d20 3e20 7374  idx][i_idx] > st
+000023f0: 7265 6e67 7468 5b69 5f69 6478 5d5b 6a5f  rength[i_idx][j_
+00002400: 6964 785d 3a0a 2020 2020 2020 2020 2020  idx]:.          
+00002410: 2020 2020 2020 2020 2020 7769 6e6e 6572            winner
+00002420: 735b 695d 203d 2046 616c 7365 0a20 2020  s[i] = False.   
+00002430: 2072 6574 7572 6e20 736f 7274 6564 285b   return sorted([
+00002440: 6320 666f 7220 6320 696e 2063 616e 6469  c for c in candi
+00002450: 6461 7465 7320 6966 2077 696e 6e65 7273  dates if winners
+00002460: 5b63 5d5d 290a 0a62 705f 7072 6f70 6572  [c]])..bp_proper
+00002470: 7469 6573 203d 2056 6f74 696e 674d 6574  ties = VotingMet
+00002480: 686f 6450 726f 7065 7274 6965 7328 0a20  hodProperties(. 
+00002490: 2020 2063 6f6e 646f 7263 6574 5f77 696e     condorcet_win
+000024a0: 6e65 723d 5472 7565 2c20 0a20 2020 2063  ner=True, .    c
+000024b0: 6f6e 646f 7263 6574 5f6c 6f73 6572 3d54  ondorcet_loser=T
+000024c0: 7275 652c 0a20 2020 2070 6172 6574 6f5f  rue,.    pareto_
+000024d0: 646f 6d69 6e61 6e63 653d 5472 7565 2c20  dominance=True, 
+000024e0: 0a20 2020 2029 0a40 766d 286e 616d 653d  .    ).@vm(name=
+000024f0: 2242 6561 7420 5061 7468 222c 0a20 2020  "Beat Path",.   
+00002500: 2070 726f 7065 7274 6965 733d 6270 5f70   properties=bp_p
+00002510: 726f 7065 7274 6965 732c 0a20 2020 2069  roperties,.    i
+00002520: 6e70 7574 5f74 7970 6573 3d5b 456c 6563  nput_types=[Elec
+00002530: 7469 6f6e 5479 7065 732e 5052 4f46 494c  tionTypes.PROFIL
+00002540: 452c 2045 6c65 6374 696f 6e54 7970 6573  E, ElectionTypes
+00002550: 2e50 524f 4649 4c45 5f57 4954 485f 5449  .PROFILE_WITH_TI
+00002560: 4553 2c20 456c 6563 7469 6f6e 5479 7065  ES, ElectionType
+00002570: 732e 4d41 5247 494e 5f47 5241 5048 5d29  s.MARGIN_GRAPH])
+00002580: 0a64 6566 2062 6561 745f 7061 7468 280a  .def beat_path(.
+00002590: 2020 2020 6564 6174 612c 200a 2020 2020      edata, .    
+000025a0: 6375 7272 5f63 616e 6473 203d 204e 6f6e  curr_cands = Non
+000025b0: 652c 200a 2020 2020 7374 7265 6e67 7468  e, .    strength
+000025c0: 5f66 756e 6374 696f 6e20 3d20 4e6f 6e65  _function = None
+000025d0: 2c20 0a20 2020 2061 6c67 6f72 6974 686d  , .    algorithm
+000025e0: 203d 2027 666c 6f79 645f 7761 7273 6861   = 'floyd_warsha
+000025f0: 6c6c 2729 3a20 200a 0a20 2020 2022 2222  ll'):  ..    """
+00002600: 466f 7220 6361 6e64 6964 6174 6573 203a  For candidates :
+00002610: 6d61 7468 3a60 6160 2061 6e64 203a 6d61  math:`a` and :ma
+00002620: 7468 3a60 6260 2c20 6120 2a2a 7061 7468  th:`b`, a **path
+00002630: 2a2a 2066 726f 6d20 3a6d 6174 683a 6061  ** from :math:`a
+00002640: 6020 746f 203a 6d61 7468 3a60 6260 2069  ` to :math:`b` i
+00002650: 7320 6120 7365 7175 656e 6365 200a 2020  s a sequence .  
+00002660: 2020 3a6d 6174 683a 6078 5f31 2c20 5c6c    :math:`x_1, \l
+00002670: 646f 7473 2c20 785f 6e60 206f 6620 6469  dots, x_n` of di
+00002680: 7374 696e 6374 2063 616e 6469 6461 7465  stinct candidate
+00002690: 7320 2077 6974 6820 203a 6d61 7468 3a60  s  with  :math:`
+000026a0: 785f 313d 6160 2061 6e64 203a 6d61 7468  x_1=a` and :math
+000026b0: 3a60 785f 6e3d 6260 2073 7563 6820 7468  :`x_n=b` such th
+000026c0: 6174 200a 2020 2020 666f 7220 3a6d 6174  at .    for :mat
+000026d0: 683a 6031 5c6c 6571 206b 5c6c 6571 206e  h:`1\leq k\leq n
+000026e0: 2d31 602c 203a 6d61 7468 3a60 785f 6b60  -1`, :math:`x_k`
+000026f0: 2069 7320 6d61 6a6f 7269 7479 2070 7265   is majority pre
+00002700: 6665 7272 6564 2074 6f20 3a6d 6174 683a  ferred to :math:
+00002710: 6078 5f7b 6b2b 317d 602e 2020 5468 6520  `x_{k+1}`.  The 
+00002720: 2a2a 7374 7265 6e67 7468 206f 6620 6120  **strength of a 
+00002730: 7061 7468 2a2a 0a20 2020 2069 7320 7468  path**.    is th
+00002740: 6520 6d69 6e69 6d61 6c20 6d61 7267 696e  e minimal margin
+00002750: 2061 6c6f 6e67 2074 6861 7420 7061 7468   along that path
+00002760: 2e20 2053 6179 2074 6861 7420 3a6d 6174  .  Say that :mat
+00002770: 683a 6061 6020 6465 6665 6174 7320 3a6d  h:`a` defeats :m
+00002780: 6174 683a 6062 6020 6163 636f 7264 696e  ath:`b` accordin
+00002790: 6720 746f 2042 6561 7420 5061 7468 2069  g to Beat Path i
+000027a0: 6620 7468 6520 7468 6520 7374 7265 6e67  f the the streng
+000027b0: 7468 206f 6620 7468 6520 7374 726f 6e67  th of the strong
+000027c0: 6573 7420 7061 7468 2066 726f 6d20 3a6d  est path from :m
+000027d0: 6174 683a 6061 6020 746f 203a 6d61 7468  ath:`a` to :math
+000027e0: 3a60 6260 2069 7320 6772 6561 7465 7220  :`b` is greater 
+000027f0: 7468 616e 2074 6865 2073 7472 656e 6774  than the strengt
+00002800: 6820 6f66 2074 6865 2073 7472 6f6e 6765  h of the stronge
+00002810: 7374 2070 6174 6820 6672 6f6d 203a 6d61  st path from :ma
+00002820: 7468 3a60 6260 2074 6f20 3a6d 6174 683a  th:`b` to :math:
+00002830: 6061 602e 2054 6865 6e2c 2074 6865 2063  `a`. Then, the c
+00002840: 616e 6469 6461 7465 7320 7468 6174 2061  andidates that a
+00002850: 7265 2075 6e64 6566 6561 7465 6420 6163  re undefeated ac
+00002860: 636f 7264 696e 6720 746f 2042 6561 7420  cording to Beat 
+00002870: 5061 7468 2061 7265 2074 6865 2077 696e  Path are the win
+00002880: 6e65 7273 2e20 2041 6c73 6f20 6b6e 6f77  ners.  Also know
+00002890: 6e20 6173 2074 6865 2053 6368 756c 7a65  n as the Schulze
+000028a0: 2052 756c 652e 200a 0a20 2020 2041 7267   Rule. ..    Arg
+000028b0: 733a 0a20 2020 2020 2020 2065 6461 7461  s:.        edata
+000028c0: 2028 5072 6f66 696c 652c 2050 726f 6669   (Profile, Profi
+000028d0: 6c65 5769 7468 5469 6573 2c20 4d61 7267  leWithTies, Marg
+000028e0: 696e 4772 6170 6829 3a20 416e 7920 656c  inGraph): Any el
+000028f0: 6563 7469 6f6e 2064 6174 6120 7468 6174  ection data that
+00002900: 2068 6173 2061 2060 6d61 7267 696e 6020   has a `margin` 
+00002910: 6d65 7468 6f64 2e20 0a20 2020 2020 2020  method. .       
+00002920: 2063 7572 725f 6361 6e64 7320 284c 6973   curr_cands (Lis
+00002930: 745b 696e 745d 2c20 6f70 7469 6f6e 616c  t[int], optional
+00002940: 293a 2049 6620 7365 742c 2074 6865 6e20  ): If set, then 
+00002950: 6669 6e64 2074 6865 2077 696e 6e65 7273  find the winners
+00002960: 2066 6f72 2074 6865 2070 726f 6669 6c65   for the profile
+00002970: 2072 6573 7472 6963 7465 6420 746f 2074   restricted to t
+00002980: 6865 2063 616e 6469 6461 7465 7320 696e  he candidates in
+00002990: 2060 6063 7572 725f 6361 6e64 7360 600a   ``curr_cands``.
+000029a0: 2020 2020 2020 2020 7374 7265 6e67 7468          strength
+000029b0: 5f66 756e 6374 696f 6e20 2866 756e 6374  _function (funct
+000029c0: 696f 6e2c 206f 7074 696f 6e61 6c29 3a20  ion, optional): 
+000029d0: 5468 6520 7374 7265 6e67 7468 2066 756e  The strength fun
+000029e0: 6374 696f 6e20 746f 2062 6520 7573 6564  ction to be used
+000029f0: 2074 6f20 6361 6c63 756c 6174 6520 7468   to calculate th
+00002a00: 6520 7374 7265 6e67 7468 206f 6620 6120  e strength of a 
+00002a10: 7061 7468 2e20 2020 5468 6520 6465 6661  path.   The defa
+00002a20: 756c 7420 6973 2074 6865 206d 6172 6769  ult is the margi
+00002a30: 6e20 6d65 7468 6f64 206f 6620 6060 6564  n method of ``ed
+00002a40: 6174 6160 602e 2020 2054 6869 7320 6f6e  ata``.   This on
+00002a50: 6c79 206d 6174 7465 7273 2077 6865 6e20  ly matters when 
+00002a60: 7468 6520 6261 6c6c 6f74 7320 6172 6520  the ballots are 
+00002a70: 6e6f 7420 6c69 6e65 6172 206f 7264 6572  not linear order
+00002a80: 732e 200a 2020 2020 2020 2020 616c 676f  s. .        algo
+00002a90: 7269 7468 6d20 2873 7472 293a 2053 7065  rithm (str): Spe
+00002aa0: 6369 6679 2077 6869 6368 2061 6c67 6f72  cify which algor
+00002ab0: 6974 686d 2074 6f20 7573 652e 2020 4f70  ithm to use.  Op
+00002ac0: 7469 6f6e 7320 6172 6520 2766 6c6f 7964  tions are 'floyd
+00002ad0: 5f77 6172 7368 616c 6c27 2028 7468 6520  _warshall' (the 
+00002ae0: 6465 6661 756c 7429 2061 6e64 2027 6261  default) and 'ba
+00002af0: 7369 6327 2e0a 0a20 2020 2052 6574 7572  sic'...    Retur
+00002b00: 6e73 3a20 0a20 2020 2020 2020 2041 2073  ns: .        A s
+00002b10: 6f72 7465 6420 6c69 7374 206f 6620 6361  orted list of ca
+00002b20: 6e64 6964 6174 6573 2e20 0a0a 2020 2020  ndidates. ..    
+00002b30: 2e2e 2073 6565 616c 736f 3a3a 0a0a 2020  .. seealso::..  
+00002b40: 2020 2020 2020 3a6d 6574 683a 6070 7265        :meth:`pre
+00002b50: 665f 766f 7469 6e67 2e6d 6172 6769 6e5f  f_voting.margin_
+00002b60: 6261 7365 645f 6d65 7468 6f64 732e 6265  based_methods.be
+00002b70: 6174 5f70 6174 685f 6465 6665 6174 600a  at_path_defeat`.
+00002b80: 0a20 2020 203a 4578 616d 706c 653a 200a  .    :Example: .
+00002b90: 0a20 2020 202e 2e20 706c 6f74 3a3a 2020  .    .. plot::  
+00002ba0: 6d61 7267 696e 5f67 7261 7068 735f 6578  margin_graphs_ex
+00002bb0: 616d 706c 6573 2f6d 675f 6578 5f62 705f  amples/mg_ex_bp_
+00002bc0: 7270 2e70 790a 2020 2020 2020 2020 3a63  rp.py.        :c
+00002bd0: 6f6e 7465 7874 3a20 7265 7365 7420 200a  ontext: reset  .
+00002be0: 2020 2020 2020 2020 3a69 6e63 6c75 6465          :include
+00002bf0: 2d73 6f75 7263 653a 2054 7275 650a 0a0a  -source: True...
+00002c00: 2020 2020 2e2e 2063 6f64 652d 626c 6f63      .. code-bloc
+00002c10: 6b3a 3a20 0a0a 2020 2020 2020 2020 6672  k:: ..        fr
+00002c20: 6f6d 2070 7265 665f 766f 7469 6e67 2e6d  om pref_voting.m
+00002c30: 6172 6769 6e5f 6261 7365 645f 6d65 7468  argin_based_meth
+00002c40: 6f64 7320 696d 706f 7274 2062 6561 745f  ods import beat_
+00002c50: 7061 7468 0a0a 2020 2020 2020 2020 6265  path..        be
+00002c60: 6174 5f70 6174 682e 6469 7370 6c61 7928  at_path.display(
+00002c70: 6d67 290a 0a0a 2020 2020 2e2e 2065 7865  mg)...    .. exe
+00002c80: 635f 636f 6465 3a3a 200a 2020 2020 2020  c_code:: .      
+00002c90: 2020 3a68 6964 655f 636f 6465 3a0a 0a20    :hide_code:.. 
+00002ca0: 2020 2020 2020 2066 726f 6d20 7072 6566         from pref
+00002cb0: 5f76 6f74 696e 672e 7765 6967 6874 6564  _voting.weighted
+00002cc0: 5f6d 616a 6f72 6974 795f 6772 6170 6873  _majority_graphs
+00002cd0: 2069 6d70 6f72 7420 4d61 7267 696e 4772   import MarginGr
+00002ce0: 6170 680a 2020 2020 2020 2020 6672 6f6d  aph.        from
+00002cf0: 2070 7265 665f 766f 7469 6e67 2e6d 6172   pref_voting.mar
+00002d00: 6769 6e5f 6261 7365 645f 6d65 7468 6f64  gin_based_method
+00002d10: 7320 696d 706f 7274 2062 6561 745f 7061  s import beat_pa
+00002d20: 7468 0a20 2020 2020 2020 200a 2020 2020  th.        .    
+00002d30: 2020 2020 6d67 203d 204d 6172 6769 6e47      mg = MarginG
+00002d40: 7261 7068 285b 302c 2031 2c20 322c 2033  raph([0, 1, 2, 3
+00002d50: 5d2c 205b 2830 2c20 322c 2033 292c 2028  ], [(0, 2, 3), (
+00002d60: 312c 2030 2c20 3529 2c20 2832 2c20 312c  1, 0, 5), (2, 1,
+00002d70: 2035 292c 2028 322c 2033 2c20 3129 2c20   5), (2, 3, 1), 
+00002d80: 2833 2c20 302c 2033 292c 2028 332c 2031  (3, 0, 3), (3, 1
+00002d90: 2c20 3129 5d29 0a20 2020 2020 2020 200a  , 1)]).        .
+00002da0: 2020 2020 2020 2020 6265 6174 5f70 6174          beat_pat
+00002db0: 682e 6469 7370 6c61 7928 6d67 290a 2020  h.display(mg).  
+00002dc0: 2020 2020 2020 6265 6174 5f70 6174 682e        beat_path.
+00002dd0: 6469 7370 6c61 7928 6d67 2c20 616c 676f  display(mg, algo
+00002de0: 7269 7468 6d3d 2766 6c6f 7964 5f77 6172  rithm='floyd_war
+00002df0: 7368 616c 6c27 2920 0a20 2020 2020 2020  shall') .       
+00002e00: 2062 6561 745f 7061 7468 2e64 6973 706c   beat_path.displ
+00002e10: 6179 286d 672c 2061 6c67 6f72 6974 686d  ay(mg, algorithm
+00002e20: 3d27 6261 7369 6327 290a 2020 2020 2222  ='basic').    ""
+00002e30: 220a 0a20 2020 2069 6620 616c 676f 7269  "..    if algori
+00002e40: 7468 6d20 3d3d 2027 666c 6f79 645f 7761  thm == 'floyd_wa
+00002e50: 7273 6861 6c6c 273a 0a20 2020 2020 2020  rshall':.       
+00002e60: 2072 6574 7572 6e20 5f62 6561 745f 7061   return _beat_pa
+00002e70: 7468 5f66 6c6f 7964 5f77 6172 7368 616c  th_floyd_warshal
+00002e80: 6c28 6564 6174 612c 2063 7572 725f 6361  l(edata, curr_ca
+00002e90: 6e64 7320 3d20 6375 7272 5f63 616e 6473  nds = curr_cands
+00002ea0: 2c20 7374 7265 6e67 7468 5f66 756e 6374  , strength_funct
+00002eb0: 696f 6e20 3d20 7374 7265 6e67 7468 5f66  ion = strength_f
+00002ec0: 756e 6374 696f 6e29 0a20 2020 2065 6c69  unction).    eli
+00002ed0: 6620 616c 676f 7269 7468 6d20 3d3d 2027  f algorithm == '
+00002ee0: 6261 7369 6327 3a0a 2020 2020 2020 2020  basic':.        
+00002ef0: 7265 7475 726e 205f 6265 6174 5f70 6174  return _beat_pat
+00002f00: 685f 6261 7369 6328 6564 6174 612c 2063  h_basic(edata, c
+00002f10: 7572 725f 6361 6e64 7320 3d20 6375 7272  urr_cands = curr
+00002f20: 5f63 616e 6473 2c20 7374 7265 6e67 7468  _cands, strength
+00002f30: 5f66 756e 6374 696f 6e20 3d20 7374 7265  _function = stre
+00002f40: 6e67 7468 5f66 756e 6374 696f 6e29 0a20  ngth_function). 
+00002f50: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00002f60: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00002f70: 7228 2249 6e76 616c 6964 2061 6c67 6f72  r("Invalid algor
+00002f80: 6974 686d 2073 7065 6369 6669 6564 2e22  ithm specified."
+00002f90: 290a 0a64 6566 2062 6561 745f 7061 7468  )..def beat_path
+00002fa0: 5f64 6566 6561 7428 6564 6174 612c 2063  _defeat(edata, c
+00002fb0: 7572 725f 6361 6e64 7320 3d20 4e6f 6e65  urr_cands = None
+00002fc0: 2c20 7374 7265 6e67 7468 5f66 756e 6374  , strength_funct
+00002fd0: 696f 6e20 3d20 4e6f 6e65 293a 2020 200a  ion = None):   .
+00002fe0: 2020 2020 2222 2252 6574 7572 6e73 2074      """Returns t
+00002ff0: 6865 2064 6566 6561 7420 7265 6c61 7469  he defeat relati
+00003000: 6f6e 2066 6f72 2042 6561 7420 5061 7468  on for Beat Path
+00003010: 2e20 0a20 2020 200a 2020 2020 4172 6773  . .    .    Args
+00003020: 3a0a 2020 2020 2020 2020 6564 6174 6120  :.        edata 
+00003030: 2850 726f 6669 6c65 2c20 5072 6f66 696c  (Profile, Profil
+00003040: 6557 6974 6854 6965 732c 204d 6172 6769  eWithTies, Margi
+00003050: 6e47 7261 7068 293a 2041 6e79 2065 6c65  nGraph): Any ele
+00003060: 6374 696f 6e20 6461 7461 2074 6861 7420  ction data that 
+00003070: 6861 7320 6120 606d 6172 6769 6e60 206d  has a `margin` m
+00003080: 6574 686f 642e 200a 2020 2020 2020 2020  ethod. .        
+00003090: 6375 7272 5f63 616e 6473 2028 4c69 7374  curr_cands (List
+000030a0: 5b69 6e74 5d2c 206f 7074 696f 6e61 6c29  [int], optional)
+000030b0: 3a20 4966 2073 6574 2c20 7468 656e 2066  : If set, then f
+000030c0: 696e 6420 7468 6520 7769 6e6e 6572 7320  ind the winners 
+000030d0: 666f 7220 7468 6520 7072 6f66 696c 6520  for the profile 
+000030e0: 7265 7374 7269 6374 6564 2074 6f20 7468  restricted to th
+000030f0: 6520 6361 6e64 6964 6174 6573 2069 6e20  e candidates in 
+00003100: 6060 6375 7272 5f63 616e 6473 6060 0a20  ``curr_cands``. 
+00003110: 2020 2020 2020 2073 7472 656e 6774 685f         strength_
+00003120: 6675 6e63 7469 6f6e 2028 6675 6e63 7469  function (functi
+00003130: 6f6e 2c20 6f70 7469 6f6e 616c 293a 2054  on, optional): T
+00003140: 6865 2073 7472 656e 6774 6820 6675 6e63  he strength func
+00003150: 7469 6f6e 2074 6f20 6265 2075 7365 6420  tion to be used 
+00003160: 746f 2063 616c 6375 6c61 7465 2074 6865  to calculate the
+00003170: 2073 7472 656e 6774 6820 6f66 2061 2070   strength of a p
+00003180: 6174 682e 2020 2054 6865 2064 6566 6175  ath.   The defau
+00003190: 6c74 2069 7320 7468 6520 6d61 7267 696e  lt is the margin
+000031a0: 206d 6574 686f 6420 6f66 2060 6065 6461   method of ``eda
+000031b0: 7461 6060 2e20 2020 5468 6973 206f 6e6c  ta``.   This onl
+000031c0: 7920 6d61 7474 6572 7320 7768 656e 2074  y matters when t
+000031d0: 6865 2062 616c 6c6f 7473 2061 7265 206e  he ballots are n
+000031e0: 6f74 206c 696e 6561 7220 6f72 6465 7273  ot linear orders
+000031f0: 2e20 0a0a 2020 2020 5265 7475 726e 733a  . ..    Returns:
+00003200: 200a 2020 2020 2020 2020 4120 6e65 7477   .        A netw
+00003210: 6f72 6b78 2044 6947 7261 7068 2072 6570  orkx DiGraph rep
+00003220: 7265 7365 6e74 696e 6720 7468 6520 4265  resenting the Be
+00003230: 6174 2050 6174 6820 6465 6665 6174 2072  at Path defeat r
+00003240: 656c 6174 696f 6e2e 200a 0a20 2020 202e  elation. ..    .
+00003250: 2e20 7365 6561 6c73 6f3a 3a0a 0a20 2020  . seealso::..   
+00003260: 2020 2020 203a 6d65 7468 3a60 7072 6566       :meth:`pref
+00003270: 5f76 6f74 696e 672e 6d61 7267 696e 5f62  _voting.margin_b
+00003280: 6173 6564 5f6d 6574 686f 6473 2e62 6561  ased_methods.bea
+00003290: 745f 7061 7468 602c 203a 6d65 7468 3a60  t_path`, :meth:`
+000032a0: 7072 6566 5f76 6f74 696e 672e 6d61 7267  pref_voting.marg
+000032b0: 696e 5f62 6173 6564 5f6d 6574 686f 6473  in_based_methods
+000032c0: 2e62 6561 745f 7061 7468 5f46 6c6f 7964  .beat_path_Floyd
+000032d0: 5f57 6172 7368 616c 6c60 0a0a 2020 2020  _Warshall`..    
+000032e0: 3a45 7861 6d70 6c65 3a20 0a0a 2020 2020  :Example: ..    
+000032f0: 2e2e 2070 6c6f 743a 3a20 206d 6172 6769  .. plot::  margi
+00003300: 6e5f 6772 6170 6873 5f65 7861 6d70 6c65  n_graphs_example
+00003310: 732f 6d67 5f65 785f 6270 5f64 6566 6561  s/mg_ex_bp_defea
+00003320: 742e 7079 0a20 2020 2020 2020 203a 636f  t.py.        :co
+00003330: 6e74 6578 743a 2072 6573 6574 2020 0a20  ntext: reset  . 
+00003340: 2020 2020 2020 203a 696e 636c 7564 652d         :include-
+00003350: 736f 7572 6365 3a20 5472 7565 0a0a 2020  source: True..  
+00003360: 2020 2222 220a 0a20 2020 2063 616e 6469    """..    candi
+00003370: 6461 7465 7320 3d20 6564 6174 612e 6361  dates = edata.ca
+00003380: 6e64 6964 6174 6573 2069 6620 6375 7272  ndidates if curr
+00003390: 5f63 616e 6473 2069 7320 4e6f 6e65 2065  _cands is None e
+000033a0: 6c73 6520 6375 7272 5f63 616e 6473 2020  lse curr_cands  
+000033b0: 2020 0a20 2020 2073 7472 656e 6774 685f    .    strength_
+000033c0: 6675 6e63 7469 6f6e 203d 2065 6461 7461  function = edata
+000033d0: 2e6d 6172 6769 6e20 6966 2073 7472 656e  .margin if stren
+000033e0: 6774 685f 6675 6e63 7469 6f6e 2069 7320  gth_function is 
+000033f0: 4e6f 6e65 2065 6c73 6520 7374 7265 6e67  None else streng
+00003400: 7468 5f66 756e 6374 696f 6e0a 2020 2020  th_function.    
+00003410: 2020 2020 0a20 2020 2073 5f6d 6174 7269      .    s_matri
+00003420: 7820 3d20 5b5b 2d6e 702e 696e 6620 666f  x = [[-np.inf fo
+00003430: 7220 5f20 696e 2063 616e 6469 6461 7465  r _ in candidate
+00003440: 735d 2066 6f72 205f 2069 6e20 6361 6e64  s] for _ in cand
+00003450: 6964 6174 6573 5d0a 2020 2020 666f 7220  idates].    for 
+00003460: 6331 5f69 6478 2c20 6331 2069 6e20 656e  c1_idx, c1 in en
+00003470: 756d 6572 6174 6528 6361 6e64 6964 6174  umerate(candidat
+00003480: 6573 293a 0a20 2020 2020 2020 2066 6f72  es):.        for
+00003490: 2063 325f 6964 782c 2063 3220 696e 2065   c2_idx, c2 in e
+000034a0: 6e75 6d65 7261 7465 2863 616e 6469 6461  numerate(candida
+000034b0: 7465 7329 3a0a 2020 2020 2020 2020 2020  tes):.          
+000034c0: 2020 6966 2028 6564 6174 612e 6d61 6a6f    if (edata.majo
+000034d0: 7269 7479 5f70 7265 6665 7273 2863 312c  rity_prefers(c1,
+000034e0: 2063 3229 206f 7220 6331 203d 3d20 6332   c2) or c1 == c2
+000034f0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00003500: 2020 2073 5f6d 6174 7269 785b 6331 5f69     s_matrix[c1_i
+00003510: 6478 5d5b 6332 5f69 6478 5d20 3d20 7374  dx][c2_idx] = st
+00003520: 7265 6e67 7468 5f66 756e 6374 696f 6e28  rength_function(
+00003530: 6331 2c20 6332 2920 0a20 2020 2073 7472  c1, c2) .    str
+00003540: 656e 6774 6820 3d20 6c69 7374 286d 6170  ength = list(map
+00003550: 286c 616d 6264 6120 6920 3a20 6c69 7374  (lambda i : list
+00003560: 286d 6170 286c 616d 6264 6120 6a20 3a20  (map(lambda j : 
+00003570: 6a20 2c20 6929 2920 2c20 735f 6d61 7472  j , i)) , s_matr
+00003580: 6978 2929 0a20 2020 2066 6f72 2069 5f69  ix)).    for i_i
+00003590: 6478 2c20 6920 696e 2065 6e75 6d65 7261  dx, i in enumera
+000035a0: 7465 2863 616e 6469 6461 7465 7329 3a20  te(candidates): 
+000035b0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000035c0: 2066 6f72 206a 5f69 6478 2c20 6a20 696e   for j_idx, j in
+000035d0: 2065 6e75 6d65 7261 7465 2863 616e 6469   enumerate(candi
+000035e0: 6461 7465 7329 3a20 0a20 2020 2020 2020  dates): .       
+000035f0: 2020 2020 2069 6620 6921 3d20 6a3a 0a20       if i!= j:. 
+00003600: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00003610: 6f72 206b 5f69 6478 2c20 6b20 696e 2065  or k_idx, k in e
+00003620: 6e75 6d65 7261 7465 2863 616e 6469 6461  numerate(candida
+00003630: 7465 7329 3a20 0a20 2020 2020 2020 2020  tes): .         
+00003640: 2020 2020 2020 2020 2020 2069 6620 6921             if i!
+00003650: 3d20 6b20 616e 6420 6a20 213d 206b 3a0a  = k and j != k:.
+00003660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003670: 2020 2020 2020 2020 7374 7265 6e67 7468          strength
+00003680: 5b6a 5f69 6478 5d5b 6b5f 6964 785d 203d  [j_idx][k_idx] =
+00003690: 206d 6178 2873 7472 656e 6774 685b 6a5f   max(strength[j_
+000036a0: 6964 785d 5b6b 5f69 6478 5d2c 206d 696e  idx][k_idx], min
+000036b0: 2873 7472 656e 6774 685b 6a5f 6964 785d  (strength[j_idx]
+000036c0: 5b69 5f69 6478 5d2c 7374 7265 6e67 7468  [i_idx],strength
+000036d0: 5b69 5f69 6478 5d5b 6b5f 6964 785d 2929  [i_idx][k_idx]))
+000036e0: 0a0a 2020 2020 6465 6665 6174 5f67 7261  ..    defeat_gra
+000036f0: 7068 203d 206e 782e 4469 4772 6170 6828  ph = nx.DiGraph(
+00003700: 290a 2020 2020 6465 6665 6174 5f67 7261  ).    defeat_gra
+00003710: 7068 2e61 6464 5f6e 6f64 6573 5f66 726f  ph.add_nodes_fro
+00003720: 6d28 6361 6e64 6964 6174 6573 290a 2020  m(candidates).  
+00003730: 2020 0a20 2020 2066 6f72 2069 5f69 6478    .    for i_idx
+00003740: 2c20 6920 696e 2065 6e75 6d65 7261 7465  , i in enumerate
+00003750: 2863 616e 6469 6461 7465 7329 3a20 0a20  (candidates): . 
+00003760: 2020 2020 2020 2066 6f72 206a 5f69 6478         for j_idx
+00003770: 2c20 6a20 696e 2065 6e75 6d65 7261 7465  , j in enumerate
+00003780: 2863 616e 6469 6461 7465 7329 3a0a 2020  (candidates):.  
+00003790: 2020 2020 2020 2020 2020 6966 2069 213d            if i!=
+000037a0: 6a3a 0a20 2020 2020 2020 2020 2020 2020  j:.             
+000037b0: 2020 2069 6620 7374 7265 6e67 7468 5b6a     if strength[j
+000037c0: 5f69 6478 5d5b 695f 6964 785d 203e 2073  _idx][i_idx] > s
+000037d0: 7472 656e 6774 685b 695f 6964 785d 5b6a  trength[i_idx][j
+000037e0: 5f69 6478 5d3a 0a20 2020 2020 2020 2020  _idx]:.         
+000037f0: 2020 2020 2020 2020 2020 2064 6566 6561             defea
+00003800: 745f 6772 6170 682e 6164 645f 7765 6967  t_graph.add_weig
+00003810: 6874 6564 5f65 6467 6573 5f66 726f 6d28  hted_edges_from(
+00003820: 5b28 6a2c 692c 735f 6d61 7472 6978 5b6a  [(j,i,s_matrix[j
+00003830: 5f69 6478 5d5b 695f 6964 785d 295d 290a  _idx][i_idx])]).
+00003840: 0a20 2020 2072 6574 7572 6e20 6465 6665  .    return defe
+00003850: 6174 5f67 7261 7068 0a0a 0a0a 6465 6620  at_graph....def 
+00003860: 6861 735f 7374 726f 6e67 5f70 6174 6828  has_strong_path(
+00003870: 412c 2073 6f75 7263 652c 2074 6172 6765  A, source, targe
+00003880: 742c 206b 293a 0a20 2020 2022 2222 4769  t, k):.    """Gi
+00003890: 7665 6e20 6120 7371 7561 7265 206d 6174  ven a square mat
+000038a0: 7269 7820 412c 2072 6574 7572 6e20 5472  rix A, return Tr
+000038b0: 7565 2069 6620 7468 6572 6520 6973 2061  ue if there is a
+000038c0: 2070 6174 6820 6672 6f6d 2073 6f75 7263   path from sourc
+000038d0: 6520 746f 2074 6172 6765 7420 696e 2074  e to target in t
+000038e0: 6865 2061 7373 6f63 6961 7465 6420 6469  he associated di
+000038f0: 7265 6374 6564 2067 7261 7068 2020 2020  rected graph    
+00003900: 2077 6865 7265 2065 6163 6820 6564 6765   where each edge
+00003910: 2068 6173 2061 2077 6569 6768 7420 6772   has a weight gr
+00003920: 6561 7465 7220 7468 616e 206f 7220 6571  eater than or eq
+00003930: 7561 6c20 746f 206b 2c20 616e 6420 4661  ual to k, and Fa
+00003940: 6c73 6520 6f74 6865 7277 6973 652e 2222  lse otherwise.""
+00003950: 220a 2020 2020 0a20 2020 206e 203d 2041  ".    .    n = A
+00003960: 2e73 6861 7065 5b30 5d20 2320 6173 7375  .shape[0] # assu
+00003970: 6d65 2041 2069 7320 6120 7371 7561 7265  me A is a square
+00003980: 206d 6174 7269 780a 2020 2020 7669 7369   matrix.    visi
+00003990: 7465 6420 3d20 6e70 2e7a 6572 6f73 286e  ted = np.zeros(n
+000039a0: 2c20 6474 7970 653d 626f 6f6c 290a 0a20  , dtype=bool).. 
+000039b0: 2020 2064 6566 2064 6673 286e 6f64 6529     def dfs(node)
+000039c0: 3a0a 2020 2020 2020 2020 6966 206e 6f64  :.        if nod
+000039d0: 6520 3d3d 2074 6172 6765 743a 0a20 2020  e == target:.   
+000039e0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000039f0: 5472 7565 0a20 2020 2020 2020 2076 6973  True.        vis
+00003a00: 6974 6564 5b6e 6f64 655d 203d 2054 7275  ited[node] = Tru
+00003a10: 650a 2020 2020 2020 2020 666f 7220 6e65  e.        for ne
+00003a20: 6967 6862 6f72 2c20 7765 6967 6874 2069  ighbor, weight i
+00003a30: 6e20 656e 756d 6572 6174 6528 415b 6e6f  n enumerate(A[no
+00003a40: 6465 2c20 3a5d 293a 0a20 2020 2020 2020  de, :]):.       
+00003a50: 2020 2020 2069 6620 415b 6e6f 6465 5d5b       if A[node][
+00003a60: 6e65 6967 6862 6f72 5d20 3e20 415b 6e65  neighbor] > A[ne
+00003a70: 6967 6862 6f72 5d5b 6e6f 6465 5d20 616e  ighbor][node] an
+00003a80: 6420 7765 6967 6874 203e 3d20 6b20 616e  d weight >= k an
+00003a90: 6420 6e6f 7420 7669 7369 7465 645b 6e65  d not visited[ne
+00003aa0: 6967 6862 6f72 5d3a 0a20 2020 2020 2020  ighbor]:.       
+00003ab0: 2020 2020 2020 2020 2069 6620 6466 7328           if dfs(
+00003ac0: 6e65 6967 6862 6f72 293a 0a20 2020 2020  neighbor):.     
+00003ad0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00003ae0: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
+00003af0: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+00003b00: 0a20 2020 2072 6574 7572 6e20 6466 7328  .    return dfs(
+00003b10: 736f 7572 6365 290a 0a64 6566 205f 7370  source)..def _sp
+00003b20: 6c69 745f 6379 636c 655f 6261 7369 6328  lit_cycle_basic(
+00003b30: 0a20 2020 2020 2020 2065 6461 7461 2c20  .        edata, 
+00003b40: 0a20 2020 2020 2020 2063 7572 725f 6361  .        curr_ca
+00003b50: 6e64 7320 3d20 4e6f 6e65 2c20 0a20 2020  nds = None, .   
+00003b60: 2020 2020 2073 7472 656e 6774 685f 6675       strength_fu
+00003b70: 6e63 7469 6f6e 203d 204e 6f6e 6529 3a0a  nction = None):.
+00003b80: 2020 2020 2222 2241 6e20 696d 706c 656d      """An implem
+00003b90: 656e 7461 7469 6f6e 206f 6620 5370 6c69  entation of Spli
+00003ba0: 7420 4379 636c 6520 6261 7365 6420 6f6e  t Cycle based on
+00003bb0: 2074 6865 206d 6174 6865 6d61 7469 6361   the mathematica
+00003bc0: 6c20 6465 6669 6e69 7469 6f6e 2e20 2054  l definition.  T
+00003bd0: 6869 7320 6973 206d 6f72 6520 6566 6669  his is more effi
+00003be0: 6369 656e 7420 7468 616e 2074 6865 2066  cient than the f
+00003bf0: 6c6f 7964 5f77 6172 7368 616c 6c20 696d  loyd_warshall im
+00003c00: 706c 656d 656e 7461 7469 6f6e 2e20 0a20  plementation. . 
+00003c10: 2020 2022 2222 0a20 2020 2073 7472 656e     """.    stren
+00003c20: 6774 685f 6d61 7472 6978 2c20 6361 6e64  gth_matrix, cand
+00003c30: 5f74 6f5f 6369 6e64 6578 203d 2065 6461  _to_cindex = eda
+00003c40: 7461 2e73 7472 656e 6774 685f 6d61 7472  ta.strength_matr
+00003c50: 6978 2863 7572 725f 6361 6e64 7320 3d20  ix(curr_cands = 
+00003c60: 6375 7272 5f63 616e 6473 2c20 7374 7265  curr_cands, stre
+00003c70: 6e67 7468 5f66 756e 6374 696f 6e3d 7374  ngth_function=st
+00003c80: 7265 6e67 7468 5f66 756e 6374 696f 6e29  rength_function)
+00003c90: 0a0a 2020 2020 6361 6e64 6964 6174 6573  ..    candidates
+00003ca0: 203d 2065 6461 7461 2e63 616e 6469 6461   = edata.candida
+00003cb0: 7465 7320 6966 2063 7572 725f 6361 6e64  tes if curr_cand
+00003cc0: 7320 6973 204e 6f6e 6520 656c 7365 2063  s is None else c
+00003cd0: 7572 725f 6361 6e64 7320 200a 0a20 2020  urr_cands  ..   
+00003ce0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+00003cf0: 6f6e 203d 2065 6461 7461 2e6d 6172 6769  on = edata.margi
+00003d00: 6e20 6966 2073 7472 656e 6774 685f 6675  n if strength_fu
+00003d10: 6e63 7469 6f6e 2069 7320 4e6f 6e65 2065  nction is None e
+00003d20: 6c73 6520 7374 7265 6e67 7468 5f66 756e  lse strength_fun
+00003d30: 6374 696f 6e20 0a0a 2020 2020 706f 7465  ction ..    pote
+00003d40: 6e74 6961 6c5f 7769 6e6e 6572 7320 3d20  ntial_winners = 
+00003d50: 7365 7428 6361 6e64 6964 6174 6573 290a  set(candidates).
+00003d60: 0a20 2020 2066 6f72 2061 2069 6e20 6361  .    for a in ca
+00003d70: 6e64 6964 6174 6573 3a0a 2020 2020 2020  ndidates:.      
+00003d80: 2020 666f 7220 6220 696e 2063 616e 6469    for b in candi
+00003d90: 6461 7465 733a 0a20 2020 2020 2020 2020  dates:.         
+00003da0: 2020 2069 6620 7374 7265 6e67 7468 5f66     if strength_f
+00003db0: 756e 6374 696f 6e28 622c 2061 2920 3e20  unction(b, a) > 
+00003dc0: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+00003dd0: 6e28 612c 2062 2920 616e 6420 6e6f 7420  n(a, b) and not 
+00003de0: 6861 735f 7374 726f 6e67 5f70 6174 6828  has_strong_path(
+00003df0: 7374 7265 6e67 7468 5f6d 6174 7269 782c  strength_matrix,
+00003e00: 2063 616e 645f 746f 5f63 696e 6465 7828   cand_to_cindex(
+00003e10: 6129 2c20 6361 6e64 5f74 6f5f 6369 6e64  a), cand_to_cind
+00003e20: 6578 2862 292c 2073 7472 656e 6774 685f  ex(b), strength_
+00003e30: 6675 6e63 7469 6f6e 2862 2c61 2929 3a0a  function(b,a)):.
+00003e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e50: 706f 7465 6e74 6961 6c5f 7769 6e6e 6572  potential_winner
+00003e60: 732e 6469 7363 6172 6428 6129 0a20 2020  s.discard(a).   
+00003e70: 2020 2020 2020 2020 2020 2020 2062 7265               bre
+00003e80: 616b 0a0a 2020 2020 7265 7475 726e 2073  ak..    return s
+00003e90: 6f72 7465 6428 706f 7465 6e74 6961 6c5f  orted(potential_
+00003ea0: 7769 6e6e 6572 7329 0a0a 6465 6620 5f73  winners)..def _s
+00003eb0: 706c 6974 5f63 7963 6c65 5f66 6c6f 7964  plit_cycle_floyd
+00003ec0: 5f77 6172 7368 616c 6c28 0a20 2020 2020  _warshall(.     
+00003ed0: 2020 2065 6461 7461 2c20 0a20 2020 2020     edata, .     
+00003ee0: 2020 2063 7572 725f 6361 6e64 7320 3d20     curr_cands = 
+00003ef0: 4e6f 6e65 2c20 0a20 2020 2020 2020 2073  None, .        s
+00003f00: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+00003f10: 203d 204e 6f6e 6529 3a20 2020 0a20 2020   = None):   .   
+00003f20: 2022 2222 416e 2069 6d70 6c65 6d65 6e74   """An implement
+00003f30: 6174 696f 6e20 6f66 2053 706c 6974 2043  ation of Split C
+00003f40: 7963 6c65 2062 6173 6564 206f 6e20 7468  ycle based on th
+00003f50: 6520 466c 6f79 642d 5761 7273 6861 6c6c  e Floyd-Warshall
+00003f60: 2041 6c67 6f72 6974 686d 2e20 0a0a 2020   Algorithm. ..  
+00003f70: 2020 5365 6520 6874 7470 733a 2f2f 6769    See https://gi
+00003f80: 7468 7562 2e63 6f6d 2f65 7061 6375 6974  thub.com/epacuit
+00003f90: 2f73 706c 6974 6379 636c 6520 616e 6420  /splitcycle and 
+00003fa0: 7468 6520 7061 7065 7220 6874 7470 733a  the paper https:
+00003fb0: 2f2f 6172 7869 762e 6f72 672f 6162 732f  //arxiv.org/abs/
+00003fc0: 3230 3034 2e30 3233 3530 2066 6f72 206d  2004.02350 for m
+00003fd0: 6f72 6520 696e 666f 726d 6174 696f 6e2e  ore information.
+00003fe0: 200a 0a20 2020 2022 2222 0a0a 2020 2020   ..    """..    
+00003ff0: 6361 6e64 6964 6174 6573 203d 2065 6461  candidates = eda
+00004000: 7461 2e63 616e 6469 6461 7465 7320 6966  ta.candidates if
+00004010: 2063 7572 725f 6361 6e64 7320 6973 204e   curr_cands is N
+00004020: 6f6e 6520 656c 7365 2063 7572 725f 6361  one else curr_ca
+00004030: 6e64 7320 2020 200a 2020 2020 7374 7265  nds    .    stre
+00004040: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
+00004050: 6564 6174 612e 6d61 7267 696e 2069 6620  edata.margin if 
+00004060: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+00004070: 6e20 6973 204e 6f6e 6520 656c 7365 2073  n is None else s
+00004080: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+00004090: 200a 200a 2020 2020 7765 616b 5f63 6f6e   . .    weak_con
+000040a0: 646f 7263 6574 5f77 696e 6e65 7273 203d  dorcet_winners =
+000040b0: 207b 633a 5472 7565 2066 6f72 2063 2069   {c:True for c i
+000040c0: 6e20 6361 6e64 6964 6174 6573 7d0a 2020  n candidates}.  
+000040d0: 2020 735f 6d61 7472 6978 203d 205b 5b2d    s_matrix = [[-
+000040e0: 6e70 2e69 6e66 2066 6f72 205f 2069 6e20  np.inf for _ in 
+000040f0: 6361 6e64 6964 6174 6573 5d20 666f 7220  candidates] for 
+00004100: 5f20 696e 2063 616e 6469 6461 7465 735d  _ in candidates]
+00004110: 0a20 2020 200a 2020 2020 2320 696e 6974  .    .    # init
+00004120: 6961 6c69 7a65 2074 6865 2073 5f6d 6174  ialize the s_mat
+00004130: 7269 780a 2020 2020 666f 7220 6331 5f69  rix.    for c1_i
+00004140: 6478 2c20 6331 2069 6e20 656e 756d 6572  dx, c1 in enumer
+00004150: 6174 6528 6361 6e64 6964 6174 6573 293a  ate(candidates):
+00004160: 0a20 2020 2020 2020 2066 6f72 2063 325f  .        for c2_
+00004170: 6964 782c 2063 3220 696e 2065 6e75 6d65  idx, c2 in enume
+00004180: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
+00004190: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+000041a0: 2028 6564 6174 612e 6d61 6a6f 7269 7479   (edata.majority
+000041b0: 5f70 7265 6665 7273 2863 312c 2063 3229  _prefers(c1, c2)
+000041c0: 206f 7220 6331 203d 3d20 6332 293a 0a20   or c1 == c2):. 
+000041d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000041e0: 5f6d 6174 7269 785b 6331 5f69 6478 5d5b  _matrix[c1_idx][
+000041f0: 6332 5f69 6478 5d20 3d20 7374 7265 6e67  c2_idx] = streng
+00004200: 7468 5f66 756e 6374 696f 6e28 6331 2c20  th_function(c1, 
+00004210: 6332 2920 0a20 2020 2020 2020 2020 2020  c2) .           
+00004220: 2020 2020 2077 6561 6b5f 636f 6e64 6f72       weak_condor
+00004230: 6365 745f 7769 6e6e 6572 735b 6332 5d20  cet_winners[c2] 
+00004240: 3d20 7765 616b 5f63 6f6e 646f 7263 6574  = weak_condorcet
+00004250: 5f77 696e 6e65 7273 5b63 325d 2061 6e64  _winners[c2] and
+00004260: 2028 6331 203d 3d20 6332 2920 2320 5765   (c1 == c2) # We
+00004270: 616b 2043 6f6e 646f 7263 6574 2077 696e  ak Condorcet win
+00004280: 6e65 7273 2061 7265 2053 706c 6974 2043  ners are Split C
+00004290: 7963 6c65 2077 696e 6e65 7273 0a20 2020  ycle winners.   
+000042a0: 200a 2020 2020 7374 7265 6e67 7468 203d   .    strength =
+000042b0: 206c 6973 7428 6d61 7028 6c61 6d62 6461   list(map(lambda
+000042c0: 2069 203a 206c 6973 7428 6d61 7028 6c61   i : list(map(la
+000042d0: 6d62 6461 206a 203a 206a 202c 2069 2929  mbda j : j , i))
+000042e0: 202c 2073 5f6d 6174 7269 7829 290a 2020   , s_matrix)).  
+000042f0: 2020 666f 7220 695f 6964 782c 2069 2069    for i_idx, i i
+00004300: 6e20 656e 756d 6572 6174 6528 6361 6e64  n enumerate(cand
+00004310: 6964 6174 6573 293a 200a 2020 2020 2020  idates): .      
+00004320: 2020 666f 7220 6a5f 6964 782c 206a 2069    for j_idx, j i
+00004330: 6e20 656e 756d 6572 6174 6528 6361 6e64  n enumerate(cand
+00004340: 6964 6174 6573 293a 0a20 2020 2020 2020  idates):.       
+00004350: 2020 2020 2069 6620 6921 3d20 6a3a 0a20       if i!= j:. 
+00004360: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00004370: 6620 6e6f 7420 7765 616b 5f63 6f6e 646f  f not weak_condo
+00004380: 7263 6574 5f77 696e 6e65 7273 5b6a 5d3a  rcet_winners[j]:
+00004390: 2023 2077 6561 6b20 436f 6e64 6f72 6365   # weak Condorce
+000043a0: 7420 7769 6e6e 6572 7320 6172 6520 5370  t winners are Sp
+000043b0: 6c69 7420 4379 636c 6520 7769 6e6e 6572  lit Cycle winner
+000043c0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+000043d0: 2020 2020 2020 666f 7220 6b5f 6964 782c        for k_idx,
+000043e0: 206b 2069 6e20 656e 756d 6572 6174 6528   k in enumerate(
+000043f0: 6361 6e64 6964 6174 6573 293a 200a 2020  candidates): .  
+00004400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004410: 2020 2020 2020 6966 2069 2021 3d20 6b20        if i != k 
+00004420: 616e 6420 6a20 213d 206b 3a0a 2020 2020  and j != k:.    
+00004430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004440: 2020 2020 2020 2020 7374 7265 6e67 7468          strength
+00004450: 5b6a 5f69 6478 5d5b 6b5f 6964 785d 203d  [j_idx][k_idx] =
+00004460: 206d 6178 2873 7472 656e 6774 685b 6a5f   max(strength[j_
+00004470: 6964 785d 5b6b 5f69 6478 5d2c 206d 696e  idx][k_idx], min
+00004480: 2873 7472 656e 6774 685b 6a5f 6964 785d  (strength[j_idx]
+00004490: 5b69 5f69 6478 5d2c 7374 7265 6e67 7468  [i_idx],strength
+000044a0: 5b69 5f69 6478 5d5b 6b5f 6964 785d 2929  [i_idx][k_idx]))
+000044b0: 0a20 2020 2077 696e 6e65 7273 203d 207b  .    winners = {
+000044c0: 693a 5472 7565 2066 6f72 2069 2069 6e20  i:True for i in 
+000044d0: 6361 6e64 6964 6174 6573 7d0a 2020 2020  candidates}.    
+000044e0: 666f 7220 695f 6964 782c 2069 2069 6e20  for i_idx, i in 
+000044f0: 656e 756d 6572 6174 6528 6361 6e64 6964  enumerate(candid
+00004500: 6174 6573 293a 0a20 2020 2020 2020 2066  ates):.        f
+00004510: 6f72 206a 5f69 6478 2c20 6a20 696e 2065  or j_idx, j in e
+00004520: 6e75 6d65 7261 7465 2863 616e 6469 6461  numerate(candida
+00004530: 7465 7329 3a0a 2020 2020 2020 2020 2020  tes):.          
+00004540: 2020 6966 2069 2021 3d20 6a3a 0a20 2020    if i != j:.   
+00004550: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00004560: 735f 6d61 7472 6978 5b6a 5f69 6478 5d5b  s_matrix[j_idx][
+00004570: 695f 6964 785d 203e 2073 7472 656e 6774  i_idx] > strengt
+00004580: 685b 695f 6964 785d 5b6a 5f69 6478 5d3a  h[i_idx][j_idx]:
+00004590: 2023 2074 6865 206d 6169 6e20 6469 6666   # the main diff
+000045a0: 6572 656e 6365 2077 6974 6820 4265 6174  erence with Beat
+000045b0: 2050 6174 680a 2020 2020 2020 2020 2020   Path.          
+000045c0: 2020 2020 2020 2020 2020 7769 6e6e 6572            winner
+000045d0: 735b 695d 203d 2046 616c 7365 0a20 2020  s[i] = False.   
+000045e0: 2072 6574 7572 6e20 736f 7274 6564 285b   return sorted([
+000045f0: 6320 666f 7220 6320 696e 2063 616e 6469  c for c in candi
+00004600: 6461 7465 7320 6966 2077 696e 6e65 7273  dates if winners
+00004610: 5b63 5d5d 290a 0a73 635f 7072 6f70 6572  [c]])..sc_proper
+00004620: 7469 6573 203d 2056 6f74 696e 674d 6574  ties = VotingMet
+00004630: 686f 6450 726f 7065 7274 6965 7328 0a20  hodProperties(. 
+00004640: 2020 2063 6f6e 646f 7263 6574 5f77 696e     condorcet_win
+00004650: 6e65 723d 5472 7565 2c20 0a20 2020 2063  ner=True, .    c
+00004660: 6f6e 646f 7263 6574 5f6c 6f73 6572 3d54  ondorcet_loser=T
+00004670: 7275 652c 0a20 2020 2070 6172 6574 6f5f  rue,.    pareto_
+00004680: 646f 6d69 6e61 6e63 653d 5472 7565 2c20  dominance=True, 
+00004690: 0a20 2020 2029 0a40 766d 286e 616d 653d  .    ).@vm(name=
+000046a0: 2253 706c 6974 2043 7963 6c65 222c 0a20  "Split Cycle",. 
+000046b0: 2020 2070 726f 7065 7274 6965 733d 7363     properties=sc
+000046c0: 5f70 726f 7065 7274 6965 732c 0a20 2020  _properties,.   
+000046d0: 2069 6e70 7574 5f74 7970 6573 3d5b 456c   input_types=[El
+000046e0: 6563 7469 6f6e 5479 7065 732e 5052 4f46  ectionTypes.PROF
+000046f0: 494c 452c 2045 6c65 6374 696f 6e54 7970  ILE, ElectionTyp
+00004700: 6573 2e50 524f 4649 4c45 5f57 4954 485f  es.PROFILE_WITH_
+00004710: 5449 4553 2c20 456c 6563 7469 6f6e 5479  TIES, ElectionTy
+00004720: 7065 732e 4d41 5247 494e 5f47 5241 5048  pes.MARGIN_GRAPH
+00004730: 5d29 0a64 6566 2073 706c 6974 5f63 7963  ]).def split_cyc
+00004740: 6c65 280a 2020 2020 6564 6174 612c 200a  le(.    edata, .
+00004750: 2020 2020 6375 7272 5f63 616e 6473 3d4e      curr_cands=N
+00004760: 6f6e 652c 200a 2020 2020 7374 7265 6e67  one, .    streng
+00004770: 7468 5f66 756e 6374 696f 6e3d 4e6f 6e65  th_function=None
+00004780: 2c0a 2020 2020 616c 676f 7269 7468 6d3d  ,.    algorithm=
+00004790: 2762 6173 6963 2729 3a0a 0a20 2020 2022  'basic'):..    "
+000047a0: 2222 4120 2a2a 6d61 6a6f 7269 7479 2063  ""A **majority c
+000047b0: 7963 6c65 2a2a 2069 7320 6120 7365 7175  ycle** is a sequ
+000047c0: 656e 6365 203a 6d61 7468 3a60 785f 312c  ence :math:`x_1,
+000047d0: 205c 6c64 6f74 7320 2c78 5f6e 6020 6f66   \ldots ,x_n` of
+000047e0: 2064 6973 7469 6e63 7420 6361 6e64 6964   distinct candid
+000047f0: 6174 6573 2077 6974 6820 3a6d 6174 683a  ates with :math:
+00004800: 6078 5f31 3d78 5f6e 6020 7375 6368 2074  `x_1=x_n` such t
+00004810: 6861 7420 666f 7220 3a6d 6174 683a 6031  hat for :math:`1
+00004820: 205c 6c65 7120 6b20 5c6c 6571 206e 2d31   \leq k \leq n-1
+00004830: 602c 2020 3a6d 6174 683a 6078 5f6b 6020  `,  :math:`x_k` 
+00004840: 6973 206d 616a 6f72 6974 7920 7072 6566  is majority pref
+00004850: 6572 7265 6420 746f 203a 6d61 7468 3a60  erred to :math:`
+00004860: 785f 7b6b 2b31 7d60 2e20 2054 6865 2053  x_{k+1}`.  The S
+00004870: 706c 6974 2043 7963 6c65 2077 696e 6e65  plit Cycle winne
+00004880: 7273 2061 7265 2064 6574 6572 6d69 6e65  rs are determine
+00004890: 6420 6173 2066 6f6c 6c6f 7773 3a20 200a  d as follows:  .
+000048a0: 2020 2020 0a20 2020 2049 6620 6361 6e64      .    If cand
+000048b0: 6964 6174 6520 7820 6861 7320 6120 706f  idate x has a po
+000048c0: 7369 7469 7665 206d 6172 6769 6e20 6f76  sitive margin ov
+000048d0: 6572 2079 2061 6e64 2028 782c 7929 2069  er y and (x,y) i
+000048e0: 7320 6e6f 7420 7468 6520 7765 616b 6573  s not the weakes
+000048f0: 7420 6564 6765 2069 6e20 6120 6379 636c  t edge in a cycl
+00004900: 652c 2074 6865 6e20 7820 6465 6665 6174  e, then x defeat
+00004910: 7320 792e 2045 7175 6976 616c 656e 746c  s y. Equivalentl
+00004920: 792c 2069 6620 7820 6861 7320 6120 706f  y, if x has a po
+00004930: 7369 7469 7665 206d 6172 6769 6e20 6f76  sitive margin ov
+00004940: 6572 2079 2061 6e64 2074 6865 7265 2069  er y and there i
+00004950: 7320 6e6f 2070 6174 6820 6672 6f6d 2079  s no path from y
+00004960: 2062 6163 6b20 746f 2078 206f 6620 7374   back to x of st
+00004970: 7265 6e67 7468 2061 7420 6c65 6173 7420  rength at least 
+00004980: 7468 6520 6d61 7267 696e 206f 6620 7820  the margin of x 
+00004990: 6f76 6572 2079 2c20 7468 656e 2078 2064  over y, then x d
+000049a0: 6566 6561 7473 2079 2e20 0a20 2020 200a  efeats y. .    .
+000049b0: 2020 2020 5468 6520 6361 6e64 6964 6174      The candidat
+000049c0: 6573 2074 6861 7420 6172 6520 756e 6465  es that are unde
+000049d0: 6665 6174 6564 2061 7265 2074 6865 2053  feated are the S
+000049e0: 706c 6974 2043 7963 6c65 2077 696e 6e65  plit Cycle winne
+000049f0: 7273 2e0a 0a20 2020 2053 6565 2068 7474  rs...    See htt
+00004a00: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00004a10: 6570 6163 7569 742f 7370 6c69 7463 7963  epacuit/splitcyc
+00004a20: 6c65 2061 6e64 2074 6865 2070 6170 6572  le and the paper
+00004a30: 2068 7474 7073 3a2f 2f61 7278 6976 2e6f   https://arxiv.o
+00004a40: 7267 2f61 6273 2f32 3030 342e 3032 3335  rg/abs/2004.0235
+00004a50: 3020 666f 7220 6d6f 7265 2069 6e66 6f72  0 for more infor
+00004a60: 6d61 7469 6f6e 2e20 0a0a 2020 2020 4172  mation. ..    Ar
+00004a70: 6773 3a0a 2020 2020 2020 2020 6564 6174  gs:.        edat
+00004a80: 6120 2850 726f 6669 6c65 2c20 5072 6f66  a (Profile, Prof
+00004a90: 696c 6557 6974 6854 6965 732c 204d 6172  ileWithTies, Mar
+00004aa0: 6769 6e47 7261 7068 293a 2041 6e79 2065  ginGraph): Any e
+00004ab0: 6c65 6374 696f 6e20 6461 7461 2074 6861  lection data tha
+00004ac0: 7420 6861 7320 6120 606d 6172 6769 6e60  t has a `margin`
+00004ad0: 206d 6574 686f 642e 200a 2020 2020 2020   method. .      
+00004ae0: 2020 6375 7272 5f63 616e 6473 2028 4c69    curr_cands (Li
+00004af0: 7374 5b69 6e74 5d2c 206f 7074 696f 6e61  st[int], optiona
+00004b00: 6c29 3a20 4966 2073 6574 2c20 7468 656e  l): If set, then
+00004b10: 2066 696e 6420 7468 6520 7769 6e6e 6572   find the winner
+00004b20: 7320 666f 7220 7468 6520 7072 6f66 696c  s for the profil
+00004b30: 6520 7265 7374 7269 6374 6564 2074 6f20  e restricted to 
+00004b40: 7468 6520 6361 6e64 6964 6174 6573 2069  the candidates i
+00004b50: 6e20 6060 6375 7272 5f63 616e 6473 6060  n ``curr_cands``
+00004b60: 0a20 2020 2020 2020 2073 7472 656e 6774  .        strengt
+00004b70: 685f 6675 6e63 7469 6f6e 2028 6675 6e63  h_function (func
+00004b80: 7469 6f6e 2c20 6f70 7469 6f6e 616c 293a  tion, optional):
+00004b90: 2054 6865 2073 7472 656e 6774 6820 6675   The strength fu
+00004ba0: 6e63 7469 6f6e 2074 6f20 6265 2075 7365  nction to be use
+00004bb0: 6420 746f 2063 616c 6375 6c61 7465 2074  d to calculate t
+00004bc0: 6865 2073 7472 656e 6774 6820 6f66 2061  he strength of a
+00004bd0: 2070 6174 682e 2020 2054 6865 2064 6566   path.   The def
+00004be0: 6175 6c74 2069 7320 7468 6520 6d61 7267  ault is the marg
+00004bf0: 696e 206d 6574 686f 6420 6f66 2060 6065  in method of ``e
+00004c00: 6461 7461 6060 2e20 2020 5468 6973 206f  data``.   This o
+00004c10: 6e6c 7920 6d61 7474 6572 7320 7768 656e  nly matters when
+00004c20: 2074 6865 2062 616c 6c6f 7473 2061 7265   the ballots are
+00004c30: 206e 6f74 206c 696e 6561 7220 6f72 6465   not linear orde
+00004c40: 7273 2e20 0a20 2020 2020 2020 2061 6c67  rs. .        alg
+00004c50: 6f72 6974 686d 2028 7374 7229 3a20 5370  orithm (str): Sp
+00004c60: 6563 6966 7920 7768 6963 6820 616c 676f  ecify which algo
+00004c70: 7269 7468 6d20 746f 2075 7365 2e20 204f  rithm to use.  O
+00004c80: 7074 696f 6e73 2061 7265 2027 6261 7369  ptions are 'basi
+00004c90: 6327 2028 7468 6520 6465 6661 756c 7429  c' (the default)
+00004ca0: 2061 6e64 2027 666c 6f79 645f 7761 7273   and 'floyd_wars
+00004cb0: 6861 6c6c 272e 0a0a 2020 2020 5265 7475  hall'...    Retu
+00004cc0: 726e 733a 200a 2020 2020 2020 2020 4120  rns: .        A 
+00004cd0: 736f 7274 6564 206c 6973 7420 6f66 2063  sorted list of c
+00004ce0: 616e 6469 6461 7465 732e 200a 0a20 2020  andidates. ..   
+00004cf0: 202e 2e20 7365 6561 6c73 6f3a 3a0a 0a20   .. seealso::.. 
+00004d00: 2020 2020 2020 203a 6d65 7468 3a60 7072         :meth:`pr
+00004d10: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
+00004d20: 5f62 6173 6564 5f6d 6574 686f 6473 2e73  _based_methods.s
+00004d30: 706c 6974 5f63 7963 6c65 5f64 6566 6561  plit_cycle_defea
+00004d40: 7460 0a0a 2020 2020 3a45 7861 6d70 6c65  t`..    :Example
+00004d50: 3a20 0a0a 2020 2020 2e2e 2070 6c6f 743a  : ..    .. plot:
+00004d60: 3a20 206d 6172 6769 6e5f 6772 6170 6873  :  margin_graphs
+00004d70: 5f65 7861 6d70 6c65 732f 6d67 5f65 785f  _examples/mg_ex_
+00004d80: 6270 5f72 702e 7079 0a20 2020 2020 2020  bp_rp.py.       
+00004d90: 203a 636f 6e74 6578 743a 2072 6573 6574   :context: reset
+00004da0: 2020 0a20 2020 2020 2020 203a 696e 636c    .        :incl
+00004db0: 7564 652d 736f 7572 6365 3a20 5472 7565  ude-source: True
+00004dc0: 0a0a 2020 2020 2e2e 2063 6f64 652d 626c  ..    .. code-bl
+00004dd0: 6f63 6b3a 3a20 0a0a 2020 2020 2020 2020  ock:: ..        
+00004de0: 6672 6f6d 2070 7265 665f 766f 7469 6e67  from pref_voting
+00004df0: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
+00004e00: 7468 6f64 7320 696d 706f 7274 2073 706c  thods import spl
+00004e10: 6974 5f63 7963 6c65 0a0a 2020 2020 2020  it_cycle..      
+00004e20: 2020 7370 6c69 745f 6379 636c 652e 6469    split_cycle.di
+00004e30: 7370 6c61 7928 6d67 290a 0a0a 2020 2020  splay(mg)...    
+00004e40: 2e2e 2065 7865 635f 636f 6465 3a3a 200a  .. exec_code:: .
+00004e50: 2020 2020 2020 2020 3a68 6964 655f 636f          :hide_co
+00004e60: 6465 3a0a 0a20 2020 2020 2020 2066 726f  de:..        fro
+00004e70: 6d20 7072 6566 5f76 6f74 696e 672e 7765  m pref_voting.we
+00004e80: 6967 6874 6564 5f6d 616a 6f72 6974 795f  ighted_majority_
+00004e90: 6772 6170 6873 2069 6d70 6f72 7420 4d61  graphs import Ma
+00004ea0: 7267 696e 4772 6170 680a 2020 2020 2020  rginGraph.      
+00004eb0: 2020 6672 6f6d 2070 7265 665f 766f 7469    from pref_voti
+00004ec0: 6e67 2e6d 6172 6769 6e5f 6261 7365 645f  ng.margin_based_
+00004ed0: 6d65 7468 6f64 7320 696d 706f 7274 2073  methods import s
+00004ee0: 706c 6974 5f63 7963 6c65 0a20 2020 2020  plit_cycle.     
+00004ef0: 2020 200a 2020 2020 2020 2020 6d67 203d     .        mg =
+00004f00: 204d 6172 6769 6e47 7261 7068 285b 302c   MarginGraph([0,
+00004f10: 2031 2c20 322c 2033 5d2c 205b 2830 2c20   1, 2, 3], [(0, 
+00004f20: 322c 2033 292c 2028 312c 2030 2c20 3529  2, 3), (1, 0, 5)
+00004f30: 2c20 2832 2c20 312c 2035 292c 2028 322c  , (2, 1, 5), (2,
+00004f40: 2033 2c20 3129 2c20 2833 2c20 302c 2033   3, 1), (3, 0, 3
+00004f50: 292c 2028 332c 2031 2c20 3129 5d29 0a20  ), (3, 1, 1)]). 
+00004f60: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00004f70: 7370 6c69 745f 6379 636c 652e 6469 7370  split_cycle.disp
+00004f80: 6c61 7928 6d67 290a 2020 2020 2020 2020  lay(mg).        
+00004f90: 7370 6c69 745f 6379 636c 652e 6469 7370  split_cycle.disp
+00004fa0: 6c61 7928 6d67 2c20 616c 676f 7269 7468  lay(mg, algorith
+00004fb0: 6d3d 2762 6173 6963 2729 0a20 2020 2020  m='basic').     
+00004fc0: 2020 2073 706c 6974 5f63 7963 6c65 2e64     split_cycle.d
+00004fd0: 6973 706c 6179 286d 672c 2061 6c67 6f72  isplay(mg, algor
+00004fe0: 6974 686d 3d27 666c 6f79 645f 7761 7273  ithm='floyd_wars
+00004ff0: 6861 6c6c 2729 0a20 2020 2022 2222 0a20  hall').    """. 
+00005000: 2020 200a 2020 2020 6966 2061 6c67 6f72     .    if algor
+00005010: 6974 686d 203d 3d20 2762 6173 6963 273a  ithm == 'basic':
+00005020: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00005030: 5f73 706c 6974 5f63 7963 6c65 5f62 6173  _split_cycle_bas
+00005040: 6963 2865 6461 7461 2c20 6375 7272 5f63  ic(edata, curr_c
+00005050: 616e 6473 203d 2063 7572 725f 6361 6e64  ands = curr_cand
+00005060: 732c 2073 7472 656e 6774 685f 6675 6e63  s, strength_func
+00005070: 7469 6f6e 203d 2073 7472 656e 6774 685f  tion = strength_
+00005080: 6675 6e63 7469 6f6e 290a 2020 2020 656c  function).    el
+00005090: 6966 2061 6c67 6f72 6974 686d 203d 3d20  if algorithm == 
+000050a0: 2766 6c6f 7964 5f77 6172 7368 616c 6c27  'floyd_warshall'
+000050b0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+000050c0: 205f 7370 6c69 745f 6379 636c 655f 666c   _split_cycle_fl
+000050d0: 6f79 645f 7761 7273 6861 6c6c 2865 6461  oyd_warshall(eda
+000050e0: 7461 2c20 6375 7272 5f63 616e 6473 203d  ta, curr_cands =
+000050f0: 2063 7572 725f 6361 6e64 732c 2073 7472   curr_cands, str
+00005100: 656e 6774 685f 6675 6e63 7469 6f6e 203d  ength_function =
+00005110: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+00005120: 6f6e 290a 2020 2020 656c 7365 3a0a 2020  on).    else:.  
+00005130: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00005140: 6545 7272 6f72 2822 496e 7661 6c69 6420  eError("Invalid 
+00005150: 616c 676f 7269 7468 6d20 7370 6563 6966  algorithm specif
+00005160: 6965 642e 2229 0a0a 0a64 6566 2073 706c  ied.")...def spl
+00005170: 6974 5f63 7963 6c65 5f64 6566 6561 7428  it_cycle_defeat(
+00005180: 6564 6174 612c 2063 7572 725f 6361 6e64  edata, curr_cand
+00005190: 7320 3d20 4e6f 6e65 2c20 7374 7265 6e67  s = None, streng
+000051a0: 7468 5f66 756e 6374 696f 6e20 3d20 4e6f  th_function = No
+000051b0: 6e65 293a 2020 200a 2020 2020 2222 220a  ne):   .    """.
+000051c0: 2020 2020 5265 7475 726e 7320 7468 6520      Returns the 
+000051d0: 5370 6c69 7420 4379 636c 6520 6465 6665  Split Cycle defe
+000051e0: 6174 2072 656c 6174 696f 6e2e 200a 0a20  at relation. .. 
+000051f0: 2020 2053 6565 2068 7474 7073 3a2f 2f61     See https://a
+00005200: 7278 6976 2e6f 7267 2f61 6273 2f32 3030  rxiv.org/abs/200
+00005210: 382e 3038 3435 3120 666f 7220 616e 2065  8.08451 for an e
+00005220: 7874 656e 6465 6420 6469 7363 7573 7369  xtended discussi
+00005230: 6f6e 206f 6620 7468 6973 206e 6f74 696f  on of this notio
+00005240: 6e20 6f66 2064 6566 6561 7420 696e 2061  n of defeat in a
+00005250: 6e20 656c 6563 7469 6f6e 2e20 0a0a 2020  n election. ..  
+00005260: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00005270: 6564 6174 6120 2850 726f 6669 6c65 2c20  edata (Profile, 
+00005280: 5072 6f66 696c 6557 6974 6854 6965 732c  ProfileWithTies,
+00005290: 204d 6172 6769 6e47 7261 7068 293a 2041   MarginGraph): A
+000052a0: 6e79 2065 6c65 6374 696f 6e20 6461 7461  ny election data
+000052b0: 2074 6861 7420 6861 7320 6120 606d 6172   that has a `mar
+000052c0: 6769 6e60 206d 6574 686f 642e 200a 2020  gin` method. .  
+000052d0: 2020 2020 2020 6375 7272 5f63 616e 6473        curr_cands
+000052e0: 2028 4c69 7374 5b69 6e74 5d2c 206f 7074   (List[int], opt
+000052f0: 696f 6e61 6c29 3a20 4966 2073 6574 2c20  ional): If set, 
+00005300: 7468 656e 2066 696e 6420 7468 6520 7769  then find the wi
+00005310: 6e6e 6572 7320 666f 7220 7468 6520 7072  nners for the pr
+00005320: 6f66 696c 6520 7265 7374 7269 6374 6564  ofile restricted
+00005330: 2074 6f20 7468 6520 6361 6e64 6964 6174   to the candidat
+00005340: 6573 2069 6e20 6060 6375 7272 5f63 616e  es in ``curr_can
+00005350: 6473 6060 0a0a 2020 2020 5265 7475 726e  ds``..    Return
+00005360: 733a 200a 2020 2020 2020 2020 4120 6e65  s: .        A ne
+00005370: 7477 6f72 6b78 2044 6947 7261 7068 2072  tworkx DiGraph r
+00005380: 6570 7265 7365 6e74 696e 6720 7468 6520  epresenting the 
+00005390: 5370 6c69 7420 4379 636c 6520 6465 6665  Split Cycle defe
+000053a0: 6174 2072 656c 6174 696f 6e2e 200a 0a20  at relation. .. 
+000053b0: 2020 202e 2e20 7365 6561 6c73 6f3a 3a0a     .. seealso::.
+000053c0: 0a20 2020 2020 2020 203a 6d65 7468 3a60  .        :meth:`
+000053d0: 7072 6566 5f76 6f74 696e 672e 6d61 7267  pref_voting.marg
+000053e0: 696e 5f62 6173 6564 5f6d 6574 686f 6473  in_based_methods
+000053f0: 2e73 706c 6974 5f63 7963 6c65 602c 203a  .split_cycle`, :
+00005400: 6d65 7468 3a60 7072 6566 5f76 6f74 696e  meth:`pref_votin
+00005410: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
+00005420: 6574 686f 6473 2e73 706c 6974 5f63 7963  ethods.split_cyc
+00005430: 6c65 5f46 6c6f 7964 5f57 6172 7368 616c  le_Floyd_Warshal
+00005440: 6c60 0a0a 2020 2020 3a45 7861 6d70 6c65  l`..    :Example
+00005450: 3a20 0a0a 2020 2020 2e2e 2070 6c6f 743a  : ..    .. plot:
+00005460: 3a20 206d 6172 6769 6e5f 6772 6170 6873  :  margin_graphs
+00005470: 5f65 7861 6d70 6c65 732f 6d67 5f65 785f  _examples/mg_ex_
+00005480: 7363 5f64 6566 6561 742e 7079 0a20 2020  sc_defeat.py.   
+00005490: 2020 2020 203a 636f 6e74 6578 743a 2072       :context: r
+000054a0: 6573 6574 2020 0a20 2020 2020 2020 203a  eset  .        :
+000054b0: 696e 636c 7564 652d 736f 7572 6365 3a20  include-source: 
+000054c0: 5472 7565 0a0a 2020 2020 2222 220a 0a20  True..    """.. 
+000054d0: 2020 2063 616e 6469 6461 7465 7320 3d20     candidates = 
+000054e0: 6564 6174 612e 6361 6e64 6964 6174 6573  edata.candidates
+000054f0: 2069 6620 6375 7272 5f63 616e 6473 2069   if curr_cands i
+00005500: 7320 4e6f 6e65 2065 6c73 6520 6375 7272  s None else curr
+00005510: 5f63 616e 6473 2020 2020 0a20 2020 2073  _cands    .    s
+00005520: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+00005530: 203d 2065 6461 7461 2e6d 6172 6769 6e20   = edata.margin 
+00005540: 6966 2073 7472 656e 6774 685f 6675 6e63  if strength_func
+00005550: 7469 6f6e 2069 7320 4e6f 6e65 2065 6c73  tion is None els
+00005560: 6520 7374 7265 6e67 7468 5f66 756e 6374  e strength_funct
+00005570: 696f 6e20 0a20 0a20 2020 2077 6561 6b5f  ion . .    weak_
+00005580: 636f 6e64 6f72 6365 745f 7769 6e6e 6572  condorcet_winner
+00005590: 7320 3d20 7b63 3a54 7275 6520 666f 7220  s = {c:True for 
+000055a0: 6320 696e 2063 616e 6469 6461 7465 737d  c in candidates}
+000055b0: 0a20 2020 2073 5f6d 6174 7269 7820 3d20  .    s_matrix = 
+000055c0: 5b5b 2d6e 702e 696e 6620 666f 7220 5f20  [[-np.inf for _ 
+000055d0: 696e 2063 616e 6469 6461 7465 735d 2066  in candidates] f
+000055e0: 6f72 205f 2069 6e20 6361 6e64 6964 6174  or _ in candidat
+000055f0: 6573 5d0a 2020 2020 0a20 2020 2023 2069  es].    .    # i
+00005600: 6e69 7469 616c 697a 6520 7468 6520 735f  nitialize the s_
+00005610: 6d61 7472 6978 0a20 2020 2066 6f72 2063  matrix.    for c
+00005620: 315f 6964 782c 2063 3120 696e 2065 6e75  1_idx, c1 in enu
+00005630: 6d65 7261 7465 2863 616e 6469 6461 7465  merate(candidate
+00005640: 7329 3a0a 2020 2020 2020 2020 666f 7220  s):.        for 
+00005650: 6332 5f69 6478 2c20 6332 2069 6e20 656e  c2_idx, c2 in en
+00005660: 756d 6572 6174 6528 6361 6e64 6964 6174  umerate(candidat
+00005670: 6573 293a 0a20 2020 2020 2020 2020 2020  es):.           
+00005680: 2069 6620 2865 6461 7461 2e6d 616a 6f72   if (edata.major
+00005690: 6974 795f 7072 6566 6572 7328 6331 2c20  ity_prefers(c1, 
+000056a0: 6332 2920 6f72 2063 3120 3d3d 2063 3229  c2) or c1 == c2)
+000056b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000056c0: 2020 735f 6d61 7472 6978 5b63 315f 6964    s_matrix[c1_id
+000056d0: 785d 5b63 325f 6964 785d 203d 2073 7472  x][c2_idx] = str
+000056e0: 656e 6774 685f 6675 6e63 7469 6f6e 2863  ength_function(c
+000056f0: 312c 2063 3229 200a 2020 2020 2020 2020  1, c2) .        
+00005700: 2020 2020 2020 2020 7765 616b 5f63 6f6e          weak_con
+00005710: 646f 7263 6574 5f77 696e 6e65 7273 5b63  dorcet_winners[c
+00005720: 325d 203d 2077 6561 6b5f 636f 6e64 6f72  2] = weak_condor
+00005730: 6365 745f 7769 6e6e 6572 735b 6332 5d20  cet_winners[c2] 
+00005740: 616e 6420 2863 3120 3d3d 2063 3229 2023  and (c1 == c2) #
+00005750: 2077 6561 6b20 436f 6e64 6f72 6365 7420   weak Condorcet 
+00005760: 7769 6e6e 6572 7320 6172 6520 5370 6c69  winners are Spli
+00005770: 7420 4379 636c 6520 7769 6e6e 6572 730a  t Cycle winners.
+00005780: 2020 2020 0a20 2020 2073 7472 656e 6774      .    strengt
+00005790: 6820 3d20 6c69 7374 286d 6170 286c 616d  h = list(map(lam
+000057a0: 6264 6120 6920 3a20 6c69 7374 286d 6170  bda i : list(map
+000057b0: 286c 616d 6264 6120 6a20 3a20 6a20 2c20  (lambda j : j , 
+000057c0: 6929 2920 2c20 735f 6d61 7472 6978 2929  i)) , s_matrix))
+000057d0: 0a20 2020 2066 6f72 2069 5f69 6478 2c20  .    for i_idx, 
+000057e0: 6920 696e 2065 6e75 6d65 7261 7465 2863  i in enumerate(c
+000057f0: 616e 6469 6461 7465 7329 3a20 0a20 2020  andidates): .   
+00005800: 2020 2020 2066 6f72 206a 5f69 6478 2c20       for j_idx, 
+00005810: 6a20 696e 2065 6e75 6d65 7261 7465 2863  j in enumerate(c
+00005820: 616e 6469 6461 7465 7329 3a0a 2020 2020  andidates):.    
+00005830: 2020 2020 2020 2020 6966 2069 213d 206a          if i!= j
+00005840: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00005850: 2020 6966 206e 6f74 2077 6561 6b5f 636f    if not weak_co
+00005860: 6e64 6f72 6365 745f 7769 6e6e 6572 735b  ndorcet_winners[
+00005870: 6a5d 3a20 2320 7765 616b 2043 6f6e 646f  j]: # weak Condo
+00005880: 7263 6574 2077 696e 6e65 7273 2061 7265  rcet winners are
+00005890: 2053 706c 6974 2043 7963 6c65 2077 696e   Split Cycle win
+000058a0: 6e65 7273 0a20 2020 2020 2020 2020 2020  ners.           
+000058b0: 2020 2020 2020 2020 2066 6f72 206b 5f69           for k_i
+000058c0: 6478 2c20 6b20 696e 2065 6e75 6d65 7261  dx, k in enumera
+000058d0: 7465 2863 616e 6469 6461 7465 7329 3a20  te(candidates): 
+000058e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000058f0: 2020 2020 2020 2020 2069 6620 6920 213d           if i !=
+00005900: 206b 2061 6e64 206a 2021 3d20 6b3a 0a20   k and j != k:. 
+00005910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005920: 2020 2020 2020 2020 2020 2073 7472 656e             stren
+00005930: 6774 685b 6a5f 6964 785d 5b6b 5f69 6478  gth[j_idx][k_idx
+00005940: 5d20 3d20 6d61 7828 7374 7265 6e67 7468  ] = max(strength
+00005950: 5b6a 5f69 6478 5d5b 6b5f 6964 785d 2c20  [j_idx][k_idx], 
+00005960: 6d69 6e28 7374 7265 6e67 7468 5b6a 5f69  min(strength[j_i
+00005970: 6478 5d5b 695f 6964 785d 2c73 7472 656e  dx][i_idx],stren
+00005980: 6774 685b 695f 6964 785d 5b6b 5f69 6478  gth[i_idx][k_idx
+00005990: 5d29 290a 200a 2020 2020 6465 6665 6174  ])). .    defeat
+000059a0: 5f67 7261 7068 203d 206e 782e 4469 4772  _graph = nx.DiGr
+000059b0: 6170 6828 290a 2020 2020 6465 6665 6174  aph().    defeat
+000059c0: 5f67 7261 7068 2e61 6464 5f6e 6f64 6573  _graph.add_nodes
+000059d0: 5f66 726f 6d28 6361 6e64 6964 6174 6573  _from(candidates
+000059e0: 290a 0a20 2020 2066 6f72 2069 5f69 6478  )..    for i_idx
+000059f0: 2c20 6920 696e 2065 6e75 6d65 7261 7465  , i in enumerate
+00005a00: 2863 616e 6469 6461 7465 7329 3a0a 2020  (candidates):.  
+00005a10: 2020 2020 2020 666f 7220 6a5f 6964 782c        for j_idx,
+00005a20: 206a 2069 6e20 656e 756d 6572 6174 6528   j in enumerate(
+00005a30: 6361 6e64 6964 6174 6573 293a 0a20 2020  candidates):.   
+00005a40: 2020 2020 2020 2020 2069 6620 6920 213d           if i !=
+00005a50: 206a 3a0a 2020 2020 2020 2020 2020 2020   j:.            
+00005a60: 2020 2020 6966 2073 5f6d 6174 7269 785b      if s_matrix[
+00005a70: 6a5f 6964 785d 5b69 5f69 6478 5d20 3e20  j_idx][i_idx] > 
+00005a80: 7374 7265 6e67 7468 5b69 5f69 6478 5d5b  strength[i_idx][
+00005a90: 6a5f 6964 785d 3a20 2320 7468 6520 6d61  j_idx]: # the ma
+00005aa0: 696e 2064 6966 6665 7265 6e63 6520 7769  in difference wi
+00005ab0: 7468 2042 6561 7420 5061 7468 0a20 2020  th Beat Path.   
+00005ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ad0: 2064 6566 6561 745f 6772 6170 682e 6164   defeat_graph.ad
+00005ae0: 645f 7765 6967 6874 6564 5f65 6467 6573  d_weighted_edges
+00005af0: 5f66 726f 6d28 5b28 6a2c 692c 735f 6d61  _from([(j,i,s_ma
+00005b00: 7472 6978 5b6a 5f69 6478 5d5b 695f 6964  trix[j_idx][i_id
+00005b10: 785d 295d 290a 2020 2020 2020 2020 2020  x])]).          
+00005b20: 2020 2020 2020 0a20 2020 2072 6574 7572        .    retur
+00005b30: 6e20 6465 6665 6174 5f67 7261 7068 0a0a  n defeat_graph..
+00005b40: 0a23 2066 6c61 7474 656e 2061 2032 6420  .# flatten a 2d 
+00005b50: 6c69 7374 202d 2074 7572 6e20 6120 3264  list - turn a 2d
+00005b60: 206c 6973 7420 696e 746f 2061 2073 696e   list into a sin
+00005b70: 676c 6520 6c69 7374 206f 6620 6974 656d  gle list of item
+00005b80: 730a 666c 6174 7465 6e20 3d20 6c61 6d62  s.flatten = lamb
+00005b90: 6461 206c 3a20 5b69 7465 6d20 666f 7220  da l: [item for 
+00005ba0: 7375 626c 6973 7420 696e 206c 2066 6f72  sublist in l for
+00005bb0: 2069 7465 6d20 696e 2073 7562 6c69 7374   item in sublist
+00005bc0: 5d0a 0a64 6566 2064 6f65 735f 6372 6561  ]..def does_crea
+00005bd0: 7465 5f63 7963 6c65 2867 2c20 6564 6765  te_cycle(g, edge
+00005be0: 293a 0a20 2020 2027 2727 7265 7475 726e  ):.    '''return
+00005bf0: 2054 7275 6520 6966 2061 6464 696e 6720   True if adding 
+00005c00: 7468 6520 6564 6765 2074 6f20 6720 6372  the edge to g cr
+00005c10: 6561 7465 2061 2063 7963 6c65 2e0a 2020  eate a cycle..  
+00005c20: 2020 6974 2069 7320 6173 7375 6d65 6420    it is assumed 
+00005c30: 7468 6174 2065 6467 6520 6973 2061 6c72  that edge is alr
+00005c40: 6561 6479 2069 6e20 6727 2727 0a20 2020  eady in g'''.   
+00005c50: 2073 6f75 7263 6520 3d20 6564 6765 5b30   source = edge[0
+00005c60: 5d0a 2020 2020 7461 7267 6574 203d 2065  ].    target = e
+00005c70: 6467 655b 315d 0a20 2020 2066 6f72 206e  dge[1].    for n
+00005c80: 2069 6e20 672e 7072 6564 6563 6573 736f   in g.predecesso
+00005c90: 7273 2873 6f75 7263 6529 3a0a 2020 2020  rs(source):.    
+00005ca0: 2020 2020 6966 206e 782e 6861 735f 7061      if nx.has_pa
+00005cb0: 7468 2867 2c20 7461 7267 6574 2c20 6e29  th(g, target, n)
+00005cc0: 3a20 0a20 2020 2020 2020 2020 2020 2072  : .            r
+00005cd0: 6574 7572 6e20 5472 7565 0a20 2020 2072  eturn True.    r
+00005ce0: 6574 7572 6e20 4661 6c73 650a 0a0a 0a64  eturn False....d
+00005cf0: 6566 2070 6f77 6572 7365 7428 6974 6572  ef powerset(iter
+00005d00: 6162 6c65 293a 0a20 2020 2022 2222 0a20  able):.    """. 
+00005d10: 2020 2052 6574 7572 6e20 7468 6520 706f     Return the po
+00005d20: 7765 7273 6574 206f 6620 6060 6974 6572  werset of ``iter
+00005d30: 6162 6c65 6060 0a0a 2020 2020 706f 7765  able``..    powe
+00005d40: 7273 6574 285b 312c 322c 335d 2920 2d2d  rset([1,2,3]) --
+00005d50: 3e20 2829 2028 312c 2920 2832 2c29 2028  > () (1,) (2,) (
+00005d60: 332c 2920 2831 2c32 2920 2831 2c33 2920  3,) (1,2) (1,3) 
+00005d70: 2832 2c33 2920 2831 2c32 2c33 290a 2020  (2,3) (1,2,3).  
+00005d80: 2020 2222 220a 2020 2020 7320 3d20 6c69    """.    s = li
+00005d90: 7374 2869 7465 7261 626c 6529 0a20 2020  st(iterable).   
+00005da0: 2072 6574 7572 6e20 6368 6169 6e2e 6672   return chain.fr
+00005db0: 6f6d 5f69 7465 7261 626c 6528 636f 6d62  om_iterable(comb
+00005dc0: 696e 6174 696f 6e73 2873 2c20 7229 2066  inations(s, r) f
+00005dd0: 6f72 2072 2069 6e20 7261 6e67 6528 6c65  or r in range(le
+00005de0: 6e28 7329 2b31 2929 0a0a 0a64 6566 2069  n(s)+1))...def i
+00005df0: 735f 7374 6163 6b28 6564 6174 612c 2063  s_stack(edata, c
+00005e00: 616e 645f 6c69 7374 2c20 6375 7272 5f63  and_list, curr_c
+00005e10: 616e 6473 3d4e 6f6e 6529 3a20 0a20 2020  ands=None): .   
+00005e20: 2022 2222 0a20 2020 2041 202a 2a73 7461   """.    A **sta
+00005e30: 636b 2a2a 2069 7320 6120 6c69 6e65 6172  ck** is a linear
+00005e40: 206f 7264 6572 203a 6d61 7468 3a60 4c60   order :math:`L`
+00005e50: 206f 6e20 7468 6520 6361 6e64 6964 6174   on the candidat
+00005e60: 6520 7375 6368 2074 6861 7420 666f 7220  e such that for 
+00005e70: 616c 6c20 6361 6e64 6964 6174 6573 203a  all candidates :
+00005e80: 6d61 7468 3a60 6160 2061 6e64 203a 6d61  math:`a` and :ma
+00005e90: 7468 3a60 6260 2c20 6966 203a 6d61 7468  th:`b`, if :math
+00005ea0: 3a60 614c 6260 2c20 7468 656e 2074 6865  :`aLb`, then the
+00005eb0: 7265 2061 7265 2064 6973 7469 6e63 7420  re are distinct 
+00005ec0: 6361 6e64 6964 6174 6573 203a 6d61 7468  candidates :math
+00005ed0: 3a60 785f 312c 5c64 6f74 732c 785f 6e60  :`x_1,\dots,x_n`
+00005ee0: 2077 6974 6820 3a6d 6174 683a 6078 5f31   with :math:`x_1
+00005ef0: 3d61 6020 616e 6420 3a6d 6174 683a 6078  =a` and :math:`x
+00005f00: 5f6e 3d62 6020 7375 6368 2074 6861 7420  _n=b` such that 
+00005f10: 3a6d 6174 683a 6078 5f69 204c 2078 5f7b  :math:`x_i L x_{
+00005f20: 692b 317d 6020 616e 6420 666f 7220 616c  i+1}` and for al
+00005f30: 6c20 3a6d 6174 683a 6069 5c69 6e20 5c7b  l :math:`i\in \{
+00005f40: 312c 5c64 6f74 732c 206e 2d31 5c7d 602c  1,\dots, n-1\}`,
+00005f50: 2074 6865 206d 6172 6769 6e20 6f66 203a   the margin of :
+00005f60: 6d61 7468 3a60 785f 3160 206f 7665 7220  math:`x_1` over 
+00005f70: 3a6d 6174 683a 6078 5f7b 692b 317d 6020  :math:`x_{i+1}` 
+00005f80: 6973 2067 7265 6174 6572 2074 6861 6e20  is greater than 
+00005f90: 6f72 2065 7175 616c 2074 6f20 7468 6520  or equal to the 
+00005fa0: 6d61 7267 696e 206f 6620 3a6d 6174 683a  margin of :math:
+00005fb0: 6062 6020 6f76 6572 203a 6d61 7468 3a60  `b` over :math:`
+00005fc0: 6160 2e0a 0a20 2020 2054 6869 7320 6465  a`...    This de
+00005fd0: 6669 6e69 7469 6f6e 2069 7320 6475 6520  finition is due 
+00005fe0: 746f 205a 6176 6973 7420 616e 6420 5469  to Zavist and Ti
+00005ff0: 6465 6d61 6e20 3139 3839 2c20 616e 6420  deman 1989, and 
+00006000: 6973 2075 7365 6420 6173 2061 6e20 616c  is used as an al
+00006010: 7465 726e 6174 6976 6520 6368 6172 6163  ternative charac
+00006020: 7465 7269 7a61 7469 6f6e 206f 6620 5261  terization of Ra
+00006030: 6e6b 6564 2050 6169 7273 3a20 3a6d 6174  nked Pairs: :mat
+00006040: 683a 6061 6020 6973 2061 2052 616e 6b65  h:`a` is a Ranke
+00006050: 6420 5061 6972 7320 7769 6e6e 6572 2069  d Pairs winner i
+00006060: 6620 616e 6420 6f6e 6c79 2069 6620 3a6d  f and only if :m
+00006070: 6174 683a 6061 6020 6973 2074 6865 206d  ath:`a` is the m
+00006080: 6178 696d 756d 2065 6c65 6d65 6e74 206f  aximum element o
+00006090: 6620 736f 6d65 2073 7461 636b 2e20 0a0a  f some stack. ..
+000060a0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+000060b0: 2020 6564 6174 6120 2850 726f 6669 6c65    edata (Profile
+000060c0: 2c20 5072 6f66 696c 6557 6974 6854 6965  , ProfileWithTie
+000060d0: 732c 204d 6172 6769 6e47 7261 7068 293a  s, MarginGraph):
+000060e0: 2041 6e79 2065 6c65 6374 696f 6e20 6461   Any election da
+000060f0: 7461 2074 6861 7420 6861 7320 6120 606d  ta that has a `m
+00006100: 6172 6769 6e60 206d 6574 686f 642e 200a  argin` method. .
+00006110: 2020 2020 2020 2020 6361 6e64 5f6c 6973          cand_lis
+00006120: 7420 286c 6973 7429 3a20 5468 6520 6c69  t (list): The li
+00006130: 7374 206f 6620 6361 6e64 6964 6174 6573  st of candidates
+00006140: 2074 6861 7420 6d61 7920 6265 2061 2073   that may be a s
+00006150: 7461 636b 0a20 2020 2020 2020 2063 7572  tack.        cur
+00006160: 725f 6361 6e64 7320 284c 6973 745b 696e  r_cands (List[in
+00006170: 745d 2c20 6f70 7469 6f6e 616c 293a 2049  t], optional): I
+00006180: 6620 7365 742c 2074 6865 6e20 6669 6e64  f set, then find
+00006190: 2074 6865 2077 696e 6e65 7273 2066 6f72   the winners for
+000061a0: 2074 6865 2070 726f 6669 6c65 2072 6573   the profile res
+000061b0: 7472 6963 7465 6420 746f 2074 6865 2063  tricted to the c
+000061c0: 616e 6469 6461 7465 7320 696e 2060 6063  andidates in ``c
+000061d0: 7572 725f 6361 6e64 7360 600a 0a20 2020  urr_cands``..   
+000061e0: 2052 6574 7572 6e73 3a20 0a20 2020 2020   Returns: .     
+000061f0: 2020 2054 7275 6520 6966 2060 6063 616e     True if ``can
+00006200: 645f 6c69 7374 6060 2069 7320 6120 7374  d_list`` is a st
+00006210: 6163 6b20 616e 6420 4661 6c73 6520 6f74  ack and False ot
+00006220: 6865 7277 6973 650a 0a20 2020 203a 4578  herwise..    :Ex
+00006230: 616d 706c 653a 200a 2020 2020 0a20 2020  ample: .    .   
+00006240: 202e 2e20 706c 6f74 3a3a 2020 6d61 7267   .. plot::  marg
+00006250: 696e 5f67 7261 7068 735f 6578 616d 706c  in_graphs_exampl
+00006260: 6573 2f6d 675f 6578 5f72 705f 7374 6163  es/mg_ex_rp_stac
+00006270: 6b73 2e70 790a 2020 2020 2020 2020 3a63  ks.py.        :c
+00006280: 6f6e 7465 7874 3a20 7265 7365 7420 200a  ontext: reset  .
+00006290: 2020 2020 2020 2020 3a69 6e63 6c75 6465          :include
+000062a0: 2d73 6f75 7263 653a 2054 7275 650a 0a0a  -source: True...
+000062b0: 2020 2020 2e2e 2065 7865 635f 636f 6465      .. exec_code
+000062c0: 3a3a 0a20 2020 2020 2020 200a 2020 2020  ::.        .    
+000062d0: 2020 2020 6672 6f6d 2070 7265 665f 766f      from pref_vo
+000062e0: 7469 6e67 2e77 6569 6768 7465 645f 6d61  ting.weighted_ma
+000062f0: 6a6f 7269 7479 5f67 7261 7068 7320 696d  jority_graphs im
+00006300: 706f 7274 204d 6172 6769 6e47 7261 7068  port MarginGraph
+00006310: 0a20 2020 2020 2020 2066 726f 6d20 7072  .        from pr
+00006320: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
+00006330: 5f62 6173 6564 5f6d 6574 686f 6473 2069  _based_methods i
+00006340: 6d70 6f72 7420 6973 5f73 7461 636b 0a20  mport is_stack. 
+00006350: 2020 2020 2020 2066 726f 6d20 6974 6572         from iter
+00006360: 746f 6f6c 7320 696d 706f 7274 2070 6572  tools import per
+00006370: 6d75 7461 7469 6f6e 730a 2020 2020 2020  mutations.      
+00006380: 2020 0a20 2020 2020 2020 206d 6720 3d20    .        mg = 
+00006390: 4d61 7267 696e 4772 6170 6828 5b30 2c20  MarginGraph([0, 
+000063a0: 312c 2032 5d2c 205b 2830 2c20 312c 2032  1, 2], [(0, 1, 2
+000063b0: 292c 2028 312c 2032 2c20 3429 2c20 2832  ), (1, 2, 4), (2
+000063c0: 2c20 302c 2032 295d 290a 2020 2020 2020  , 0, 2)]).      
+000063d0: 2020 0a20 2020 2020 2020 2066 6f72 2063    .        for c
+000063e0: 6c69 7374 2069 6e20 7065 726d 7574 6174  list in permutat
+000063f0: 696f 6e73 286d 672e 6361 6e64 6964 6174  ions(mg.candidat
+00006400: 6573 293a 200a 2020 2020 2020 2020 2020  es): .          
+00006410: 2020 7072 696e 7428 6622 7b63 6c69 7374    print(f"{clist
+00006420: 7d20 7b27 6973 2720 6966 2069 735f 7374  } {'is' if is_st
+00006430: 6163 6b28 6d67 2c20 636c 6973 7429 2065  ack(mg, clist) e
+00006440: 6c73 6520 2769 7320 6e6f 7427 7d20 6120  lse 'is not'} a 
+00006450: 7374 6163 6b22 290a 2020 2020 2020 2020  stack").        
+00006460: 2020 2020 0a20 2020 2022 2222 0a20 2020      .    """.   
+00006470: 200a 2020 2020 6361 6e64 6964 6174 6573   .    candidates
+00006480: 203d 2063 7572 725f 6361 6e64 7320 6966   = curr_cands if
+00006490: 2063 7572 725f 6361 6e64 7320 6973 206e   curr_cands is n
+000064a0: 6f74 204e 6f6e 6520 656c 7365 2065 6461  ot None else eda
+000064b0: 7461 2e63 616e 6469 6461 7465 730a 2020  ta.candidates.  
+000064c0: 2020 6361 6e64 5f70 6169 7273 203d 205b    cand_pairs = [
+000064d0: 2861 2c20 6229 2069 6620 6361 6e64 5f6c  (a, b) if cand_l
+000064e0: 6973 742e 696e 6465 7828 6129 203c 2063  ist.index(a) < c
+000064f0: 616e 645f 6c69 7374 2e69 6e64 6578 2862  and_list.index(b
+00006500: 2920 656c 7365 2028 622c 2061 2920 666f  ) else (b, a) fo
+00006510: 7220 612c 2062 2069 6e20 636f 6d62 696e  r a, b in combin
+00006520: 6174 696f 6e73 2863 616e 6469 6461 7465  ations(candidate
+00006530: 732c 2032 295d 0a20 2020 2020 2020 200a  s, 2)].        .
+00006540: 2020 2020 666f 7220 612c 2062 2069 6e20      for a, b in 
+00006550: 6361 6e64 5f70 6169 7273 3a0a 2020 2020  cand_pairs:.    
+00006560: 2020 2020 6f74 6865 725f 6361 6e64 7320      other_cands 
+00006570: 3d20 5b63 2066 6f72 2063 2069 6e20 6361  = [c for c in ca
+00006580: 6e64 6964 6174 6573 2069 6620 6320 213d  ndidates if c !=
+00006590: 2061 2061 6e64 2063 2021 3d20 625d 0a20   a and c != b]. 
+000065a0: 2020 2020 2020 2066 6f75 6e64 5f70 6174         found_pat
+000065b0: 6820 3d20 4661 6c73 650a 2020 2020 2020  h = False.      
+000065c0: 2020 0a20 2020 2020 2020 2073 7562 6c69    .        subli
+000065d0: 7374 203d 2063 616e 645f 6c69 7374 5b63  st = cand_list[c
+000065e0: 616e 645f 6c69 7374 2e69 6e64 6578 2861  and_list.index(a
+000065f0: 2920 2b20 313a 6361 6e64 5f6c 6973 742e  ) + 1:cand_list.
+00006600: 696e 6465 7828 6229 5d0a 2020 2020 2020  index(b)].      
+00006610: 2020 0a20 2020 2020 2020 2066 6f72 2069    .        for i
+00006620: 6e64 6963 6573 2069 6e20 706f 7765 7273  ndices in powers
+00006630: 6574 2872 616e 6765 286c 656e 2873 7562  et(range(len(sub
+00006640: 6c69 7374 2929 293a 200a 2020 2020 2020  list))): .      
+00006650: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
+00006660: 2020 2070 6174 6820 3d20 5b61 5d20 2b20     path = [a] + 
+00006670: 5b73 7562 6c69 7374 5b69 5d20 666f 7220  [sublist[i] for 
+00006680: 6920 696e 2073 6f72 7465 6428 696e 6469  i in sorted(indi
+00006690: 6365 7329 5d20 2b20 5b62 5d0a 2020 2020  ces)] + [b].    
+000066a0: 2020 2020 2020 2020 6d61 7267 696e 7320          margins 
+000066b0: 3d20 5b65 6461 7461 2e6d 6172 6769 6e28  = [edata.margin(
+000066c0: 7869 2c20 7061 7468 5b69 202b 2031 5d29  xi, path[i + 1])
+000066d0: 2066 6f72 2069 2c20 7869 2069 6e20 656e   for i, xi in en
+000066e0: 756d 6572 6174 6528 7061 7468 5b30 3a2d  umerate(path[0:-
+000066f0: 315d 295d 0a20 2020 2020 2020 2020 2020  1])].           
+00006700: 2069 6620 616c 6c28 5b63 616e 645f 6c69   if all([cand_li
+00006710: 7374 2e69 6e64 6578 2878 6929 203c 2063  st.index(xi) < c
+00006720: 616e 645f 6c69 7374 2e69 6e64 6578 2870  and_list.index(p
+00006730: 6174 685b 692b 315d 2920 666f 7220 692c  ath[i+1]) for i,
+00006740: 2078 6920 696e 2065 6e75 6d65 7261 7465   xi in enumerate
+00006750: 2870 6174 685b 303a 2d31 5d29 5d29 2061  (path[0:-1])]) a
+00006760: 6e64 2061 6c6c 285b 6d20 3e3d 2065 6461  nd all([m >= eda
+00006770: 7461 2e6d 6172 6769 6e28 622c 2061 2920  ta.margin(b, a) 
+00006780: 666f 7220 6d20 696e 206d 6172 6769 6e73  for m in margins
+00006790: 5d29 3a20 0a20 2020 2020 2020 2020 2020  ]): .           
+000067a0: 2020 2020 2066 6f75 6e64 5f70 6174 6820       found_path 
+000067b0: 3d20 5472 7565 0a20 2020 2020 2020 2020  = True.         
+000067c0: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
+000067d0: 2020 2020 2069 6620 6e6f 7420 666f 756e       if not foun
+000067e0: 645f 7061 7468 3a20 0a20 2020 2020 2020  d_path: .       
+000067f0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00006800: 650a 2020 2020 7265 7475 726e 2054 7275  e.    return Tru
+00006810: 650a 0a64 6566 205f 7261 6e6b 6564 5f70  e..def _ranked_p
+00006820: 6169 7273 5f66 726f 6d5f 7374 6163 6b73  airs_from_stacks
+00006830: 2865 6461 7461 2c20 6375 7272 5f63 616e  (edata, curr_can
+00006840: 6473 203d 204e 6f6e 6529 3a20 0a20 2020  ds = None): .   
+00006850: 2022 2222 4669 6e64 2074 6865 2052 616e   """Find the Ran
+00006860: 6b65 6420 5061 6972 7320 7769 6e6e 6572  ked Pairs winner
+00006870: 7320 6279 2069 7465 7261 7469 6e67 206f  s by iterating o
+00006880: 7665 7220 616c 6c20 7065 726d 7574 6174  ver all permutat
+00006890: 696f 6e73 206f 6620 6361 6e64 6964 6174  ions of candidat
+000068a0: 6573 2028 7265 7374 7269 6374 6564 2074  es (restricted t
+000068b0: 6f20 6060 6375 7272 5f63 616e 6473 6060  o ``curr_cands``
+000068c0: 2069 6620 6e6f 7420 4e6f 6e65 292c 2061   if not None), a
+000068d0: 6e64 2063 6865 636b 696e 6720 6966 2074  nd checking if t
+000068e0: 6865 206c 6973 7420 6973 2061 2073 7461  he list is a sta
+000068f0: 636b 2e20 0a0a 2020 2020 4172 6773 3a0a  ck. ..    Args:.
+00006900: 2020 2020 2020 2020 6564 6174 6120 2850          edata (P
+00006910: 726f 6669 6c65 2c20 5072 6f66 696c 6557  rofile, ProfileW
+00006920: 6974 6854 6965 732c 204d 6172 6769 6e47  ithTies, MarginG
+00006930: 7261 7068 293a 2041 6e79 2065 6c65 6374  raph): Any elect
+00006940: 696f 6e20 6461 7461 2074 6861 7420 6861  ion data that ha
+00006950: 7320 6120 606d 6172 6769 6e60 206d 6574  s a `margin` met
+00006960: 686f 642e 200a 2020 2020 2020 2020 6375  hod. .        cu
+00006970: 7272 5f63 616e 6473 2028 4c69 7374 5b69  rr_cands (List[i
+00006980: 6e74 5d2c 206f 7074 696f 6e61 6c29 3a20  nt], optional): 
+00006990: 4966 2073 6574 2c20 7468 656e 2066 696e  If set, then fin
+000069a0: 6420 7468 6520 7769 6e6e 6572 7320 666f  d the winners fo
+000069b0: 7220 7468 6520 7072 6f66 696c 6520 7265  r the profile re
+000069c0: 7374 7269 6374 6564 2074 6f20 7468 6520  stricted to the 
+000069d0: 6361 6e64 6964 6174 6573 2069 6e20 6060  candidates in ``
+000069e0: 6375 7272 5f63 616e 6473 6060 0a0a 2020  curr_cands``..  
+000069f0: 2020 5265 7475 726e 733a 200a 2020 2020    Returns: .    
+00006a00: 2020 2020 4120 736f 7274 6564 206c 6973      A sorted lis
+00006a10: 7420 6f66 2063 616e 6469 6461 7465 732e  t of candidates.
+00006a20: 200a 0a20 2020 202e 2e20 7365 6561 6c73   ..    .. seeals
+00006a30: 6f3a 3a0a 2020 2020 2020 2020 0a20 2020  o::.        .   
+00006a40: 2020 2020 203a 6d65 7468 3a60 7072 6566       :meth:`pref
+00006a50: 5f76 6f74 696e 672e 6d61 7267 696e 5f62  _voting.margin_b
+00006a60: 6173 6564 5f6d 6574 686f 6473 2e69 735f  ased_methods.is_
+00006a70: 7374 6163 6b60 0a0a 0a20 2020 2022 2222  stack`...    """
+00006a80: 2020 2020 0a0a 2020 2020 6361 6e64 6964      ..    candid
+00006a90: 6174 6573 203d 2063 7572 725f 6361 6e64  ates = curr_cand
+00006aa0: 7320 6966 2063 7572 725f 6361 6e64 7320  s if curr_cands 
+00006ab0: 6973 206e 6f74 204e 6f6e 6520 656c 7365  is not None else
+00006ac0: 2065 6461 7461 2e63 616e 6469 6461 7465   edata.candidate
+00006ad0: 730a 2020 2020 7769 6e6e 6572 7320 3d20  s.    winners = 
+00006ae0: 6c69 7374 2829 0a20 2020 2066 6f72 2063  list().    for c
+00006af0: 6c69 7374 2069 6e20 7065 726d 7574 6174  list in permutat
+00006b00: 696f 6e73 2863 616e 6469 6461 7465 7329  ions(candidates)
+00006b10: 3a20 0a20 2020 2020 2020 2069 7373 7461  : .        issta
+00006b20: 636b 203d 2069 735f 7374 6163 6b28 6564  ck = is_stack(ed
+00006b30: 6174 612c 2063 6c69 7374 2c20 6375 7272  ata, clist, curr
+00006b40: 5f63 616e 6473 203d 2063 7572 725f 6361  _cands = curr_ca
+00006b50: 6e64 7329 0a20 2020 2020 2020 2069 6620  nds).        if 
+00006b60: 6973 7374 6163 6b3a 200a 2020 2020 2020  isstack: .      
+00006b70: 2020 2020 2020 7769 6e6e 6572 732e 6170        winners.ap
+00006b80: 7065 6e64 2863 6c69 7374 5b30 5d29 0a20  pend(clist[0]). 
+00006b90: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+00006ba0: 7265 7475 726e 2073 6f72 7465 6428 6c69  return sorted(li
+00006bb0: 7374 2873 6574 2877 696e 6e65 7273 2929  st(set(winners))
+00006bc0: 290a 0a64 6566 205f 7261 6e6b 6564 5f70  )..def _ranked_p
+00006bd0: 6169 7273 5f62 6173 6963 280a 2020 2020  airs_basic(.    
+00006be0: 6564 6174 612c 200a 2020 2020 6375 7272  edata, .    curr
+00006bf0: 5f63 616e 6473 203d 204e 6f6e 652c 200a  _cands = None, .
+00006c00: 2020 2020 7374 7265 6e67 7468 5f66 756e      strength_fun
+00006c10: 6374 696f 6e20 3d20 4e6f 6e65 293a 2020  ction = None):  
+00006c20: 200a 2020 2020 2222 2241 6e20 696d 706c   .    """An impl
+00006c30: 656d 656e 7461 7469 6f6e 206f 6620 5261  ementation of Ra
+00006c40: 6e6b 6564 2050 6169 7273 2074 6861 7420  nked Pairs that 
+00006c50: 7573 6573 2061 2062 6173 6963 2061 6c67  uses a basic alg
+00006c60: 6f72 6974 686d 2e20 0a0a 2020 2020 4172  orithm. ..    Ar
+00006c70: 6773 3a0a 2020 2020 2020 2020 6564 6174  gs:.        edat
+00006c80: 6120 2850 726f 6669 6c65 2c20 5072 6f66  a (Profile, Prof
+00006c90: 696c 6557 6974 6854 6965 732c 204d 6172  ileWithTies, Mar
+00006ca0: 6769 6e47 7261 7068 293a 2041 6e79 2065  ginGraph): Any e
+00006cb0: 6c65 6374 696f 6e20 6461 7461 2074 6861  lection data tha
+00006cc0: 7420 6861 7320 6120 606d 6172 6769 6e60  t has a `margin`
+00006cd0: 206d 6574 686f 642e 200a 2020 2020 2020   method. .      
+00006ce0: 2020 6375 7272 5f63 616e 6473 2028 4c69    curr_cands (Li
+00006cf0: 7374 5b69 6e74 5d2c 206f 7074 696f 6e61  st[int], optiona
+00006d00: 6c29 3a20 4966 2073 6574 2c20 7468 656e  l): If set, then
+00006d10: 2066 696e 6420 7468 6520 7769 6e6e 6572   find the winner
+00006d20: 7320 666f 7220 7468 6520 7072 6f66 696c  s for the profil
+00006d30: 6520 7265 7374 7269 6374 6564 2074 6f20  e restricted to 
+00006d40: 7468 6520 6361 6e64 6964 6174 6573 2069  the candidates i
+00006d50: 6e20 6060 6375 7272 5f63 616e 6473 6060  n ``curr_cands``
+00006d60: 0a0a 2020 2020 5265 7475 726e 733a 200a  ..    Returns: .
+00006d70: 2020 2020 2020 2020 4120 736f 7274 6564          A sorted
+00006d80: 206c 6973 7420 6f66 2063 616e 6469 6461   list of candida
+00006d90: 7465 732e 200a 0a20 2020 2022 2222 0a20  tes. ..    """. 
+00006da0: 2020 2063 616e 6469 6461 7465 7320 3d20     candidates = 
+00006db0: 6564 6174 612e 6361 6e64 6964 6174 6573  edata.candidates
+00006dc0: 2069 6620 6375 7272 5f63 616e 6473 2069   if curr_cands i
+00006dd0: 7320 4e6f 6e65 2065 6c73 6520 6375 7272  s None else curr
+00006de0: 5f63 616e 6473 200a 2020 2020 6369 6478  _cands .    cidx
+00006df0: 5f74 6f5f 6361 6e64 203d 207b 6369 6478  _to_cand = {cidx
+00006e00: 3a20 6320 666f 7220 6369 6478 2c20 6320  : c for cidx, c 
+00006e10: 696e 2065 6e75 6d65 7261 7465 2863 616e  in enumerate(can
+00006e20: 6469 6461 7465 7329 7d20 200a 2020 2020  didates)}  .    
+00006e30: 6361 6e64 5f74 6f5f 6369 6478 203d 207b  cand_to_cidx = {
+00006e40: 633a 2063 6964 7820 666f 7220 6369 6478  c: cidx for cidx
+00006e50: 2c20 6320 696e 2065 6e75 6d65 7261 7465  , c in enumerate
+00006e60: 2863 616e 6469 6461 7465 7329 7d20 200a  (candidates)}  .
+00006e70: 2020 2020 7374 7265 6e67 7468 5f66 756e      strength_fun
+00006e80: 6374 696f 6e20 3d20 6564 6174 612e 6d61  ction = edata.ma
+00006e90: 7267 696e 2069 6620 7374 7265 6e67 7468  rgin if strength
+00006ea0: 5f66 756e 6374 696f 6e20 6973 204e 6f6e  _function is Non
+00006eb0: 6520 656c 7365 2073 7472 656e 6774 685f  e else strength_
+00006ec0: 6675 6e63 7469 6f6e 2020 2020 0a0a 2020  function    ..  
+00006ed0: 2020 6377 203d 2065 6461 7461 2e63 6f6e    cw = edata.con
+00006ee0: 646f 7263 6574 5f77 696e 6e65 7228 6375  dorcet_winner(cu
+00006ef0: 7272 5f63 616e 6473 3d63 7572 725f 6361  rr_cands=curr_ca
+00006f00: 6e64 7329 0a20 2020 2023 2052 616e 6b65  nds).    # Ranke
+00006f10: 6420 5061 6972 7320 6973 2043 6f6e 646f  d Pairs is Condo
+00006f20: 7263 6574 2063 6f6e 7369 7374 656e 742c  rcet consistent,
+00006f30: 2073 6f20 7369 6d70 6c79 2072 6574 7572   so simply retur
+00006f40: 6e20 7468 6520 436f 6e64 6f72 6365 7420  n the Condorcet 
+00006f50: 7769 6e6e 6572 2069 6620 6578 6973 7473  winner if exists
+00006f60: 0a20 2020 2069 6620 6377 2069 7320 6e6f  .    if cw is no
+00006f70: 7420 4e6f 6e65 3a20 0a20 2020 2020 2020  t None: .       
+00006f80: 2077 696e 6e65 7273 203d 205b 6377 5d0a   winners = [cw].
+00006f90: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00006fa0: 2020 775f 6564 6765 7320 3d20 5b28 6331    w_edges = [(c1
+00006fb0: 2c20 6332 2c20 7374 7265 6e67 7468 5f66  , c2, strength_f
+00006fc0: 756e 6374 696f 6e28 6331 2c20 6332 2929  unction(c1, c2))
+00006fd0: 2066 6f72 2063 3120 696e 2063 616e 6469   for c1 in candi
+00006fe0: 6461 7465 7320 666f 7220 6332 2069 6e20  dates for c2 in 
+00006ff0: 6361 6e64 6964 6174 6573 200a 2020 2020  candidates .    
+00007000: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00007010: 6620 6331 2021 3d20 6332 2061 6e64 2028  f c1 != c2 and (
+00007020: 6564 6174 612e 6d61 6a6f 7269 7479 5f70  edata.majority_p
+00007030: 7265 6665 7273 2863 312c 2063 3229 206f  refers(c1, c2) o
+00007040: 7220 6564 6174 612e 6973 5f74 6965 6428  r edata.is_tied(
+00007050: 6331 2c20 6332 2929 5d0a 2020 2020 2020  c1, c2))].      
+00007060: 2020 7769 6e6e 6572 7320 3d20 6c69 7374    winners = list
+00007070: 2829 2020 200a 2020 2020 2020 2020 6966  ()   .        if
+00007080: 206c 656e 2877 5f65 6467 6573 2920 3e20   len(w_edges) > 
+00007090: 303a 2020 2020 2020 2020 2020 0a20 2020  0:          .   
+000070a0: 2020 2020 2020 2020 2073 7472 656e 6774           strengt
+000070b0: 6873 203d 2073 6f72 7465 6428 6c69 7374  hs = sorted(list
+000070c0: 2873 6574 285b 655b 325d 2066 6f72 2065  (set([e[2] for e
+000070d0: 2069 6e20 775f 6564 6765 735d 2929 2c20   in w_edges])), 
+000070e0: 7265 7665 7273 653d 5472 7565 290a 2020  reverse=True).  
+000070f0: 2020 2020 2020 2020 2020 736f 7274 6564            sorted
+00007100: 5f65 6467 6573 203d 205b 5b65 2066 6f72  _edges = [[e for
+00007110: 2065 2069 6e20 775f 6564 6765 7320 6966   e in w_edges if
+00007120: 2065 5b32 5d20 3d3d 2073 5d20 666f 7220   e[2] == s] for 
+00007130: 7320 696e 2073 7472 656e 6774 6873 5d0a  s in strengths].
+00007140: 2020 2020 2020 2020 2020 2020 7462 7320              tbs 
+00007150: 3d20 7072 6f64 7563 7428 2a5b 7065 726d  = product(*[perm
+00007160: 7574 6174 696f 6e73 2865 6467 6573 2920  utations(edges) 
+00007170: 666f 7220 6564 6765 7320 696e 2073 6f72  for edges in sor
+00007180: 7465 645f 6564 6765 735d 290a 2020 2020  ted_edges]).    
+00007190: 2020 2020 2020 2020 666f 7220 7462 2069          for tb i
+000071a0: 6e20 7462 733a 0a20 2020 2020 2020 2020  n tbs:.         
+000071b0: 2020 2020 2020 2065 6467 6573 203d 2066         edges = f
+000071c0: 6c61 7474 656e 2874 6229 0a20 2020 2020  latten(tb).     
+000071d0: 2020 2020 2020 2020 2020 2072 705f 6465             rp_de
+000071e0: 6665 6174 203d 2053 504f 286c 656e 2863  feat = SPO(len(c
+000071f0: 616e 6469 6461 7465 7329 290a 2020 2020  andidates)).    
+00007200: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00007210: 6530 2c65 312c 7320 696e 2065 6467 6573  e0,e1,s in edges
+00007220: 3a20 0a20 2020 2020 2020 2020 2020 2020  : .             
+00007230: 2020 2020 2020 2069 6620 6e6f 7420 7270         if not rp
+00007240: 5f64 6566 6561 742e 505b 6361 6e64 5f74  _defeat.P[cand_t
+00007250: 6f5f 6369 6478 5b65 315d 5d5b 6361 6e64  o_cidx[e1]][cand
+00007260: 5f74 6f5f 6369 6478 5b65 305d 5d3a 0a20  _to_cidx[e0]]:. 
+00007270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007280: 2020 2020 2020 2072 705f 6465 6665 6174         rp_defeat
+00007290: 2e61 6464 2863 616e 645f 746f 5f63 6964  .add(cand_to_cid
+000072a0: 785b 6530 5d2c 6361 6e64 5f74 6f5f 6369  x[e0],cand_to_ci
+000072b0: 6478 5b65 315d 290a 2020 2020 2020 2020  dx[e1]).        
+000072c0: 2020 2020 2020 2020 7769 6e6e 6572 732e          winners.
+000072d0: 6170 7065 6e64 2863 6964 785f 746f 5f63  append(cidx_to_c
+000072e0: 616e 645b 7270 5f64 6566 6561 742e 696e  and[rp_defeat.in
+000072f0: 6974 6961 6c5f 656c 656d 656e 7473 2829  itial_elements()
+00007300: 5b30 5d5d 290a 2020 2020 2020 2020 656c  [0]]).        el
+00007310: 7365 3a20 0a20 2020 2020 2020 2020 2020  se: .           
+00007320: 2077 696e 6e65 7273 203d 2063 616e 6469   winners = candi
+00007330: 6461 7465 730a 2020 2020 7265 7475 726e  dates.    return
+00007340: 2073 6f72 7465 6428 6c69 7374 2873 6574   sorted(list(set
+00007350: 2877 696e 6e65 7273 2929 290a 0a0a 7270  (winners)))...rp
+00007360: 5f70 726f 7065 7274 6965 7320 3d20 566f  _properties = Vo
+00007370: 7469 6e67 4d65 7468 6f64 5072 6f70 6572  tingMethodProper
+00007380: 7469 6573 280a 2020 2020 636f 6e64 6f72  ties(.    condor
+00007390: 6365 745f 7769 6e6e 6572 3d54 7275 652c  cet_winner=True,
+000073a0: 200a 2020 2020 636f 6e64 6f72 6365 745f   .    condorcet_
+000073b0: 6c6f 7365 723d 5472 7565 2c0a 2020 2020  loser=True,.    
+000073c0: 7061 7265 746f 5f64 6f6d 696e 616e 6365  pareto_dominance
+000073d0: 3d54 7275 652c 200a 2020 2020 290a 4076  =True, .    ).@v
+000073e0: 6d28 6e61 6d65 3d22 5261 6e6b 6564 2050  m(name="Ranked P
+000073f0: 6169 7273 222c 0a20 2020 2070 726f 7065  airs",.    prope
+00007400: 7274 6965 733d 7270 5f70 726f 7065 7274  rties=rp_propert
+00007410: 6965 732c 0a20 2020 2069 6e70 7574 5f74  ies,.    input_t
+00007420: 7970 6573 3d5b 456c 6563 7469 6f6e 5479  ypes=[ElectionTy
+00007430: 7065 732e 5052 4f46 494c 452c 2045 6c65  pes.PROFILE, Ele
+00007440: 6374 696f 6e54 7970 6573 2e50 524f 4649  ctionTypes.PROFI
+00007450: 4c45 5f57 4954 485f 5449 4553 2c20 456c  LE_WITH_TIES, El
+00007460: 6563 7469 6f6e 5479 7065 732e 4d41 5247  ectionTypes.MARG
+00007470: 494e 5f47 5241 5048 5d29 0a64 6566 2072  IN_GRAPH]).def r
+00007480: 616e 6b65 645f 7061 6972 7328 0a20 2020  anked_pairs(.   
+00007490: 2065 6461 7461 2c20 0a20 2020 2063 7572   edata, .    cur
+000074a0: 725f 6361 6e64 733d 4e6f 6e65 2c20 0a20  r_cands=None, . 
+000074b0: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
+000074c0: 7469 6f6e 3d4e 6f6e 652c 200a 2020 2020  tion=None, .    
+000074d0: 616c 676f 7269 7468 6d3d 2762 6173 6963  algorithm='basic
+000074e0: 2729 3a20 2020 0a20 2020 2022 2222 0a20  '):   .    """. 
+000074f0: 2020 204f 7264 6572 2074 6865 2065 6467     Order the edg
+00007500: 6573 2069 6e20 7468 6520 6d61 7267 696e  es in the margin
+00007510: 2067 7261 7068 2066 726f 6d20 6c61 7267   graph from larg
+00007520: 6573 7420 746f 2073 6d61 6c6c 6573 7420  est to smallest 
+00007530: 616e 6420 6c6f 636b 2074 6865 6d20 696e  and lock them in
+00007540: 2069 6e20 7468 6174 206f 7264 6572 2c20   in that order, 
+00007550: 736b 6970 7069 6e67 2065 6467 6573 2074  skipping edges t
+00007560: 6861 7420 6372 6561 7465 2061 2063 7963  hat create a cyc
+00007570: 6c65 2e20 2049 6620 7468 6572 6520 6172  le.  If there ar
+00007580: 6520 7469 6573 2069 6e20 7468 6520 6d61  e ties in the ma
+00007590: 7267 696e 732c 2062 7265 616b 2074 6865  rgins, break the
+000075a0: 2074 6965 7320 7573 696e 6720 6120 7469   ties using a ti
+000075b0: 652d 6272 6561 6b69 6e67 2072 756c 653a  e-breaking rule:
+000075c0: 2061 206c 696e 6561 7220 6f72 6465 7269   a linear orderi
+000075d0: 6e67 206f 7665 7220 7468 6520 6564 6765  ng over the edge
+000075e0: 732e 2020 2041 2063 616e 6469 6461 7465  s.   A candidate
+000075f0: 2069 7320 6120 5261 6e6b 6564 2050 6169   is a Ranked Pai
+00007600: 7273 2077 696e 6e65 7220 6966 2069 7420  rs winner if it 
+00007610: 7769 6e73 2061 6363 6f72 6469 6e67 2074  wins according t
+00007620: 6f20 736f 6d65 2074 6965 2d62 7265 616b  o some tie-break
+00007630: 696e 6720 7275 6c65 2e20 416c 736f 206b  ing rule. Also k
+00007640: 6e6f 776e 2061 7320 5469 6465 6d61 6e27  nown as Tideman'
+00007650: 7320 5275 6c65 2e0a 0a20 2020 202e 2e20  s Rule...    .. 
+00007660: 7761 726e 696e 673a 3a20 0a20 2020 2020  warning:: .     
+00007670: 2020 2054 6869 7320 6d65 7468 6f64 2063     This method c
+00007680: 616e 2074 616b 6520 6120 7665 7279 206c  an take a very l
+00007690: 6f6e 6720 7469 6d65 2074 6f20 6669 6e64  ong time to find
+000076a0: 2077 696e 6e65 7273 2e20 0a20 2020 2020   winners. .     
+000076b0: 2020 200a 2020 2020 4172 6773 3a0a 2020     .    Args:.  
+000076c0: 2020 2020 2020 6564 6174 6120 2850 726f        edata (Pro
+000076d0: 6669 6c65 2c20 5072 6f66 696c 6557 6974  file, ProfileWit
+000076e0: 6854 6965 732c 204d 6172 6769 6e47 7261  hTies, MarginGra
+000076f0: 7068 293a 2041 6e79 2065 6c65 6374 696f  ph): Any electio
+00007700: 6e20 6461 7461 2074 6861 7420 6861 7320  n data that has 
+00007710: 6120 606d 6172 6769 6e60 206d 6574 686f  a `margin` metho
+00007720: 642e 200a 2020 2020 2020 2020 6375 7272  d. .        curr
+00007730: 5f63 616e 6473 2028 4c69 7374 5b69 6e74  _cands (List[int
+00007740: 5d2c 206f 7074 696f 6e61 6c29 3a20 4966  ], optional): If
+00007750: 2073 6574 2c20 7468 656e 2066 696e 6420   set, then find 
+00007760: 7468 6520 7769 6e6e 6572 7320 666f 7220  the winners for 
+00007770: 7468 6520 7072 6f66 696c 6520 7265 7374  the profile rest
+00007780: 7269 6374 6564 2074 6f20 7468 6520 6361  ricted to the ca
+00007790: 6e64 6964 6174 6573 2069 6e20 6060 6375  ndidates in ``cu
+000077a0: 7272 5f63 616e 6473 6060 0a20 2020 2020  rr_cands``.     
+000077b0: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
+000077c0: 7469 6f6e 2028 6675 6e63 7469 6f6e 2c20  tion (function, 
+000077d0: 6f70 7469 6f6e 616c 293a 2054 6865 2073  optional): The s
+000077e0: 7472 656e 6774 6820 6675 6e63 7469 6f6e  trength function
+000077f0: 2074 6f20 6265 2075 7365 6420 746f 2063   to be used to c
+00007800: 616c 6375 6c61 7465 2074 6865 2073 7472  alculate the str
+00007810: 656e 6774 6820 6f66 2061 2070 6174 682e  ength of a path.
+00007820: 2020 2054 6865 2064 6566 6175 6c74 2069     The default i
+00007830: 7320 7468 6520 6d61 7267 696e 206d 6574  s the margin met
+00007840: 686f 6420 6f66 2060 6065 6461 7461 6060  hod of ``edata``
+00007850: 2e20 2020 5468 6973 206f 6e6c 7920 6d61  .   This only ma
+00007860: 7474 6572 7320 7768 656e 2074 6865 2062  tters when the b
+00007870: 616c 6c6f 7473 2061 7265 206e 6f74 206c  allots are not l
+00007880: 696e 6561 7220 6f72 6465 7273 2e20 0a20  inear orders. . 
+00007890: 2020 2020 2020 2061 6c67 6f72 6974 686d         algorithm
+000078a0: 2028 7374 722c 206f 7074 696f 6e61 6c29   (str, optional)
+000078b0: 3a20 5370 6563 6966 7920 7768 6963 6820  : Specify which 
+000078c0: 616c 676f 7269 7468 6d20 746f 2075 7365  algorithm to use
+000078d0: 2e20 204f 7074 696f 6e73 2061 7265 2027  .  Options are '
+000078e0: 6261 7369 6327 2028 7468 6520 6465 6661  basic' (the defa
+000078f0: 756c 7429 2061 6e64 2027 6672 6f6d 5f73  ult) and 'from_s
+00007900: 7461 636b 7327 2e0a 0a20 2020 2052 6574  tacks'...    Ret
+00007910: 7572 6e73 3a20 0a20 2020 2020 2020 2041  urns: .        A
+00007920: 2073 6f72 7465 6420 6c69 7374 206f 6620   sorted list of 
+00007930: 6361 6e64 6964 6174 6573 2e20 0a0a 2020  candidates. ..  
+00007940: 2020 2e2e 2073 6565 616c 736f 3a3a 0a0a    .. seealso::..
+00007950: 2020 2020 2020 2020 3a6d 6574 683a 6070          :meth:`p
+00007960: 7265 665f 766f 7469 6e67 2e6d 6172 6769  ref_voting.margi
+00007970: 6e5f 6261 7365 645f 6d65 7468 6f64 732e  n_based_methods.
+00007980: 7261 6e6b 6564 5f70 6169 7273 5f77 6974  ranked_pairs_wit
+00007990: 685f 7465 7374 602c 203a 6d65 7468 3a60  h_test`, :meth:`
+000079a0: 7072 6566 5f76 6f74 696e 672e 6d61 7267  pref_voting.marg
+000079b0: 696e 5f62 6173 6564 5f6d 6574 686f 6473  in_based_methods
+000079c0: 2e72 616e 6b65 645f 7061 6972 735f 7a74  .ranked_pairs_zt
+000079d0: 602c 203a 6d65 7468 3a60 7072 6566 5f76  `, :meth:`pref_v
+000079e0: 6f74 696e 672e 6d61 7267 696e 5f62 6173  oting.margin_bas
+000079f0: 6564 5f6d 6574 686f 6473 2e72 616e 6b65  ed_methods.ranke
+00007a00: 645f 7061 6972 735f 6465 6665 6174 7360  d_pairs_defeats`
+00007a10: 0a0a 2020 2020 3a45 7861 6d70 6c65 3a20  ..    :Example: 
+00007a20: 0a0a 2020 2020 2e2e 2070 6c6f 743a 3a20  ..    .. plot:: 
+00007a30: 206d 6172 6769 6e5f 6772 6170 6873 5f65   margin_graphs_e
+00007a40: 7861 6d70 6c65 732f 6d67 5f65 785f 6270  xamples/mg_ex_bp
+00007a50: 5f72 702e 7079 0a20 2020 2020 2020 203a  _rp.py.        :
+00007a60: 636f 6e74 6578 743a 2072 6573 6574 2020  context: reset  
+00007a70: 0a20 2020 2020 2020 203a 696e 636c 7564  .        :includ
+00007a80: 652d 736f 7572 6365 3a20 5472 7565 0a0a  e-source: True..
+00007a90: 0a20 2020 202e 2e20 636f 6465 2d62 6c6f  .    .. code-blo
+00007aa0: 636b 3a3a 200a 0a20 2020 2020 2020 2066  ck:: ..        f
+00007ab0: 726f 6d20 7072 6566 5f76 6f74 696e 672e  rom pref_voting.
+00007ac0: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
+00007ad0: 686f 6473 2069 6d70 6f72 7420 7261 6e6b  hods import rank
+00007ae0: 6564 5f70 6169 7273 0a0a 2020 2020 2020  ed_pairs..      
+00007af0: 2020 7261 6e6b 6564 5f70 6169 7273 2e64    ranked_pairs.d
+00007b00: 6973 706c 6179 286d 6729 0a20 2020 2020  isplay(mg).     
+00007b10: 2020 2072 616e 6b65 645f 7061 6972 732e     ranked_pairs.
+00007b20: 6469 7370 6c61 7928 6d67 2c20 616c 676f  display(mg, algo
+00007b30: 7269 7468 6d3d 2762 6173 6963 2729 200a  rithm='basic') .
+00007b40: 2020 2020 2020 2020 7261 6e6b 6564 5f70          ranked_p
+00007b50: 6169 7273 2e64 6973 706c 6179 286d 672c  airs.display(mg,
+00007b60: 2061 6c67 6f72 6974 686d 3d27 6672 6f6d   algorithm='from
+00007b70: 5f73 7461 636b 7327 2920 2020 200a 0a0a  _stacks')    ...
+00007b80: 2020 2020 2e2e 2065 7865 635f 636f 6465      .. exec_code
+00007b90: 3a3a 200a 2020 2020 2020 2020 3a68 6964  :: .        :hid
+00007ba0: 655f 636f 6465 3a0a 0a20 2020 2020 2020  e_code:..       
+00007bb0: 2066 726f 6d20 7072 6566 5f76 6f74 696e   from pref_votin
+00007bc0: 672e 7765 6967 6874 6564 5f6d 616a 6f72  g.weighted_major
+00007bd0: 6974 795f 6772 6170 6873 2069 6d70 6f72  ity_graphs impor
+00007be0: 7420 4d61 7267 696e 4772 6170 680a 2020  t MarginGraph.  
+00007bf0: 2020 2020 2020 6672 6f6d 2070 7265 665f        from pref_
+00007c00: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
+00007c10: 7365 645f 6d65 7468 6f64 7320 696d 706f  sed_methods impo
+00007c20: 7274 2072 616e 6b65 645f 7061 6972 730a  rt ranked_pairs.
+00007c30: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00007c40: 206d 6720 3d20 4d61 7267 696e 4772 6170   mg = MarginGrap
+00007c50: 6828 5b30 2c20 312c 2032 2c20 335d 2c20  h([0, 1, 2, 3], 
+00007c60: 5b28 302c 2032 2c20 3329 2c20 2831 2c20  [(0, 2, 3), (1, 
+00007c70: 302c 2035 292c 2028 322c 2031 2c20 3529  0, 5), (2, 1, 5)
+00007c80: 2c20 2832 2c20 332c 2031 292c 2028 332c  , (2, 3, 1), (3,
+00007c90: 2030 2c20 3329 2c20 2833 2c20 312c 2031   0, 3), (3, 1, 1
+00007ca0: 295d 290a 2020 2020 2020 2020 0a20 2020  )]).        .   
+00007cb0: 2020 2020 2072 616e 6b65 645f 7061 6972       ranked_pair
+00007cc0: 732e 6469 7370 6c61 7928 6d67 290a 2020  s.display(mg).  
+00007cd0: 2020 2020 2020 7261 6e6b 6564 5f70 6169        ranked_pai
+00007ce0: 7273 2e64 6973 706c 6179 286d 672c 2061  rs.display(mg, a
+00007cf0: 6c67 6f72 6974 686d 3d27 6261 7369 6327  lgorithm='basic'
+00007d00: 290a 2020 2020 2020 2020 7261 6e6b 6564  ).        ranked
+00007d10: 5f70 6169 7273 2e64 6973 706c 6179 286d  _pairs.display(m
+00007d20: 672c 2061 6c67 6f72 6974 686d 3d27 6672  g, algorithm='fr
+00007d30: 6f6d 5f73 7461 636b 7327 290a 0a20 2020  om_stacks')..   
+00007d40: 2022 2222 0a0a 2020 2020 6966 2061 6c67   """..    if alg
+00007d50: 6f72 6974 686d 203d 3d20 2762 6173 6963  orithm == 'basic
+00007d60: 273a 0a20 2020 2020 2020 2072 6574 7572  ':.        retur
+00007d70: 6e20 5f72 616e 6b65 645f 7061 6972 735f  n _ranked_pairs_
+00007d80: 6261 7369 6328 6564 6174 612c 2063 7572  basic(edata, cur
+00007d90: 725f 6361 6e64 7320 3d20 6375 7272 5f63  r_cands = curr_c
+00007da0: 616e 6473 2c20 7374 7265 6e67 7468 5f66  ands, strength_f
+00007db0: 756e 6374 696f 6e20 3d20 7374 7265 6e67  unction = streng
+00007dc0: 7468 5f66 756e 6374 696f 6e29 0a20 2020  th_function).   
+00007dd0: 2065 6c69 6620 616c 676f 7269 7468 6d20   elif algorithm 
+00007de0: 3d3d 2027 6672 6f6d 5f73 7461 636b 7327  == 'from_stacks'
+00007df0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00007e00: 205f 7261 6e6b 6564 5f70 6169 7273 5f66   _ranked_pairs_f
+00007e10: 726f 6d5f 7374 6163 6b73 2865 6461 7461  rom_stacks(edata
+00007e20: 2c20 6375 7272 5f63 616e 6473 203d 2063  , curr_cands = c
+00007e30: 7572 725f 6361 6e64 7329 0a20 2020 2065  urr_cands).    e
+00007e40: 6c73 653a 0a20 2020 2020 2020 2072 6169  lse:.        rai
+00007e50: 7365 2056 616c 7565 4572 726f 7228 2249  se ValueError("I
+00007e60: 6e76 616c 6964 2061 6c67 6f72 6974 686d  nvalid algorithm
+00007e70: 2073 7065 6369 6669 6564 2e22 290a 0a40   specified.")..@
+00007e80: 766d 286e 616d 653d 2252 616e 6b65 6420  vm(name="Ranked 
+00007e90: 5061 6972 7322 2c0a 2020 2020 736b 6970  Pairs",.    skip
+00007ea0: 5f72 6567 6973 7472 6174 696f 6e3d 5472  _registration=Tr
+00007eb0: 7565 290a 6465 6620 7261 6e6b 6564 5f70  ue).def ranked_p
+00007ec0: 6169 7273 5f77 6974 685f 7465 7374 280a  airs_with_test(.
+00007ed0: 2020 2020 6564 6174 612c 200a 2020 2020      edata, .    
+00007ee0: 6375 7272 5f63 616e 6473 3d4e 6f6e 652c  curr_cands=None,
+00007ef0: 200a 2020 2020 7374 7265 6e67 7468 5f66   .    strength_f
+00007f00: 756e 6374 696f 6e3d 4e6f 6e65 293a 2020  unction=None):  
+00007f10: 200a 2020 2020 2222 2246 696e 6420 7468   .    """Find th
+00007f20: 6520 5261 6e6b 6564 2050 6169 7273 2077  e Ranked Pairs w
+00007f30: 696e 6e65 7273 2c20 6275 7420 696e 636c  inners, but incl
+00007f40: 7564 6520 6120 7465 7374 2074 6f20 6465  ude a test to de
+00007f50: 7465 726d 696e 6564 2069 6620 6974 2077  termined if it w
+00007f60: 696c 6c20 7461 6b65 2074 6f6f 206c 6f6e  ill take too lon
+00007f70: 6720 746f 2063 6f6d 7075 7465 2074 6865  g to compute the
+00007f80: 2052 616e 6b65 6420 5061 6972 7320 7769   Ranked Pairs wi
+00007f90: 6e6e 6572 732e 2049 6620 7468 6520 6361  nners. If the ca
+00007fa0: 6c63 756c 6174 696f 6e20 6f66 2074 6865  lculation of the
+00007fb0: 2077 696e 6e65 7273 2077 696c 6c20 7461   winners will ta
+00007fc0: 6b65 2074 6f6f 206c 6f6e 672c 2072 6574  ke too long, ret
+00007fd0: 7572 6e20 4e6f 6e65 2e0a 0a20 2020 202e  urn None...    .
+00007fe0: 2e20 696d 706f 7274 616e 743a 3a0a 2020  . important::.  
+00007ff0: 2020 2020 2020 5468 6973 2076 6f74 696e        This votin
+00008000: 6720 6d65 7468 6f64 2074 6861 7420 6d69  g method that mi
+00008010: 6768 7420 7265 7475 726e 204e 6f6e 6520  ght return None 
+00008020: 7261 7468 6572 2074 6861 6e20 6120 6c69  rather than a li
+00008030: 7374 206f 6620 6361 6e64 6964 6174 6573  st of candidates
+00008040: 2e20 200a 0a20 2020 2041 7267 733a 0a20  .  ..    Args:. 
+00008050: 2020 2020 2020 2065 6461 7461 2028 5072         edata (Pr
+00008060: 6f66 696c 652c 2050 726f 6669 6c65 5769  ofile, ProfileWi
+00008070: 7468 5469 6573 2c20 4d61 7267 696e 4772  thTies, MarginGr
+00008080: 6170 6829 3a20 416e 7920 656c 6563 7469  aph): Any electi
+00008090: 6f6e 2064 6174 6120 7468 6174 2068 6173  on data that has
+000080a0: 2061 2060 6d61 7267 696e 6020 6d65 7468   a `margin` meth
+000080b0: 6f64 2e20 0a20 2020 2020 2020 2063 7572  od. .        cur
+000080c0: 725f 6361 6e64 7320 284c 6973 745b 696e  r_cands (List[in
+000080d0: 745d 2c20 6f70 7469 6f6e 616c 293a 2049  t], optional): I
+000080e0: 6620 7365 742c 2074 6865 6e20 6669 6e64  f set, then find
+000080f0: 2074 6865 2077 696e 6e65 7273 2066 6f72   the winners for
+00008100: 2074 6865 2070 726f 6669 6c65 2072 6573   the profile res
+00008110: 7472 6963 7465 6420 746f 2074 6865 2063  tricted to the c
+00008120: 616e 6469 6461 7465 7320 696e 2060 6063  andidates in ``c
+00008130: 7572 725f 6361 6e64 7360 600a 2020 2020  urr_cands``.    
+00008140: 2020 2020 7374 7265 6e67 7468 5f66 756e      strength_fun
+00008150: 6374 696f 6e20 2866 756e 6374 696f 6e2c  ction (function,
+00008160: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
+00008170: 7374 7265 6e67 7468 2066 756e 6374 696f  strength functio
+00008180: 6e20 746f 2062 6520 7573 6564 2074 6f20  n to be used to 
+00008190: 6361 6c63 756c 6174 6520 7468 6520 7374  calculate the st
+000081a0: 7265 6e67 7468 206f 6620 6120 7061 7468  rength of a path
+000081b0: 2e20 2020 5468 6520 6465 6661 756c 7420  .   The default 
+000081c0: 6973 2074 6865 206d 6172 6769 6e20 6d65  is the margin me
+000081d0: 7468 6f64 206f 6620 6060 6564 6174 6160  thod of ``edata`
+000081e0: 602e 2020 2054 6869 7320 6f6e 6c79 206d  `.   This only m
+000081f0: 6174 7465 7273 2077 6865 6e20 7468 6520  atters when the 
+00008200: 6261 6c6c 6f74 7320 6172 6520 6e6f 7420  ballots are not 
+00008210: 6c69 6e65 6172 206f 7264 6572 732e 200a  linear orders. .
+00008220: 0a20 2020 2052 6574 7572 6e73 3a20 0a20  .    Returns: . 
+00008230: 2020 2020 2020 2041 2073 6f72 7465 6420         A sorted 
+00008240: 6c69 7374 206f 6620 6361 6e64 6964 6174  list of candidat
+00008250: 6573 2e20 0a0a 2020 2020 2e2e 2073 6565  es. ..    .. see
+00008260: 616c 736f 3a3a 0a0a 2020 2020 2020 2020  also::..        
+00008270: 3a6d 6574 683a 6070 7265 665f 766f 7469  :meth:`pref_voti
+00008280: 6e67 2e6d 6172 6769 6e5f 6261 7365 645f  ng.margin_based_
+00008290: 6d65 7468 6f64 732e 7261 6e6b 6564 5f70  methods.ranked_p
+000082a0: 6169 7273 5f77 6974 685f 7465 7374 602c  airs_with_test`,
+000082b0: 203a 6d65 7468 3a60 7072 6566 5f76 6f74   :meth:`pref_vot
+000082c0: 696e 672e 6d61 7267 696e 5f62 6173 6564  ing.margin_based
+000082d0: 5f6d 6574 686f 6473 2e72 616e 6b65 645f  _methods.ranked_
+000082e0: 7061 6972 735f 7a74 602c 203a 6d65 7468  pairs_zt`, :meth
+000082f0: 3a60 7072 6566 5f76 6f74 696e 672e 6d61  :`pref_voting.ma
+00008300: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
+00008310: 6473 2e72 616e 6b65 645f 7061 6972 735f  ds.ranked_pairs_
+00008320: 6465 6665 6174 7360 0a0a 2020 2020 3a45  defeats`..    :E
+00008330: 7861 6d70 6c65 3a20 0a0a 2020 2020 2e2e  xample: ..    ..
+00008340: 2070 6c6f 743a 3a20 206d 6172 6769 6e5f   plot::  margin_
+00008350: 6772 6170 6873 5f65 7861 6d70 6c65 732f  graphs_examples/
+00008360: 6d67 5f65 785f 7270 5f77 6974 685f 7465  mg_ex_rp_with_te
+00008370: 7374 2e70 790a 2020 2020 2020 2020 3a63  st.py.        :c
+00008380: 6f6e 7465 7874 3a20 7265 7365 7420 200a  ontext: reset  .
+00008390: 2020 2020 2020 2020 3a69 6e63 6c75 6465          :include
+000083a0: 2d73 6f75 7263 653a 2054 7275 650a 0a0a  -source: True...
+000083b0: 2020 2020 2e2e 2063 6f64 652d 626c 6f63      .. code-bloc
+000083c0: 6b3a 3a20 0a0a 2020 2020 2020 2020 6672  k:: ..        fr
+000083d0: 6f6d 2070 7265 665f 766f 7469 6e67 2e6d  om pref_voting.m
+000083e0: 6172 6769 6e5f 6261 7365 645f 6d65 7468  argin_based_meth
+000083f0: 6f64 7320 696d 706f 7274 2072 616e 6b65  ods import ranke
+00008400: 645f 7061 6972 735f 7769 7468 5f74 6573  d_pairs_with_tes
+00008410: 740a 0a20 2020 2020 2020 2072 616e 6b65  t..        ranke
+00008420: 645f 7061 6972 735f 7769 7468 5f74 6573  d_pairs_with_tes
+00008430: 742e 6469 7370 6c61 7928 6d67 290a 0a0a  t.display(mg)...
+00008440: 2020 2020 2e2e 2065 7865 635f 636f 6465      .. exec_code
+00008450: 3a3a 200a 2020 2020 2020 2020 3a68 6964  :: .        :hid
+00008460: 655f 636f 6465 3a0a 0a20 2020 2020 2020  e_code:..       
+00008470: 2066 726f 6d20 7072 6566 5f76 6f74 696e   from pref_votin
+00008480: 672e 7765 6967 6874 6564 5f6d 616a 6f72  g.weighted_major
+00008490: 6974 795f 6772 6170 6873 2069 6d70 6f72  ity_graphs impor
+000084a0: 7420 4d61 7267 696e 4772 6170 680a 2020  t MarginGraph.  
+000084b0: 2020 2020 2020 6672 6f6d 2070 7265 665f        from pref_
+000084c0: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
+000084d0: 7365 645f 6d65 7468 6f64 7320 696d 706f  sed_methods impo
+000084e0: 7274 2072 616e 6b65 645f 7061 6972 735f  rt ranked_pairs_
+000084f0: 7769 7468 5f74 6573 740a 2020 2020 2020  with_test.      
+00008500: 2020 0a20 2020 2020 2020 206d 6720 3d20    .        mg = 
+00008510: 4d61 7267 696e 4772 6170 6828 5b30 2c20  MarginGraph([0, 
+00008520: 312c 2032 2c20 335d 2c20 5b28 312c 2032  1, 2, 3], [(1, 2
+00008530: 2c20 3229 2c20 2831 2c20 332c 2032 292c  , 2), (1, 3, 2),
+00008540: 2028 322c 2030 2c20 3229 5d29 0a20 2020   (2, 0, 2)]).   
+00008550: 2020 2020 200a 2020 2020 2020 2020 7261       .        ra
+00008560: 6e6b 6564 5f70 6169 7273 5f77 6974 685f  nked_pairs_with_
+00008570: 7465 7374 2e64 6973 706c 6179 286d 6729  test.display(mg)
+00008580: 0a0a 0a20 2020 2022 2222 2020 2020 0a20  ...    """    . 
+00008590: 2020 2063 616e 6469 6461 7465 7320 3d20     candidates = 
+000085a0: 6564 6174 612e 6361 6e64 6964 6174 6573  edata.candidates
+000085b0: 2069 6620 6375 7272 5f63 616e 6473 2069   if curr_cands i
+000085c0: 7320 4e6f 6e65 2065 6c73 6520 6375 7272  s None else curr
+000085d0: 5f63 616e 6473 2020 2020 0a20 2020 2063  _cands    .    c
+000085e0: 6964 785f 746f 5f63 616e 6420 3d20 7b63  idx_to_cand = {c
+000085f0: 6964 783a 2063 2066 6f72 2063 6964 782c  idx: c for cidx,
+00008600: 2063 2069 6e20 656e 756d 6572 6174 6528   c in enumerate(
+00008610: 6361 6e64 6964 6174 6573 297d 2020 0a20  candidates)}  . 
+00008620: 2020 2063 616e 645f 746f 5f63 6964 7820     cand_to_cidx 
+00008630: 3d20 7b63 3a20 6369 6478 2066 6f72 2063  = {c: cidx for c
+00008640: 6964 782c 2063 2069 6e20 656e 756d 6572  idx, c in enumer
+00008650: 6174 6528 6361 6e64 6964 6174 6573 297d  ate(candidates)}
+00008660: 2020 0a20 2020 200a 2020 2020 7374 7265    .    .    stre
+00008670: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
+00008680: 6564 6174 612e 6d61 7267 696e 2069 6620  edata.margin if 
+00008690: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+000086a0: 6e20 6973 204e 6f6e 6520 656c 7365 2073  n is None else s
+000086b0: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+000086c0: 2020 200a 0a20 2020 2063 7720 3d20 6564     ..    cw = ed
+000086d0: 6174 612e 636f 6e64 6f72 6365 745f 7769  ata.condorcet_wi
+000086e0: 6e6e 6572 2863 7572 725f 6361 6e64 7320  nner(curr_cands 
+000086f0: 3d20 6375 7272 5f63 616e 6473 290a 2020  = curr_cands).  
+00008700: 2020 2320 5261 6e6b 6564 2050 6169 7273    # Ranked Pairs
+00008710: 2069 7320 436f 6e64 6f72 6365 7420 636f   is Condorcet co
+00008720: 6e73 6973 7465 6e74 2c20 736f 2073 696d  nsistent, so sim
+00008730: 706c 7920 7265 7475 726e 2074 6865 2043  ply return the C
+00008740: 6f6e 646f 7263 6574 2077 696e 6e65 7220  ondorcet winner 
+00008750: 6966 2065 7869 7374 730a 2020 2020 6966  if exists.    if
+00008760: 2063 7720 6973 206e 6f74 204e 6f6e 653a   cw is not None:
+00008770: 200a 2020 2020 2020 2020 7769 6e6e 6572   .        winner
+00008780: 7320 3d20 5b63 775d 0a20 2020 2065 6c73  s = [cw].    els
+00008790: 653a 0a20 2020 2020 2020 2077 5f65 6467  e:.        w_edg
+000087a0: 6573 203d 205b 2863 312c 2063 322c 2073  es = [(c1, c2, s
+000087b0: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+000087c0: 2863 312c 2063 3229 2920 666f 7220 6331  (c1, c2)) for c1
+000087d0: 2069 6e20 6361 6e64 6964 6174 6573 2066   in candidates f
+000087e0: 6f72 2063 3220 696e 2063 616e 6469 6461  or c2 in candida
+000087f0: 7465 7320 0a20 2020 2020 2020 2020 2020  tes .           
+00008800: 2020 2020 2020 2020 6966 2063 3120 213d          if c1 !=
+00008810: 2063 3220 616e 6420 2865 6461 7461 2e6d   c2 and (edata.m
+00008820: 616a 6f72 6974 795f 7072 6566 6572 7328  ajority_prefers(
+00008830: 6331 2c20 6332 2920 6f72 2065 6461 7461  c1, c2) or edata
+00008840: 2e69 735f 7469 6564 2863 312c 2063 3229  .is_tied(c1, c2)
+00008850: 295d 0a20 2020 2020 2020 2077 696e 6e65  )].        winne
+00008860: 7273 203d 206c 6973 7428 2920 2020 2020  rs = list()     
+00008870: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00008880: 7374 7265 6e67 7468 7320 3d20 736f 7274  strengths = sort
+00008890: 6564 286c 6973 7428 7365 7428 5b65 5b32  ed(list(set([e[2
+000088a0: 5d20 666f 7220 6520 696e 2077 5f65 6467  ] for e in w_edg
+000088b0: 6573 5d29 292c 2072 6576 6572 7365 3d54  es])), reverse=T
+000088c0: 7275 6529 0a20 2020 2020 2020 2073 6f72  rue).        sor
+000088d0: 7465 645f 6564 6765 7320 3d20 5b5b 6520  ted_edges = [[e 
+000088e0: 666f 7220 6520 696e 2077 5f65 6467 6573  for e in w_edges
+000088f0: 2069 6620 655b 325d 203d 3d20 735d 2066   if e[2] == s] f
+00008900: 6f72 2073 2069 6e20 7374 7265 6e67 7468  or s in strength
+00008910: 735d 0a20 2020 2020 2020 2069 6620 6e70  s].        if np
+00008920: 2e70 726f 6428 5b6d 6174 682e 6661 6374  .prod([math.fact
+00008930: 6f72 6961 6c28 6c65 6e28 6573 2929 2066  orial(len(es)) f
+00008940: 6f72 2065 7320 696e 2073 6f72 7465 645f  or es in sorted_
+00008950: 6564 6765 735d 2920 3e20 3330 3030 3a20  edges]) > 3000: 
+00008960: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00008970: 7572 6e20 4e6f 6e65 0a20 2020 2020 2020  urn None.       
+00008980: 2065 6c73 653a 200a 2020 2020 2020 2020   else: .        
+00008990: 2020 2020 7462 7320 3d20 7072 6f64 7563      tbs = produc
+000089a0: 7428 2a5b 7065 726d 7574 6174 696f 6e73  t(*[permutations
+000089b0: 2865 6467 6573 2920 666f 7220 6564 6765  (edges) for edge
+000089c0: 7320 696e 2073 6f72 7465 645f 6564 6765  s in sorted_edge
+000089d0: 735d 290a 2020 2020 2020 2020 2020 2020  s]).            
+000089e0: 666f 7220 7462 2069 6e20 7462 733a 0a20  for tb in tbs:. 
+000089f0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00008a00: 6467 6573 203d 2066 6c61 7474 656e 2874  dges = flatten(t
+00008a10: 6229 0a20 2020 2020 2020 2020 2020 2020  b).             
+00008a20: 2020 2072 705f 6465 6665 6174 203d 2053     rp_defeat = S
+00008a30: 504f 286c 656e 2863 616e 6469 6461 7465  PO(len(candidate
+00008a40: 7329 290a 2020 2020 2020 2020 2020 2020  s)).            
+00008a50: 2020 2020 666f 7220 6530 2c65 312c 7320      for e0,e1,s 
+00008a60: 696e 2065 6467 6573 3a20 0a20 2020 2020  in edges: .     
+00008a70: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00008a80: 6620 6e6f 7420 7270 5f64 6566 6561 742e  f not rp_defeat.
+00008a90: 505b 6361 6e64 5f74 6f5f 6369 6478 5b65  P[cand_to_cidx[e
+00008aa0: 315d 5d5b 6361 6e64 5f74 6f5f 6369 6478  1]][cand_to_cidx
+00008ab0: 5b65 305d 5d3a 0a20 2020 2020 2020 2020  [e0]]:.         
+00008ac0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00008ad0: 705f 6465 6665 6174 2e61 6464 2863 616e  p_defeat.add(can
+00008ae0: 645f 746f 5f63 6964 785b 6530 5d2c 6361  d_to_cidx[e0],ca
+00008af0: 6e64 5f74 6f5f 6369 6478 5b65 315d 290a  nd_to_cidx[e1]).
+00008b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b10: 7769 6e6e 6572 732e 6170 7065 6e64 2863  winners.append(c
+00008b20: 6964 785f 746f 5f63 616e 645b 7270 5f64  idx_to_cand[rp_d
+00008b30: 6566 6561 742e 696e 6974 6961 6c5f 656c  efeat.initial_el
+00008b40: 656d 656e 7473 2829 5b30 5d5d 290a 2020  ements()[0]]).  
+00008b50: 2020 7265 7475 726e 2073 6f72 7465 6428    return sorted(
+00008b60: 6c69 7374 2873 6574 2877 696e 6e65 7273  list(set(winners
+00008b70: 2929 290a 0a64 6566 2072 616e 6b65 645f  )))..def ranked_
+00008b80: 7061 6972 735f 6465 6665 6174 7328 6564  pairs_defeats(ed
+00008b90: 6174 612c 2063 7572 725f 6361 6e64 7320  ata, curr_cands 
+00008ba0: 3d20 4e6f 6e65 2c20 7374 7265 6e67 7468  = None, strength
+00008bb0: 5f66 756e 6374 696f 6e20 3d20 4e6f 6e65  _function = None
+00008bc0: 293a 2020 200a 2020 2020 2222 220a 2020  ):   .    """.  
+00008bd0: 2020 5265 7475 726e 7320 7468 6520 5261    Returns the Ra
+00008be0: 6e6b 6564 2050 6169 7273 2064 6566 6561  nked Pairs defea
+00008bf0: 7420 7265 6c61 7469 6f6e 7320 7072 6f64  t relations prod
+00008c00: 7563 6564 2062 7920 7468 6520 5261 6e6b  uced by the Rank
+00008c10: 6564 2050 6169 7273 2061 6c67 6f72 6974  ed Pairs algorit
+00008c20: 686d 2e20 0a0a 2020 2020 2e2e 2069 6d70  hm. ..    .. imp
+00008c30: 6f72 7461 6e74 3a3a 0a20 2020 2020 2020  ortant::.       
+00008c40: 2055 6e6c 696b 6520 7468 6520 6f74 6865   Unlike the othe
+00008c50: 7220 6675 6e63 7469 6f6e 7320 7468 6174  r functions that
+00008c60: 2072 6574 7572 6e20 6120 7369 6e67 6c65   return a single
+00008c70: 2064 6566 6561 7420 7265 6c61 7469 6f6e   defeat relation
+00008c80: 2c20 7468 6973 2072 6574 7572 6e73 2061  , this returns a
+00008c90: 206c 6973 7420 6f66 2064 6566 6561 7420   list of defeat 
+00008ca0: 7265 6c61 7469 6f6e 732e 200a 2020 2020  relations. .    
+00008cb0: 2020 2020 0a20 2020 2041 7267 733a 0a20      .    Args:. 
+00008cc0: 2020 2020 2020 2065 6461 7461 2028 5072         edata (Pr
+00008cd0: 6f66 696c 652c 2050 726f 6669 6c65 5769  ofile, ProfileWi
+00008ce0: 7468 5469 6573 2c20 4d61 7267 696e 4772  thTies, MarginGr
+00008cf0: 6170 6829 3a20 416e 7920 656c 6563 7469  aph): Any electi
+00008d00: 6f6e 2064 6174 6120 7468 6174 2068 6173  on data that has
+00008d10: 2061 2060 6d61 7267 696e 6020 6d65 7468   a `margin` meth
+00008d20: 6f64 2e20 0a20 2020 2020 2020 2063 7572  od. .        cur
+00008d30: 725f 6361 6e64 7320 284c 6973 745b 696e  r_cands (List[in
+00008d40: 745d 2c20 6f70 7469 6f6e 616c 293a 2049  t], optional): I
+00008d50: 6620 7365 742c 2074 6865 6e20 6669 6e64  f set, then find
+00008d60: 2074 6865 2077 696e 6e65 7273 2066 6f72   the winners for
+00008d70: 2074 6865 2070 726f 6669 6c65 2072 6573   the profile res
+00008d80: 7472 6963 7465 6420 746f 2074 6865 2063  tricted to the c
+00008d90: 616e 6469 6461 7465 7320 696e 2060 6063  andidates in ``c
+00008da0: 7572 725f 6361 6e64 7360 600a 2020 2020  urr_cands``.    
+00008db0: 2020 2020 7374 7265 6e67 7468 5f66 756e      strength_fun
+00008dc0: 6374 696f 6e20 2866 756e 6374 696f 6e2c  ction (function,
+00008dd0: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
+00008de0: 7374 7265 6e67 7468 2066 756e 6374 696f  strength functio
+00008df0: 6e20 746f 2062 6520 7573 6564 2074 6f20  n to be used to 
+00008e00: 6361 6c63 756c 6174 6520 7468 6520 7374  calculate the st
+00008e10: 7265 6e67 7468 206f 6620 6120 7061 7468  rength of a path
+00008e20: 2e20 2020 5468 6520 6465 6661 756c 7420  .   The default 
+00008e30: 6973 2074 6865 206d 6172 6769 6e20 6d65  is the margin me
+00008e40: 7468 6f64 206f 6620 6060 6564 6174 6160  thod of ``edata`
+00008e50: 602e 2020 2054 6869 7320 6f6e 6c79 206d  `.   This only m
+00008e60: 6174 7465 7273 2077 6865 6e20 7468 6520  atters when the 
+00008e70: 6261 6c6c 6f74 7320 6172 6520 6e6f 7420  ballots are not 
+00008e80: 6c69 6e65 6172 206f 7264 6572 732e 200a  linear orders. .
+00008e90: 0a20 2020 2052 6574 7572 6e73 3a20 0a20  .    Returns: . 
+00008ea0: 2020 2020 2020 2041 206e 6574 776f 726b         A network
+00008eb0: 7820 4469 4772 6170 6820 7265 7072 6573  x DiGraph repres
+00008ec0: 656e 7469 6e67 2074 6865 2052 616e 6b65  enting the Ranke
+00008ed0: 6420 5061 6972 7320 6465 6665 6174 2072  d Pairs defeat r
+00008ee0: 656c 6174 696f 6e2e 200a 0a20 2020 202e  elation. ..    .
+00008ef0: 2e20 7365 6561 6c73 6f3a 3a0a 0a20 2020  . seealso::..   
+00008f00: 2020 2020 203a 6d65 7468 3a60 7072 6566       :meth:`pref
+00008f10: 5f76 6f74 696e 672e 6d61 7267 696e 5f62  _voting.margin_b
+00008f20: 6173 6564 5f6d 6574 686f 6473 2e72 616e  ased_methods.ran
+00008f30: 6b65 645f 7061 6972 7360 2c20 3a6d 6574  ked_pairs`, :met
+00008f40: 683a 6070 7265 665f 766f 7469 6e67 2e6d  h:`pref_voting.m
+00008f50: 6172 6769 6e5f 6261 7365 645f 6d65 7468  argin_based_meth
+00008f60: 6f64 732e 7261 6e6b 6564 5f70 6169 7273  ods.ranked_pairs
+00008f70: 5f77 6974 685f 7465 7374 600a 0a20 2020  _with_test`..   
+00008f80: 203a 4578 616d 706c 653a 200a 0a20 2020   :Example: ..   
+00008f90: 202e 2e20 706c 6f74 3a3a 2020 6d61 7267   .. plot::  marg
+00008fa0: 696e 5f67 7261 7068 735f 6578 616d 706c  in_graphs_exampl
+00008fb0: 6573 2f6d 675f 6578 5f72 705f 6465 6665  es/mg_ex_rp_defe
+00008fc0: 6174 732e 7079 0a20 2020 2020 2020 203a  ats.py.        :
+00008fd0: 636f 6e74 6578 743a 2072 6573 6574 2020  context: reset  
+00008fe0: 0a20 2020 2020 2020 203a 696e 636c 7564  .        :includ
+00008ff0: 652d 736f 7572 6365 3a20 5472 7565 0a0a  e-source: True..
+00009000: 2020 2020 2e2e 2065 7865 635f 636f 6465      .. exec_code
+00009010: 3a3a 0a0a 0a20 2020 2020 2020 2066 726f  ::...        fro
+00009020: 6d20 7072 6566 5f76 6f74 696e 672e 7765  m pref_voting.we
+00009030: 6967 6874 6564 5f6d 616a 6f72 6974 795f  ighted_majority_
+00009040: 6772 6170 6873 2069 6d70 6f72 7420 4d61  graphs import Ma
+00009050: 7267 696e 4772 6170 680a 2020 2020 2020  rginGraph.      
+00009060: 2020 6672 6f6d 2070 7265 665f 766f 7469    from pref_voti
+00009070: 6e67 2e6d 6172 6769 6e5f 6261 7365 645f  ng.margin_based_
+00009080: 6d65 7468 6f64 7320 696d 706f 7274 2072  methods import r
+00009090: 616e 6b65 645f 7061 6972 735f 6465 6665  anked_pairs_defe
+000090a0: 6174 730a 0a20 2020 2020 2020 206d 6720  ats..        mg 
+000090b0: 3d20 4d61 7267 696e 4772 6170 6828 5b30  = MarginGraph([0
+000090c0: 2c20 312c 2032 2c20 335d 2c20 5b28 302c  , 1, 2, 3], [(0,
+000090d0: 2031 2c20 3130 292c 2028 302c 2032 2c20   1, 10), (0, 2, 
+000090e0: 3229 2c20 2831 2c20 332c 2034 292c 2028  2), (1, 3, 4), (
+000090f0: 322c 2031 2c20 3629 2c20 2832 2c20 332c  2, 1, 6), (2, 3,
+00009100: 2038 292c 2028 332c 2030 2c20 3429 5d29   8), (3, 0, 4)])
+00009110: 0a20 2020 2020 2020 2072 705f 6465 6665  .        rp_defe
+00009120: 6174 7320 3d20 7261 6e6b 6564 5f70 6169  ats = ranked_pai
+00009130: 7273 5f64 6566 6561 7473 286d 6729 0a0a  rs_defeats(mg)..
+00009140: 2020 2020 2020 2020 666f 7220 7270 6420          for rpd 
+00009150: 696e 2072 705f 6465 6665 6174 733a 200a  in rp_defeats: .
+00009160: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00009170: 7428 7270 642e 6564 6765 7329 0a0a 2020  t(rpd.edges)..  
+00009180: 2020 2222 220a 2020 2020 0a20 2020 2063    """.    .    c
+00009190: 616e 6469 6461 7465 7320 3d20 6564 6174  andidates = edat
+000091a0: 612e 6361 6e64 6964 6174 6573 2069 6620  a.candidates if 
+000091b0: 6375 7272 5f63 616e 6473 2069 7320 4e6f  curr_cands is No
+000091c0: 6e65 2065 6c73 6520 6375 7272 5f63 616e  ne else curr_can
+000091d0: 6473 2020 2020 0a20 2020 2073 7472 656e  ds    .    stren
+000091e0: 6774 685f 6675 6e63 7469 6f6e 203d 2065  gth_function = e
+000091f0: 6461 7461 2e6d 6172 6769 6e20 6966 2073  data.margin if s
+00009200: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+00009210: 2069 7320 4e6f 6e65 2065 6c73 6520 7374   is None else st
+00009220: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
+00009230: 2020 200a 0a20 2020 2077 5f65 6467 6573     ..    w_edges
+00009240: 203d 205b 2863 312c 2063 322c 2073 7472   = [(c1, c2, str
+00009250: 656e 6774 685f 6675 6e63 7469 6f6e 2863  ength_function(c
+00009260: 312c 2063 3229 2920 666f 7220 6331 2069  1, c2)) for c1 i
+00009270: 6e20 6361 6e64 6964 6174 6573 2066 6f72  n candidates for
+00009280: 2063 3220 696e 2063 616e 6469 6461 7465   c2 in candidate
+00009290: 7320 6966 2063 3120 213d 2063 3220 616e  s if c1 != c2 an
+000092a0: 6420 2865 6461 7461 2e6d 616a 6f72 6974  d (edata.majorit
+000092b0: 795f 7072 6566 6572 7328 6331 2c20 6332  y_prefers(c1, c2
+000092c0: 2920 6f72 2065 6461 7461 2e69 735f 7469  ) or edata.is_ti
+000092d0: 6564 2863 312c 2063 3229 295d 0a20 2020  ed(c1, c2))].   
+000092e0: 2077 696e 6e65 7273 203d 206c 6973 7428   winners = list(
+000092f0: 2920 2020 2020 2020 2020 2020 200a 2020  )            .  
+00009300: 2020 7374 7265 6e67 7468 7320 3d20 736f    strengths = so
+00009310: 7274 6564 286c 6973 7428 7365 7428 5b65  rted(list(set([e
+00009320: 5b32 5d20 666f 7220 6520 696e 2077 5f65  [2] for e in w_e
+00009330: 6467 6573 5d29 292c 2072 6576 6572 7365  dges])), reverse
+00009340: 3d54 7275 6529 0a20 2020 2073 6f72 7465  =True).    sorte
+00009350: 645f 6564 6765 7320 3d20 5b5b 6520 666f  d_edges = [[e fo
+00009360: 7220 6520 696e 2077 5f65 6467 6573 2069  r e in w_edges i
+00009370: 6620 655b 325d 203d 3d20 735d 2066 6f72  f e[2] == s] for
+00009380: 2073 2069 6e20 7374 7265 6e67 7468 735d   s in strengths]
+00009390: 0a20 2020 2074 6273 203d 2070 726f 6475  .    tbs = produ
+000093a0: 6374 282a 5b70 6572 6d75 7461 7469 6f6e  ct(*[permutation
+000093b0: 7328 6564 6765 7329 2066 6f72 2065 6467  s(edges) for edg
+000093c0: 6573 2069 6e20 736f 7274 6564 5f65 6467  es in sorted_edg
+000093d0: 6573 5d29 0a20 2020 2072 705f 6465 6665  es]).    rp_defe
+000093e0: 6174 7320 3d20 6c69 7374 2829 0a20 2020  ats = list().   
+000093f0: 2066 6f72 2074 6220 696e 2074 6273 3a0a   for tb in tbs:.
+00009400: 2020 2020 2020 2020 6564 6765 7320 3d20          edges = 
+00009410: 666c 6174 7465 6e28 7462 290a 2020 2020  flatten(tb).    
+00009420: 2020 2020 7270 5f64 6566 6561 7420 3d20      rp_defeat = 
+00009430: 6e78 2e44 6947 7261 7068 2829 200a 2020  nx.DiGraph() .  
+00009440: 2020 2020 2020 666f 7220 6520 696e 2065        for e in e
+00009450: 6467 6573 3a20 0a20 2020 2020 2020 2020  dges: .         
+00009460: 2020 2072 705f 6465 6665 6174 2e61 6464     rp_defeat.add
+00009470: 5f65 6467 6528 655b 305d 2c20 655b 315d  _edge(e[0], e[1]
+00009480: 2c20 7765 6967 6874 3d65 5b32 5d29 0a20  , weight=e[2]). 
+00009490: 2020 2020 2020 2020 2020 2069 6620 646f             if do
+000094a0: 6573 5f63 7265 6174 655f 6379 636c 6528  es_create_cycle(
+000094b0: 7270 5f64 6566 6561 742c 2065 293a 0a20  rp_defeat, e):. 
+000094c0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000094d0: 705f 6465 6665 6174 2e72 656d 6f76 655f  p_defeat.remove_
+000094e0: 6564 6765 2865 5b30 5d2c 2065 5b31 5d29  edge(e[0], e[1])
+000094f0: 0a20 2020 2020 2020 2072 705f 6465 6665  .        rp_defe
+00009500: 6174 732e 6170 7065 6e64 2872 705f 6465  ats.append(rp_de
+00009510: 6665 6174 290a 2020 2020 2020 2020 7769  feat).        wi
+00009520: 6e6e 6572 732e 6170 7065 6e64 286d 6178  nners.append(max
+00009530: 696d 616c 5f65 6c65 6d65 6e74 7328 7270  imal_elements(rp
+00009540: 5f64 6566 6561 7429 5b30 5d29 0a20 2020  _defeat)[0]).   
+00009550: 2072 6574 7572 6e20 7270 5f64 6566 6561   return rp_defea
+00009560: 7473 0a0a 7270 5f74 625f 7072 6f70 6572  ts..rp_tb_proper
+00009570: 7469 6573 203d 2056 6f74 696e 674d 6574  ties = VotingMet
+00009580: 686f 6450 726f 7065 7274 6965 7328 0a20  hodProperties(. 
+00009590: 2020 2063 6f6e 646f 7263 6574 5f77 696e     condorcet_win
+000095a0: 6e65 723d 5472 7565 2c20 0a20 2020 2063  ner=True, .    c
+000095b0: 6f6e 646f 7263 6574 5f6c 6f73 6572 3d54  ondorcet_loser=T
+000095c0: 7275 652c 0a20 2020 2070 6172 6574 6f5f  rue,.    pareto_
+000095d0: 646f 6d69 6e61 6e63 653d 5472 7565 2c20  dominance=True, 
+000095e0: 0a20 2020 2029 0a40 766d 286e 616d 653d  .    ).@vm(name=
+000095f0: 2252 616e 6b65 6420 5061 6972 7320 5442  "Ranked Pairs TB
+00009600: 222c 0a20 2020 2070 726f 7065 7274 6965  ",.    propertie
+00009610: 733d 7270 5f74 625f 7072 6f70 6572 7469  s=rp_tb_properti
+00009620: 6573 2c0a 2020 2020 696e 7075 745f 7479  es,.    input_ty
+00009630: 7065 733d 5b45 6c65 6374 696f 6e54 7970  pes=[ElectionTyp
+00009640: 6573 2e50 524f 4649 4c45 2c20 456c 6563  es.PROFILE, Elec
+00009650: 7469 6f6e 5479 7065 732e 5052 4f46 494c  tionTypes.PROFIL
+00009660: 455f 5749 5448 5f54 4945 532c 2045 6c65  E_WITH_TIES, Ele
+00009670: 6374 696f 6e54 7970 6573 2e4d 4152 4749  ctionTypes.MARGI
+00009680: 4e5f 4752 4150 485d 290a 6465 6620 7261  N_GRAPH]).def ra
+00009690: 6e6b 6564 5f70 6169 7273 5f74 6228 0a20  nked_pairs_tb(. 
+000096a0: 2020 2065 6461 7461 2c20 0a20 2020 2063     edata, .    c
+000096b0: 7572 725f 6361 6e64 7320 3d20 4e6f 6e65  urr_cands = None
+000096c0: 2c20 0a20 2020 2074 6965 5f62 7265 616b  , .    tie_break
+000096d0: 6572 203d 204e 6f6e 652c 200a 2020 2020  er = None, .    
+000096e0: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+000096f0: 6e20 3d20 4e6f 6e65 293a 2020 200a 2020  n = None):   .  
+00009700: 2020 2222 220a 2020 2020 5261 6e6b 6564    """.    Ranked
+00009710: 2050 6169 7273 2077 6974 6820 6120 6669   Pairs with a fi
+00009720: 7865 6420 6c69 6e65 6172 206f 7264 6572  xed linear order
+00009730: 206f 6e20 7468 6520 6361 6e64 6964 6174   on the candidat
+00009740: 6573 2074 6f20 6272 6561 6b20 616e 7920  es to break any 
+00009750: 7469 6573 2069 6e20 7468 6520 6d61 7267  ties in the marg
+00009760: 696e 732e 2020 200a 2020 2020 5369 6e63  ins.   .    Sinc
+00009770: 6520 7468 6520 7469 655f 6272 6561 6b65  e the tie_breake
+00009780: 7220 6973 2061 206c 696e 6561 7220 6f72  r is a linear or
+00009790: 6465 722c 2074 6869 7320 6d65 7468 6f64  der, this method
+000097a0: 2069 7320 7265 736f 6c75 7465 2e20 2020   is resolute.   
+000097b0: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+000097c0: 2020 2020 6564 6174 6120 2850 726f 6669      edata (Profi
+000097d0: 6c65 2c20 5072 6f66 696c 6557 6974 6854  le, ProfileWithT
+000097e0: 6965 732c 204d 6172 6769 6e47 7261 7068  ies, MarginGraph
+000097f0: 293a 2041 6e79 2065 6c65 6374 696f 6e20  ): Any election 
+00009800: 6461 7461 2074 6861 7420 6861 7320 6120  data that has a 
+00009810: 606d 6172 6769 6e60 206d 6574 686f 642e  `margin` method.
+00009820: 200a 2020 2020 2020 2020 6375 7272 5f63   .        curr_c
+00009830: 616e 6473 2028 4c69 7374 5b69 6e74 5d2c  ands (List[int],
+00009840: 206f 7074 696f 6e61 6c29 3a20 4966 2073   optional): If s
+00009850: 6574 2c20 7468 656e 2066 696e 6420 7468  et, then find th
+00009860: 6520 7769 6e6e 6572 7320 666f 7220 7468  e winners for th
+00009870: 6520 7072 6f66 696c 6520 7265 7374 7269  e profile restri
+00009880: 6374 6564 2074 6f20 7468 6520 6361 6e64  cted to the cand
+00009890: 6964 6174 6573 2069 6e20 6060 6375 7272  idates in ``curr
+000098a0: 5f63 616e 6473 6060 0a20 2020 2020 2020  _cands``.       
+000098b0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+000098c0: 6f6e 2028 6675 6e63 7469 6f6e 2c20 6f70  on (function, op
+000098d0: 7469 6f6e 616c 293a 2054 6865 2073 7472  tional): The str
+000098e0: 656e 6774 6820 6675 6e63 7469 6f6e 2074  ength function t
+000098f0: 6f20 6265 2075 7365 6420 746f 2063 616c  o be used to cal
+00009900: 6375 6c61 7465 2074 6865 2073 7472 656e  culate the stren
+00009910: 6774 6820 6f66 2061 2070 6174 682e 2020  gth of a path.  
+00009920: 2054 6865 2064 6566 6175 6c74 2069 7320   The default is 
+00009930: 7468 6520 6d61 7267 696e 206d 6574 686f  the margin metho
+00009940: 6420 6f66 2060 6065 6461 7461 6060 2e20  d of ``edata``. 
+00009950: 2020 5468 6973 206f 6e6c 7920 6d61 7474    This only matt
+00009960: 6572 7320 7768 656e 2074 6865 2062 616c  ers when the bal
+00009970: 6c6f 7473 2061 7265 206e 6f74 206c 696e  lots are not lin
+00009980: 6561 7220 6f72 6465 7273 2e20 0a0a 2020  ear orders. ..  
+00009990: 2020 5265 7475 726e 733a 200a 2020 2020    Returns: .    
+000099a0: 2020 2020 4120 736f 7274 6564 206c 6973      A sorted lis
+000099b0: 7420 6f66 2063 616e 6469 6461 7465 732e  t of candidates.
+000099c0: 200a 0a20 2020 202e 2e20 7365 6561 6c73   ..    .. seeals
+000099d0: 6f3a 3a0a 0a20 2020 2020 2020 203a 6d65  o::..        :me
+000099e0: 7468 3a60 7072 6566 5f76 6f74 696e 672e  th:`pref_voting.
+000099f0: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
+00009a00: 686f 6473 2e72 616e 6b65 645f 7061 6972  hods.ranked_pair
+00009a10: 7360 2c20 3a6d 6574 683a 6070 7265 665f  s`, :meth:`pref_
+00009a20: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
+00009a30: 7365 645f 6d65 7468 6f64 732e 7261 6e6b  sed_methods.rank
+00009a40: 6564 5f70 6169 7273 5f77 6974 685f 7465  ed_pairs_with_te
+00009a50: 7374 600a 0a20 2020 202e 2e20 6578 6563  st`..    .. exec
+00009a60: 5f63 6f64 653a 3a0a 0a20 2020 2020 2020  _code::..       
+00009a70: 2066 726f 6d20 7072 6566 5f76 6f74 696e   from pref_votin
+00009a80: 672e 7072 6f66 696c 6573 2069 6d70 6f72  g.profiles impor
+00009a90: 7420 5072 6f66 696c 650a 2020 2020 2020  t Profile.      
+00009aa0: 2020 6672 6f6d 2070 7265 665f 766f 7469    from pref_voti
+00009ab0: 6e67 2e6d 6172 6769 6e5f 6261 7365 645f  ng.margin_based_
+00009ac0: 6d65 7468 6f64 7320 696d 706f 7274 2072  methods import r
+00009ad0: 616e 6b65 645f 7061 6972 735f 7462 2c20  anked_pairs_tb, 
+00009ae0: 7261 6e6b 6564 5f70 6169 7273 5f7a 740a  ranked_pairs_zt.
+00009af0: 0a20 2020 2020 2020 2070 726f 6620 3d20  .        prof = 
+00009b00: 5072 6f66 696c 6528 5b5b 322c 2033 2c20  Profile([[2, 3, 
+00009b10: 312c 2030 5d2c 205b 302c 2033 2c20 312c  1, 0], [0, 3, 1,
+00009b20: 2032 5d2c 205b 312c 2033 2c20 322c 2030   2], [1, 3, 2, 0
+00009b30: 5d2c 205b 322c 2031 2c20 332c 2030 5d5d  ], [2, 1, 3, 0]]
+00009b40: 2c20 5b31 2c20 312c 2031 2c20 315d 290a  , [1, 1, 1, 1]).
+00009b50: 0a20 2020 2020 2020 2070 726f 662e 6469  .        prof.di
+00009b60: 7370 6c61 7928 290a 0a20 2020 2020 2020  splay()..       
+00009b70: 2072 616e 6b65 645f 7061 6972 735f 7462   ranked_pairs_tb
+00009b80: 2e64 6973 706c 6179 2870 726f 6629 0a20  .display(prof). 
+00009b90: 2020 2020 2020 2072 616e 6b65 645f 7061         ranked_pa
+00009ba0: 6972 735f 7462 2e64 6973 706c 6179 2870  irs_tb.display(p
+00009bb0: 726f 662c 2074 6965 5f62 7265 616b 6572  rof, tie_breaker
+00009bc0: 203d 205b 332c 2032 2c20 312c 2030 5d29   = [3, 2, 1, 0])
+00009bd0: 0a20 2020 2020 2020 2072 616e 6b65 645f  .        ranked_
+00009be0: 7061 6972 735f 7a74 2e64 6973 706c 6179  pairs_zt.display
+00009bf0: 2870 726f 6629 0a0a 2020 2020 2222 220a  (prof)..    """.
+00009c00: 0a20 2020 2063 616e 6469 6461 7465 7320  .    candidates 
+00009c10: 3d20 6564 6174 612e 6361 6e64 6964 6174  = edata.candidat
+00009c20: 6573 2069 6620 6375 7272 5f63 616e 6473  es if curr_cands
+00009c30: 2069 7320 4e6f 6e65 2065 6c73 6520 6375   is None else cu
+00009c40: 7272 5f63 616e 6473 2020 2020 0a20 2020  rr_cands    .   
+00009c50: 2063 6964 785f 746f 5f63 616e 6420 3d20   cidx_to_cand = 
+00009c60: 7b63 6964 783a 2063 2066 6f72 2063 6964  {cidx: c for cid
+00009c70: 782c 2063 2069 6e20 656e 756d 6572 6174  x, c in enumerat
+00009c80: 6528 6361 6e64 6964 6174 6573 297d 2020  e(candidates)}  
+00009c90: 0a20 2020 2063 616e 645f 746f 5f63 6964  .    cand_to_cid
+00009ca0: 7820 3d20 7b63 3a20 6369 6478 2066 6f72  x = {c: cidx for
+00009cb0: 2063 6964 782c 2063 2069 6e20 656e 756d   cidx, c in enum
+00009cc0: 6572 6174 6528 6361 6e64 6964 6174 6573  erate(candidates
+00009cd0: 297d 2020 0a0a 2020 2020 7374 7265 6e67  )}  ..    streng
+00009ce0: 7468 5f66 756e 6374 696f 6e20 3d20 6564  th_function = ed
+00009cf0: 6174 612e 6d61 7267 696e 2069 6620 7374  ata.margin if st
+00009d00: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
+00009d10: 6973 204e 6f6e 6520 656c 7365 2073 7472  is None else str
+00009d20: 656e 6774 685f 6675 6e63 7469 6f6e 0a20  ength_function. 
+00009d30: 2020 200a 2020 2020 7462 5f72 616e 6b69     .    tb_ranki
+00009d40: 6e67 203d 2074 6965 5f62 7265 616b 6572  ng = tie_breaker
+00009d50: 2069 6620 7469 655f 6272 6561 6b65 7220   if tie_breaker 
+00009d60: 6973 206e 6f74 204e 6f6e 6520 656c 7365  is not None else
+00009d70: 2073 6f72 7465 6428 6c69 7374 2863 616e   sorted(list(can
+00009d80: 6469 6461 7465 7329 290a 0a20 2020 2063  didates))..    c
+00009d90: 7720 3d20 6564 6174 612e 636f 6e64 6f72  w = edata.condor
+00009da0: 6365 745f 7769 6e6e 6572 2863 7572 725f  cet_winner(curr_
+00009db0: 6361 6e64 733d 6375 7272 5f63 616e 6473  cands=curr_cands
+00009dc0: 290a 2020 2020 2320 5261 6e6b 6564 2050  ).    # Ranked P
+00009dd0: 6169 7273 2069 7320 436f 6e64 6f72 6365  airs is Condorce
+00009de0: 7420 636f 6e73 6973 7465 6e74 2c20 736f  t consistent, so
+00009df0: 2073 696d 706c 7920 7265 7475 726e 2074   simply return t
+00009e00: 6865 2043 6f6e 646f 7263 6574 2077 696e  he Condorcet win
+00009e10: 6e65 7220 6966 2065 7869 7374 730a 2020  ner if exists.  
+00009e20: 2020 6966 2063 7720 6973 206e 6f74 204e    if cw is not N
+00009e30: 6f6e 653a 200a 2020 2020 2020 2020 7769  one: .        wi
+00009e40: 6e6e 6572 7320 3d20 5b63 775d 0a20 2020  nners = [cw].   
+00009e50: 2065 6c73 653a 0a20 2020 2020 2020 2077   else:.        w
+00009e60: 5f65 6467 6573 203d 205b 2863 312c 2063  _edges = [(c1, c
+00009e70: 322c 2073 7472 656e 6774 685f 6675 6e63  2, strength_func
+00009e80: 7469 6f6e 2863 312c 2063 3229 2920 666f  tion(c1, c2)) fo
+00009e90: 7220 6331 2069 6e20 6361 6e64 6964 6174  r c1 in candidat
+00009ea0: 6573 2066 6f72 2063 3220 696e 2063 616e  es for c2 in can
+00009eb0: 6469 6461 7465 7320 0a20 2020 2020 2020  didates .       
+00009ec0: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+00009ed0: 3120 213d 2063 3220 616e 6420 2865 6461  1 != c2 and (eda
+00009ee0: 7461 2e6d 616a 6f72 6974 795f 7072 6566  ta.majority_pref
+00009ef0: 6572 7328 6331 2c20 6332 2920 6f72 2065  ers(c1, c2) or e
+00009f00: 6461 7461 2e69 735f 7469 6564 2863 312c  data.is_tied(c1,
+00009f10: 2063 3229 295d 0a20 2020 2020 2020 2077   c2))].        w
+00009f20: 696e 6e65 7273 203d 206c 6973 7428 2920  inners = list() 
+00009f30: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+00009f40: 2020 2020 7374 7265 6e67 7468 7320 3d20      strengths = 
+00009f50: 736f 7274 6564 286c 6973 7428 7365 7428  sorted(list(set(
+00009f60: 5b65 5b32 5d20 666f 7220 6520 696e 2077  [e[2] for e in w
+00009f70: 5f65 6467 6573 5d29 292c 2072 6576 6572  _edges])), rever
+00009f80: 7365 3d54 7275 6529 0a20 2020 2020 2020  se=True).       
+00009f90: 200a 2020 2020 2020 2020 7270 5f64 6566   .        rp_def
+00009fa0: 6561 7420 3d20 5350 4f28 6c65 6e28 6361  eat = SPO(len(ca
+00009fb0: 6e64 6964 6174 6573 2929 0a0a 2020 2020  ndidates))..    
+00009fc0: 2020 2020 666f 7220 7320 696e 2073 7472      for s in str
+00009fd0: 656e 6774 6873 3a20 0a20 2020 2020 2020  engths: .       
+00009fe0: 2020 2020 2065 6467 6573 203d 205b 6520       edges = [e 
+00009ff0: 666f 7220 6520 696e 2077 5f65 6467 6573  for e in w_edges
+0000a000: 2069 6620 655b 325d 203d 3d20 735d 0a20   if e[2] == s]. 
+0000a010: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+0000a020: 2020 2020 2020 2020 2320 6272 6561 6b20          # break 
+0000a030: 7469 6573 2075 7369 6e67 2074 6865 206c  ties using the l
+0000a040: 6578 6963 6f67 7261 7068 6963 206f 7264  exicographic ord
+0000a050: 6572 696e 6720 6f6e 2074 7570 6c65 7320  ering on tuples 
+0000a060: 6769 7665 6e20 7462 5f72 616e 6b69 6e67  given tb_ranking
+0000a070: 0a20 2020 2020 2020 2020 2020 2073 6f72  .            sor
+0000a080: 7465 645f 6564 6765 7320 3d20 736f 7274  ted_edges = sort
+0000a090: 6564 2865 6467 6573 2c20 6b65 7920 3d20  ed(edges, key = 
+0000a0a0: 6c61 6d62 6461 2065 3a20 2874 625f 7261  lambda e: (tb_ra
+0000a0b0: 6e6b 696e 672e 696e 6465 7828 655b 305d  nking.index(e[0]
+0000a0c0: 292c 2074 625f 7261 6e6b 696e 672e 696e  ), tb_ranking.in
+0000a0d0: 6465 7828 655b 315d 2929 2c20 7265 7665  dex(e[1])), reve
+0000a0e0: 7273 653d 4661 6c73 6529 0a20 2020 2020  rse=False).     
+0000a0f0: 2020 2020 2020 2066 6f72 2065 302c 6531         for e0,e1
+0000a100: 2c73 2069 6e20 6564 6765 733a 200a 2020  ,s in edges: .  
+0000a110: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000a120: 206e 6f74 2072 705f 6465 6665 6174 2e50   not rp_defeat.P
+0000a130: 5b63 616e 645f 746f 5f63 6964 785b 6531  [cand_to_cidx[e1
+0000a140: 5d5d 5b63 616e 645f 746f 5f63 6964 785b  ]][cand_to_cidx[
+0000a150: 6530 5d5d 3a0a 2020 2020 2020 2020 2020  e0]]:.          
+0000a160: 2020 2020 2020 2020 2020 7270 5f64 6566            rp_def
+0000a170: 6561 742e 6164 6428 6361 6e64 5f74 6f5f  eat.add(cand_to_
+0000a180: 6369 6478 5b65 305d 2c63 616e 645f 746f  cidx[e0],cand_to
+0000a190: 5f63 6964 785b 6531 5d29 0a20 2020 2020  _cidx[e1]).     
+0000a1a0: 2020 2020 2020 2077 696e 6e65 7273 2e61         winners.a
+0000a1b0: 7070 656e 6428 6369 6478 5f74 6f5f 6361  ppend(cidx_to_ca
+0000a1c0: 6e64 5b72 705f 6465 6665 6174 2e69 6e69  nd[rp_defeat.ini
+0000a1d0: 7469 616c 5f65 6c65 6d65 6e74 7328 295b  tial_elements()[
+0000a1e0: 305d 5d29 0a0a 2020 2020 7265 7475 726e  0]])..    return
+0000a1f0: 2073 6f72 7465 6428 6c69 7374 2873 6574   sorted(list(set
+0000a200: 2877 696e 6e65 7273 2929 290a 0a72 705f  (winners)))..rp_
+0000a210: 7a74 5f70 726f 7065 7274 6965 7320 3d20  zt_properties = 
+0000a220: 566f 7469 6e67 4d65 7468 6f64 5072 6f70  VotingMethodProp
+0000a230: 6572 7469 6573 280a 2020 2020 636f 6e64  erties(.    cond
+0000a240: 6f72 6365 745f 7769 6e6e 6572 3d54 7275  orcet_winner=Tru
+0000a250: 652c 200a 2020 2020 636f 6e64 6f72 6365  e, .    condorce
+0000a260: 745f 6c6f 7365 723d 5472 7565 2c0a 2020  t_loser=True,.  
+0000a270: 2020 7061 7265 746f 5f64 6f6d 696e 616e    pareto_dominan
+0000a280: 6365 3d54 7275 652c 200a 2020 2020 290a  ce=True, .    ).
+0000a290: 4076 6d28 6e61 6d65 3d22 5261 6e6b 6564  @vm(name="Ranked
+0000a2a0: 2050 6169 7273 205a 5422 2c0a 2020 2020   Pairs ZT",.    
+0000a2b0: 7072 6f70 6572 7469 6573 3d72 705f 7a74  properties=rp_zt
+0000a2c0: 5f70 726f 7065 7274 6965 732c 0a20 2020  _properties,.   
+0000a2d0: 2069 6e70 7574 5f74 7970 6573 3d5b 456c   input_types=[El
+0000a2e0: 6563 7469 6f6e 5479 7065 732e 5052 4f46  ectionTypes.PROF
+0000a2f0: 494c 455d 290a 6465 6620 7261 6e6b 6564  ILE]).def ranked
+0000a300: 5f70 6169 7273 5f7a 7428 0a20 2020 2070  _pairs_zt(.    p
+0000a310: 726f 6669 6c65 2c20 0a20 2020 2063 7572  rofile, .    cur
+0000a320: 725f 6361 6e64 7320 3d20 4e6f 6e65 2c20  r_cands = None, 
+0000a330: 0a20 2020 2073 7472 656e 6774 685f 6675  .    strength_fu
+0000a340: 6e63 7469 6f6e 203d 204e 6f6e 6529 3a20  nction = None): 
+0000a350: 2020 0a20 2020 2022 2222 5261 6e6b 6564    .    """Ranked
+0000a360: 2070 6169 7273 2077 6865 7265 2061 2066   pairs where a f
+0000a370: 6978 6564 2076 6f74 6572 2062 7265 616b  ixed voter break
+0000a380: 7320 616e 7920 7469 6573 2069 6e20 7468  s any ties in th
+0000a390: 6520 6d61 7267 696e 732e 2020 4974 2069  e margins.  It i
+0000a3a0: 7320 616c 7761 7973 2074 6865 2076 6f74  s always the vot
+0000a3b0: 6572 2069 6e20 706f 7369 7469 6f6e 2030  er in position 0
+0000a3c0: 2074 6861 7420 6272 6561 6b73 2074 6865   that breaks the
+0000a3d0: 2074 6965 732e 2020 5369 6e63 6520 766f   ties.  Since vo
+0000a3e0: 7465 7273 2068 6176 6520 7374 7269 6374  ters have strict
+0000a3f0: 2070 7265 6665 7265 6e63 6573 2c20 7468   preferences, th
+0000a400: 6973 206d 6574 686f 6420 6973 2072 6573  is method is res
+0000a410: 6f6c 7574 652e 2020 5468 6973 2069 7320  olute.  This is 
+0000a420: 6b6e 6f77 6e20 6173 2052 616e 6b65 6420  known as Ranked 
+0000a430: 5061 6972 7320 5a54 2c20 666f 7220 5a61  Pairs ZT, for Za
+0000a440: 7669 7374 2054 6964 656d 616e 2e0a 0a20  vist Tideman... 
+0000a450: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+0000a460: 2065 6461 7461 2028 5072 6f66 696c 6529   edata (Profile)
+0000a470: 3a20 4120 7072 6f66 696c 6520 6f66 206c  : A profile of l
+0000a480: 696e 6561 7220 6f72 6465 7273 0a20 2020  inear orders.   
+0000a490: 2020 2020 2063 7572 725f 6361 6e64 7320       curr_cands 
+0000a4a0: 284c 6973 745b 696e 745d 2c20 6f70 7469  (List[int], opti
+0000a4b0: 6f6e 616c 293a 2049 6620 7365 742c 2074  onal): If set, t
+0000a4c0: 6865 6e20 6669 6e64 2074 6865 2077 696e  hen find the win
+0000a4d0: 6e65 7273 2066 6f72 2074 6865 2070 726f  ners for the pro
+0000a4e0: 6669 6c65 2072 6573 7472 6963 7465 6420  file restricted 
+0000a4f0: 746f 2074 6865 2063 616e 6469 6461 7465  to the candidate
+0000a500: 7320 696e 2060 6063 7572 725f 6361 6e64  s in ``curr_cand
+0000a510: 7360 600a 0a20 2020 2052 6574 7572 6e73  s``..    Returns
+0000a520: 3a20 0a20 2020 2020 2020 2041 2073 6f72  : .        A sor
+0000a530: 7465 6420 6c69 7374 206f 6620 6361 6e64  ted list of cand
+0000a540: 6964 6174 6573 2e20 0a0a 2020 2020 2e2e  idates. ..    ..
+0000a550: 2073 6565 616c 736f 3a3a 0a0a 2020 2020   seealso::..    
+0000a560: 2020 2020 3a6d 6574 683a 6070 7265 665f      :meth:`pref_
+0000a570: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
+0000a580: 7365 645f 6d65 7468 6f64 732e 7261 6e6b  sed_methods.rank
+0000a590: 6564 5f70 6169 7273 602c 203a 6d65 7468  ed_pairs`, :meth
+0000a5a0: 3a60 7072 6566 5f76 6f74 696e 672e 6d61  :`pref_voting.ma
+0000a5b0: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
+0000a5c0: 6473 2e72 616e 6b65 645f 7061 6972 735f  ds.ranked_pairs_
+0000a5d0: 7769 7468 5f74 6573 7460 0a0a 2020 2020  with_test`..    
+0000a5e0: 2e2e 2065 7865 635f 636f 6465 3a3a 0a0a  .. exec_code::..
+0000a5f0: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
+0000a600: 665f 766f 7469 6e67 2e70 726f 6669 6c65  f_voting.profile
+0000a610: 7320 696d 706f 7274 2050 726f 6669 6c65  s import Profile
+0000a620: 0a20 2020 2020 2020 2066 726f 6d20 7072  .        from pr
+0000a630: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
+0000a640: 5f62 6173 6564 5f6d 6574 686f 6473 2069  _based_methods i
+0000a650: 6d70 6f72 7420 7261 6e6b 6564 5f70 6169  mport ranked_pai
+0000a660: 7273 5f74 622c 2072 616e 6b65 645f 7061  rs_tb, ranked_pa
+0000a670: 6972 735f 7a74 0a0a 2020 2020 2020 2020  irs_zt..        
+0000a680: 7072 6f66 203d 2050 726f 6669 6c65 285b  prof = Profile([
+0000a690: 5b32 2c20 332c 2031 2c20 305d 2c20 5b30  [2, 3, 1, 0], [0
+0000a6a0: 2c20 332c 2031 2c20 325d 2c20 5b31 2c20  , 3, 1, 2], [1, 
+0000a6b0: 332c 2032 2c20 305d 2c20 5b32 2c20 312c  3, 2, 0], [2, 1,
+0000a6c0: 2033 2c20 305d 5d2c 205b 312c 2031 2c20   3, 0]], [1, 1, 
+0000a6d0: 312c 2031 5d29 0a0a 2020 2020 2020 2020  1, 1])..        
+0000a6e0: 7072 6f66 2e64 6973 706c 6179 2829 0a0a  prof.display()..
+0000a6f0: 2020 2020 2020 2020 7261 6e6b 6564 5f70          ranked_p
+0000a700: 6169 7273 5f74 622e 6469 7370 6c61 7928  airs_tb.display(
+0000a710: 7072 6f66 290a 2020 2020 2020 2020 7261  prof).        ra
+0000a720: 6e6b 6564 5f70 6169 7273 5f74 622e 6469  nked_pairs_tb.di
+0000a730: 7370 6c61 7928 7072 6f66 2c20 7469 655f  splay(prof, tie_
+0000a740: 6272 6561 6b65 7220 3d20 5b33 2c20 322c  breaker = [3, 2,
+0000a750: 2031 2c20 305d 290a 2020 2020 2020 2020   1, 0]).        
+0000a760: 7261 6e6b 6564 5f70 6169 7273 5f7a 742e  ranked_pairs_zt.
+0000a770: 6469 7370 6c61 7928 7072 6f66 290a 0a20  display(prof).. 
+0000a780: 2020 200a 2020 2020 2222 220a 2020 2020     .    """.    
+0000a790: 6361 6e64 6964 6174 6573 203d 2070 726f  candidates = pro
+0000a7a0: 6669 6c65 2e63 616e 6469 6461 7465 7320  file.candidates 
+0000a7b0: 6966 2063 7572 725f 6361 6e64 7320 6973  if curr_cands is
+0000a7c0: 204e 6f6e 6520 656c 7365 2063 7572 725f   None else curr_
+0000a7d0: 6361 6e64 7320 2020 200a 2020 2020 0a20  cands    .    . 
+0000a7e0: 2020 2023 2074 6865 2074 6965 2d62 7265     # the tie-bre
+0000a7f0: 616b 6572 2069 7320 616c 7761 7973 2074  aker is always t
+0000a800: 6865 2066 6972 7374 2076 6f74 6572 2e20  he first voter. 
+0000a810: 0a20 2020 2074 625f 7261 6e6b 696e 6720  .    tb_ranking 
+0000a820: 3d20 7475 706c 6528 5b63 2066 6f72 2063  = tuple([c for c
+0000a830: 2069 6e20 6c69 7374 2870 726f 6669 6c65   in list(profile
+0000a840: 2e5f 7261 6e6b 696e 6773 5b30 5d29 2069  ._rankings[0]) i
+0000a850: 6620 6320 696e 2063 616e 6469 6461 7465  f c in candidate
+0000a860: 735d 290a 2020 2020 0a20 2020 2072 6574  s]).    .    ret
+0000a870: 7572 6e20 7261 6e6b 6564 5f70 6169 7273  urn ranked_pairs
+0000a880: 5f74 6228 7072 6f66 696c 652c 2063 7572  _tb(profile, cur
+0000a890: 725f 6361 6e64 7320 3d20 6375 7272 5f63  r_cands = curr_c
+0000a8a0: 616e 6473 2c20 7469 655f 6272 6561 6b65  ands, tie_breake
+0000a8b0: 7220 3d20 7462 5f72 616e 6b69 6e67 2c20  r = tb_ranking, 
+0000a8c0: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+0000a8d0: 6e20 3d20 7374 7265 6e67 7468 5f66 756e  n = strength_fun
+0000a8e0: 6374 696f 6e29 0a0a 7269 7665 725f 7072  ction)..river_pr
+0000a8f0: 6f70 6572 7469 6573 203d 2056 6f74 696e  operties = Votin
+0000a900: 674d 6574 686f 6450 726f 7065 7274 6965  gMethodPropertie
+0000a910: 7328 0a20 2020 2063 6f6e 646f 7263 6574  s(.    condorcet
+0000a920: 5f77 696e 6e65 723d 5472 7565 2c20 0a20  _winner=True, . 
+0000a930: 2020 2063 6f6e 646f 7263 6574 5f6c 6f73     condorcet_los
+0000a940: 6572 3d54 7275 652c 0a20 2020 2070 6172  er=True,.    par
+0000a950: 6574 6f5f 646f 6d69 6e61 6e63 653d 5472  eto_dominance=Tr
+0000a960: 7565 2c20 0a20 2020 2029 0a40 766d 286e  ue, .    ).@vm(n
+0000a970: 616d 653d 2252 6976 6572 222c 0a20 2020  ame="River",.   
+0000a980: 2070 726f 7065 7274 6965 733d 7269 7665   properties=rive
+0000a990: 725f 7072 6f70 6572 7469 6573 2c0a 2020  r_properties,.  
+0000a9a0: 2020 696e 7075 745f 7479 7065 733d 5b45    input_types=[E
+0000a9b0: 6c65 6374 696f 6e54 7970 6573 2e50 524f  lectionTypes.PRO
+0000a9c0: 4649 4c45 2c20 456c 6563 7469 6f6e 5479  FILE, ElectionTy
+0000a9d0: 7065 732e 5052 4f46 494c 455f 5749 5448  pes.PROFILE_WITH
+0000a9e0: 5f54 4945 532c 2045 6c65 6374 696f 6e54  _TIES, ElectionT
+0000a9f0: 7970 6573 2e4d 4152 4749 4e5f 4752 4150  ypes.MARGIN_GRAP
+0000aa00: 485d 290a 6465 6620 7269 7665 7228 6564  H]).def river(ed
+0000aa10: 6174 612c 2063 7572 725f 6361 6e64 7320  ata, curr_cands 
+0000aa20: 3d20 4e6f 6e65 2c20 7374 7265 6e67 7468  = None, strength
+0000aa30: 5f66 756e 6374 696f 6e20 3d20 4e6f 6e65  _function = None
+0000aa40: 293a 2020 200a 2020 2020 2222 220a 2020  ):   .    """.  
+0000aa50: 2020 4f72 6465 7220 7468 6520 6564 6765    Order the edge
+0000aa60: 7320 696e 2074 6865 2077 6561 6b20 6d61  s in the weak ma
+0000aa70: 7267 696e 2067 7261 7068 2066 726f 6d20  rgin graph from 
+0000aa80: 6c61 7267 6573 7420 746f 2073 6d61 6c6c  largest to small
+0000aa90: 6573 7420 616e 6420 6c6f 636b 2074 6865  est and lock the
+0000aaa0: 6d20 696e 2069 6e20 7468 6174 206f 7264  m in in that ord
+0000aab0: 6572 2c20 736b 6970 7069 6e67 2065 6467  er, skipping edg
+0000aac0: 6573 2074 6861 7420 6372 6561 7465 2061  es that create a
+0000aad0: 2063 7963 6c65 202a 616e 6420 6564 6765   cycle *and edge
+0000aae0: 7320 696e 2077 6869 6368 2074 6865 7265  s in which there
+0000aaf0: 2069 7320 616c 7265 6164 7920 616e 2065   is already an e
+0000ab00: 6467 6520 706f 696e 7469 6e67 2074 6f20  dge pointing to 
+0000ab10: 7468 6520 7461 7267 6574 2a2e 2020 4272  the target*.  Br
+0000ab20: 6561 6b20 7469 6573 2075 7369 6e67 2061  eak ties using a
+0000ab30: 2074 6965 2d62 7265 616b 696e 6720 206c   tie-breaking  l
+0000ab40: 696e 6561 7220 6f72 6465 7269 6e67 206f  inear ordering o
+0000ab50: 7665 7220 7468 6520 6564 6765 732e 2020  ver the edges.  
+0000ab60: 4120 6361 6e64 6964 6174 6520 6973 2061  A candidate is a
+0000ab70: 2052 6976 6572 2077 696e 6e65 7220 6966   River winner if
+0000ab80: 2069 7420 7769 6e73 2061 6363 6f72 6469   it wins accordi
+0000ab90: 6e67 2074 6f20 736f 6d65 2074 6965 2d62  ng to some tie-b
+0000aba0: 7265 616b 696e 6720 7275 6c65 2e20 5365  reaking rule. Se
+0000abb0: 6520 6874 7470 733a 2f2f 656c 6563 746f  e https://electo
+0000abc0: 7769 6b69 2e6f 7267 2f77 696b 692f 5269  wiki.org/wiki/Ri
+0000abd0: 7665 722e 0a0a 2020 2020 4172 6773 3a0a  ver...    Args:.
+0000abe0: 2020 2020 2020 2020 6564 6174 6120 2850          edata (P
+0000abf0: 726f 6669 6c65 2c20 5072 6f66 696c 6557  rofile, ProfileW
+0000ac00: 6974 6854 6965 732c 204d 6172 6769 6e47  ithTies, MarginG
+0000ac10: 7261 7068 293a 2041 6e79 2065 6c65 6374  raph): Any elect
+0000ac20: 696f 6e20 6461 7461 2074 6861 7420 6861  ion data that ha
+0000ac30: 7320 6120 606d 6172 6769 6e60 206d 6574  s a `margin` met
+0000ac40: 686f 642e 200a 2020 2020 2020 2020 6375  hod. .        cu
+0000ac50: 7272 5f63 616e 6473 2028 4c69 7374 5b69  rr_cands (List[i
+0000ac60: 6e74 5d2c 206f 7074 696f 6e61 6c29 3a20  nt], optional): 
+0000ac70: 4966 2073 6574 2c20 7468 656e 2066 696e  If set, then fin
+0000ac80: 6420 7468 6520 7769 6e6e 6572 7320 666f  d the winners fo
+0000ac90: 7220 7468 6520 7072 6f66 696c 6520 7265  r the profile re
+0000aca0: 7374 7269 6374 6564 2074 6f20 7468 6520  stricted to the 
+0000acb0: 6361 6e64 6964 6174 6573 2069 6e20 6060  candidates in ``
+0000acc0: 6375 7272 5f63 616e 6473 6060 0a20 2020  curr_cands``.   
+0000acd0: 2020 2020 2073 7472 656e 6774 685f 6675       strength_fu
+0000ace0: 6e63 7469 6f6e 2028 6675 6e63 7469 6f6e  nction (function
+0000acf0: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
+0000ad00: 2073 7472 656e 6774 6820 6675 6e63 7469   strength functi
+0000ad10: 6f6e 2074 6f20 6265 2075 7365 6420 746f  on to be used to
+0000ad20: 2063 616c 6375 6c61 7465 2074 6865 2073   calculate the s
+0000ad30: 7472 656e 6774 6820 6f66 2061 2070 6174  trength of a pat
+0000ad40: 682e 2020 2054 6865 2064 6566 6175 6c74  h.   The default
+0000ad50: 2069 7320 7468 6520 6d61 7267 696e 206d   is the margin m
+0000ad60: 6574 686f 6420 6f66 2060 6065 6461 7461  ethod of ``edata
+0000ad70: 6060 2e20 2020 5468 6973 206f 6e6c 7920  ``.   This only 
+0000ad80: 6d61 7474 6572 7320 7768 656e 2074 6865  matters when the
+0000ad90: 2062 616c 6c6f 7473 2061 7265 206e 6f74   ballots are not
+0000ada0: 206c 696e 6561 7220 6f72 6465 7273 2e20   linear orders. 
+0000adb0: 0a0a 2020 2020 5265 7475 726e 733a 200a  ..    Returns: .
+0000adc0: 2020 2020 2020 2020 4120 736f 7274 6564          A sorted
+0000add0: 206c 6973 7420 6f66 2063 616e 6469 6461   list of candida
+0000ade0: 7465 732e 200a 0a20 2020 203a 4578 616d  tes. ..    :Exam
+0000adf0: 706c 653a 200a 0a20 2020 202e 2e20 6578  ple: ..    .. ex
+0000ae00: 6563 5f63 6f64 653a 3a20 0a0a 2020 2020  ec_code:: ..    
+0000ae10: 2020 2020 6672 6f6d 2070 7265 665f 766f      from pref_vo
+0000ae20: 7469 6e67 2e77 6569 6768 7465 645f 6d61  ting.weighted_ma
+0000ae30: 6a6f 7269 7479 5f67 7261 7068 7320 696d  jority_graphs im
+0000ae40: 706f 7274 204d 6172 6769 6e47 7261 7068  port MarginGraph
+0000ae50: 0a20 2020 2020 2020 2066 726f 6d20 7072  .        from pr
+0000ae60: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
+0000ae70: 5f62 6173 6564 5f6d 6574 686f 6473 2069  _based_methods i
+0000ae80: 6d70 6f72 7420 7269 7665 722c 2072 616e  mport river, ran
+0000ae90: 6b65 645f 7061 6972 730a 2020 2020 2020  ked_pairs.      
+0000aea0: 2020 0a20 2020 2020 2020 206d 6720 3d20    .        mg = 
+0000aeb0: 4d61 7267 696e 4772 6170 6828 5b30 2c20  MarginGraph([0, 
+0000aec0: 312c 2032 2c20 335d 2c20 5b28 302c 2032  1, 2, 3], [(0, 2
+0000aed0: 2c20 3229 2c20 2830 2c20 332c 2038 292c  , 2), (0, 3, 8),
+0000aee0: 2028 312c 2030 2c20 3132 292c 2028 322c   (1, 0, 12), (2,
+0000aef0: 2033 2c20 3132 292c 2028 332c 2031 2c20   3, 12), (3, 1, 
+0000af00: 3629 5d29 0a0a 2020 2020 2020 2020 7261  6)])..        ra
+0000af10: 6e6b 6564 5f70 6169 7273 2e64 6973 706c  nked_pairs.displ
+0000af20: 6179 286d 6729 0a20 2020 2020 2020 2072  ay(mg).        r
+0000af30: 6976 6572 2e64 6973 706c 6179 286d 6729  iver.display(mg)
+0000af40: 0a0a 2020 2020 2222 220a 2020 2020 6361  ..    """.    ca
+0000af50: 6e64 6964 6174 6573 203d 2065 6461 7461  ndidates = edata
+0000af60: 2e63 616e 6469 6461 7465 7320 6966 2063  .candidates if c
+0000af70: 7572 725f 6361 6e64 7320 6973 204e 6f6e  urr_cands is Non
+0000af80: 6520 656c 7365 2063 7572 725f 6361 6e64  e else curr_cand
+0000af90: 7320 2020 200a 2020 2020 6369 6478 5f74  s    .    cidx_t
+0000afa0: 6f5f 6361 6e64 203d 207b 6369 6478 3a20  o_cand = {cidx: 
+0000afb0: 6320 666f 7220 6369 6478 2c20 6320 696e  c for cidx, c in
+0000afc0: 2065 6e75 6d65 7261 7465 2863 616e 6469   enumerate(candi
+0000afd0: 6461 7465 7329 7d20 200a 2020 2020 6361  dates)}  .    ca
+0000afe0: 6e64 5f74 6f5f 6369 6478 203d 207b 633a  nd_to_cidx = {c:
+0000aff0: 2063 6964 7820 666f 7220 6369 6478 2c20   cidx for cidx, 
+0000b000: 6320 696e 2065 6e75 6d65 7261 7465 2863  c in enumerate(c
+0000b010: 616e 6469 6461 7465 7329 7d20 200a 0a20  andidates)}  .. 
+0000b020: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
+0000b030: 7469 6f6e 203d 2065 6461 7461 2e6d 6172  tion = edata.mar
+0000b040: 6769 6e20 6966 2073 7472 656e 6774 685f  gin if strength_
+0000b050: 6675 6e63 7469 6f6e 2069 7320 4e6f 6e65  function is None
+0000b060: 2065 6c73 6520 7374 7265 6e67 7468 5f66   else strength_f
+0000b070: 756e 6374 696f 6e20 2020 200a 0a20 2020  unction    ..   
+0000b080: 2063 7720 3d20 6564 6174 612e 636f 6e64   cw = edata.cond
+0000b090: 6f72 6365 745f 7769 6e6e 6572 2863 7572  orcet_winner(cur
+0000b0a0: 725f 6361 6e64 733d 6375 7272 5f63 616e  r_cands=curr_can
+0000b0b0: 6473 290a 2020 2020 2320 5261 6e6b 6564  ds).    # Ranked
+0000b0c0: 2050 6169 7273 2069 7320 436f 6e64 6f72   Pairs is Condor
+0000b0d0: 6365 7420 636f 6e73 6973 7465 6e74 2c20  cet consistent, 
+0000b0e0: 736f 2073 696d 706c 7920 7265 7475 726e  so simply return
+0000b0f0: 2074 6865 2043 6f6e 646f 7263 6574 2077   the Condorcet w
+0000b100: 696e 6e65 7220 6966 2065 7869 7374 730a  inner if exists.
+0000b110: 2020 2020 6966 2063 7720 6973 206e 6f74      if cw is not
+0000b120: 204e 6f6e 653a 200a 2020 2020 2020 2020   None: .        
+0000b130: 7769 6e6e 6572 7320 3d20 5b63 775d 0a20  winners = [cw]. 
+0000b140: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000b150: 2077 5f65 6467 6573 203d 205b 2863 312c   w_edges = [(c1,
+0000b160: 2063 322c 2073 7472 656e 6774 685f 6675   c2, strength_fu
+0000b170: 6e63 7469 6f6e 2863 312c 2063 3229 2920  nction(c1, c2)) 
+0000b180: 666f 7220 6331 2069 6e20 6361 6e64 6964  for c1 in candid
+0000b190: 6174 6573 2066 6f72 2063 3220 696e 2063  ates for c2 in c
+0000b1a0: 616e 6469 6461 7465 7320 0a20 2020 2020  andidates .     
+0000b1b0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000b1c0: 2063 3120 213d 2063 3220 616e 6420 2865   c1 != c2 and (e
+0000b1d0: 6461 7461 2e6d 616a 6f72 6974 795f 7072  data.majority_pr
+0000b1e0: 6566 6572 7328 6331 2c20 6332 2920 6f72  efers(c1, c2) or
+0000b1f0: 2065 6461 7461 2e69 735f 7469 6564 2863   edata.is_tied(c
+0000b200: 312c 2063 3229 295d 0a20 2020 2020 2020  1, c2))].       
+0000b210: 2077 696e 6e65 7273 203d 206c 6973 7428   winners = list(
+0000b220: 2920 2020 2020 2020 2020 2020 200a 2020  )            .  
+0000b230: 2020 2020 2020 7374 7265 6e67 7468 7320        strengths 
+0000b240: 3d20 736f 7274 6564 286c 6973 7428 7365  = sorted(list(se
+0000b250: 7428 5b65 5b32 5d20 666f 7220 6520 696e  t([e[2] for e in
+0000b260: 2077 5f65 6467 6573 5d29 292c 2072 6576   w_edges])), rev
+0000b270: 6572 7365 3d54 7275 6529 0a20 2020 2020  erse=True).     
+0000b280: 2020 2073 6f72 7465 645f 6564 6765 7320     sorted_edges 
+0000b290: 3d20 5b5b 6520 666f 7220 6520 696e 2077  = [[e for e in w
+0000b2a0: 5f65 6467 6573 2069 6620 655b 325d 203d  _edges if e[2] =
+0000b2b0: 3d20 735d 2066 6f72 2073 2069 6e20 7374  = s] for s in st
+0000b2c0: 7265 6e67 7468 735d 0a20 2020 2020 2020  rengths].       
+0000b2d0: 2074 6273 203d 2070 726f 6475 6374 282a   tbs = product(*
+0000b2e0: 5b70 6572 6d75 7461 7469 6f6e 7328 6564  [permutations(ed
+0000b2f0: 6765 7329 2066 6f72 2065 6467 6573 2069  ges) for edges i
+0000b300: 6e20 736f 7274 6564 5f65 6467 6573 5d29  n sorted_edges])
+0000b310: 0a20 2020 2020 2020 2066 6f72 2074 6220  .        for tb 
+0000b320: 696e 2074 6273 3a0a 2020 2020 2020 2020  in tbs:.        
+0000b330: 2020 2020 6564 6765 7320 3d20 666c 6174      edges = flat
+0000b340: 7465 6e28 7462 290a 2020 2020 2020 2020  ten(tb).        
+0000b350: 2020 2020 7276 5f64 6566 6561 7420 3d20      rv_defeat = 
+0000b360: 5350 4f28 6c65 6e28 6361 6e64 6964 6174  SPO(len(candidat
+0000b370: 6573 2929 0a20 2020 2020 2020 2020 2020  es)).           
+0000b380: 2066 6f72 2065 302c 6531 2c73 2069 6e20   for e0,e1,s in 
+0000b390: 6564 6765 733a 200a 2020 2020 2020 2020  edges: .        
+0000b3a0: 2020 2020 2020 2020 6966 206e 6f74 2072          if not r
+0000b3b0: 765f 6465 6665 6174 2e50 5b63 616e 645f  v_defeat.P[cand_
+0000b3c0: 746f 5f63 6964 785b 6531 5d5d 5b63 616e  to_cidx[e1]][can
+0000b3d0: 645f 746f 5f63 6964 785b 6530 5d5d 2061  d_to_cidx[e0]] a
+0000b3e0: 6e64 206c 656e 2872 765f 6465 6665 6174  nd len(rv_defeat
+0000b3f0: 2e70 7265 6473 5b63 616e 645f 746f 5f63  .preds[cand_to_c
+0000b400: 6964 785b 6531 5d5d 2920 3d3d 2030 3a0a  idx[e1]]) == 0:.
+0000b410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b420: 2020 2020 7276 5f64 6566 6561 742e 6164      rv_defeat.ad
+0000b430: 6428 6361 6e64 5f74 6f5f 6369 6478 5b65  d(cand_to_cidx[e
+0000b440: 305d 2c63 616e 645f 746f 5f63 6964 785b  0],cand_to_cidx[
+0000b450: 6531 5d29 0a20 2020 2020 2020 2020 2020  e1]).           
+0000b460: 2077 696e 6e65 7273 2e61 7070 656e 6428   winners.append(
+0000b470: 6369 6478 5f74 6f5f 6361 6e64 5b72 765f  cidx_to_cand[rv_
+0000b480: 6465 6665 6174 2e69 6e69 7469 616c 5f65  defeat.initial_e
+0000b490: 6c65 6d65 6e74 7328 295b 305d 5d29 0a0a  lements()[0]])..
+0000b4a0: 2020 2020 7265 7475 726e 2073 6f72 7465      return sorte
+0000b4b0: 6428 6c69 7374 2873 6574 2877 696e 6e65  d(list(set(winne
+0000b4c0: 7273 2929 290a 0a64 6566 2072 6976 6572  rs)))..def river
+0000b4d0: 5f64 6566 6561 7473 2865 6461 7461 2c20  _defeats(edata, 
+0000b4e0: 6375 7272 5f63 616e 6473 203d 204e 6f6e  curr_cands = Non
+0000b4f0: 652c 2073 7472 656e 6774 685f 6675 6e63  e, strength_func
+0000b500: 7469 6f6e 203d 204e 6f6e 6529 3a0a 2020  tion = None):.  
+0000b510: 2020 2222 220a 2020 2020 5265 7475 726e    """.    Return
+0000b520: 7320 7468 6520 5269 7665 7220 6465 6665  s the River defe
+0000b530: 6174 2072 656c 6174 696f 6e73 2070 726f  at relations pro
+0000b540: 6475 6365 6420 6279 2074 6865 2052 6976  duced by the Riv
+0000b550: 6572 2061 6c67 6f72 6974 686d 2e0a 0a20  er algorithm... 
+0000b560: 2020 202e 2e20 696d 706f 7274 616e 743a     .. important:
+0000b570: 3a0a 2020 2020 2020 2020 556e 6c69 6b65  :.        Unlike
+0000b580: 2074 6865 206f 7468 6572 2066 756e 6374   the other funct
+0000b590: 696f 6e73 2074 6861 7420 7265 7475 726e  ions that return
+0000b5a0: 2061 2073 696e 676c 6520 6465 6665 6174   a single defeat
+0000b5b0: 2072 656c 6174 696f 6e2c 2074 6869 7320   relation, this 
+0000b5c0: 7265 7475 726e 7320 6120 6c69 7374 206f  returns a list o
+0000b5d0: 6620 6465 6665 6174 2072 656c 6174 696f  f defeat relatio
+0000b5e0: 6e73 2e20 0a20 2020 2020 2020 200a 2020  ns. .        .  
+0000b5f0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+0000b600: 6564 6174 6120 2850 726f 6669 6c65 2c20  edata (Profile, 
+0000b610: 5072 6f66 696c 6557 6974 6854 6965 732c  ProfileWithTies,
+0000b620: 204d 6172 6769 6e47 7261 7068 293a 2041   MarginGraph): A
+0000b630: 6e79 2065 6c65 6374 696f 6e20 6461 7461  ny election data
+0000b640: 2074 6861 7420 6861 7320 6120 606d 6172   that has a `mar
+0000b650: 6769 6e60 206d 6574 686f 642e 200a 2020  gin` method. .  
+0000b660: 2020 2020 2020 6375 7272 5f63 616e 6473        curr_cands
+0000b670: 2028 4c69 7374 5b69 6e74 5d2c 206f 7074   (List[int], opt
+0000b680: 696f 6e61 6c29 3a20 4966 2073 6574 2c20  ional): If set, 
+0000b690: 7468 656e 2066 696e 6420 7468 6520 7769  then find the wi
+0000b6a0: 6e6e 6572 7320 666f 7220 7468 6520 7072  nners for the pr
+0000b6b0: 6f66 696c 6520 7265 7374 7269 6374 6564  ofile restricted
+0000b6c0: 2074 6f20 7468 6520 6361 6e64 6964 6174   to the candidat
+0000b6d0: 6573 2069 6e20 6060 6375 7272 5f63 616e  es in ``curr_can
+0000b6e0: 6473 6060 0a20 2020 2020 2020 2073 7472  ds``.        str
+0000b6f0: 656e 6774 685f 6675 6e63 7469 6f6e 2028  ength_function (
+0000b700: 6675 6e63 7469 6f6e 2c20 6f70 7469 6f6e  function, option
+0000b710: 616c 293a 2054 6865 2073 7472 656e 6774  al): The strengt
+0000b720: 6820 6675 6e63 7469 6f6e 2074 6f20 6265  h function to be
+0000b730: 2075 7365 6420 746f 2063 616c 6375 6c61   used to calcula
+0000b740: 7465 2074 6865 2073 7472 656e 6774 6820  te the strength 
+0000b750: 6f66 2061 2070 6174 682e 2020 2054 6865  of a path.   The
+0000b760: 2064 6566 6175 6c74 2069 7320 7468 6520   default is the 
+0000b770: 6d61 7267 696e 206d 6574 686f 6420 6f66  margin method of
+0000b780: 2060 6065 6461 7461 6060 2e20 2020 5468   ``edata``.   Th
+0000b790: 6973 206f 6e6c 7920 6d61 7474 6572 7320  is only matters 
+0000b7a0: 7768 656e 2074 6865 2062 616c 6c6f 7473  when the ballots
+0000b7b0: 2061 7265 206e 6f74 206c 696e 6561 7220   are not linear 
+0000b7c0: 6f72 6465 7273 2e20 0a0a 2020 2020 5265  orders. ..    Re
+0000b7d0: 7475 726e 733a 200a 2020 2020 2020 2020  turns: .        
+0000b7e0: 4120 6e65 7477 6f72 6b78 2044 6947 7261  A networkx DiGra
+0000b7f0: 7068 2072 6570 7265 7365 6e74 696e 6720  ph representing 
+0000b800: 7468 6520 5269 7665 7220 6465 6665 6174  the River defeat
+0000b810: 2072 656c 6174 696f 6e2e 200a 2020 2020   relation. .    
+0000b820: 2222 220a 0a20 2020 2063 616e 6469 6461  """..    candida
+0000b830: 7465 7320 3d20 6564 6174 612e 6361 6e64  tes = edata.cand
+0000b840: 6964 6174 6573 2069 6620 6375 7272 5f63  idates if curr_c
+0000b850: 616e 6473 2069 7320 4e6f 6e65 2065 6c73  ands is None els
+0000b860: 6520 6375 7272 5f63 616e 6473 2020 2020  e curr_cands    
+0000b870: 0a20 2020 2073 7472 656e 6774 685f 6675  .    strength_fu
+0000b880: 6e63 7469 6f6e 203d 2065 6461 7461 2e6d  nction = edata.m
+0000b890: 6172 6769 6e20 6966 2073 7472 656e 6774  argin if strengt
+0000b8a0: 685f 6675 6e63 7469 6f6e 2069 7320 4e6f  h_function is No
+0000b8b0: 6e65 2065 6c73 6520 7374 7265 6e67 7468  ne else strength
+0000b8c0: 5f66 756e 6374 696f 6e20 2020 200a 0a20  _function    .. 
+0000b8d0: 2020 2077 5f65 6467 6573 203d 205b 2863     w_edges = [(c
+0000b8e0: 312c 2063 322c 2073 7472 656e 6774 685f  1, c2, strength_
+0000b8f0: 6675 6e63 7469 6f6e 2863 312c 2063 3229  function(c1, c2)
+0000b900: 2920 666f 7220 6331 2069 6e20 6361 6e64  ) for c1 in cand
+0000b910: 6964 6174 6573 2066 6f72 2063 3220 696e  idates for c2 in
+0000b920: 2063 616e 6469 6461 7465 7320 6966 2063   candidates if c
+0000b930: 3120 213d 2063 3220 616e 6420 2865 6461  1 != c2 and (eda
+0000b940: 7461 2e6d 616a 6f72 6974 795f 7072 6566  ta.majority_pref
+0000b950: 6572 7328 6331 2c20 6332 2920 6f72 2065  ers(c1, c2) or e
+0000b960: 6461 7461 2e69 735f 7469 6564 2863 312c  data.is_tied(c1,
+0000b970: 2063 3229 295d 0a0a 2020 2020 7374 7265   c2))]..    stre
+0000b980: 6e67 7468 7320 3d20 736f 7274 6564 286c  ngths = sorted(l
+0000b990: 6973 7428 7365 7428 5b65 5b32 5d20 666f  ist(set([e[2] fo
+0000b9a0: 7220 6520 696e 2077 5f65 6467 6573 5d29  r e in w_edges])
+0000b9b0: 292c 2072 6576 6572 7365 3d54 7275 6529  ), reverse=True)
+0000b9c0: 0a20 2020 2073 6f72 7465 645f 6564 6765  .    sorted_edge
+0000b9d0: 7320 3d20 5b5b 6520 666f 7220 6520 696e  s = [[e for e in
+0000b9e0: 2077 5f65 6467 6573 2069 6620 655b 325d   w_edges if e[2]
+0000b9f0: 203d 3d20 735d 2066 6f72 2073 2069 6e20   == s] for s in 
+0000ba00: 7374 7265 6e67 7468 735d 0a20 2020 2074  strengths].    t
+0000ba10: 6273 203d 2070 726f 6475 6374 282a 5b70  bs = product(*[p
+0000ba20: 6572 6d75 7461 7469 6f6e 7328 6564 6765  ermutations(edge
+0000ba30: 7329 2066 6f72 2065 6467 6573 2069 6e20  s) for edges in 
+0000ba40: 736f 7274 6564 5f65 6467 6573 5d29 0a0a  sorted_edges])..
+0000ba50: 2020 2020 7269 7665 725f 6465 6665 6174      river_defeat
+0000ba60: 7320 3d20 6c69 7374 2829 0a20 2020 2066  s = list().    f
+0000ba70: 6f72 2074 6220 696e 2074 6273 3a0a 2020  or tb in tbs:.  
+0000ba80: 2020 2020 2020 6564 6765 7320 3d20 666c        edges = fl
+0000ba90: 6174 7465 6e28 7462 290a 2020 2020 2020  atten(tb).      
+0000baa0: 2020 7269 7665 725f 6465 6665 6174 203d    river_defeat =
+0000bab0: 206e 782e 4469 4772 6170 6828 2920 0a20   nx.DiGraph() . 
+0000bac0: 2020 2020 2020 2066 6f72 2065 2069 6e20         for e in 
+0000bad0: 6564 6765 733a 200a 2020 2020 2020 2020  edges: .        
+0000bae0: 2020 2020 6966 2065 5b31 5d20 6e6f 7420      if e[1] not 
+0000baf0: 696e 2072 6976 6572 5f64 6566 6561 742e  in river_defeat.
+0000bb00: 6e6f 6465 7320 6f72 206c 656e 286c 6973  nodes or len(lis
+0000bb10: 7428 7269 7665 725f 6465 6665 6174 2e69  t(river_defeat.i
+0000bb20: 6e5f 6564 6765 7328 655b 315d 2929 2920  n_edges(e[1]))) 
+0000bb30: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
+0000bb40: 2020 2020 2020 7269 7665 725f 6465 6665        river_defe
+0000bb50: 6174 2e61 6464 5f65 6467 6528 655b 305d  at.add_edge(e[0]
+0000bb60: 2c20 655b 315d 2c20 7765 6967 6874 3d65  , e[1], weight=e
+0000bb70: 5b32 5d29 0a20 2020 2020 2020 2020 2020  [2]).           
+0000bb80: 2020 2020 2069 6620 646f 6573 5f63 7265       if does_cre
+0000bb90: 6174 655f 6379 636c 6528 7269 7665 725f  ate_cycle(river_
+0000bba0: 6465 6665 6174 2c20 6529 3a0a 2020 2020  defeat, e):.    
+0000bbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bbc0: 7269 7665 725f 6465 6665 6174 2e72 656d  river_defeat.rem
+0000bbd0: 6f76 655f 6564 6765 2865 5b30 5d2c 2065  ove_edge(e[0], e
+0000bbe0: 5b31 5d29 0a20 2020 2020 2020 2020 2020  [1]).           
+0000bbf0: 200a 2020 2020 2020 2020 7269 7665 725f   .        river_
+0000bc00: 6465 6665 6174 732e 6170 7065 6e64 2872  defeats.append(r
+0000bc10: 6976 6572 5f64 6566 6561 7429 0a0a 2020  iver_defeat)..  
+0000bc20: 2020 7265 7475 726e 2072 6976 6572 5f64    return river_d
+0000bc30: 6566 6561 7473 0a0a 4076 6d28 6e61 6d65  efeats..@vm(name
+0000bc40: 3d22 5269 7665 7222 2c0a 2020 2020 736b  ="River",.    sk
+0000bc50: 6970 5f72 6567 6973 7472 6174 696f 6e3d  ip_registration=
+0000bc60: 5472 7565 290a 6465 6620 7269 7665 725f  True).def river_
+0000bc70: 7769 7468 5f74 6573 7428 6564 6174 612c  with_test(edata,
+0000bc80: 2063 7572 725f 6361 6e64 7320 3d20 4e6f   curr_cands = No
+0000bc90: 6e65 2c20 7374 7265 6e67 7468 5f66 756e  ne, strength_fun
+0000bca0: 6374 696f 6e20 3d20 4e6f 6e65 293a 2020  ction = None):  
+0000bcb0: 200a 2020 2020 2222 2246 696e 6420 7468   .    """Find th
+0000bcc0: 6520 5269 7665 7220 7769 6e6e 6572 7320  e River winners 
+0000bcd0: 7769 7468 2061 2074 6573 7420 746f 2064  with a test to d
+0000bce0: 6574 6572 6d69 6e65 6420 6966 2069 7420  etermined if it 
+0000bcf0: 7769 6c6c 2074 616b 6520 746f 6f20 6c6f  will take too lo
+0000bd00: 6e67 2074 6f20 636f 6d70 7574 6520 7468  ng to compute th
+0000bd10: 6520 5269 7665 7220 7769 6e6e 6572 732e  e River winners.
+0000bd20: 2049 6620 7468 6520 6361 6c63 756c 6174   If the calculat
+0000bd30: 696f 6e20 6f66 2074 6865 2077 696e 6e65  ion of the winne
+0000bd40: 7273 2077 696c 6c20 7461 6b65 2074 6f6f  rs will take too
+0000bd50: 206c 6f6e 672c 2072 6574 7572 6e20 4e6f   long, return No
+0000bd60: 6e65 2e20 0a20 2020 2020 2020 200a 2020  ne. .        .  
+0000bd70: 2020 2e2e 2069 6d70 6f72 7461 6e74 3a3a    .. important::
+0000bd80: 0a20 2020 2020 2020 2054 6869 7320 766f  .        This vo
+0000bd90: 7469 6e67 206d 6574 686f 6420 7468 6174  ting method that
+0000bda0: 206d 6967 6874 2072 6574 7572 6e20 4e6f   might return No
+0000bdb0: 6e65 2072 6174 6865 7220 7468 616e 2061  ne rather than a
+0000bdc0: 206c 6973 7420 6f66 2063 616e 6469 6461   list of candida
+0000bdd0: 7465 732e 2020 0a0a 2020 2020 4172 6773  tes.  ..    Args
+0000bde0: 3a0a 2020 2020 2020 2020 6564 6174 6120  :.        edata 
+0000bdf0: 2850 726f 6669 6c65 2c20 5072 6f66 696c  (Profile, Profil
+0000be00: 6557 6974 6854 6965 732c 204d 6172 6769  eWithTies, Margi
+0000be10: 6e47 7261 7068 293a 2041 6e79 2065 6c65  nGraph): Any ele
+0000be20: 6374 696f 6e20 6461 7461 2074 6861 7420  ction data that 
+0000be30: 6861 7320 6120 606d 6172 6769 6e60 206d  has a `margin` m
+0000be40: 6574 686f 642e 200a 2020 2020 2020 2020  ethod. .        
+0000be50: 6375 7272 5f63 616e 6473 2028 4c69 7374  curr_cands (List
+0000be60: 5b69 6e74 5d2c 206f 7074 696f 6e61 6c29  [int], optional)
+0000be70: 3a20 4966 2073 6574 2c20 7468 656e 2066  : If set, then f
+0000be80: 696e 6420 7468 6520 7769 6e6e 6572 7320  ind the winners 
+0000be90: 666f 7220 7468 6520 7072 6f66 696c 6520  for the profile 
+0000bea0: 7265 7374 7269 6374 6564 2074 6f20 7468  restricted to th
+0000beb0: 6520 6361 6e64 6964 6174 6573 2069 6e20  e candidates in 
+0000bec0: 6060 6375 7272 5f63 616e 6473 6060 0a20  ``curr_cands``. 
+0000bed0: 2020 2020 2020 2073 7472 656e 6774 685f         strength_
+0000bee0: 6675 6e63 7469 6f6e 2028 6675 6e63 7469  function (functi
+0000bef0: 6f6e 2c20 6f70 7469 6f6e 616c 293a 2054  on, optional): T
+0000bf00: 6865 2073 7472 656e 6774 6820 6675 6e63  he strength func
+0000bf10: 7469 6f6e 2074 6f20 6265 2075 7365 6420  tion to be used 
+0000bf20: 746f 2063 616c 6375 6c61 7465 2074 6865  to calculate the
+0000bf30: 2073 7472 656e 6774 6820 6f66 2061 2070   strength of a p
+0000bf40: 6174 682e 2020 2054 6865 2064 6566 6175  ath.   The defau
+0000bf50: 6c74 2069 7320 7468 6520 6d61 7267 696e  lt is the margin
+0000bf60: 206d 6574 686f 6420 6f66 2060 6065 6461   method of ``eda
+0000bf70: 7461 6060 2e20 2020 5468 6973 206f 6e6c  ta``.   This onl
+0000bf80: 7920 6d61 7474 6572 7320 7768 656e 2074  y matters when t
+0000bf90: 6865 2062 616c 6c6f 7473 2061 7265 206e  he ballots are n
+0000bfa0: 6f74 206c 696e 6561 7220 6f72 6465 7273  ot linear orders
+0000bfb0: 2e20 0a0a 2020 2020 5265 7475 726e 733a  . ..    Returns:
+0000bfc0: 200a 2020 2020 2020 2020 4120 736f 7274   .        A sort
+0000bfd0: 6564 206c 6973 7420 6f66 2063 616e 6469  ed list of candi
+0000bfe0: 6461 7465 732e 200a 0a20 2020 202e 2e20  dates. ..    .. 
+0000bff0: 7365 6561 6c73 6f3a 3a0a 0a20 2020 2020  seealso::..     
+0000c000: 2020 203a 6d65 7468 3a60 7072 6566 5f76     :meth:`pref_v
+0000c010: 6f74 696e 672e 6d61 7267 696e 5f62 6173  oting.margin_bas
+0000c020: 6564 5f6d 6574 686f 6473 2e72 616e 6b65  ed_methods.ranke
+0000c030: 645f 7061 6972 735f 7769 7468 5f74 6573  d_pairs_with_tes
+0000c040: 7460 2c20 3a6d 6574 683a 6070 7265 665f  t`, :meth:`pref_
+0000c050: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
+0000c060: 7365 645f 6d65 7468 6f64 732e 7269 7665  sed_methods.rive
+0000c070: 7260 0a0a 2020 2020 2222 220a 2020 2020  r`..    """.    
+0000c080: 6361 6e64 6964 6174 6573 203d 2065 6461  candidates = eda
+0000c090: 7461 2e63 616e 6469 6461 7465 7320 6966  ta.candidates if
+0000c0a0: 2063 7572 725f 6361 6e64 7320 6973 204e   curr_cands is N
+0000c0b0: 6f6e 6520 656c 7365 2063 7572 725f 6361  one else curr_ca
+0000c0c0: 6e64 7320 2020 200a 2020 2020 6369 6478  nds    .    cidx
+0000c0d0: 5f74 6f5f 6361 6e64 203d 207b 6369 6478  _to_cand = {cidx
+0000c0e0: 3a20 6320 666f 7220 6369 6478 2c20 6320  : c for cidx, c 
+0000c0f0: 696e 2065 6e75 6d65 7261 7465 2863 616e  in enumerate(can
+0000c100: 6469 6461 7465 7329 7d20 200a 2020 2020  didates)}  .    
+0000c110: 6361 6e64 5f74 6f5f 6369 6478 203d 207b  cand_to_cidx = {
+0000c120: 633a 2063 6964 7820 666f 7220 6369 6478  c: cidx for cidx
+0000c130: 2c20 6320 696e 2065 6e75 6d65 7261 7465  , c in enumerate
+0000c140: 2863 616e 6469 6461 7465 7329 7d20 200a  (candidates)}  .
+0000c150: 0a20 2020 2073 7472 656e 6774 685f 6675  .    strength_fu
+0000c160: 6e63 7469 6f6e 203d 2065 6461 7461 2e6d  nction = edata.m
+0000c170: 6172 6769 6e20 6966 2073 7472 656e 6774  argin if strengt
+0000c180: 685f 6675 6e63 7469 6f6e 2069 7320 4e6f  h_function is No
+0000c190: 6e65 2065 6c73 6520 7374 7265 6e67 7468  ne else strength
+0000c1a0: 5f66 756e 6374 696f 6e20 2020 200a 0a20  _function    .. 
+0000c1b0: 2020 2063 7720 3d20 6564 6174 612e 636f     cw = edata.co
+0000c1c0: 6e64 6f72 6365 745f 7769 6e6e 6572 2863  ndorcet_winner(c
+0000c1d0: 7572 725f 6361 6e64 733d 6375 7272 5f63  urr_cands=curr_c
+0000c1e0: 616e 6473 290a 2020 2020 2320 5261 6e6b  ands).    # Rank
+0000c1f0: 6564 2050 6169 7273 2069 7320 436f 6e64  ed Pairs is Cond
+0000c200: 6f72 6365 7420 636f 6e73 6973 7465 6e74  orcet consistent
+0000c210: 2c20 736f 2073 696d 706c 7920 7265 7475  , so simply retu
+0000c220: 726e 2074 6865 2043 6f6e 646f 7263 6574  rn the Condorcet
+0000c230: 2077 696e 6e65 7220 6966 2065 7869 7374   winner if exist
+0000c240: 730a 2020 2020 6966 2063 7720 6973 206e  s.    if cw is n
+0000c250: 6f74 204e 6f6e 653a 200a 2020 2020 2020  ot None: .      
+0000c260: 2020 7769 6e6e 6572 7320 3d20 5b63 775d    winners = [cw]
+0000c270: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+0000c280: 2020 2077 5f65 6467 6573 203d 205b 2863     w_edges = [(c
+0000c290: 312c 2063 322c 2073 7472 656e 6774 685f  1, c2, strength_
+0000c2a0: 6675 6e63 7469 6f6e 2863 312c 2063 3229  function(c1, c2)
+0000c2b0: 2920 666f 7220 6331 2069 6e20 6361 6e64  ) for c1 in cand
+0000c2c0: 6964 6174 6573 2066 6f72 2063 3220 696e  idates for c2 in
+0000c2d0: 2063 616e 6469 6461 7465 7320 0a20 2020   candidates .   
+0000c2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c2f0: 6966 2063 3120 213d 2063 3220 616e 6420  if c1 != c2 and 
+0000c300: 2865 6461 7461 2e6d 616a 6f72 6974 795f  (edata.majority_
+0000c310: 7072 6566 6572 7328 6331 2c20 6332 2920  prefers(c1, c2) 
+0000c320: 6f72 2065 6461 7461 2e69 735f 7469 6564  or edata.is_tied
+0000c330: 2863 312c 2063 3229 295d 0a20 2020 2020  (c1, c2))].     
+0000c340: 2020 2077 696e 6e65 7273 203d 206c 6973     winners = lis
+0000c350: 7428 2920 2020 2020 2020 2020 2020 200a  t()            .
+0000c360: 2020 2020 2020 2020 7374 7265 6e67 7468          strength
+0000c370: 7320 3d20 736f 7274 6564 286c 6973 7428  s = sorted(list(
+0000c380: 7365 7428 5b65 5b32 5d20 666f 7220 6520  set([e[2] for e 
+0000c390: 696e 2077 5f65 6467 6573 5d29 292c 2072  in w_edges])), r
+0000c3a0: 6576 6572 7365 3d54 7275 6529 0a20 2020  everse=True).   
+0000c3b0: 2020 2020 2073 6f72 7465 645f 6564 6765       sorted_edge
+0000c3c0: 7320 3d20 5b5b 6520 666f 7220 6520 696e  s = [[e for e in
+0000c3d0: 2077 5f65 6467 6573 2069 6620 655b 325d   w_edges if e[2]
+0000c3e0: 203d 3d20 735d 2066 6f72 2073 2069 6e20   == s] for s in 
+0000c3f0: 7374 7265 6e67 7468 735d 0a20 2020 2020  strengths].     
+0000c400: 2020 2069 6620 6e70 2e70 726f 6428 5b6d     if np.prod([m
+0000c410: 6174 682e 6661 6374 6f72 6961 6c28 6c65  ath.factorial(le
+0000c420: 6e28 6573 2929 2066 6f72 2065 7320 696e  n(es)) for es in
+0000c430: 2073 6f72 7465 645f 6564 6765 735d 2920   sorted_edges]) 
+0000c440: 3e20 3330 3030 3a20 0a20 2020 2020 2020  > 3000: .       
+0000c450: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+0000c460: 0a20 2020 2020 2020 2065 6c73 653a 200a  .        else: .
+0000c470: 2020 2020 2020 2020 2020 2020 7462 7320              tbs 
+0000c480: 3d20 7072 6f64 7563 7428 2a5b 7065 726d  = product(*[perm
+0000c490: 7574 6174 696f 6e73 2865 6467 6573 2920  utations(edges) 
+0000c4a0: 666f 7220 6564 6765 7320 696e 2073 6f72  for edges in sor
+0000c4b0: 7465 645f 6564 6765 735d 290a 2020 2020  ted_edges]).    
+0000c4c0: 2020 2020 2020 2020 666f 7220 7462 2069          for tb i
+0000c4d0: 6e20 7462 733a 0a20 2020 2020 2020 2020  n tbs:.         
+0000c4e0: 2020 2020 2020 2065 6467 6573 203d 2066         edges = f
+0000c4f0: 6c61 7474 656e 2874 6229 0a20 2020 2020  latten(tb).     
+0000c500: 2020 2020 2020 2020 2020 2072 765f 6465             rv_de
+0000c510: 6665 6174 203d 2053 504f 286c 656e 2863  feat = SPO(len(c
+0000c520: 616e 6469 6461 7465 7329 290a 2020 2020  andidates)).    
+0000c530: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000c540: 6530 2c65 312c 7320 696e 2065 6467 6573  e0,e1,s in edges
+0000c550: 3a20 0a20 2020 2020 2020 2020 2020 2020  : .             
+0000c560: 2020 2020 2020 2069 6620 6e6f 7420 7276         if not rv
+0000c570: 5f64 6566 6561 742e 505b 6361 6e64 5f74  _defeat.P[cand_t
+0000c580: 6f5f 6369 6478 5b65 315d 5d5b 6361 6e64  o_cidx[e1]][cand
+0000c590: 5f74 6f5f 6369 6478 5b65 305d 5d20 616e  _to_cidx[e0]] an
+0000c5a0: 6420 6c65 6e28 7276 5f64 6566 6561 742e  d len(rv_defeat.
+0000c5b0: 7072 6564 735b 6361 6e64 5f74 6f5f 6369  preds[cand_to_ci
+0000c5c0: 6478 5b65 315d 5d29 203d 3d20 303a 0a20  dx[e1]]) == 0:. 
+0000c5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5e0: 2020 2020 2020 2072 765f 6465 6665 6174         rv_defeat
+0000c5f0: 2e61 6464 2863 616e 645f 746f 5f63 6964  .add(cand_to_cid
+0000c600: 785b 6530 5d2c 6361 6e64 5f74 6f5f 6369  x[e0],cand_to_ci
+0000c610: 6478 5b65 315d 290a 2020 2020 2020 2020  dx[e1]).        
+0000c620: 2020 2020 2020 2020 7769 6e6e 6572 732e          winners.
+0000c630: 6170 7065 6e64 2863 6964 785f 746f 5f63  append(cidx_to_c
+0000c640: 616e 645b 7276 5f64 6566 6561 742e 696e  and[rv_defeat.in
+0000c650: 6974 6961 6c5f 656c 656d 656e 7473 2829  itial_elements()
+0000c660: 5b30 5d5d 290a 2020 2020 7265 7475 726e  [0]]).    return
+0000c670: 2073 6f72 7465 6428 6c69 7374 2873 6574   sorted(list(set
+0000c680: 2877 696e 6e65 7273 2929 290a 0a72 705f  (winners)))..rp_
+0000c690: 7462 5f70 726f 7065 7274 6965 7320 3d20  tb_properties = 
+0000c6a0: 566f 7469 6e67 4d65 7468 6f64 5072 6f70  VotingMethodProp
+0000c6b0: 6572 7469 6573 280a 2020 2020 636f 6e64  erties(.    cond
+0000c6c0: 6f72 6365 745f 7769 6e6e 6572 3d54 7275  orcet_winner=Tru
+0000c6d0: 652c 200a 2020 2020 636f 6e64 6f72 6365  e, .    condorce
+0000c6e0: 745f 6c6f 7365 723d 5472 7565 2c0a 2020  t_loser=True,.  
+0000c6f0: 2020 7061 7265 746f 5f64 6f6d 696e 616e    pareto_dominan
+0000c700: 6365 3d54 7275 652c 200a 2020 2020 290a  ce=True, .    ).
+0000c710: 4076 6d28 6e61 6d65 3d22 5269 7665 7220  @vm(name="River 
+0000c720: 5442 222c 0a20 2020 2070 726f 7065 7274  TB",.    propert
+0000c730: 6965 733d 7270 5f74 625f 7072 6f70 6572  ies=rp_tb_proper
+0000c740: 7469 6573 2c0a 2020 2020 696e 7075 745f  ties,.    input_
+0000c750: 7479 7065 733d 5b45 6c65 6374 696f 6e54  types=[ElectionT
+0000c760: 7970 6573 2e50 524f 4649 4c45 2c20 456c  ypes.PROFILE, El
+0000c770: 6563 7469 6f6e 5479 7065 732e 5052 4f46  ectionTypes.PROF
+0000c780: 494c 455f 5749 5448 5f54 4945 532c 2045  ILE_WITH_TIES, E
+0000c790: 6c65 6374 696f 6e54 7970 6573 2e4d 4152  lectionTypes.MAR
+0000c7a0: 4749 4e5f 4752 4150 485d 290a 6465 6620  GIN_GRAPH]).def 
+0000c7b0: 7269 7665 725f 7462 2865 6461 7461 2c20  river_tb(edata, 
+0000c7c0: 6375 7272 5f63 616e 6473 203d 204e 6f6e  curr_cands = Non
+0000c7d0: 652c 2074 6965 5f62 7265 616b 6572 203d  e, tie_breaker =
+0000c7e0: 204e 6f6e 652c 2073 7472 656e 6774 685f   None, strength_
+0000c7f0: 6675 6e63 7469 6f6e 203d 204e 6f6e 6529  function = None)
+0000c800: 3a20 2020 0a20 2020 2022 2222 0a20 2020  :   .    """.   
+0000c810: 2052 6976 6572 2077 6974 6820 6120 6669   River with a fi
+0000c820: 7865 6420 6c69 6e65 6172 206f 7264 6572  xed linear order
+0000c830: 206f 6e20 7468 6520 6361 6e64 6964 6174   on the candidat
+0000c840: 6573 2074 6f20 6272 6561 6b20 616e 7920  es to break any 
+0000c850: 7469 6573 2069 6e20 7468 6520 6d61 7267  ties in the marg
+0000c860: 696e 732e 2020 5369 6e63 6520 7468 6520  ins.  Since the 
+0000c870: 7469 655f 6272 6561 6b65 7220 6973 2061  tie_breaker is a
+0000c880: 206c 696e 6561 7220 6f72 6465 722c 2074   linear order, t
+0000c890: 6869 7320 6d65 7468 6f64 2069 7320 7265  his method is re
+0000c8a0: 736f 6c75 7465 2e20 2020 0a0a 2020 2020  solute.   ..    
+0000c8b0: 4172 6773 3a0a 2020 2020 2020 2020 6564  Args:.        ed
+0000c8c0: 6174 6120 2850 726f 6669 6c65 2c20 5072  ata (Profile, Pr
+0000c8d0: 6f66 696c 6557 6974 6854 6965 732c 204d  ofileWithTies, M
+0000c8e0: 6172 6769 6e47 7261 7068 293a 2041 6e79  arginGraph): Any
+0000c8f0: 2065 6c65 6374 696f 6e20 6461 7461 2074   election data t
+0000c900: 6861 7420 6861 7320 6120 606d 6172 6769  hat has a `margi
+0000c910: 6e60 206d 6574 686f 642e 200a 2020 2020  n` method. .    
+0000c920: 2020 2020 6375 7272 5f63 616e 6473 2028      curr_cands (
+0000c930: 4c69 7374 5b69 6e74 5d2c 206f 7074 696f  List[int], optio
+0000c940: 6e61 6c29 3a20 4966 2073 6574 2c20 7468  nal): If set, th
+0000c950: 656e 2066 696e 6420 7468 6520 7769 6e6e  en find the winn
+0000c960: 6572 7320 666f 7220 7468 6520 7072 6f66  ers for the prof
+0000c970: 696c 6520 7265 7374 7269 6374 6564 2074  ile restricted t
+0000c980: 6f20 7468 6520 6361 6e64 6964 6174 6573  o the candidates
+0000c990: 2069 6e20 6060 6375 7272 5f63 616e 6473   in ``curr_cands
+0000c9a0: 6060 0a20 2020 2020 2020 2074 6965 5f62  ``.        tie_b
+0000c9b0: 7265 616b 6572 2028 4c69 7374 5b69 6e74  reaker (List[int
+0000c9c0: 5d2c 206f 7074 696f 6e61 6c29 3a20 4120  ], optional): A 
+0000c9d0: 6c69 6e65 6172 206f 7264 6572 206f 6e20  linear order on 
+0000c9e0: 7468 6520 6361 6e64 6964 6174 6573 2e20  the candidates. 
+0000c9f0: 2049 6620 6e6f 7420 7365 742c 2074 6865   If not set, the
+0000ca00: 6e20 7468 6520 6361 6e64 6964 6174 6573  n the candidates
+0000ca10: 2061 7265 2073 6f72 7465 6420 696e 2061   are sorted in a
+0000ca20: 7363 656e 6469 6e67 206f 7264 6572 2e0a  scending order..
+0000ca30: 2020 2020 2020 2020 7374 7265 6e67 7468          strength
+0000ca40: 5f66 756e 6374 696f 6e20 2866 756e 6374  _function (funct
+0000ca50: 696f 6e2c 206f 7074 696f 6e61 6c29 3a20  ion, optional): 
+0000ca60: 5468 6520 7374 7265 6e67 7468 2066 756e  The strength fun
+0000ca70: 6374 696f 6e20 746f 2062 6520 7573 6564  ction to be used
+0000ca80: 2074 6f20 6361 6c63 756c 6174 6520 7468   to calculate th
+0000ca90: 6520 7374 7265 6e67 7468 206f 6620 6120  e strength of a 
+0000caa0: 7061 7468 2e20 2020 5468 6520 6465 6661  path.   The defa
+0000cab0: 756c 7420 6973 2074 6865 206d 6172 6769  ult is the margi
+0000cac0: 6e20 6d65 7468 6f64 206f 6620 6060 6564  n method of ``ed
+0000cad0: 6174 6160 602e 2020 2054 6869 7320 6f6e  ata``.   This on
+0000cae0: 6c79 206d 6174 7465 7273 2077 6865 6e20  ly matters when 
+0000caf0: 7468 6520 6261 6c6c 6f74 7320 6172 6520  the ballots are 
+0000cb00: 6e6f 7420 6c69 6e65 6172 206f 7264 6572  not linear order
+0000cb10: 732e 200a 0a20 2020 2052 6574 7572 6e73  s. ..    Returns
+0000cb20: 3a20 0a20 2020 2020 2020 2041 2073 6f72  : .        A sor
+0000cb30: 7465 6420 6c69 7374 206f 6620 6361 6e64  ted list of cand
+0000cb40: 6964 6174 6573 2e20 0a0a 2020 2020 2222  idates. ..    ""
+0000cb50: 220a 2020 2020 6361 6e64 6964 6174 6573  ".    candidates
+0000cb60: 203d 2065 6461 7461 2e63 616e 6469 6461   = edata.candida
+0000cb70: 7465 7320 6966 2063 7572 725f 6361 6e64  tes if curr_cand
+0000cb80: 7320 6973 204e 6f6e 6520 656c 7365 2063  s is None else c
+0000cb90: 7572 725f 6361 6e64 7320 2020 200a 2020  urr_cands    .  
+0000cba0: 2020 6369 6478 5f74 6f5f 6361 6e64 203d    cidx_to_cand =
+0000cbb0: 207b 6369 6478 3a20 6320 666f 7220 6369   {cidx: c for ci
+0000cbc0: 6478 2c20 6320 696e 2065 6e75 6d65 7261  dx, c in enumera
+0000cbd0: 7465 2863 616e 6469 6461 7465 7329 7d20  te(candidates)} 
+0000cbe0: 200a 2020 2020 6361 6e64 5f74 6f5f 6369   .    cand_to_ci
+0000cbf0: 6478 203d 207b 633a 2063 6964 7820 666f  dx = {c: cidx fo
+0000cc00: 7220 6369 6478 2c20 6320 696e 2065 6e75  r cidx, c in enu
+0000cc10: 6d65 7261 7465 2863 616e 6469 6461 7465  merate(candidate
+0000cc20: 7329 7d20 200a 2020 2020 7374 7265 6e67  s)}  .    streng
+0000cc30: 7468 5f66 756e 6374 696f 6e20 3d20 6564  th_function = ed
+0000cc40: 6174 612e 6d61 7267 696e 2069 6620 7374  ata.margin if st
+0000cc50: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
+0000cc60: 6973 204e 6f6e 6520 656c 7365 2073 7472  is None else str
+0000cc70: 656e 6774 685f 6675 6e63 7469 6f6e 2020  ength_function  
+0000cc80: 2020 0a0a 2020 2020 7462 5f72 616e 6b69    ..    tb_ranki
+0000cc90: 6e67 203d 2074 6965 5f62 7265 616b 6572  ng = tie_breaker
+0000cca0: 2069 6620 7469 655f 6272 6561 6b65 7220   if tie_breaker 
+0000ccb0: 6973 206e 6f74 204e 6f6e 6520 656c 7365  is not None else
+0000ccc0: 2073 6f72 7465 6428 6c69 7374 2863 616e   sorted(list(can
+0000ccd0: 6469 6461 7465 7329 290a 0a20 2020 2063  didates))..    c
+0000cce0: 7720 3d20 6564 6174 612e 636f 6e64 6f72  w = edata.condor
+0000ccf0: 6365 745f 7769 6e6e 6572 2863 7572 725f  cet_winner(curr_
+0000cd00: 6361 6e64 733d 6375 7272 5f63 616e 6473  cands=curr_cands
+0000cd10: 290a 2020 2020 2320 5269 7665 7220 6973  ).    # River is
+0000cd20: 2043 6f6e 646f 7263 6574 2063 6f6e 7369   Condorcet consi
+0000cd30: 7374 656e 742c 2073 6f20 7369 6d70 6c79  stent, so simply
+0000cd40: 2072 6574 7572 6e20 7468 6520 436f 6e64   return the Cond
+0000cd50: 6f72 6365 7420 7769 6e6e 6572 2069 6620  orcet winner if 
+0000cd60: 6578 6973 7473 0a20 2020 2069 6620 6377  exists.    if cw
+0000cd70: 2069 7320 6e6f 7420 4e6f 6e65 3a20 0a20   is not None: . 
+0000cd80: 2020 2020 2020 2077 696e 6e65 7273 203d         winners =
+0000cd90: 205b 6377 5d0a 2020 2020 656c 7365 3a0a   [cw].    else:.
+0000cda0: 2020 2020 2020 2020 775f 6564 6765 7320          w_edges 
+0000cdb0: 3d20 5b28 6331 2c20 6332 2c20 7374 7265  = [(c1, c2, stre
+0000cdc0: 6e67 7468 5f66 756e 6374 696f 6e28 6331  ngth_function(c1
+0000cdd0: 2c20 6332 2929 2066 6f72 2063 3120 696e  , c2)) for c1 in
+0000cde0: 2063 616e 6469 6461 7465 7320 666f 7220   candidates for 
+0000cdf0: 6332 2069 6e20 6361 6e64 6964 6174 6573  c2 in candidates
+0000ce00: 2069 6620 6331 2021 3d20 6332 2061 6e64   if c1 != c2 and
+0000ce10: 2028 6564 6174 612e 6d61 6a6f 7269 7479   (edata.majority
+0000ce20: 5f70 7265 6665 7273 2863 312c 2063 3229  _prefers(c1, c2)
+0000ce30: 206f 7220 6564 6174 612e 6973 5f74 6965   or edata.is_tie
+0000ce40: 6428 6331 2c20 6332 2929 5d0a 2020 2020  d(c1, c2))].    
+0000ce50: 2020 2020 7769 6e6e 6572 7320 3d20 6c69      winners = li
+0000ce60: 7374 2829 2020 0a20 2020 2020 2020 2073  st()  .        s
+0000ce70: 7472 656e 6774 6873 203d 2073 6f72 7465  trengths = sorte
+0000ce80: 6428 6c69 7374 2873 6574 285b 655b 325d  d(list(set([e[2]
+0000ce90: 2066 6f72 2065 2069 6e20 775f 6564 6765   for e in w_edge
+0000cea0: 735d 2929 2c20 7265 7665 7273 653d 5472  s])), reverse=Tr
+0000ceb0: 7565 290a 0a20 2020 2020 2020 2072 765f  ue)..        rv_
+0000cec0: 6465 6665 6174 203d 2053 504f 286c 656e  defeat = SPO(len
+0000ced0: 2863 616e 6469 6461 7465 7329 290a 0a20  (candidates)).. 
+0000cee0: 2020 2020 2020 2066 6f72 2073 2069 6e20         for s in 
+0000cef0: 7374 7265 6e67 7468 733a 200a 2020 2020  strengths: .    
+0000cf00: 2020 2020 2020 2020 6564 6765 7320 3d20          edges = 
+0000cf10: 5b65 2066 6f72 2065 2069 6e20 775f 6564  [e for e in w_ed
+0000cf20: 6765 7320 6966 2065 5b32 5d20 3d3d 2073  ges if e[2] == s
+0000cf30: 5d0a 2020 2020 2020 2020 2020 2020 0a20  ].            . 
+0000cf40: 2020 2020 2020 2020 2020 2023 2062 7265             # bre
+0000cf50: 616b 2074 6965 7320 7573 696e 6720 7468  ak ties using th
+0000cf60: 6520 6c65 7869 636f 6772 6170 6869 6320  e lexicographic 
+0000cf70: 6f72 6465 7269 6e67 206f 6e20 7475 706c  ordering on tupl
+0000cf80: 6573 2067 6976 656e 2074 625f 7261 6e6b  es given tb_rank
+0000cf90: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
+0000cfa0: 736f 7274 6564 5f65 6467 6573 203d 2073  sorted_edges = s
+0000cfb0: 6f72 7465 6428 6564 6765 732c 206b 6579  orted(edges, key
+0000cfc0: 203d 206c 616d 6264 6120 653a 2028 7462   = lambda e: (tb
+0000cfd0: 5f72 616e 6b69 6e67 2e69 6e64 6578 2865  _ranking.index(e
+0000cfe0: 5b30 5d29 2c20 7462 5f72 616e 6b69 6e67  [0]), tb_ranking
+0000cff0: 2e69 6e64 6578 2865 5b31 5d29 292c 2072  .index(e[1])), r
+0000d000: 6576 6572 7365 3d46 616c 7365 290a 2020  everse=False).  
+0000d010: 2020 2020 2020 2020 2020 666f 7220 6530            for e0
+0000d020: 2c65 312c 7320 696e 2073 6f72 7465 645f  ,e1,s in sorted_
+0000d030: 6564 6765 733a 200a 2020 2020 2020 2020  edges: .        
+0000d040: 2020 2020 2020 2020 6966 206e 6f74 2072          if not r
+0000d050: 765f 6465 6665 6174 2e50 5b63 616e 645f  v_defeat.P[cand_
+0000d060: 746f 5f63 6964 785b 6531 5d5d 5b63 616e  to_cidx[e1]][can
+0000d070: 645f 746f 5f63 6964 785b 6530 5d5d 2061  d_to_cidx[e0]] a
+0000d080: 6e64 206c 656e 2872 765f 6465 6665 6174  nd len(rv_defeat
+0000d090: 2e70 7265 6473 5b63 616e 645f 746f 5f63  .preds[cand_to_c
+0000d0a0: 6964 785b 6531 5d5d 2920 3d3d 2030 3a0a  idx[e1]]) == 0:.
 0000d0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0d0: 736f 7274 6564 5f6d 6174 6368 6573 203d  sorted_matches =
-0000d0e0: 205b 2861 2c20 632c 2073 2920 666f 7220   [(a, c, s) for 
-0000d0f0: 612c 2063 2c20 7320 696e 2073 6f72 7465  a, c, s in sorte
-0000d100: 645f 6d61 7463 6865 7320 6966 2061 2021  d_matches if a !
-0000d110: 3d20 6220 616e 6420 6320 213d 2062 5d2c  = b and c != b],
-0000d120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d150: 2020 2020 2020 2020 2020 2020 6d65 6d5f              mem_
-0000d160: 7376 5f77 696e 6e65 7273 203d 206d 656d  sv_winners = mem
-0000d170: 5f73 765f 7769 6e6e 6572 7329 0a20 2020  _sv_winners).   
-0000d180: 2020 2020 2020 2020 2020 2020 206d 656d               mem
-0000d190: 5f73 765f 7769 6e6e 6572 735b 6361 6e64  _sv_winners[cand
-0000d1a0: 735f 6d69 6e75 735f 625f 6b65 795d 203d  s_minus_b_key] =
-0000d1b0: 2077 730a 2020 2020 2020 2020 2020 2020   ws.            
-0000d1c0: 656c 7365 3a20 0a20 2020 2020 2020 2020  else: .         
-0000d1d0: 2020 2020 2020 2077 7320 3d20 6d65 6d5f         ws = mem_
-0000d1e0: 7376 5f77 696e 6e65 7273 5b63 616e 6473  sv_winners[cands
-0000d1f0: 5f6d 696e 7573 5f62 5f6b 6579 5d0a 2020  _minus_b_key].  
-0000d200: 2020 2020 2020 2020 2020 6966 2061 2069            if a i
-0000d210: 6e20 7773 3a0a 2020 2020 2020 2020 2020  n ws:.          
-0000d220: 2020 2020 2020 7376 5f77 696e 6e65 7273        sv_winners
-0000d230: 2e61 7070 656e 6428 6129 0a20 2020 2020  .append(a).     
-0000d240: 2020 2020 2020 2020 2020 206d 6172 6769             margi
-0000d250: 6e5f 7769 746e 6573 7369 6e67 5f77 696e  n_witnessing_win
-0000d260: 203d 2073 0a0a 2020 2020 7265 7475 726e   = s..    return
-0000d270: 2073 765f 7769 6e6e 6572 732c 206d 656d   sv_winners, mem
-0000d280: 5f73 765f 7769 6e6e 6572 730a 2020 2020  _sv_winners.    
-0000d290: 0a0a 4076 6d28 6e61 6d65 203d 2022 5369  ..@vm(name = "Si
-0000d2a0: 6d70 6c65 2053 7461 626c 6520 566f 7469  mple Stable Voti
-0000d2b0: 6e67 2229 0a64 6566 205f 7369 6d70 6c65  ng").def _simple
-0000d2c0: 5f73 7461 626c 655f 766f 7469 6e67 5f77  _stable_voting_w
-0000d2d0: 6974 685f 636f 6e64 6f72 6365 745f 6368  ith_condorcet_ch
-0000d2e0: 6563 6b28 0a20 2020 2065 6461 7461 2c20  eck(.    edata, 
-0000d2f0: 0a20 2020 2063 7572 725f 6361 6e64 7320  .    curr_cands 
-0000d300: 3d20 4e6f 6e65 2c20 0a20 2020 2073 7472  = None, .    str
-0000d310: 656e 6774 685f 6675 6e63 7469 6f6e 203d  ength_function =
-0000d320: 204e 6f6e 6529 3a20 0a20 2020 2022 2222   None): .    """
-0000d330: 5369 6d70 6c65 2053 7461 626c 6520 566f  Simple Stable Vo
-0000d340: 7469 6e67 2069 7320 436f 6e64 6f72 6365  ting is Condorce
-0000d350: 7420 636f 6e73 6973 7465 6e74 2e20 2020  t consistent.   
-0000d360: 4974 2069 7320 6661 7374 6572 2074 6f20  It is faster to 
-0000d370: 736b 6970 2065 7865 6375 7469 6e67 2074  skip executing t
-0000d380: 6865 2072 6563 7572 7369 7665 2061 6c67  he recursive alg
-0000d390: 6f72 6974 686d 2077 6865 6e20 7468 6572  orithm when ther
-0000d3a0: 6520 6973 2061 2043 6f6e 646f 7263 6574  e is a Condorcet
-0000d3b0: 2077 696e 6e65 7246 6972 7374 2063 6865   winnerFirst che
-0000d3c0: 636b 2069 6620 7468 6572 6520 6973 2061  ck if there is a
-0000d3d0: 2043 6f6e 646f 7263 6574 2077 696e 6e65   Condorcet winne
-0000d3e0: 722e 2020 4966 2073 6f2c 2072 6574 7572  r.  If so, retur
-0000d3f0: 6e20 7468 6520 436f 6e64 6f72 6365 7420  n the Condorcet 
-0000d400: 7769 6e6e 6572 2c20 6f74 6865 7277 6973  winner, otherwis
-0000d410: 6520 6669 6e64 2074 6865 2053 696d 706c  e find the Simpl
-0000d420: 6520 5374 6162 6c65 2056 6f74 696e 6720  e Stable Voting 
-0000d430: 7769 6e6e 6572 2075 7369 6e67 205f 7369  winner using _si
-0000d440: 6d70 6c65 5f73 7461 626c 655f 766f 7469  mple_stable_voti
-0000d450: 6e67 0a0a 2020 2020 4172 6773 3a0a 2020  ng..    Args:.  
-0000d460: 2020 2020 2020 6564 6174 6120 2850 726f        edata (Pro
-0000d470: 6669 6c65 2c20 5072 6f66 696c 6557 6974  file, ProfileWit
-0000d480: 6854 6965 732c 204d 6172 6769 6e47 7261  hTies, MarginGra
-0000d490: 7068 293a 2041 6e79 2065 6c65 6374 696f  ph): Any electio
-0000d4a0: 6e20 6461 7461 2074 6861 7420 6861 7320  n data that has 
-0000d4b0: 6120 606d 6172 6769 6e60 206d 6574 686f  a `margin` metho
-0000d4c0: 642e 200a 2020 2020 2020 2020 6375 7272  d. .        curr
-0000d4d0: 5f63 616e 6473 2028 4c69 7374 5b69 6e74  _cands (List[int
-0000d4e0: 5d2c 206f 7074 696f 6e61 6c29 3a20 4966  ], optional): If
-0000d4f0: 2073 6574 2c20 7468 656e 2066 696e 6420   set, then find 
-0000d500: 7468 6520 7769 6e6e 6572 7320 666f 7220  the winners for 
-0000d510: 7468 6520 7072 6f66 696c 6520 7265 7374  the profile rest
-0000d520: 7269 6374 6564 2074 6f20 7468 6520 6361  ricted to the ca
-0000d530: 6e64 6964 6174 6573 2069 6e20 6060 6375  ndidates in ``cu
-0000d540: 7272 5f63 616e 6473 6060 0a20 2020 2020  rr_cands``.     
-0000d550: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
-0000d560: 7469 6f6e 2028 6675 6e63 7469 6f6e 2c20  tion (function, 
-0000d570: 6f70 7469 6f6e 616c 293a 2054 6865 2073  optional): The s
-0000d580: 7472 656e 6774 6820 6675 6e63 7469 6f6e  trength function
-0000d590: 2074 6f20 6265 2075 7365 6420 746f 2063   to be used to c
-0000d5a0: 616c 6375 6c61 7465 2074 6865 2073 7472  alculate the str
-0000d5b0: 656e 6774 6820 6f66 2061 2070 6174 682e  ength of a path.
-0000d5c0: 2020 2054 6865 2064 6566 6175 6c74 2069     The default i
-0000d5d0: 7320 7468 6520 6d61 7267 696e 206d 6574  s the margin met
-0000d5e0: 686f 6420 6f66 2060 6065 6461 7461 6060  hod of ``edata``
-0000d5f0: 2e20 2020 5468 6973 206f 6e6c 7920 6d61  .   This only ma
-0000d600: 7474 6572 7320 7768 656e 2074 6865 2062  tters when the b
-0000d610: 616c 6c6f 7473 2061 7265 206e 6f74 206c  allots are not l
-0000d620: 696e 6561 7220 6f72 6465 7273 2e20 0a0a  inear orders. ..
-0000d630: 2020 2020 5265 7475 726e 733a 200a 2020      Returns: .  
-0000d640: 2020 2020 2020 4120 736f 7274 6564 206c        A sorted l
-0000d650: 6973 7420 6f66 2063 616e 6469 6461 7465  ist of candidate
-0000d660: 732e 200a 0a20 2020 2022 2222 0a20 2020  s. ..    """.   
-0000d670: 200a 2020 2020 6377 203d 2065 6461 7461   .    cw = edata
-0000d680: 2e63 6f6e 646f 7263 6574 5f77 696e 6e65  .condorcet_winne
-0000d690: 7228 6375 7272 5f63 616e 6473 203d 2063  r(curr_cands = c
-0000d6a0: 7572 725f 6361 6e64 7329 0a20 2020 2069  urr_cands).    i
-0000d6b0: 6620 6377 2069 7320 6e6f 7420 4e6f 6e65  f cw is not None
-0000d6c0: 3a20 0a20 2020 2020 2020 2072 6574 7572  : .        retur
-0000d6d0: 6e20 5b63 775d 0a20 2020 2065 6c73 653a  n [cw].    else:
-0000d6e0: 200a 2020 2020 2020 2020 6375 7272 5f63   .        curr_c
-0000d6f0: 616e 6473 203d 2065 6461 7461 2e63 616e  ands = edata.can
-0000d700: 6469 6461 7465 7320 6966 2063 7572 725f  didates if curr_
-0000d710: 6361 6e64 7320 6973 204e 6f6e 6520 656c  cands is None el
-0000d720: 7365 2063 7572 725f 6361 6e64 730a 2020  se curr_cands.  
-0000d730: 2020 2020 2020 7374 7265 6e67 7468 5f66        strength_f
-0000d740: 756e 6374 696f 6e20 3d20 6564 6174 612e  unction = edata.
-0000d750: 6d61 7267 696e 2069 6620 7374 7265 6e67  margin if streng
-0000d760: 7468 5f66 756e 6374 696f 6e20 6973 204e  th_function is N
-0000d770: 6f6e 6520 656c 7365 2073 7472 656e 6774  one else strengt
-0000d780: 685f 6675 6e63 7469 6f6e 2020 0a0a 2020  h_function  ..  
-0000d790: 2020 2020 2020 6d61 7463 6865 7320 3d20        matches = 
-0000d7a0: 5b28 612c 2062 2c20 7374 7265 6e67 7468  [(a, b, strength
-0000d7b0: 5f66 756e 6374 696f 6e28 612c 2062 2929  _function(a, b))
-0000d7c0: 2066 6f72 2061 2069 6e20 6375 7272 5f63   for a in curr_c
-0000d7d0: 616e 6473 2066 6f72 2062 2069 6e20 6375  ands for b in cu
-0000d7e0: 7272 5f63 616e 6473 2069 6620 6120 213d  rr_cands if a !=
-0000d7f0: 2062 5d0a 2020 2020 2020 2020 736f 7274   b].        sort
-0000d800: 6564 5f6d 6174 6368 6573 203d 2073 6f72  ed_matches = sor
-0000d810: 7465 6428 6d61 7463 6865 732c 2072 6576  ted(matches, rev
-0000d820: 6572 7365 3d54 7275 652c 206b 6579 3d6c  erse=True, key=l
-0000d830: 616d 6264 6120 6d5f 775f 7765 6967 6874  ambda m_w_weight
-0000d840: 3a20 6d5f 775f 7765 6967 6874 5b32 5d29  : m_w_weight[2])
-0000d850: 0a20 2020 200a 2020 2020 2020 2020 7265  .    .        re
-0000d860: 7475 726e 2073 6f72 7465 6428 5f73 696d  turn sorted(_sim
-0000d870: 706c 655f 7374 6162 6c65 5f76 6f74 696e  ple_stable_votin
-0000d880: 6728 6375 7272 5f63 616e 6473 203d 2063  g(curr_cands = c
-0000d890: 7572 725f 6361 6e64 732c 200a 2020 2020  urr_cands, .    
-0000d8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8c0: 2020 2020 2020 2020 736f 7274 6564 5f6d          sorted_m
-0000d8d0: 6174 6368 6573 203d 2073 6f72 7465 645f  atches = sorted_
-0000d8e0: 6d61 7463 6865 732c 0a20 2020 2020 2020  matches,.       
-0000d8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d910: 2020 2020 206d 656d 5f73 765f 7769 6e6e       mem_sv_winn
-0000d920: 6572 7320 3d20 7b7d 295b 305d 290a 0a0a  ers = {})[0])...
-0000d930: 6465 6620 5f73 696d 706c 655f 7374 6162  def _simple_stab
-0000d940: 6c65 5f76 6f74 696e 675f 6261 7369 6328  le_voting_basic(
-0000d950: 6564 6174 612c 2063 7572 725f 6361 6e64  edata, curr_cand
-0000d960: 7320 3d20 4e6f 6e65 2c20 7374 7265 6e67  s = None, streng
-0000d970: 7468 5f66 756e 6374 696f 6e20 3d20 4e6f  th_function = No
-0000d980: 6e65 293a 200a 2020 2020 2222 2249 6d70  ne): .    """Imp
-0000d990: 6c65 6d65 6e74 6174 696f 6e20 6f66 2053  lementation of S
-0000d9a0: 696d 706c 6520 5374 6162 6c65 2056 6f74  imple Stable Vot
-0000d9b0: 696e 6720 6672 6f6d 2068 7474 7073 3a2f  ing from https:/
-0000d9c0: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
-0000d9d0: 3130 382e 3030 3534 322e 200a 0a20 2020  108.00542. ..   
-0000d9e0: 2041 7267 733a 0a20 2020 2020 2020 2065   Args:.        e
-0000d9f0: 6461 7461 2028 5072 6f66 696c 652c 2050  data (Profile, P
-0000da00: 726f 6669 6c65 5769 7468 5469 6573 2c20  rofileWithTies, 
-0000da10: 4d61 7267 696e 4772 6170 6829 3a20 416e  MarginGraph): An
-0000da20: 7920 656c 6563 7469 6f6e 2064 6174 6120  y election data 
-0000da30: 7468 6174 2068 6173 2061 2060 6d61 7267  that has a `marg
-0000da40: 696e 6020 6d65 7468 6f64 2e20 0a20 2020  in` method. .   
-0000da50: 2020 2020 2063 7572 725f 6361 6e64 7320       curr_cands 
-0000da60: 284c 6973 745b 696e 745d 2c20 6f70 7469  (List[int], opti
-0000da70: 6f6e 616c 293a 2049 6620 7365 742c 2074  onal): If set, t
-0000da80: 6865 6e20 6669 6e64 2074 6865 2077 696e  hen find the win
-0000da90: 6e65 7273 2066 6f72 2074 6865 2070 726f  ners for the pro
-0000daa0: 6669 6c65 2072 6573 7472 6963 7465 6420  file restricted 
-0000dab0: 746f 2074 6865 2063 616e 6469 6461 7465  to the candidate
-0000dac0: 7320 696e 2060 6063 7572 725f 6361 6e64  s in ``curr_cand
-0000dad0: 7360 600a 2020 2020 2020 2020 7374 7265  s``.        stre
-0000dae0: 6e67 7468 5f66 756e 6374 696f 6e20 2866  ngth_function (f
-0000daf0: 756e 6374 696f 6e2c 206f 7074 696f 6e61  unction, optiona
-0000db00: 6c29 3a20 5468 6520 7374 7265 6e67 7468  l): The strength
-0000db10: 2066 756e 6374 696f 6e20 746f 2062 6520   function to be 
-0000db20: 7573 6564 2074 6f20 6361 6c63 756c 6174  used to calculat
-0000db30: 6520 7468 6520 7374 7265 6e67 7468 206f  e the strength o
-0000db40: 6620 6120 7061 7468 2e20 2020 5468 6520  f a path.   The 
-0000db50: 6465 6661 756c 7420 6973 2074 6865 206d  default is the m
-0000db60: 6172 6769 6e20 6d65 7468 6f64 206f 6620  argin method of 
-0000db70: 6060 6564 6174 6160 602e 2020 2054 6869  ``edata``.   Thi
-0000db80: 7320 6f6e 6c79 206d 6174 7465 7273 2077  s only matters w
-0000db90: 6865 6e20 7468 6520 6261 6c6c 6f74 7320  hen the ballots 
-0000dba0: 6172 6520 6e6f 7420 6c69 6e65 6172 206f  are not linear o
-0000dbb0: 7264 6572 732e 200a 0a20 2020 2052 6574  rders. ..    Ret
-0000dbc0: 7572 6e73 3a20 0a20 2020 2020 2020 2041  urns: .        A
-0000dbd0: 2073 6f72 7465 6420 6c69 7374 206f 6620   sorted list of 
-0000dbe0: 6361 6e64 6964 6174 6573 2e20 0a0a 2020  candidates. ..  
-0000dbf0: 2020 2222 220a 2020 2020 0a20 2020 2063    """.    .    c
-0000dc00: 7572 725f 6361 6e64 7320 3d20 6564 6174  urr_cands = edat
-0000dc10: 612e 6361 6e64 6964 6174 6573 2069 6620  a.candidates if 
-0000dc20: 6375 7272 5f63 616e 6473 2069 7320 4e6f  curr_cands is No
-0000dc30: 6e65 2065 6c73 6520 6375 7272 5f63 616e  ne else curr_can
-0000dc40: 6473 0a20 2020 2073 7472 656e 6774 685f  ds.    strength_
-0000dc50: 6675 6e63 7469 6f6e 203d 2065 6461 7461  function = edata
-0000dc60: 2e6d 6172 6769 6e20 6966 2073 7472 656e  .margin if stren
-0000dc70: 6774 685f 6675 6e63 7469 6f6e 2069 7320  gth_function is 
-0000dc80: 4e6f 6e65 2065 6c73 6520 7374 7265 6e67  None else streng
-0000dc90: 7468 5f66 756e 6374 696f 6e20 200a 0a20  th_function  .. 
-0000dca0: 2020 206d 6174 6368 6573 203d 205b 2861     matches = [(a
-0000dcb0: 2c20 622c 2073 7472 656e 6774 685f 6675  , b, strength_fu
-0000dcc0: 6e63 7469 6f6e 2861 2c20 6229 2920 666f  nction(a, b)) fo
-0000dcd0: 7220 6120 696e 2063 7572 725f 6361 6e64  r a in curr_cand
-0000dce0: 7320 666f 7220 6220 696e 2063 7572 725f  s for b in curr_
-0000dcf0: 6361 6e64 7320 6966 2061 2021 3d20 625d  cands if a != b]
-0000dd00: 0a20 2020 2073 6f72 7465 645f 6d61 7463  .    sorted_matc
-0000dd10: 6865 7320 3d20 736f 7274 6564 286d 6174  hes = sorted(mat
-0000dd20: 6368 6573 2c20 7265 7665 7273 653d 5472  ches, reverse=Tr
-0000dd30: 7565 2c20 6b65 793d 6c61 6d62 6461 206d  ue, key=lambda m
-0000dd40: 5f77 5f77 6569 6768 743a 206d 5f77 5f77  _w_weight: m_w_w
-0000dd50: 6569 6768 745b 325d 290a 2020 2020 0a20  eight[2]).    . 
-0000dd60: 2020 2072 6574 7572 6e20 736f 7274 6564     return sorted
-0000dd70: 285f 7369 6d70 6c65 5f73 7461 626c 655f  (_simple_stable_
-0000dd80: 766f 7469 6e67 2863 7572 725f 6361 6e64  voting(curr_cand
-0000dd90: 7320 3d20 6375 7272 5f63 616e 6473 2c20  s = curr_cands, 
-0000dda0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ddb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ddc0: 2020 2020 2020 2020 2073 6f72 7465 645f           sorted_
-0000ddd0: 6d61 7463 6865 7320 3d20 736f 7274 6564  matches = sorted
-0000dde0: 5f6d 6174 6368 6573 2c0a 2020 2020 2020  _matches,.      
-0000ddf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de10: 2020 6d65 6d5f 7376 5f77 696e 6e65 7273    mem_sv_winners
-0000de20: 203d 207b 7d29 5b30 5d29 0a0a 0a40 766d   = {})[0])...@vm
-0000de30: 286e 616d 6520 3d20 2253 696d 706c 6520  (name = "Simple 
-0000de40: 5374 6162 6c65 2056 6f74 696e 6722 290a  Stable Voting").
-0000de50: 6465 6620 7369 6d70 6c65 5f73 7461 626c  def simple_stabl
-0000de60: 655f 766f 7469 6e67 280a 2020 2020 6564  e_voting(.    ed
-0000de70: 6174 612c 200a 2020 2020 6375 7272 5f63  ata, .    curr_c
-0000de80: 616e 6473 3d4e 6f6e 652c 200a 2020 2020  ands=None, .    
-0000de90: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-0000dea0: 6e3d 4e6f 6e65 2c0a 2020 2020 616c 676f  n=None,.    algo
-0000deb0: 7269 7468 6d20 3d20 2762 6173 6963 2729  rithm = 'basic')
-0000dec0: 3a20 0a0a 2020 2020 2222 2249 6d70 6c65  : ..    """Imple
-0000ded0: 6d65 6e74 6174 696f 6e20 6f66 2053 696d  mentation of Sim
-0000dee0: 706c 6520 5374 6162 6c65 2056 6f74 696e  ple Stable Votin
-0000def0: 6720 6672 6f6d 2068 7474 7073 3a2f 2f61  g from https://a
-0000df00: 7278 6976 2e6f 7267 2f61 6273 2f32 3130  rxiv.org/abs/210
-0000df10: 382e 3030 3534 322e 200a 0a20 2020 2053  8.00542. ..    S
-0000df20: 696d 706c 6520 5374 6162 6c65 2056 6f74  imple Stable Vot
-0000df30: 696e 6720 6973 2061 2072 6563 7572 7369  ing is a recursi
-0000df40: 7665 2076 6f74 696e 6720 6d65 7468 6f64  ve voting method
-0000df50: 2064 6566 696e 6564 2061 7320 666f 6c6c   defined as foll
-0000df60: 6f77 733a 200a 0a20 2020 2031 2e20 4966  ows: ..    1. If
-0000df70: 2074 6865 7265 2069 7320 6f6e 6c79 206f   there is only o
-0000df80: 6e65 2063 616e 6469 6461 7465 2069 6e20  ne candidate in 
-0000df90: 7468 6520 7072 6f66 696c 652c 2074 6865  the profile, the
-0000dfa0: 6e20 7468 6174 2063 616e 6469 6461 7465  n that candidate
-0000dfb0: 2069 7320 7468 6520 7769 6e6e 6572 2e20   is the winner. 
-0000dfc0: 0a20 2020 2032 2e20 4f72 6465 7220 7468  .    2. Order th
-0000dfd0: 6520 7061 6972 7320 3a6d 6174 683a 6028  e pairs :math:`(
-0000dfe0: 612c 6229 6020 6f66 2063 616e 6469 6461  a,b)` of candida
-0000dff0: 7465 7320 6672 6f6d 206c 6172 6765 7374  tes from largest
-0000e000: 2074 6f20 736d 616c 6c65 7374 2076 616c   to smallest val
-0000e010: 7565 206f 6620 7468 6520 6d61 7267 696e  ue of the margin
-0000e020: 206f 6620 3a6d 6174 683a 6061 6020 6f76   of :math:`a` ov
-0000e030: 6572 203a 6d61 7468 3a60 6260 2c20 616e  er :math:`b`, an
-0000e040: 6420 6465 636c 6172 6520 6173 2053 696d  d declare as Sim
-0000e050: 706c 6520 5374 6162 6c65 2056 6f74 696e  ple Stable Votin
-0000e060: 6720 7769 6e6e 6572 7320 7468 6520 6361  g winners the ca
-0000e070: 6e64 6964 6174 6528 7329 203a 6d61 7468  ndidate(s) :math
-0000e080: 3a60 6160 2066 726f 6d20 7468 6520 6561  :`a` from the ea
-0000e090: 726c 6965 7374 2070 6169 7228 7329 203a  rliest pair(s) :
-0000e0a0: 6d61 7468 3a60 2861 2c62 2960 2073 7563  math:`(a,b)` suc
-0000e0b0: 6820 7468 6174 203a 6d61 7468 3a60 6160  h that :math:`a`
-0000e0c0: 2069 7320 6120 5369 6d70 6c65 2053 7461   is a Simple Sta
-0000e0d0: 626c 6520 566f 7469 6e67 2077 696e 6e65  ble Voting winne
-0000e0e0: 7220 696e 2074 6865 2065 6c65 6374 696f  r in the electio
-0000e0f0: 6e20 7769 7468 6f75 7420 3a6d 6174 683a  n without :math:
-0000e100: 6062 602e 200a 0a20 2020 2041 7267 733a  `b`. ..    Args:
-0000e110: 0a20 2020 2020 2020 2065 6461 7461 2028  .        edata (
-0000e120: 5072 6f66 696c 652c 2050 726f 6669 6c65  Profile, Profile
-0000e130: 5769 7468 5469 6573 2c20 4d61 7267 696e  WithTies, Margin
-0000e140: 4772 6170 6829 3a20 416e 7920 656c 6563  Graph): Any elec
-0000e150: 7469 6f6e 2064 6174 6120 7468 6174 2068  tion data that h
-0000e160: 6173 2061 2060 6d61 7267 696e 6020 6d65  as a `margin` me
-0000e170: 7468 6f64 2e20 0a20 2020 2020 2020 2063  thod. .        c
-0000e180: 7572 725f 6361 6e64 7320 284c 6973 745b  urr_cands (List[
-0000e190: 696e 745d 2c20 6f70 7469 6f6e 616c 293a  int], optional):
-0000e1a0: 2049 6620 7365 742c 2074 6865 6e20 6669   If set, then fi
-0000e1b0: 6e64 2074 6865 2077 696e 6e65 7273 2066  nd the winners f
-0000e1c0: 6f72 2074 6865 2070 726f 6669 6c65 2072  or the profile r
-0000e1d0: 6573 7472 6963 7465 6420 746f 2074 6865  estricted to the
-0000e1e0: 2063 616e 6469 6461 7465 7320 696e 2060   candidates in `
-0000e1f0: 6063 7572 725f 6361 6e64 7360 600a 2020  `curr_cands``.  
-0000e200: 2020 2020 2020 7374 7265 6e67 7468 5f66        strength_f
-0000e210: 756e 6374 696f 6e20 2866 756e 6374 696f  unction (functio
-0000e220: 6e2c 206f 7074 696f 6e61 6c29 3a20 5468  n, optional): Th
-0000e230: 6520 7374 7265 6e67 7468 2066 756e 6374  e strength funct
-0000e240: 696f 6e20 746f 2062 6520 7573 6564 2074  ion to be used t
-0000e250: 6f20 6361 6c63 756c 6174 6520 7468 6520  o calculate the 
-0000e260: 7374 7265 6e67 7468 206f 6620 6120 7061  strength of a pa
-0000e270: 7468 2e20 2020 5468 6520 6465 6661 756c  th.   The defaul
-0000e280: 7420 6973 2074 6865 206d 6172 6769 6e20  t is the margin 
-0000e290: 6d65 7468 6f64 206f 6620 6060 6564 6174  method of ``edat
-0000e2a0: 6160 602e 2020 2054 6869 7320 6f6e 6c79  a``.   This only
-0000e2b0: 206d 6174 7465 7273 2077 6865 6e20 7468   matters when th
-0000e2c0: 6520 6261 6c6c 6f74 7320 6172 6520 6e6f  e ballots are no
-0000e2d0: 7420 6c69 6e65 6172 206f 7264 6572 732e  t linear orders.
-0000e2e0: 200a 2020 2020 2020 2020 616c 676f 7269   .        algori
-0000e2f0: 7468 6d20 2873 7472 2c20 6f70 7469 6f6e  thm (str, option
-0000e300: 616c 293a 2053 7065 6369 6679 2077 6869  al): Specify whi
-0000e310: 6368 2061 6c67 6f72 6974 686d 2074 6f20  ch algorithm to 
-0000e320: 7573 652e 2020 4f70 7469 6f6e 7320 6172  use.  Options ar
-0000e330: 6520 2762 6173 6963 2720 2874 6865 2064  e 'basic' (the d
-0000e340: 6566 6175 6c74 2920 616e 6420 2777 6974  efault) and 'wit
-0000e350: 685f 636f 6e64 6f72 6365 745f 6368 6563  h_condorcet_chec
-0000e360: 6b27 2e0a 0a20 2020 2052 6574 7572 6e73  k'...    Returns
-0000e370: 3a20 0a20 2020 2020 2020 2041 2073 6f72  : .        A sor
-0000e380: 7465 6420 6c69 7374 206f 6620 6361 6e64  ted list of cand
-0000e390: 6964 6174 6573 2e20 0a0a 2020 2020 2e2e  idates. ..    ..
-0000e3a0: 2073 6565 616c 736f 3a3a 0a0a 2020 2020   seealso::..    
-0000e3b0: 2020 2020 3a6d 6574 683a 6070 7265 665f      :meth:`pref_
-0000e3c0: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
-0000e3d0: 7365 645f 6d65 7468 6f64 732e 7374 6162  sed_methods.stab
-0000e3e0: 6c65 5f76 6f74 696e 6760 0a0a 2020 2020  le_voting`..    
-0000e3f0: 3a45 7861 6d70 6c65 3a20 0a0a 2020 2020  :Example: ..    
-0000e400: 2e2e 2065 7865 635f 636f 6465 3a3a 0a0a  .. exec_code::..
-0000e410: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
-0000e420: 665f 766f 7469 6e67 2e77 6569 6768 7465  f_voting.weighte
-0000e430: 645f 6d61 6a6f 7269 7479 5f67 7261 7068  d_majority_graph
-0000e440: 7320 696d 706f 7274 204d 6172 6769 6e47  s import MarginG
-0000e450: 7261 7068 0a20 2020 2020 2020 2066 726f  raph.        fro
-0000e460: 6d20 7072 6566 5f76 6f74 696e 672e 6d61  m pref_voting.ma
-0000e470: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
-0000e480: 6473 2069 6d70 6f72 7420 7369 6d70 6c65  ds import simple
-0000e490: 5f73 7461 626c 655f 766f 7469 6e67 0a0a  _stable_voting..
-0000e4a0: 2020 2020 2020 2020 6d67 203d 204d 6172          mg = Mar
-0000e4b0: 6769 6e47 7261 7068 285b 302c 2031 2c20  ginGraph([0, 1, 
-0000e4c0: 322c 2033 5d2c 205b 2830 2c20 332c 2038  2, 3], [(0, 3, 8
-0000e4d0: 292c 2028 312c 2030 2c20 3130 292c 2028  ), (1, 0, 10), (
-0000e4e0: 322c 2030 2c20 3429 2c20 2832 2c20 312c  2, 0, 4), (2, 1,
-0000e4f0: 2038 292c 2028 332c 2031 2c20 3829 5d29   8), (3, 1, 8)])
-0000e500: 0a0a 2020 2020 2020 2020 7369 6d70 6c65  ..        simple
-0000e510: 5f73 7461 626c 655f 766f 7469 6e67 2e64  _stable_voting.d
-0000e520: 6973 706c 6179 286d 6729 0a20 2020 2020  isplay(mg).     
-0000e530: 2020 2073 696d 706c 655f 7374 6162 6c65     simple_stable
-0000e540: 5f76 6f74 696e 672e 6469 7370 6c61 7928  _voting.display(
-0000e550: 6d67 2c20 616c 676f 7269 7468 6d3d 2762  mg, algorithm='b
-0000e560: 6173 6963 2729 0a20 2020 2020 2020 2073  asic').        s
-0000e570: 696d 706c 655f 7374 6162 6c65 5f76 6f74  imple_stable_vot
-0000e580: 696e 672e 6469 7370 6c61 7928 6d67 2c20  ing.display(mg, 
-0000e590: 616c 676f 7269 7468 6d3d 2777 6974 685f  algorithm='with_
-0000e5a0: 636f 6e64 6f72 6365 745f 6368 6563 6b27  condorcet_check'
-0000e5b0: 290a 0a20 2020 2022 2222 0a20 2020 200a  )..    """.    .
-0000e5c0: 2020 2020 6966 2061 6c67 6f72 6974 686d      if algorithm
-0000e5d0: 203d 3d20 2762 6173 6963 273a 200a 2020   == 'basic': .  
-0000e5e0: 2020 2020 2020 7265 7475 726e 205f 7369        return _si
-0000e5f0: 6d70 6c65 5f73 7461 626c 655f 766f 7469  mple_stable_voti
-0000e600: 6e67 5f62 6173 6963 2865 6461 7461 2c20  ng_basic(edata, 
-0000e610: 6375 7272 5f63 616e 6473 203d 2063 7572  curr_cands = cur
-0000e620: 725f 6361 6e64 732c 2073 7472 656e 6774  r_cands, strengt
-0000e630: 685f 6675 6e63 7469 6f6e 203d 2073 7472  h_function = str
-0000e640: 656e 6774 685f 6675 6e63 7469 6f6e 290a  ength_function).
-0000e650: 2020 2020 656c 6966 2061 6c67 6f72 6974      elif algorit
-0000e660: 686d 203d 3d20 2777 6974 685f 636f 6e64  hm == 'with_cond
-0000e670: 6f72 6365 745f 6368 6563 6b27 3a0a 2020  orcet_check':.  
-0000e680: 2020 2020 2020 7265 7475 726e 205f 7369        return _si
-0000e690: 6d70 6c65 5f73 7461 626c 655f 766f 7469  mple_stable_voti
-0000e6a0: 6e67 5f77 6974 685f 636f 6e64 6f72 6365  ng_with_condorce
-0000e6b0: 745f 6368 6563 6b28 6564 6174 612c 2063  t_check(edata, c
-0000e6c0: 7572 725f 6361 6e64 7320 3d20 6375 7272  urr_cands = curr
-0000e6d0: 5f63 616e 6473 2c20 7374 7265 6e67 7468  _cands, strength
-0000e6e0: 5f66 756e 6374 696f 6e20 3d20 7374 7265  _function = stre
-0000e6f0: 6e67 7468 5f66 756e 6374 696f 6e29 0a20  ngth_function). 
-0000e700: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000e710: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-0000e720: 7228 2249 6e76 616c 6964 2061 6c67 6f72  r("Invalid algor
-0000e730: 6974 686d 2073 7065 6369 6669 6564 2e22  ithm specified."
-0000e740: 290a 2020 2020 0a0a 6465 6620 5f73 7461  ).    ..def _sta
-0000e750: 626c 655f 766f 7469 6e67 2865 6461 7461  ble_voting(edata
-0000e760: 2c20 0a20 2020 2020 2020 2020 2020 2020  , .             
-0000e770: 2020 2020 2020 6375 7272 5f63 616e 6473        curr_cands
-0000e780: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000e790: 2020 2020 2073 7472 656e 6774 685f 6675       strength_fu
-0000e7a0: 6e63 7469 6f6e 2c0a 2020 2020 2020 2020  nction,.        
-0000e7b0: 2020 2020 2020 2020 2020 2073 6f72 7465             sorte
-0000e7c0: 645f 6d61 7463 6865 732c 0a20 2020 2020  d_matches,.     
-0000e7d0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-0000e7e0: 6d5f 7376 5f77 696e 6e65 7273 293a 200a  m_sv_winners): .
-0000e7f0: 2020 2020 2727 270a 2020 2020 4465 7465      '''.    Dete
-0000e800: 726d 696e 6520 7468 6520 5374 6162 6c65  rmine the Stable
-0000e810: 2056 6f74 696e 6720 7769 6e6e 6572 7320   Voting winners 
-0000e820: 666f 7220 7468 6520 7072 6f66 696c 6520  for the profile 
-0000e830: 7768 696c 6520 6b65 6570 696e 6720 7472  while keeping tr
-0000e840: 6163 6b20 6f66 2074 6865 2077 696e 6e65  ack of the winne
-0000e850: 7273 2069 6e20 616e 7920 7375 6270 726f  rs in any subpro
-0000e860: 6669 6c65 7320 6368 6563 6b65 6420 6475  files checked du
-0000e870: 7269 6e67 2063 6f6d 7075 7461 7469 6f6e  ring computation
-0000e880: 2e20 0a20 2020 2027 2727 0a20 2020 200a  . .    '''.    .
-0000e890: 2020 2020 7376 5f77 696e 6e65 7273 203d      sv_winners =
-0000e8a0: 206c 6973 7428 290a 2020 2020 0a20 2020   list().    .   
-0000e8b0: 2075 6e64 6566 6561 7465 645f 6361 6e64   undefeated_cand
-0000e8c0: 6964 6174 6573 203d 2073 706c 6974 5f63  idates = split_c
-0000e8d0: 7963 6c65 2865 6461 7461 2c20 6375 7272  ycle(edata, curr
-0000e8e0: 5f63 616e 6473 203d 2063 7572 725f 6361  _cands = curr_ca
-0000e8f0: 6e64 732c 2073 7472 656e 6774 685f 6675  nds, strength_fu
-0000e900: 6e63 7469 6f6e 203d 2073 7472 656e 6774  nction = strengt
-0000e910: 685f 6675 6e63 7469 6f6e 290a 0a20 2020  h_function)..   
-0000e920: 2069 6620 6c65 6e28 6375 7272 5f63 616e   if len(curr_can
-0000e930: 6473 2920 3d3d 2031 3a20 0a20 2020 2020  ds) == 1: .     
-0000e940: 2020 206d 656d 5f73 765f 7769 6e6e 6572     mem_sv_winner
-0000e950: 735b 7475 706c 6528 6375 7272 5f63 616e  s[tuple(curr_can
-0000e960: 6473 295d 203d 2063 7572 725f 6361 6e64  ds)] = curr_cand
-0000e970: 730a 2020 2020 2020 2020 7265 7475 726e  s.        return
-0000e980: 2063 7572 725f 6361 6e64 732c 206d 656d   curr_cands, mem
-0000e990: 5f73 765f 7769 6e6e 6572 730a 2020 2020  _sv_winners.    
-0000e9a0: 0a20 2020 206d 6172 6769 6e5f 7769 746e  .    margin_witn
-0000e9b0: 6573 7369 6e67 5f77 696e 203d 202d 6d61  essing_win = -ma
-0000e9c0: 7468 2e69 6e66 0a0a 2020 2020 666f 7220  th.inf..    for 
-0000e9d0: 612c 2062 2c20 7320 696e 2073 6f72 7465  a, b, s in sorte
-0000e9e0: 645f 6d61 7463 6865 733a 0a20 2020 2020  d_matches:.     
-0000e9f0: 2020 2069 6620 7320 3c20 6d61 7267 696e     if s < margin
-0000ea00: 5f77 6974 6e65 7373 696e 675f 7769 6e3a  _witnessing_win:
-0000ea10: 200a 2020 2020 2020 2020 2020 2020 6272   .            br
-0000ea20: 6561 6b0a 2020 2020 2020 2020 6966 2061  eak.        if a
-0000ea30: 2069 6e20 756e 6465 6665 6174 6564 5f63   in undefeated_c
-0000ea40: 616e 6469 6461 7465 7320 616e 6420 6120  andidates and a 
-0000ea50: 6e6f 7420 696e 2073 765f 7769 6e6e 6572  not in sv_winner
-0000ea60: 733a 200a 2020 2020 2020 2020 2020 2020  s: .            
-0000ea70: 6361 6e64 735f 6d69 6e75 735f 6220 3d20  cands_minus_b = 
-0000ea80: 5b63 2066 6f72 2063 2069 6e20 6375 7272  [c for c in curr
-0000ea90: 5f63 616e 6473 2069 6620 6320 213d 2062  _cands if c != b
-0000eaa0: 5d0a 2020 2020 2020 2020 2020 2020 6361  ].            ca
-0000eab0: 6e64 735f 6d69 6e75 735f 625f 6b65 7920  nds_minus_b_key 
-0000eac0: 3d20 7475 706c 6528 736f 7274 6564 2863  = tuple(sorted(c
-0000ead0: 616e 6473 5f6d 696e 7573 5f62 2929 0a20  ands_minus_b)). 
-0000eae0: 2020 2020 2020 2020 2020 2069 6620 6361             if ca
-0000eaf0: 6e64 735f 6d69 6e75 735f 625f 6b65 7920  nds_minus_b_key 
-0000eb00: 6e6f 7420 696e 206d 656d 5f73 765f 7769  not in mem_sv_wi
-0000eb10: 6e6e 6572 732e 6b65 7973 2829 3a20 0a20  nners.keys(): . 
-0000eb20: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-0000eb30: 732c 206d 656d 5f73 765f 7769 6e6e 6572  s, mem_sv_winner
-0000eb40: 7320 3d20 5f73 7461 626c 655f 766f 7469  s = _stable_voti
-0000eb50: 6e67 2865 6461 7461 2c0a 2020 2020 2020  ng(edata,.      
-0000eb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb80: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-0000eb90: 7272 5f63 616e 6473 203d 2063 616e 6473  rr_cands = cands
-0000eba0: 5f6d 696e 7573 5f62 2c0a 2020 2020 2020  _minus_b,.      
-0000ebb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ebc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ebd0: 2020 2020 2020 2020 2020 2020 2020 7374                st
-0000ebe0: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
-0000ebf0: 3d20 7374 7265 6e67 7468 5f66 756e 6374  = strength_funct
-0000ec00: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
-0000ec10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec30: 2020 2020 2020 2020 2073 6f72 7465 645f           sorted_
-0000ec40: 6d61 7463 6865 7320 3d20 5b28 612c 2063  matches = [(a, c
-0000ec50: 2c20 7329 2066 6f72 2061 2c20 632c 2073  , s) for a, c, s
-0000ec60: 2069 6e20 736f 7274 6564 5f6d 6174 6368   in sorted_match
-0000ec70: 6573 2069 6620 6120 213d 2062 2061 6e64  es if a != b and
-0000ec80: 2063 2021 3d20 625d 2c0a 2020 2020 2020   c != b],.      
-0000ec90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ecb0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-0000ecc0: 6d5f 7376 5f77 696e 6e65 7273 203d 206d  m_sv_winners = m
-0000ecd0: 656d 5f73 765f 7769 6e6e 6572 7329 0a20  em_sv_winners). 
-0000ece0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0000ecf0: 656d 5f73 765f 7769 6e6e 6572 735b 6361  em_sv_winners[ca
-0000ed00: 6e64 735f 6d69 6e75 735f 625f 6b65 795d  nds_minus_b_key]
-0000ed10: 203d 2077 730a 2020 2020 2020 2020 2020   = ws.          
-0000ed20: 2020 656c 7365 3a20 0a20 2020 2020 2020    else: .       
-0000ed30: 2020 2020 2020 2020 2077 7320 3d20 6d65           ws = me
-0000ed40: 6d5f 7376 5f77 696e 6e65 7273 5b63 616e  m_sv_winners[can
-0000ed50: 6473 5f6d 696e 7573 5f62 5f6b 6579 5d0a  ds_minus_b_key].
-0000ed60: 2020 2020 2020 2020 2020 2020 6966 2061              if a
-0000ed70: 2069 6e20 7773 3a0a 2020 2020 2020 2020   in ws:.        
-0000ed80: 2020 2020 2020 2020 7376 5f77 696e 6e65          sv_winne
-0000ed90: 7273 2e61 7070 656e 6428 6129 0a20 2020  rs.append(a).   
-0000eda0: 2020 2020 2020 2020 2020 2020 206d 6172               mar
-0000edb0: 6769 6e5f 7769 746e 6573 7369 6e67 5f77  gin_witnessing_w
-0000edc0: 696e 203d 2073 0a20 2020 2020 2020 2020  in = s.         
-0000edd0: 2020 2020 2020 200a 2020 2020 7265 7475         .    retu
-0000ede0: 726e 2073 765f 7769 6e6e 6572 732c 206d  rn sv_winners, m
-0000edf0: 656d 5f73 765f 7769 6e6e 6572 730a 2020  em_sv_winners.  
-0000ee00: 2020 2020 2020 0a40 766d 286e 616d 6520        .@vm(name 
-0000ee10: 3d20 2253 7461 626c 6520 566f 7469 6e67  = "Stable Voting
-0000ee20: 2229 0a64 6566 205f 7374 6162 6c65 5f76  ").def _stable_v
-0000ee30: 6f74 696e 675f 7769 7468 5f63 6f6e 646f  oting_with_condo
-0000ee40: 7263 6574 5f63 6865 636b 280a 2020 2020  rcet_check(.    
-0000ee50: 6564 6174 612c 200a 2020 2020 6375 7272  edata, .    curr
-0000ee60: 5f63 616e 6473 3d4e 6f6e 652c 200a 2020  _cands=None, .  
-0000ee70: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
-0000ee80: 696f 6e3d 4e6f 6e65 293a 200a 2020 2020  ion=None): .    
-0000ee90: 2222 220a 2020 2020 5374 6162 6c65 2056  """.    Stable V
-0000eea0: 6f74 696e 6720 6973 2043 6f6e 646f 7263  oting is Condorc
-0000eeb0: 6574 2063 6f6e 7369 7374 656e 742e 2020  et consistent.  
-0000eec0: 2049 7420 6973 2066 6173 7465 7220 746f   It is faster to
-0000eed0: 2073 6b69 7020 6578 6563 7574 696e 6720   skip executing 
-0000eee0: 7468 6520 7265 6375 7273 6976 6520 616c  the recursive al
-0000eef0: 676f 7269 7468 6d20 7768 656e 2074 6865  gorithm when the
-0000ef00: 7265 2069 7320 6120 436f 6e64 6f72 6365  re is a Condorce
-0000ef10: 7420 7769 6e6e 6572 2e20 200a 0a20 2020  t winner.  ..   
-0000ef20: 2041 7267 733a 0a20 2020 2020 2020 2065   Args:.        e
-0000ef30: 6461 7461 2028 5072 6f66 696c 652c 2050  data (Profile, P
-0000ef40: 726f 6669 6c65 5769 7468 5469 6573 2c20  rofileWithTies, 
-0000ef50: 4d61 7267 696e 4772 6170 6829 3a20 416e  MarginGraph): An
-0000ef60: 7920 656c 6563 7469 6f6e 2064 6174 6120  y election data 
-0000ef70: 7468 6174 2068 6173 2061 2060 6d61 7267  that has a `marg
-0000ef80: 696e 6020 6d65 7468 6f64 2e20 0a20 2020  in` method. .   
-0000ef90: 2020 2020 2063 7572 725f 6361 6e64 7320       curr_cands 
-0000efa0: 284c 6973 745b 696e 745d 2c20 6f70 7469  (List[int], opti
-0000efb0: 6f6e 616c 293a 2049 6620 7365 742c 2074  onal): If set, t
-0000efc0: 6865 6e20 6669 6e64 2074 6865 2077 696e  hen find the win
-0000efd0: 6e65 7273 2066 6f72 2074 6865 2070 726f  ners for the pro
-0000efe0: 6669 6c65 2072 6573 7472 6963 7465 6420  file restricted 
-0000eff0: 746f 2074 6865 2063 616e 6469 6461 7465  to the candidate
-0000f000: 7320 696e 2060 6063 7572 725f 6361 6e64  s in ``curr_cand
-0000f010: 7360 600a 2020 2020 2020 2020 7374 7265  s``.        stre
-0000f020: 6e67 7468 5f66 756e 6374 696f 6e20 2866  ngth_function (f
-0000f030: 756e 6374 696f 6e2c 206f 7074 696f 6e61  unction, optiona
-0000f040: 6c29 3a20 5468 6520 7374 7265 6e67 7468  l): The strength
-0000f050: 2066 756e 6374 696f 6e20 746f 2062 6520   function to be 
-0000f060: 7573 6564 2074 6f20 6361 6c63 756c 6174  used to calculat
-0000f070: 6520 7468 6520 7374 7265 6e67 7468 206f  e the strength o
-0000f080: 6620 6120 7061 7468 2e20 2020 5468 6520  f a path.   The 
-0000f090: 6465 6661 756c 7420 6973 2074 6865 206d  default is the m
-0000f0a0: 6172 6769 6e20 6d65 7468 6f64 206f 6620  argin method of 
-0000f0b0: 6060 6564 6174 6160 602e 2020 2054 6869  ``edata``.   Thi
-0000f0c0: 7320 6f6e 6c79 206d 6174 7465 7273 2077  s only matters w
-0000f0d0: 6865 6e20 7468 6520 6261 6c6c 6f74 7320  hen the ballots 
-0000f0e0: 6172 6520 6e6f 7420 6c69 6e65 6172 206f  are not linear o
-0000f0f0: 7264 6572 732e 200a 0a20 2020 2052 6574  rders. ..    Ret
-0000f100: 7572 6e73 3a20 0a20 2020 2020 2020 2041  urns: .        A
-0000f110: 2073 6f72 7465 6420 6c69 7374 206f 6620   sorted list of 
-0000f120: 6361 6e64 6964 6174 6573 2e20 0a0a 2020  candidates. ..  
-0000f130: 2020 2222 220a 2020 2020 6377 203d 2065    """.    cw = e
-0000f140: 6461 7461 2e63 6f6e 646f 7263 6574 5f77  data.condorcet_w
-0000f150: 696e 6e65 7228 6375 7272 5f63 616e 6473  inner(curr_cands
-0000f160: 203d 2063 7572 725f 6361 6e64 7329 0a20   = curr_cands). 
-0000f170: 2020 2069 6620 6377 2069 7320 6e6f 7420     if cw is not 
-0000f180: 4e6f 6e65 3a20 0a20 2020 2020 2020 2072  None: .        r
-0000f190: 6574 7572 6e20 5b63 775d 0a20 2020 2065  eturn [cw].    e
-0000f1a0: 6c73 653a 200a 2020 2020 2020 2020 6375  lse: .        cu
-0000f1b0: 7272 5f63 616e 6473 203d 2065 6461 7461  rr_cands = edata
-0000f1c0: 2e63 616e 6469 6461 7465 7320 6966 2063  .candidates if c
-0000f1d0: 7572 725f 6361 6e64 7320 6973 204e 6f6e  urr_cands is Non
-0000f1e0: 6520 656c 7365 2063 7572 725f 6361 6e64  e else curr_cand
-0000f1f0: 730a 2020 2020 2020 2020 7374 7265 6e67  s.        streng
-0000f200: 7468 5f66 756e 6374 696f 6e20 3d20 6564  th_function = ed
-0000f210: 6174 612e 6d61 7267 696e 2069 6620 7374  ata.margin if st
-0000f220: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
-0000f230: 6973 204e 6f6e 6520 656c 7365 2073 7472  is None else str
-0000f240: 656e 6774 685f 6675 6e63 7469 6f6e 2020  ength_function  
-0000f250: 0a0a 2020 2020 2020 2020 6d61 7463 6865  ..        matche
-0000f260: 7320 3d20 5b28 612c 2062 2c20 7374 7265  s = [(a, b, stre
-0000f270: 6e67 7468 5f66 756e 6374 696f 6e28 612c  ngth_function(a,
-0000f280: 2062 2929 2066 6f72 2061 2069 6e20 6375   b)) for a in cu
-0000f290: 7272 5f63 616e 6473 2066 6f72 2062 2069  rr_cands for b i
-0000f2a0: 6e20 6375 7272 5f63 616e 6473 2069 6620  n curr_cands if 
-0000f2b0: 6120 213d 2062 5d0a 2020 2020 2020 2020  a != b].        
-0000f2c0: 736f 7274 6564 5f6d 6174 6368 6573 203d  sorted_matches =
-0000f2d0: 2073 6f72 7465 6428 6d61 7463 6865 732c   sorted(matches,
-0000f2e0: 2072 6576 6572 7365 3d54 7275 652c 206b   reverse=True, k
-0000f2f0: 6579 3d6c 616d 6264 6120 6d5f 775f 7765  ey=lambda m_w_we
-0000f300: 6967 6874 3a20 6d5f 775f 7765 6967 6874  ight: m_w_weight
-0000f310: 5b32 5d29 0a0a 2020 2020 2020 2020 7265  [2])..        re
-0000f320: 7475 726e 2073 6f72 7465 6428 5f73 7461  turn sorted(_sta
-0000f330: 626c 655f 766f 7469 6e67 2865 6461 7461  ble_voting(edata
-0000f340: 2c20 0a20 2020 2020 2020 2020 2020 2020  , .             
-0000f350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f360: 2020 2020 2020 2063 7572 725f 6361 6e64         curr_cand
-0000f370: 7320 3d20 6375 7272 5f63 616e 6473 2c20  s = curr_cands, 
-0000f380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f3a0: 2020 2020 2073 7472 656e 6774 685f 6675       strength_fu
-0000f3b0: 6e63 7469 6f6e 203d 2073 7472 656e 6774  nction = strengt
-0000f3c0: 685f 6675 6e63 7469 6f6e 2c0a 2020 2020  h_function,.    
-0000f3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f3f0: 736f 7274 6564 5f6d 6174 6368 6573 203d  sorted_matches =
-0000f400: 2073 6f72 7465 645f 6d61 7463 6865 732c   sorted_matches,
-0000f410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f430: 2020 2020 206d 656d 5f73 765f 7769 6e6e       mem_sv_winn
-0000f440: 6572 7320 3d20 7b7d 295b 305d 290a 0a64  ers = {})[0])..d
-0000f450: 6566 205f 7374 6162 6c65 5f76 6f74 696e  ef _stable_votin
-0000f460: 675f 6261 7369 6328 0a20 2020 2020 2020  g_basic(.       
-0000f470: 2065 6461 7461 2c20 0a20 2020 2020 2020   edata, .       
-0000f480: 2063 7572 725f 6361 6e64 7320 3d20 4e6f   curr_cands = No
-0000f490: 6e65 2c20 0a20 2020 2020 2020 2073 7472  ne, .        str
-0000f4a0: 656e 6774 685f 6675 6e63 7469 6f6e 203d  ength_function =
-0000f4b0: 204e 6f6e 6529 3a20 0a20 2020 2022 2222   None): .    """
-0000f4c0: 496d 706c 656d 656e 7461 7469 6f6e 206f  Implementation o
-0000f4d0: 6620 2053 7461 626c 6520 566f 7469 6e67  f  Stable Voting
-0000f4e0: 2066 726f 6d20 6874 7470 733a 2f2f 6172   from https://ar
-0000f4f0: 7869 762e 6f72 672f 6162 732f 3231 3038  xiv.org/abs/2108
-0000f500: 2e30 3035 3432 2e20 0a0a 2020 2020 4172  .00542. ..    Ar
-0000f510: 6773 3a0a 2020 2020 2020 2020 6564 6174  gs:.        edat
-0000f520: 6120 2850 726f 6669 6c65 2c20 5072 6f66  a (Profile, Prof
-0000f530: 696c 6557 6974 6854 6965 732c 204d 6172  ileWithTies, Mar
-0000f540: 6769 6e47 7261 7068 293a 2041 6e79 2065  ginGraph): Any e
-0000f550: 6c65 6374 696f 6e20 6461 7461 2074 6861  lection data tha
-0000f560: 7420 6861 7320 6120 606d 6172 6769 6e60  t has a `margin`
-0000f570: 206d 6574 686f 642e 200a 2020 2020 2020   method. .      
-0000f580: 2020 6375 7272 5f63 616e 6473 2028 4c69    curr_cands (Li
-0000f590: 7374 5b69 6e74 5d2c 206f 7074 696f 6e61  st[int], optiona
-0000f5a0: 6c29 3a20 4966 2073 6574 2c20 7468 656e  l): If set, then
-0000f5b0: 2066 696e 6420 7468 6520 7769 6e6e 6572   find the winner
-0000f5c0: 7320 666f 7220 7468 6520 7072 6f66 696c  s for the profil
-0000f5d0: 6520 7265 7374 7269 6374 6564 2074 6f20  e restricted to 
-0000f5e0: 7468 6520 6361 6e64 6964 6174 6573 2069  the candidates i
-0000f5f0: 6e20 6060 6375 7272 5f63 616e 6473 6060  n ``curr_cands``
-0000f600: 0a20 2020 2020 2020 2073 7472 656e 6774  .        strengt
-0000f610: 685f 6675 6e63 7469 6f6e 2028 6675 6e63  h_function (func
-0000f620: 7469 6f6e 2c20 6f70 7469 6f6e 616c 293a  tion, optional):
-0000f630: 2054 6865 2073 7472 656e 6774 6820 6675   The strength fu
-0000f640: 6e63 7469 6f6e 2074 6f20 6265 2075 7365  nction to be use
-0000f650: 6420 746f 2063 616c 6375 6c61 7465 2074  d to calculate t
-0000f660: 6865 2073 7472 656e 6774 6820 6f66 2061  he strength of a
-0000f670: 2070 6174 682e 2020 2054 6865 2064 6566   path.   The def
-0000f680: 6175 6c74 2069 7320 7468 6520 6d61 7267  ault is the marg
-0000f690: 696e 206d 6574 686f 6420 6f66 2060 6065  in method of ``e
-0000f6a0: 6461 7461 6060 2e20 2020 5468 6973 206f  data``.   This o
-0000f6b0: 6e6c 7920 6d61 7474 6572 7320 7768 656e  nly matters when
-0000f6c0: 2074 6865 2062 616c 6c6f 7473 2061 7265   the ballots are
-0000f6d0: 206e 6f74 206c 696e 6561 7220 6f72 6465   not linear orde
-0000f6e0: 7273 2e20 0a0a 2020 2020 5265 7475 726e  rs. ..    Return
-0000f6f0: 733a 200a 2020 2020 2020 2020 4120 736f  s: .        A so
-0000f700: 7274 6564 206c 6973 7420 6f66 2063 616e  rted list of can
-0000f710: 6469 6461 7465 732e 200a 0a20 2020 2022  didates. ..    "
-0000f720: 2222 0a0a 2020 2020 6375 7272 5f63 616e  ""..    curr_can
-0000f730: 6473 203d 2065 6461 7461 2e63 616e 6469  ds = edata.candi
-0000f740: 6461 7465 7320 6966 2063 7572 725f 6361  dates if curr_ca
-0000f750: 6e64 7320 6973 204e 6f6e 6520 656c 7365  nds is None else
-0000f760: 2063 7572 725f 6361 6e64 730a 2020 2020   curr_cands.    
-0000f770: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-0000f780: 6e20 3d20 6564 6174 612e 6d61 7267 696e  n = edata.margin
-0000f790: 2069 6620 7374 7265 6e67 7468 5f66 756e   if strength_fun
-0000f7a0: 6374 696f 6e20 6973 204e 6f6e 6520 656c  ction is None el
-0000f7b0: 7365 2073 7472 656e 6774 685f 6675 6e63  se strength_func
-0000f7c0: 7469 6f6e 2020 0a0a 2020 2020 6d61 7463  tion  ..    matc
-0000f7d0: 6865 7320 3d20 5b28 612c 2062 2c20 7374  hes = [(a, b, st
-0000f7e0: 7265 6e67 7468 5f66 756e 6374 696f 6e28  rength_function(
-0000f7f0: 612c 2062 2929 2066 6f72 2061 2069 6e20  a, b)) for a in 
-0000f800: 6375 7272 5f63 616e 6473 2066 6f72 2062  curr_cands for b
-0000f810: 2069 6e20 6375 7272 5f63 616e 6473 2069   in curr_cands i
-0000f820: 6620 6120 213d 2062 5d0a 2020 2020 736f  f a != b].    so
-0000f830: 7274 6564 5f6d 6174 6368 6573 203d 2073  rted_matches = s
-0000f840: 6f72 7465 6428 6d61 7463 6865 732c 2072  orted(matches, r
-0000f850: 6576 6572 7365 3d54 7275 652c 206b 6579  everse=True, key
-0000f860: 3d6c 616d 6264 6120 6d5f 775f 7765 6967  =lambda m_w_weig
-0000f870: 6874 3a20 6d5f 775f 7765 6967 6874 5b32  ht: m_w_weight[2
-0000f880: 5d29 0a0a 2020 2020 7265 7475 726e 2073  ])..    return s
-0000f890: 6f72 7465 6428 5f73 7461 626c 655f 766f  orted(_stable_vo
-0000f8a0: 7469 6e67 2865 6461 7461 2c20 0a20 2020  ting(edata, .   
-0000f8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f8c0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-0000f8d0: 7272 5f63 616e 6473 203d 2063 7572 725f  rr_cands = curr_
-0000f8e0: 6361 6e64 732c 200a 2020 2020 2020 2020  cands, .        
-0000f8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f900: 2020 2020 2020 2020 2073 7472 656e 6774           strengt
-0000f910: 685f 6675 6e63 7469 6f6e 203d 2073 7472  h_function = str
-0000f920: 656e 6774 685f 6675 6e63 7469 6f6e 2c0a  ength_function,.
-0000f930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f950: 2073 6f72 7465 645f 6d61 7463 6865 7320   sorted_matches 
-0000f960: 3d20 736f 7274 6564 5f6d 6174 6368 6573  = sorted_matches
-0000f970: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000f980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f990: 2020 206d 656d 5f73 765f 7769 6e6e 6572     mem_sv_winner
-0000f9a0: 7320 3d20 7b7d 295b 305d 290a 0a0a 0a40  s = {})[0])....@
-0000f9b0: 766d 286e 616d 6520 3d20 2253 7461 626c  vm(name = "Stabl
-0000f9c0: 6520 566f 7469 6e67 2229 0a64 6566 2073  e Voting").def s
-0000f9d0: 7461 626c 655f 766f 7469 6e67 280a 2020  table_voting(.  
-0000f9e0: 2020 6564 6174 612c 200a 2020 2020 6375    edata, .    cu
-0000f9f0: 7272 5f63 616e 6473 3d4e 6f6e 652c 200a  rr_cands=None, .
-0000fa00: 2020 2020 7374 7265 6e67 7468 5f66 756e      strength_fun
-0000fa10: 6374 696f 6e3d 4e6f 6e65 2c20 0a20 2020  ction=None, .   
-0000fa20: 2061 6c67 6f72 6974 686d 3d27 6261 7369   algorithm='basi
-0000fa30: 6327 293a 200a 2020 2020 2222 2249 6d70  c'): .    """Imp
-0000fa40: 6c65 6d65 6e74 6174 696f 6e20 6f66 2020  lementation of  
-0000fa50: 5374 6162 6c65 2056 6f74 696e 6720 6672  Stable Voting fr
-0000fa60: 6f6d 2068 7474 7073 3a2f 2f61 7278 6976  om https://arxiv
-0000fa70: 2e6f 7267 2f61 6273 2f32 3130 382e 3030  .org/abs/2108.00
-0000fa80: 3534 322e 200a 0a20 2020 2053 7461 626c  542. ..    Stabl
-0000fa90: 6520 566f 7469 6e67 2069 7320 6120 7265  e Voting is a re
-0000faa0: 6375 7273 6976 6520 766f 7469 6e67 206d  cursive voting m
-0000fab0: 6574 686f 6420 6465 6669 6e65 6420 6173  ethod defined as
-0000fac0: 2066 6f6c 6c6f 7773 3a20 0a0a 2020 2020   follows: ..    
-0000fad0: 312e 2020 4966 2074 6865 7265 2069 7320  1.  If there is 
-0000fae0: 6f6e 6c79 206f 6e65 2063 616e 6469 6461  only one candida
-0000faf0: 7465 2069 6e20 7468 6520 7072 6f66 696c  te in the profil
-0000fb00: 652c 2074 6865 6e20 7468 6174 2063 616e  e, then that can
-0000fb10: 6469 6461 7465 2069 7320 7468 6520 7769  didate is the wi
-0000fb20: 6e6e 6572 2e20 0a20 2020 2032 2e20 4f72  nner. .    2. Or
-0000fb30: 6465 7220 7468 6520 7061 6972 7320 3a6d  der the pairs :m
-0000fb40: 6174 683a 6028 612c 6229 6020 6f66 2063  ath:`(a,b)` of c
-0000fb50: 616e 6469 6461 7465 7320 6672 6f6d 206c  andidates from l
-0000fb60: 6172 6765 7374 2074 6f20 736d 616c 6c65  argest to smalle
-0000fb70: 7374 2076 616c 7565 206f 6620 7468 6520  st value of the 
-0000fb80: 6d61 7267 696e 206f 6620 3a6d 6174 683a  margin of :math:
-0000fb90: 6061 6020 6f76 6572 203a 6d61 7468 3a60  `a` over :math:`
-0000fba0: 6260 2073 7563 6820 7468 6174 203a 6d61  b` such that :ma
-0000fbb0: 7468 3a60 6160 2069 7320 756e 6465 6665  th:`a` is undefe
-0000fbc0: 6174 6564 2061 6363 6f72 6469 6e67 2074  ated according t
-0000fbd0: 6f20 5370 6c69 7420 4379 636c 652c 2061  o Split Cycle, a
-0000fbe0: 6e64 2064 6563 6c61 7265 2061 7320 5374  nd declare as St
-0000fbf0: 6162 6c65 2056 6f74 696e 6720 7769 6e6e  able Voting winn
-0000fc00: 6572 7320 7468 6520 6361 6e64 6964 6174  ers the candidat
-0000fc10: 6528 7329 203a 6d61 7468 3a60 6160 2066  e(s) :math:`a` f
-0000fc20: 726f 6d20 7468 6520 6561 726c 6965 7374  rom the earliest
-0000fc30: 2070 6169 7228 7329 203a 6d61 7468 3a60   pair(s) :math:`
-0000fc40: 2861 2c62 2960 2073 7563 6820 7468 6174  (a,b)` such that
-0000fc50: 203a 6d61 7468 3a60 6160 2069 7320 6120   :math:`a` is a 
-0000fc60: 5369 6d70 6c65 2053 7461 626c 6520 566f  Simple Stable Vo
-0000fc70: 7469 6e67 2077 696e 6e65 7220 696e 2074  ting winner in t
-0000fc80: 6865 2065 6c65 6374 696f 6e20 7769 7468  he election with
-0000fc90: 6f75 7420 3a6d 6174 683a 6062 602e 200a  out :math:`b`. .
-0000fca0: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-0000fcb0: 2020 2065 6461 7461 2028 5072 6f66 696c     edata (Profil
-0000fcc0: 652c 2050 726f 6669 6c65 5769 7468 5469  e, ProfileWithTi
-0000fcd0: 6573 2c20 4d61 7267 696e 4772 6170 6829  es, MarginGraph)
-0000fce0: 3a20 416e 7920 656c 6563 7469 6f6e 2064  : Any election d
-0000fcf0: 6174 6120 7468 6174 2068 6173 2061 2060  ata that has a `
-0000fd00: 6d61 7267 696e 6020 6d65 7468 6f64 2e20  margin` method. 
-0000fd10: 0a20 2020 2020 2020 2063 7572 725f 6361  .        curr_ca
-0000fd20: 6e64 7320 284c 6973 745b 696e 745d 2c20  nds (List[int], 
-0000fd30: 6f70 7469 6f6e 616c 293a 2049 6620 7365  optional): If se
-0000fd40: 742c 2074 6865 6e20 6669 6e64 2074 6865  t, then find the
-0000fd50: 2077 696e 6e65 7273 2066 6f72 2074 6865   winners for the
-0000fd60: 2070 726f 6669 6c65 2072 6573 7472 6963   profile restric
-0000fd70: 7465 6420 746f 2074 6865 2063 616e 6469  ted to the candi
-0000fd80: 6461 7465 7320 696e 2060 6063 7572 725f  dates in ``curr_
-0000fd90: 6361 6e64 7360 600a 2020 2020 2020 2020  cands``.        
-0000fda0: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-0000fdb0: 6e20 2866 756e 6374 696f 6e2c 206f 7074  n (function, opt
-0000fdc0: 696f 6e61 6c29 3a20 5468 6520 7374 7265  ional): The stre
-0000fdd0: 6e67 7468 2066 756e 6374 696f 6e20 746f  ngth function to
-0000fde0: 2062 6520 7573 6564 2074 6f20 6361 6c63   be used to calc
-0000fdf0: 756c 6174 6520 7468 6520 7374 7265 6e67  ulate the streng
-0000fe00: 7468 206f 6620 6120 7061 7468 2e20 2020  th of a path.   
-0000fe10: 5468 6520 6465 6661 756c 7420 6973 2074  The default is t
-0000fe20: 6865 206d 6172 6769 6e20 6d65 7468 6f64  he margin method
-0000fe30: 206f 6620 6060 6564 6174 6160 602e 2020   of ``edata``.  
-0000fe40: 2054 6869 7320 6f6e 6c79 206d 6174 7465   This only matte
-0000fe50: 7273 2077 6865 6e20 7468 6520 6261 6c6c  rs when the ball
-0000fe60: 6f74 7320 6172 6520 6e6f 7420 6c69 6e65  ots are not line
-0000fe70: 6172 206f 7264 6572 732e 200a 0a20 2020  ar orders. ..   
-0000fe80: 2052 6574 7572 6e73 3a20 0a20 2020 2020   Returns: .     
-0000fe90: 2020 2041 2073 6f72 7465 6420 6c69 7374     A sorted list
-0000fea0: 206f 6620 6361 6e64 6964 6174 6573 2e20   of candidates. 
-0000feb0: 0a0a 2020 2020 2e2e 2073 6565 616c 736f  ..    .. seealso
-0000fec0: 3a3a 0a0a 2020 2020 2020 2020 3a6d 6574  ::..        :met
-0000fed0: 683a 6070 7265 665f 766f 7469 6e67 2e6d  h:`pref_voting.m
-0000fee0: 6172 6769 6e5f 6261 7365 645f 6d65 7468  argin_based_meth
-0000fef0: 6f64 732e 7369 6d70 6c65 5f73 7461 626c  ods.simple_stabl
-0000ff00: 655f 766f 7469 6e67 600a 0a0a 2020 2020  e_voting`...    
-0000ff10: 3a45 7861 6d70 6c65 3a20 0a0a 2020 2020  :Example: ..    
-0000ff20: 2e2e 2065 7865 635f 636f 6465 3a3a 0a0a  .. exec_code::..
-0000ff30: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
-0000ff40: 665f 766f 7469 6e67 2e77 6569 6768 7465  f_voting.weighte
-0000ff50: 645f 6d61 6a6f 7269 7479 5f67 7261 7068  d_majority_graph
-0000ff60: 7320 696d 706f 7274 204d 6172 6769 6e47  s import MarginG
-0000ff70: 7261 7068 0a20 2020 2020 2020 2066 726f  raph.        fro
-0000ff80: 6d20 7072 6566 5f76 6f74 696e 672e 6d61  m pref_voting.ma
-0000ff90: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
-0000ffa0: 6473 2069 6d70 6f72 7420 7374 6162 6c65  ds import stable
-0000ffb0: 5f76 6f74 696e 670a 0a20 2020 2020 2020  _voting..       
-0000ffc0: 206d 6720 3d20 4d61 7267 696e 4772 6170   mg = MarginGrap
-0000ffd0: 6828 5b30 2c20 312c 2032 2c20 335d 2c20  h([0, 1, 2, 3], 
-0000ffe0: 5b28 302c 2033 2c20 3829 2c20 2831 2c20  [(0, 3, 8), (1, 
-0000fff0: 302c 2031 3029 2c20 2832 2c20 302c 2034  0, 10), (2, 0, 4
-00010000: 292c 2028 322c 2031 2c20 3829 2c20 2833  ), (2, 1, 8), (3
-00010010: 2c20 312c 2038 295d 290a 0a20 2020 2020  , 1, 8)])..     
-00010020: 2020 2073 7461 626c 655f 766f 7469 6e67     stable_voting
-00010030: 2e64 6973 706c 6179 286d 6729 0a20 2020  .display(mg).   
-00010040: 2020 2020 2073 7461 626c 655f 766f 7469       stable_voti
-00010050: 6e67 2e64 6973 706c 6179 286d 672c 2061  ng.display(mg, a
-00010060: 6c67 6f72 6974 686d 3d27 6261 7369 6327  lgorithm='basic'
-00010070: 290a 2020 2020 2020 2020 7374 6162 6c65  ).        stable
-00010080: 5f76 6f74 696e 672e 6469 7370 6c61 7928  _voting.display(
-00010090: 6d67 2c20 616c 676f 7269 7468 6d3d 2777  mg, algorithm='w
-000100a0: 6974 685f 636f 6e64 6f72 6365 745f 6368  ith_condorcet_ch
-000100b0: 6563 6b27 290a 0a20 2020 2022 2222 0a0a  eck')..    """..
-000100c0: 2020 2020 6966 2061 6c67 6f72 6974 686d      if algorithm
-000100d0: 203d 3d20 2762 6173 6963 273a 200a 2020   == 'basic': .  
-000100e0: 2020 2020 2020 7265 7475 726e 205f 7374        return _st
-000100f0: 6162 6c65 5f76 6f74 696e 675f 6261 7369  able_voting_basi
-00010100: 6328 6564 6174 612c 2063 7572 725f 6361  c(edata, curr_ca
-00010110: 6e64 7320 3d20 6375 7272 5f63 616e 6473  nds = curr_cands
-00010120: 2c20 7374 7265 6e67 7468 5f66 756e 6374  , strength_funct
-00010130: 696f 6e20 3d20 7374 7265 6e67 7468 5f66  ion = strength_f
-00010140: 756e 6374 696f 6e29 0a20 2020 2065 6c69  unction).    eli
-00010150: 6620 616c 676f 7269 7468 6d20 3d3d 2027  f algorithm == '
-00010160: 7769 7468 5f63 6f6e 646f 7263 6574 5f63  with_condorcet_c
-00010170: 6865 636b 273a 0a20 2020 2020 2020 2072  heck':.        r
-00010180: 6574 7572 6e20 5f73 7461 626c 655f 766f  eturn _stable_vo
-00010190: 7469 6e67 5f77 6974 685f 636f 6e64 6f72  ting_with_condor
-000101a0: 6365 745f 6368 6563 6b28 6564 6174 612c  cet_check(edata,
-000101b0: 2063 7572 725f 6361 6e64 7320 3d20 6375   curr_cands = cu
-000101c0: 7272 5f63 616e 6473 2c20 7374 7265 6e67  rr_cands, streng
-000101d0: 7468 5f66 756e 6374 696f 6e20 3d20 7374  th_function = st
-000101e0: 7265 6e67 7468 5f66 756e 6374 696f 6e29  rength_function)
-000101f0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-00010200: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-00010210: 726f 7228 2249 6e76 616c 6964 2061 6c67  ror("Invalid alg
-00010220: 6f72 6974 686d 2073 7065 6369 6669 6564  orithm specified
-00010230: 2e22 290a 2020 2020 0a0a 0a0a 4076 6d28  .").    ....@vm(
-00010240: 6e61 6d65 3d22 4573 7365 6e74 6961 6c20  name="Essential 
-00010250: 5365 7422 290a 6465 6620 6573 7365 6e74  Set").def essent
-00010260: 6961 6c28 6564 6174 612c 2063 7572 725f  ial(edata, curr_
-00010270: 6361 6e64 7320 3d20 4e6f 6e65 2c20 7468  cands = None, th
-00010280: 7265 7368 6f6c 6420 3d20 302e 3030 3030  reshold = 0.0000
-00010290: 3030 3129 3a20 0a20 2020 2022 2222 5468  001): .    """Th
-000102a0: 6520 4573 7365 6e74 6961 6c20 5365 7420  e Essential Set 
-000102b0: 6973 2074 6865 2073 7570 706f 7274 206f  is the support o
-000102c0: 6620 7468 6520 2863 686f 7365 6e29 2043  f the (chosen) C
-000102d0: 3220 6d61 7869 6d61 6c20 6c6f 7474 6572  2 maximal lotter
-000102e0: 792e 0a0a 2020 2020 4172 6773 3a0a 2020  y...    Args:.  
-000102f0: 2020 2020 2020 6564 6174 6120 2850 726f        edata (Pro
-00010300: 6669 6c65 2c20 5072 6f66 696c 6557 6974  file, ProfileWit
-00010310: 6854 6965 732c 204d 6172 6769 6e47 7261  hTies, MarginGra
-00010320: 7068 293a 2041 6e79 2065 6c65 6374 696f  ph): Any electio
-00010330: 6e20 6461 7461 2074 6861 7420 6861 7320  n data that has 
-00010340: 6120 606d 6172 6769 6e5f 6d61 7472 6978  a `margin_matrix
-00010350: 6020 6174 7472 6962 7574 652e 0a20 2020  ` attribute..   
-00010360: 2020 2020 2063 7572 725f 6361 6e64 7320       curr_cands 
-00010370: 284c 6973 745b 696e 745d 2c20 6f70 7469  (List[int], opti
-00010380: 6f6e 616c 293a 2049 6620 7365 742c 2074  onal): If set, t
-00010390: 6865 6e20 6669 6e64 2074 6865 2077 696e  hen find the win
-000103a0: 6e65 7273 2066 6f72 2074 6865 2070 726f  ners for the pro
-000103b0: 6669 6c65 2072 6573 7472 6963 7465 6420  file restricted 
-000103c0: 746f 2074 6865 2063 616e 6469 6461 7465  to the candidate
-000103d0: 7320 696e 2060 6063 7572 725f 6361 6e64  s in ``curr_cand
-000103e0: 7360 600a 0a20 2020 2052 6574 7572 6e73  s``..    Returns
-000103f0: 3a0a 2020 2020 2020 2020 4120 736f 7274  :.        A sort
-00010400: 6564 206c 6973 7420 6f66 2063 616e 6469  ed list of candi
-00010410: 6461 7465 732e 0a0a 2020 2020 2222 220a  dates...    """.
-00010420: 2020 2020 6d6c 203d 206d 6178 696d 616c      ml = maximal
-00010430: 5f6c 6f74 7465 7279 2865 6461 7461 2c20  _lottery(edata, 
-00010440: 6375 7272 5f63 616e 6473 3d63 7572 725f  curr_cands=curr_
-00010450: 6361 6e64 7329 0a0a 2020 2020 7265 7475  cands)..    retu
-00010460: 726e 2073 6f72 7465 6428 5b63 2066 6f72  rn sorted([c for
-00010470: 2063 2069 6e20 6d6c 2e6b 6579 7328 2920   c in ml.keys() 
-00010480: 6966 206d 6c5b 635d 203e 2074 6872 6573  if ml[c] > thres
-00010490: 686f 6c64 5d29 0a0a 4076 6d28 6e61 6d65  hold])..@vm(name
-000104a0: 3d22 5765 6967 6874 6564 2043 6f76 6572  ="Weighted Cover
-000104b0: 696e 6722 290a 6465 6620 7765 6967 6874  ing").def weight
-000104c0: 6564 5f63 6f76 6572 696e 6728 6564 6174  ed_covering(edat
-000104d0: 612c 2063 7572 725f 6361 6e64 733d 4e6f  a, curr_cands=No
-000104e0: 6e65 293a 200a 2020 2020 2222 2241 6363  ne): .    """Acc
-000104f0: 6f72 6469 6e67 2074 6f20 5765 6967 6874  ording to Weight
-00010500: 6564 2043 6f76 6572 696e 672c 2078 2064  ed Covering, x d
-00010510: 6566 6561 7473 2079 2069 6620 7468 6520  efeats y if the 
-00010520: 6d61 7267 696e 206f 6620 7820 6f76 6572  margin of x over
-00010530: 2079 2069 7320 706f 7369 7469 7665 2061   y is positive a
-00010540: 6e64 2066 6f72 2065 7665 7279 206f 7468  nd for every oth
-00010550: 6572 207a 2c20 7468 6520 6d61 7267 696e  er z, the margin
-00010560: 206f 6620 7820 6f76 6572 207a 2069 7320   of x over z is 
-00010570: 6772 6561 7465 7220 7468 616e 206f 7220  greater than or 
-00010580: 6571 7561 6c20 746f 2074 6865 206d 6172  equal to the mar
-00010590: 6769 6e20 6f66 2079 206f 7665 7220 7a2e  gin of y over z.
-000105a0: 200a 0a20 2020 2041 7267 733a 0a20 2020   ..    Args:.   
-000105b0: 2020 2020 2065 6461 7461 2028 5072 6f66       edata (Prof
-000105c0: 696c 652c 2050 726f 6669 6c65 5769 7468  ile, ProfileWith
-000105d0: 5469 6573 2c20 4d61 7267 696e 4772 6170  Ties, MarginGrap
-000105e0: 6829 3a20 416e 7920 656c 6563 7469 6f6e  h): Any election
-000105f0: 2064 6174 6120 7468 6174 2068 6173 2061   data that has a
-00010600: 2060 6d61 7267 696e 6020 6d65 7468 6f64   `margin` method
-00010610: 2e0a 2020 2020 2020 2020 6375 7272 5f63  ..        curr_c
-00010620: 616e 6473 2028 4c69 7374 5b69 6e74 5d2c  ands (List[int],
-00010630: 206f 7074 696f 6e61 6c29 3a20 4966 2073   optional): If s
-00010640: 6574 2c20 7468 656e 2066 696e 6420 7468  et, then find th
-00010650: 6520 7769 6e6e 6572 7320 666f 7220 7468  e winners for th
-00010660: 6520 7072 6f66 696c 6520 7265 7374 7269  e profile restri
-00010670: 6374 6564 2074 6f20 7468 6520 6361 6e64  cted to the cand
-00010680: 6964 6174 6573 2069 6e20 6060 6375 7272  idates in ``curr
-00010690: 5f63 616e 6473 6060 0a0a 2020 2020 5265  _cands``..    Re
-000106a0: 7475 726e 733a 0a20 2020 2020 2020 2041  turns:.        A
-000106b0: 2073 6f72 7465 6420 6c69 7374 206f 6620   sorted list of 
-000106c0: 6361 6e64 6964 6174 6573 2e0a 0a20 2020  candidates...   
-000106d0: 202e 2e20 6e6f 7465 3a3a 0a20 2020 2020   .. note::.     
-000106e0: 2020 2053 6565 2c20 652e 672e 2c20 4268     See, e.g., Bh
-000106f0: 6173 6b61 7220 4475 7474 6120 616e 6420  askar Dutta and 
-00010700: 4a65 616e 2d46 7261 6e63 6f69 7320 4c61  Jean-Francois La
-00010710: 736c 6965 722c 2022 436f 6d70 6172 6973  slier, "Comparis
-00010720: 6f6e 2066 756e 6374 696f 6e73 2061 6e64  on functions and
-00010730: 2063 686f 6963 6520 636f 7272 6573 706f   choice correspo
-00010740: 6e64 656e 6365 732c 2220 536f 6369 616c  ndences," Social
-00010750: 2043 686f 6963 6520 616e 6420 5765 6c66   Choice and Welf
-00010760: 6172 652c 2031 363a 3531 33e2 8093 3533  are, 16:513...53
-00010770: 322c 2031 3939 392c 2064 6f69 3a31 302e  2, 1999, doi:10.
-00010780: 3130 3037 2f73 3030 3335 3530 3035 3031  1007/s0035500501
-00010790: 3538 2c20 616e 6420 5261 75cc 816c 2050  58, and Rau..l P
-000107a0: 65cc 8172 657a 2d46 6572 6e61 cc81 6e64  e..rez-Ferna..nd
-000107b0: 657a 2061 6e64 2042 6572 6e61 7264 2044  ez and Bernard D
-000107c0: 6520 4261 6574 732c 2022 5468 6520 7375  e Baets, "The su
-000107d0: 7065 7263 6f76 6572 696e 6720 7265 6c61  percovering rela
-000107e0: 7469 6f6e 2c20 7468 6520 7061 6972 7769  tion, the pairwi
-000107f0: 7365 2077 696e 6e65 722c 2061 6e64 206d  se winner, and m
-00010800: 6f72 6520 6d69 7373 696e 6720 6c69 6e6b  ore missing link
-00010810: 7320 6265 7477 6565 6e20 426f 7264 6120  s between Borda 
-00010820: 616e 6420 436f 6e64 6f72 6365 742c 2220  and Condorcet," 
-00010830: 536f 6369 616c 2043 686f 6963 6520 616e  Social Choice an
-00010840: 6420 5765 6c66 6172 652c 2035 303a 3332  d Welfare, 50:32
-00010850: 39e2 8093 3335 322c 2032 3031 382c 2064  9...352, 2018, d
-00010860: 6f69 3a31 302e 3130 3037 2f73 3030 3335  oi:10.1007/s0035
-00010870: 352d 3031 372d 3130 3836 2d30 2e0a 2020  5-017-1086-0..  
-00010880: 2020 2222 220a 0a20 2020 2063 616e 6469    """..    candi
-00010890: 6461 7465 7320 3d20 6564 6174 612e 6361  dates = edata.ca
-000108a0: 6e64 6964 6174 6573 2069 6620 6375 7272  ndidates if curr
-000108b0: 5f63 616e 6473 2069 7320 4e6f 6e65 2065  _cands is None e
-000108c0: 6c73 6520 6375 7272 5f63 616e 6473 0a0a  lse curr_cands..
-000108d0: 2020 2020 646f 6d20 3d20 7b63 3a20 7365      dom = {c: se
-000108e0: 7428 6564 6174 612e 646f 6d69 6e61 746f  t(edata.dominato
-000108f0: 7273 2863 2c20 6375 7272 5f63 616e 6473  rs(c, curr_cands
-00010900: 203d 2063 7572 725f 6361 6e64 7329 2920   = curr_cands)) 
-00010910: 666f 7220 6320 696e 2063 616e 6469 6461  for c in candida
-00010920: 7465 737d 0a20 2020 2075 635f 7365 7420  tes}.    uc_set 
-00010930: 3d20 6c69 7374 2829 0a0a 2020 2020 666f  = list()..    fo
-00010940: 7220 7920 696e 2063 616e 6469 6461 7465  r y in candidate
-00010950: 733a 0a20 2020 2020 2020 2069 735f 696e  s:.        is_in
-00010960: 5f75 6373 203d 2054 7275 650a 2020 2020  _ucs = True.    
-00010970: 2020 2020 666f 7220 7820 696e 2065 6461      for x in eda
-00010980: 7461 2e64 6f6d 696e 6174 6f72 7328 792c  ta.dominators(y,
-00010990: 2063 7572 725f 6361 6e64 7320 3d20 6375   curr_cands = cu
-000109a0: 7272 5f63 616e 6473 293a 0a20 2020 2020  rr_cands):.     
-000109b0: 2020 2020 2020 2023 2063 6865 636b 2069         # check i
-000109c0: 6620 7920 636f 7665 7273 2078 2c20 692e  f y covers x, i.
-000109d0: 652e 2c20 666f 7220 6576 6572 7920 7a2c  e., for every z,
-000109e0: 206d 6172 6769 6e28 782c 207a 2920 3e3d   margin(x, z) >=
-000109f0: 206d 6172 6769 6e28 792c 207a 290a 2020   margin(y, z).  
-00010a00: 2020 2020 2020 2020 2020 636f 7665 7273            covers
-00010a10: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
-00010a20: 2020 2020 666f 7220 7a20 696e 2063 616e      for z in can
-00010a30: 6469 6461 7465 733a 0a20 2020 2020 2020  didates:.       
-00010a40: 2020 2020 2020 2020 2069 6620 6564 6174           if edat
-00010a50: 612e 6d61 7267 696e 2878 2c20 7a29 203c  a.margin(x, z) <
-00010a60: 2065 6461 7461 2e6d 6172 6769 6e28 792c   edata.margin(y,
-00010a70: 207a 293a 0a20 2020 2020 2020 2020 2020   z):.           
-00010a80: 2020 2020 2020 2020 2063 6f76 6572 7320           covers 
-00010a90: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
-00010aa0: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-00010ab0: 6b0a 2020 2020 2020 2020 2020 0a20 2020  k.          .   
-00010ac0: 2020 2020 2020 2020 2069 6620 636f 7665           if cove
-00010ad0: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
-00010ae0: 2020 2020 6973 5f69 6e5f 7563 7320 3d20      is_in_ucs = 
-00010af0: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
-00010b00: 2020 2020 2020 6272 6561 6b0a 2020 2020        break.    
-00010b10: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
-00010b20: 2020 2020 2069 6620 6973 5f69 6e5f 7563       if is_in_uc
-00010b30: 733a 0a20 2020 2020 2020 2020 2020 2075  s:.            u
-00010b40: 635f 7365 742e 6170 7065 6e64 2879 290a  c_set.append(y).
-00010b50: 0a20 2020 2072 6574 7572 6e20 736f 7274  .    return sort
-00010b60: 6564 2875 635f 7365 7429 0a0a 4076 6d28  ed(uc_set)..@vm(
-00010b70: 6e61 6d65 203d 2022 4c6f 7373 2d54 7269  name = "Loss-Tri
-00010b80: 6d6d 6572 2056 6f74 696e 6722 290a 6465  mmer Voting").de
-00010b90: 6620 6c6f 7373 5f74 7269 6d6d 6572 2865  f loss_trimmer(e
-00010ba0: 6461 7461 2c20 6375 7272 5f63 616e 6473  data, curr_cands
-00010bb0: 203d 204e 6f6e 6529 3a0a 2020 2020 2222   = None):.    ""
-00010bc0: 2249 7465 7261 7469 7665 6c79 2065 6c69  "Iteratively eli
-00010bd0: 6d69 6e61 7465 2074 6865 2063 616e 6469  minate the candi
-00010be0: 6461 7465 2077 6974 6820 7468 6520 6c61  date with the la
-00010bf0: 7267 6573 7420 7375 6d20 6f66 206d 6172  rgest sum of mar
-00010c00: 6769 6e73 206f 6620 6c6f 7373 2075 6e74  gins of loss unt
-00010c10: 696c 2061 2043 6f6e 646f 7263 6574 2077  il a Condorcet w
-00010c20: 696e 6e65 7220 6973 2066 6f75 6e64 2e20  inner is found. 
-00010c30: 496e 2074 6869 7320 7665 7273 696f 6e20  In this version 
-00010c40: 6f66 2074 6865 206d 6574 686f 642c 2070  of the method, p
-00010c50: 6172 616c 6c65 6c2d 756e 6976 6572 7365  arallel-universe
-00010c60: 2074 6965 6272 6561 6b69 6e67 2069 7320   tiebreaking is 
-00010c70: 7573 6564 2069 6620 7468 6572 6520 6172  used if there ar
-00010c80: 6520 6d75 6c74 6970 6c65 2063 616e 6469  e multiple candi
-00010c90: 6461 7465 7320 7769 7468 2074 6865 206c  dates with the l
-00010ca0: 6172 6765 7374 2073 756d 206f 6620 6d61  argest sum of ma
-00010cb0: 7267 696e 7320 6f66 206c 6f73 732e 0a0a  rgins of loss...
-00010cc0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00010cd0: 2020 6564 6174 6120 2850 726f 6669 6c65    edata (Profile
-00010ce0: 2c20 5072 6f66 696c 6557 6974 6854 6965  , ProfileWithTie
-00010cf0: 732c 204d 6172 6769 6e47 7261 7068 293a  s, MarginGraph):
-00010d00: 2041 6e79 2065 6c65 6374 696f 6e20 6461   Any election da
-00010d10: 7461 2074 6861 7420 6861 7320 6120 6d61  ta that has a ma
-00010d20: 7267 696e 206d 6574 686f 642e 0a20 2020  rgin method..   
-00010d30: 2020 2020 2063 7572 725f 6361 6e64 7320       curr_cands 
-00010d40: 284c 6973 745b 696e 745d 2c20 6f70 7469  (List[int], opti
-00010d50: 6f6e 616c 293a 2049 6620 7365 742c 2074  onal): If set, t
-00010d60: 6865 6e20 6669 6e64 2074 6865 2077 696e  hen find the win
-00010d70: 6e65 7273 2066 6f72 2074 6865 2070 726f  ners for the pro
-00010d80: 6669 6c65 2072 6573 7472 6963 7465 6420  file restricted 
-00010d90: 746f 2074 6865 2063 616e 6469 6461 7465  to the candidate
-00010da0: 7320 696e 2060 6063 7572 725f 6361 6e64  s in ``curr_cand
-00010db0: 7360 600a 0a20 2020 2052 6574 7572 6e73  s``..    Returns
-00010dc0: 3a20 0a20 2020 2020 2020 2041 2073 6f72  : .        A sor
-00010dd0: 7465 6420 6c69 7374 206f 6620 6361 6e64  ted list of cand
-00010de0: 6964 6174 6573 0a0a 2020 2020 2e2e 206e  idates..    .. n
-00010df0: 6f74 653a 3a0a 2020 2020 2020 2020 4d65  ote::.        Me
-00010e00: 7468 6f64 2070 726f 706f 7365 6420 6279  thod proposed by
-00010e10: 2052 6963 6861 7264 2042 2e20 4461 726c   Richard B. Darl
-00010e20: 696e 6774 6f6e 2069 6e20 2254 6865 2043  ington in "The C
-00010e30: 6173 6520 666f 7220 7468 6520 4c6f 7373  ase for the Loss
-00010e40: 2d54 7269 6d6d 6572 2056 6f74 696e 6720  -Trimmer Voting 
-00010e50: 5379 7374 656d 2e22 0a0a 2020 2020 2222  System."..    ""
-00010e60: 220a 0a20 2020 2063 7572 725f 6361 6e64  "..    curr_cand
-00010e70: 7320 3d20 6564 6174 612e 6361 6e64 6964  s = edata.candid
-00010e80: 6174 6573 2069 6620 6375 7272 5f63 616e  ates if curr_can
-00010e90: 6473 2069 7320 4e6f 6e65 2065 6c73 6520  ds is None else 
-00010ea0: 6375 7272 5f63 616e 6473 0a0a 2020 2020  curr_cands..    
-00010eb0: 7765 616b 5f63 7720 3d20 6564 6174 612e  weak_cw = edata.
-00010ec0: 7765 616b 5f63 6f6e 646f 7263 6574 5f77  weak_condorcet_w
-00010ed0: 696e 6e65 7228 6375 7272 5f63 616e 6473  inner(curr_cands
-00010ee0: 203d 2063 7572 725f 6361 6e64 7329 0a20   = curr_cands). 
-00010ef0: 2020 2023 2049 6620 7468 6572 6520 6172     # If there ar
-00010f00: 6520 7765 616b 2043 6f6e 646f 7263 6574  e weak Condorcet
-00010f10: 2077 696e 6e65 7273 2c20 7265 7475 726e   winners, return
-00010f20: 2074 686f 7365 2063 616e 6469 6461 7465   those candidate
-00010f30: 730a 2020 2020 6966 2065 6461 7461 2e77  s.    if edata.w
-00010f40: 6561 6b5f 636f 6e64 6f72 6365 745f 7769  eak_condorcet_wi
-00010f50: 6e6e 6572 2863 7572 725f 6361 6e64 7320  nner(curr_cands 
-00010f60: 3d20 6375 7272 5f63 616e 6473 2920 6973  = curr_cands) is
-00010f70: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00010f80: 2020 2072 6574 7572 6e20 736f 7274 6564     return sorted
-00010f90: 2877 6561 6b5f 6377 290a 2020 2020 0a20  (weak_cw).    . 
-00010fa0: 2020 2023 204f 7468 6572 7769 7365 2c20     # Otherwise, 
-00010fb0: 6361 6c63 756c 6174 6520 7468 6520 7375  calculate the su
-00010fc0: 6d20 6f66 206d 6172 6769 6e73 206f 6620  m of margins of 
-00010fd0: 6c6f 7373 2066 6f72 2065 6163 6820 6361  loss for each ca
-00010fe0: 6e64 6964 6174 650a 2020 2020 7375 6d5f  ndidate.    sum_
-00010ff0: 6f66 5f6d 6172 6769 6e73 5f6f 665f 6c6f  of_margins_of_lo
-00011000: 7373 203d 207b 6361 6e64 3a20 7375 6d28  ss = {cand: sum(
-00011010: 5b65 6461 7461 2e6d 6172 6769 6e28 6f74  [edata.margin(ot
-00011020: 6865 725f 6361 6e64 2c20 6361 6e64 2920  her_cand, cand) 
-00011030: 666f 7220 6f74 6865 725f 6361 6e64 2069  for other_cand i
-00011040: 6e20 6375 7272 5f63 616e 6473 2069 6620  n curr_cands if 
-00011050: 6564 6174 612e 6d61 7267 696e 286f 7468  edata.margin(oth
-00011060: 6572 5f63 616e 642c 2063 616e 6429 203e  er_cand, cand) >
-00011070: 2030 5d29 2066 6f72 2063 616e 6420 696e   0]) for cand in
-00011080: 2063 7572 725f 6361 6e64 737d 0a0a 2020   curr_cands}..  
-00011090: 2020 2320 4669 6e64 2074 6865 2063 616e    # Find the can
-000110a0: 6469 6461 7465 7320 7769 7468 2074 6865  didates with the
-000110b0: 206c 6172 6765 7374 2073 756d 206f 6620   largest sum of 
-000110c0: 6d61 7267 696e 7320 6f66 206c 6f73 730a  margins of loss.
-000110d0: 2020 2020 6d61 785f 7375 6d5f 6f66 5f6d      max_sum_of_m
-000110e0: 6172 6769 6e73 5f6f 665f 6c6f 7373 203d  argins_of_loss =
-000110f0: 206d 6178 2873 756d 5f6f 665f 6d61 7267   max(sum_of_marg
-00011100: 696e 735f 6f66 5f6c 6f73 732e 7661 6c75  ins_of_loss.valu
-00011110: 6573 2829 290a 2020 2020 6269 6767 6573  es()).    bigges
-00011120: 745f 6c6f 7365 7273 203d 205b 6361 6e64  t_losers = [cand
-00011130: 2066 6f72 2063 616e 6420 696e 2063 7572   for cand in cur
-00011140: 725f 6361 6e64 7320 6966 2073 756d 5f6f  r_cands if sum_o
-00011150: 665f 6d61 7267 696e 735f 6f66 5f6c 6f73  f_margins_of_los
-00011160: 735b 6361 6e64 5d20 3d3d 206d 6178 5f73  s[cand] == max_s
-00011170: 756d 5f6f 665f 6d61 7267 696e 735f 6f66  um_of_margins_of
-00011180: 5f6c 6f73 735d 0a0a 2020 2020 7769 6e6e  _loss]..    winn
-00011190: 6572 7320 3d20 5b5d 0a0a 2020 2020 2320  ers = []..    # 
-000111a0: 466f 7220 6561 6368 2062 6967 6765 7374  For each biggest
-000111b0: 206c 6f73 6572 2c20 6361 6c63 756c 6174   loser, calculat
-000111c0: 6520 7468 6520 7769 6e6e 6572 7320 6166  e the winners af
-000111d0: 7465 7220 7265 6d6f 7669 6e67 2074 6861  ter removing tha
-000111e0: 7420 6361 6e64 6964 6174 652e 2054 6865  t candidate. The
-000111f0: 2075 6e69 6f6e 206f 6620 7468 6573 6520   union of these 
-00011200: 7365 7473 2069 7320 7468 6520 7365 7420  sets is the set 
-00011210: 6f66 2077 696e 6e65 7273 2e0a 2020 2020  of winners..    
-00011220: 666f 7220 626c 2069 6e20 6269 6767 6573  for bl in bigges
-00011230: 745f 6c6f 7365 7273 3a0a 2020 2020 2020  t_losers:.      
-00011240: 2020 7769 6e6e 6572 735f 7769 7468 6f75    winners_withou
-00011250: 745f 626c 203d 206c 6f73 735f 7472 696d  t_bl = loss_trim
-00011260: 6d65 7228 6564 6174 612c 2063 7572 725f  mer(edata, curr_
-00011270: 6361 6e64 7320 3d20 5b63 616e 6420 666f  cands = [cand fo
-00011280: 7220 6361 6e64 2069 6e20 6375 7272 5f63  r cand in curr_c
-00011290: 616e 6473 2069 6620 6361 6e64 2021 3d20  ands if cand != 
-000112a0: 626c 5d29 0a20 2020 2020 2020 2077 696e  bl]).        win
-000112b0: 6e65 7273 202b 3d20 7769 6e6e 6572 735f  ners += winners_
-000112c0: 7769 7468 6f75 745f 626c 0a0a 2020 2020  without_bl..    
-000112d0: 7265 7475 726e 2073 6f72 7465 6428 6c69  return sorted(li
-000112e0: 7374 2873 6574 2877 696e 6e65 7273 2929  st(set(winners))
-000112f0: 290a 0a0a 6465 6620 6469 7374 616e 6365  )...def distance
-00011300: 5f74 6f5f 6d61 7267 696e 5f67 7261 7068  _to_margin_graph
-00011310: 2865 6461 7461 2c20 7265 6c2c 2065 7870  (edata, rel, exp
-00011320: 203d 2031 2c20 6375 7272 5f63 616e 6473   = 1, curr_cands
-00011330: 203d 204e 6f6e 6529 3a20 0a20 2020 2022   = None): .    "
-00011340: 2222 0a20 2020 2043 616c 6375 6c61 7465  "".    Calculate
-00011350: 2074 6865 2064 6973 7461 6e63 6520 6f66   the distance of
-00011360: 2060 6072 656c 6060 2028 6120 7265 6c61   ``rel`` (a rela
-00011370: 7469 6f6e 2920 746f 2074 6865 206d 616a  tion) to the maj
-00011380: 6f72 6974 7920 6772 6170 6820 6f66 2060  ority graph of `
-00011390: 6065 6461 7461 6060 2e20 0a20 2020 2022  `edata``. .    "
-000113a0: 2222 0a20 2020 2063 616e 6469 6461 7465  "".    candidate
-000113b0: 7320 3d20 6564 6174 612e 6361 6e64 6964  s = edata.candid
-000113c0: 6174 6573 2069 6620 6375 7272 5f63 616e  ates if curr_can
-000113d0: 6473 2069 7320 4e6f 6e65 2065 6c73 6520  ds is None else 
-000113e0: 6375 7272 5f63 616e 6473 0a20 2020 200a  curr_cands.    .
-000113f0: 2020 2020 6966 2074 7970 6528 6564 6174      if type(edat
-00011400: 6129 203d 3d20 4d61 6a6f 7269 7479 4772  a) == MajorityGr
-00011410: 6170 6820 616e 6420 6578 7020 3d3d 2030  aph and exp == 0
-00011420: 3a0a 2020 2020 2020 2020 2320 6966 2065  :.        # if e
-00011430: 6461 7461 2069 7320 6120 4d61 6a6f 7269  data is a Majori
-00011440: 7479 4772 6170 682c 2077 6520 6e65 6564  tyGraph, we need
-00011450: 2074 6f20 6164 6420 6d61 7267 696e 7320   to add margins 
-00011460: 666f 7220 7468 6520 666f 6c6c 6f77 696e  for the followin
-00011470: 6720 636f 6465 2074 6f20 776f 726b 2e20  g code to work. 
-00011480: 2054 6865 206d 6172 6769 6e73 2064 6f20   The margins do 
-00011490: 6e6f 7420 6d61 7474 6572 2077 6865 6e20  not matter when 
-000114a0: 6578 703d 3d30 2e20 2020 0a20 2020 2020  exp==0.   .     
-000114b0: 2020 2065 6461 7461 203d 204d 6172 6769     edata = Margi
-000114c0: 6e47 7261 7068 2863 616e 6469 6461 7465  nGraph(candidate
-000114d0: 732c 205b 2863 312c 2063 322c 2031 2920  s, [(c1, c2, 1) 
-000114e0: 666f 7220 6331 2c20 6332 2069 6e20 6564  for c1, c2 in ed
-000114f0: 6174 612e 6564 6765 7320 6966 2028 6331  ata.edges if (c1
-00011500: 2069 6e20 6361 6e64 6964 6174 6573 2061   in candidates a
-00011510: 6e64 2063 3220 696e 2063 616e 6469 6461  nd c2 in candida
-00011520: 7465 7329 5d29 0a20 2020 2070 656e 616c  tes)]).    penal
-00011530: 7479 203d 2030 0a20 2020 2066 6f72 2061  ty = 0.    for a
-00011540: 2c62 2069 6e20 636f 6d62 696e 6174 696f  ,b in combinatio
-00011550: 6e73 2863 616e 6469 6461 7465 732c 2032  ns(candidates, 2
-00011560: 293a 200a 2020 2020 2020 2020 6966 2065  ): .        if e
-00011570: 6461 7461 2e6d 616a 6f72 6974 795f 7072  data.majority_pr
-00011580: 6566 6572 7328 612c 2062 2920 616e 6420  efers(a, b) and 
-00011590: 2862 2c61 2920 696e 2072 656c 3a20 0a20  (b,a) in rel: . 
-000115a0: 2020 2020 2020 2020 2020 2070 656e 616c             penal
-000115b0: 7479 202b 3d20 2865 6461 7461 2e6d 6172  ty += (edata.mar
-000115c0: 6769 6e28 612c 2062 2920 2a2a 2065 7870  gin(a, b) ** exp
-000115d0: 290a 2020 2020 2020 2020 656c 6966 2065  ).        elif e
-000115e0: 6461 7461 2e6d 616a 6f72 6974 795f 7072  data.majority_pr
-000115f0: 6566 6572 7328 622c 2061 2920 616e 6420  efers(b, a) and 
-00011600: 2861 2c62 2920 696e 2072 656c 3a20 0a20  (a,b) in rel: . 
-00011610: 2020 2020 2020 2020 2020 2070 656e 616c             penal
-00011620: 7479 202b 3d20 2865 6461 7461 2e6d 6172  ty += (edata.mar
-00011630: 6769 6e28 622c 2061 2920 2a2a 2065 7870  gin(b, a) ** exp
-00011640: 290a 2020 2020 2020 2020 656c 6966 2065  ).        elif e
-00011650: 6461 7461 2e6d 616a 6f72 6974 795f 7072  data.majority_pr
-00011660: 6566 6572 7328 612c 2062 2920 616e 6420  efers(a, b) and 
-00011670: 2861 2c62 2920 6e6f 7420 696e 2072 656c  (a,b) not in rel
-00011680: 2061 6e64 2028 622c 6129 206e 6f74 2069   and (b,a) not i
-00011690: 6e20 7265 6c3a 200a 2020 2020 2020 2020  n rel: .        
-000116a0: 2020 2020 7065 6e61 6c74 7920 2b3d 2028      penalty += (
-000116b0: 6564 6174 612e 6d61 7267 696e 2861 2c20  edata.margin(a, 
-000116c0: 6229 202a 2a20 6578 7029 202f 2032 200a  b) ** exp) / 2 .
-000116d0: 2020 2020 2020 2020 656c 6966 2065 6461          elif eda
-000116e0: 7461 2e6d 616a 6f72 6974 795f 7072 6566  ta.majority_pref
-000116f0: 6572 7328 622c 2061 2920 616e 6420 2861  ers(b, a) and (a
-00011700: 2c62 2920 6e6f 7420 696e 2072 656c 2061  ,b) not in rel a
-00011710: 6e64 2028 622c 6129 206e 6f74 2069 6e20  nd (b,a) not in 
-00011720: 7265 6c3a 200a 2020 2020 2020 2020 2020  rel: .          
-00011730: 2020 7065 6e61 6c74 7920 2b3d 2028 6564    penalty += (ed
-00011740: 6174 612e 6d61 7267 696e 2862 2c20 6129  ata.margin(b, a)
-00011750: 202a 2a20 6578 7029 2020 2f20 320a 2020   ** exp)  / 2.  
-00011760: 2020 7265 7475 726e 2070 656e 616c 7479    return penalty
-00011770: 0a0a 0a6d 675f 766d 7320 3d20 5b0a 2020  ...mg_vms = [.  
-00011780: 2020 6d69 6e69 6d61 782c 200a 2020 2020    minimax, .    
-00011790: 7370 6c69 745f 6379 636c 652c 0a20 2020  split_cycle,.   
-000117a0: 2023 6265 6174 5f70 6174 682c 0a20 2020   #beat_path,.   
-000117b0: 2023 7261 6e6b 6564 5f70 6169 7273 2c0a   #ranked_pairs,.
-000117c0: 2020 2020 2372 616e 6b65 645f 7061 6972      #ranked_pair
-000117d0: 735f 7769 7468 5f74 6573 742c 0a20 2020  s_with_test,.   
-000117e0: 2072 616e 6b65 645f 7061 6972 735f 7a74   ranked_pairs_zt
-000117f0: 2c0a 2020 2020 7261 6e6b 6564 5f70 6169  ,.    ranked_pai
-00011800: 7273 5f74 622c 0a20 2020 2023 7269 7665  rs_tb,.    #rive
-00011810: 722c 0a20 2020 2023 7269 7665 725f 7769  r,.    #river_wi
-00011820: 7468 5f74 6573 742c 200a 2020 2020 7369  th_test, .    si
-00011830: 6d70 6c65 5f73 7461 626c 655f 766f 7469  mple_stable_voti
-00011840: 6e67 2c0a 2020 2020 7374 6162 6c65 5f76  ng,.    stable_v
-00011850: 6f74 696e 672c 0a20 2020 2065 7373 656e  oting,.    essen
-00011860: 7469 616c 2c0a 2020 2020 7765 6967 6874  tial,.    weight
-00011870: 6564 5f63 6f76 6572 696e 672c 0a20 2020  ed_covering,.   
-00011880: 206c 6f73 735f 7472 696d 6d65 720a 5d0a   loss_trimmer.].
-00011890: 0a0a 6d67 5f76 6d73 5f61 6c6c 203d 205b  ..mg_vms_all = [
-000118a0: 0a20 2020 206d 696e 696d 6178 2c20 0a20  .    minimax, . 
-000118b0: 2020 2073 706c 6974 5f63 7963 6c65 2c0a     split_cycle,.
-000118c0: 2020 2020 6265 6174 5f70 6174 682c 0a20      beat_path,. 
-000118d0: 2020 2072 616e 6b65 645f 7061 6972 732c     ranked_pairs,
-000118e0: 0a20 2020 2072 616e 6b65 645f 7061 6972  .    ranked_pair
-000118f0: 735f 7769 7468 5f74 6573 742c 0a20 2020  s_with_test,.   
-00011900: 2072 616e 6b65 645f 7061 6972 735f 7a74   ranked_pairs_zt
-00011910: 2c0a 2020 2020 7261 6e6b 6564 5f70 6169  ,.    ranked_pai
-00011920: 7273 5f74 622c 0a20 2020 2072 6976 6572  rs_tb,.    river
-00011930: 2c0a 2020 2020 7269 7665 725f 7769 7468  ,.    river_with
-00011940: 5f74 6573 742c 200a 2020 2020 7369 6d70  _test, .    simp
-00011950: 6c65 5f73 7461 626c 655f 766f 7469 6e67  le_stable_voting
-00011960: 2c0a 2020 2020 7374 6162 6c65 5f76 6f74  ,.    stable_vot
-00011970: 696e 672c 0a20 2020 2065 7373 656e 7469  ing,.    essenti
-00011980: 616c 2c0a 2020 2020 7765 6967 6874 6564  al,.    weighted
-00011990: 5f63 6f76 6572 696e 672c 0a20 2020 206c  _covering,.    l
-000119a0: 6f73 735f 7472 696d 6d65 720a 5d         oss_trimmer.]
+0000d0c0: 2020 2020 7276 5f64 6566 6561 742e 6164      rv_defeat.ad
+0000d0d0: 6428 6361 6e64 5f74 6f5f 6369 6478 5b65  d(cand_to_cidx[e
+0000d0e0: 305d 2c63 616e 645f 746f 5f63 6964 785b  0],cand_to_cidx[
+0000d0f0: 6531 5d29 0a20 2020 2020 2020 2020 2020  e1]).           
+0000d100: 2077 696e 6e65 7273 2e61 7070 656e 6428   winners.append(
+0000d110: 6369 6478 5f74 6f5f 6361 6e64 5b72 765f  cidx_to_cand[rv_
+0000d120: 6465 6665 6174 2e69 6e69 7469 616c 5f65  defeat.initial_e
+0000d130: 6c65 6d65 6e74 7328 295b 305d 5d29 0a20  lements()[0]]). 
+0000d140: 2020 2072 6574 7572 6e20 736f 7274 6564     return sorted
+0000d150: 286c 6973 7428 7365 7428 7769 6e6e 6572  (list(set(winner
+0000d160: 7329 2929 0a0a 7269 7665 725f 7a74 5f70  s)))..river_zt_p
+0000d170: 726f 7065 7274 6965 7320 3d20 566f 7469  roperties = Voti
+0000d180: 6e67 4d65 7468 6f64 5072 6f70 6572 7469  ngMethodProperti
+0000d190: 6573 280a 2020 2020 636f 6e64 6f72 6365  es(.    condorce
+0000d1a0: 745f 7769 6e6e 6572 3d54 7275 652c 200a  t_winner=True, .
+0000d1b0: 2020 2020 636f 6e64 6f72 6365 745f 6c6f      condorcet_lo
+0000d1c0: 7365 723d 5472 7565 2c0a 2020 2020 7061  ser=True,.    pa
+0000d1d0: 7265 746f 5f64 6f6d 696e 616e 6365 3d54  reto_dominance=T
+0000d1e0: 7275 652c 200a 2020 2020 290a 4076 6d28  rue, .    ).@vm(
+0000d1f0: 6e61 6d65 3d22 5269 7665 7220 5a54 222c  name="River ZT",
+0000d200: 0a20 2020 2070 726f 7065 7274 6965 733d  .    properties=
+0000d210: 7269 7665 725f 7a74 5f70 726f 7065 7274  river_zt_propert
+0000d220: 6965 732c 0a20 2020 2069 6e70 7574 5f74  ies,.    input_t
+0000d230: 7970 6573 3d5b 456c 6563 7469 6f6e 5479  ypes=[ElectionTy
+0000d240: 7065 732e 5052 4f46 494c 455d 290a 6465  pes.PROFILE]).de
+0000d250: 6620 7269 7665 725f 7a74 2870 726f 6669  f river_zt(profi
+0000d260: 6c65 2c20 6375 7272 5f63 616e 6473 203d  le, curr_cands =
+0000d270: 204e 6f6e 652c 2073 7472 656e 6774 685f   None, strength_
+0000d280: 6675 6e63 7469 6f6e 203d 204e 6f6e 6529  function = None)
+0000d290: 3a20 2020 0a20 2020 2022 2222 5269 7665  :   .    """Rive
+0000d2a0: 7220 7768 6572 6520 6120 6669 7865 6420  r where a fixed 
+0000d2b0: 766f 7465 7220 6272 6561 6b73 2061 6e79  voter breaks any
+0000d2c0: 2074 6965 7320 696e 2074 6865 206d 6172   ties in the mar
+0000d2d0: 6769 6e73 2e20 2049 7420 6973 2061 6c77  gins.  It is alw
+0000d2e0: 6179 7320 7468 6520 766f 7465 7220 696e  ays the voter in
+0000d2f0: 2070 6f73 6974 696f 6e20 3020 7468 6174   position 0 that
+0000d300: 2062 7265 616b 7320 7468 6520 7469 6573   breaks the ties
+0000d310: 2e20 2053 696e 6365 2076 6f74 6572 7320  .  Since voters 
+0000d320: 6861 7665 2073 7472 6963 7420 7072 6566  have strict pref
+0000d330: 6572 656e 6365 732c 2074 6869 7320 6d65  erences, this me
+0000d340: 7468 6f64 2069 7320 7265 736f 6c75 7465  thod is resolute
+0000d350: 2e20 200a 0a20 2020 2041 7267 733a 0a20  .  ..    Args:. 
+0000d360: 2020 2020 2020 2065 6461 7461 2028 5072         edata (Pr
+0000d370: 6f66 696c 6529 3a20 4120 7072 6f66 696c  ofile): A profil
+0000d380: 6520 6f66 206c 696e 6561 7220 6f72 6465  e of linear orde
+0000d390: 7273 0a20 2020 2020 2020 2063 7572 725f  rs.        curr_
+0000d3a0: 6361 6e64 7320 284c 6973 745b 696e 745d  cands (List[int]
+0000d3b0: 2c20 6f70 7469 6f6e 616c 293a 2049 6620  , optional): If 
+0000d3c0: 7365 742c 2074 6865 6e20 6669 6e64 2074  set, then find t
+0000d3d0: 6865 2077 696e 6e65 7273 2066 6f72 2074  he winners for t
+0000d3e0: 6865 2070 726f 6669 6c65 2072 6573 7472  he profile restr
+0000d3f0: 6963 7465 6420 746f 2074 6865 2063 616e  icted to the can
+0000d400: 6469 6461 7465 7320 696e 2060 6063 7572  didates in ``cur
+0000d410: 725f 6361 6e64 7360 600a 0a20 2020 2052  r_cands``..    R
+0000d420: 6574 7572 6e73 3a20 0a20 2020 2020 2020  eturns: .       
+0000d430: 2041 2073 6f72 7465 6420 6c69 7374 206f   A sorted list o
+0000d440: 6620 6361 6e64 6964 6174 6573 2e20 0a0a  f candidates. ..
+0000d450: 2020 2020 2e2e 2073 6565 616c 736f 3a3a      .. seealso::
+0000d460: 0a0a 2020 2020 2020 2020 3a6d 6574 683a  ..        :meth:
+0000d470: 6070 7265 665f 766f 7469 6e67 2e6d 6172  `pref_voting.mar
+0000d480: 6769 6e5f 6261 7365 645f 6d65 7468 6f64  gin_based_method
+0000d490: 732e 7269 7665 7260 2c20 3a6d 6574 683a  s.river`, :meth:
+0000d4a0: 6070 7265 665f 766f 7469 6e67 2e6d 6172  `pref_voting.mar
+0000d4b0: 6769 6e5f 6261 7365 645f 6d65 7468 6f64  gin_based_method
+0000d4c0: 732e 7269 7665 725f 7769 7468 5f74 6573  s.river_with_tes
+0000d4d0: 7460 2c20 3a6d 6574 683a 6070 7265 665f  t`, :meth:`pref_
+0000d4e0: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
+0000d4f0: 7365 645f 6d65 7468 6f64 732e 7261 6e6b  sed_methods.rank
+0000d500: 6564 5f70 6169 7273 600a 0a20 2020 200a  ed_pairs`..    .
+0000d510: 2020 2020 2222 220a 2020 2020 6361 6e64      """.    cand
+0000d520: 6964 6174 6573 203d 2070 726f 6669 6c65  idates = profile
+0000d530: 2e63 616e 6469 6461 7465 7320 6966 2063  .candidates if c
+0000d540: 7572 725f 6361 6e64 7320 6973 204e 6f6e  urr_cands is Non
+0000d550: 6520 656c 7365 2063 7572 725f 6361 6e64  e else curr_cand
+0000d560: 7320 2020 200a 2020 2020 0a20 2020 2023  s    .    .    #
+0000d570: 2074 6865 2074 6965 2d62 7265 616b 6572   the tie-breaker
+0000d580: 2069 7320 616c 7761 7973 2074 6865 2066   is always the f
+0000d590: 6972 7374 2076 6f74 6572 2e20 0a20 2020  irst voter. .   
+0000d5a0: 2074 625f 7261 6e6b 696e 6720 3d20 7475   tb_ranking = tu
+0000d5b0: 706c 6528 5b63 2066 6f72 2063 2069 6e20  ple([c for c in 
+0000d5c0: 6c69 7374 2870 726f 6669 6c65 2e5f 7261  list(profile._ra
+0000d5d0: 6e6b 696e 6773 5b30 5d29 2069 6620 6320  nkings[0]) if c 
+0000d5e0: 696e 2063 616e 6469 6461 7465 735d 290a  in candidates]).
+0000d5f0: 2020 2020 0a20 2020 2072 6574 7572 6e20      .    return 
+0000d600: 7269 7665 725f 7462 2870 726f 6669 6c65  river_tb(profile
+0000d610: 2c20 6375 7272 5f63 616e 6473 203d 2063  , curr_cands = c
+0000d620: 7572 725f 6361 6e64 732c 2074 6965 5f62  urr_cands, tie_b
+0000d630: 7265 616b 6572 203d 2074 625f 7261 6e6b  reaker = tb_rank
+0000d640: 696e 672c 2073 7472 656e 6774 685f 6675  ing, strength_fu
+0000d650: 6e63 7469 6f6e 203d 2073 7472 656e 6774  nction = strengt
+0000d660: 685f 6675 6e63 7469 6f6e 290a 2020 2020  h_function).    
+0000d670: 0a0a 2320 5369 6d70 6c65 2053 7461 626c  ..# Simple Stabl
+0000d680: 6520 566f 7469 6e67 200a 6465 6620 5f73  e Voting .def _s
+0000d690: 696d 706c 655f 7374 6162 6c65 5f76 6f74  imple_stable_vot
+0000d6a0: 696e 6728 6375 7272 5f63 616e 6473 2c20  ing(curr_cands, 
+0000d6b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d6c0: 2020 2020 2020 2020 2020 2073 6f72 7465             sorte
+0000d6d0: 645f 6d61 7463 6865 732c 0a20 2020 2020  d_matches,.     
+0000d6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6f0: 2020 2020 206d 656d 5f73 765f 7769 6e6e       mem_sv_winn
+0000d700: 6572 7329 3a0a 2020 2020 2727 270a 2020  ers):.    '''.  
+0000d710: 2020 4465 7465 726d 696e 6520 7468 6520    Determine the 
+0000d720: 5369 6d70 6c65 2053 7461 626c 6520 566f  Simple Stable Vo
+0000d730: 7469 6e67 2077 696e 6e65 7273 2077 6869  ting winners whi
+0000d740: 6c65 206b 6565 7069 6e67 2074 7261 636b  le keeping track
+0000d750: 200a 2020 2020 6f66 2074 6865 2077 696e   .    of the win
+0000d760: 6e65 7273 2069 6e20 616e 7920 7375 6270  ners in any subp
+0000d770: 726f 6669 6c65 7320 6368 6563 6b65 6420  rofiles checked 
+0000d780: 6475 7269 6e67 2063 6f6d 7075 7461 7469  during computati
+0000d790: 6f6e 2e20 0a20 2020 2027 2727 0a20 2020  on. .    '''.   
+0000d7a0: 200a 2020 2020 7376 5f77 696e 6e65 7273   .    sv_winners
+0000d7b0: 203d 206c 6973 7428 290a 2020 2020 2020   = list().      
+0000d7c0: 2020 0a20 2020 2069 6620 6c65 6e28 6375    .    if len(cu
+0000d7d0: 7272 5f63 616e 6473 2920 3d3d 2031 3a20  rr_cands) == 1: 
+0000d7e0: 0a20 2020 2020 2020 206d 656d 5f73 765f  .        mem_sv_
+0000d7f0: 7769 6e6e 6572 735b 7475 706c 6528 6375  winners[tuple(cu
+0000d800: 7272 5f63 616e 6473 295d 203d 2063 7572  rr_cands)] = cur
+0000d810: 725f 6361 6e64 730a 2020 2020 2020 2020  r_cands.        
+0000d820: 7265 7475 726e 2063 7572 725f 6361 6e64  return curr_cand
+0000d830: 732c 206d 656d 5f73 765f 7769 6e6e 6572  s, mem_sv_winner
+0000d840: 730a 2020 2020 0a20 2020 206d 6172 6769  s.    .    margi
+0000d850: 6e5f 7769 746e 6573 7369 6e67 5f77 696e  n_witnessing_win
+0000d860: 203d 202d 6d61 7468 2e69 6e66 0a0a 2020   = -math.inf..  
+0000d870: 2020 666f 7220 612c 2062 2c20 7320 696e    for a, b, s in
+0000d880: 2073 6f72 7465 645f 6d61 7463 6865 733a   sorted_matches:
+0000d890: 0a20 2020 2020 2020 2069 6620 7320 3c20  .        if s < 
+0000d8a0: 6d61 7267 696e 5f77 6974 6e65 7373 696e  margin_witnessin
+0000d8b0: 675f 7769 6e3a 200a 2020 2020 2020 2020  g_win: .        
+0000d8c0: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
+0000d8d0: 2020 6966 2061 206e 6f74 2069 6e20 7376    if a not in sv
+0000d8e0: 5f77 696e 6e65 7273 3a20 0a20 2020 2020  _winners: .     
+0000d8f0: 2020 2020 2020 2063 616e 6473 5f6d 696e         cands_min
+0000d900: 7573 5f62 203d 205b 6320 666f 7220 6320  us_b = [c for c 
+0000d910: 696e 2063 7572 725f 6361 6e64 7320 6966  in curr_cands if
+0000d920: 2063 2021 3d20 625d 0a20 2020 2020 2020   c != b].       
+0000d930: 2020 2020 2063 616e 6473 5f6d 696e 7573       cands_minus
+0000d940: 5f62 5f6b 6579 203d 2074 7570 6c65 2873  _b_key = tuple(s
+0000d950: 6f72 7465 6428 6361 6e64 735f 6d69 6e75  orted(cands_minu
+0000d960: 735f 6229 290a 2020 2020 2020 2020 2020  s_b)).          
+0000d970: 2020 6966 2063 616e 6473 5f6d 696e 7573    if cands_minus
+0000d980: 5f62 5f6b 6579 206e 6f74 2069 6e20 6d65  _b_key not in me
+0000d990: 6d5f 7376 5f77 696e 6e65 7273 2e6b 6579  m_sv_winners.key
+0000d9a0: 7328 293a 200a 2020 2020 2020 2020 2020  s(): .          
+0000d9b0: 2020 2020 2020 7773 2c20 6d65 6d5f 7376        ws, mem_sv
+0000d9c0: 5f77 696e 6e65 7273 203d 205f 7369 6d70  _winners = _simp
+0000d9d0: 6c65 5f73 7461 626c 655f 766f 7469 6e67  le_stable_voting
+0000d9e0: 2863 7572 725f 6361 6e64 7320 3d20 6361  (curr_cands = ca
+0000d9f0: 6e64 735f 6d69 6e75 735f 622c 0a20 2020  nds_minus_b,.   
+0000da00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da30: 2020 2020 2020 2020 736f 7274 6564 5f6d          sorted_m
+0000da40: 6174 6368 6573 203d 205b 2861 2c20 632c  atches = [(a, c,
+0000da50: 2073 2920 666f 7220 612c 2063 2c20 7320   s) for a, c, s 
+0000da60: 696e 2073 6f72 7465 645f 6d61 7463 6865  in sorted_matche
+0000da70: 7320 6966 2061 2021 3d20 6220 616e 6420  s if a != b and 
+0000da80: 6320 213d 2062 5d2c 0a20 2020 2020 2020  c != b],.       
+0000da90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000daa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dac0: 2020 2020 6d65 6d5f 7376 5f77 696e 6e65      mem_sv_winne
+0000dad0: 7273 203d 206d 656d 5f73 765f 7769 6e6e  rs = mem_sv_winn
+0000dae0: 6572 7329 0a20 2020 2020 2020 2020 2020  ers).           
+0000daf0: 2020 2020 206d 656d 5f73 765f 7769 6e6e       mem_sv_winn
+0000db00: 6572 735b 6361 6e64 735f 6d69 6e75 735f  ers[cands_minus_
+0000db10: 625f 6b65 795d 203d 2077 730a 2020 2020  b_key] = ws.    
+0000db20: 2020 2020 2020 2020 656c 7365 3a20 0a20          else: . 
+0000db30: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+0000db40: 7320 3d20 6d65 6d5f 7376 5f77 696e 6e65  s = mem_sv_winne
+0000db50: 7273 5b63 616e 6473 5f6d 696e 7573 5f62  rs[cands_minus_b
+0000db60: 5f6b 6579 5d0a 2020 2020 2020 2020 2020  _key].          
+0000db70: 2020 6966 2061 2069 6e20 7773 3a0a 2020    if a in ws:.  
+0000db80: 2020 2020 2020 2020 2020 2020 2020 7376                sv
+0000db90: 5f77 696e 6e65 7273 2e61 7070 656e 6428  _winners.append(
+0000dba0: 6129 0a20 2020 2020 2020 2020 2020 2020  a).             
+0000dbb0: 2020 206d 6172 6769 6e5f 7769 746e 6573     margin_witnes
+0000dbc0: 7369 6e67 5f77 696e 203d 2073 0a0a 2020  sing_win = s..  
+0000dbd0: 2020 7265 7475 726e 2073 765f 7769 6e6e    return sv_winn
+0000dbe0: 6572 732c 206d 656d 5f73 765f 7769 6e6e  ers, mem_sv_winn
+0000dbf0: 6572 730a 2020 2020 0a0a 4076 6d28 6e61  ers.    ..@vm(na
+0000dc00: 6d65 203d 2022 5369 6d70 6c65 2053 7461  me = "Simple Sta
+0000dc10: 626c 6520 566f 7469 6e67 2229 0a64 6566  ble Voting").def
+0000dc20: 205f 7369 6d70 6c65 5f73 7461 626c 655f   _simple_stable_
+0000dc30: 766f 7469 6e67 5f77 6974 685f 636f 6e64  voting_with_cond
+0000dc40: 6f72 6365 745f 6368 6563 6b28 0a20 2020  orcet_check(.   
+0000dc50: 2065 6461 7461 2c20 0a20 2020 2063 7572   edata, .    cur
+0000dc60: 725f 6361 6e64 7320 3d20 4e6f 6e65 2c20  r_cands = None, 
+0000dc70: 0a20 2020 2073 7472 656e 6774 685f 6675  .    strength_fu
+0000dc80: 6e63 7469 6f6e 203d 204e 6f6e 6529 3a20  nction = None): 
+0000dc90: 0a20 2020 2022 2222 5369 6d70 6c65 2053  .    """Simple S
+0000dca0: 7461 626c 6520 566f 7469 6e67 2069 7320  table Voting is 
+0000dcb0: 436f 6e64 6f72 6365 7420 636f 6e73 6973  Condorcet consis
+0000dcc0: 7465 6e74 2e20 2020 4974 2069 7320 6661  tent.   It is fa
+0000dcd0: 7374 6572 2074 6f20 736b 6970 2065 7865  ster to skip exe
+0000dce0: 6375 7469 6e67 2074 6865 2072 6563 7572  cuting the recur
+0000dcf0: 7369 7665 2061 6c67 6f72 6974 686d 2077  sive algorithm w
+0000dd00: 6865 6e20 7468 6572 6520 6973 2061 2043  hen there is a C
+0000dd10: 6f6e 646f 7263 6574 2077 696e 6e65 7246  ondorcet winnerF
+0000dd20: 6972 7374 2063 6865 636b 2069 6620 7468  irst check if th
+0000dd30: 6572 6520 6973 2061 2043 6f6e 646f 7263  ere is a Condorc
+0000dd40: 6574 2077 696e 6e65 722e 2020 4966 2073  et winner.  If s
+0000dd50: 6f2c 2072 6574 7572 6e20 7468 6520 436f  o, return the Co
+0000dd60: 6e64 6f72 6365 7420 7769 6e6e 6572 2c20  ndorcet winner, 
+0000dd70: 6f74 6865 7277 6973 6520 6669 6e64 2074  otherwise find t
+0000dd80: 6865 2053 696d 706c 6520 5374 6162 6c65  he Simple Stable
+0000dd90: 2056 6f74 696e 6720 7769 6e6e 6572 2075   Voting winner u
+0000dda0: 7369 6e67 205f 7369 6d70 6c65 5f73 7461  sing _simple_sta
+0000ddb0: 626c 655f 766f 7469 6e67 0a0a 2020 2020  ble_voting..    
+0000ddc0: 4172 6773 3a0a 2020 2020 2020 2020 6564  Args:.        ed
+0000ddd0: 6174 6120 2850 726f 6669 6c65 2c20 5072  ata (Profile, Pr
+0000dde0: 6f66 696c 6557 6974 6854 6965 732c 204d  ofileWithTies, M
+0000ddf0: 6172 6769 6e47 7261 7068 293a 2041 6e79  arginGraph): Any
+0000de00: 2065 6c65 6374 696f 6e20 6461 7461 2074   election data t
+0000de10: 6861 7420 6861 7320 6120 606d 6172 6769  hat has a `margi
+0000de20: 6e60 206d 6574 686f 642e 200a 2020 2020  n` method. .    
+0000de30: 2020 2020 6375 7272 5f63 616e 6473 2028      curr_cands (
+0000de40: 4c69 7374 5b69 6e74 5d2c 206f 7074 696f  List[int], optio
+0000de50: 6e61 6c29 3a20 4966 2073 6574 2c20 7468  nal): If set, th
+0000de60: 656e 2066 696e 6420 7468 6520 7769 6e6e  en find the winn
+0000de70: 6572 7320 666f 7220 7468 6520 7072 6f66  ers for the prof
+0000de80: 696c 6520 7265 7374 7269 6374 6564 2074  ile restricted t
+0000de90: 6f20 7468 6520 6361 6e64 6964 6174 6573  o the candidates
+0000dea0: 2069 6e20 6060 6375 7272 5f63 616e 6473   in ``curr_cands
+0000deb0: 6060 0a20 2020 2020 2020 2073 7472 656e  ``.        stren
+0000dec0: 6774 685f 6675 6e63 7469 6f6e 2028 6675  gth_function (fu
+0000ded0: 6e63 7469 6f6e 2c20 6f70 7469 6f6e 616c  nction, optional
+0000dee0: 293a 2054 6865 2073 7472 656e 6774 6820  ): The strength 
+0000def0: 6675 6e63 7469 6f6e 2074 6f20 6265 2075  function to be u
+0000df00: 7365 6420 746f 2063 616c 6375 6c61 7465  sed to calculate
+0000df10: 2074 6865 2073 7472 656e 6774 6820 6f66   the strength of
+0000df20: 2061 2070 6174 682e 2020 2054 6865 2064   a path.   The d
+0000df30: 6566 6175 6c74 2069 7320 7468 6520 6d61  efault is the ma
+0000df40: 7267 696e 206d 6574 686f 6420 6f66 2060  rgin method of `
+0000df50: 6065 6461 7461 6060 2e20 2020 5468 6973  `edata``.   This
+0000df60: 206f 6e6c 7920 6d61 7474 6572 7320 7768   only matters wh
+0000df70: 656e 2074 6865 2062 616c 6c6f 7473 2061  en the ballots a
+0000df80: 7265 206e 6f74 206c 696e 6561 7220 6f72  re not linear or
+0000df90: 6465 7273 2e20 0a0a 2020 2020 5265 7475  ders. ..    Retu
+0000dfa0: 726e 733a 200a 2020 2020 2020 2020 4120  rns: .        A 
+0000dfb0: 736f 7274 6564 206c 6973 7420 6f66 2063  sorted list of c
+0000dfc0: 616e 6469 6461 7465 732e 200a 0a20 2020  andidates. ..   
+0000dfd0: 2022 2222 0a20 2020 200a 2020 2020 6377   """.    .    cw
+0000dfe0: 203d 2065 6461 7461 2e63 6f6e 646f 7263   = edata.condorc
+0000dff0: 6574 5f77 696e 6e65 7228 6375 7272 5f63  et_winner(curr_c
+0000e000: 616e 6473 203d 2063 7572 725f 6361 6e64  ands = curr_cand
+0000e010: 7329 0a20 2020 2069 6620 6377 2069 7320  s).    if cw is 
+0000e020: 6e6f 7420 4e6f 6e65 3a20 0a20 2020 2020  not None: .     
+0000e030: 2020 2072 6574 7572 6e20 5b63 775d 0a20     return [cw]. 
+0000e040: 2020 2065 6c73 653a 200a 2020 2020 2020     else: .      
+0000e050: 2020 6375 7272 5f63 616e 6473 203d 2065    curr_cands = e
+0000e060: 6461 7461 2e63 616e 6469 6461 7465 7320  data.candidates 
+0000e070: 6966 2063 7572 725f 6361 6e64 7320 6973  if curr_cands is
+0000e080: 204e 6f6e 6520 656c 7365 2063 7572 725f   None else curr_
+0000e090: 6361 6e64 730a 2020 2020 2020 2020 7374  cands.        st
+0000e0a0: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
+0000e0b0: 3d20 6564 6174 612e 6d61 7267 696e 2069  = edata.margin i
+0000e0c0: 6620 7374 7265 6e67 7468 5f66 756e 6374  f strength_funct
+0000e0d0: 696f 6e20 6973 204e 6f6e 6520 656c 7365  ion is None else
+0000e0e0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+0000e0f0: 6f6e 2020 0a0a 2020 2020 2020 2020 6d61  on  ..        ma
+0000e100: 7463 6865 7320 3d20 5b28 612c 2062 2c20  tches = [(a, b, 
+0000e110: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+0000e120: 6e28 612c 2062 2929 2066 6f72 2061 2069  n(a, b)) for a i
+0000e130: 6e20 6375 7272 5f63 616e 6473 2066 6f72  n curr_cands for
+0000e140: 2062 2069 6e20 6375 7272 5f63 616e 6473   b in curr_cands
+0000e150: 2069 6620 6120 213d 2062 5d0a 2020 2020   if a != b].    
+0000e160: 2020 2020 736f 7274 6564 5f6d 6174 6368      sorted_match
+0000e170: 6573 203d 2073 6f72 7465 6428 6d61 7463  es = sorted(matc
+0000e180: 6865 732c 2072 6576 6572 7365 3d54 7275  hes, reverse=Tru
+0000e190: 652c 206b 6579 3d6c 616d 6264 6120 6d5f  e, key=lambda m_
+0000e1a0: 775f 7765 6967 6874 3a20 6d5f 775f 7765  w_weight: m_w_we
+0000e1b0: 6967 6874 5b32 5d29 0a20 2020 200a 2020  ight[2]).    .  
+0000e1c0: 2020 2020 2020 7265 7475 726e 2073 6f72        return sor
+0000e1d0: 7465 6428 5f73 696d 706c 655f 7374 6162  ted(_simple_stab
+0000e1e0: 6c65 5f76 6f74 696e 6728 6375 7272 5f63  le_voting(curr_c
+0000e1f0: 616e 6473 203d 2063 7572 725f 6361 6e64  ands = curr_cand
+0000e200: 732c 200a 2020 2020 2020 2020 2020 2020  s, .            
+0000e210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e230: 736f 7274 6564 5f6d 6174 6368 6573 203d  sorted_matches =
+0000e240: 2073 6f72 7465 645f 6d61 7463 6865 732c   sorted_matches,
+0000e250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e270: 2020 2020 2020 2020 2020 2020 206d 656d               mem
+0000e280: 5f73 765f 7769 6e6e 6572 7320 3d20 7b7d  _sv_winners = {}
+0000e290: 295b 305d 290a 0a0a 6465 6620 5f73 696d  )[0])...def _sim
+0000e2a0: 706c 655f 7374 6162 6c65 5f76 6f74 696e  ple_stable_votin
+0000e2b0: 675f 6261 7369 6328 6564 6174 612c 2063  g_basic(edata, c
+0000e2c0: 7572 725f 6361 6e64 7320 3d20 4e6f 6e65  urr_cands = None
+0000e2d0: 2c20 7374 7265 6e67 7468 5f66 756e 6374  , strength_funct
+0000e2e0: 696f 6e20 3d20 4e6f 6e65 293a 200a 2020  ion = None): .  
+0000e2f0: 2020 2222 2249 6d70 6c65 6d65 6e74 6174    """Implementat
+0000e300: 696f 6e20 6f66 2053 696d 706c 6520 5374  ion of Simple St
+0000e310: 6162 6c65 2056 6f74 696e 6720 6672 6f6d  able Voting from
+0000e320: 2068 7474 7073 3a2f 2f61 7278 6976 2e6f   https://arxiv.o
+0000e330: 7267 2f61 6273 2f32 3130 382e 3030 3534  rg/abs/2108.0054
+0000e340: 322e 200a 0a20 2020 2041 7267 733a 0a20  2. ..    Args:. 
+0000e350: 2020 2020 2020 2065 6461 7461 2028 5072         edata (Pr
+0000e360: 6f66 696c 652c 2050 726f 6669 6c65 5769  ofile, ProfileWi
+0000e370: 7468 5469 6573 2c20 4d61 7267 696e 4772  thTies, MarginGr
+0000e380: 6170 6829 3a20 416e 7920 656c 6563 7469  aph): Any electi
+0000e390: 6f6e 2064 6174 6120 7468 6174 2068 6173  on data that has
+0000e3a0: 2061 2060 6d61 7267 696e 6020 6d65 7468   a `margin` meth
+0000e3b0: 6f64 2e20 0a20 2020 2020 2020 2063 7572  od. .        cur
+0000e3c0: 725f 6361 6e64 7320 284c 6973 745b 696e  r_cands (List[in
+0000e3d0: 745d 2c20 6f70 7469 6f6e 616c 293a 2049  t], optional): I
+0000e3e0: 6620 7365 742c 2074 6865 6e20 6669 6e64  f set, then find
+0000e3f0: 2074 6865 2077 696e 6e65 7273 2066 6f72   the winners for
+0000e400: 2074 6865 2070 726f 6669 6c65 2072 6573   the profile res
+0000e410: 7472 6963 7465 6420 746f 2074 6865 2063  tricted to the c
+0000e420: 616e 6469 6461 7465 7320 696e 2060 6063  andidates in ``c
+0000e430: 7572 725f 6361 6e64 7360 600a 2020 2020  urr_cands``.    
+0000e440: 2020 2020 7374 7265 6e67 7468 5f66 756e      strength_fun
+0000e450: 6374 696f 6e20 2866 756e 6374 696f 6e2c  ction (function,
+0000e460: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
+0000e470: 7374 7265 6e67 7468 2066 756e 6374 696f  strength functio
+0000e480: 6e20 746f 2062 6520 7573 6564 2074 6f20  n to be used to 
+0000e490: 6361 6c63 756c 6174 6520 7468 6520 7374  calculate the st
+0000e4a0: 7265 6e67 7468 206f 6620 6120 7061 7468  rength of a path
+0000e4b0: 2e20 2020 5468 6520 6465 6661 756c 7420  .   The default 
+0000e4c0: 6973 2074 6865 206d 6172 6769 6e20 6d65  is the margin me
+0000e4d0: 7468 6f64 206f 6620 6060 6564 6174 6160  thod of ``edata`
+0000e4e0: 602e 2020 2054 6869 7320 6f6e 6c79 206d  `.   This only m
+0000e4f0: 6174 7465 7273 2077 6865 6e20 7468 6520  atters when the 
+0000e500: 6261 6c6c 6f74 7320 6172 6520 6e6f 7420  ballots are not 
+0000e510: 6c69 6e65 6172 206f 7264 6572 732e 200a  linear orders. .
+0000e520: 0a20 2020 2052 6574 7572 6e73 3a20 0a20  .    Returns: . 
+0000e530: 2020 2020 2020 2041 2073 6f72 7465 6420         A sorted 
+0000e540: 6c69 7374 206f 6620 6361 6e64 6964 6174  list of candidat
+0000e550: 6573 2e20 0a0a 2020 2020 2222 220a 2020  es. ..    """.  
+0000e560: 2020 0a20 2020 2063 7572 725f 6361 6e64    .    curr_cand
+0000e570: 7320 3d20 6564 6174 612e 6361 6e64 6964  s = edata.candid
+0000e580: 6174 6573 2069 6620 6375 7272 5f63 616e  ates if curr_can
+0000e590: 6473 2069 7320 4e6f 6e65 2065 6c73 6520  ds is None else 
+0000e5a0: 6375 7272 5f63 616e 6473 0a20 2020 2073  curr_cands.    s
+0000e5b0: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+0000e5c0: 203d 2065 6461 7461 2e6d 6172 6769 6e20   = edata.margin 
+0000e5d0: 6966 2073 7472 656e 6774 685f 6675 6e63  if strength_func
+0000e5e0: 7469 6f6e 2069 7320 4e6f 6e65 2065 6c73  tion is None els
+0000e5f0: 6520 7374 7265 6e67 7468 5f66 756e 6374  e strength_funct
+0000e600: 696f 6e20 200a 0a20 2020 206d 6174 6368  ion  ..    match
+0000e610: 6573 203d 205b 2861 2c20 622c 2073 7472  es = [(a, b, str
+0000e620: 656e 6774 685f 6675 6e63 7469 6f6e 2861  ength_function(a
+0000e630: 2c20 6229 2920 666f 7220 6120 696e 2063  , b)) for a in c
+0000e640: 7572 725f 6361 6e64 7320 666f 7220 6220  urr_cands for b 
+0000e650: 696e 2063 7572 725f 6361 6e64 7320 6966  in curr_cands if
+0000e660: 2061 2021 3d20 625d 0a20 2020 2073 6f72   a != b].    sor
+0000e670: 7465 645f 6d61 7463 6865 7320 3d20 736f  ted_matches = so
+0000e680: 7274 6564 286d 6174 6368 6573 2c20 7265  rted(matches, re
+0000e690: 7665 7273 653d 5472 7565 2c20 6b65 793d  verse=True, key=
+0000e6a0: 6c61 6d62 6461 206d 5f77 5f77 6569 6768  lambda m_w_weigh
+0000e6b0: 743a 206d 5f77 5f77 6569 6768 745b 325d  t: m_w_weight[2]
+0000e6c0: 290a 2020 2020 0a20 2020 2072 6574 7572  ).    .    retur
+0000e6d0: 6e20 736f 7274 6564 285f 7369 6d70 6c65  n sorted(_simple
+0000e6e0: 5f73 7461 626c 655f 766f 7469 6e67 2863  _stable_voting(c
+0000e6f0: 7572 725f 6361 6e64 7320 3d20 6375 7272  urr_cands = curr
+0000e700: 5f63 616e 6473 2c20 0a20 2020 2020 2020  _cands, .       
+0000e710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e730: 2073 6f72 7465 645f 6d61 7463 6865 7320   sorted_matches 
+0000e740: 3d20 736f 7274 6564 5f6d 6174 6368 6573  = sorted_matches
+0000e750: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000e760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e770: 2020 2020 2020 2020 2020 6d65 6d5f 7376            mem_sv
+0000e780: 5f77 696e 6e65 7273 203d 207b 7d29 5b30  _winners = {})[0
+0000e790: 5d29 0a0a 7373 765f 7072 6f70 6572 7469  ])..ssv_properti
+0000e7a0: 6573 203d 2056 6f74 696e 674d 6574 686f  es = VotingMetho
+0000e7b0: 6450 726f 7065 7274 6965 7328 0a20 2020  dProperties(.   
+0000e7c0: 2063 6f6e 646f 7263 6574 5f77 696e 6e65   condorcet_winne
+0000e7d0: 723d 5472 7565 2c20 0a20 2020 2063 6f6e  r=True, .    con
+0000e7e0: 646f 7263 6574 5f6c 6f73 6572 3d54 7275  dorcet_loser=Tru
+0000e7f0: 652c 0a20 2020 2070 6172 6574 6f5f 646f  e,.    pareto_do
+0000e800: 6d69 6e61 6e63 653d 5472 7565 2c20 0a20  minance=True, . 
+0000e810: 2020 2029 0a40 766d 286e 616d 6520 3d20     ).@vm(name = 
+0000e820: 2253 696d 706c 6520 5374 6162 6c65 2056  "Simple Stable V
+0000e830: 6f74 696e 6722 2c0a 2020 2020 7072 6f70  oting",.    prop
+0000e840: 6572 7469 6573 203d 2073 7376 5f70 726f  erties = ssv_pro
+0000e850: 7065 7274 6965 732c 0a20 2020 2069 6e70  perties,.    inp
+0000e860: 7574 5f74 7970 6573 203d 205b 456c 6563  ut_types = [Elec
+0000e870: 7469 6f6e 5479 7065 732e 5052 4f46 494c  tionTypes.PROFIL
+0000e880: 452c 2045 6c65 6374 696f 6e54 7970 6573  E, ElectionTypes
+0000e890: 2e50 524f 4649 4c45 5f57 4954 485f 5449  .PROFILE_WITH_TI
+0000e8a0: 4553 2c20 456c 6563 7469 6f6e 5479 7065  ES, ElectionType
+0000e8b0: 732e 4d41 5247 494e 5f47 5241 5048 5d29  s.MARGIN_GRAPH])
+0000e8c0: 0a64 6566 2073 696d 706c 655f 7374 6162  .def simple_stab
+0000e8d0: 6c65 5f76 6f74 696e 6728 0a20 2020 2065  le_voting(.    e
+0000e8e0: 6461 7461 2c20 0a20 2020 2063 7572 725f  data, .    curr_
+0000e8f0: 6361 6e64 733d 4e6f 6e65 2c20 0a20 2020  cands=None, .   
+0000e900: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+0000e910: 6f6e 3d4e 6f6e 652c 0a20 2020 2061 6c67  on=None,.    alg
+0000e920: 6f72 6974 686d 203d 2027 6261 7369 6327  orithm = 'basic'
+0000e930: 293a 200a 0a20 2020 2022 2222 496d 706c  ): ..    """Impl
+0000e940: 656d 656e 7461 7469 6f6e 206f 6620 5369  ementation of Si
+0000e950: 6d70 6c65 2053 7461 626c 6520 566f 7469  mple Stable Voti
+0000e960: 6e67 2066 726f 6d20 6874 7470 733a 2f2f  ng from https://
+0000e970: 6172 7869 762e 6f72 672f 6162 732f 3231  arxiv.org/abs/21
+0000e980: 3038 2e30 3035 3432 2e20 0a0a 2020 2020  08.00542. ..    
+0000e990: 5369 6d70 6c65 2053 7461 626c 6520 566f  Simple Stable Vo
+0000e9a0: 7469 6e67 2069 7320 6120 7265 6375 7273  ting is a recurs
+0000e9b0: 6976 6520 766f 7469 6e67 206d 6574 686f  ive voting metho
+0000e9c0: 6420 6465 6669 6e65 6420 6173 2066 6f6c  d defined as fol
+0000e9d0: 6c6f 7773 3a20 0a0a 2020 2020 312e 2049  lows: ..    1. I
+0000e9e0: 6620 7468 6572 6520 6973 206f 6e6c 7920  f there is only 
+0000e9f0: 6f6e 6520 6361 6e64 6964 6174 6520 696e  one candidate in
+0000ea00: 2074 6865 2070 726f 6669 6c65 2c20 7468   the profile, th
+0000ea10: 656e 2074 6861 7420 6361 6e64 6964 6174  en that candidat
+0000ea20: 6520 6973 2074 6865 2077 696e 6e65 722e  e is the winner.
+0000ea30: 200a 2020 2020 322e 204f 7264 6572 2074   .    2. Order t
+0000ea40: 6865 2070 6169 7273 203a 6d61 7468 3a60  he pairs :math:`
+0000ea50: 2861 2c62 2960 206f 6620 6361 6e64 6964  (a,b)` of candid
+0000ea60: 6174 6573 2066 726f 6d20 6c61 7267 6573  ates from larges
+0000ea70: 7420 746f 2073 6d61 6c6c 6573 7420 7661  t to smallest va
+0000ea80: 6c75 6520 6f66 2074 6865 206d 6172 6769  lue of the margi
+0000ea90: 6e20 6f66 203a 6d61 7468 3a60 6160 206f  n of :math:`a` o
+0000eaa0: 7665 7220 3a6d 6174 683a 6062 602c 2061  ver :math:`b`, a
+0000eab0: 6e64 2064 6563 6c61 7265 2061 7320 5369  nd declare as Si
+0000eac0: 6d70 6c65 2053 7461 626c 6520 566f 7469  mple Stable Voti
+0000ead0: 6e67 2077 696e 6e65 7273 2074 6865 2063  ng winners the c
+0000eae0: 616e 6469 6461 7465 2873 2920 3a6d 6174  andidate(s) :mat
+0000eaf0: 683a 6061 6020 6672 6f6d 2074 6865 2065  h:`a` from the e
+0000eb00: 6172 6c69 6573 7420 7061 6972 2873 2920  arliest pair(s) 
+0000eb10: 3a6d 6174 683a 6028 612c 6229 6020 7375  :math:`(a,b)` su
+0000eb20: 6368 2074 6861 7420 3a6d 6174 683a 6061  ch that :math:`a
+0000eb30: 6020 6973 2061 2053 696d 706c 6520 5374  ` is a Simple St
+0000eb40: 6162 6c65 2056 6f74 696e 6720 7769 6e6e  able Voting winn
+0000eb50: 6572 2069 6e20 7468 6520 656c 6563 7469  er in the electi
+0000eb60: 6f6e 2077 6974 686f 7574 203a 6d61 7468  on without :math
+0000eb70: 3a60 6260 2e20 0a0a 2020 2020 4172 6773  :`b`. ..    Args
+0000eb80: 3a0a 2020 2020 2020 2020 6564 6174 6120  :.        edata 
+0000eb90: 2850 726f 6669 6c65 2c20 5072 6f66 696c  (Profile, Profil
+0000eba0: 6557 6974 6854 6965 732c 204d 6172 6769  eWithTies, Margi
+0000ebb0: 6e47 7261 7068 293a 2041 6e79 2065 6c65  nGraph): Any ele
+0000ebc0: 6374 696f 6e20 6461 7461 2074 6861 7420  ction data that 
+0000ebd0: 6861 7320 6120 606d 6172 6769 6e60 206d  has a `margin` m
+0000ebe0: 6574 686f 642e 200a 2020 2020 2020 2020  ethod. .        
+0000ebf0: 6375 7272 5f63 616e 6473 2028 4c69 7374  curr_cands (List
+0000ec00: 5b69 6e74 5d2c 206f 7074 696f 6e61 6c29  [int], optional)
+0000ec10: 3a20 4966 2073 6574 2c20 7468 656e 2066  : If set, then f
+0000ec20: 696e 6420 7468 6520 7769 6e6e 6572 7320  ind the winners 
+0000ec30: 666f 7220 7468 6520 7072 6f66 696c 6520  for the profile 
+0000ec40: 7265 7374 7269 6374 6564 2074 6f20 7468  restricted to th
+0000ec50: 6520 6361 6e64 6964 6174 6573 2069 6e20  e candidates in 
+0000ec60: 6060 6375 7272 5f63 616e 6473 6060 0a20  ``curr_cands``. 
+0000ec70: 2020 2020 2020 2073 7472 656e 6774 685f         strength_
+0000ec80: 6675 6e63 7469 6f6e 2028 6675 6e63 7469  function (functi
+0000ec90: 6f6e 2c20 6f70 7469 6f6e 616c 293a 2054  on, optional): T
+0000eca0: 6865 2073 7472 656e 6774 6820 6675 6e63  he strength func
+0000ecb0: 7469 6f6e 2074 6f20 6265 2075 7365 6420  tion to be used 
+0000ecc0: 746f 2063 616c 6375 6c61 7465 2074 6865  to calculate the
+0000ecd0: 2073 7472 656e 6774 6820 6f66 2061 2070   strength of a p
+0000ece0: 6174 682e 2020 2054 6865 2064 6566 6175  ath.   The defau
+0000ecf0: 6c74 2069 7320 7468 6520 6d61 7267 696e  lt is the margin
+0000ed00: 206d 6574 686f 6420 6f66 2060 6065 6461   method of ``eda
+0000ed10: 7461 6060 2e20 2020 5468 6973 206f 6e6c  ta``.   This onl
+0000ed20: 7920 6d61 7474 6572 7320 7768 656e 2074  y matters when t
+0000ed30: 6865 2062 616c 6c6f 7473 2061 7265 206e  he ballots are n
+0000ed40: 6f74 206c 696e 6561 7220 6f72 6465 7273  ot linear orders
+0000ed50: 2e20 0a20 2020 2020 2020 2061 6c67 6f72  . .        algor
+0000ed60: 6974 686d 2028 7374 722c 206f 7074 696f  ithm (str, optio
+0000ed70: 6e61 6c29 3a20 5370 6563 6966 7920 7768  nal): Specify wh
+0000ed80: 6963 6820 616c 676f 7269 7468 6d20 746f  ich algorithm to
+0000ed90: 2075 7365 2e20 204f 7074 696f 6e73 2061   use.  Options a
+0000eda0: 7265 2027 6261 7369 6327 2028 7468 6520  re 'basic' (the 
+0000edb0: 6465 6661 756c 7429 2061 6e64 2027 7769  default) and 'wi
+0000edc0: 7468 5f63 6f6e 646f 7263 6574 5f63 6865  th_condorcet_che
+0000edd0: 636b 272e 0a0a 2020 2020 5265 7475 726e  ck'...    Return
+0000ede0: 733a 200a 2020 2020 2020 2020 4120 736f  s: .        A so
+0000edf0: 7274 6564 206c 6973 7420 6f66 2063 616e  rted list of can
+0000ee00: 6469 6461 7465 732e 200a 0a20 2020 202e  didates. ..    .
+0000ee10: 2e20 7365 6561 6c73 6f3a 3a0a 0a20 2020  . seealso::..   
+0000ee20: 2020 2020 203a 6d65 7468 3a60 7072 6566       :meth:`pref
+0000ee30: 5f76 6f74 696e 672e 6d61 7267 696e 5f62  _voting.margin_b
+0000ee40: 6173 6564 5f6d 6574 686f 6473 2e73 7461  ased_methods.sta
+0000ee50: 626c 655f 766f 7469 6e67 600a 0a20 2020  ble_voting`..   
+0000ee60: 203a 4578 616d 706c 653a 200a 0a20 2020   :Example: ..   
+0000ee70: 202e 2e20 6578 6563 5f63 6f64 653a 3a0a   .. exec_code::.
+0000ee80: 0a20 2020 2020 2020 2066 726f 6d20 7072  .        from pr
+0000ee90: 6566 5f76 6f74 696e 672e 7765 6967 6874  ef_voting.weight
+0000eea0: 6564 5f6d 616a 6f72 6974 795f 6772 6170  ed_majority_grap
+0000eeb0: 6873 2069 6d70 6f72 7420 4d61 7267 696e  hs import Margin
+0000eec0: 4772 6170 680a 2020 2020 2020 2020 6672  Graph.        fr
+0000eed0: 6f6d 2070 7265 665f 766f 7469 6e67 2e6d  om pref_voting.m
+0000eee0: 6172 6769 6e5f 6261 7365 645f 6d65 7468  argin_based_meth
+0000eef0: 6f64 7320 696d 706f 7274 2073 696d 706c  ods import simpl
+0000ef00: 655f 7374 6162 6c65 5f76 6f74 696e 670a  e_stable_voting.
+0000ef10: 0a20 2020 2020 2020 206d 6720 3d20 4d61  .        mg = Ma
+0000ef20: 7267 696e 4772 6170 6828 5b30 2c20 312c  rginGraph([0, 1,
+0000ef30: 2032 2c20 335d 2c20 5b28 302c 2033 2c20   2, 3], [(0, 3, 
+0000ef40: 3829 2c20 2831 2c20 302c 2031 3029 2c20  8), (1, 0, 10), 
+0000ef50: 2832 2c20 302c 2034 292c 2028 322c 2031  (2, 0, 4), (2, 1
+0000ef60: 2c20 3829 2c20 2833 2c20 312c 2038 295d  , 8), (3, 1, 8)]
+0000ef70: 290a 0a20 2020 2020 2020 2073 696d 706c  )..        simpl
+0000ef80: 655f 7374 6162 6c65 5f76 6f74 696e 672e  e_stable_voting.
+0000ef90: 6469 7370 6c61 7928 6d67 290a 2020 2020  display(mg).    
+0000efa0: 2020 2020 7369 6d70 6c65 5f73 7461 626c      simple_stabl
+0000efb0: 655f 766f 7469 6e67 2e64 6973 706c 6179  e_voting.display
+0000efc0: 286d 672c 2061 6c67 6f72 6974 686d 3d27  (mg, algorithm='
+0000efd0: 6261 7369 6327 290a 2020 2020 2020 2020  basic').        
+0000efe0: 7369 6d70 6c65 5f73 7461 626c 655f 766f  simple_stable_vo
+0000eff0: 7469 6e67 2e64 6973 706c 6179 286d 672c  ting.display(mg,
+0000f000: 2061 6c67 6f72 6974 686d 3d27 7769 7468   algorithm='with
+0000f010: 5f63 6f6e 646f 7263 6574 5f63 6865 636b  _condorcet_check
+0000f020: 2729 0a0a 2020 2020 2222 220a 2020 2020  ')..    """.    
+0000f030: 0a20 2020 2069 6620 616c 676f 7269 7468  .    if algorith
+0000f040: 6d20 3d3d 2027 6261 7369 6327 3a20 0a20  m == 'basic': . 
+0000f050: 2020 2020 2020 2072 6574 7572 6e20 5f73         return _s
+0000f060: 696d 706c 655f 7374 6162 6c65 5f76 6f74  imple_stable_vot
+0000f070: 696e 675f 6261 7369 6328 6564 6174 612c  ing_basic(edata,
+0000f080: 2063 7572 725f 6361 6e64 7320 3d20 6375   curr_cands = cu
+0000f090: 7272 5f63 616e 6473 2c20 7374 7265 6e67  rr_cands, streng
+0000f0a0: 7468 5f66 756e 6374 696f 6e20 3d20 7374  th_function = st
+0000f0b0: 7265 6e67 7468 5f66 756e 6374 696f 6e29  rength_function)
+0000f0c0: 0a20 2020 2065 6c69 6620 616c 676f 7269  .    elif algori
+0000f0d0: 7468 6d20 3d3d 2027 7769 7468 5f63 6f6e  thm == 'with_con
+0000f0e0: 646f 7263 6574 5f63 6865 636b 273a 0a20  dorcet_check':. 
+0000f0f0: 2020 2020 2020 2072 6574 7572 6e20 5f73         return _s
+0000f100: 696d 706c 655f 7374 6162 6c65 5f76 6f74  imple_stable_vot
+0000f110: 696e 675f 7769 7468 5f63 6f6e 646f 7263  ing_with_condorc
+0000f120: 6574 5f63 6865 636b 2865 6461 7461 2c20  et_check(edata, 
+0000f130: 6375 7272 5f63 616e 6473 203d 2063 7572  curr_cands = cur
+0000f140: 725f 6361 6e64 732c 2073 7472 656e 6774  r_cands, strengt
+0000f150: 685f 6675 6e63 7469 6f6e 203d 2073 7472  h_function = str
+0000f160: 656e 6774 685f 6675 6e63 7469 6f6e 290a  ength_function).
+0000f170: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000f180: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+0000f190: 6f72 2822 496e 7661 6c69 6420 616c 676f  or("Invalid algo
+0000f1a0: 7269 7468 6d20 7370 6563 6966 6965 642e  rithm specified.
+0000f1b0: 2229 0a20 2020 200a 0a64 6566 205f 7374  ").    ..def _st
+0000f1c0: 6162 6c65 5f76 6f74 696e 6728 6564 6174  able_voting(edat
+0000f1d0: 612c 200a 2020 2020 2020 2020 2020 2020  a, .            
+0000f1e0: 2020 2020 2020 2063 7572 725f 6361 6e64         curr_cand
+0000f1f0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+0000f200: 2020 2020 2020 7374 7265 6e67 7468 5f66        strength_f
+0000f210: 756e 6374 696f 6e2c 0a20 2020 2020 2020  unction,.       
+0000f220: 2020 2020 2020 2020 2020 2020 736f 7274              sort
+0000f230: 6564 5f6d 6174 6368 6573 2c0a 2020 2020  ed_matches,.    
+0000f240: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0000f250: 656d 5f73 765f 7769 6e6e 6572 7329 3a20  em_sv_winners): 
+0000f260: 0a20 2020 2027 2727 0a20 2020 2044 6574  .    '''.    Det
+0000f270: 6572 6d69 6e65 2074 6865 2053 7461 626c  ermine the Stabl
+0000f280: 6520 566f 7469 6e67 2077 696e 6e65 7273  e Voting winners
+0000f290: 2066 6f72 2074 6865 2070 726f 6669 6c65   for the profile
+0000f2a0: 2077 6869 6c65 206b 6565 7069 6e67 2074   while keeping t
+0000f2b0: 7261 636b 206f 6620 7468 6520 7769 6e6e  rack of the winn
+0000f2c0: 6572 7320 696e 2061 6e79 2073 7562 7072  ers in any subpr
+0000f2d0: 6f66 696c 6573 2063 6865 636b 6564 2064  ofiles checked d
+0000f2e0: 7572 696e 6720 636f 6d70 7574 6174 696f  uring computatio
+0000f2f0: 6e2e 200a 2020 2020 2727 270a 2020 2020  n. .    '''.    
+0000f300: 0a20 2020 2073 765f 7769 6e6e 6572 7320  .    sv_winners 
+0000f310: 3d20 6c69 7374 2829 0a20 2020 200a 2020  = list().    .  
+0000f320: 2020 756e 6465 6665 6174 6564 5f63 616e    undefeated_can
+0000f330: 6469 6461 7465 7320 3d20 7370 6c69 745f  didates = split_
+0000f340: 6379 636c 6528 6564 6174 612c 2063 7572  cycle(edata, cur
+0000f350: 725f 6361 6e64 7320 3d20 6375 7272 5f63  r_cands = curr_c
+0000f360: 616e 6473 2c20 7374 7265 6e67 7468 5f66  ands, strength_f
+0000f370: 756e 6374 696f 6e20 3d20 7374 7265 6e67  unction = streng
+0000f380: 7468 5f66 756e 6374 696f 6e29 0a0a 2020  th_function)..  
+0000f390: 2020 6966 206c 656e 2863 7572 725f 6361    if len(curr_ca
+0000f3a0: 6e64 7329 203d 3d20 313a 200a 2020 2020  nds) == 1: .    
+0000f3b0: 2020 2020 6d65 6d5f 7376 5f77 696e 6e65      mem_sv_winne
+0000f3c0: 7273 5b74 7570 6c65 2863 7572 725f 6361  rs[tuple(curr_ca
+0000f3d0: 6e64 7329 5d20 3d20 6375 7272 5f63 616e  nds)] = curr_can
+0000f3e0: 6473 0a20 2020 2020 2020 2072 6574 7572  ds.        retur
+0000f3f0: 6e20 6375 7272 5f63 616e 6473 2c20 6d65  n curr_cands, me
+0000f400: 6d5f 7376 5f77 696e 6e65 7273 0a20 2020  m_sv_winners.   
+0000f410: 200a 2020 2020 6d61 7267 696e 5f77 6974   .    margin_wit
+0000f420: 6e65 7373 696e 675f 7769 6e20 3d20 2d6d  nessing_win = -m
+0000f430: 6174 682e 696e 660a 0a20 2020 2066 6f72  ath.inf..    for
+0000f440: 2061 2c20 622c 2073 2069 6e20 736f 7274   a, b, s in sort
+0000f450: 6564 5f6d 6174 6368 6573 3a0a 2020 2020  ed_matches:.    
+0000f460: 2020 2020 6966 2073 203c 206d 6172 6769      if s < margi
+0000f470: 6e5f 7769 746e 6573 7369 6e67 5f77 696e  n_witnessing_win
+0000f480: 3a20 0a20 2020 2020 2020 2020 2020 2062  : .            b
+0000f490: 7265 616b 0a20 2020 2020 2020 2069 6620  reak.        if 
+0000f4a0: 6120 696e 2075 6e64 6566 6561 7465 645f  a in undefeated_
+0000f4b0: 6361 6e64 6964 6174 6573 2061 6e64 2061  candidates and a
+0000f4c0: 206e 6f74 2069 6e20 7376 5f77 696e 6e65   not in sv_winne
+0000f4d0: 7273 3a20 0a20 2020 2020 2020 2020 2020  rs: .           
+0000f4e0: 2063 616e 6473 5f6d 696e 7573 5f62 203d   cands_minus_b =
+0000f4f0: 205b 6320 666f 7220 6320 696e 2063 7572   [c for c in cur
+0000f500: 725f 6361 6e64 7320 6966 2063 2021 3d20  r_cands if c != 
+0000f510: 625d 0a20 2020 2020 2020 2020 2020 2063  b].            c
+0000f520: 616e 6473 5f6d 696e 7573 5f62 5f6b 6579  ands_minus_b_key
+0000f530: 203d 2074 7570 6c65 2873 6f72 7465 6428   = tuple(sorted(
+0000f540: 6361 6e64 735f 6d69 6e75 735f 6229 290a  cands_minus_b)).
+0000f550: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+0000f560: 616e 6473 5f6d 696e 7573 5f62 5f6b 6579  ands_minus_b_key
+0000f570: 206e 6f74 2069 6e20 6d65 6d5f 7376 5f77   not in mem_sv_w
+0000f580: 696e 6e65 7273 2e6b 6579 7328 293a 200a  inners.keys(): .
+0000f590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f5a0: 7773 2c20 6d65 6d5f 7376 5f77 696e 6e65  ws, mem_sv_winne
+0000f5b0: 7273 203d 205f 7374 6162 6c65 5f76 6f74  rs = _stable_vot
+0000f5c0: 696e 6728 6564 6174 612c 0a20 2020 2020  ing(edata,.     
+0000f5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f5f0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000f600: 7572 725f 6361 6e64 7320 3d20 6361 6e64  urr_cands = cand
+0000f610: 735f 6d69 6e75 735f 622c 0a20 2020 2020  s_minus_b,.     
+0000f620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f640: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000f650: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+0000f660: 203d 2073 7472 656e 6774 685f 6675 6e63   = strength_func
+0000f670: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
+0000f680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f6a0: 2020 2020 2020 2020 2020 736f 7274 6564            sorted
+0000f6b0: 5f6d 6174 6368 6573 203d 205b 2861 2c20  _matches = [(a, 
+0000f6c0: 632c 2073 2920 666f 7220 612c 2063 2c20  c, s) for a, c, 
+0000f6d0: 7320 696e 2073 6f72 7465 645f 6d61 7463  s in sorted_matc
+0000f6e0: 6865 7320 6966 2061 2021 3d20 6220 616e  hes if a != b an
+0000f6f0: 6420 6320 213d 2062 5d2c 0a20 2020 2020  d c != b],.     
+0000f700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f720: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0000f730: 656d 5f73 765f 7769 6e6e 6572 7320 3d20  em_sv_winners = 
+0000f740: 6d65 6d5f 7376 5f77 696e 6e65 7273 290a  mem_sv_winners).
+0000f750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f760: 6d65 6d5f 7376 5f77 696e 6e65 7273 5b63  mem_sv_winners[c
+0000f770: 616e 6473 5f6d 696e 7573 5f62 5f6b 6579  ands_minus_b_key
+0000f780: 5d20 3d20 7773 0a20 2020 2020 2020 2020  ] = ws.         
+0000f790: 2020 2065 6c73 653a 200a 2020 2020 2020     else: .      
+0000f7a0: 2020 2020 2020 2020 2020 7773 203d 206d            ws = m
+0000f7b0: 656d 5f73 765f 7769 6e6e 6572 735b 6361  em_sv_winners[ca
+0000f7c0: 6e64 735f 6d69 6e75 735f 625f 6b65 795d  nds_minus_b_key]
+0000f7d0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000f7e0: 6120 696e 2077 733a 0a20 2020 2020 2020  a in ws:.       
+0000f7f0: 2020 2020 2020 2020 2073 765f 7769 6e6e           sv_winn
+0000f800: 6572 732e 6170 7065 6e64 2861 290a 2020  ers.append(a).  
+0000f810: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+0000f820: 7267 696e 5f77 6974 6e65 7373 696e 675f  rgin_witnessing_
+0000f830: 7769 6e20 3d20 730a 2020 2020 2020 2020  win = s.        
+0000f840: 2020 2020 2020 2020 0a20 2020 2072 6574          .    ret
+0000f850: 7572 6e20 7376 5f77 696e 6e65 7273 2c20  urn sv_winners, 
+0000f860: 6d65 6d5f 7376 5f77 696e 6e65 7273 0a20  mem_sv_winners. 
+0000f870: 2020 2020 2020 200a 6465 6620 5f73 7461         .def _sta
+0000f880: 626c 655f 766f 7469 6e67 5f77 6974 685f  ble_voting_with_
+0000f890: 636f 6e64 6f72 6365 745f 6368 6563 6b28  condorcet_check(
+0000f8a0: 0a20 2020 2065 6461 7461 2c20 0a20 2020  .    edata, .   
+0000f8b0: 2063 7572 725f 6361 6e64 733d 4e6f 6e65   curr_cands=None
+0000f8c0: 2c20 0a20 2020 2073 7472 656e 6774 685f  , .    strength_
+0000f8d0: 6675 6e63 7469 6f6e 3d4e 6f6e 6529 3a20  function=None): 
+0000f8e0: 0a20 2020 2022 2222 0a20 2020 2053 7461  .    """.    Sta
+0000f8f0: 626c 6520 566f 7469 6e67 2069 7320 436f  ble Voting is Co
+0000f900: 6e64 6f72 6365 7420 636f 6e73 6973 7465  ndorcet consiste
+0000f910: 6e74 2e20 2020 4974 2069 7320 6661 7374  nt.   It is fast
+0000f920: 6572 2074 6f20 736b 6970 2065 7865 6375  er to skip execu
+0000f930: 7469 6e67 2074 6865 2072 6563 7572 7369  ting the recursi
+0000f940: 7665 2061 6c67 6f72 6974 686d 2077 6865  ve algorithm whe
+0000f950: 6e20 7468 6572 6520 6973 2061 2043 6f6e  n there is a Con
+0000f960: 646f 7263 6574 2077 696e 6e65 722e 2020  dorcet winner.  
+0000f970: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+0000f980: 2020 2020 6564 6174 6120 2850 726f 6669      edata (Profi
+0000f990: 6c65 2c20 5072 6f66 696c 6557 6974 6854  le, ProfileWithT
+0000f9a0: 6965 732c 204d 6172 6769 6e47 7261 7068  ies, MarginGraph
+0000f9b0: 293a 2041 6e79 2065 6c65 6374 696f 6e20  ): Any election 
+0000f9c0: 6461 7461 2074 6861 7420 6861 7320 6120  data that has a 
+0000f9d0: 606d 6172 6769 6e60 206d 6574 686f 642e  `margin` method.
+0000f9e0: 200a 2020 2020 2020 2020 6375 7272 5f63   .        curr_c
+0000f9f0: 616e 6473 2028 4c69 7374 5b69 6e74 5d2c  ands (List[int],
+0000fa00: 206f 7074 696f 6e61 6c29 3a20 4966 2073   optional): If s
+0000fa10: 6574 2c20 7468 656e 2066 696e 6420 7468  et, then find th
+0000fa20: 6520 7769 6e6e 6572 7320 666f 7220 7468  e winners for th
+0000fa30: 6520 7072 6f66 696c 6520 7265 7374 7269  e profile restri
+0000fa40: 6374 6564 2074 6f20 7468 6520 6361 6e64  cted to the cand
+0000fa50: 6964 6174 6573 2069 6e20 6060 6375 7272  idates in ``curr
+0000fa60: 5f63 616e 6473 6060 0a20 2020 2020 2020  _cands``.       
+0000fa70: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+0000fa80: 6f6e 2028 6675 6e63 7469 6f6e 2c20 6f70  on (function, op
+0000fa90: 7469 6f6e 616c 293a 2054 6865 2073 7472  tional): The str
+0000faa0: 656e 6774 6820 6675 6e63 7469 6f6e 2074  ength function t
+0000fab0: 6f20 6265 2075 7365 6420 746f 2063 616c  o be used to cal
+0000fac0: 6375 6c61 7465 2074 6865 2073 7472 656e  culate the stren
+0000fad0: 6774 6820 6f66 2061 2070 6174 682e 2020  gth of a path.  
+0000fae0: 2054 6865 2064 6566 6175 6c74 2069 7320   The default is 
+0000faf0: 7468 6520 6d61 7267 696e 206d 6574 686f  the margin metho
+0000fb00: 6420 6f66 2060 6065 6461 7461 6060 2e20  d of ``edata``. 
+0000fb10: 2020 5468 6973 206f 6e6c 7920 6d61 7474    This only matt
+0000fb20: 6572 7320 7768 656e 2074 6865 2062 616c  ers when the bal
+0000fb30: 6c6f 7473 2061 7265 206e 6f74 206c 696e  lots are not lin
+0000fb40: 6561 7220 6f72 6465 7273 2e20 0a0a 2020  ear orders. ..  
+0000fb50: 2020 5265 7475 726e 733a 200a 2020 2020    Returns: .    
+0000fb60: 2020 2020 4120 736f 7274 6564 206c 6973      A sorted lis
+0000fb70: 7420 6f66 2063 616e 6469 6461 7465 732e  t of candidates.
+0000fb80: 200a 0a20 2020 2022 2222 0a20 2020 2063   ..    """.    c
+0000fb90: 7720 3d20 6564 6174 612e 636f 6e64 6f72  w = edata.condor
+0000fba0: 6365 745f 7769 6e6e 6572 2863 7572 725f  cet_winner(curr_
+0000fbb0: 6361 6e64 7320 3d20 6375 7272 5f63 616e  cands = curr_can
+0000fbc0: 6473 290a 2020 2020 6966 2063 7720 6973  ds).    if cw is
+0000fbd0: 206e 6f74 204e 6f6e 653a 200a 2020 2020   not None: .    
+0000fbe0: 2020 2020 7265 7475 726e 205b 6377 5d0a      return [cw].
+0000fbf0: 2020 2020 656c 7365 3a20 0a20 2020 2020      else: .     
+0000fc00: 2020 2063 7572 725f 6361 6e64 7320 3d20     curr_cands = 
+0000fc10: 6564 6174 612e 6361 6e64 6964 6174 6573  edata.candidates
+0000fc20: 2069 6620 6375 7272 5f63 616e 6473 2069   if curr_cands i
+0000fc30: 7320 4e6f 6e65 2065 6c73 6520 6375 7272  s None else curr
+0000fc40: 5f63 616e 6473 0a20 2020 2020 2020 2073  _cands.        s
+0000fc50: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+0000fc60: 203d 2065 6461 7461 2e6d 6172 6769 6e20   = edata.margin 
+0000fc70: 6966 2073 7472 656e 6774 685f 6675 6e63  if strength_func
+0000fc80: 7469 6f6e 2069 7320 4e6f 6e65 2065 6c73  tion is None els
+0000fc90: 6520 7374 7265 6e67 7468 5f66 756e 6374  e strength_funct
+0000fca0: 696f 6e20 200a 0a20 2020 2020 2020 206d  ion  ..        m
+0000fcb0: 6174 6368 6573 203d 205b 2861 2c20 622c  atches = [(a, b,
+0000fcc0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+0000fcd0: 6f6e 2861 2c20 6229 2920 666f 7220 6120  on(a, b)) for a 
+0000fce0: 696e 2063 7572 725f 6361 6e64 7320 666f  in curr_cands fo
+0000fcf0: 7220 6220 696e 2063 7572 725f 6361 6e64  r b in curr_cand
+0000fd00: 7320 6966 2061 2021 3d20 625d 0a20 2020  s if a != b].   
+0000fd10: 2020 2020 2073 6f72 7465 645f 6d61 7463       sorted_matc
+0000fd20: 6865 7320 3d20 736f 7274 6564 286d 6174  hes = sorted(mat
+0000fd30: 6368 6573 2c20 7265 7665 7273 653d 5472  ches, reverse=Tr
+0000fd40: 7565 2c20 6b65 793d 6c61 6d62 6461 206d  ue, key=lambda m
+0000fd50: 5f77 5f77 6569 6768 743a 206d 5f77 5f77  _w_weight: m_w_w
+0000fd60: 6569 6768 745b 325d 290a 0a20 2020 2020  eight[2])..     
+0000fd70: 2020 2072 6574 7572 6e20 736f 7274 6564     return sorted
+0000fd80: 285f 7374 6162 6c65 5f76 6f74 696e 6728  (_stable_voting(
+0000fd90: 6564 6174 612c 200a 2020 2020 2020 2020  edata, .        
+0000fda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fdb0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+0000fdc0: 5f63 616e 6473 203d 2063 7572 725f 6361  _cands = curr_ca
+0000fdd0: 6e64 732c 200a 2020 2020 2020 2020 2020  nds, .          
+0000fde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fdf0: 2020 2020 2020 2020 2020 7374 7265 6e67            streng
+0000fe00: 7468 5f66 756e 6374 696f 6e20 3d20 7374  th_function = st
+0000fe10: 7265 6e67 7468 5f66 756e 6374 696f 6e2c  rength_function,
+0000fe20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fe30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fe40: 2020 2020 2073 6f72 7465 645f 6d61 7463       sorted_matc
+0000fe50: 6865 7320 3d20 736f 7274 6564 5f6d 6174  hes = sorted_mat
+0000fe60: 6368 6573 2c0a 2020 2020 2020 2020 2020  ches,.          
+0000fe70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fe80: 2020 2020 2020 2020 2020 6d65 6d5f 7376            mem_sv
+0000fe90: 5f77 696e 6e65 7273 203d 207b 7d29 5b30  _winners = {})[0
+0000fea0: 5d29 0a0a 6465 6620 5f73 7461 626c 655f  ])..def _stable_
+0000feb0: 766f 7469 6e67 5f62 6173 6963 280a 2020  voting_basic(.  
+0000fec0: 2020 2020 2020 6564 6174 612c 200a 2020        edata, .  
+0000fed0: 2020 2020 2020 6375 7272 5f63 616e 6473        curr_cands
+0000fee0: 203d 204e 6f6e 652c 200a 2020 2020 2020   = None, .      
+0000fef0: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
+0000ff00: 696f 6e20 3d20 4e6f 6e65 293a 200a 2020  ion = None): .  
+0000ff10: 2020 2222 2249 6d70 6c65 6d65 6e74 6174    """Implementat
+0000ff20: 696f 6e20 6f66 2020 5374 6162 6c65 2056  ion of  Stable V
+0000ff30: 6f74 696e 6720 6672 6f6d 2068 7474 7073  oting from https
+0000ff40: 3a2f 2f61 7278 6976 2e6f 7267 2f61 6273  ://arxiv.org/abs
+0000ff50: 2f32 3130 382e 3030 3534 322e 200a 0a20  /2108.00542. .. 
+0000ff60: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+0000ff70: 2065 6461 7461 2028 5072 6f66 696c 652c   edata (Profile,
+0000ff80: 2050 726f 6669 6c65 5769 7468 5469 6573   ProfileWithTies
+0000ff90: 2c20 4d61 7267 696e 4772 6170 6829 3a20  , MarginGraph): 
+0000ffa0: 416e 7920 656c 6563 7469 6f6e 2064 6174  Any election dat
+0000ffb0: 6120 7468 6174 2068 6173 2061 2060 6d61  a that has a `ma
+0000ffc0: 7267 696e 6020 6d65 7468 6f64 2e20 0a20  rgin` method. . 
+0000ffd0: 2020 2020 2020 2063 7572 725f 6361 6e64         curr_cand
+0000ffe0: 7320 284c 6973 745b 696e 745d 2c20 6f70  s (List[int], op
+0000fff0: 7469 6f6e 616c 293a 2049 6620 7365 742c  tional): If set,
+00010000: 2074 6865 6e20 6669 6e64 2074 6865 2077   then find the w
+00010010: 696e 6e65 7273 2066 6f72 2074 6865 2070  inners for the p
+00010020: 726f 6669 6c65 2072 6573 7472 6963 7465  rofile restricte
+00010030: 6420 746f 2074 6865 2063 616e 6469 6461  d to the candida
+00010040: 7465 7320 696e 2060 6063 7572 725f 6361  tes in ``curr_ca
+00010050: 6e64 7360 600a 2020 2020 2020 2020 7374  nds``.        st
+00010060: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
+00010070: 2866 756e 6374 696f 6e2c 206f 7074 696f  (function, optio
+00010080: 6e61 6c29 3a20 5468 6520 7374 7265 6e67  nal): The streng
+00010090: 7468 2066 756e 6374 696f 6e20 746f 2062  th function to b
+000100a0: 6520 7573 6564 2074 6f20 6361 6c63 756c  e used to calcul
+000100b0: 6174 6520 7468 6520 7374 7265 6e67 7468  ate the strength
+000100c0: 206f 6620 6120 7061 7468 2e20 2020 5468   of a path.   Th
+000100d0: 6520 6465 6661 756c 7420 6973 2074 6865  e default is the
+000100e0: 206d 6172 6769 6e20 6d65 7468 6f64 206f   margin method o
+000100f0: 6620 6060 6564 6174 6160 602e 2020 2054  f ``edata``.   T
+00010100: 6869 7320 6f6e 6c79 206d 6174 7465 7273  his only matters
+00010110: 2077 6865 6e20 7468 6520 6261 6c6c 6f74   when the ballot
+00010120: 7320 6172 6520 6e6f 7420 6c69 6e65 6172  s are not linear
+00010130: 206f 7264 6572 732e 200a 0a20 2020 2052   orders. ..    R
+00010140: 6574 7572 6e73 3a20 0a20 2020 2020 2020  eturns: .       
+00010150: 2041 2073 6f72 7465 6420 6c69 7374 206f   A sorted list o
+00010160: 6620 6361 6e64 6964 6174 6573 2e20 0a0a  f candidates. ..
+00010170: 2020 2020 2222 220a 0a20 2020 2063 7572      """..    cur
+00010180: 725f 6361 6e64 7320 3d20 6564 6174 612e  r_cands = edata.
+00010190: 6361 6e64 6964 6174 6573 2069 6620 6375  candidates if cu
+000101a0: 7272 5f63 616e 6473 2069 7320 4e6f 6e65  rr_cands is None
+000101b0: 2065 6c73 6520 6375 7272 5f63 616e 6473   else curr_cands
+000101c0: 0a20 2020 2073 7472 656e 6774 685f 6675  .    strength_fu
+000101d0: 6e63 7469 6f6e 203d 2065 6461 7461 2e6d  nction = edata.m
+000101e0: 6172 6769 6e20 6966 2073 7472 656e 6774  argin if strengt
+000101f0: 685f 6675 6e63 7469 6f6e 2069 7320 4e6f  h_function is No
+00010200: 6e65 2065 6c73 6520 7374 7265 6e67 7468  ne else strength
+00010210: 5f66 756e 6374 696f 6e20 200a 0a20 2020  _function  ..   
+00010220: 206d 6174 6368 6573 203d 205b 2861 2c20   matches = [(a, 
+00010230: 622c 2073 7472 656e 6774 685f 6675 6e63  b, strength_func
+00010240: 7469 6f6e 2861 2c20 6229 2920 666f 7220  tion(a, b)) for 
+00010250: 6120 696e 2063 7572 725f 6361 6e64 7320  a in curr_cands 
+00010260: 666f 7220 6220 696e 2063 7572 725f 6361  for b in curr_ca
+00010270: 6e64 7320 6966 2061 2021 3d20 625d 0a20  nds if a != b]. 
+00010280: 2020 2073 6f72 7465 645f 6d61 7463 6865     sorted_matche
+00010290: 7320 3d20 736f 7274 6564 286d 6174 6368  s = sorted(match
+000102a0: 6573 2c20 7265 7665 7273 653d 5472 7565  es, reverse=True
+000102b0: 2c20 6b65 793d 6c61 6d62 6461 206d 5f77  , key=lambda m_w
+000102c0: 5f77 6569 6768 743a 206d 5f77 5f77 6569  _weight: m_w_wei
+000102d0: 6768 745b 325d 290a 0a20 2020 2072 6574  ght[2])..    ret
+000102e0: 7572 6e20 736f 7274 6564 285f 7374 6162  urn sorted(_stab
+000102f0: 6c65 5f76 6f74 696e 6728 6564 6174 612c  le_voting(edata,
+00010300: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+00010310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010320: 2020 2063 7572 725f 6361 6e64 7320 3d20     curr_cands = 
+00010330: 6375 7272 5f63 616e 6473 2c20 0a20 2020  curr_cands, .   
+00010340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010350: 2020 2020 2020 2020 2020 2020 2020 7374                st
+00010360: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
+00010370: 3d20 7374 7265 6e67 7468 5f66 756e 6374  = strength_funct
+00010380: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+00010390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103a0: 2020 2020 2020 736f 7274 6564 5f6d 6174        sorted_mat
+000103b0: 6368 6573 203d 2073 6f72 7465 645f 6d61  ches = sorted_ma
+000103c0: 7463 6865 732c 0a20 2020 2020 2020 2020  tches,.         
+000103d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103e0: 2020 2020 2020 2020 6d65 6d5f 7376 5f77          mem_sv_w
+000103f0: 696e 6e65 7273 203d 207b 7d29 5b30 5d29  inners = {})[0])
+00010400: 0a0a 7376 5f70 726f 7065 7274 6965 7320  ..sv_properties 
+00010410: 3d20 566f 7469 6e67 4d65 7468 6f64 5072  = VotingMethodPr
+00010420: 6f70 6572 7469 6573 280a 2020 2020 636f  operties(.    co
+00010430: 6e64 6f72 6365 745f 7769 6e6e 6572 3d54  ndorcet_winner=T
+00010440: 7275 652c 200a 2020 2020 636f 6e64 6f72  rue, .    condor
+00010450: 6365 745f 6c6f 7365 723d 5472 7565 2c0a  cet_loser=True,.
+00010460: 2020 2020 7061 7265 746f 5f64 6f6d 696e      pareto_domin
+00010470: 616e 6365 3d54 7275 652c 200a 2020 2020  ance=True, .    
+00010480: 290a 4076 6d28 6e61 6d65 203d 2022 5374  ).@vm(name = "St
+00010490: 6162 6c65 2056 6f74 696e 6722 2c0a 2020  able Voting",.  
+000104a0: 2020 7072 6f70 6572 7469 6573 203d 2073    properties = s
+000104b0: 765f 7072 6f70 6572 7469 6573 2c0a 2020  v_properties,.  
+000104c0: 2020 696e 7075 745f 7479 7065 7320 3d20    input_types = 
+000104d0: 5b45 6c65 6374 696f 6e54 7970 6573 2e50  [ElectionTypes.P
+000104e0: 524f 4649 4c45 2c20 456c 6563 7469 6f6e  ROFILE, Election
+000104f0: 5479 7065 732e 5052 4f46 494c 455f 5749  Types.PROFILE_WI
+00010500: 5448 5f54 4945 532c 2045 6c65 6374 696f  TH_TIES, Electio
+00010510: 6e54 7970 6573 2e4d 4152 4749 4e5f 4752  nTypes.MARGIN_GR
+00010520: 4150 485d 290a 6465 6620 7374 6162 6c65  APH]).def stable
+00010530: 5f76 6f74 696e 6728 0a20 2020 2065 6461  _voting(.    eda
+00010540: 7461 2c20 0a20 2020 2063 7572 725f 6361  ta, .    curr_ca
+00010550: 6e64 733d 4e6f 6e65 2c20 0a20 2020 2073  nds=None, .    s
+00010560: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+00010570: 3d4e 6f6e 652c 200a 2020 2020 616c 676f  =None, .    algo
+00010580: 7269 7468 6d3d 2762 6173 6963 2729 3a20  rithm='basic'): 
+00010590: 0a20 2020 2022 2222 496d 706c 656d 656e  .    """Implemen
+000105a0: 7461 7469 6f6e 206f 6620 2053 7461 626c  tation of  Stabl
+000105b0: 6520 566f 7469 6e67 2066 726f 6d20 6874  e Voting from ht
+000105c0: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
+000105d0: 6162 732f 3231 3038 2e30 3035 3432 2e20  abs/2108.00542. 
+000105e0: 0a0a 2020 2020 5374 6162 6c65 2056 6f74  ..    Stable Vot
+000105f0: 696e 6720 6973 2061 2072 6563 7572 7369  ing is a recursi
+00010600: 7665 2076 6f74 696e 6720 6d65 7468 6f64  ve voting method
+00010610: 2064 6566 696e 6564 2061 7320 666f 6c6c   defined as foll
+00010620: 6f77 733a 200a 0a20 2020 2031 2e20 2049  ows: ..    1.  I
+00010630: 6620 7468 6572 6520 6973 206f 6e6c 7920  f there is only 
+00010640: 6f6e 6520 6361 6e64 6964 6174 6520 696e  one candidate in
+00010650: 2074 6865 2070 726f 6669 6c65 2c20 7468   the profile, th
+00010660: 656e 2074 6861 7420 6361 6e64 6964 6174  en that candidat
+00010670: 6520 6973 2074 6865 2077 696e 6e65 722e  e is the winner.
+00010680: 200a 2020 2020 322e 204f 7264 6572 2074   .    2. Order t
+00010690: 6865 2070 6169 7273 203a 6d61 7468 3a60  he pairs :math:`
+000106a0: 2861 2c62 2960 206f 6620 6361 6e64 6964  (a,b)` of candid
+000106b0: 6174 6573 2066 726f 6d20 6c61 7267 6573  ates from larges
+000106c0: 7420 746f 2073 6d61 6c6c 6573 7420 7661  t to smallest va
+000106d0: 6c75 6520 6f66 2074 6865 206d 6172 6769  lue of the margi
+000106e0: 6e20 6f66 203a 6d61 7468 3a60 6160 206f  n of :math:`a` o
+000106f0: 7665 7220 3a6d 6174 683a 6062 6020 7375  ver :math:`b` su
+00010700: 6368 2074 6861 7420 3a6d 6174 683a 6061  ch that :math:`a
+00010710: 6020 6973 2075 6e64 6566 6561 7465 6420  ` is undefeated 
+00010720: 6163 636f 7264 696e 6720 746f 2053 706c  according to Spl
+00010730: 6974 2043 7963 6c65 2c20 616e 6420 6465  it Cycle, and de
+00010740: 636c 6172 6520 6173 2053 7461 626c 6520  clare as Stable 
+00010750: 566f 7469 6e67 2077 696e 6e65 7273 2074  Voting winners t
+00010760: 6865 2063 616e 6469 6461 7465 2873 2920  he candidate(s) 
+00010770: 3a6d 6174 683a 6061 6020 6672 6f6d 2074  :math:`a` from t
+00010780: 6865 2065 6172 6c69 6573 7420 7061 6972  he earliest pair
+00010790: 2873 2920 3a6d 6174 683a 6028 612c 6229  (s) :math:`(a,b)
+000107a0: 6020 7375 6368 2074 6861 7420 3a6d 6174  ` such that :mat
+000107b0: 683a 6061 6020 6973 2061 2053 696d 706c  h:`a` is a Simpl
+000107c0: 6520 5374 6162 6c65 2056 6f74 696e 6720  e Stable Voting 
+000107d0: 7769 6e6e 6572 2069 6e20 7468 6520 656c  winner in the el
+000107e0: 6563 7469 6f6e 2077 6974 686f 7574 203a  ection without :
+000107f0: 6d61 7468 3a60 6260 2e20 0a0a 2020 2020  math:`b`. ..    
+00010800: 4172 6773 3a0a 2020 2020 2020 2020 6564  Args:.        ed
+00010810: 6174 6120 2850 726f 6669 6c65 2c20 5072  ata (Profile, Pr
+00010820: 6f66 696c 6557 6974 6854 6965 732c 204d  ofileWithTies, M
+00010830: 6172 6769 6e47 7261 7068 293a 2041 6e79  arginGraph): Any
+00010840: 2065 6c65 6374 696f 6e20 6461 7461 2074   election data t
+00010850: 6861 7420 6861 7320 6120 606d 6172 6769  hat has a `margi
+00010860: 6e60 206d 6574 686f 642e 200a 2020 2020  n` method. .    
+00010870: 2020 2020 6375 7272 5f63 616e 6473 2028      curr_cands (
+00010880: 4c69 7374 5b69 6e74 5d2c 206f 7074 696f  List[int], optio
+00010890: 6e61 6c29 3a20 4966 2073 6574 2c20 7468  nal): If set, th
+000108a0: 656e 2066 696e 6420 7468 6520 7769 6e6e  en find the winn
+000108b0: 6572 7320 666f 7220 7468 6520 7072 6f66  ers for the prof
+000108c0: 696c 6520 7265 7374 7269 6374 6564 2074  ile restricted t
+000108d0: 6f20 7468 6520 6361 6e64 6964 6174 6573  o the candidates
+000108e0: 2069 6e20 6060 6375 7272 5f63 616e 6473   in ``curr_cands
+000108f0: 6060 0a20 2020 2020 2020 2073 7472 656e  ``.        stren
+00010900: 6774 685f 6675 6e63 7469 6f6e 2028 6675  gth_function (fu
+00010910: 6e63 7469 6f6e 2c20 6f70 7469 6f6e 616c  nction, optional
+00010920: 293a 2054 6865 2073 7472 656e 6774 6820  ): The strength 
+00010930: 6675 6e63 7469 6f6e 2074 6f20 6265 2075  function to be u
+00010940: 7365 6420 746f 2063 616c 6375 6c61 7465  sed to calculate
+00010950: 2074 6865 2073 7472 656e 6774 6820 6f66   the strength of
+00010960: 2061 2070 6174 682e 2020 2054 6865 2064   a path.   The d
+00010970: 6566 6175 6c74 2069 7320 7468 6520 6d61  efault is the ma
+00010980: 7267 696e 206d 6574 686f 6420 6f66 2060  rgin method of `
+00010990: 6065 6461 7461 6060 2e20 2020 5468 6973  `edata``.   This
+000109a0: 206f 6e6c 7920 6d61 7474 6572 7320 7768   only matters wh
+000109b0: 656e 2074 6865 2062 616c 6c6f 7473 2061  en the ballots a
+000109c0: 7265 206e 6f74 206c 696e 6561 7220 6f72  re not linear or
+000109d0: 6465 7273 2e20 0a0a 2020 2020 5265 7475  ders. ..    Retu
+000109e0: 726e 733a 200a 2020 2020 2020 2020 4120  rns: .        A 
+000109f0: 736f 7274 6564 206c 6973 7420 6f66 2063  sorted list of c
+00010a00: 616e 6469 6461 7465 732e 200a 0a20 2020  andidates. ..   
+00010a10: 202e 2e20 7365 6561 6c73 6f3a 3a0a 0a20   .. seealso::.. 
+00010a20: 2020 2020 2020 203a 6d65 7468 3a60 7072         :meth:`pr
+00010a30: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
+00010a40: 5f62 6173 6564 5f6d 6574 686f 6473 2e73  _based_methods.s
+00010a50: 696d 706c 655f 7374 6162 6c65 5f76 6f74  imple_stable_vot
+00010a60: 696e 6760 0a0a 0a20 2020 203a 4578 616d  ing`...    :Exam
+00010a70: 706c 653a 200a 0a20 2020 202e 2e20 6578  ple: ..    .. ex
+00010a80: 6563 5f63 6f64 653a 3a0a 0a20 2020 2020  ec_code::..     
+00010a90: 2020 2066 726f 6d20 7072 6566 5f76 6f74     from pref_vot
+00010aa0: 696e 672e 7765 6967 6874 6564 5f6d 616a  ing.weighted_maj
+00010ab0: 6f72 6974 795f 6772 6170 6873 2069 6d70  ority_graphs imp
+00010ac0: 6f72 7420 4d61 7267 696e 4772 6170 680a  ort MarginGraph.
+00010ad0: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
+00010ae0: 665f 766f 7469 6e67 2e6d 6172 6769 6e5f  f_voting.margin_
+00010af0: 6261 7365 645f 6d65 7468 6f64 7320 696d  based_methods im
+00010b00: 706f 7274 2073 7461 626c 655f 766f 7469  port stable_voti
+00010b10: 6e67 0a0a 2020 2020 2020 2020 6d67 203d  ng..        mg =
+00010b20: 204d 6172 6769 6e47 7261 7068 285b 302c   MarginGraph([0,
+00010b30: 2031 2c20 322c 2033 5d2c 205b 2830 2c20   1, 2, 3], [(0, 
+00010b40: 332c 2038 292c 2028 312c 2030 2c20 3130  3, 8), (1, 0, 10
+00010b50: 292c 2028 322c 2030 2c20 3429 2c20 2832  ), (2, 0, 4), (2
+00010b60: 2c20 312c 2038 292c 2028 332c 2031 2c20  , 1, 8), (3, 1, 
+00010b70: 3829 5d29 0a0a 2020 2020 2020 2020 7374  8)])..        st
+00010b80: 6162 6c65 5f76 6f74 696e 672e 6469 7370  able_voting.disp
+00010b90: 6c61 7928 6d67 290a 2020 2020 2020 2020  lay(mg).        
+00010ba0: 7374 6162 6c65 5f76 6f74 696e 672e 6469  stable_voting.di
+00010bb0: 7370 6c61 7928 6d67 2c20 616c 676f 7269  splay(mg, algori
+00010bc0: 7468 6d3d 2762 6173 6963 2729 0a20 2020  thm='basic').   
+00010bd0: 2020 2020 2073 7461 626c 655f 766f 7469       stable_voti
+00010be0: 6e67 2e64 6973 706c 6179 286d 672c 2061  ng.display(mg, a
+00010bf0: 6c67 6f72 6974 686d 3d27 7769 7468 5f63  lgorithm='with_c
+00010c00: 6f6e 646f 7263 6574 5f63 6865 636b 2729  ondorcet_check')
+00010c10: 0a0a 2020 2020 2222 220a 0a20 2020 2069  ..    """..    i
+00010c20: 6620 616c 676f 7269 7468 6d20 3d3d 2027  f algorithm == '
+00010c30: 6261 7369 6327 3a20 0a20 2020 2020 2020  basic': .       
+00010c40: 2072 6574 7572 6e20 5f73 7461 626c 655f   return _stable_
+00010c50: 766f 7469 6e67 5f62 6173 6963 2865 6461  voting_basic(eda
+00010c60: 7461 2c20 6375 7272 5f63 616e 6473 203d  ta, curr_cands =
+00010c70: 2063 7572 725f 6361 6e64 732c 2073 7472   curr_cands, str
+00010c80: 656e 6774 685f 6675 6e63 7469 6f6e 203d  ength_function =
+00010c90: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+00010ca0: 6f6e 290a 2020 2020 656c 6966 2061 6c67  on).    elif alg
+00010cb0: 6f72 6974 686d 203d 3d20 2777 6974 685f  orithm == 'with_
+00010cc0: 636f 6e64 6f72 6365 745f 6368 6563 6b27  condorcet_check'
+00010cd0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00010ce0: 205f 7374 6162 6c65 5f76 6f74 696e 675f   _stable_voting_
+00010cf0: 7769 7468 5f63 6f6e 646f 7263 6574 5f63  with_condorcet_c
+00010d00: 6865 636b 2865 6461 7461 2c20 6375 7272  heck(edata, curr
+00010d10: 5f63 616e 6473 203d 2063 7572 725f 6361  _cands = curr_ca
+00010d20: 6e64 732c 2073 7472 656e 6774 685f 6675  nds, strength_fu
+00010d30: 6e63 7469 6f6e 203d 2073 7472 656e 6774  nction = strengt
+00010d40: 685f 6675 6e63 7469 6f6e 290a 2020 2020  h_function).    
+00010d50: 656c 7365 3a0a 2020 2020 2020 2020 7261  else:.        ra
+00010d60: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
+00010d70: 496e 7661 6c69 6420 616c 676f 7269 7468  Invalid algorith
+00010d80: 6d20 7370 6563 6966 6965 642e 2229 0a20  m specified."). 
+00010d90: 2020 200a 0a65 7373 656e 7469 616c 5f73     ..essential_s
+00010da0: 6574 5f70 726f 7065 7274 6965 7320 3d20  et_properties = 
+00010db0: 566f 7469 6e67 4d65 7468 6f64 5072 6f70  VotingMethodProp
+00010dc0: 6572 7469 6573 280a 2020 2020 636f 6e64  erties(.    cond
+00010dd0: 6f72 6365 745f 7769 6e6e 6572 3d54 7275  orcet_winner=Tru
+00010de0: 652c 200a 2020 2020 636f 6e64 6f72 6365  e, .    condorce
+00010df0: 745f 6c6f 7365 723d 5472 7565 2c0a 2020  t_loser=True,.  
+00010e00: 2020 7061 7265 746f 5f64 6f6d 696e 616e    pareto_dominan
+00010e10: 6365 3d54 7275 652c 200a 2020 2020 290a  ce=True, .    ).
+00010e20: 4076 6d28 6e61 6d65 3d22 4573 7365 6e74  @vm(name="Essent
+00010e30: 6961 6c20 5365 7422 2c0a 2020 2020 7072  ial Set",.    pr
+00010e40: 6f70 6572 7469 6573 3d65 7373 656e 7469  operties=essenti
+00010e50: 616c 5f73 6574 5f70 726f 7065 7274 6965  al_set_propertie
+00010e60: 732c 0a20 2020 2069 6e70 7574 5f74 7970  s,.    input_typ
+00010e70: 6573 3d5b 456c 6563 7469 6f6e 5479 7065  es=[ElectionType
+00010e80: 732e 5052 4f46 494c 452c 2045 6c65 6374  s.PROFILE, Elect
+00010e90: 696f 6e54 7970 6573 2e50 524f 4649 4c45  ionTypes.PROFILE
+00010ea0: 5f57 4954 485f 5449 4553 2c20 456c 6563  _WITH_TIES, Elec
+00010eb0: 7469 6f6e 5479 7065 732e 4d41 5247 494e  tionTypes.MARGIN
+00010ec0: 5f47 5241 5048 5d29 0a64 6566 2065 7373  _GRAPH]).def ess
+00010ed0: 656e 7469 616c 2865 6461 7461 2c20 6375  ential(edata, cu
+00010ee0: 7272 5f63 616e 6473 203d 204e 6f6e 652c  rr_cands = None,
+00010ef0: 2074 6872 6573 686f 6c64 203d 2030 2e30   threshold = 0.0
+00010f00: 3030 3030 3031 293a 200a 2020 2020 2222  000001): .    ""
+00010f10: 2254 6865 2045 7373 656e 7469 616c 2053  "The Essential S
+00010f20: 6574 2069 7320 7468 6520 7375 7070 6f72  et is the suppor
+00010f30: 7420 6f66 2074 6865 2028 6368 6f73 656e  t of the (chosen
+00010f40: 2920 4332 206d 6178 696d 616c 206c 6f74  ) C2 maximal lot
+00010f50: 7465 7279 2e0a 0a20 2020 2041 7267 733a  tery...    Args:
+00010f60: 0a20 2020 2020 2020 2065 6461 7461 2028  .        edata (
+00010f70: 5072 6f66 696c 652c 2050 726f 6669 6c65  Profile, Profile
+00010f80: 5769 7468 5469 6573 2c20 4d61 7267 696e  WithTies, Margin
+00010f90: 4772 6170 6829 3a20 416e 7920 656c 6563  Graph): Any elec
+00010fa0: 7469 6f6e 2064 6174 6120 7468 6174 2068  tion data that h
+00010fb0: 6173 2061 2060 6d61 7267 696e 5f6d 6174  as a `margin_mat
+00010fc0: 7269 7860 2061 7474 7269 6275 7465 2e0a  rix` attribute..
+00010fd0: 2020 2020 2020 2020 6375 7272 5f63 616e          curr_can
+00010fe0: 6473 2028 4c69 7374 5b69 6e74 5d2c 206f  ds (List[int], o
+00010ff0: 7074 696f 6e61 6c29 3a20 4966 2073 6574  ptional): If set
+00011000: 2c20 7468 656e 2066 696e 6420 7468 6520  , then find the 
+00011010: 7769 6e6e 6572 7320 666f 7220 7468 6520  winners for the 
+00011020: 7072 6f66 696c 6520 7265 7374 7269 6374  profile restrict
+00011030: 6564 2074 6f20 7468 6520 6361 6e64 6964  ed to the candid
+00011040: 6174 6573 2069 6e20 6060 6375 7272 5f63  ates in ``curr_c
+00011050: 616e 6473 6060 0a0a 2020 2020 5265 7475  ands``..    Retu
+00011060: 726e 733a 0a20 2020 2020 2020 2041 2073  rns:.        A s
+00011070: 6f72 7465 6420 6c69 7374 206f 6620 6361  orted list of ca
+00011080: 6e64 6964 6174 6573 2e0a 0a20 2020 2022  ndidates...    "
+00011090: 2222 0a20 2020 206d 6c20 3d20 6d61 7869  "".    ml = maxi
+000110a0: 6d61 6c5f 6c6f 7474 6572 7928 6564 6174  mal_lottery(edat
+000110b0: 612c 2063 7572 725f 6361 6e64 733d 6375  a, curr_cands=cu
+000110c0: 7272 5f63 616e 6473 290a 0a20 2020 2072  rr_cands)..    r
+000110d0: 6574 7572 6e20 736f 7274 6564 285b 6320  eturn sorted([c 
+000110e0: 666f 7220 6320 696e 206d 6c2e 6b65 7973  for c in ml.keys
+000110f0: 2829 2069 6620 6d6c 5b63 5d20 3e20 7468  () if ml[c] > th
+00011100: 7265 7368 6f6c 645d 290a 0a77 6569 6768  reshold])..weigh
+00011110: 7465 645f 636f 7665 7269 6e67 5f70 726f  ted_covering_pro
+00011120: 7065 7274 6965 7320 3d20 566f 7469 6e67  perties = Voting
+00011130: 4d65 7468 6f64 5072 6f70 6572 7469 6573  MethodProperties
+00011140: 280a 2020 2020 636f 6e64 6f72 6365 745f  (.    condorcet_
+00011150: 7769 6e6e 6572 3d54 7275 652c 200a 2020  winner=True, .  
+00011160: 2020 636f 6e64 6f72 6365 745f 6c6f 7365    condorcet_lose
+00011170: 723d 5472 7565 2c0a 2020 2020 7061 7265  r=True,.    pare
+00011180: 746f 5f64 6f6d 696e 616e 6365 3d54 7275  to_dominance=Tru
+00011190: 652c 200a 2020 2020 290a 4076 6d28 6e61  e, .    ).@vm(na
+000111a0: 6d65 3d22 5765 6967 6874 6564 2043 6f76  me="Weighted Cov
+000111b0: 6572 696e 6722 2c0a 2020 2020 7072 6f70  ering",.    prop
+000111c0: 6572 7469 6573 3d77 6569 6768 7465 645f  erties=weighted_
+000111d0: 636f 7665 7269 6e67 5f70 726f 7065 7274  covering_propert
+000111e0: 6965 732c 0a20 2020 2069 6e70 7574 5f74  ies,.    input_t
+000111f0: 7970 6573 3d5b 456c 6563 7469 6f6e 5479  ypes=[ElectionTy
+00011200: 7065 732e 5052 4f46 494c 452c 2045 6c65  pes.PROFILE, Ele
+00011210: 6374 696f 6e54 7970 6573 2e50 524f 4649  ctionTypes.PROFI
+00011220: 4c45 5f57 4954 485f 5449 4553 2c20 456c  LE_WITH_TIES, El
+00011230: 6563 7469 6f6e 5479 7065 732e 4d41 5247  ectionTypes.MARG
+00011240: 494e 5f47 5241 5048 5d29 0a64 6566 2077  IN_GRAPH]).def w
+00011250: 6569 6768 7465 645f 636f 7665 7269 6e67  eighted_covering
+00011260: 2865 6461 7461 2c20 6375 7272 5f63 616e  (edata, curr_can
+00011270: 6473 3d4e 6f6e 6529 3a20 0a20 2020 2022  ds=None): .    "
+00011280: 2222 4163 636f 7264 696e 6720 746f 2057  ""According to W
+00011290: 6569 6768 7465 6420 436f 7665 7269 6e67  eighted Covering
+000112a0: 2c20 7820 6465 6665 6174 7320 7920 6966  , x defeats y if
+000112b0: 2074 6865 206d 6172 6769 6e20 6f66 2078   the margin of x
+000112c0: 206f 7665 7220 7920 6973 2070 6f73 6974   over y is posit
+000112d0: 6976 6520 616e 6420 666f 7220 6576 6572  ive and for ever
+000112e0: 7920 6f74 6865 7220 7a2c 2074 6865 206d  y other z, the m
+000112f0: 6172 6769 6e20 6f66 2078 206f 7665 7220  argin of x over 
+00011300: 7a20 6973 2067 7265 6174 6572 2074 6861  z is greater tha
+00011310: 6e20 6f72 2065 7175 616c 2074 6f20 7468  n or equal to th
+00011320: 6520 6d61 7267 696e 206f 6620 7920 6f76  e margin of y ov
+00011330: 6572 207a 2e20 0a0a 2020 2020 4172 6773  er z. ..    Args
+00011340: 3a0a 2020 2020 2020 2020 6564 6174 6120  :.        edata 
+00011350: 2850 726f 6669 6c65 2c20 5072 6f66 696c  (Profile, Profil
+00011360: 6557 6974 6854 6965 732c 204d 6172 6769  eWithTies, Margi
+00011370: 6e47 7261 7068 293a 2041 6e79 2065 6c65  nGraph): Any ele
+00011380: 6374 696f 6e20 6461 7461 2074 6861 7420  ction data that 
+00011390: 6861 7320 6120 606d 6172 6769 6e60 206d  has a `margin` m
+000113a0: 6574 686f 642e 0a20 2020 2020 2020 2063  ethod..        c
+000113b0: 7572 725f 6361 6e64 7320 284c 6973 745b  urr_cands (List[
+000113c0: 696e 745d 2c20 6f70 7469 6f6e 616c 293a  int], optional):
+000113d0: 2049 6620 7365 742c 2074 6865 6e20 6669   If set, then fi
+000113e0: 6e64 2074 6865 2077 696e 6e65 7273 2066  nd the winners f
+000113f0: 6f72 2074 6865 2070 726f 6669 6c65 2072  or the profile r
+00011400: 6573 7472 6963 7465 6420 746f 2074 6865  estricted to the
+00011410: 2063 616e 6469 6461 7465 7320 696e 2060   candidates in `
+00011420: 6063 7572 725f 6361 6e64 7360 600a 0a20  `curr_cands``.. 
+00011430: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00011440: 2020 2020 4120 736f 7274 6564 206c 6973      A sorted lis
+00011450: 7420 6f66 2063 616e 6469 6461 7465 732e  t of candidates.
+00011460: 0a0a 2020 2020 2e2e 206e 6f74 653a 3a0a  ..    .. note::.
+00011470: 2020 2020 2020 2020 5365 652c 2065 2e67          See, e.g
+00011480: 2e2c 2042 6861 736b 6172 2044 7574 7461  ., Bhaskar Dutta
+00011490: 2061 6e64 204a 6561 6e2d 4672 616e 636f   and Jean-Franco
+000114a0: 6973 204c 6173 6c69 6572 2c20 2243 6f6d  is Laslier, "Com
+000114b0: 7061 7269 736f 6e20 6675 6e63 7469 6f6e  parison function
+000114c0: 7320 616e 6420 6368 6f69 6365 2063 6f72  s and choice cor
+000114d0: 7265 7370 6f6e 6465 6e63 6573 2c22 2053  respondences," S
+000114e0: 6f63 6961 6c20 4368 6f69 6365 2061 6e64  ocial Choice and
+000114f0: 2057 656c 6661 7265 2c20 3136 3a35 3133   Welfare, 16:513
+00011500: e280 9335 3332 2c20 3139 3939 2c20 646f  ...532, 1999, do
+00011510: 693a 3130 2e31 3030 372f 7330 3033 3535  i:10.1007/s00355
+00011520: 3030 3530 3135 382c 2061 6e64 2052 6175  0050158, and Rau
+00011530: cc81 6c20 5065 cc81 7265 7a2d 4665 726e  ..l Pe..rez-Fern
+00011540: 61cc 816e 6465 7a20 616e 6420 4265 726e  a..ndez and Bern
+00011550: 6172 6420 4465 2042 6165 7473 2c20 2254  ard De Baets, "T
+00011560: 6865 2073 7570 6572 636f 7665 7269 6e67  he supercovering
+00011570: 2072 656c 6174 696f 6e2c 2074 6865 2070   relation, the p
+00011580: 6169 7277 6973 6520 7769 6e6e 6572 2c20  airwise winner, 
+00011590: 616e 6420 6d6f 7265 206d 6973 7369 6e67  and more missing
+000115a0: 206c 696e 6b73 2062 6574 7765 656e 2042   links between B
+000115b0: 6f72 6461 2061 6e64 2043 6f6e 646f 7263  orda and Condorc
+000115c0: 6574 2c22 2053 6f63 6961 6c20 4368 6f69  et," Social Choi
+000115d0: 6365 2061 6e64 2057 656c 6661 7265 2c20  ce and Welfare, 
+000115e0: 3530 3a33 3239 e280 9333 3532 2c20 3230  50:329...352, 20
+000115f0: 3138 2c20 646f 693a 3130 2e31 3030 372f  18, doi:10.1007/
+00011600: 7330 3033 3535 2d30 3137 2d31 3038 362d  s00355-017-1086-
+00011610: 302e 0a20 2020 2022 2222 0a0a 2020 2020  0..    """..    
+00011620: 6361 6e64 6964 6174 6573 203d 2065 6461  candidates = eda
+00011630: 7461 2e63 616e 6469 6461 7465 7320 6966  ta.candidates if
+00011640: 2063 7572 725f 6361 6e64 7320 6973 204e   curr_cands is N
+00011650: 6f6e 6520 656c 7365 2063 7572 725f 6361  one else curr_ca
+00011660: 6e64 730a 0a20 2020 2075 635f 7365 7420  nds..    uc_set 
+00011670: 3d20 6c69 7374 2829 0a0a 2020 2020 666f  = list()..    fo
+00011680: 7220 7920 696e 2063 616e 6469 6461 7465  r y in candidate
+00011690: 733a 0a20 2020 2020 2020 2069 735f 696e  s:.        is_in
+000116a0: 5f75 6373 203d 2054 7275 650a 2020 2020  _ucs = True.    
+000116b0: 2020 2020 666f 7220 7820 696e 2065 6461      for x in eda
+000116c0: 7461 2e64 6f6d 696e 6174 6f72 7328 792c  ta.dominators(y,
+000116d0: 2063 7572 725f 6361 6e64 7320 3d20 6375   curr_cands = cu
+000116e0: 7272 5f63 616e 6473 293a 0a20 2020 2020  rr_cands):.     
+000116f0: 2020 2020 2020 2023 2063 6865 636b 2069         # check i
+00011700: 6620 7920 636f 7665 7273 2078 2c20 692e  f y covers x, i.
+00011710: 652e 2c20 666f 7220 6576 6572 7920 7a2c  e., for every z,
+00011720: 206d 6172 6769 6e28 782c 207a 2920 3e3d   margin(x, z) >=
+00011730: 206d 6172 6769 6e28 792c 207a 290a 2020   margin(y, z).  
+00011740: 2020 2020 2020 2020 2020 636f 7665 7273            covers
+00011750: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
+00011760: 2020 2020 666f 7220 7a20 696e 2063 616e      for z in can
+00011770: 6469 6461 7465 733a 0a20 2020 2020 2020  didates:.       
+00011780: 2020 2020 2020 2020 2069 6620 6564 6174           if edat
+00011790: 612e 6d61 7267 696e 2878 2c20 7a29 203c  a.margin(x, z) <
+000117a0: 2065 6461 7461 2e6d 6172 6769 6e28 792c   edata.margin(y,
+000117b0: 207a 293a 0a20 2020 2020 2020 2020 2020   z):.           
+000117c0: 2020 2020 2020 2020 2063 6f76 6572 7320           covers 
+000117d0: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
+000117e0: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+000117f0: 6b0a 2020 2020 2020 2020 2020 0a20 2020  k.          .   
+00011800: 2020 2020 2020 2020 2069 6620 636f 7665           if cove
+00011810: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
+00011820: 2020 2020 6973 5f69 6e5f 7563 7320 3d20      is_in_ucs = 
+00011830: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
+00011840: 2020 2020 2020 6272 6561 6b0a 2020 2020        break.    
+00011850: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+00011860: 2020 2020 2069 6620 6973 5f69 6e5f 7563       if is_in_uc
+00011870: 733a 0a20 2020 2020 2020 2020 2020 2075  s:.            u
+00011880: 635f 7365 742e 6170 7065 6e64 2879 290a  c_set.append(y).
+00011890: 0a20 2020 2072 6574 7572 6e20 736f 7274  .    return sort
+000118a0: 6564 2875 635f 7365 7429 0a0a 6c6f 7373  ed(uc_set)..loss
+000118b0: 5f74 7269 6d6d 6572 5f70 726f 7065 7274  _trimmer_propert
+000118c0: 6965 7320 3d20 566f 7469 6e67 4d65 7468  ies = VotingMeth
+000118d0: 6f64 5072 6f70 6572 7469 6573 280a 2020  odProperties(.  
+000118e0: 2020 636f 6e64 6f72 6365 745f 7769 6e6e    condorcet_winn
+000118f0: 6572 3d54 7275 652c 200a 2020 2020 636f  er=True, .    co
+00011900: 6e64 6f72 6365 745f 6c6f 7365 723d 5472  ndorcet_loser=Tr
+00011910: 7565 2c0a 2020 2020 7061 7265 746f 5f64  ue,.    pareto_d
+00011920: 6f6d 696e 616e 6365 3d54 7275 652c 200a  ominance=True, .
+00011930: 2020 2020 290a 4076 6d28 6e61 6d65 203d      ).@vm(name =
+00011940: 2022 4c6f 7373 2d54 7269 6d6d 6572 2056   "Loss-Trimmer V
+00011950: 6f74 696e 6722 2c0a 2020 2020 7072 6f70  oting",.    prop
+00011960: 6572 7469 6573 203d 206c 6f73 735f 7472  erties = loss_tr
+00011970: 696d 6d65 725f 7072 6f70 6572 7469 6573  immer_properties
+00011980: 2c0a 2020 2020 696e 7075 745f 7479 7065  ,.    input_type
+00011990: 7320 3d20 5b45 6c65 6374 696f 6e54 7970  s = [ElectionTyp
+000119a0: 6573 2e50 524f 4649 4c45 2c20 456c 6563  es.PROFILE, Elec
+000119b0: 7469 6f6e 5479 7065 732e 5052 4f46 494c  tionTypes.PROFIL
+000119c0: 455f 5749 5448 5f54 4945 532c 2045 6c65  E_WITH_TIES, Ele
+000119d0: 6374 696f 6e54 7970 6573 2e4d 4152 4749  ctionTypes.MARGI
+000119e0: 4e5f 4752 4150 485d 290a 6465 6620 6c6f  N_GRAPH]).def lo
+000119f0: 7373 5f74 7269 6d6d 6572 2865 6461 7461  ss_trimmer(edata
+00011a00: 2c20 6375 7272 5f63 616e 6473 203d 204e  , curr_cands = N
+00011a10: 6f6e 6529 3a0a 2020 2020 2222 2249 7465  one):.    """Ite
+00011a20: 7261 7469 7665 6c79 2065 6c69 6d69 6e61  ratively elimina
+00011a30: 7465 2074 6865 2063 616e 6469 6461 7465  te the candidate
+00011a40: 2077 6974 6820 7468 6520 6c61 7267 6573   with the larges
+00011a50: 7420 7375 6d20 6f66 206d 6172 6769 6e73  t sum of margins
+00011a60: 206f 6620 6c6f 7373 2075 6e74 696c 2061   of loss until a
+00011a70: 2043 6f6e 646f 7263 6574 2077 696e 6e65   Condorcet winne
+00011a80: 7220 6973 2066 6f75 6e64 2e20 496e 2074  r is found. In t
+00011a90: 6869 7320 7665 7273 696f 6e20 6f66 2074  his version of t
+00011aa0: 6865 206d 6574 686f 642c 2070 6172 616c  he method, paral
+00011ab0: 6c65 6c2d 756e 6976 6572 7365 2074 6965  lel-universe tie
+00011ac0: 6272 6561 6b69 6e67 2069 7320 7573 6564  breaking is used
+00011ad0: 2069 6620 7468 6572 6520 6172 6520 6d75   if there are mu
+00011ae0: 6c74 6970 6c65 2063 616e 6469 6461 7465  ltiple candidate
+00011af0: 7320 7769 7468 2074 6865 206c 6172 6765  s with the large
+00011b00: 7374 2073 756d 206f 6620 6d61 7267 696e  st sum of margin
+00011b10: 7320 6f66 206c 6f73 732e 0a0a 2020 2020  s of loss...    
+00011b20: 4172 6773 3a0a 2020 2020 2020 2020 6564  Args:.        ed
+00011b30: 6174 6120 2850 726f 6669 6c65 2c20 5072  ata (Profile, Pr
+00011b40: 6f66 696c 6557 6974 6854 6965 732c 204d  ofileWithTies, M
+00011b50: 6172 6769 6e47 7261 7068 293a 2041 6e79  arginGraph): Any
+00011b60: 2065 6c65 6374 696f 6e20 6461 7461 2074   election data t
+00011b70: 6861 7420 6861 7320 6120 6d61 7267 696e  hat has a margin
+00011b80: 206d 6574 686f 642e 0a20 2020 2020 2020   method..       
+00011b90: 2063 7572 725f 6361 6e64 7320 284c 6973   curr_cands (Lis
+00011ba0: 745b 696e 745d 2c20 6f70 7469 6f6e 616c  t[int], optional
+00011bb0: 293a 2049 6620 7365 742c 2074 6865 6e20  ): If set, then 
+00011bc0: 6669 6e64 2074 6865 2077 696e 6e65 7273  find the winners
+00011bd0: 2066 6f72 2074 6865 2070 726f 6669 6c65   for the profile
+00011be0: 2072 6573 7472 6963 7465 6420 746f 2074   restricted to t
+00011bf0: 6865 2063 616e 6469 6461 7465 7320 696e  he candidates in
+00011c00: 2060 6063 7572 725f 6361 6e64 7360 600a   ``curr_cands``.
+00011c10: 0a20 2020 2052 6574 7572 6e73 3a20 0a20  .    Returns: . 
+00011c20: 2020 2020 2020 2041 2073 6f72 7465 6420         A sorted 
+00011c30: 6c69 7374 206f 6620 6361 6e64 6964 6174  list of candidat
+00011c40: 6573 0a0a 2020 2020 2e2e 206e 6f74 653a  es..    .. note:
+00011c50: 3a0a 2020 2020 2020 2020 4d65 7468 6f64  :.        Method
+00011c60: 2070 726f 706f 7365 6420 6279 2052 6963   proposed by Ric
+00011c70: 6861 7264 2042 2e20 4461 726c 696e 6774  hard B. Darlingt
+00011c80: 6f6e 2069 6e20 2254 6865 2043 6173 6520  on in "The Case 
+00011c90: 666f 7220 7468 6520 4c6f 7373 2d54 7269  for the Loss-Tri
+00011ca0: 6d6d 6572 2056 6f74 696e 6720 5379 7374  mmer Voting Syst
+00011cb0: 656d 2e22 0a0a 2020 2020 2222 220a 0a20  em."..    """.. 
+00011cc0: 2020 2063 7572 725f 6361 6e64 7320 3d20     curr_cands = 
+00011cd0: 6564 6174 612e 6361 6e64 6964 6174 6573  edata.candidates
+00011ce0: 2069 6620 6375 7272 5f63 616e 6473 2069   if curr_cands i
+00011cf0: 7320 4e6f 6e65 2065 6c73 6520 6375 7272  s None else curr
+00011d00: 5f63 616e 6473 0a0a 2020 2020 7765 616b  _cands..    weak
+00011d10: 5f63 7720 3d20 6564 6174 612e 7765 616b  _cw = edata.weak
+00011d20: 5f63 6f6e 646f 7263 6574 5f77 696e 6e65  _condorcet_winne
+00011d30: 7228 6375 7272 5f63 616e 6473 203d 2063  r(curr_cands = c
+00011d40: 7572 725f 6361 6e64 7329 0a20 2020 2023  urr_cands).    #
+00011d50: 2049 6620 7468 6572 6520 6172 6520 7765   If there are we
+00011d60: 616b 2043 6f6e 646f 7263 6574 2077 696e  ak Condorcet win
+00011d70: 6e65 7273 2c20 7265 7475 726e 2074 686f  ners, return tho
+00011d80: 7365 2063 616e 6469 6461 7465 730a 2020  se candidates.  
+00011d90: 2020 6966 2065 6461 7461 2e77 6561 6b5f    if edata.weak_
+00011da0: 636f 6e64 6f72 6365 745f 7769 6e6e 6572  condorcet_winner
+00011db0: 2863 7572 725f 6361 6e64 7320 3d20 6375  (curr_cands = cu
+00011dc0: 7272 5f63 616e 6473 2920 6973 206e 6f74  rr_cands) is not
+00011dd0: 204e 6f6e 653a 0a20 2020 2020 2020 2072   None:.        r
+00011de0: 6574 7572 6e20 736f 7274 6564 2877 6561  eturn sorted(wea
+00011df0: 6b5f 6377 290a 2020 2020 0a20 2020 2023  k_cw).    .    #
+00011e00: 204f 7468 6572 7769 7365 2c20 6361 6c63   Otherwise, calc
+00011e10: 756c 6174 6520 7468 6520 7375 6d20 6f66  ulate the sum of
+00011e20: 206d 6172 6769 6e73 206f 6620 6c6f 7373   margins of loss
+00011e30: 2066 6f72 2065 6163 6820 6361 6e64 6964   for each candid
+00011e40: 6174 650a 2020 2020 7375 6d5f 6f66 5f6d  ate.    sum_of_m
+00011e50: 6172 6769 6e73 5f6f 665f 6c6f 7373 203d  argins_of_loss =
+00011e60: 207b 6361 6e64 3a20 7375 6d28 5b65 6461   {cand: sum([eda
+00011e70: 7461 2e6d 6172 6769 6e28 6f74 6865 725f  ta.margin(other_
+00011e80: 6361 6e64 2c20 6361 6e64 2920 666f 7220  cand, cand) for 
+00011e90: 6f74 6865 725f 6361 6e64 2069 6e20 6375  other_cand in cu
+00011ea0: 7272 5f63 616e 6473 2069 6620 6564 6174  rr_cands if edat
+00011eb0: 612e 6d61 7267 696e 286f 7468 6572 5f63  a.margin(other_c
+00011ec0: 616e 642c 2063 616e 6429 203e 2030 5d29  and, cand) > 0])
+00011ed0: 2066 6f72 2063 616e 6420 696e 2063 7572   for cand in cur
+00011ee0: 725f 6361 6e64 737d 0a0a 2020 2020 2320  r_cands}..    # 
+00011ef0: 4669 6e64 2074 6865 2063 616e 6469 6461  Find the candida
+00011f00: 7465 7320 7769 7468 2074 6865 206c 6172  tes with the lar
+00011f10: 6765 7374 2073 756d 206f 6620 6d61 7267  gest sum of marg
+00011f20: 696e 7320 6f66 206c 6f73 730a 2020 2020  ins of loss.    
+00011f30: 6d61 785f 7375 6d5f 6f66 5f6d 6172 6769  max_sum_of_margi
+00011f40: 6e73 5f6f 665f 6c6f 7373 203d 206d 6178  ns_of_loss = max
+00011f50: 2873 756d 5f6f 665f 6d61 7267 696e 735f  (sum_of_margins_
+00011f60: 6f66 5f6c 6f73 732e 7661 6c75 6573 2829  of_loss.values()
+00011f70: 290a 2020 2020 6269 6767 6573 745f 6c6f  ).    biggest_lo
+00011f80: 7365 7273 203d 205b 6361 6e64 2066 6f72  sers = [cand for
+00011f90: 2063 616e 6420 696e 2063 7572 725f 6361   cand in curr_ca
+00011fa0: 6e64 7320 6966 2073 756d 5f6f 665f 6d61  nds if sum_of_ma
+00011fb0: 7267 696e 735f 6f66 5f6c 6f73 735b 6361  rgins_of_loss[ca
+00011fc0: 6e64 5d20 3d3d 206d 6178 5f73 756d 5f6f  nd] == max_sum_o
+00011fd0: 665f 6d61 7267 696e 735f 6f66 5f6c 6f73  f_margins_of_los
+00011fe0: 735d 0a0a 2020 2020 7769 6e6e 6572 7320  s]..    winners 
+00011ff0: 3d20 5b5d 0a0a 2020 2020 2320 466f 7220  = []..    # For 
+00012000: 6561 6368 2062 6967 6765 7374 206c 6f73  each biggest los
+00012010: 6572 2c20 6361 6c63 756c 6174 6520 7468  er, calculate th
+00012020: 6520 7769 6e6e 6572 7320 6166 7465 7220  e winners after 
+00012030: 7265 6d6f 7669 6e67 2074 6861 7420 6361  removing that ca
+00012040: 6e64 6964 6174 652e 2054 6865 2075 6e69  ndidate. The uni
+00012050: 6f6e 206f 6620 7468 6573 6520 7365 7473  on of these sets
+00012060: 2069 7320 7468 6520 7365 7420 6f66 2077   is the set of w
+00012070: 696e 6e65 7273 2e0a 2020 2020 666f 7220  inners..    for 
+00012080: 626c 2069 6e20 6269 6767 6573 745f 6c6f  bl in biggest_lo
+00012090: 7365 7273 3a0a 2020 2020 2020 2020 7769  sers:.        wi
+000120a0: 6e6e 6572 735f 7769 7468 6f75 745f 626c  nners_without_bl
+000120b0: 203d 206c 6f73 735f 7472 696d 6d65 7228   = loss_trimmer(
+000120c0: 6564 6174 612c 2063 7572 725f 6361 6e64  edata, curr_cand
+000120d0: 7320 3d20 5b63 616e 6420 666f 7220 6361  s = [cand for ca
+000120e0: 6e64 2069 6e20 6375 7272 5f63 616e 6473  nd in curr_cands
+000120f0: 2069 6620 6361 6e64 2021 3d20 626c 5d29   if cand != bl])
+00012100: 0a20 2020 2020 2020 2077 696e 6e65 7273  .        winners
+00012110: 202b 3d20 7769 6e6e 6572 735f 7769 7468   += winners_with
+00012120: 6f75 745f 626c 0a0a 2020 2020 7265 7475  out_bl..    retu
+00012130: 726e 2073 6f72 7465 6428 6c69 7374 2873  rn sorted(list(s
+00012140: 6574 2877 696e 6e65 7273 2929 290a 0a0a  et(winners)))...
+00012150: 6465 6620 6469 7374 616e 6365 5f74 6f5f  def distance_to_
+00012160: 6d61 7267 696e 5f67 7261 7068 2865 6461  margin_graph(eda
+00012170: 7461 2c20 7265 6c2c 2065 7870 203d 2031  ta, rel, exp = 1
+00012180: 2c20 6375 7272 5f63 616e 6473 203d 204e  , curr_cands = N
+00012190: 6f6e 6529 3a20 0a20 2020 2022 2222 0a20  one): .    """. 
+000121a0: 2020 2043 616c 6375 6c61 7465 2074 6865     Calculate the
+000121b0: 2064 6973 7461 6e63 6520 6f66 2060 6072   distance of ``r
+000121c0: 656c 6060 2028 6120 7265 6c61 7469 6f6e  el`` (a relation
+000121d0: 2920 746f 2074 6865 206d 616a 6f72 6974  ) to the majorit
+000121e0: 7920 6772 6170 6820 6f66 2060 6065 6461  y graph of ``eda
+000121f0: 7461 6060 2e20 0a20 2020 2022 2222 0a20  ta``. .    """. 
+00012200: 2020 2063 616e 6469 6461 7465 7320 3d20     candidates = 
+00012210: 6564 6174 612e 6361 6e64 6964 6174 6573  edata.candidates
+00012220: 2069 6620 6375 7272 5f63 616e 6473 2069   if curr_cands i
+00012230: 7320 4e6f 6e65 2065 6c73 6520 6375 7272  s None else curr
+00012240: 5f63 616e 6473 0a20 2020 200a 2020 2020  _cands.    .    
+00012250: 6966 2074 7970 6528 6564 6174 6129 203d  if type(edata) =
+00012260: 3d20 4d61 6a6f 7269 7479 4772 6170 6820  = MajorityGraph 
+00012270: 616e 6420 6578 7020 3d3d 2030 3a0a 2020  and exp == 0:.  
+00012280: 2020 2020 2020 2320 6966 2065 6461 7461        # if edata
+00012290: 2069 7320 6120 4d61 6a6f 7269 7479 4772   is a MajorityGr
+000122a0: 6170 682c 2077 6520 6e65 6564 2074 6f20  aph, we need to 
+000122b0: 6164 6420 6d61 7267 696e 7320 666f 7220  add margins for 
+000122c0: 7468 6520 666f 6c6c 6f77 696e 6720 636f  the following co
+000122d0: 6465 2074 6f20 776f 726b 2e20 2054 6865  de to work.  The
+000122e0: 206d 6172 6769 6e73 2064 6f20 6e6f 7420   margins do not 
+000122f0: 6d61 7474 6572 2077 6865 6e20 6578 703d  matter when exp=
+00012300: 3d30 2e20 2020 0a20 2020 2020 2020 2065  =0.   .        e
+00012310: 6461 7461 203d 204d 6172 6769 6e47 7261  data = MarginGra
+00012320: 7068 2863 616e 6469 6461 7465 732c 205b  ph(candidates, [
+00012330: 2863 312c 2063 322c 2031 2920 666f 7220  (c1, c2, 1) for 
+00012340: 6331 2c20 6332 2069 6e20 6564 6174 612e  c1, c2 in edata.
+00012350: 6564 6765 7320 6966 2028 6331 2069 6e20  edges if (c1 in 
+00012360: 6361 6e64 6964 6174 6573 2061 6e64 2063  candidates and c
+00012370: 3220 696e 2063 616e 6469 6461 7465 7329  2 in candidates)
+00012380: 5d29 0a20 2020 2070 656e 616c 7479 203d  ]).    penalty =
+00012390: 2030 0a20 2020 2066 6f72 2061 2c62 2069   0.    for a,b i
+000123a0: 6e20 636f 6d62 696e 6174 696f 6e73 2863  n combinations(c
+000123b0: 616e 6469 6461 7465 732c 2032 293a 200a  andidates, 2): .
+000123c0: 2020 2020 2020 2020 6966 2065 6461 7461          if edata
+000123d0: 2e6d 616a 6f72 6974 795f 7072 6566 6572  .majority_prefer
+000123e0: 7328 612c 2062 2920 616e 6420 2862 2c61  s(a, b) and (b,a
+000123f0: 2920 696e 2072 656c 3a20 0a20 2020 2020  ) in rel: .     
+00012400: 2020 2020 2020 2070 656e 616c 7479 202b         penalty +
+00012410: 3d20 2865 6461 7461 2e6d 6172 6769 6e28  = (edata.margin(
+00012420: 612c 2062 2920 2a2a 2065 7870 290a 2020  a, b) ** exp).  
+00012430: 2020 2020 2020 656c 6966 2065 6461 7461        elif edata
+00012440: 2e6d 616a 6f72 6974 795f 7072 6566 6572  .majority_prefer
+00012450: 7328 622c 2061 2920 616e 6420 2861 2c62  s(b, a) and (a,b
+00012460: 2920 696e 2072 656c 3a20 0a20 2020 2020  ) in rel: .     
+00012470: 2020 2020 2020 2070 656e 616c 7479 202b         penalty +
+00012480: 3d20 2865 6461 7461 2e6d 6172 6769 6e28  = (edata.margin(
+00012490: 622c 2061 2920 2a2a 2065 7870 290a 2020  b, a) ** exp).  
+000124a0: 2020 2020 2020 656c 6966 2065 6461 7461        elif edata
+000124b0: 2e6d 616a 6f72 6974 795f 7072 6566 6572  .majority_prefer
+000124c0: 7328 612c 2062 2920 616e 6420 2861 2c62  s(a, b) and (a,b
+000124d0: 2920 6e6f 7420 696e 2072 656c 2061 6e64  ) not in rel and
+000124e0: 2028 622c 6129 206e 6f74 2069 6e20 7265   (b,a) not in re
+000124f0: 6c3a 200a 2020 2020 2020 2020 2020 2020  l: .            
+00012500: 7065 6e61 6c74 7920 2b3d 2028 6564 6174  penalty += (edat
+00012510: 612e 6d61 7267 696e 2861 2c20 6229 202a  a.margin(a, b) *
+00012520: 2a20 6578 7029 202f 2032 200a 2020 2020  * exp) / 2 .    
+00012530: 2020 2020 656c 6966 2065 6461 7461 2e6d      elif edata.m
+00012540: 616a 6f72 6974 795f 7072 6566 6572 7328  ajority_prefers(
+00012550: 622c 2061 2920 616e 6420 2861 2c62 2920  b, a) and (a,b) 
+00012560: 6e6f 7420 696e 2072 656c 2061 6e64 2028  not in rel and (
+00012570: 622c 6129 206e 6f74 2069 6e20 7265 6c3a  b,a) not in rel:
+00012580: 200a 2020 2020 2020 2020 2020 2020 7065   .            pe
+00012590: 6e61 6c74 7920 2b3d 2028 6564 6174 612e  nalty += (edata.
+000125a0: 6d61 7267 696e 2862 2c20 6129 202a 2a20  margin(b, a) ** 
+000125b0: 6578 7029 2020 2f20 320a 2020 2020 7265  exp)  / 2.    re
+000125c0: 7475 726e 2070 656e 616c 7479 0a         turn penalty.
```

### Comparing `pref_voting-1.2.0/pref_voting/margin_based_methods_old.py` & `pref_voting-1.3.0/pref_voting/margin_based_methods_old.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/monotonicity_axioms.py` & `pref_voting-1.3.0/pref_voting/monotonicity_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/other_methods.py` & `pref_voting-1.3.0/pref_voting/other_methods.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,20 +7,21 @@
     Implementations of 
 '''
 
 from pref_voting.voting_method import *
 from pref_voting.scoring_methods import plurality
 from pref_voting.profiles import _find_updated_profile, _num_rank
 from pref_voting.profiles_with_ties import ProfileWithTies
-from pref_voting.helper import get_mg
+from pref_voting.weighted_majority_graphs import MarginGraph
 from itertools import combinations, permutations
-import networkx as nx
+from pref_voting.voting_method_properties import VotingMethodProperties, ElectionTypes
 
-
-@vm(name = "Majority")
+@vm(name = "Majority",
+    skip_registration=True, # skip registration since majority may return an empty list
+    input_types = [ElectionTypes.PROFILE])
 def majority(profile, curr_cands = None):
     """The majority winner is the candidate with a strict majority  of first place votes.  Returns an empty list if there is no candidate with a strict majority of first place votes. Returns the majority winner in the ``profile`` restricted to ``curr_cands``.
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
@@ -49,47 +50,54 @@
     curr_cands = profile.candidates if curr_cands is None else curr_cands
 
     plurality_scores = profile.plurality_scores(curr_cands = curr_cands)
     maj_winner = [c for c in curr_cands if plurality_scores[c] >= maj_size]
 
     return sorted(maj_winner)
 
-@vm(name = "Pareto")
-def pareto(prof, curr_cands = None, strong_Pareto = False, use_extended_strict_preferences = True):
+pareto_properties = VotingMethodProperties(
+    condorcet_winner=False,
+    condorcet_loser=False,
+    pareto_dominance=True,
+)
+@vm(name = "Pareto",
+    properties = pareto_properties,
+    input_types = [ElectionTypes.PROFILE, ElectionTypes.PROFILE_WITH_TIES])
+def pareto(profile, curr_cands = None, strong_Pareto = False, use_extended_strict_preferences = True):
     """Returns the set of candidates who are not Pareto dominated.
 
     For ProfilesWithTies, if strong_Pareto == True, then a dominates b if some voter strictly prefers a to b and no voter strictly prefers b to a.
 
     Args:
         prof (Profile, ProfileWithTies): An anonymous profile of linear (or strict weak) orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
     Returns: 
         A sorted list of candidates
 
     """
 
-    if type(prof) == ProfileWithTies:
-        currently_using_extended_strict_preferences = prof.using_extended_strict_preference
+    if type(profile) == ProfileWithTies:
+        currently_using_extended_strict_preferences = profile.using_extended_strict_preference
         if use_extended_strict_preferences:
-            prof.use_extended_strict_preference()
+            profile.use_extended_strict_preference()
         
     Pareto_dominated = set()
-    candidates = prof.candidates if curr_cands is None else curr_cands
+    candidates = profile.candidates if curr_cands is None else curr_cands
     for a in candidates:
         for b in candidates:
-            if not strong_Pareto and prof.support(a,b) == prof.num_voters:
+            if not strong_Pareto and profile.support(a,b) == profile.num_voters:
                 Pareto_dominated.add(b)
 
-            if strong_Pareto and prof.support(a,b) > 0 and prof.support(b,a) == 0:
+            if strong_Pareto and profile.support(a,b) > 0 and profile.support(b,a) == 0:
                 Pareto_dominated.add(b)     
 
-    if type(prof) == ProfileWithTies and use_extended_strict_preferences:
+    if type(profile) == ProfileWithTies and use_extended_strict_preferences:
         if not currently_using_extended_strict_preferences:
-            prof.use_strict_preference()
+            profile.use_strict_preference()
 
     return sorted(list(set(candidates) - Pareto_dominated))
     
 
 ## Kemeny-Young Method 
 #
 def kendalltau_dist(rank_a, rank_b):
@@ -151,21 +159,29 @@
     """
     candidates = profile.candidates if curr_cands is None else curr_cands
     
     rankings = profile._rankings if curr_cands is None else _find_updated_profile(profile._rankings, np.array([c for c in profile.candidates if c not in curr_cands]),  profile.num_cands)
     return _kemeny_young_rankings(list(rankings), list(profile._rcounts), candidates)
 
 
-@vm(name = "Kemeny-Young")
-def kemeny_young(profile, curr_cands = None): 
-    """A Kemeny-Young ranking is a ranking that minimizes the sum of the Kendall tau distances to the voters' rankings.  The Kemeny-Young winners are the candidates that are ranked first by some Kemeny-Young ranking.
+kemeny_young_properties = VotingMethodProperties(
+    condorcet_winner=True,
+    condorcet_loser=True,
+    pareto_dominance=True,
+)
+@vm(name = "Kemeny-Young",
+    properties = kemeny_young_properties,
+    input_types = [ElectionTypes.PROFILE,ElectionTypes.PROFILE_WITH_TIES,  ElectionTypes.MARGIN_GRAPH])
+def kemeny_young(edata, curr_cands = None, algorithm = "marginal"): 
+    """A Kemeny-Young ranking is a ranking that maximizes the sum of the margins of pairs of candidates in the ranking. Equivalently, a Kemeny-Young ranking is a ranking that minimizes the sum of the Kendall tau distances to the voters' rankings. The Kemeny-Young winners are the candidates that are ranked first by some Kemeny-Young ranking.
 
     Args:
-        profile (Profile): An anonymous profile of linear orders on a set of candidates
+        edata (Profile, ProfileWithTies, MarginGraph): Any election data that has a `margin` method.
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
+        algorithm (str, optional): The algorithm to use.  Options are "marginal" and "Kendall tau". If "marginal" is used, then the Kemeny-Young rankings are computed by finding the sum of the margins of each pair of candidates in the ranking.  If "Kendall tau" is used, then the Kemeny-Young rankings are computed by summing the Kendall tau distances to the voters' rankings.  Default is "marginal".
 
     Returns: 
         A sorted list of candidates
 
     :Example:
 
         .. exec_code::
@@ -186,25 +202,108 @@
             kyrs, d = kemeny_young_rankings(prof2)
             print(f"Minimal distance: {d}")
             for kyr in kyrs: 
                 print(f"ranking: {kyr}")
             kemeny_young.display(prof2)
 
     """
+    assert algorithm in ["marginal", "Kendall tau"], "Algorithm must be either 'marginal' or 'Kendall tau'."
 
-    candidates = profile.candidates if curr_cands is None else curr_cands
-    
-    rankings = profile._rankings if curr_cands is None else _find_updated_profile(profile._rankings, np.array([c for c in profile.candidates if c not in curr_cands]),  profile.num_cands)
-    ky_rankings, min_dist = _kemeny_young_rankings(list(rankings), list(profile._rcounts), candidates)
+    candidates = edata.candidates if curr_cands is None else curr_cands
+
+    if isinstance(edata, MarginGraph) or isinstance(edata,ProfileWithTies):
+        algorithm = "marginal"
+
+    if algorithm == "Kendall tau":
+        rankings = edata._rankings if curr_cands is None else _find_updated_profile(edata._rankings, np.array([c for c in edata.candidates if c not in curr_cands]), edata.num_cands)
+        ky_rankings, min_dist = _kemeny_young_rankings(list(rankings), list(edata._rcounts), candidates)
+
+    if algorithm == "marginal":
+
+        best_ranking_score = 0
+        ky_rankings = []
+
+        for r in permutations(candidates):
+
+            score_of_r = 0 
+            for i in r[:-1]:
+                for j in r[r.index(i)+1:]:
+                    score_of_r += edata.margin(i,j)
+
+            if score_of_r > best_ranking_score:
+                best_ranking_score = score_of_r
+                ky_rankings = [r]
+            if score_of_r == best_ranking_score:
+                ky_rankings.append(r)
     
     return sorted(list(set([r[0] for r in ky_rankings])))
 
+preliminary_weighted_condorcet_properties = VotingMethodProperties(
+    condorcet_winner=True,
+    condorcet_loser=True,
+    pareto_dominance=True,
+)
+@vm("Preliminary Weighted Condorcet",
+    properties = preliminary_weighted_condorcet_properties,
+    input_types = [ElectionTypes.PROFILE])
+def preliminary_weighted_condorcet(prof, curr_cands = None, show_orders = False, require_positive_plurality_score = False):
+    """The preliminary version of the Weighted Condorcet Rule in Tideman's book, Collective Decisions and Voting (p. 223). The winners are the candidates ranked first by some linear order of the candidates with highest score, where the score of an order (c_1,...,c_n) is the sum over all i<j of the margin of c_i vs. c_j multiplied by the plurality scores of c_i and c_j. 
+    
+    The multiplication by plurality scores is what distinguishes this method from the Kemeny-Young method.
+    
+    Tideman (p. 224) defines a more complicated Weighted Condorcet rule that is intended to be used when some candidates receive zero first-place votes.
+    
+    Args:
+        prof (Profile): An anonymous profile of linear orders on a set of candidates
+        curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
+        show_orders (bool): If True, then print the set of best orders.
+        require_positive_plurality_score (bool): If True, then require that all candidates have a positive plurality score.
+
+    Returns:
+        A sorted list of candidates
+    """
+
+    cands = curr_cands if curr_cands is not None else prof.candidates
+
+    if require_positive_plurality_score:
+        assert all([prof.plurality_scores(curr_cands=curr_cands)[c] > 0 for c in cands]), "All candidates must have a positive plurality score."
+
+    best_order_score = 0
+    best_orders = []
+
+    for r in permutations(cands):
+
+        score_of_r = 0 
+        for i in r[:-1]:
+            for j in r[r.index(i)+1:]:
+                score_of_r += (prof.plurality_scores(curr_cands=curr_cands)[i] * prof.plurality_scores(curr_cands=curr_cands)[j] * prof.margin(i,j))
+
+        if score_of_r > best_order_score:
+            best_order_score = score_of_r
+            best_orders = [r]
+        if score_of_r == best_order_score:
+            best_orders.append(r)
+
+    if show_orders == True:
+        print(f"Best orders: {set(best_orders)}")
+
+    winners = [r[0] for r in best_orders]
+
+    return list(set(winners))
+
 ### Bucklin
 
-@vm(name = "Bucklin")
+bucklin_properties = VotingMethodProperties(
+    condorcet_winner=False,
+    condorcet_loser=False,
+    pareto_dominance=True,
+)
+@vm(name = "Bucklin",
+    properties = bucklin_properties,
+    input_types = [ElectionTypes.PROFILE])
 def bucklin(profile, curr_cands = None): 
     """If a candidate has a strict majority of first-place votes, then that candidate is the winner. If no such candidate exists, then check the candidates that are ranked first or second.  If a candidate has a strict majority of first- or second-place voters, then that candidate is the winner. If no such winner is found move on to the 3rd, 4th, etc. place votes.  Return the candidates with the greatest overall score.  
     
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
@@ -299,16 +398,22 @@
                        for c in candidates}
         if any([s >= strict_maj_size for s in cand_scores.values()]):
             break
     max_score = max(cand_scores.values())
     return sorted([c for c in candidates if cand_scores[c] >= max_score]), cand_scores
 
 
-
-@vm(name = "Simplified Bucklin")
+simplified_bucklin_properties = VotingMethodProperties(
+    condorcet_winner=False,
+    condorcet_loser=False,
+    pareto_dominance=True,
+)
+@vm(name = "Simplified Bucklin",
+    properties = simplified_bucklin_properties,
+    input_types = [ElectionTypes.PROFILE])
 def simplified_bucklin(profile, curr_cands = None): 
     """If a candidate has a strict majority of first-place votes, then that candidate is the winner. If no such candidate exists, then check the candidates that are ranked first or second.  If a candidate has a strict majority of first- or second-place voters, then that candidate is the winner. If no such winner is found move on to the 3rd, 4th, etc. place votes. 
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
@@ -401,16 +506,22 @@
         cand_scores = {c:sum([cand_to_num_voters_rank[_r][c] for _r in cand_to_num_voters_rank.keys()]) 
                        for c in candidates}
         if any([s >= strict_maj_size for s in cand_scores.values()]):
             break
             
     return sorted([c for c in candidates if cand_scores[c] >= strict_maj_size]), cand_scores
 
-
-@vm(name = "Weighted Bucklin")
+weighted_bucklin_properties = VotingMethodProperties(
+    condorcet_winner=False,
+    condorcet_loser=None,
+    pareto_dominance=True,
+)
+@vm(name = "Weighted Bucklin",
+    properties = weighted_bucklin_properties,
+    input_types = [ElectionTypes.PROFILE])
 def weighted_bucklin(profile, curr_cands = None, strict_threshold = False, score = lambda num_cands, rank: (num_cands - rank)/ (num_cands - 1) if num_cands > 1 else 1): 
     """The Weighted Bucklin procedure, studied by D. Marc Kilgour, Jean-Charles Grégoire, and Angèle Foley. The k-th Weighted Bucklin score of a candidate c is the sum for j \leq k of the product of score(num_cands,j) and the number of voters who rank c in j-th place. Compute higher-order Weighted Bucklin scores until reaching a k such that some candidate's k-th Weighted Bucklin score is at least half the number of voters (or the strict majority size if strict_threshold = True). Then return the candidates with maximal k-th Weighted Bucklin score. Bucklin is the special case where strict_threshold = True and score = lambda num_cands, rank: 1.
     
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
         strict_threshold: If True, makes the threshold for the Bucklin procedure the strict majority size; otherwise threshold is half the number of voters, following Kilgour et al.
@@ -456,16 +567,22 @@
                        for c in candidates}
         if any([s >= threshold for s in cand_scores.values()]):
             break
     max_score = max(cand_scores.values())
 
     return sorted([c for c in candidates if cand_scores[c] >= max_score])
 
-
-@vm(name = "Bracket Voting")
+bracket_voting_properties = VotingMethodProperties(
+    condorcet_winner=False,
+    condorcet_loser=True,
+    pareto_dominance=True,
+)
+@vm(name = "Bracket Voting",
+    properties = bracket_voting_properties,
+    input_types = [ElectionTypes.PROFILE])
 def bracket_voting(profile, curr_cands = None, seed = None):
     """The candidates with the top four plurality scores are seeded into a bracket: the candidate with the highest plurality score is seeded 1st, the candidate with the second highest plurality score is seeded 2nd, etc. The 1st seed faces the 4th seed in a head-to-head match decided by majority rule, and the 2nd seed faces the 3rd seed in a head-to-head match decided by majority rule. The winners of these two matches face each other in a final head-to-head match decided by majority rule. The winner of the final is the winner of the election.
 
     .. note::
         A version of bracket voting as proposed by Edward B. Foley. This is a probabilistic method that always returns a unique winner. Ties are broken using a random tie breaking ordering of the candidates.
 
     Args:
@@ -522,15 +639,22 @@
 
     # Ties in the final head-to-head match are broken in favor of the higher-seeded candidate
     else:
         winner = one_four_winner if one_four_winner_seed < two_three_winner_seed else two_three_winner
 
     return [winner]
 
-@vm(name = "Superior Voting")
+superior_voting_properties = VotingMethodProperties(
+    condorcet_winner=False,
+    condorcet_loser=True,
+    pareto_dominance=True,
+)
+@vm(name = "Superior Voting",
+    properties = superior_voting_properties,
+    input_types = [ElectionTypes.PROFILE])
 def superior_voting(profile, curr_cands = None):
     """One candidate is superior to another if more ballots rank the first candidate above the second than vice versa. A candidate earns a point from a ballot if they are ranked first on that ballot or they are superior to the candidate ranked first on that ballot. The candidate with the most points wins.
 
     .. note::
         Devised by Wesley H. Holliday as a simple Condorcet-compliant method for political elections. Always elects a Condorcet winner if one exists and elects only the Condorcet winner provided the Condorcet winner receives at least one first-place vote. Edward B. Foley suggested the name 'Superior Voting' because the method is based on the idea that if A is superior to B, then A should get B's first-place votes added to their own.
 
     Args:
@@ -551,17 +675,7 @@
                 points[cand] += profile.plurality_scores(curr_cands)[other_cand]
     
     # Find the candidates with the most points
     max_score = max(points.values())
     winners = [cand for cand in curr_cands if points[cand] == max_score]
 
     return winners
-
-other_vms = [
-    kemeny_young, 
-    majority, 
-    bucklin,
-    simplified_bucklin,
-    weighted_bucklin,
-    bracket_voting,
-    superior_voting
-]
```

### Comparing `pref_voting-1.2.0/pref_voting/prob_voting_method.py` & `pref_voting-1.3.0/pref_voting/prob_voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/probabilistic_methods.py` & `pref_voting-1.3.0/pref_voting/probabilistic_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/profiles.py` & `pref_voting-1.3.0/pref_voting/profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/profiles_with_ties.py` & `pref_voting-1.3.0/pref_voting/profiles_with_ties.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/rankings.py` & `pref_voting-1.3.0/pref_voting/rankings.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/scoring_methods.py` & `pref_voting-1.3.0/pref_voting/scoring_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 '''
 from pref_voting.voting_method import  *
 from pref_voting.social_welfare_function import  *
 from pref_voting.profiles import Profile
 from pref_voting.rankings import Ranking, break_ties_alphabetically
 from pref_voting.voting_method import _num_rank_last 
 from pref_voting.profiles import _find_updated_profile, _num_rank
+from pref_voting.weighted_majority_graphs import MarginGraph
 from pref_voting.voting_method_properties import VotingMethodProperties, ElectionTypes
 
 pl_properties = VotingMethodProperties(
     condorcet_winner=False, 
     condorcet_loser=False,
-    pareto_dominance=False, 
+    pareto_dominance=True, 
     )
 @vm(name = "Plurality", 
     properties=pl_properties, 
     input_types=[ElectionTypes.PROFILE, 
                  ElectionTypes.TRUNCATED_LINEAR_PROFILE])
 def plurality(profile, curr_cands = None):
     """The **Plurality score** of a candidate :math:`c` is the number of voters that rank :math:`c` in first place. The Plurality winners are the candidates with the largest Plurality score in the ``profile`` restricted to ``curr_cands``.
@@ -106,25 +107,28 @@
 borda_properties = VotingMethodProperties(
     condorcet_winner=False, 
     condorcet_loser=True,
     pareto_dominance=True, 
     )
 @vm(name = "Borda",
     properties=borda_properties,
-    input_types=[ElectionTypes.PROFILE])
-def borda(profile, curr_cands = None):
-    r"""The **Borda score** of a candidate is calculated as follows: If there are :math:`m` candidates, then the Borda score of candidate :math:`c` is :math:`\sum_{r=1}^{m} (m - r) * Rank(c,r)` where :math:`Rank(c,r)` is the number of voters that rank candidate :math:`c` in position :math:`r`. The Borda winners are the candidates with the largest Borda score in the ``profile`` restricted to ``curr_cands``. 
-
+    input_types=[ElectionTypes.PROFILE, ElectionTypes.MARGIN_GRAPH])
+def borda(edata, curr_cands = None, algorithm = "positional"):
+    """The **Borda score** of a candidate is calculated as follows: If there are :math:`m` candidates, then the Borda score of candidate :math:`c` is :math:`\sum_{r=1}^{m} (m - r) * Rank(c,r)` where :math:`Rank(c,r)` is the number of voters that rank candidate :math:`c` in position :math:`r`. The Borda winners are the candidates with the largest Borda score in the ``profile`` restricted to ``curr_cands``. 
     Args:
-        profile (Profile): An anonymous profile of linear orders on a set of candidates
+        edata (Profile, MarginGraph): An anonymous profile of linear orders or a MarginGraph.
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
+        algorithm (String): if "positional", then the Borda score of a candidate is calculated from each voter's ranking as described above. If "marginal", then the Borda score of a candidate is calculated as the sum of the margins of the candidate vs. all other candidates. The positional scores and marginal scores are affinely equivalent.
 
     Returns: 
         A sorted list of candidates
 
+    .. note:
+        If edata is a MarginGraph, then the "marginal" algorithm is used.
+
     .. seealso::
 
         The method :meth:`pref_voting.profiles.Profile.borda_scores` returns a dictionary assigning the Borda score to each candidate. 
         
     :Example:
 
     .. exec_code::
@@ -140,18 +144,25 @@
         prof2 = Profile([[0, 1, 2], [1, 0, 2], [1, 2, 0]], [3, 1, 2])
         prof2.display()
         print(borda(prof2)) # [1]
         borda.display(prof2)
 
     """
 
-    curr_cands = profile.candidates if curr_cands is None else curr_cands
+    curr_cands = edata.candidates if curr_cands is None else curr_cands
 
-    # get the Borda scores for all the candidates in curr_cands
-    borda_scores = profile.borda_scores(curr_cands = curr_cands)
+    if isinstance(edata,MarginGraph):
+        algorithm = "marginal"
+
+    if algorithm == "positional":
+        # get the Borda scores for all the candidates in curr_cands
+        borda_scores = edata.borda_scores(curr_cands = curr_cands)
+
+    if algorithm == "marginal":
+        borda_scores = {c: sum([edata.margin(c,d) for d in curr_cands]) for c in curr_cands}
     
     max_borda_score = max(borda_scores.values())
     
     return sorted([c for c in curr_cands if borda_scores[c] == max_borda_score])
 
 @swf(name="Borda ranking")
 def borda_ranking(profile, curr_cands=None, local=True, tie_breaking=None):
@@ -467,15 +478,15 @@
 
 
 borda_prof_with_ties_properties = VotingMethodProperties(
     condorcet_winner=None, 
     condorcet_loser=None,
     pareto_dominance=None, 
     )
-@vm(name="Borda",
+@vm(name="Borda (for Truncated Profiles)",
     properties=borda_prof_with_ties_properties,
     input_types=[ElectionTypes.TRUNCATED_LINEAR_PROFILE])
 def borda_for_profile_with_ties(
     profile, 
     curr_cands=None, 
     borda_scores=symmetric_borda_scores): 
     """
@@ -500,29 +511,7 @@
 scoring_swfs = [
     plurality_ranking,
     borda_ranking,
     anti_plurality_ranking,
     score_ranking   
 ]
 
-scoring_vms = [
-    anti_plurality,
-    plurality, 
-    borda, 
-    borda_for_profile_with_ties,
-    dowdall,
-    scoring_rule,
-    positive_negative_voting,
-]
-
-scoring_vms_profiles = [
-    plurality, 
-    borda, 
-    anti_plurality,
-    scoring_rule, 
-    positive_negative_voting,
-    anti_plurality  
-]
-
-scoring_vms_profiles_with_ties = [
-    borda_for_profile_with_ties
-]
```

### Comparing `pref_voting-1.2.0/pref_voting/social_welfare_function.py` & `pref_voting-1.3.0/pref_voting/social_welfare_function.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/spatial_profiles.py` & `pref_voting-1.3.0/pref_voting/spatial_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/strategic_axioms.py` & `pref_voting-1.3.0/pref_voting/strategic_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/swf_axioms.py` & `pref_voting-1.3.0/pref_voting/swf_axioms.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,20 +111,20 @@
                     core_support_for_y_vs_y = [r for r in prof.rankings if r.index(y) == 0 or r.index(y) < min([r.index(c) for c in maj_cand_for_y if c != y])]
                     core_support = core_support_for_x_vs_y + core_support_for_y_vs_y
                     restricted_prof = Profile(core_support)
 
                 if not restricted_prof.majority_prefers(x,y):
                     if verbose:
                         print(f"Core support violation by {swf} for {x} relative to {y}:")
-                        print(prof)
+                        print(prof.anonymize())
                         prof.display_margin_graph()
                         print("Social ranking:",social_ranking)
                         print(f"Major candidates relative to {y}:",maj_cand_for_y)
                         print(f"Profile restricted to voters in core support for {x} relative to {y} and for {y} relative to {y}:")
-                        print(restricted_prof)
+                        print(restricted_prof.anonymize())
                         restricted_prof.display_margin_graph()
                     return True
     return False
 
 def find_all_core_support_violations(prof,swf,verbose=False):
     """Returns a list of all pairs of candidates for which the swf violates the "core support criterion" of https://arxiv.org/abs/2308.08430 for the given profile. If verbose is True, prints the profile and the core support violation.
 
@@ -152,20 +152,20 @@
                     core_support_for_y_vs_y = [r for r in prof.rankings if r.index(y) == 0 or r.index(y) < min([r.index(c) for c in maj_cand_for_y if c != y])]
                     core_support = core_support_for_x_vs_y + core_support_for_y_vs_y
                     restricted_prof = Profile(core_support)
 
                 if not restricted_prof.majority_prefers(x,y):
                     if verbose:
                         print(f"Core support violation by {swf} for {x} relative to {y}:")
-                        print(prof)
+                        print(prof.anonymize())
                         prof.display_margin_graph()
                         print("Social ranking:",social_ranking)
                         print(f"Major candidates relative to {y}:",maj_cand_for_y)
                         print(f"Profile restricted to voters in core support for {x} relative to {y} and for {y} relative to {y}:")
-                        print(restricted_prof)
+                        print(restricted_prof.anonymize())
                         restricted_prof.display_margin_graph()
                     violations.append((x,y))
     return violations
 
 core_support = Axiom(
     "Core Support",
     has_violation = has_core_support_violation,
```

### Comparing `pref_voting-1.2.0/pref_voting/tests/conftest.py` & `pref_voting-1.3.0/pref_voting/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/tests/test_c1_methods.py` & `pref_voting-1.3.0/pref_voting/tests/test_c1_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/tests/test_combined_methods.py` & `pref_voting-1.3.0/pref_voting/tests/test_combined_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/tests/test_generate_profiles.py` & `pref_voting-1.3.0/pref_voting/tests/test_generate_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/tests/test_generate_spatial_profile.py` & `pref_voting-1.3.0/pref_voting/tests/test_generate_spatial_profile.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/tests/test_io.py` & `pref_voting-1.3.0/pref_voting/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/tests/test_iterative_methods.py` & `pref_voting-1.3.0/pref_voting/tests/test_iterative_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/tests/test_majority_graph.py` & `pref_voting-1.3.0/pref_voting/tests/test_majority_graph.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/tests/test_mapping.py` & `pref_voting-1.3.0/pref_voting/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/tests/test_margin_based_methods.py` & `pref_voting-1.3.0/pref_voting/tests/test_margin_based_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/tests/test_margin_graph.py` & `pref_voting-1.3.0/pref_voting/tests/test_margin_graph.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/tests/test_other_methods.py` & `pref_voting-1.3.0/pref_voting/tests/test_other_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/tests/test_prob_voting_method.py` & `pref_voting-1.3.0/pref_voting/tests/test_prob_voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/tests/test_profile.py` & `pref_voting-1.3.0/pref_voting/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/tests/test_profile_with_ties.py` & `pref_voting-1.3.0/pref_voting/tests/test_profile_with_ties.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/tests/test_ranking.py` & `pref_voting-1.3.0/pref_voting/tests/test_ranking.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/tests/test_scoring_rules.py` & `pref_voting-1.3.0/pref_voting/tests/test_scoring_rules.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/tests/test_social_welfare_functions.py` & `pref_voting-1.3.0/pref_voting/tests/test_social_welfare_functions.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/tests/test_spatial_profile.py` & `pref_voting-1.3.0/pref_voting/tests/test_spatial_profile.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/tests/test_support_graph.py` & `pref_voting-1.3.0/pref_voting/tests/test_support_graph.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/tests/test_utility_function.py` & `pref_voting-1.3.0/pref_voting/tests/test_utility_function.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/tests/test_utility_functions.py` & `pref_voting-1.3.0/pref_voting/tests/test_utility_functions.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/tests/test_voting_method.py` & `pref_voting-1.3.0/pref_voting/tests/test_voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/utility_functions.py` & `pref_voting-1.3.0/pref_voting/utility_functions.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/utility_methods.py` & `pref_voting-1.3.0/pref_voting/utility_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/utility_profiles.py` & `pref_voting-1.3.0/pref_voting/utility_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/variable_candidate_axioms.py` & `pref_voting-1.3.0/pref_voting/variable_candidate_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/variable_voter_axioms.py` & `pref_voting-1.3.0/pref_voting/variable_voter_axioms.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,15 +271,15 @@
     if require_uniquely_weighted and not prof.is_uniquely_weighted():
         return False
 
     if violation_type == "Removal":
         if uniform_coalition:
             for loser in losers:
 
-                relevant_ranking_types = [r for r in prof.ranking_types if prof.rankings.count(r) >= coalition_size]
+                relevant_ranking_types = [r for r in prof.ranking_types if r[0] == loser and prof.rankings.count(r) >= coalition_size]
 
                 for r in relevant_ranking_types:
 
                     rankings = prof.rankings
 
                     for i in range(coalition_size):
                         rankings.remove(r) # remove coalition_size-many tokens of the type of ranking
```

### Comparing `pref_voting-1.2.0/pref_voting/voting_method.py` & `pref_voting-1.3.0/pref_voting/voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/voting_method_properties.py` & `pref_voting-1.3.0/pref_voting/voting_method_properties.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pref_voting/weighted_majority_graphs.py` & `pref_voting-1.3.0/pref_voting/weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.2.0/pyproject.toml` & `pref_voting-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "pref_voting"
-version = "1.2.0"
+version = "1.3.0"
 description = "pref_voting is a Python package that contains tools to reason about elections and margin graphs, and implementations of voting methods."
 authors = ["Eric Pacuit <epacuit@umd.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/voting-tools/pref_voting"
 repository = "https://github.com/voting-tools/pref_voting"
```

### Comparing `pref_voting-1.2.0/setup.py` & `pref_voting-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'prefsampling>=0.1.16,<0.2.0',
  'random2>=1.0.1,<2.0.0',
  'scipy>=1.0.0,<2.0.0',
  'tabulate>=0.9.0,<0.10.0']
 
 setup_kwargs = {
     'name': 'pref-voting',
-    'version': '1.2.0',
+    'version': '1.3.0',
     'description': 'pref_voting is a Python package that contains tools to reason about elections and margin graphs, and implementations of voting methods.',
     'long_description': 'pref_voting\n==========\n\n## Installation\n\nWith pip package manager:\n\n```bash\npip install pref_voting\n```\n\n## Documentation\n\nOnline documentation is available at [https://pref-voting.readthedocs.io](https://pref-voting.readthedocs.io).\n\n## Example Usage\n\nA profile (of linear orders over the candidates) is created by initializing a `Profile` class object.  Simply provide a list of rankings (each ranking is a tuple of numbers) and a list giving the number of voters with each ranking:\n\n```python\nfrom pref_voting.profiles import Profile\n\nrankings = [\n    (0, 1, 2, 3), \n    (2, 3, 1, 0), \n    (3, 1, 2, 0), \n    (1, 2, 0, 3), \n    (1, 3, 2, 0)]\n\nrcounts = [5, 3, 2, 4, 3]\n\nprof = Profile(rankings, rcounts=rcounts)\n```\n\nThe function `generate_profile` is used to generate a profile for a given number of candidates and voters:  \n\n```python\nfrom pref_voting.generate_profiles import generate_profile\n\n# generate a profile using the Impartial Culture probability model\nprof = generate_profile(3, 4) # prof is a Profile object\n\n# generate a profile using the Impartial Anonymous Culture probability model\nprof = generate_profile(3, 4, probmod = "IAC") # prof is a Profile object \n```\n\nTo use one of the many voting methods, import the function from `pref_voting.voting_methods` and apply it to the profile: \n\n```python\nfrom pref_voting.generate_profiles import generate_profile\nfrom pref_voting.voting_methods import *\n\nprof = generate_profile(3, 4)\nsplit_cycle(prof) # returns the sorted list of winning candidates\nsplit_cycle.display(prof) # display the winning candidates\n\n```\n\n## Questions?\n\nFeel free to [send an email](https://pacuit.org/) if you have questions about the project.\n\n## License\n\n[MIT](https://github.com/jontingvold/pyrankvote/blob/master/LICENSE.txt)\n',
     'author': 'Eric Pacuit',
     'author_email': 'epacuit@umd.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/voting-tools/pref_voting',
```

### Comparing `pref_voting-1.2.0/PKG-INFO` & `pref_voting-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pref-voting
-Version: 1.2.0
+Version: 1.3.0
 Summary: pref_voting is a Python package that contains tools to reason about elections and margin graphs, and implementations of voting methods.
 Home-page: https://github.com/voting-tools/pref_voting
 License: MIT
 Author: Eric Pacuit
 Author-email: epacuit@umd.edu
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

