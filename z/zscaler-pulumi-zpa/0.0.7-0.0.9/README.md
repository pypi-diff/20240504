# Comparing `tmp/zscaler_pulumi_zpa-0.0.7.tar.gz` & `tmp/zscaler_pulumi_zpa-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zscaler_pulumi_zpa-0.0.7.tar", last modified: Wed Mar 27 02:03:53 2024, max compression
+gzip compressed data, was "zscaler_pulumi_zpa-0.0.9.tar", last modified: Wed Mar 27 03:20:54 2024, max compression
```

## Comparing `zscaler_pulumi_zpa-0.0.7.tar` & `zscaler_pulumi_zpa-0.0.9.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 02:03:53.866340 zscaler_pulumi_zpa-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-03-27 02:03:53.866340 zscaler_pulumi_zpa-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 02:03:53.866340 zscaler_pulumi_zpa-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 02:03:53.862340 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/
--rw-r--r--   0 runner    (1001) docker     (127)     8529 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   138501 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    65305 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/application_segment.py
--rw-r--r--   0 runner    (1001) docker     (127)    66847 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/application_segment_browser_access.py
--rw-r--r--   0 runner    (1001) docker     (127)    69755 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/application_segment_inspection.py
--rw-r--r--   0 runner    (1001) docker     (127)    70525 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/application_segment_pra.py
--rw-r--r--   0 runner    (1001) docker     (127)    21010 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/application_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    22037 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/assistant_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)    62588 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/browser_access.py
--rw-r--r--   0 runner    (1001) docker     (127)    14673 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/browser_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    20976 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/cloud_browser_isolation_banner.py
--rw-r--r--   0 runner    (1001) docker     (127)     9156 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/cloud_browser_isolation_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    34370 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/cloud_browser_isolation_external_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 02:03:53.862340 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    62708 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/connector_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    24552 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_app_connector_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    20598 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_app_connector_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    19481 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_application_segment.py
--rw-r--r--   0 runner    (1001) docker     (127)    16535 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_application_segment_browser_access.py
--rw-r--r--   0 runner    (1001) docker     (127)    21823 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_application_segment_inspection.py
--rw-r--r--   0 runner    (1001) docker     (127)    19171 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_application_segment_pra.py
--rw-r--r--   0 runner    (1001) docker     (127)     9668 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_application_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_assistant_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11668 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_ba_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_cloud_browser_isolation_banner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_cloud_browser_isolation_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8498 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_cloud_browser_isolation_external_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_cloud_browser_isolation_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_cloud_browser_isolation_zpa_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     9771 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_cloud_connector_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_customer_version_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    15072 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_enrollment_cert.py
--rw-r--r--   0 runner    (1001) docker     (127)    19313 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_id_p_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_inspection_all_predefined_controls.py
--rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_inspection_custom_controls.py
--rw-r--r--   0 runner    (1001) docker     (127)    13238 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_inspection_predefined_controls.py
--rw-r--r--   0 runner    (1001) docker     (127)    11434 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_inspection_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     7419 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_isolation_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_lss_client_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_lss_config_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_lss_log_type_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_lss_status_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9055 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_machine_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     9298 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_microtenant.py
--rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_policy_client_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_policy_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)    12903 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_policy_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_posture_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    15340 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_provisioning_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_saml_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)    11992 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_scim_attribute_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_scim_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    10154 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_segment_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_server_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    23981 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_service_edge_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    15693 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_service_edge_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_trusted_network.py
--rw-r--r--   0 runner    (1001) docker     (127)    34848 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/inspection_custom_controls.py
--rw-r--r--   0 runner    (1001) docker     (127)    32040 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/inspection_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    11625 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/lss_config_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    19759 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/microtenant.py
--rw-r--r--   0 runner    (1001) docker     (127)   291960 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    41336 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/policy_access_forwarding_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    41336 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/policy_access_inspection_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    41300 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/policy_access_isolation_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/policy_access_reorder_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    57011 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/policy_access_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    41228 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/policy_access_time_out_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9009 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    35233 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/provisioning_key.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    23646 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/segment_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    33326 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/server_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    52563 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/service_edge_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 02:03:53.862340 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-27 02:03:53.000000 zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 03:20:54.267030 zscaler_pulumi_zpa-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-03-27 03:20:54.267030 zscaler_pulumi_zpa-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 03:20:54.267030 zscaler_pulumi_zpa-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 03:20:54.263030 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/
+-rw-r--r--   0 runner    (1001) docker     (127)     8529 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   138501 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65305 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/application_segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66847 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/application_segment_browser_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69755 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/application_segment_inspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70525 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/application_segment_pra.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21010 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/application_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22037 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/assistant_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62588 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/browser_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14673 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/browser_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20976 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/cloud_browser_isolation_banner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9156 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/cloud_browser_isolation_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34370 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/cloud_browser_isolation_external_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 03:20:54.267030 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62708 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/connector_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24552 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_app_connector_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20598 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_app_connector_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19481 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_application_segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16535 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_application_segment_browser_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21823 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_application_segment_inspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19171 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_application_segment_pra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9668 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_application_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_assistant_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11668 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_ba_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_cloud_browser_isolation_banner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_cloud_browser_isolation_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8498 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_cloud_browser_isolation_external_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_cloud_browser_isolation_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_cloud_browser_isolation_zpa_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9771 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_cloud_connector_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_customer_version_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15072 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_enrollment_cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19313 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_id_p_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_inspection_all_predefined_controls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_inspection_custom_controls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13238 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_inspection_predefined_controls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11434 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_inspection_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7419 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_isolation_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_lss_client_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_lss_config_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_lss_log_type_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_lss_status_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9055 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_machine_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9298 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_microtenant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_policy_client_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_policy_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12903 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_policy_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_posture_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15340 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_provisioning_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_saml_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11992 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_scim_attribute_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_scim_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10154 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_segment_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_server_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23981 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_service_edge_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15693 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_service_edge_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_trusted_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34848 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/inspection_custom_controls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32040 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/inspection_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11625 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/lss_config_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19759 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/microtenant.py
+-rw-r--r--   0 runner    (1001) docker     (127)   291960 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41336 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/policy_access_forwarding_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41336 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/policy_access_inspection_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41300 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/policy_access_isolation_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/policy_access_reorder_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57011 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/policy_access_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41228 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/policy_access_time_out_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9009 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35233 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/provisioning_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    23646 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/segment_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33326 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/server_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52563 2024-03-27 03:20:53.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/service_edge_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 03:20:54.267030 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-03-27 03:20:54.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-03-27 03:20:54.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 03:20:54.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 03:20:54.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 03:20:54.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-27 03:20:54.000000 zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa.egg-info/top_level.txt
```

### Comparing `zscaler_pulumi_zpa-0.0.7/PKG-INFO` & `zscaler_pulumi_zpa-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zscaler_pulumi_zpa
-Version: 0.0.7
+Version: 0.0.9
 Summary: A Pulumi package for creating and managing Zscaler Private Access (ZPA) cloud resources.
 Home-page: https://www.zscaler.com
 License: MIT
 Project-URL: Repository, https://github.com/zscaler/pulumi-zpa
 Keywords: pulumi zpa zscaler category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `zscaler_pulumi_zpa-0.0.7/README.md` & `zscaler_pulumi_zpa-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/setup.py` & `zscaler_pulumi_zpa-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import errno
 import os
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.7"
+VERSION = "0.0.9"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "zpa Pulumi Package - Development Version"
```

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/__init__.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/__init__.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/_inputs.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/_inputs.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/_utilities.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/_utilities.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/application_segment.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/application_segment.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/application_segment_browser_access.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/application_segment_browser_access.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/application_segment_inspection.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/application_segment_inspection.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/application_segment_pra.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/application_segment_pra.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/application_server.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/application_server.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/assistant_schedule.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/assistant_schedule.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/browser_access.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/browser_access.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/browser_certificate.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/browser_certificate.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/cloud_browser_isolation_banner.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/cloud_browser_isolation_banner.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/cloud_browser_isolation_certificate.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/cloud_browser_isolation_certificate.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/cloud_browser_isolation_external_profile.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/cloud_browser_isolation_external_profile.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/config/vars.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/config/vars.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/connector_group.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/connector_group.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_app_connector_controller.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_app_connector_controller.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_app_connector_group.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_app_connector_group.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_application_segment.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_application_segment.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_application_segment_browser_access.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_application_segment_browser_access.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_application_segment_inspection.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_application_segment_inspection.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_application_segment_pra.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_application_segment_pra.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_application_server.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_application_server.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_assistant_schedule.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_assistant_schedule.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_ba_certificate.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_ba_certificate.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_cloud_browser_isolation_banner.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_cloud_browser_isolation_banner.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_cloud_browser_isolation_certificate.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_cloud_browser_isolation_certificate.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_cloud_browser_isolation_external_profile.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_cloud_browser_isolation_external_profile.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_cloud_browser_isolation_region.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_cloud_browser_isolation_region.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_cloud_browser_isolation_zpa_profile.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_cloud_browser_isolation_zpa_profile.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_cloud_connector_group.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_cloud_connector_group.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_customer_version_profile.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_customer_version_profile.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_enrollment_cert.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_enrollment_cert.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_id_p_controller.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_id_p_controller.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_inspection_all_predefined_controls.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_inspection_all_predefined_controls.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_inspection_custom_controls.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_inspection_custom_controls.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_inspection_predefined_controls.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_inspection_predefined_controls.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_inspection_profile.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_inspection_profile.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_isolation_profile.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_isolation_profile.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_lss_client_types.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_lss_client_types.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_lss_config_controller.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_lss_config_controller.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_lss_log_type_formats.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_lss_log_type_formats.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_lss_status_codes.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_lss_status_codes.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_machine_group.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_machine_group.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_microtenant.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_microtenant.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_policy_client_type.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_policy_client_type.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_policy_platform.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_policy_platform.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_policy_type.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_policy_type.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_posture_profile.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_posture_profile.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_provisioning_key.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_provisioning_key.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_saml_attribute.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_saml_attribute.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_scim_attribute_header.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_scim_attribute_header.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_scim_groups.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_scim_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_segment_group.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_segment_group.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_server_group.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_server_group.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_service_edge_controller.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_service_edge_controller.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_service_edge_group.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_service_edge_group.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/get_trusted_network.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/get_trusted_network.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/inspection_custom_controls.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/inspection_custom_controls.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/inspection_profile.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/inspection_profile.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/lss_config_controller.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/lss_config_controller.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/microtenant.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/microtenant.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/outputs.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/outputs.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/policy_access_forwarding_rule.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/policy_access_forwarding_rule.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/policy_access_inspection_rule.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/policy_access_inspection_rule.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/policy_access_isolation_rule.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/policy_access_isolation_rule.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/policy_access_reorder_rule.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/policy_access_reorder_rule.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/policy_access_rule.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/policy_access_rule.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/policy_access_time_out_rule.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/policy_access_time_out_rule.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/provider.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/provider.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/provisioning_key.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/provisioning_key.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/segment_group.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/segment_group.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/server_group.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/server_group.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa/service_edge_group.py` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa/service_edge_group.py`

 * *Files identical despite different names*

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa.egg-info/PKG-INFO` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zscaler-pulumi-zpa
-Version: 0.0.7
+Version: 0.0.9
 Summary: A Pulumi package for creating and managing Zscaler Private Access (ZPA) cloud resources.
 Home-page: https://www.zscaler.com
 License: MIT
 Project-URL: Repository, https://github.com/zscaler/pulumi-zpa
 Keywords: pulumi zpa zscaler category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `zscaler_pulumi_zpa-0.0.7/zscaler_pulumi_zpa.egg-info/SOURCES.txt` & `zscaler_pulumi_zpa-0.0.9/zscaler_pulumi_zpa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

