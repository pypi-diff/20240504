# Comparing `tmp/koku-nise-4.4.8.tar.gz` & `tmp/koku-nise-4.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koku-nise-4.4.8.tar", last modified: Tue Nov 14 14:22:42 2023, max compression
+gzip compressed data, was "koku-nise-4.4.9.tar", last modified: Wed Nov 15 11:12:26 2023, max compression
```

## Comparing `koku-nise-4.4.8.tar` & `koku-nise-4.4.9.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:22:42.196024 koku-nise-4.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)    34520 2023-11-14 14:22:26.000000 koku-nise-4.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-11-14 14:22:26.000000 koku-nise-4.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      464 2023-11-14 14:22:42.196024 koku-nise-4.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9834 2023-11-14 14:22:26.000000 koku-nise-4.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:22:42.184024 koku-nise-4.4.8/koku_nise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2023-11-14 14:22:41.000000 koku-nise-4.4.8/koku_nise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2023-11-14 14:22:42.000000 koku-nise-4.4.8/koku_nise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 14:22:41.000000 koku-nise-4.4.8/koku_nise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-11-14 14:22:41.000000 koku-nise-4.4.8/koku_nise.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 14:22:41.000000 koku-nise-4.4.8/koku_nise.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      156 2023-11-14 14:22:41.000000 koku-nise-4.4.8/koku_nise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-14 14:22:41.000000 koku-nise-4.4.8/koku_nise.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:22:42.184024 koku-nise-4.4.8/nise/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28663 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/aws-template-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:22:42.188024 koku-nise-4.4.8/nise/generators/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:22:42.188024 koku-nise-4.4.8/nise/generators/aws/
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/aws/aws_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    13391 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/aws/aws_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5659 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/aws/data_transfer_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/aws/ebs_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6905 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/aws/ec2_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7315 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/aws/marketplace_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6495 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/aws/rds_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/aws/route53_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4009 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/aws/s3_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/aws/vpc_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:22:42.188024 koku-nise-4.4.8/nise/generators/azure/
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16623 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/azure/azure_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/azure/bandwidth_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/azure/ccsp_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/azure/sql_database_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/azure/storage_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/azure/virtual_machine_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/azure/virtual_network_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:22:42.192024 koku-nise-4.4.8/nise/generators/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7594 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/gcp/cloud_storage_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9603 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/gcp/compute_engine_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7860 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/gcp/gcp_database_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11867 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/gcp/gcp_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8099 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/gcp/gcp_network_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/gcp/hcs_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/gcp/project_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5287 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:22:42.192024 koku-nise-4.4.8/nise/generators/oci/
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/oci/oci_block_storage_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/oci/oci_compute_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/oci/oci_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/oci/oci_database_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10817 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/oci/oci_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/oci/oci_network_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:22:42.192024 koku-nise-4.4.8/nise/generators/ocp/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/ocp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40379 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/generators/ocp/ocp_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    55930 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/report.py
--rw-r--r--   0 runner    (1001) docker     (127)    15635 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:22:42.192024 koku-nise-4.4.8/nise/util/
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/util/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     7688 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_gen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:22:42.192024 koku-nise-4.4.8/nise/yaml_generators/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:22:42.192024 koku-nise-4.4.8/nise/yaml_generators/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_generators/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    71376 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_generators/aws/ec2_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     9814 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_generators/aws/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13953 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_generators/aws/rds_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_generators/aws/regions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:22:42.192024 koku-nise-4.4.8/nise/yaml_generators/azure/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_generators/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7923 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_generators/azure/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:22:42.192024 koku-nise-4.4.8/nise/yaml_generators/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_generators/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_generators/gcp/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_generators/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:22:42.196024 koku-nise-4.4.8/nise/yaml_generators/oci/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_generators/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5636 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_generators/oci/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_generators/oci/oci_yaml_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:22:42.196024 koku-nise-4.4.8/nise/yaml_generators/ocp/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_generators/ocp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12882 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_generators/ocp/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:22:42.196024 koku-nise-4.4.8/nise/yaml_generators/ocp_on_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_generators/ocp_on_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_generators/ocp_on_cloud/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:22:42.196024 koku-nise-4.4.8/nise/yaml_generators/static/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_generators/static/aws_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_generators/static/aws_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      537 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_generators/static/azure_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_generators/static/azure_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      403 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_generators/static/gcp_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_generators/static/gcp_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      484 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_generators/static/oci_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_generators/static/oci_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      896 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_generators/static/ocp_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      595 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_generators/static/ocp_on_cloud_options.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_generators/static/ocp_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2023-11-14 14:22:26.000000 koku-nise-4.4.8/nise/yaml_generators/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 14:22:42.196024 koku-nise-4.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2023-11-14 14:22:26.000000 koku-nise-4.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.459130 koku-nise-4.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2023-11-15 11:12:08.000000 koku-nise-4.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2023-11-15 11:12:08.000000 koku-nise-4.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2023-11-15 11:12:26.459130 koku-nise-4.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9834 2023-11-15 11:12:08.000000 koku-nise-4.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.451130 koku-nise-4.4.9/koku_nise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2023-11-15 11:12:26.000000 koku-nise-4.4.9/koku_nise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2023-11-15 11:12:26.000000 koku-nise-4.4.9/koku_nise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-15 11:12:26.000000 koku-nise-4.4.9/koku_nise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2023-11-15 11:12:26.000000 koku-nise-4.4.9/koku_nise.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-15 11:12:26.000000 koku-nise-4.4.9/koku_nise.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2023-11-15 11:12:26.000000 koku-nise-4.4.9/koku_nise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-15 11:12:26.000000 koku-nise-4.4.9/koku_nise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.451130 koku-nise-4.4.9/nise/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28577 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/aws-template-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.451130 koku-nise-4.4.9/nise/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.451130 koku-nise-4.4.9/nise/generators/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/aws/aws_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13391 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/aws/aws_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5659 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/aws/data_transfer_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/aws/ebs_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6905 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/aws/ec2_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7315 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/aws/marketplace_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6495 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/aws/rds_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/aws/route53_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4009 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/aws/s3_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/aws/vpc_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.455130 koku-nise-4.4.9/nise/generators/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16623 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/azure/azure_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/azure/bandwidth_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/azure/ccsp_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/azure/sql_database_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/azure/storage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/azure/virtual_machine_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/azure/virtual_network_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.455130 koku-nise-4.4.9/nise/generators/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/gcp/cloud_storage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9603 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/gcp/compute_engine_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7860 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/gcp/gcp_database_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11867 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/gcp/gcp_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8099 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/gcp/gcp_network_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/gcp/hcs_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/gcp/project_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.455130 koku-nise-4.4.9/nise/generators/oci/
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/oci/oci_block_storage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/oci/oci_compute_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/oci/oci_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/oci/oci_database_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10817 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/oci/oci_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/oci/oci_network_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.455130 koku-nise-4.4.9/nise/generators/ocp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/ocp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40379 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/generators/ocp/ocp_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55930 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15635 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.455130 koku-nise-4.4.9/nise/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/util/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7688 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.455130 koku-nise-4.4.9/nise/yaml_generators/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.455130 koku-nise-4.4.9/nise/yaml_generators/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71376 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/aws/ec2_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9814 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/aws/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13953 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/aws/rds_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/aws/regions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.455130 koku-nise-4.4.9/nise/yaml_generators/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7923 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/azure/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.459130 koku-nise-4.4.9/nise/yaml_generators/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/gcp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.459130 koku-nise-4.4.9/nise/yaml_generators/oci/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/oci/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/oci/oci_yaml_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.459130 koku-nise-4.4.9/nise/yaml_generators/ocp/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/ocp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12882 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/ocp/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.459130 koku-nise-4.4.9/nise/yaml_generators/ocp_on_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/ocp_on_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/ocp_on_cloud/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 11:12:26.459130 koku-nise-4.4.9/nise/yaml_generators/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/static/aws_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/static/aws_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/static/azure_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/static/azure_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/static/gcp_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/static/gcp_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/static/oci_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/static/oci_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/static/ocp_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/static/ocp_on_cloud_options.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/static/ocp_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2023-11-15 11:12:08.000000 koku-nise-4.4.9/nise/yaml_generators/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-15 11:12:26.459130 koku-nise-4.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2023-11-15 11:12:08.000000 koku-nise-4.4.9/setup.py
```

### Comparing `koku-nise-4.4.8/LICENSE` & `koku-nise-4.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/README.md` & `koku-nise-4.4.9/README.md`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/koku_nise.egg-info/SOURCES.txt` & `koku-nise-4.4.9/koku_nise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/__main__.py` & `koku-nise-4.4.9/nise/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -738,15 +738,15 @@
 def calculate_start_date(start_date):
     """Return a datetime for the start date."""
     if start_date == "last_month":
         generated_start_date = today().replace(day=1, hour=0, minute=0, second=0) + relativedelta(months=-1)
     elif start_date == "today":
         generated_start_date = today().replace(hour=0, minute=0, second=0)
     elif start_date and isinstance(start_date, datetime.date):
-        generated_start_date = datetime.datetime.fromordinal(start_date.toordinal())
+        generated_start_date = start_date
     elif start_date:
         generated_start_date = date_parser.parse(start_date)
     else:
         generated_start_date = today().replace(day=1, hour=0, minute=0, second=0)
     if generated_start_date.tzinfo is None:
         generated_start_date = generated_start_date.replace(tzinfo=timezone.utc)
     return generated_start_date
@@ -756,15 +756,15 @@
     """Return a datetime for the end date."""
     try:
         if end_date == "last_month":
             generated_end_date = today().replace(day=1, hour=0, minute=0, second=0) + relativedelta(months=-1)
         elif end_date == "today":
             generated_end_date = today().replace(hour=0, minute=0, second=0)
         elif end_date and isinstance(end_date, datetime.date):
-            generated_end_date = datetime.datetime.fromordinal(end_date.toordinal())
+            generated_end_date = end_date
         else:
             generated_end_date = date_parser.parse(end_date)
     except TypeError:
         offset = end_date
         offset_date = start_date + relativedelta(days=offset)
         if offset_date.month > start_date.month:
             generated_end_date = offset_date
```

