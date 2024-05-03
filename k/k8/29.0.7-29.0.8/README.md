# Comparing `tmp/k8-29.0.7.tar.gz` & `tmp/k8-29.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k8-29.0.7.tar", last modified: Tue Apr  9 14:41:07 2024, max compression
+gzip compressed data, was "k8-29.0.8.tar", last modified: Fri May  3 23:47:32 2024, max compression
```

## Comparing `k8-29.0.7.tar` & `k8-29.0.8.tar`

### file list

```diff
@@ -1,579 +1,579 @@
-drwxr-xr-x   0 nickc      (503) staff       (20)        0 2024-04-09 14:41:07.000985 k8-29.0.7/
--rw-r--r--   0 nickc      (503) staff       (20)     1068 2024-03-21 02:36:58.000000 k8-29.0.7/LICENSE
--rw-r--r--   0 nickc      (503) staff       (20)      631 2024-04-09 14:41:07.000469 k8-29.0.7/PKG-INFO
--rw-r--r--   0 nickc      (503) staff       (20)       55 2024-03-21 02:50:06.000000 k8-29.0.7/README.md
--rw-r--r--   0 nickc      (503) staff       (20)      765 2024-04-09 14:40:34.000000 k8-29.0.7/pyproject.toml
--rw-r--r--   0 nickc      (503) staff       (20)       38 2024-04-09 14:41:07.001058 k8-29.0.7/setup.cfg
-drwxr-xr-x   0 nickc      (503) staff       (20)        0 2024-04-09 14:41:06.636794 k8-29.0.7/src/
-drwxr-xr-x   0 nickc      (503) staff       (20)        0 2024-04-09 14:41:06.996655 k8-29.0.7/src/k8/
--rw-r--r--   0 nickc      (503) staff       (20)        1 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/__init__.py
--rw-r--r--   0 nickc      (503) staff       (20)     3922 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/admissionregistration_v1_service_reference.py
--rw-r--r--   0 nickc      (503) staff       (20)     5802 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/admissionregistration_v1_webhook_client_config.py
--rw-r--r--   0 nickc      (503) staff       (20)     3895 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/apiextensions_v1_service_reference.py
--rw-r--r--   0 nickc      (503) staff       (20)     5743 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/apiextensions_v1_webhook_client_config.py
--rw-r--r--   0 nickc      (503) staff       (20)     3734 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/apiregistration_v1_service_reference.py
--rw-r--r--   0 nickc      (503) staff       (20)     5080 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/authentication_v1_token_request.py
--rw-r--r--   0 nickc      (503) staff       (20)     4714 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/core_v1_endpoint_port.py
--rw-r--r--   0 nickc      (503) staff       (20)     8384 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/core_v1_event.py
--rw-r--r--   0 nickc      (503) staff       (20)     4799 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/core_v1_event_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     3574 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/core_v1_event_series.py
--rw-r--r--   0 nickc      (503) staff       (20)     5204 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/discovery_v1_endpoint_port.py
--rw-r--r--   0 nickc      (503) staff       (20)     9299 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/events_v1_event.py
--rw-r--r--   0 nickc      (503) staff       (20)     4840 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/events_v1_event_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     3841 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/events_v1_event_series.py
--rw-r--r--   0 nickc      (503) staff       (20)     4590 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/flowcontrol_v1_subject.py
--rw-r--r--   0 nickc      (503) staff       (20)     4255 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/rbac_v1_subject.py
--rw-r--r--   0 nickc      (503) staff       (20)     3691 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/storage_v1_token_request.py
--rw-r--r--   0 nickc      (503) staff       (20)     4457 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_affinity.py
--rw-r--r--   0 nickc      (503) staff       (20)     4019 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_aggregation_rule.py
--rw-r--r--   0 nickc      (503) staff       (20)     6667 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_api_group.py
--rw-r--r--   0 nickc      (503) staff       (20)     4500 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_api_group_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     5927 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_api_resource.py
--rw-r--r--   0 nickc      (503) staff       (20)     4885 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_api_resource_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     5068 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_api_service.py
--rw-r--r--   0 nickc      (503) staff       (20)     4074 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_api_service_condition.py
--rw-r--r--   0 nickc      (503) staff       (20)     4840 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_api_service_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     7249 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_api_service_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     3746 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_api_service_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     5607 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_api_versions.py
--rw-r--r--   0 nickc      (503) staff       (20)     3387 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_attached_volume.py
--rw-r--r--   0 nickc      (503) staff       (20)     4846 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_aws_elastic_block_store_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     4616 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_azure_disk_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     4109 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_azure_file_persistent_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     3771 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_azure_file_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     4748 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_binding.py
--rw-r--r--   0 nickc      (503) staff       (20)     3732 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_bound_object_reference.py
--rw-r--r--   0 nickc      (503) staff       (20)     3347 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_capabilities.py
--rw-r--r--   0 nickc      (503) staff       (20)     5030 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_ceph_fs_persistent_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     5021 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_ceph_fs_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     5815 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_certificate_signing_request.py
--rw-r--r--   0 nickc      (503) staff       (20)     5217 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_certificate_signing_request_condition.py
--rw-r--r--   0 nickc      (503) staff       (20)     5008 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_certificate_signing_request_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     9097 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_certificate_signing_request_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     6079 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_certificate_signing_request_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     4698 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_cinder_persistent_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     4683 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_cinder_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     4300 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_claim_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     3470 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_client_ip_config.py
--rw-r--r--   0 nickc      (503) staff       (20)     5476 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_cluster_role.py
--rw-r--r--   0 nickc      (503) staff       (20)     5424 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_cluster_role_binding.py
--rw-r--r--   0 nickc      (503) staff       (20)     4918 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_cluster_role_binding_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     4847 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_cluster_role_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     4799 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_cluster_trust_bundle_projection.py
--rw-r--r--   0 nickc      (503) staff       (20)     3842 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_component_condition.py
--rw-r--r--   0 nickc      (503) staff       (20)     5032 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_component_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     4958 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_component_status_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     4939 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_condition.py
--rw-r--r--   0 nickc      (503) staff       (20)     5716 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_config_map.py
--rw-r--r--   0 nickc      (503) staff       (20)     3638 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_config_map_env_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     3595 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_config_map_key_selector.py
--rw-r--r--   0 nickc      (503) staff       (20)     4854 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_config_map_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     4536 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_config_map_node_config_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     4857 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_config_map_projection.py
--rw-r--r--   0 nickc      (503) staff       (20)     5472 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_config_map_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)    17018 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_container.py
--rw-r--r--   0 nickc      (503) staff       (20)     3512 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_container_image.py
--rw-r--r--   0 nickc      (503) staff       (20)     4343 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_container_port.py
--rw-r--r--   0 nickc      (503) staff       (20)     3601 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_container_resize_policy.py
--rw-r--r--   0 nickc      (503) staff       (20)     4443 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_container_state.py
--rw-r--r--   0 nickc      (503) staff       (20)     3318 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_container_state_running.py
--rw-r--r--   0 nickc      (503) staff       (20)     4486 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_container_state_terminated.py
--rw-r--r--   0 nickc      (503) staff       (20)     3447 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_container_state_waiting.py
--rw-r--r--   0 nickc      (503) staff       (20)     7439 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_container_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     5298 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_controller_revision.py
--rw-r--r--   0 nickc      (503) staff       (20)     4943 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_controller_revision_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     5000 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_cron_job.py
--rw-r--r--   0 nickc      (503) staff       (20)     4812 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_cron_job_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     6505 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_cron_job_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     4237 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_cron_job_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     3802 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_cross_version_object_reference.py
--rw-r--r--   0 nickc      (503) staff       (20)     4902 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_csi_driver.py
--rw-r--r--   0 nickc      (503) staff       (20)     4836 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_csi_driver_list.py
--rw-r--r--   0 nickc      (503) staff       (20)    11067 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_csi_driver_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     5144 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_csi_node.py
--rw-r--r--   0 nickc      (503) staff       (20)     5298 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_csi_node_driver.py
--rw-r--r--   0 nickc      (503) staff       (20)     4816 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_csi_node_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     3775 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_csi_node_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     7015 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_csi_persistent_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     7650 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_csi_storage_capacity.py
--rw-r--r--   0 nickc      (503) staff       (20)     4936 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_csi_storage_capacity_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     4832 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_csi_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     4768 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_custom_resource_column_definition.py
--rw-r--r--   0 nickc      (503) staff       (20)     4062 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_custom_resource_conversion.py
--rw-r--r--   0 nickc      (503) staff       (20)     5262 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_custom_resource_definition.py
--rw-r--r--   0 nickc      (503) staff       (20)     4229 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_custom_resource_definition_condition.py
--rw-r--r--   0 nickc      (503) staff       (20)     4990 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_custom_resource_definition_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     4909 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_custom_resource_definition_names.py
--rw-r--r--   0 nickc      (503) staff       (20)     6630 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_custom_resource_definition_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     5068 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_custom_resource_definition_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     6678 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_custom_resource_definition_version.py
--rw-r--r--   0 nickc      (503) staff       (20)     5065 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_custom_resource_subresource_scale.py
--rw-r--r--   0 nickc      (503) staff       (20)     4015 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_custom_resource_subresources.py
--rw-r--r--   0 nickc      (503) staff       (20)     3625 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_custom_resource_validation.py
--rw-r--r--   0 nickc      (503) staff       (20)     3215 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_daemon_endpoint.py
--rw-r--r--   0 nickc      (503) staff       (20)     5019 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_daemon_set.py
--rw-r--r--   0 nickc      (503) staff       (20)     4023 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_daemon_set_condition.py
--rw-r--r--   0 nickc      (503) staff       (20)     4822 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_daemon_set_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     5116 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_daemon_set_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     6779 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_daemon_set_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     3856 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_daemon_set_update_strategy.py
--rw-r--r--   0 nickc      (503) staff       (20)     6420 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_delete_options.py
--rw-r--r--   0 nickc      (503) staff       (20)     5037 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_deployment.py
--rw-r--r--   0 nickc      (503) staff       (20)     4248 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_deployment_condition.py
--rw-r--r--   0 nickc      (503) staff       (20)     4834 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_deployment_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     6021 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_deployment_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     5951 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_deployment_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     3821 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_deployment_strategy.py
--rw-r--r--   0 nickc      (503) staff       (20)     3818 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_downward_api_projection.py
--rw-r--r--   0 nickc      (503) staff       (20)     4946 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_downward_api_volume_file.py
--rw-r--r--   0 nickc      (503) staff       (20)     4512 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_downward_api_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     4117 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_empty_dir_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     6309 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_endpoint.py
--rw-r--r--   0 nickc      (503) staff       (20)     4169 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_endpoint_address.py
--rw-r--r--   0 nickc      (503) staff       (20)     4383 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_endpoint_conditions.py
--rw-r--r--   0 nickc      (503) staff       (20)     3766 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_endpoint_hints.py
--rw-r--r--   0 nickc      (503) staff       (20)     6493 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_endpoint_slice.py
--rw-r--r--   0 nickc      (503) staff       (20)     4873 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_endpoint_slice_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     5703 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_endpoint_subset.py
--rw-r--r--   0 nickc      (503) staff       (20)     5712 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_endpoints.py
--rw-r--r--   0 nickc      (503) staff       (20)     4809 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_endpoints_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     4219 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_env_from_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     4264 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_env_var.py
--rw-r--r--   0 nickc      (503) staff       (20)     5075 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_env_var_source.py
--rw-r--r--   0 nickc      (503) staff       (20)    16828 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_ephemeral_container.py
--rw-r--r--   0 nickc      (503) staff       (20)     3710 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_ephemeral_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     3390 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_event_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     4914 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_eviction.py
--rw-r--r--   0 nickc      (503) staff       (20)     3586 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_exec_action.py
--rw-r--r--   0 nickc      (503) staff       (20)     4836 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_exempt_priority_level_configuration.py
--rw-r--r--   0 nickc      (503) staff       (20)     3312 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_external_documentation.py
--rw-r--r--   0 nickc      (503) staff       (20)     4444 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_fc_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     4593 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_flex_persistent_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     4557 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_flex_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     3766 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_flocker_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     3309 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_flow_distinguisher_method.py
--rw-r--r--   0 nickc      (503) staff       (20)     5207 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_flow_schema.py
--rw-r--r--   0 nickc      (503) staff       (20)     4183 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_flow_schema_condition.py
--rw-r--r--   0 nickc      (503) staff       (20)     4842 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_flow_schema_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     5732 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_flow_schema_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     3766 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_flow_schema_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     3192 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_for_zone.py
--rw-r--r--   0 nickc      (503) staff       (20)     4941 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_gce_persistent_disk_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     4118 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_git_repo_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     4439 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_glusterfs_persistent_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     3971 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_glusterfs_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     3359 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_group_subject.py
--rw-r--r--   0 nickc      (503) staff       (20)     3615 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_group_version_for_discovery.py
--rw-r--r--   0 nickc      (503) staff       (20)     3531 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_grpc_action.py
--rw-r--r--   0 nickc      (503) staff       (20)     5165 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_horizontal_pod_autoscaler.py
--rw-r--r--   0 nickc      (503) staff       (20)     4951 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_horizontal_pod_autoscaler_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     4842 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_horizontal_pod_autoscaler_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     4707 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_horizontal_pod_autoscaler_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     3430 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_host_alias.py
--rw-r--r--   0 nickc      (503) staff       (20)     3203 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_host_ip.py
--rw-r--r--   0 nickc      (503) staff       (20)     3646 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_host_path_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     4436 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_http_get_action.py
--rw-r--r--   0 nickc      (503) staff       (20)     3388 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_http_header.py
--rw-r--r--   0 nickc      (503) staff       (20)     4901 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_http_ingress_path.py
--rw-r--r--   0 nickc      (503) staff       (20)     3914 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_http_ingress_rule_value.py
--rw-r--r--   0 nickc      (503) staff       (20)     5196 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_ingress.py
--rw-r--r--   0 nickc      (503) staff       (20)     3921 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_ingress_backend.py
--rw-r--r--   0 nickc      (503) staff       (20)     4977 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_ingress_class.py
--rw-r--r--   0 nickc      (503) staff       (20)     4863 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_ingress_class_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     4359 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_ingress_class_parameters_reference.py
--rw-r--r--   0 nickc      (503) staff       (20)     4109 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_ingress_class_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     4808 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_ingress_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     4150 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_ingress_load_balancer_ingress.py
--rw-r--r--   0 nickc      (503) staff       (20)     3807 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_ingress_load_balancer_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     3881 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_ingress_port_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     5110 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_ingress_rule.py
--rw-r--r--   0 nickc      (503) staff       (20)     3670 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_ingress_service_backend.py
--rw-r--r--   0 nickc      (503) staff       (20)     6008 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_ingress_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     3578 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_ingress_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     3947 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_ingress_tls.py
--rw-r--r--   0 nickc      (503) staff       (20)     3764 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_ip_block.py
--rw-r--r--   0 nickc      (503) staff       (20)     6364 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_iscsi_persistent_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     6339 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_iscsi_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     4945 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_job.py
--rw-r--r--   0 nickc      (503) staff       (20)     4199 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_job_condition.py
--rw-r--r--   0 nickc      (503) staff       (20)     4770 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_job_list.py
--rw-r--r--   0 nickc      (503) staff       (20)    11957 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_job_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     8149 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_job_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     3791 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_job_template_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)    19861 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_json_schema_props.py
--rw-r--r--   0 nickc      (503) staff       (20)     3954 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_key_to_path.py
--rw-r--r--   0 nickc      (503) staff       (20)     4475 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_label_selector.py
--rw-r--r--   0 nickc      (503) staff       (20)     3888 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_label_selector_requirement.py
--rw-r--r--   0 nickc      (503) staff       (20)     4586 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_lease.py
--rw-r--r--   0 nickc      (503) staff       (20)     4797 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_lease_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     4412 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_lease_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     4114 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_lifecycle.py
--rw-r--r--   0 nickc      (503) staff       (20)     4766 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_lifecycle_handler.py
--rw-r--r--   0 nickc      (503) staff       (20)     4671 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_limit_range.py
--rw-r--r--   0 nickc      (503) staff       (20)     4565 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_limit_range_item.py
--rw-r--r--   0 nickc      (503) staff       (20)     4935 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_limit_range_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     3690 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_limit_range_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     3867 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_limit_response.py
--rw-r--r--   0 nickc      (503) staff       (20)     6479 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_limited_priority_level_configuration.py
--rw-r--r--   0 nickc      (503) staff       (20)     5611 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_list_meta.py
--rw-r--r--   0 nickc      (503) staff       (20)     4894 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_load_balancer_ingress.py
--rw-r--r--   0 nickc      (503) staff       (20)     3823 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_load_balancer_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     3378 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_local_object_reference.py
--rw-r--r--   0 nickc      (503) staff       (20)     5305 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_local_subject_access_review.py
--rw-r--r--   0 nickc      (503) staff       (20)     3702 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_local_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     5604 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_managed_fields_entry.py
--rw-r--r--   0 nickc      (503) staff       (20)     4751 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_match_condition.py
--rw-r--r--   0 nickc      (503) staff       (20)     4223 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_modify_volume_status.py
--rw-r--r--   0 nickc      (503) staff       (20)    11820 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_mutating_webhook.py
--rw-r--r--   0 nickc      (503) staff       (20)     5086 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_mutating_webhook_configuration.py
--rw-r--r--   0 nickc      (503) staff       (20)     5001 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_mutating_webhook_configuration_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     5039 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_namespace.py
--rw-r--r--   0 nickc      (503) staff       (20)     3955 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_namespace_condition.py
--rw-r--r--   0 nickc      (503) staff       (20)     4932 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_namespace_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     3390 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_namespace_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     4041 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_namespace_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     4686 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_network_policy.py
--rw-r--r--   0 nickc      (503) staff       (20)     5124 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_network_policy_egress_rule.py
--rw-r--r--   0 nickc      (503) staff       (20)     5181 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_network_policy_ingress_rule.py
--rw-r--r--   0 nickc      (503) staff       (20)     4870 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_network_policy_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     4441 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_network_policy_peer.py
--rw-r--r--   0 nickc      (503) staff       (20)     4137 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_network_policy_port.py
--rw-r--r--   0 nickc      (503) staff       (20)     6764 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_network_policy_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     3895 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_nfs_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     5012 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_node.py
--rw-r--r--   0 nickc      (503) staff       (20)     3326 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_node_address.py
--rw-r--r--   0 nickc      (503) staff       (20)     5543 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_node_affinity.py
--rw-r--r--   0 nickc      (503) staff       (20)     4225 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_node_condition.py
--rw-r--r--   0 nickc      (503) staff       (20)     3653 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_node_config_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     5431 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_node_config_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     3594 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_node_daemon_endpoints.py
--rw-r--r--   0 nickc      (503) staff       (20)     4811 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_node_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     3933 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_node_selector.py
--rw-r--r--   0 nickc      (503) staff       (20)     3982 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_node_selector_requirement.py
--rw-r--r--   0 nickc      (503) staff       (20)     4629 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_node_selector_term.py
--rw-r--r--   0 nickc      (503) staff       (20)     5541 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_node_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     8764 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_node_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     5390 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_node_system_info.py
--rw-r--r--   0 nickc      (503) staff       (20)     3456 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_non_resource_attributes.py
--rw-r--r--   0 nickc      (503) staff       (20)     4137 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_non_resource_policy_rule.py
--rw-r--r--   0 nickc      (503) staff       (20)     3667 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_non_resource_rule.py
--rw-r--r--   0 nickc      (503) staff       (20)     3522 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_object_field_selector.py
--rw-r--r--   0 nickc      (503) staff       (20)    13308 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_object_meta.py
--rw-r--r--   0 nickc      (503) staff       (20)     5340 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_object_reference.py
--rw-r--r--   0 nickc      (503) staff       (20)     3322 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_overhead.py
--rw-r--r--   0 nickc      (503) staff       (20)     4886 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_owner_reference.py
--rw-r--r--   0 nickc      (503) staff       (20)     5218 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_persistent_volume.py
--rw-r--r--   0 nickc      (503) staff       (20)     5176 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_persistent_volume_claim.py
--rw-r--r--   0 nickc      (503) staff       (20)     4356 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_persistent_volume_claim_condition.py
--rw-r--r--   0 nickc      (503) staff       (20)     5048 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_persistent_volume_claim_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     7476 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_persistent_volume_claim_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     9690 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_persistent_volume_claim_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     3924 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_persistent_volume_claim_template.py
--rw-r--r--   0 nickc      (503) staff       (20)     3923 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_persistent_volume_claim_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     4973 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_persistent_volume_list.py
--rw-r--r--   0 nickc      (503) staff       (20)    17377 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_persistent_volume_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     4360 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_persistent_volume_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     3626 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_photon_persistent_disk_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     5015 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_pod.py
--rw-r--r--   0 nickc      (503) staff       (20)     6237 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_pod_affinity.py
--rw-r--r--   0 nickc      (503) staff       (20)     6993 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_pod_affinity_term.py
--rw-r--r--   0 nickc      (503) staff       (20)     6279 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_pod_anti_affinity.py
--rw-r--r--   0 nickc      (503) staff       (20)     4432 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_pod_condition.py
--rw-r--r--   0 nickc      (503) staff       (20)     5180 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_pod_disruption_budget.py
--rw-r--r--   0 nickc      (503) staff       (20)     4929 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_pod_disruption_budget_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     5982 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_pod_disruption_budget_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     6871 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_pod_disruption_budget_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     4532 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_pod_dns_config.py
--rw-r--r--   0 nickc      (503) staff       (20)     3298 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_pod_dns_config_option.py
--rw-r--r--   0 nickc      (503) staff       (20)     3974 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_pod_failure_policy.py
--rw-r--r--   0 nickc      (503) staff       (20)     5275 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_pod_failure_policy_on_exit_codes_requirement.py
--rw-r--r--   0 nickc      (503) staff       (20)     3664 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_pod_failure_policy_on_pod_conditions_pattern.py
--rw-r--r--   0 nickc      (503) staff       (20)     5675 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_pod_failure_policy_rule.py
--rw-r--r--   0 nickc      (503) staff       (20)     3197 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_pod_ip.py
--rw-r--r--   0 nickc      (503) staff       (20)     4846 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_pod_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     3477 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_pod_os.py
--rw-r--r--   0 nickc      (503) staff       (20)     3307 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_pod_readiness_gate.py
--rw-r--r--   0 nickc      (503) staff       (20)     3798 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_pod_resource_claim.py
--rw-r--r--   0 nickc      (503) staff       (20)     3929 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_pod_resource_claim_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     3254 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_pod_scheduling_gate.py
--rw-r--r--   0 nickc      (503) staff       (20)     9173 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_pod_security_context.py
--rw-r--r--   0 nickc      (503) staff       (20)    25854 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_pod_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)    13217 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_pod_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     4708 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_pod_template.py
--rw-r--r--   0 nickc      (503) staff       (20)     4832 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_pod_template_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     3791 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_pod_template_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     4925 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_policy_rule.py
--rw-r--r--   0 nickc      (503) staff       (20)     6040 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_policy_rules_with_subjects.py
--rw-r--r--   0 nickc      (503) staff       (20)     3870 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_port_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     3856 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_portworx_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     3461 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_preconditions.py
--rw-r--r--   0 nickc      (503) staff       (20)     3798 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_preferred_scheduling_term.py
--rw-r--r--   0 nickc      (503) staff       (20)     5797 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_priority_class.py
--rw-r--r--   0 nickc      (503) staff       (20)     4873 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_priority_class_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     5229 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_priority_level_configuration.py
--rw-r--r--   0 nickc      (503) staff       (20)     4249 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_priority_level_configuration_condition.py
--rw-r--r--   0 nickc      (503) staff       (20)     4994 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_priority_level_configuration_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     3352 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_priority_level_configuration_reference.py
--rw-r--r--   0 nickc      (503) staff       (20)     4645 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_priority_level_configuration_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     3904 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_priority_level_configuration_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     7406 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_probe.py
--rw-r--r--   0 nickc      (503) staff       (20)     4315 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_projected_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     4743 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_queuing_configuration.py
--rw-r--r--   0 nickc      (503) staff       (20)     4504 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_quobyte_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     5534 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_rbd_persistent_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     5525 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_rbd_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     5064 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_replica_set.py
--rw-r--r--   0 nickc      (503) staff       (20)     4035 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_replica_set_condition.py
--rw-r--r--   0 nickc      (503) staff       (20)     4919 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_replica_set_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     4625 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_replica_set_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     5213 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_replica_set_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     5175 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_replication_controller.py
--rw-r--r--   0 nickc      (503) staff       (20)     4101 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_replication_controller_condition.py
--rw-r--r--   0 nickc      (503) staff       (20)     5031 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_replication_controller_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     4857 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_replication_controller_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     5332 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_replication_controller_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     4850 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_resource_attributes.py
--rw-r--r--   0 nickc      (503) staff       (20)     3312 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_resource_claim.py
--rw-r--r--   0 nickc      (503) staff       (20)     3693 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_resource_field_selector.py
--rw-r--r--   0 nickc      (503) staff       (20)     5527 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_resource_policy_rule.py
--rw-r--r--   0 nickc      (503) staff       (20)     5078 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_resource_quota.py
--rw-r--r--   0 nickc      (503) staff       (20)     4946 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_resource_quota_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     4081 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_resource_quota_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     3563 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_resource_quota_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     4681 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_resource_requirements.py
--rw-r--r--   0 nickc      (503) staff       (20)     4431 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_resource_rule.py
--rw-r--r--   0 nickc      (503) staff       (20)     4913 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_role.py
--rw-r--r--   0 nickc      (503) staff       (20)     5555 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_role_binding.py
--rw-r--r--   0 nickc      (503) staff       (20)     4847 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_role_binding_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     4776 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_role_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     3500 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_role_ref.py
--rw-r--r--   0 nickc      (503) staff       (20)     5491 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_rolling_update_daemon_set.py
--rw-r--r--   0 nickc      (503) staff       (20)     4723 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_rolling_update_deployment.py
--rw-r--r--   0 nickc      (503) staff       (20)     4355 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_rolling_update_stateful_set_strategy.py
--rw-r--r--   0 nickc      (503) staff       (20)     5314 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_rule_with_operations.py
--rw-r--r--   0 nickc      (503) staff       (20)     6129 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_runtime_class.py
--rw-r--r--   0 nickc      (503) staff       (20)     4861 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_runtime_class_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     4968 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_scale.py
--rw-r--r--   0 nickc      (503) staff       (20)     5760 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_scale_io_persistent_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     5732 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_scale_io_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     3259 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_scale_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     3737 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_scale_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     4369 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_scheduling.py
--rw-r--r--   0 nickc      (503) staff       (20)     3951 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_scope_selector.py
--rw-r--r--   0 nickc      (503) staff       (20)     3964 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_scoped_resource_selector_requirement.py
--rw-r--r--   0 nickc      (503) staff       (20)     3773 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_se_linux_options.py
--rw-r--r--   0 nickc      (503) staff       (20)     3964 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_seccomp_profile.py
--rw-r--r--   0 nickc      (503) staff       (20)     5951 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_secret.py
--rw-r--r--   0 nickc      (503) staff       (20)     3617 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_secret_env_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     3644 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_secret_key_selector.py
--rw-r--r--   0 nickc      (503) staff       (20)     4866 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_secret_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     4756 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_secret_projection.py
--rw-r--r--   0 nickc      (503) staff       (20)     3515 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_secret_reference.py
--rw-r--r--   0 nickc      (503) staff       (20)     5443 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_secret_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     8498 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_security_context.py
--rw-r--r--   0 nickc      (503) staff       (20)     5336 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_self_subject_access_review.py
--rw-r--r--   0 nickc      (503) staff       (20)     4352 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_self_subject_access_review_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     5001 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_self_subject_review.py
--rw-r--r--   0 nickc      (503) staff       (20)     3522 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_self_subject_review_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     5725 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_self_subject_rules_review.py
--rw-r--r--   0 nickc      (503) staff       (20)     3312 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_self_subject_rules_review_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     3697 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_server_address_by_client_cidr.py
--rw-r--r--   0 nickc      (503) staff       (20)     5171 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_service.py
--rw-r--r--   0 nickc      (503) staff       (20)     7119 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_service_account.py
--rw-r--r--   0 nickc      (503) staff       (20)     4963 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_service_account_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     3488 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_service_account_subject.py
--rw-r--r--   0 nickc      (503) staff       (20)     4451 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_service_account_token_projection.py
--rw-r--r--   0 nickc      (503) staff       (20)     3545 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_service_backend_port.py
--rw-r--r--   0 nickc      (503) staff       (20)     4793 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_service_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     6301 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_service_port.py
--rw-r--r--   0 nickc      (503) staff       (20)    18983 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_service_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     4158 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_service_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     3533 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_session_affinity_config.py
--rw-r--r--   0 nickc      (503) staff       (20)     3186 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_sleep_action.py
--rw-r--r--   0 nickc      (503) staff       (20)     5276 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_stateful_set.py
--rw-r--r--   0 nickc      (503) staff       (20)     4035 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_stateful_set_condition.py
--rw-r--r--   0 nickc      (503) staff       (20)     4852 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_stateful_set_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     3698 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_stateful_set_ordinals.py
--rw-r--r--   0 nickc      (503) staff       (20)     4143 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_stateful_set_persistent_volume_claim_retention_policy.py
--rw-r--r--   0 nickc      (503) staff       (20)     9277 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_stateful_set_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     6573 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_stateful_set_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     4011 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_stateful_set_update_strategy.py
--rw-r--r--   0 nickc      (503) staff       (20)     5646 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     4137 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_status_cause.py
--rw-r--r--   0 nickc      (503) staff       (20)     5578 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_status_details.py
--rw-r--r--   0 nickc      (503) staff       (20)     7306 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_storage_class.py
--rw-r--r--   0 nickc      (503) staff       (20)     4863 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_storage_class_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     5041 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_storage_os_persistent_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     5032 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_storage_os_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     5139 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_subject_access_review.py
--rw-r--r--   0 nickc      (503) staff       (20)     5208 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_subject_access_review_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     4311 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_subject_access_review_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     5804 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_subject_rules_review_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     3263 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_sysctl.py
--rw-r--r--   0 nickc      (503) staff       (20)     3903 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_taint.py
--rw-r--r--   0 nickc      (503) staff       (20)     3470 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_tcp_socket_action.py
--rw-r--r--   0 nickc      (503) staff       (20)     4504 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_token_request_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     3477 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_token_request_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     5136 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_token_review.py
--rw-r--r--   0 nickc      (503) staff       (20)     3710 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_token_review_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     4587 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_token_review_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     4850 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_toleration.py
--rw-r--r--   0 nickc      (503) staff       (20)     3525 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_topology_selector_label_requirement.py
--rw-r--r--   0 nickc      (503) staff       (20)     4172 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_topology_selector_term.py
--rw-r--r--   0 nickc      (503) staff       (20)    10308 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_topology_spread_constraint.py
--rw-r--r--   0 nickc      (503) staff       (20)     3787 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_typed_local_object_reference.py
--rw-r--r--   0 nickc      (503) staff       (20)     4183 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_typed_object_reference.py
--rw-r--r--   0 nickc      (503) staff       (20)     3500 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_uncounted_terminated_pods.py
--rw-r--r--   0 nickc      (503) staff       (20)     3911 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_user_info.py
--rw-r--r--   0 nickc      (503) staff       (20)     3231 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_user_subject.py
--rw-r--r--   0 nickc      (503) staff       (20)    10621 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_validating_webhook.py
--rw-r--r--   0 nickc      (503) staff       (20)     5107 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_validating_webhook_configuration.py
--rw-r--r--   0 nickc      (503) staff       (20)     5021 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_validating_webhook_configuration_list.py
--rw-r--r--   0 nickc      (503) staff       (20)    11739 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_validation_rule.py
--rw-r--r--   0 nickc      (503) staff       (20)    16512 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_volume.py
--rw-r--r--   0 nickc      (503) staff       (20)     5175 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_volume_attachment.py
--rw-r--r--   0 nickc      (503) staff       (20)     4907 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_volume_attachment_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     4089 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_volume_attachment_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     3912 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_volume_attachment_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     4727 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_volume_attachment_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     3445 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_volume_device.py
--rw-r--r--   0 nickc      (503) staff       (20)     3548 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_volume_error.py
--rw-r--r--   0 nickc      (503) staff       (20)     4742 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_volume_mount.py
--rw-r--r--   0 nickc      (503) staff       (20)     3493 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_volume_node_affinity.py
--rw-r--r--   0 nickc      (503) staff       (20)     3619 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_volume_node_resources.py
--rw-r--r--   0 nickc      (503) staff       (20)     5614 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_volume_projection.py
--rw-r--r--   0 nickc      (503) staff       (20)     3898 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_volume_resource_requirements.py
--rw-r--r--   0 nickc      (503) staff       (20)     4187 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_vsphere_virtual_disk_volume_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     3465 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_watch_event.py
--rw-r--r--   0 nickc      (503) staff       (20)     4299 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_webhook_conversion.py
--rw-r--r--   0 nickc      (503) staff       (20)     3823 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_weighted_pod_affinity_term.py
--rw-r--r--   0 nickc      (503) staff       (20)     4794 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1_windows_security_context_options.py
--rw-r--r--   0 nickc      (503) staff       (20)     4813 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_audit_annotation.py
--rw-r--r--   0 nickc      (503) staff       (20)     5551 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_cluster_trust_bundle.py
--rw-r--r--   0 nickc      (503) staff       (20)     4980 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_cluster_trust_bundle_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     4813 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_cluster_trust_bundle_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     3707 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_expression_warning.py
--rw-r--r--   0 nickc      (503) staff       (20)     5224 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_ip_address.py
--rw-r--r--   0 nickc      (503) staff       (20)     4873 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_ip_address_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     3547 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_ip_address_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     4691 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_match_condition.py
--rw-r--r--   0 nickc      (503) staff       (20)     7181 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_match_resources.py
--rw-r--r--   0 nickc      (503) staff       (20)     5600 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_named_rule_with_operations.py
--rw-r--r--   0 nickc      (503) staff       (20)     3499 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_param_kind.py
--rw-r--r--   0 nickc      (503) staff       (20)     5261 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_param_ref.py
--rw-r--r--   0 nickc      (503) staff       (20)     3803 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_parent_reference.py
--rw-r--r--   0 nickc      (503) staff       (20)     5043 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_self_subject_review.py
--rw-r--r--   0 nickc      (503) staff       (20)     3540 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_self_subject_review_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     4267 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_server_storage_version.py
--rw-r--r--   0 nickc      (503) staff       (20)     5215 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_service_cidr.py
--rw-r--r--   0 nickc      (503) staff       (20)     4900 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_service_cidr_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     3469 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_service_cidr_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     3800 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_service_cidr_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     4874 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_storage_version.py
--rw-r--r--   0 nickc      (503) staff       (20)     4310 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_storage_version_condition.py
--rw-r--r--   0 nickc      (503) staff       (20)     4894 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_storage_version_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     5215 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_storage_version_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     3912 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_type_checking.py
--rw-r--r--   0 nickc      (503) staff       (20)     5347 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_validating_admission_policy.py
--rw-r--r--   0 nickc      (503) staff       (20)     5537 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_validating_admission_policy_binding.py
--rw-r--r--   0 nickc      (503) staff       (20)     5089 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_validating_admission_policy_binding_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     6871 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_validating_admission_policy_binding_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     5037 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_validating_admission_policy_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     9352 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_validating_admission_policy_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     4574 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_validating_admission_policy_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     8617 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_validation.py
--rw-r--r--   0 nickc      (503) staff       (20)     3714 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_variable.py
--rw-r--r--   0 nickc      (503) staff       (20)     5666 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_volume_attributes_class.py
--rw-r--r--   0 nickc      (503) staff       (20)     5008 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha1_volume_attributes_class_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     5284 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha2_allocation_result.py
--rw-r--r--   0 nickc      (503) staff       (20)     5374 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha2_pod_scheduling_context.py
--rw-r--r--   0 nickc      (503) staff       (20)     4992 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha2_pod_scheduling_context_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     3946 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha2_pod_scheduling_context_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     4073 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha2_pod_scheduling_context_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     5317 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha2_resource_claim.py
--rw-r--r--   0 nickc      (503) staff       (20)     4037 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha2_resource_claim_consumer_reference.py
--rw-r--r--   0 nickc      (503) staff       (20)     4906 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha2_resource_claim_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     3946 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha2_resource_claim_parameters_reference.py
--rw-r--r--   0 nickc      (503) staff       (20)     3796 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha2_resource_claim_scheduling_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     4295 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha2_resource_claim_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     5352 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha2_resource_claim_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     4758 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha2_resource_claim_template.py
--rw-r--r--   0 nickc      (503) staff       (20)     4989 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha2_resource_claim_template_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     3885 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha2_resource_claim_template_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     5822 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha2_resource_class.py
--rw-r--r--   0 nickc      (503) staff       (20)     4908 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha2_resource_class_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     4120 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha2_resource_class_parameters_reference.py
--rw-r--r--   0 nickc      (503) staff       (20)     4118 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1alpha2_resource_handle.py
--rw-r--r--   0 nickc      (503) staff       (20)     4810 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta1_audit_annotation.py
--rw-r--r--   0 nickc      (503) staff       (20)     3704 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta1_expression_warning.py
--rw-r--r--   0 nickc      (503) staff       (20)     4766 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta1_match_condition.py
--rw-r--r--   0 nickc      (503) staff       (20)     7172 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta1_match_resources.py
--rw-r--r--   0 nickc      (503) staff       (20)     5597 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta1_named_rule_with_operations.py
--rw-r--r--   0 nickc      (503) staff       (20)     3496 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta1_param_kind.py
--rw-r--r--   0 nickc      (503) staff       (20)     5476 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta1_param_ref.py
--rw-r--r--   0 nickc      (503) staff       (20)     5036 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta1_self_subject_review.py
--rw-r--r--   0 nickc      (503) staff       (20)     3537 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta1_self_subject_review_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     3905 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta1_type_checking.py
--rw-r--r--   0 nickc      (503) staff       (20)     5336 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta1_validating_admission_policy.py
--rw-r--r--   0 nickc      (503) staff       (20)     5530 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta1_validating_admission_policy_binding.py
--rw-r--r--   0 nickc      (503) staff       (20)     5082 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta1_validating_admission_policy_binding_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     6860 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta1_validating_admission_policy_binding_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     5030 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta1_validating_admission_policy_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     9325 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta1_validating_admission_policy_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     4570 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta1_validating_admission_policy_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     8614 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta1_validation.py
--rw-r--r--   0 nickc      (503) staff       (20)     3756 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta1_variable.py
--rw-r--r--   0 nickc      (503) staff       (20)     4851 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta3_exempt_priority_level_configuration.py
--rw-r--r--   0 nickc      (503) staff       (20)     3324 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta3_flow_distinguisher_method.py
--rw-r--r--   0 nickc      (503) staff       (20)     5262 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta3_flow_schema.py
--rw-r--r--   0 nickc      (503) staff       (20)     4198 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta3_flow_schema_condition.py
--rw-r--r--   0 nickc      (503) staff       (20)     4877 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta3_flow_schema_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     5807 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta3_flow_schema_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     3801 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta3_flow_schema_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     3374 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta3_group_subject.py
--rw-r--r--   0 nickc      (503) staff       (20)     3902 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta3_limit_response.py
--rw-r--r--   0 nickc      (503) staff       (20)     6366 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta3_limited_priority_level_configuration.py
--rw-r--r--   0 nickc      (503) staff       (20)     4152 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta3_non_resource_policy_rule.py
--rw-r--r--   0 nickc      (503) staff       (20)     6070 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta3_policy_rules_with_subjects.py
--rw-r--r--   0 nickc      (503) staff       (20)     5284 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta3_priority_level_configuration.py
--rw-r--r--   0 nickc      (503) staff       (20)     4264 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta3_priority_level_configuration_condition.py
--rw-r--r--   0 nickc      (503) staff       (20)     5029 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta3_priority_level_configuration_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     3367 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta3_priority_level_configuration_reference.py
--rw-r--r--   0 nickc      (503) staff       (20)     4700 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta3_priority_level_configuration_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     3939 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta3_priority_level_configuration_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     4758 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta3_queuing_configuration.py
--rw-r--r--   0 nickc      (503) staff       (20)     5542 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta3_resource_policy_rule.py
--rw-r--r--   0 nickc      (503) staff       (20)     3503 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta3_service_account_subject.py
--rw-r--r--   0 nickc      (503) staff       (20)     4632 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta3_subject.py
--rw-r--r--   0 nickc      (503) staff       (20)     3246 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v1beta3_user_subject.py
--rw-r--r--   0 nickc      (503) staff       (20)     4191 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v2_container_resource_metric_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     4132 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v2_container_resource_metric_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     3802 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v2_cross_version_object_reference.py
--rw-r--r--   0 nickc      (503) staff       (20)     3933 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v2_external_metric_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     3865 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v2_external_metric_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     5326 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v2_horizontal_pod_autoscaler.py
--rw-r--r--   0 nickc      (503) staff       (20)     4030 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v2_horizontal_pod_autoscaler_behavior.py
--rw-r--r--   0 nickc      (503) staff       (20)     4157 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v2_horizontal_pod_autoscaler_condition.py
--rw-r--r--   0 nickc      (503) staff       (20)     4984 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v2_horizontal_pod_autoscaler_list.py
--rw-r--r--   0 nickc      (503) staff       (20)     6024 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v2_horizontal_pod_autoscaler_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     5935 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v2_horizontal_pod_autoscaler_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     3749 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v2_hpa_scaling_policy.py
--rw-r--r--   0 nickc      (503) staff       (20)     5134 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v2_hpa_scaling_rules.py
--rw-r--r--   0 nickc      (503) staff       (20)     3610 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v2_metric_identifier.py
--rw-r--r--   0 nickc      (503) staff       (20)     5673 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v2_metric_spec.py
--rw-r--r--   0 nickc      (503) staff       (20)     5619 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v2_metric_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     4167 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v2_metric_target.py
--rw-r--r--   0 nickc      (503) staff       (20)     3929 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v2_metric_value_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     4392 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v2_object_metric_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     4427 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v2_object_metric_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     3942 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v2_pods_metric_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     3897 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v2_pods_metric_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     3974 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v2_resource_metric_source.py
--rw-r--r--   0 nickc      (503) staff       (20)     3893 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/v2_resource_metric_status.py
--rw-r--r--   0 nickc      (503) staff       (20)     3966 2024-04-09 14:39:37.000000 k8-29.0.7/src/k8/version_info.py
-drwxr-xr-x   0 nickc      (503) staff       (20)        0 2024-04-09 14:41:06.999821 k8-29.0.7/src/k8.egg-info/
--rw-r--r--   0 nickc      (503) staff       (20)      631 2024-04-09 14:41:06.000000 k8-29.0.7/src/k8.egg-info/PKG-INFO
--rw-r--r--   0 nickc      (503) staff       (20)    19965 2024-04-09 14:41:06.000000 k8-29.0.7/src/k8.egg-info/SOURCES.txt
--rw-r--r--   0 nickc      (503) staff       (20)        1 2024-04-09 14:41:06.000000 k8-29.0.7/src/k8.egg-info/dependency_links.txt
--rw-r--r--   0 nickc      (503) staff       (20)       26 2024-04-09 14:41:06.000000 k8-29.0.7/src/k8.egg-info/requires.txt
--rw-r--r--   0 nickc      (503) staff       (20)        3 2024-04-09 14:41:06.000000 k8-29.0.7/src/k8.egg-info/top_level.txt
+drwxr-xr-x   0 nickc      (503) staff       (20)        0 2024-05-03 23:47:32.671162 k8-29.0.8/
+-rw-r--r--   0 nickc      (503) staff       (20)     1068 2024-03-21 02:36:58.000000 k8-29.0.8/LICENSE
+-rw-r--r--   0 nickc      (503) staff       (20)      631 2024-05-03 23:47:32.670467 k8-29.0.8/PKG-INFO
+-rw-r--r--   0 nickc      (503) staff       (20)       55 2024-03-21 02:50:06.000000 k8-29.0.8/README.md
+-rw-r--r--   0 nickc      (503) staff       (20)      765 2024-05-03 23:40:14.000000 k8-29.0.8/pyproject.toml
+-rw-r--r--   0 nickc      (503) staff       (20)       38 2024-05-03 23:47:32.671249 k8-29.0.8/setup.cfg
+drwxr-xr-x   0 nickc      (503) staff       (20)        0 2024-05-03 23:47:32.375496 k8-29.0.8/src/
+drwxr-xr-x   0 nickc      (503) staff       (20)        0 2024-05-03 23:47:32.615681 k8-29.0.8/src/k8/
+-rw-r--r--   0 nickc      (503) staff       (20)        1 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/__init__.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3922 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/admissionregistration_v1_service_reference.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5802 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/admissionregistration_v1_webhook_client_config.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3895 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/apiextensions_v1_service_reference.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5743 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/apiextensions_v1_webhook_client_config.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3734 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/apiregistration_v1_service_reference.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5080 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/authentication_v1_token_request.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4714 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/core_v1_endpoint_port.py
+-rw-r--r--   0 nickc      (503) staff       (20)     8384 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/core_v1_event.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4799 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/core_v1_event_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3574 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/core_v1_event_series.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5204 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/discovery_v1_endpoint_port.py
+-rw-r--r--   0 nickc      (503) staff       (20)     9299 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/events_v1_event.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4840 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/events_v1_event_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3841 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/events_v1_event_series.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4590 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/flowcontrol_v1_subject.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4255 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/rbac_v1_subject.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3691 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/storage_v1_token_request.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4457 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_affinity.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4019 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_aggregation_rule.py
+-rw-r--r--   0 nickc      (503) staff       (20)     6667 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_api_group.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4500 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_api_group_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5927 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_api_resource.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4885 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_api_resource_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5068 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_api_service.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4074 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_api_service_condition.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4840 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_api_service_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     7249 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_api_service_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3746 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_api_service_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5607 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_api_versions.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3387 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_attached_volume.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4846 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_aws_elastic_block_store_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4616 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_azure_disk_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4109 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_azure_file_persistent_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3771 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_azure_file_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4748 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_binding.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3732 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_bound_object_reference.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3347 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_capabilities.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5030 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_ceph_fs_persistent_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5021 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_ceph_fs_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5815 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_certificate_signing_request.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5217 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_certificate_signing_request_condition.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5008 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_certificate_signing_request_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     9097 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_certificate_signing_request_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     6079 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_certificate_signing_request_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4698 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_cinder_persistent_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4683 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_cinder_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4300 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_claim_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3470 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_client_ip_config.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5476 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_cluster_role.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5424 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_cluster_role_binding.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4918 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_cluster_role_binding_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4847 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_cluster_role_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4799 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_cluster_trust_bundle_projection.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3842 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_component_condition.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5032 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_component_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4958 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_component_status_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4939 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_condition.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5716 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_config_map.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3638 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_config_map_env_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3595 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_config_map_key_selector.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4854 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_config_map_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4536 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_config_map_node_config_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4857 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_config_map_projection.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5472 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_config_map_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)    17018 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_container.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3512 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_container_image.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4343 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_container_port.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3601 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_container_resize_policy.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4443 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_container_state.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3318 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_container_state_running.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4486 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_container_state_terminated.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3447 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_container_state_waiting.py
+-rw-r--r--   0 nickc      (503) staff       (20)     7439 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_container_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5298 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_controller_revision.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4943 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_controller_revision_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5000 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_cron_job.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4812 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_cron_job_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     6505 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_cron_job_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4237 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_cron_job_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3802 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_cross_version_object_reference.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4902 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_csi_driver.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4836 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_csi_driver_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)    11067 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_csi_driver_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5144 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_csi_node.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5298 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_csi_node_driver.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4816 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_csi_node_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3775 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_csi_node_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     7015 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_csi_persistent_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     7650 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_csi_storage_capacity.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4936 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_csi_storage_capacity_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4832 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_csi_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4768 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_custom_resource_column_definition.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4062 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_custom_resource_conversion.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5262 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_custom_resource_definition.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4229 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_custom_resource_definition_condition.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4990 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_custom_resource_definition_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4909 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_custom_resource_definition_names.py
+-rw-r--r--   0 nickc      (503) staff       (20)     6630 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_custom_resource_definition_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5068 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_custom_resource_definition_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     6678 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_custom_resource_definition_version.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5065 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_custom_resource_subresource_scale.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4015 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_custom_resource_subresources.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3625 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_custom_resource_validation.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3215 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_daemon_endpoint.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5019 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_daemon_set.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4023 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_daemon_set_condition.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4822 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_daemon_set_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5116 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_daemon_set_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     6779 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_daemon_set_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3856 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_daemon_set_update_strategy.py
+-rw-r--r--   0 nickc      (503) staff       (20)     6420 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_delete_options.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5037 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_deployment.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4248 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_deployment_condition.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4834 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_deployment_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     6021 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_deployment_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5951 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_deployment_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3821 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_deployment_strategy.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3818 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_downward_api_projection.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4946 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_downward_api_volume_file.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4512 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_downward_api_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4117 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_empty_dir_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     6309 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_endpoint.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4169 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_endpoint_address.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4383 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_endpoint_conditions.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3766 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_endpoint_hints.py
+-rw-r--r--   0 nickc      (503) staff       (20)     6493 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_endpoint_slice.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4873 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_endpoint_slice_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5703 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_endpoint_subset.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5712 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_endpoints.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4809 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_endpoints_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4219 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_env_from_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4264 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_env_var.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5075 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_env_var_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)    16828 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_ephemeral_container.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3710 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_ephemeral_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3390 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_event_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4914 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_eviction.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3586 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_exec_action.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4836 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_exempt_priority_level_configuration.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3312 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_external_documentation.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4444 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_fc_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4593 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_flex_persistent_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4557 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_flex_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3766 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_flocker_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3309 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_flow_distinguisher_method.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5207 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_flow_schema.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4183 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_flow_schema_condition.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4842 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_flow_schema_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5732 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_flow_schema_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3766 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_flow_schema_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3192 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_for_zone.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4941 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_gce_persistent_disk_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4118 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_git_repo_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4439 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_glusterfs_persistent_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3971 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_glusterfs_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3359 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_group_subject.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3615 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_group_version_for_discovery.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3531 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_grpc_action.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5165 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_horizontal_pod_autoscaler.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4951 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_horizontal_pod_autoscaler_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4842 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_horizontal_pod_autoscaler_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4707 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_horizontal_pod_autoscaler_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3430 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_host_alias.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3203 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_host_ip.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3646 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_host_path_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4431 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_http_get_action.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3388 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_http_header.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4901 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_http_ingress_path.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3914 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_http_ingress_rule_value.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5196 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_ingress.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3921 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_ingress_backend.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4977 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_ingress_class.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4863 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_ingress_class_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4359 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_ingress_class_parameters_reference.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4109 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_ingress_class_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4808 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_ingress_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4150 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_ingress_load_balancer_ingress.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3807 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_ingress_load_balancer_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3881 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_ingress_port_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5110 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_ingress_rule.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3670 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_ingress_service_backend.py
+-rw-r--r--   0 nickc      (503) staff       (20)     6008 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_ingress_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3578 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_ingress_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3947 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_ingress_tls.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3764 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_ip_block.py
+-rw-r--r--   0 nickc      (503) staff       (20)     6364 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_iscsi_persistent_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     6339 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_iscsi_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4945 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_job.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4199 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_job_condition.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4770 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_job_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)    11957 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_job_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     8149 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_job_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3791 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_job_template_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)    19861 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_json_schema_props.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3954 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_key_to_path.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4475 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_label_selector.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3888 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_label_selector_requirement.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4586 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_lease.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4797 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_lease_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4412 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_lease_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4114 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_lifecycle.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4766 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_lifecycle_handler.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4671 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_limit_range.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4565 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_limit_range_item.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4935 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_limit_range_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3690 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_limit_range_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3867 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_limit_response.py
+-rw-r--r--   0 nickc      (503) staff       (20)     6479 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_limited_priority_level_configuration.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5611 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_list_meta.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4894 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_load_balancer_ingress.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3823 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_load_balancer_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3378 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_local_object_reference.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5305 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_local_subject_access_review.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3702 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_local_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5604 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_managed_fields_entry.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4751 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_match_condition.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4223 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_modify_volume_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)    11820 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_mutating_webhook.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5086 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_mutating_webhook_configuration.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5001 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_mutating_webhook_configuration_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5039 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_namespace.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3955 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_namespace_condition.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4932 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_namespace_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3390 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_namespace_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4041 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_namespace_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4686 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_network_policy.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5124 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_network_policy_egress_rule.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5181 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_network_policy_ingress_rule.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4870 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_network_policy_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4441 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_network_policy_peer.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4137 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_network_policy_port.py
+-rw-r--r--   0 nickc      (503) staff       (20)     6764 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_network_policy_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3895 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_nfs_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5012 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_node.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3326 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_node_address.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5543 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_node_affinity.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4225 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_node_condition.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3653 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_node_config_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5431 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_node_config_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3594 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_node_daemon_endpoints.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4811 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_node_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3933 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_node_selector.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3982 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_node_selector_requirement.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4629 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_node_selector_term.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5541 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_node_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     8764 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_node_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5390 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_node_system_info.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3456 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_non_resource_attributes.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4137 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_non_resource_policy_rule.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3667 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_non_resource_rule.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3522 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_object_field_selector.py
+-rw-r--r--   0 nickc      (503) staff       (20)    13308 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_object_meta.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5340 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_object_reference.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3322 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_overhead.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4886 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_owner_reference.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5218 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_persistent_volume.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5176 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_persistent_volume_claim.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4356 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_persistent_volume_claim_condition.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5048 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_persistent_volume_claim_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     7476 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_persistent_volume_claim_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     9690 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_persistent_volume_claim_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3924 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_persistent_volume_claim_template.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3923 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_persistent_volume_claim_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4973 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_persistent_volume_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)    17377 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_persistent_volume_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4360 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_persistent_volume_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3626 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_photon_persistent_disk_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5015 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_pod.py
+-rw-r--r--   0 nickc      (503) staff       (20)     6237 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_pod_affinity.py
+-rw-r--r--   0 nickc      (503) staff       (20)     6993 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_pod_affinity_term.py
+-rw-r--r--   0 nickc      (503) staff       (20)     6279 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_pod_anti_affinity.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4432 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_pod_condition.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5180 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_pod_disruption_budget.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4929 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_pod_disruption_budget_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5982 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_pod_disruption_budget_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     6871 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_pod_disruption_budget_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4532 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_pod_dns_config.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3298 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_pod_dns_config_option.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3974 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_pod_failure_policy.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5275 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_pod_failure_policy_on_exit_codes_requirement.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3664 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_pod_failure_policy_on_pod_conditions_pattern.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5675 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_pod_failure_policy_rule.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3197 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_pod_ip.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4846 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_pod_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3477 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_pod_os.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3307 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_pod_readiness_gate.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3798 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_pod_resource_claim.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3929 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_pod_resource_claim_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3254 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_pod_scheduling_gate.py
+-rw-r--r--   0 nickc      (503) staff       (20)     9173 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_pod_security_context.py
+-rw-r--r--   0 nickc      (503) staff       (20)    25854 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_pod_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)    13217 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_pod_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4708 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_pod_template.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4832 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_pod_template_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3791 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_pod_template_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4925 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_policy_rule.py
+-rw-r--r--   0 nickc      (503) staff       (20)     6040 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_policy_rules_with_subjects.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3870 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_port_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3856 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_portworx_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3461 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_preconditions.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3798 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_preferred_scheduling_term.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5797 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_priority_class.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4873 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_priority_class_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5229 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_priority_level_configuration.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4249 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_priority_level_configuration_condition.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4994 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_priority_level_configuration_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3352 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_priority_level_configuration_reference.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4645 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_priority_level_configuration_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3904 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_priority_level_configuration_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     7406 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_probe.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4315 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_projected_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4743 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_queuing_configuration.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4504 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_quobyte_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5534 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_rbd_persistent_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5525 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_rbd_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5064 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_replica_set.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4035 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_replica_set_condition.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4919 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_replica_set_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4625 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_replica_set_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5213 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_replica_set_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5175 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_replication_controller.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4101 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_replication_controller_condition.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5031 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_replication_controller_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4857 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_replication_controller_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5332 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_replication_controller_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4850 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_resource_attributes.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3312 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_resource_claim.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3693 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_resource_field_selector.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5527 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_resource_policy_rule.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5078 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_resource_quota.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4946 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_resource_quota_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4081 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_resource_quota_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3563 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_resource_quota_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4681 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_resource_requirements.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4431 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_resource_rule.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4913 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_role.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5555 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_role_binding.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4847 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_role_binding_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4776 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_role_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3500 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_role_ref.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5491 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_rolling_update_daemon_set.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4723 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_rolling_update_deployment.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4355 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_rolling_update_stateful_set_strategy.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5314 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_rule_with_operations.py
+-rw-r--r--   0 nickc      (503) staff       (20)     6129 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_runtime_class.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4861 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_runtime_class_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4968 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_scale.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5760 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_scale_io_persistent_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5732 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_scale_io_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3259 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_scale_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3737 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_scale_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4369 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_scheduling.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3951 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_scope_selector.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3964 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_scoped_resource_selector_requirement.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3773 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_se_linux_options.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3964 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_seccomp_profile.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5951 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_secret.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3617 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_secret_env_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3644 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_secret_key_selector.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4866 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_secret_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4756 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_secret_projection.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3515 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_secret_reference.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5443 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_secret_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     8498 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_security_context.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5336 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_self_subject_access_review.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4352 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_self_subject_access_review_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5001 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_self_subject_review.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3522 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_self_subject_review_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5725 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_self_subject_rules_review.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3312 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_self_subject_rules_review_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3697 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_server_address_by_client_cidr.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5171 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_service.py
+-rw-r--r--   0 nickc      (503) staff       (20)     7119 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_service_account.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4963 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_service_account_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3488 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_service_account_subject.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4451 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_service_account_token_projection.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3545 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_service_backend_port.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4793 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_service_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     6301 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_service_port.py
+-rw-r--r--   0 nickc      (503) staff       (20)    18983 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_service_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4158 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_service_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3533 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_session_affinity_config.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3186 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_sleep_action.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5276 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_stateful_set.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4035 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_stateful_set_condition.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4852 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_stateful_set_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3698 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_stateful_set_ordinals.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4143 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_stateful_set_persistent_volume_claim_retention_policy.py
+-rw-r--r--   0 nickc      (503) staff       (20)     9277 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_stateful_set_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     6573 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_stateful_set_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4011 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_stateful_set_update_strategy.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5646 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4137 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_status_cause.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5578 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_status_details.py
+-rw-r--r--   0 nickc      (503) staff       (20)     7306 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_storage_class.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4863 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_storage_class_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5041 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_storage_os_persistent_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5032 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_storage_os_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5139 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_subject_access_review.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5208 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_subject_access_review_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4311 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_subject_access_review_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5804 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_subject_rules_review_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3263 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_sysctl.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3903 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_taint.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3470 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_tcp_socket_action.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4504 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_token_request_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3477 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_token_request_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5136 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_token_review.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3710 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_token_review_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4587 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_token_review_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4850 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_toleration.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3525 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_topology_selector_label_requirement.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4172 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_topology_selector_term.py
+-rw-r--r--   0 nickc      (503) staff       (20)    10308 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_topology_spread_constraint.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3787 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_typed_local_object_reference.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4183 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_typed_object_reference.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3500 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_uncounted_terminated_pods.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3911 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_user_info.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3231 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_user_subject.py
+-rw-r--r--   0 nickc      (503) staff       (20)    10621 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_validating_webhook.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5107 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_validating_webhook_configuration.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5021 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_validating_webhook_configuration_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)    11739 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_validation_rule.py
+-rw-r--r--   0 nickc      (503) staff       (20)    16512 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_volume.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5175 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_volume_attachment.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4907 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_volume_attachment_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4089 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_volume_attachment_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3912 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_volume_attachment_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4727 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_volume_attachment_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3445 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_volume_device.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3548 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_volume_error.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4742 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_volume_mount.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3493 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_volume_node_affinity.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3619 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_volume_node_resources.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5614 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_volume_projection.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3898 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_volume_resource_requirements.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4187 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_vsphere_virtual_disk_volume_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3465 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_watch_event.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4299 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_webhook_conversion.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3823 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1_weighted_pod_affinity_term.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4794 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1_windows_security_context_options.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4813 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha1_audit_annotation.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5551 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha1_cluster_trust_bundle.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4980 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha1_cluster_trust_bundle_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4813 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha1_cluster_trust_bundle_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3707 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha1_expression_warning.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5224 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1alpha1_ip_address.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4873 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha1_ip_address_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3547 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha1_ip_address_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4691 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha1_match_condition.py
+-rw-r--r--   0 nickc      (503) staff       (20)     7181 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha1_match_resources.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5600 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha1_named_rule_with_operations.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3499 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha1_param_kind.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5261 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha1_param_ref.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3803 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1alpha1_parent_reference.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5043 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha1_self_subject_review.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3540 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha1_self_subject_review_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4267 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha1_server_storage_version.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5215 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha1_service_cidr.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4900 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha1_service_cidr_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3469 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha1_service_cidr_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3800 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha1_service_cidr_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4874 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha1_storage_version.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4310 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha1_storage_version_condition.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4894 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha1_storage_version_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5215 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha1_storage_version_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3912 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1alpha1_type_checking.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5347 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha1_validating_admission_policy.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5537 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha1_validating_admission_policy_binding.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5089 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha1_validating_admission_policy_binding_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     6871 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha1_validating_admission_policy_binding_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5037 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1alpha1_validating_admission_policy_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     9352 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha1_validating_admission_policy_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4574 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha1_validating_admission_policy_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     8617 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1alpha1_validation.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3714 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha1_variable.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5666 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1alpha1_volume_attributes_class.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5008 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1alpha1_volume_attributes_class_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5284 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha2_allocation_result.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5374 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha2_pod_scheduling_context.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4992 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha2_pod_scheduling_context_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3946 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha2_pod_scheduling_context_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4073 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha2_pod_scheduling_context_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5317 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1alpha2_resource_claim.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4037 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha2_resource_claim_consumer_reference.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4906 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha2_resource_claim_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3946 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha2_resource_claim_parameters_reference.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3796 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1alpha2_resource_claim_scheduling_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4295 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha2_resource_claim_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5352 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha2_resource_claim_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4758 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha2_resource_claim_template.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4989 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha2_resource_claim_template_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3885 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1alpha2_resource_claim_template_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5822 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha2_resource_class.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4908 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha2_resource_class_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4120 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha2_resource_class_parameters_reference.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4118 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1alpha2_resource_handle.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4810 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta1_audit_annotation.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3704 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta1_expression_warning.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4766 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta1_match_condition.py
+-rw-r--r--   0 nickc      (503) staff       (20)     7172 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta1_match_resources.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5597 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta1_named_rule_with_operations.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3496 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta1_param_kind.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5476 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta1_param_ref.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5036 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta1_self_subject_review.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3537 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta1_self_subject_review_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3905 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta1_type_checking.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5336 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta1_validating_admission_policy.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5530 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta1_validating_admission_policy_binding.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5082 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1beta1_validating_admission_policy_binding_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     6860 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta1_validating_admission_policy_binding_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5030 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta1_validating_admission_policy_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     9325 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta1_validating_admission_policy_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4570 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta1_validating_admission_policy_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     8614 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1beta1_validation.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3756 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta1_variable.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4851 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta3_exempt_priority_level_configuration.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3324 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta3_flow_distinguisher_method.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5262 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta3_flow_schema.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4198 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta3_flow_schema_condition.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4877 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta3_flow_schema_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5807 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta3_flow_schema_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3801 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta3_flow_schema_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3374 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1beta3_group_subject.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3902 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta3_limit_response.py
+-rw-r--r--   0 nickc      (503) staff       (20)     6366 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta3_limited_priority_level_configuration.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4152 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1beta3_non_resource_policy_rule.py
+-rw-r--r--   0 nickc      (503) staff       (20)     6070 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta3_policy_rules_with_subjects.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5284 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta3_priority_level_configuration.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4264 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1beta3_priority_level_configuration_condition.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5029 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta3_priority_level_configuration_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3367 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta3_priority_level_configuration_reference.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4700 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta3_priority_level_configuration_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3939 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta3_priority_level_configuration_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4758 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1beta3_queuing_configuration.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5542 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta3_resource_policy_rule.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3503 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta3_service_account_subject.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4632 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v1beta3_subject.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3246 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v1beta3_user_subject.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4191 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v2_container_resource_metric_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4132 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v2_container_resource_metric_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3802 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v2_cross_version_object_reference.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3933 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v2_external_metric_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3865 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v2_external_metric_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5326 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v2_horizontal_pod_autoscaler.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4030 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v2_horizontal_pod_autoscaler_behavior.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4157 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v2_horizontal_pod_autoscaler_condition.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4984 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v2_horizontal_pod_autoscaler_list.py
+-rw-r--r--   0 nickc      (503) staff       (20)     6024 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v2_horizontal_pod_autoscaler_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5935 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v2_horizontal_pod_autoscaler_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3749 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v2_hpa_scaling_policy.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5134 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v2_hpa_scaling_rules.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3610 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v2_metric_identifier.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5673 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v2_metric_spec.py
+-rw-r--r--   0 nickc      (503) staff       (20)     5619 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v2_metric_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4167 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v2_metric_target.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3929 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v2_metric_value_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4392 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v2_object_metric_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     4427 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v2_object_metric_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3942 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v2_pods_metric_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3897 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/v2_pods_metric_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3974 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v2_resource_metric_source.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3893 2024-05-03 23:41:06.000000 k8-29.0.8/src/k8/v2_resource_metric_status.py
+-rw-r--r--   0 nickc      (503) staff       (20)     3966 2024-05-03 23:41:05.000000 k8-29.0.8/src/k8/version_info.py
+drwxr-xr-x   0 nickc      (503) staff       (20)        0 2024-05-03 23:47:32.669626 k8-29.0.8/src/k8.egg-info/
+-rw-r--r--   0 nickc      (503) staff       (20)      631 2024-05-03 23:47:32.000000 k8-29.0.8/src/k8.egg-info/PKG-INFO
+-rw-r--r--   0 nickc      (503) staff       (20)    19965 2024-05-03 23:47:32.000000 k8-29.0.8/src/k8.egg-info/SOURCES.txt
+-rw-r--r--   0 nickc      (503) staff       (20)        1 2024-05-03 23:47:32.000000 k8-29.0.8/src/k8.egg-info/dependency_links.txt
+-rw-r--r--   0 nickc      (503) staff       (20)       26 2024-05-03 23:47:32.000000 k8-29.0.8/src/k8.egg-info/requires.txt
+-rw-r--r--   0 nickc      (503) staff       (20)        3 2024-05-03 23:47:32.000000 k8-29.0.8/src/k8.egg-info/top_level.txt
```

### Comparing `k8-29.0.7/LICENSE` & `k8-29.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/PKG-INFO` & `k8-29.0.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k8
-Version: 29.0.7
+Version: 29.0.8
 Summary: Kubernetes Python Models
 Author-email: Nick Cooper <nick@not.fun>
 Project-URL: Homepage, https://github.com/nicknotfun/k8
 Project-URL: Issues, https://github.com/nicknotfun/k8/issues
 Keywords: OpenAPI,OpenAPI-Generator,Kubernetes
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `k8-29.0.7/pyproject.toml` & `k8-29.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "k8"
-version = "29.0.7" # Note, should match kubernetes-client/python in refresh.sh
+version = "29.0.8" # Note, should match kubernetes-client/python in refresh.sh
 authors = [
   { name="Nick Cooper", email="nick@not.fun" },
 ]
 description = "Kubernetes Python Models"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `k8-29.0.7/src/k8/admissionregistration_v1_service_reference.py` & `k8-29.0.8/src/k8/admissionregistration_v1_service_reference.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/admissionregistration_v1_webhook_client_config.py` & `k8-29.0.8/src/k8/admissionregistration_v1_webhook_client_config.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/apiextensions_v1_service_reference.py` & `k8-29.0.8/src/k8/apiextensions_v1_service_reference.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/apiextensions_v1_webhook_client_config.py` & `k8-29.0.8/src/k8/apiextensions_v1_webhook_client_config.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/apiregistration_v1_service_reference.py` & `k8-29.0.8/src/k8/apiregistration_v1_service_reference.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/authentication_v1_token_request.py` & `k8-29.0.8/src/k8/authentication_v1_token_request.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/core_v1_endpoint_port.py` & `k8-29.0.8/src/k8/core_v1_endpoint_port.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/core_v1_event.py` & `k8-29.0.8/src/k8/core_v1_event.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/core_v1_event_list.py` & `k8-29.0.8/src/k8/core_v1_event_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/core_v1_event_series.py` & `k8-29.0.8/src/k8/core_v1_event_series.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/discovery_v1_endpoint_port.py` & `k8-29.0.8/src/k8/discovery_v1_endpoint_port.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/events_v1_event.py` & `k8-29.0.8/src/k8/events_v1_event.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/events_v1_event_list.py` & `k8-29.0.8/src/k8/events_v1_event_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/events_v1_event_series.py` & `k8-29.0.8/src/k8/events_v1_event_series.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/flowcontrol_v1_subject.py` & `k8-29.0.8/src/k8/flowcontrol_v1_subject.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/rbac_v1_subject.py` & `k8-29.0.8/src/k8/rbac_v1_subject.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/storage_v1_token_request.py` & `k8-29.0.8/src/k8/storage_v1_token_request.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_affinity.py` & `k8-29.0.8/src/k8/v1_affinity.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_aggregation_rule.py` & `k8-29.0.8/src/k8/v1_aggregation_rule.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_api_group.py` & `k8-29.0.8/src/k8/v1_api_group.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_api_group_list.py` & `k8-29.0.8/src/k8/v1_api_group_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_api_resource.py` & `k8-29.0.8/src/k8/v1_api_resource.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_api_resource_list.py` & `k8-29.0.8/src/k8/v1_api_resource_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_api_service.py` & `k8-29.0.8/src/k8/v1_api_service.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_api_service_condition.py` & `k8-29.0.8/src/k8/v1_api_service_condition.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_api_service_list.py` & `k8-29.0.8/src/k8/v1_api_service_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_api_service_spec.py` & `k8-29.0.8/src/k8/v1_api_service_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_api_service_status.py` & `k8-29.0.8/src/k8/v1_api_service_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_api_versions.py` & `k8-29.0.8/src/k8/v1_api_versions.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_attached_volume.py` & `k8-29.0.8/src/k8/v1_attached_volume.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_aws_elastic_block_store_volume_source.py` & `k8-29.0.8/src/k8/v1_aws_elastic_block_store_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_azure_disk_volume_source.py` & `k8-29.0.8/src/k8/v1_azure_disk_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_azure_file_persistent_volume_source.py` & `k8-29.0.8/src/k8/v1_azure_file_persistent_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_azure_file_volume_source.py` & `k8-29.0.8/src/k8/v1_azure_file_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_binding.py` & `k8-29.0.8/src/k8/v1_binding.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_bound_object_reference.py` & `k8-29.0.8/src/k8/v1_bound_object_reference.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_capabilities.py` & `k8-29.0.8/src/k8/v1_capabilities.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_ceph_fs_persistent_volume_source.py` & `k8-29.0.8/src/k8/v1_ceph_fs_persistent_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_ceph_fs_volume_source.py` & `k8-29.0.8/src/k8/v1_ceph_fs_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_certificate_signing_request.py` & `k8-29.0.8/src/k8/v1_certificate_signing_request.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_certificate_signing_request_condition.py` & `k8-29.0.8/src/k8/v1_certificate_signing_request_condition.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_certificate_signing_request_list.py` & `k8-29.0.8/src/k8/v1_certificate_signing_request_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_certificate_signing_request_spec.py` & `k8-29.0.8/src/k8/v1_certificate_signing_request_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_certificate_signing_request_status.py` & `k8-29.0.8/src/k8/v1_certificate_signing_request_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_cinder_persistent_volume_source.py` & `k8-29.0.8/src/k8/v1_cinder_persistent_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_cinder_volume_source.py` & `k8-29.0.8/src/k8/v1_cinder_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_claim_source.py` & `k8-29.0.8/src/k8/v1_claim_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_client_ip_config.py` & `k8-29.0.8/src/k8/v1_client_ip_config.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_cluster_role.py` & `k8-29.0.8/src/k8/v1_cluster_role.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_cluster_role_binding.py` & `k8-29.0.8/src/k8/v1_cluster_role_binding.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_cluster_role_binding_list.py` & `k8-29.0.8/src/k8/v1_cluster_role_binding_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_cluster_role_list.py` & `k8-29.0.8/src/k8/v1_cluster_role_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_cluster_trust_bundle_projection.py` & `k8-29.0.8/src/k8/v1_cluster_trust_bundle_projection.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_component_condition.py` & `k8-29.0.8/src/k8/v1_component_condition.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_component_status.py` & `k8-29.0.8/src/k8/v1_component_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_component_status_list.py` & `k8-29.0.8/src/k8/v1_component_status_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_condition.py` & `k8-29.0.8/src/k8/v1_condition.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_config_map.py` & `k8-29.0.8/src/k8/v1_config_map.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_config_map_env_source.py` & `k8-29.0.8/src/k8/v1_config_map_env_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_config_map_key_selector.py` & `k8-29.0.8/src/k8/v1_config_map_key_selector.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_config_map_list.py` & `k8-29.0.8/src/k8/v1_config_map_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_config_map_node_config_source.py` & `k8-29.0.8/src/k8/v1_config_map_node_config_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_config_map_projection.py` & `k8-29.0.8/src/k8/v1_config_map_projection.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_config_map_volume_source.py` & `k8-29.0.8/src/k8/v1_config_map_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_container.py` & `k8-29.0.8/src/k8/v1_container.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_container_image.py` & `k8-29.0.8/src/k8/v1_container_image.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_container_port.py` & `k8-29.0.8/src/k8/v1_container_port.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_container_resize_policy.py` & `k8-29.0.8/src/k8/v1_container_resize_policy.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_container_state.py` & `k8-29.0.8/src/k8/v1_container_state.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_container_state_running.py` & `k8-29.0.8/src/k8/v1_container_state_running.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_container_state_terminated.py` & `k8-29.0.8/src/k8/v1_container_state_terminated.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_container_state_waiting.py` & `k8-29.0.8/src/k8/v1_container_state_waiting.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_container_status.py` & `k8-29.0.8/src/k8/v1_container_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_controller_revision.py` & `k8-29.0.8/src/k8/v1_controller_revision.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_controller_revision_list.py` & `k8-29.0.8/src/k8/v1_controller_revision_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_cron_job.py` & `k8-29.0.8/src/k8/v1_cron_job.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_cron_job_list.py` & `k8-29.0.8/src/k8/v1_cron_job_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_cron_job_spec.py` & `k8-29.0.8/src/k8/v1_cron_job_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_cron_job_status.py` & `k8-29.0.8/src/k8/v1_cron_job_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_cross_version_object_reference.py` & `k8-29.0.8/src/k8/v1_cross_version_object_reference.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_csi_driver.py` & `k8-29.0.8/src/k8/v1_csi_driver.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_csi_driver_list.py` & `k8-29.0.8/src/k8/v1_csi_driver_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_csi_driver_spec.py` & `k8-29.0.8/src/k8/v1_csi_driver_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_csi_node.py` & `k8-29.0.8/src/k8/v1_csi_node.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_csi_node_driver.py` & `k8-29.0.8/src/k8/v1_csi_node_driver.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_csi_node_list.py` & `k8-29.0.8/src/k8/v1_csi_node_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_csi_node_spec.py` & `k8-29.0.8/src/k8/v1_csi_node_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_csi_persistent_volume_source.py` & `k8-29.0.8/src/k8/v1_csi_persistent_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_csi_storage_capacity.py` & `k8-29.0.8/src/k8/v1_csi_storage_capacity.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_csi_storage_capacity_list.py` & `k8-29.0.8/src/k8/v1_csi_storage_capacity_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_csi_volume_source.py` & `k8-29.0.8/src/k8/v1_csi_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_custom_resource_column_definition.py` & `k8-29.0.8/src/k8/v1_custom_resource_column_definition.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_custom_resource_conversion.py` & `k8-29.0.8/src/k8/v1_custom_resource_conversion.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_custom_resource_definition.py` & `k8-29.0.8/src/k8/v1_custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_custom_resource_definition_condition.py` & `k8-29.0.8/src/k8/v1_custom_resource_definition_condition.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_custom_resource_definition_list.py` & `k8-29.0.8/src/k8/v1_custom_resource_definition_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_custom_resource_definition_names.py` & `k8-29.0.8/src/k8/v1_custom_resource_definition_names.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_custom_resource_definition_spec.py` & `k8-29.0.8/src/k8/v1_custom_resource_definition_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_custom_resource_definition_status.py` & `k8-29.0.8/src/k8/v1_custom_resource_definition_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_custom_resource_definition_version.py` & `k8-29.0.8/src/k8/v1_custom_resource_definition_version.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_custom_resource_subresource_scale.py` & `k8-29.0.8/src/k8/v1_custom_resource_subresource_scale.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_custom_resource_subresources.py` & `k8-29.0.8/src/k8/v1_custom_resource_subresources.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_custom_resource_validation.py` & `k8-29.0.8/src/k8/v1_custom_resource_validation.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_daemon_endpoint.py` & `k8-29.0.8/src/k8/v1_daemon_endpoint.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_daemon_set.py` & `k8-29.0.8/src/k8/v1_daemon_set.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_daemon_set_condition.py` & `k8-29.0.8/src/k8/v1_daemon_set_condition.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_daemon_set_list.py` & `k8-29.0.8/src/k8/v1_daemon_set_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_daemon_set_spec.py` & `k8-29.0.8/src/k8/v1_daemon_set_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_daemon_set_status.py` & `k8-29.0.8/src/k8/v1_daemon_set_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_daemon_set_update_strategy.py` & `k8-29.0.8/src/k8/v1_daemon_set_update_strategy.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_delete_options.py` & `k8-29.0.8/src/k8/v1_delete_options.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_deployment.py` & `k8-29.0.8/src/k8/v1_deployment.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_deployment_condition.py` & `k8-29.0.8/src/k8/v1_deployment_condition.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_deployment_list.py` & `k8-29.0.8/src/k8/v1_deployment_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_deployment_spec.py` & `k8-29.0.8/src/k8/v1_deployment_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_deployment_status.py` & `k8-29.0.8/src/k8/v1_deployment_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_deployment_strategy.py` & `k8-29.0.8/src/k8/v1_deployment_strategy.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_downward_api_projection.py` & `k8-29.0.8/src/k8/v1_downward_api_projection.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_downward_api_volume_file.py` & `k8-29.0.8/src/k8/v1_downward_api_volume_file.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_downward_api_volume_source.py` & `k8-29.0.8/src/k8/v1_downward_api_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_empty_dir_volume_source.py` & `k8-29.0.8/src/k8/v1_empty_dir_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_endpoint.py` & `k8-29.0.8/src/k8/v1_endpoint.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_endpoint_address.py` & `k8-29.0.8/src/k8/v1_endpoint_address.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_endpoint_conditions.py` & `k8-29.0.8/src/k8/v1_endpoint_conditions.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_endpoint_hints.py` & `k8-29.0.8/src/k8/v1_endpoint_hints.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_endpoint_slice.py` & `k8-29.0.8/src/k8/v1_endpoint_slice.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_endpoint_slice_list.py` & `k8-29.0.8/src/k8/v1_endpoint_slice_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_endpoint_subset.py` & `k8-29.0.8/src/k8/v1_endpoint_subset.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_endpoints.py` & `k8-29.0.8/src/k8/v1_endpoints.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_endpoints_list.py` & `k8-29.0.8/src/k8/v1_endpoints_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_env_from_source.py` & `k8-29.0.8/src/k8/v1_env_from_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_env_var.py` & `k8-29.0.8/src/k8/v1_env_var.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_env_var_source.py` & `k8-29.0.8/src/k8/v1_env_var_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_ephemeral_container.py` & `k8-29.0.8/src/k8/v1_ephemeral_container.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_ephemeral_volume_source.py` & `k8-29.0.8/src/k8/v1_ephemeral_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_event_source.py` & `k8-29.0.8/src/k8/v1_event_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_eviction.py` & `k8-29.0.8/src/k8/v1_eviction.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_exec_action.py` & `k8-29.0.8/src/k8/v1_exec_action.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_exempt_priority_level_configuration.py` & `k8-29.0.8/src/k8/v1_exempt_priority_level_configuration.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_external_documentation.py` & `k8-29.0.8/src/k8/v1_external_documentation.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_fc_volume_source.py` & `k8-29.0.8/src/k8/v1_fc_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_flex_persistent_volume_source.py` & `k8-29.0.8/src/k8/v1_flex_persistent_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_flex_volume_source.py` & `k8-29.0.8/src/k8/v1_flex_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_flocker_volume_source.py` & `k8-29.0.8/src/k8/v1_flocker_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_flow_distinguisher_method.py` & `k8-29.0.8/src/k8/v1_flow_distinguisher_method.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_flow_schema.py` & `k8-29.0.8/src/k8/v1_flow_schema.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_flow_schema_condition.py` & `k8-29.0.8/src/k8/v1_flow_schema_condition.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_flow_schema_list.py` & `k8-29.0.8/src/k8/v1_flow_schema_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_flow_schema_spec.py` & `k8-29.0.8/src/k8/v1_flow_schema_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_flow_schema_status.py` & `k8-29.0.8/src/k8/v1_flow_schema_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_for_zone.py` & `k8-29.0.8/src/k8/v1_for_zone.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_gce_persistent_disk_volume_source.py` & `k8-29.0.8/src/k8/v1_gce_persistent_disk_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_git_repo_volume_source.py` & `k8-29.0.8/src/k8/v1_git_repo_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_glusterfs_persistent_volume_source.py` & `k8-29.0.8/src/k8/v1_glusterfs_persistent_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_glusterfs_volume_source.py` & `k8-29.0.8/src/k8/v1_glusterfs_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_group_subject.py` & `k8-29.0.8/src/k8/v1_group_subject.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_group_version_for_discovery.py` & `k8-29.0.8/src/k8/v1_group_version_for_discovery.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_grpc_action.py` & `k8-29.0.8/src/k8/v1_grpc_action.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_horizontal_pod_autoscaler.py` & `k8-29.0.8/src/k8/v1_horizontal_pod_autoscaler.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_horizontal_pod_autoscaler_list.py` & `k8-29.0.8/src/k8/v1_horizontal_pod_autoscaler_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_horizontal_pod_autoscaler_spec.py` & `k8-29.0.8/src/k8/v1_horizontal_pod_autoscaler_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_horizontal_pod_autoscaler_status.py` & `k8-29.0.8/src/k8/v1_horizontal_pod_autoscaler_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_host_alias.py` & `k8-29.0.8/src/k8/v1_host_alias.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_host_ip.py` & `k8-29.0.8/src/k8/v1_host_ip.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_host_path_volume_source.py` & `k8-29.0.8/src/k8/v1_host_path_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_http_get_action.py` & `k8-29.0.8/src/k8/v1_http_get_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 class V1HTTPGetAction(BaseModel):
     """
     HTTPGetAction describes an action based on HTTP Get requests.
     """ # noqa: E501
     host: Optional[StrictStr] = Field(default=None, description="Host name to connect to, defaults to the pod IP. You probably want to set \"Host\" in httpHeaders instead.")
     http_headers: Optional[List[V1HTTPHeader]] = Field(default=None, description="Custom headers to set in the request. HTTP allows repeated headers.", alias="httpHeaders")
     path: Optional[StrictStr] = Field(default=None, description="Path to access on the HTTP server.")