### Comparing `koku-nise-4.4.8/nise/aws-template-manifest.json` & `koku-nise-4.4.9/nise/aws-template-manifest.json`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/copy.py` & `koku-nise-4.4.9/nise/copy.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/extract.py` & `koku-nise-4.4.9/nise/extract.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/aws/__init__.py` & `koku-nise-4.4.9/nise/generators/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/aws/aws_constants.py` & `koku-nise-4.4.9/nise/generators/aws/aws_constants.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/aws/aws_generator.py` & `koku-nise-4.4.9/nise/generators/aws/aws_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/aws/data_transfer_generator.py` & `koku-nise-4.4.9/nise/generators/aws/data_transfer_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/aws/ebs_generator.py` & `koku-nise-4.4.9/nise/generators/aws/ebs_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/aws/ec2_generator.py` & `koku-nise-4.4.9/nise/generators/aws/ec2_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/aws/marketplace_generator.py` & `koku-nise-4.4.9/nise/generators/aws/marketplace_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/aws/rds_generator.py` & `koku-nise-4.4.9/nise/generators/aws/rds_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/aws/route53_generator.py` & `koku-nise-4.4.9/nise/generators/aws/route53_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/aws/s3_generator.py` & `koku-nise-4.4.9/nise/generators/aws/s3_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/aws/vpc_generator.py` & `koku-nise-4.4.9/nise/generators/aws/vpc_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/azure/__init__.py` & `koku-nise-4.4.9/nise/generators/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/azure/azure_generator.py` & `koku-nise-4.4.9/nise/generators/azure/azure_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/azure/bandwidth_generator.py` & `koku-nise-4.4.9/nise/generators/azure/bandwidth_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/azure/ccsp_generator.py` & `koku-nise-4.4.9/nise/generators/azure/ccsp_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/azure/sql_database_generator.py` & `koku-nise-4.4.9/nise/generators/azure/sql_database_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/azure/storage_generator.py` & `koku-nise-4.4.9/nise/generators/azure/storage_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/azure/virtual_machine_generator.py` & `koku-nise-4.4.9/nise/generators/azure/virtual_machine_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/azure/virtual_network_generator.py` & `koku-nise-4.4.9/nise/generators/azure/virtual_network_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/gcp/__init__.py` & `koku-nise-4.4.9/nise/generators/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/gcp/cloud_storage_generator.py` & `koku-nise-4.4.9/nise/generators/gcp/cloud_storage_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/gcp/compute_engine_generator.py` & `koku-nise-4.4.9/nise/generators/gcp/compute_engine_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/gcp/gcp_database_generator.py` & `koku-nise-4.4.9/nise/generators/gcp/gcp_database_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/gcp/gcp_generator.py` & `koku-nise-4.4.9/nise/generators/gcp/gcp_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/gcp/gcp_network_generator.py` & `koku-nise-4.4.9/nise/generators/gcp/gcp_network_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/gcp/hcs_generator.py` & `koku-nise-4.4.9/nise/generators/gcp/hcs_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/gcp/project_generator.py` & `koku-nise-4.4.9/nise/generators/gcp/project_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/generator.py` & `koku-nise-4.4.9/nise/generators/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/oci/__init__.py` & `koku-nise-4.4.9/nise/generators/oci/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/oci/oci_block_storage_generator.py` & `koku-nise-4.4.9/nise/generators/oci/oci_block_storage_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/oci/oci_compute_generator.py` & `koku-nise-4.4.9/nise/generators/oci/oci_compute_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/oci/oci_constants.py` & `koku-nise-4.4.9/nise/generators/oci/oci_constants.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/oci/oci_database_generator.py` & `koku-nise-4.4.9/nise/generators/oci/oci_database_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/oci/oci_generator.py` & `koku-nise-4.4.9/nise/generators/oci/oci_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/oci/oci_network_generator.py` & `koku-nise-4.4.9/nise/generators/oci/oci_network_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/ocp/__init__.py` & `koku-nise-4.4.9/nise/generators/ocp/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/generators/ocp/ocp_generator.py` & `koku-nise-4.4.9/nise/generators/ocp/ocp_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/manifest.py` & `koku-nise-4.4.9/nise/manifest.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/report.py` & `koku-nise-4.4.9/nise/report.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/upload.py` & `koku-nise-4.4.9/nise/upload.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/util/__init__.py` & `koku-nise-4.4.9/nise/util/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/util/log.py` & `koku-nise-4.4.9/nise/util/log.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/yaml_gen.py` & `koku-nise-4.4.9/nise/yaml_gen.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/yaml_generators/aws/ec2_instance_types.py` & `koku-nise-4.4.9/nise/yaml_generators/aws/ec2_instance_types.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/yaml_generators/aws/generator.py` & `koku-nise-4.4.9/nise/yaml_generators/aws/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/yaml_generators/aws/rds_instance_types.py` & `koku-nise-4.4.9/nise/yaml_generators/aws/rds_instance_types.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/yaml_generators/aws/regions.py` & `koku-nise-4.4.9/nise/yaml_generators/aws/regions.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/yaml_generators/azure/generator.py` & `koku-nise-4.4.9/nise/yaml_generators/azure/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/yaml_generators/gcp/generator.py` & `koku-nise-4.4.9/nise/yaml_generators/gcp/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/yaml_generators/generator.py` & `koku-nise-4.4.9/nise/yaml_generators/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/yaml_generators/oci/generator.py` & `koku-nise-4.4.9/nise/yaml_generators/oci/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/yaml_generators/oci/oci_yaml_constants.py` & `koku-nise-4.4.9/nise/yaml_generators/oci/oci_yaml_constants.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/yaml_generators/ocp/generator.py` & `koku-nise-4.4.9/nise/yaml_generators/ocp/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/yaml_generators/ocp_on_cloud/generator.py` & `koku-nise-4.4.9/nise/yaml_generators/ocp_on_cloud/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/yaml_generators/static/aws_generator_config.yml` & `koku-nise-4.4.9/nise/yaml_generators/static/aws_generator_config.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/yaml_generators/static/aws_static_data.yml.j2` & `koku-nise-4.4.9/nise/yaml_generators/static/aws_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/yaml_generators/static/azure_generator_config.yml` & `koku-nise-4.4.9/nise/yaml_generators/static/azure_generator_config.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/yaml_generators/static/azure_static_data.yml.j2` & `koku-nise-4.4.9/nise/yaml_generators/static/azure_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/yaml_generators/static/gcp_static_data.yml.j2` & `koku-nise-4.4.9/nise/yaml_generators/static/gcp_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/yaml_generators/static/oci_static_data.yml.j2` & `koku-nise-4.4.9/nise/yaml_generators/static/oci_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/yaml_generators/static/ocp_generator_config.yml` & `koku-nise-4.4.9/nise/yaml_generators/static/ocp_generator_config.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/yaml_generators/static/ocp_on_cloud_options.yml` & `koku-nise-4.4.9/nise/yaml_generators/static/ocp_on_cloud_options.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/yaml_generators/static/ocp_static_data.yml.j2` & `koku-nise-4.4.9/nise/yaml_generators/static/ocp_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/nise/yaml_generators/utils.py` & `koku-nise-4.4.9/nise/yaml_generators/utils.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.4.8/setup.py` & `koku-nise-4.4.9/setup.py`

 * *Files identical despite different names*