-    port: Dict[str, Any] = Field(description="It's an int or a string.")
+    port: int | str = Field(description="It's an int or a string.")
     scheme: Optional[StrictStr] = Field(default=None, description="Scheme to use for connecting to the host. Defaults to HTTP.")
     additional_properties: Dict[str, Any] = {}
     __properties: ClassVar[List[str]] = ["host", "httpHeaders", "path", "port", "scheme"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
```

### Comparing `k8-29.0.7/src/k8/v1_http_header.py` & `k8-29.0.8/src/k8/v1_http_header.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_http_ingress_path.py` & `k8-29.0.8/src/k8/v1_http_ingress_path.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_http_ingress_rule_value.py` & `k8-29.0.8/src/k8/v1_http_ingress_rule_value.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_ingress.py` & `k8-29.0.8/src/k8/v1_ingress.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_ingress_backend.py` & `k8-29.0.8/src/k8/v1_ingress_backend.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_ingress_class.py` & `k8-29.0.8/src/k8/v1_ingress_class.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_ingress_class_list.py` & `k8-29.0.8/src/k8/v1_ingress_class_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_ingress_class_parameters_reference.py` & `k8-29.0.8/src/k8/v1_ingress_class_parameters_reference.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_ingress_class_spec.py` & `k8-29.0.8/src/k8/v1_ingress_class_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_ingress_list.py` & `k8-29.0.8/src/k8/v1_ingress_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_ingress_load_balancer_ingress.py` & `k8-29.0.8/src/k8/v1_ingress_load_balancer_ingress.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_ingress_load_balancer_status.py` & `k8-29.0.8/src/k8/v1_ingress_load_balancer_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_ingress_port_status.py` & `k8-29.0.8/src/k8/v1_ingress_port_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_ingress_rule.py` & `k8-29.0.8/src/k8/v1_ingress_rule.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_ingress_service_backend.py` & `k8-29.0.8/src/k8/v1_ingress_service_backend.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_ingress_spec.py` & `k8-29.0.8/src/k8/v1_ingress_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_ingress_status.py` & `k8-29.0.8/src/k8/v1_ingress_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_ingress_tls.py` & `k8-29.0.8/src/k8/v1_ingress_tls.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_ip_block.py` & `k8-29.0.8/src/k8/v1_ip_block.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_iscsi_persistent_volume_source.py` & `k8-29.0.8/src/k8/v1_iscsi_persistent_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_iscsi_volume_source.py` & `k8-29.0.8/src/k8/v1_iscsi_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_job.py` & `k8-29.0.8/src/k8/v1_job.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_job_condition.py` & `k8-29.0.8/src/k8/v1_job_condition.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_job_list.py` & `k8-29.0.8/src/k8/v1_job_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_job_spec.py` & `k8-29.0.8/src/k8/v1_job_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_job_status.py` & `k8-29.0.8/src/k8/v1_job_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_job_template_spec.py` & `k8-29.0.8/src/k8/v1_job_template_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_json_schema_props.py` & `k8-29.0.8/src/k8/v1_json_schema_props.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_key_to_path.py` & `k8-29.0.8/src/k8/v1_key_to_path.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_label_selector.py` & `k8-29.0.8/src/k8/v1_label_selector.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_label_selector_requirement.py` & `k8-29.0.8/src/k8/v1_label_selector_requirement.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_lease.py` & `k8-29.0.8/src/k8/v1_lease.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_lease_list.py` & `k8-29.0.8/src/k8/v1_lease_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_lease_spec.py` & `k8-29.0.8/src/k8/v1_lease_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_lifecycle.py` & `k8-29.0.8/src/k8/v1_lifecycle.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_lifecycle_handler.py` & `k8-29.0.8/src/k8/v1_lifecycle_handler.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_limit_range.py` & `k8-29.0.8/src/k8/v1_limit_range.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_limit_range_item.py` & `k8-29.0.8/src/k8/v1_limit_range_item.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_limit_range_list.py` & `k8-29.0.8/src/k8/v1_limit_range_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_limit_range_spec.py` & `k8-29.0.8/src/k8/v1_limit_range_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_limit_response.py` & `k8-29.0.8/src/k8/v1_limit_response.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_limited_priority_level_configuration.py` & `k8-29.0.8/src/k8/v1_limited_priority_level_configuration.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_list_meta.py` & `k8-29.0.8/src/k8/v1_list_meta.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_load_balancer_ingress.py` & `k8-29.0.8/src/k8/v1_load_balancer_ingress.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_load_balancer_status.py` & `k8-29.0.8/src/k8/v1_load_balancer_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_local_object_reference.py` & `k8-29.0.8/src/k8/v1_local_object_reference.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_local_subject_access_review.py` & `k8-29.0.8/src/k8/v1_local_subject_access_review.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_local_volume_source.py` & `k8-29.0.8/src/k8/v1_local_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_managed_fields_entry.py` & `k8-29.0.8/src/k8/v1_managed_fields_entry.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_match_condition.py` & `k8-29.0.8/src/k8/v1_match_condition.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_modify_volume_status.py` & `k8-29.0.8/src/k8/v1_modify_volume_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_mutating_webhook.py` & `k8-29.0.8/src/k8/v1_mutating_webhook.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_mutating_webhook_configuration.py` & `k8-29.0.8/src/k8/v1_mutating_webhook_configuration.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_mutating_webhook_configuration_list.py` & `k8-29.0.8/src/k8/v1_mutating_webhook_configuration_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_namespace.py` & `k8-29.0.8/src/k8/v1_namespace.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_namespace_condition.py` & `k8-29.0.8/src/k8/v1_namespace_condition.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_namespace_list.py` & `k8-29.0.8/src/k8/v1_namespace_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_namespace_spec.py` & `k8-29.0.8/src/k8/v1_namespace_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_namespace_status.py` & `k8-29.0.8/src/k8/v1_namespace_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_network_policy.py` & `k8-29.0.8/src/k8/v1_network_policy.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_network_policy_egress_rule.py` & `k8-29.0.8/src/k8/v1_network_policy_egress_rule.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_network_policy_ingress_rule.py` & `k8-29.0.8/src/k8/v1_network_policy_ingress_rule.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_network_policy_list.py` & `k8-29.0.8/src/k8/v1_network_policy_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_network_policy_peer.py` & `k8-29.0.8/src/k8/v1_network_policy_peer.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_network_policy_port.py` & `k8-29.0.8/src/k8/v1_network_policy_port.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_network_policy_spec.py` & `k8-29.0.8/src/k8/v1_network_policy_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_nfs_volume_source.py` & `k8-29.0.8/src/k8/v1_nfs_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_node.py` & `k8-29.0.8/src/k8/v1_node.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_node_address.py` & `k8-29.0.8/src/k8/v1_node_address.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_node_affinity.py` & `k8-29.0.8/src/k8/v1_node_affinity.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_node_condition.py` & `k8-29.0.8/src/k8/v1_node_condition.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_node_config_source.py` & `k8-29.0.8/src/k8/v1_node_config_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_node_config_status.py` & `k8-29.0.8/src/k8/v1_node_config_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_node_daemon_endpoints.py` & `k8-29.0.8/src/k8/v1_node_daemon_endpoints.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_node_list.py` & `k8-29.0.8/src/k8/v1_node_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_node_selector.py` & `k8-29.0.8/src/k8/v1_node_selector.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_node_selector_requirement.py` & `k8-29.0.8/src/k8/v1_node_selector_requirement.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_node_selector_term.py` & `k8-29.0.8/src/k8/v1_node_selector_term.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_node_spec.py` & `k8-29.0.8/src/k8/v1_node_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_node_status.py` & `k8-29.0.8/src/k8/v1_node_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_node_system_info.py` & `k8-29.0.8/src/k8/v1_node_system_info.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_non_resource_attributes.py` & `k8-29.0.8/src/k8/v1_non_resource_attributes.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_non_resource_policy_rule.py` & `k8-29.0.8/src/k8/v1_non_resource_policy_rule.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_non_resource_rule.py` & `k8-29.0.8/src/k8/v1_non_resource_rule.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_object_field_selector.py` & `k8-29.0.8/src/k8/v1_object_field_selector.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_object_meta.py` & `k8-29.0.8/src/k8/v1_object_meta.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_object_reference.py` & `k8-29.0.8/src/k8/v1_object_reference.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_overhead.py` & `k8-29.0.8/src/k8/v1_overhead.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_owner_reference.py` & `k8-29.0.8/src/k8/v1_owner_reference.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_persistent_volume.py` & `k8-29.0.8/src/k8/v1_persistent_volume.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_persistent_volume_claim.py` & `k8-29.0.8/src/k8/v1_persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_persistent_volume_claim_condition.py` & `k8-29.0.8/src/k8/v1_persistent_volume_claim_condition.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_persistent_volume_claim_list.py` & `k8-29.0.8/src/k8/v1_persistent_volume_claim_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_persistent_volume_claim_spec.py` & `k8-29.0.8/src/k8/v1_persistent_volume_claim_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_persistent_volume_claim_status.py` & `k8-29.0.8/src/k8/v1_persistent_volume_claim_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_persistent_volume_claim_template.py` & `k8-29.0.8/src/k8/v1_persistent_volume_claim_template.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_persistent_volume_claim_volume_source.py` & `k8-29.0.8/src/k8/v1_persistent_volume_claim_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_persistent_volume_list.py` & `k8-29.0.8/src/k8/v1_persistent_volume_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_persistent_volume_spec.py` & `k8-29.0.8/src/k8/v1_persistent_volume_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_persistent_volume_status.py` & `k8-29.0.8/src/k8/v1_persistent_volume_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_photon_persistent_disk_volume_source.py` & `k8-29.0.8/src/k8/v1_photon_persistent_disk_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_pod.py` & `k8-29.0.8/src/k8/v1_pod.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_pod_affinity.py` & `k8-29.0.8/src/k8/v1_pod_affinity.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_pod_affinity_term.py` & `k8-29.0.8/src/k8/v1_pod_affinity_term.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_pod_anti_affinity.py` & `k8-29.0.8/src/k8/v1_pod_anti_affinity.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_pod_condition.py` & `k8-29.0.8/src/k8/v1_pod_condition.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_pod_disruption_budget.py` & `k8-29.0.8/src/k8/v1_pod_disruption_budget.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_pod_disruption_budget_list.py` & `k8-29.0.8/src/k8/v1_pod_disruption_budget_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_pod_disruption_budget_spec.py` & `k8-29.0.8/src/k8/v1_pod_disruption_budget_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_pod_disruption_budget_status.py` & `k8-29.0.8/src/k8/v1_pod_disruption_budget_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_pod_dns_config.py` & `k8-29.0.8/src/k8/v1_pod_dns_config.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_pod_dns_config_option.py` & `k8-29.0.8/src/k8/v1_pod_dns_config_option.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_pod_failure_policy.py` & `k8-29.0.8/src/k8/v1_pod_failure_policy.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_pod_failure_policy_on_exit_codes_requirement.py` & `k8-29.0.8/src/k8/v1_pod_failure_policy_on_exit_codes_requirement.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_pod_failure_policy_on_pod_conditions_pattern.py` & `k8-29.0.8/src/k8/v1_pod_failure_policy_on_pod_conditions_pattern.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_pod_failure_policy_rule.py` & `k8-29.0.8/src/k8/v1_pod_failure_policy_rule.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_pod_ip.py` & `k8-29.0.8/src/k8/v1_pod_ip.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_pod_list.py` & `k8-29.0.8/src/k8/v1_pod_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_pod_os.py` & `k8-29.0.8/src/k8/v1_pod_os.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_pod_readiness_gate.py` & `k8-29.0.8/src/k8/v1_pod_readiness_gate.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_pod_resource_claim.py` & `k8-29.0.8/src/k8/v1_pod_resource_claim.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_pod_resource_claim_status.py` & `k8-29.0.8/src/k8/v1_pod_resource_claim_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_pod_scheduling_gate.py` & `k8-29.0.8/src/k8/v1_pod_scheduling_gate.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_pod_security_context.py` & `k8-29.0.8/src/k8/v1_pod_security_context.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_pod_spec.py` & `k8-29.0.8/src/k8/v1_pod_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_pod_status.py` & `k8-29.0.8/src/k8/v1_pod_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_pod_template.py` & `k8-29.0.8/src/k8/v1_pod_template.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_pod_template_list.py` & `k8-29.0.8/src/k8/v1_pod_template_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_pod_template_spec.py` & `k8-29.0.8/src/k8/v1_pod_template_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_policy_rule.py` & `k8-29.0.8/src/k8/v1_policy_rule.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_policy_rules_with_subjects.py` & `k8-29.0.8/src/k8/v1_policy_rules_with_subjects.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_port_status.py` & `k8-29.0.8/src/k8/v1_port_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_portworx_volume_source.py` & `k8-29.0.8/src/k8/v1_portworx_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_preconditions.py` & `k8-29.0.8/src/k8/v1_preconditions.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_preferred_scheduling_term.py` & `k8-29.0.8/src/k8/v1_preferred_scheduling_term.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_priority_class.py` & `k8-29.0.8/src/k8/v1_priority_class.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_priority_class_list.py` & `k8-29.0.8/src/k8/v1_priority_class_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_priority_level_configuration.py` & `k8-29.0.8/src/k8/v1_priority_level_configuration.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_priority_level_configuration_condition.py` & `k8-29.0.8/src/k8/v1_priority_level_configuration_condition.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_priority_level_configuration_list.py` & `k8-29.0.8/src/k8/v1_priority_level_configuration_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_priority_level_configuration_reference.py` & `k8-29.0.8/src/k8/v1_priority_level_configuration_reference.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_priority_level_configuration_spec.py` & `k8-29.0.8/src/k8/v1_priority_level_configuration_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_priority_level_configuration_status.py` & `k8-29.0.8/src/k8/v1_priority_level_configuration_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_probe.py` & `k8-29.0.8/src/k8/v1_probe.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_projected_volume_source.py` & `k8-29.0.8/src/k8/v1_projected_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_queuing_configuration.py` & `k8-29.0.8/src/k8/v1_queuing_configuration.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_quobyte_volume_source.py` & `k8-29.0.8/src/k8/v1_quobyte_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_rbd_persistent_volume_source.py` & `k8-29.0.8/src/k8/v1_rbd_persistent_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_rbd_volume_source.py` & `k8-29.0.8/src/k8/v1_rbd_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_replica_set.py` & `k8-29.0.8/src/k8/v1_replica_set.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_replica_set_condition.py` & `k8-29.0.8/src/k8/v1_replica_set_condition.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_replica_set_list.py` & `k8-29.0.8/src/k8/v1_replica_set_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_replica_set_spec.py` & `k8-29.0.8/src/k8/v1_replica_set_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_replica_set_status.py` & `k8-29.0.8/src/k8/v1_replica_set_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_replication_controller.py` & `k8-29.0.8/src/k8/v1_replication_controller.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_replication_controller_condition.py` & `k8-29.0.8/src/k8/v1_replication_controller_condition.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_replication_controller_list.py` & `k8-29.0.8/src/k8/v1_replication_controller_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_replication_controller_spec.py` & `k8-29.0.8/src/k8/v1_replication_controller_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_replication_controller_status.py` & `k8-29.0.8/src/k8/v1_replication_controller_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_resource_attributes.py` & `k8-29.0.8/src/k8/v1_resource_attributes.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_resource_claim.py` & `k8-29.0.8/src/k8/v1_resource_claim.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_resource_field_selector.py` & `k8-29.0.8/src/k8/v1_resource_field_selector.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_resource_policy_rule.py` & `k8-29.0.8/src/k8/v1_resource_policy_rule.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_resource_quota.py` & `k8-29.0.8/src/k8/v1_resource_quota.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_resource_quota_list.py` & `k8-29.0.8/src/k8/v1_resource_quota_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_resource_quota_spec.py` & `k8-29.0.8/src/k8/v1_resource_quota_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_resource_quota_status.py` & `k8-29.0.8/src/k8/v1_resource_quota_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_resource_requirements.py` & `k8-29.0.8/src/k8/v1_resource_requirements.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_resource_rule.py` & `k8-29.0.8/src/k8/v1_resource_rule.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_role.py` & `k8-29.0.8/src/k8/v1_role.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_role_binding.py` & `k8-29.0.8/src/k8/v1_role_binding.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_role_binding_list.py` & `k8-29.0.8/src/k8/v1_role_binding_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_role_list.py` & `k8-29.0.8/src/k8/v1_role_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_role_ref.py` & `k8-29.0.8/src/k8/v1_role_ref.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_rolling_update_daemon_set.py` & `k8-29.0.8/src/k8/v1_rolling_update_daemon_set.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_rolling_update_deployment.py` & `k8-29.0.8/src/k8/v1_rolling_update_deployment.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_rolling_update_stateful_set_strategy.py` & `k8-29.0.8/src/k8/v1_rolling_update_stateful_set_strategy.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_rule_with_operations.py` & `k8-29.0.8/src/k8/v1_rule_with_operations.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_runtime_class.py` & `k8-29.0.8/src/k8/v1_runtime_class.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_runtime_class_list.py` & `k8-29.0.8/src/k8/v1_runtime_class_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_scale.py` & `k8-29.0.8/src/k8/v1_scale.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_scale_io_persistent_volume_source.py` & `k8-29.0.8/src/k8/v1_scale_io_persistent_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_scale_io_volume_source.py` & `k8-29.0.8/src/k8/v1_scale_io_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_scale_spec.py` & `k8-29.0.8/src/k8/v1_scale_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_scale_status.py` & `k8-29.0.8/src/k8/v1_scale_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_scheduling.py` & `k8-29.0.8/src/k8/v1_scheduling.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_scope_selector.py` & `k8-29.0.8/src/k8/v1_scope_selector.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_scoped_resource_selector_requirement.py` & `k8-29.0.8/src/k8/v1_scoped_resource_selector_requirement.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_se_linux_options.py` & `k8-29.0.8/src/k8/v1_se_linux_options.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_seccomp_profile.py` & `k8-29.0.8/src/k8/v1_seccomp_profile.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_secret.py` & `k8-29.0.8/src/k8/v1_secret.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_secret_env_source.py` & `k8-29.0.8/src/k8/v1_secret_env_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_secret_key_selector.py` & `k8-29.0.8/src/k8/v1_secret_key_selector.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_secret_list.py` & `k8-29.0.8/src/k8/v1_secret_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_secret_projection.py` & `k8-29.0.8/src/k8/v1_secret_projection.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_secret_reference.py` & `k8-29.0.8/src/k8/v1_secret_reference.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_secret_volume_source.py` & `k8-29.0.8/src/k8/v1_secret_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_security_context.py` & `k8-29.0.8/src/k8/v1_security_context.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_self_subject_access_review.py` & `k8-29.0.8/src/k8/v1_self_subject_access_review.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_self_subject_access_review_spec.py` & `k8-29.0.8/src/k8/v1_self_subject_access_review_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_self_subject_review.py` & `k8-29.0.8/src/k8/v1_self_subject_review.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_self_subject_review_status.py` & `k8-29.0.8/src/k8/v1_self_subject_review_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_self_subject_rules_review.py` & `k8-29.0.8/src/k8/v1_self_subject_rules_review.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_self_subject_rules_review_spec.py` & `k8-29.0.8/src/k8/v1_self_subject_rules_review_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_server_address_by_client_cidr.py` & `k8-29.0.8/src/k8/v1_server_address_by_client_cidr.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_service.py` & `k8-29.0.8/src/k8/v1_service.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_service_account.py` & `k8-29.0.8/src/k8/v1_service_account.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_service_account_list.py` & `k8-29.0.8/src/k8/v1_service_account_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_service_account_subject.py` & `k8-29.0.8/src/k8/v1_service_account_subject.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_service_account_token_projection.py` & `k8-29.0.8/src/k8/v1_service_account_token_projection.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_service_backend_port.py` & `k8-29.0.8/src/k8/v1_service_backend_port.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_service_list.py` & `k8-29.0.8/src/k8/v1_service_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_service_port.py` & `k8-29.0.8/src/k8/v1_service_port.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_service_spec.py` & `k8-29.0.8/src/k8/v1_service_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_service_status.py` & `k8-29.0.8/src/k8/v1_service_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_session_affinity_config.py` & `k8-29.0.8/src/k8/v1_session_affinity_config.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_sleep_action.py` & `k8-29.0.8/src/k8/v1_sleep_action.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_stateful_set.py` & `k8-29.0.8/src/k8/v1_stateful_set.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_stateful_set_condition.py` & `k8-29.0.8/src/k8/v1_stateful_set_condition.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_stateful_set_list.py` & `k8-29.0.8/src/k8/v1_stateful_set_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_stateful_set_ordinals.py` & `k8-29.0.8/src/k8/v1_stateful_set_ordinals.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_stateful_set_persistent_volume_claim_retention_policy.py` & `k8-29.0.8/src/k8/v1_stateful_set_persistent_volume_claim_retention_policy.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_stateful_set_spec.py` & `k8-29.0.8/src/k8/v1_stateful_set_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_stateful_set_status.py` & `k8-29.0.8/src/k8/v1_stateful_set_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_stateful_set_update_strategy.py` & `k8-29.0.8/src/k8/v1_stateful_set_update_strategy.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_status.py` & `k8-29.0.8/src/k8/v1_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_status_cause.py` & `k8-29.0.8/src/k8/v1_status_cause.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_status_details.py` & `k8-29.0.8/src/k8/v1_status_details.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_storage_class.py` & `k8-29.0.8/src/k8/v1_storage_class.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_storage_class_list.py` & `k8-29.0.8/src/k8/v1_storage_class_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_storage_os_persistent_volume_source.py` & `k8-29.0.8/src/k8/v1_storage_os_persistent_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_storage_os_volume_source.py` & `k8-29.0.8/src/k8/v1_storage_os_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_subject_access_review.py` & `k8-29.0.8/src/k8/v1_subject_access_review.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_subject_access_review_spec.py` & `k8-29.0.8/src/k8/v1_subject_access_review_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_subject_access_review_status.py` & `k8-29.0.8/src/k8/v1_subject_access_review_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_subject_rules_review_status.py` & `k8-29.0.8/src/k8/v1_subject_rules_review_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_sysctl.py` & `k8-29.0.8/src/k8/v1_sysctl.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_taint.py` & `k8-29.0.8/src/k8/v1_taint.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_tcp_socket_action.py` & `k8-29.0.8/src/k8/v1_tcp_socket_action.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_token_request_spec.py` & `k8-29.0.8/src/k8/v1_token_request_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_token_request_status.py` & `k8-29.0.8/src/k8/v1_token_request_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_token_review.py` & `k8-29.0.8/src/k8/v1_token_review.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_token_review_spec.py` & `k8-29.0.8/src/k8/v1_token_review_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_token_review_status.py` & `k8-29.0.8/src/k8/v1_token_review_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_toleration.py` & `k8-29.0.8/src/k8/v1_toleration.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_topology_selector_label_requirement.py` & `k8-29.0.8/src/k8/v1_topology_selector_label_requirement.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_topology_selector_term.py` & `k8-29.0.8/src/k8/v1_topology_selector_term.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_topology_spread_constraint.py` & `k8-29.0.8/src/k8/v1_topology_spread_constraint.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_typed_local_object_reference.py` & `k8-29.0.8/src/k8/v1_typed_local_object_reference.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_typed_object_reference.py` & `k8-29.0.8/src/k8/v1_typed_object_reference.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_uncounted_terminated_pods.py` & `k8-29.0.8/src/k8/v1_uncounted_terminated_pods.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_user_info.py` & `k8-29.0.8/src/k8/v1_user_info.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_user_subject.py` & `k8-29.0.8/src/k8/v1_user_subject.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_validating_webhook.py` & `k8-29.0.8/src/k8/v1_validating_webhook.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_validating_webhook_configuration.py` & `k8-29.0.8/src/k8/v1_validating_webhook_configuration.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_validating_webhook_configuration_list.py` & `k8-29.0.8/src/k8/v1_validating_webhook_configuration_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_validation_rule.py` & `k8-29.0.8/src/k8/v1_validation_rule.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_volume.py` & `k8-29.0.8/src/k8/v1_volume.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_volume_attachment.py` & `k8-29.0.8/src/k8/v1_volume_attachment.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_volume_attachment_list.py` & `k8-29.0.8/src/k8/v1_volume_attachment_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_volume_attachment_source.py` & `k8-29.0.8/src/k8/v1_volume_attachment_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_volume_attachment_spec.py` & `k8-29.0.8/src/k8/v1_volume_attachment_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_volume_attachment_status.py` & `k8-29.0.8/src/k8/v1_volume_attachment_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_volume_device.py` & `k8-29.0.8/src/k8/v1_volume_device.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_volume_error.py` & `k8-29.0.8/src/k8/v1_volume_error.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_volume_mount.py` & `k8-29.0.8/src/k8/v1_volume_mount.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_volume_node_affinity.py` & `k8-29.0.8/src/k8/v1_volume_node_affinity.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_volume_node_resources.py` & `k8-29.0.8/src/k8/v1_volume_node_resources.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_volume_projection.py` & `k8-29.0.8/src/k8/v1_volume_projection.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_volume_resource_requirements.py` & `k8-29.0.8/src/k8/v1_volume_resource_requirements.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_vsphere_virtual_disk_volume_source.py` & `k8-29.0.8/src/k8/v1_vsphere_virtual_disk_volume_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_watch_event.py` & `k8-29.0.8/src/k8/v1_watch_event.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_webhook_conversion.py` & `k8-29.0.8/src/k8/v1_webhook_conversion.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_weighted_pod_affinity_term.py` & `k8-29.0.8/src/k8/v1_weighted_pod_affinity_term.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1_windows_security_context_options.py` & `k8-29.0.8/src/k8/v1_windows_security_context_options.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_audit_annotation.py` & `k8-29.0.8/src/k8/v1alpha1_audit_annotation.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_cluster_trust_bundle.py` & `k8-29.0.8/src/k8/v1alpha1_cluster_trust_bundle.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_cluster_trust_bundle_list.py` & `k8-29.0.8/src/k8/v1alpha1_cluster_trust_bundle_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_cluster_trust_bundle_spec.py` & `k8-29.0.8/src/k8/v1alpha1_cluster_trust_bundle_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_expression_warning.py` & `k8-29.0.8/src/k8/v1alpha1_expression_warning.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_ip_address.py` & `k8-29.0.8/src/k8/v1alpha1_ip_address.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_ip_address_list.py` & `k8-29.0.8/src/k8/v1alpha1_ip_address_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_ip_address_spec.py` & `k8-29.0.8/src/k8/v1alpha1_ip_address_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_match_condition.py` & `k8-29.0.8/src/k8/v1alpha1_match_condition.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_match_resources.py` & `k8-29.0.8/src/k8/v1alpha1_match_resources.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_named_rule_with_operations.py` & `k8-29.0.8/src/k8/v1alpha1_named_rule_with_operations.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_param_kind.py` & `k8-29.0.8/src/k8/v1alpha1_param_kind.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_param_ref.py` & `k8-29.0.8/src/k8/v1alpha1_param_ref.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_parent_reference.py` & `k8-29.0.8/src/k8/v1alpha1_parent_reference.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_self_subject_review.py` & `k8-29.0.8/src/k8/v1alpha1_self_subject_review.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_self_subject_review_status.py` & `k8-29.0.8/src/k8/v1alpha1_self_subject_review_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_server_storage_version.py` & `k8-29.0.8/src/k8/v1alpha1_server_storage_version.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_service_cidr.py` & `k8-29.0.8/src/k8/v1alpha1_service_cidr.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_service_cidr_list.py` & `k8-29.0.8/src/k8/v1alpha1_service_cidr_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_service_cidr_spec.py` & `k8-29.0.8/src/k8/v1alpha1_service_cidr_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_service_cidr_status.py` & `k8-29.0.8/src/k8/v1alpha1_service_cidr_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_storage_version.py` & `k8-29.0.8/src/k8/v1alpha1_storage_version.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_storage_version_condition.py` & `k8-29.0.8/src/k8/v1alpha1_storage_version_condition.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_storage_version_list.py` & `k8-29.0.8/src/k8/v1alpha1_storage_version_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_storage_version_status.py` & `k8-29.0.8/src/k8/v1alpha1_storage_version_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_type_checking.py` & `k8-29.0.8/src/k8/v1alpha1_type_checking.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_validating_admission_policy.py` & `k8-29.0.8/src/k8/v1alpha1_validating_admission_policy.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_validating_admission_policy_binding.py` & `k8-29.0.8/src/k8/v1alpha1_validating_admission_policy_binding.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_validating_admission_policy_binding_list.py` & `k8-29.0.8/src/k8/v1alpha1_validating_admission_policy_binding_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_validating_admission_policy_binding_spec.py` & `k8-29.0.8/src/k8/v1alpha1_validating_admission_policy_binding_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_validating_admission_policy_list.py` & `k8-29.0.8/src/k8/v1alpha1_validating_admission_policy_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_validating_admission_policy_spec.py` & `k8-29.0.8/src/k8/v1alpha1_validating_admission_policy_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_validating_admission_policy_status.py` & `k8-29.0.8/src/k8/v1alpha1_validating_admission_policy_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_validation.py` & `k8-29.0.8/src/k8/v1alpha1_validation.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_variable.py` & `k8-29.0.8/src/k8/v1alpha1_variable.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_volume_attributes_class.py` & `k8-29.0.8/src/k8/v1alpha1_volume_attributes_class.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha1_volume_attributes_class_list.py` & `k8-29.0.8/src/k8/v1alpha1_volume_attributes_class_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha2_allocation_result.py` & `k8-29.0.8/src/k8/v1alpha2_allocation_result.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha2_pod_scheduling_context.py` & `k8-29.0.8/src/k8/v1alpha2_pod_scheduling_context.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha2_pod_scheduling_context_list.py` & `k8-29.0.8/src/k8/v1alpha2_pod_scheduling_context_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha2_pod_scheduling_context_spec.py` & `k8-29.0.8/src/k8/v1alpha2_pod_scheduling_context_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha2_pod_scheduling_context_status.py` & `k8-29.0.8/src/k8/v1alpha2_pod_scheduling_context_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha2_resource_claim.py` & `k8-29.0.8/src/k8/v1alpha2_resource_claim.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha2_resource_claim_consumer_reference.py` & `k8-29.0.8/src/k8/v1alpha2_resource_claim_consumer_reference.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha2_resource_claim_list.py` & `k8-29.0.8/src/k8/v1alpha2_resource_claim_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha2_resource_claim_parameters_reference.py` & `k8-29.0.8/src/k8/v1alpha2_resource_claim_parameters_reference.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha2_resource_claim_scheduling_status.py` & `k8-29.0.8/src/k8/v1alpha2_resource_claim_scheduling_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha2_resource_claim_spec.py` & `k8-29.0.8/src/k8/v1alpha2_resource_claim_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha2_resource_claim_status.py` & `k8-29.0.8/src/k8/v1alpha2_resource_claim_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha2_resource_claim_template.py` & `k8-29.0.8/src/k8/v1alpha2_resource_claim_template.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha2_resource_claim_template_list.py` & `k8-29.0.8/src/k8/v1alpha2_resource_claim_template_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha2_resource_claim_template_spec.py` & `k8-29.0.8/src/k8/v1alpha2_resource_claim_template_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha2_resource_class.py` & `k8-29.0.8/src/k8/v1alpha2_resource_class.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha2_resource_class_list.py` & `k8-29.0.8/src/k8/v1alpha2_resource_class_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha2_resource_class_parameters_reference.py` & `k8-29.0.8/src/k8/v1alpha2_resource_class_parameters_reference.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1alpha2_resource_handle.py` & `k8-29.0.8/src/k8/v1alpha2_resource_handle.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta1_audit_annotation.py` & `k8-29.0.8/src/k8/v1beta1_audit_annotation.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta1_expression_warning.py` & `k8-29.0.8/src/k8/v1beta1_expression_warning.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta1_match_condition.py` & `k8-29.0.8/src/k8/v1beta1_match_condition.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta1_match_resources.py` & `k8-29.0.8/src/k8/v1beta1_match_resources.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta1_named_rule_with_operations.py` & `k8-29.0.8/src/k8/v1beta1_named_rule_with_operations.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta1_param_kind.py` & `k8-29.0.8/src/k8/v1beta1_param_kind.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta1_param_ref.py` & `k8-29.0.8/src/k8/v1beta1_param_ref.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta1_self_subject_review.py` & `k8-29.0.8/src/k8/v1beta1_self_subject_review.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta1_self_subject_review_status.py` & `k8-29.0.8/src/k8/v1beta1_self_subject_review_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta1_type_checking.py` & `k8-29.0.8/src/k8/v1beta1_type_checking.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta1_validating_admission_policy.py` & `k8-29.0.8/src/k8/v1beta1_validating_admission_policy.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta1_validating_admission_policy_binding.py` & `k8-29.0.8/src/k8/v1beta1_validating_admission_policy_binding.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta1_validating_admission_policy_binding_list.py` & `k8-29.0.8/src/k8/v1beta1_validating_admission_policy_binding_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta1_validating_admission_policy_binding_spec.py` & `k8-29.0.8/src/k8/v1beta1_validating_admission_policy_binding_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta1_validating_admission_policy_list.py` & `k8-29.0.8/src/k8/v1beta1_validating_admission_policy_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta1_validating_admission_policy_spec.py` & `k8-29.0.8/src/k8/v1beta1_validating_admission_policy_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta1_validating_admission_policy_status.py` & `k8-29.0.8/src/k8/v1beta1_validating_admission_policy_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta1_validation.py` & `k8-29.0.8/src/k8/v1beta1_validation.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta1_variable.py` & `k8-29.0.8/src/k8/v1beta1_variable.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta3_exempt_priority_level_configuration.py` & `k8-29.0.8/src/k8/v1beta3_exempt_priority_level_configuration.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta3_flow_distinguisher_method.py` & `k8-29.0.8/src/k8/v1beta3_flow_distinguisher_method.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta3_flow_schema.py` & `k8-29.0.8/src/k8/v1beta3_flow_schema.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta3_flow_schema_condition.py` & `k8-29.0.8/src/k8/v1beta3_flow_schema_condition.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta3_flow_schema_list.py` & `k8-29.0.8/src/k8/v1beta3_flow_schema_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta3_flow_schema_spec.py` & `k8-29.0.8/src/k8/v1beta3_flow_schema_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta3_flow_schema_status.py` & `k8-29.0.8/src/k8/v1beta3_flow_schema_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta3_group_subject.py` & `k8-29.0.8/src/k8/v1beta3_group_subject.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta3_limit_response.py` & `k8-29.0.8/src/k8/v1beta3_limit_response.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta3_limited_priority_level_configuration.py` & `k8-29.0.8/src/k8/v1beta3_limited_priority_level_configuration.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta3_non_resource_policy_rule.py` & `k8-29.0.8/src/k8/v1beta3_non_resource_policy_rule.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta3_policy_rules_with_subjects.py` & `k8-29.0.8/src/k8/v1beta3_policy_rules_with_subjects.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta3_priority_level_configuration.py` & `k8-29.0.8/src/k8/v1beta3_priority_level_configuration.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta3_priority_level_configuration_condition.py` & `k8-29.0.8/src/k8/v1beta3_priority_level_configuration_condition.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta3_priority_level_configuration_list.py` & `k8-29.0.8/src/k8/v1beta3_priority_level_configuration_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta3_priority_level_configuration_reference.py` & `k8-29.0.8/src/k8/v1beta3_priority_level_configuration_reference.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta3_priority_level_configuration_spec.py` & `k8-29.0.8/src/k8/v1beta3_priority_level_configuration_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta3_priority_level_configuration_status.py` & `k8-29.0.8/src/k8/v1beta3_priority_level_configuration_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta3_queuing_configuration.py` & `k8-29.0.8/src/k8/v1beta3_queuing_configuration.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta3_resource_policy_rule.py` & `k8-29.0.8/src/k8/v1beta3_resource_policy_rule.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta3_service_account_subject.py` & `k8-29.0.8/src/k8/v1beta3_service_account_subject.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta3_subject.py` & `k8-29.0.8/src/k8/v1beta3_subject.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v1beta3_user_subject.py` & `k8-29.0.8/src/k8/v1beta3_user_subject.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v2_container_resource_metric_source.py` & `k8-29.0.8/src/k8/v2_container_resource_metric_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v2_container_resource_metric_status.py` & `k8-29.0.8/src/k8/v2_container_resource_metric_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v2_cross_version_object_reference.py` & `k8-29.0.8/src/k8/v2_cross_version_object_reference.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v2_external_metric_source.py` & `k8-29.0.8/src/k8/v2_external_metric_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v2_external_metric_status.py` & `k8-29.0.8/src/k8/v2_external_metric_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v2_horizontal_pod_autoscaler.py` & `k8-29.0.8/src/k8/v2_horizontal_pod_autoscaler.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v2_horizontal_pod_autoscaler_behavior.py` & `k8-29.0.8/src/k8/v2_horizontal_pod_autoscaler_behavior.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v2_horizontal_pod_autoscaler_condition.py` & `k8-29.0.8/src/k8/v2_horizontal_pod_autoscaler_condition.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v2_horizontal_pod_autoscaler_list.py` & `k8-29.0.8/src/k8/v2_horizontal_pod_autoscaler_list.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v2_horizontal_pod_autoscaler_spec.py` & `k8-29.0.8/src/k8/v2_horizontal_pod_autoscaler_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v2_horizontal_pod_autoscaler_status.py` & `k8-29.0.8/src/k8/v2_horizontal_pod_autoscaler_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v2_hpa_scaling_policy.py` & `k8-29.0.8/src/k8/v2_hpa_scaling_policy.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v2_hpa_scaling_rules.py` & `k8-29.0.8/src/k8/v2_hpa_scaling_rules.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v2_metric_identifier.py` & `k8-29.0.8/src/k8/v2_metric_identifier.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v2_metric_spec.py` & `k8-29.0.8/src/k8/v2_metric_spec.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v2_metric_status.py` & `k8-29.0.8/src/k8/v2_metric_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v2_metric_target.py` & `k8-29.0.8/src/k8/v2_metric_target.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v2_metric_value_status.py` & `k8-29.0.8/src/k8/v2_metric_value_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v2_object_metric_source.py` & `k8-29.0.8/src/k8/v2_object_metric_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v2_object_metric_status.py` & `k8-29.0.8/src/k8/v2_object_metric_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v2_pods_metric_source.py` & `k8-29.0.8/src/k8/v2_pods_metric_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v2_pods_metric_status.py` & `k8-29.0.8/src/k8/v2_pods_metric_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v2_resource_metric_source.py` & `k8-29.0.8/src/k8/v2_resource_metric_source.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/v2_resource_metric_status.py` & `k8-29.0.8/src/k8/v2_resource_metric_status.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8/version_info.py` & `k8-29.0.8/src/k8/version_info.py`

 * *Files identical despite different names*

### Comparing `k8-29.0.7/src/k8.egg-info/PKG-INFO` & `k8-29.0.8/src/k8.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k8
-Version: 29.0.7
+Version: 29.0.8
 Summary: Kubernetes Python Models
 Author-email: Nick Cooper <nick@not.fun>
 Project-URL: Homepage, https://github.com/nicknotfun/k8
 Project-URL: Issues, https://github.com/nicknotfun/k8/issues
 Keywords: OpenAPI,OpenAPI-Generator,Kubernetes
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `k8-29.0.7/src/k8.egg-info/SOURCES.txt` & `k8-29.0.8/src/k8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

