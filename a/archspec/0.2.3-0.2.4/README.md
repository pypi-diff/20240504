# Comparing `tmp/archspec-0.2.3.tar.gz` & `tmp/archspec-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archspec-0.2.3.tar", max compression
+gzip compressed data, was "archspec-0.2.4.tar", max compression
```

## Comparing `archspec-0.2.3.tar` & `archspec-0.2.4.tar`

### file list

```diff
@@ -1,71 +1,74 @@
--rw-r--r--   0        0        0    11358 2021-09-03 15:23:36.189003 archspec-0.2.3/LICENSE-APACHE
--rw-r--r--   0        0        0     1171 2021-09-03 15:23:36.189003 archspec-0.2.3/LICENSE-MIT
--rw-r--r--   0        0        0     3104 2022-10-20 07:06:28.800541 archspec-0.2.3/README.md
--rw-r--r--   0        0        0       67 2024-02-26 10:47:40.035871 archspec-0.2.3/archspec/__init__.py
--rw-r--r--   0        0        0       97 2024-02-17 09:38:08.416723 archspec-0.2.3/archspec/__main__.py
--rwxr-xr-x   0        0        0     1691 2024-02-26 10:17:51.649680 archspec-0.2.3/archspec/cli.py
--rw-r--r--   0        0        0      635 2024-02-17 09:38:08.416723 archspec-0.2.3/archspec/cpu/__init__.py
--rw-r--r--   0        0        0     2506 2023-09-27 11:46:20.510353 archspec-0.2.3/archspec/cpu/alias.py
--rw-r--r--   0        0        0    14847 2024-02-17 09:38:08.416723 archspec-0.2.3/archspec/cpu/detect.py
--rw-r--r--   0        0        0    13508 2024-02-18 16:13:21.673941 archspec-0.2.3/archspec/cpu/microarchitecture.py
--rw-r--r--   0        0        0     3687 2024-02-26 10:17:51.649680 archspec-0.2.3/archspec/cpu/schema.py
--rw-r--r--   0        0        0      805 2021-09-03 15:23:36.888990 archspec-0.2.3/archspec/json/COPYRIGHT
--rw-r--r--   0        0        0    11358 2021-09-03 15:23:36.888990 archspec-0.2.3/archspec/json/LICENSE-APACHE
--rw-r--r--   0        0        0     1171 2021-09-03 15:23:36.888990 archspec-0.2.3/archspec/json/LICENSE-MIT
--rw-r--r--   0        0        0     1167 2021-09-03 15:23:36.888990 archspec-0.2.3/archspec/json/NOTICE
--rw-r--r--   0        0        0     1531 2024-02-17 08:15:12.265169 archspec-0.2.3/archspec/json/README.md
--rw-r--r--   0        0        0    20572 2024-02-17 07:44:40.246457 archspec-0.2.3/archspec/json/cpu/cpuid.json
--rw-r--r--   0        0        0     3129 2024-02-17 07:44:40.246457 archspec-0.2.3/archspec/json/cpu/cpuid_schema.json
--rw-r--r--   0        0        0    81400 2024-02-15 14:48:47.181584 archspec-0.2.3/archspec/json/cpu/microarchitectures.json
--rw-r--r--   0        0        0     2955 2024-02-15 14:48:47.181584 archspec-0.2.3/archspec/json/cpu/microarchitectures_schema.json
--rw-r--r--   0        0        0      116 2021-09-03 15:23:36.888990 archspec-0.2.3/archspec/json/tests/targets/bgq-rhel6-power7
--rw-r--r--   0        0        0      534 2021-10-22 10:17:21.472678 archspec-0.2.3/archspec/json/tests/targets/darwin-bigsur-m1
--rw-r--r--   0        0        0      553 2024-02-14 21:23:18.209438 archspec-0.2.3/archspec/json/tests/targets/darwin-mojave-haswell
--rw-r--r--   0        0        0     2356 2021-09-03 15:23:36.888990 archspec-0.2.3/archspec/json/tests/targets/darwin-mojave-ivybridge
--rw-r--r--   0        0        0      598 2024-02-14 21:23:21.929404 archspec-0.2.3/archspec/json/tests/targets/darwin-mojave-skylake
--rw-r--r--   0        0        0     3307 2022-06-06 17:01:35.566636 archspec-0.2.3/archspec/json/tests/targets/darwin-monterey-m1
--rw-r--r--   0        0        0     3307 2022-10-20 11:44:43.351413 archspec-0.2.3/archspec/json/tests/targets/darwin-monterey-m2
--rw-r--r--   0        0        0      221 2022-10-20 07:05:46.605297 archspec-0.2.3/archspec/json/tests/targets/linux-amazon-cortex_a72
--rw-r--r--   0        0        0      276 2022-10-20 07:05:46.605297 archspec-0.2.3/archspec/json/tests/targets/linux-amazon-neoverse_n1
--rw-r--r--   0        0        0      361 2022-10-20 07:05:46.605297 archspec-0.2.3/archspec/json/tests/targets/linux-amazon-neoverse_v1
--rw-r--r--   0        0        0     1519 2023-11-06 16:40:45.253781 archspec-0.2.3/archspec/json/tests/targets/linux-amazon2-sapphirerapids
--rw-r--r--   0        0        0      363 2022-06-06 17:01:35.566636 archspec-0.2.3/archspec/json/tests/targets/linux-asahi-m1
--rw-r--r--   0        0        0      381 2022-10-20 11:44:43.351413 archspec-0.2.3/archspec/json/tests/targets/linux-asahi-m2
--rw-r--r--   0        0        0     1408 2021-09-03 15:23:36.888990 archspec-0.2.3/archspec/json/tests/targets/linux-centos7-cascadelake
--rw-r--r--   0        0        0      111 2021-09-03 15:23:36.888990 archspec-0.2.3/archspec/json/tests/targets/linux-centos7-power8le
--rw-r--r--   0        0        0      238 2021-09-03 15:23:36.888990 archspec-0.2.3/archspec/json/tests/targets/linux-centos7-thunderx2
--rw-r--r--   0        0        0     1411 2021-09-03 15:23:36.888990 archspec-0.2.3/archspec/json/tests/targets/linux-rhel6-piledriver
--rw-r--r--   0        0        0     1187 2021-09-03 15:23:36.888990 archspec-0.2.3/archspec/json/tests/targets/linux-rhel7-broadwell
--rw-r--r--   0        0        0     1095 2021-09-03 15:23:36.888990 archspec-0.2.3/archspec/json/tests/targets/linux-rhel7-haswell
--rw-r--r--   0        0        0     1009 2021-09-03 15:23:36.888990 archspec-0.2.3/archspec/json/tests/targets/linux-rhel7-ivybridge
--rw-r--r--   0        0        0     1286 2021-09-03 15:23:36.888990 archspec-0.2.3/archspec/json/tests/targets/linux-rhel7-skylake_avx512
--rw-r--r--   0        0        0     1172 2021-10-22 10:17:21.472678 archspec-0.2.3/archspec/json/tests/targets/linux-rhel7-x86_64_v3
--rw-r--r--   0        0        0     1319 2021-09-03 15:23:36.888990 archspec-0.2.3/archspec/json/tests/targets/linux-rhel7-zen
--rw-r--r--   0        0        0      135 2023-11-06 16:40:45.253781 archspec-0.2.3/archspec/json/tests/targets/linux-rhel8-power9
--rw-r--r--   0        0        0      256 2023-11-06 16:40:45.253781 archspec-0.2.3/archspec/json/tests/targets/linux-rocky8-a64fx
--rw-r--r--   0        0        0     1750 2023-11-06 16:40:45.253781 archspec-0.2.3/archspec/json/tests/targets/linux-rocky8.5-zen4
--rw-r--r--   0        0        0     1111 2021-09-03 15:23:36.888990 archspec-0.2.3/archspec/json/tests/targets/linux-scientific7-k10
--rw-r--r--   0        0        0     1149 2021-09-03 15:23:36.888990 archspec-0.2.3/archspec/json/tests/targets/linux-scientific7-piledriver
--rw-r--r--   0        0        0     1201 2021-09-03 15:23:36.888990 archspec-0.2.3/archspec/json/tests/targets/linux-scientificfermi6-bulldozer
--rw-r--r--   0        0        0     1099 2021-09-03 15:23:36.888990 archspec-0.2.3/archspec/json/tests/targets/linux-scientificfermi6-piledriver
--rw-r--r--   0        0        0      124 2021-10-22 10:17:21.472678 archspec-0.2.3/archspec/json/tests/targets/linux-sifive-u74mc
--rw-r--r--   0        0        0     1190 2021-09-03 15:23:36.888990 archspec-0.2.3/archspec/json/tests/targets/linux-ubuntu18.04-broadwell
--rw-r--r--   0        0        0     1531 2021-10-22 10:17:21.472678 archspec-0.2.3/archspec/json/tests/targets/linux-ubuntu20.04-zen3
--rw-r--r--   0        0        0      458 2023-11-06 16:40:45.253781 archspec-0.2.3/archspec/json/tests/targets/linux-ubuntu22.04-neoverse_v2
--rw-r--r--   0        0        0       83 2023-11-06 16:40:45.253781 archspec-0.2.3/archspec/json/tests/targets/linux-unknown-power10
--rw-r--r--   0        0        0     2187 2023-11-06 16:40:45.257781 archspec-0.2.3/archspec/json/tests/targets/linux-unknown-sapphirerapids
--rw-r--r--   0        0        0      231 2024-02-17 07:44:40.246457 archspec-0.2.3/archspec/json/tests/targets/windows-cpuid-broadwell
--rw-r--r--   0        0        0      254 2024-02-17 08:15:12.265169 archspec-0.2.3/archspec/json/tests/targets/windows-cpuid-icelake
--rw-r--r--   0        0        0       52 2024-02-15 22:06:34.808307 archspec-0.2.3/archspec/vendor/cpuid/.git
--rw-r--r--   0        0        0       12 2024-02-15 22:06:34.856307 archspec-0.2.3/archspec/vendor/cpuid/.gitignore
--rw-r--r--   0        0        0     1079 2024-02-15 22:06:34.856307 archspec-0.2.3/archspec/vendor/cpuid/LICENSE
--rw-r--r--   0        0        0     2400 2024-02-15 22:06:34.856307 archspec-0.2.3/archspec/vendor/cpuid/README.md
--rw-r--r--   0        0        0     6037 2024-02-17 07:41:48.471224 archspec-0.2.3/archspec/vendor/cpuid/cpuid.py
--rw-r--r--   0        0        0     1855 2024-02-15 22:09:02.081631 archspec-0.2.3/archspec/vendor/cpuid/example.py
--rw-r--r--   0        0        0     2119 2024-02-26 10:47:40.035871 archspec-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      200 2021-09-03 15:23:36.193003 archspec-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0     1678 2024-02-26 10:17:51.649680 archspec-0.2.3/tests/conftest.py
--rw-r--r--   0        0        0      393 2024-02-26 10:47:40.035871 archspec-0.2.3/tests/test_archspec.py
--rw-r--r--   0        0        0     1217 2024-02-26 10:17:51.649680 archspec-0.2.3/tests/test_cli.py
--rw-r--r--   0        0        0    16325 2024-02-26 10:17:51.649680 archspec-0.2.3/tests/test_cpu.py
--rw-r--r--   0        0        0     4375 1970-01-01 00:00:00.000000 archspec-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11358 2021-09-03 15:23:36.189003 archspec-0.2.4/LICENSE-APACHE
+-rw-r--r--   0        0        0     1171 2021-09-03 15:23:36.189003 archspec-0.2.4/LICENSE-MIT
+-rw-r--r--   0        0        0     1167 2021-09-03 15:23:36.189003 archspec-0.2.4/NOTICE
+-rw-r--r--   0        0        0     3104 2022-10-20 07:06:28.800541 archspec-0.2.4/README.md
+-rw-r--r--   0        0        0       67 2024-05-04 13:38:32.138207 archspec-0.2.4/archspec/__init__.py
+-rw-r--r--   0        0        0       97 2024-02-17 09:38:08.416723 archspec-0.2.4/archspec/__main__.py
+-rwxr-xr-x   0        0        0     1691 2024-02-26 10:17:51.649680 archspec-0.2.4/archspec/cli.py
+-rw-r--r--   0        0        0      727 2024-03-19 06:41:00.324097 archspec-0.2.4/archspec/cpu/__init__.py
+-rw-r--r--   0        0        0     2506 2023-09-27 11:46:20.510353 archspec-0.2.4/archspec/cpu/alias.py
+-rw-r--r--   0        0        0    15954 2024-03-18 06:18:01.649909 archspec-0.2.4/archspec/cpu/detect.py
+-rw-r--r--   0        0        0    14361 2024-05-04 13:16:20.869021 archspec-0.2.4/archspec/cpu/microarchitecture.py
+-rw-r--r--   0        0        0     3687 2024-02-26 10:17:51.649680 archspec-0.2.4/archspec/cpu/schema.py
+-rw-r--r--   0        0        0      805 2021-09-03 15:23:36.888990 archspec-0.2.4/archspec/json/COPYRIGHT
+-rw-r--r--   0        0        0    11358 2021-09-03 15:23:36.888990 archspec-0.2.4/archspec/json/LICENSE-APACHE
+-rw-r--r--   0        0        0     1171 2021-09-03 15:23:36.888990 archspec-0.2.4/archspec/json/LICENSE-MIT
+-rw-r--r--   0        0        0     1167 2021-09-03 15:23:36.888990 archspec-0.2.4/archspec/json/NOTICE
+-rw-r--r--   0        0        0     1531 2024-02-17 08:15:12.265169 archspec-0.2.4/archspec/json/README.md
+-rw-r--r--   0        0        0    20572 2024-02-17 07:44:40.246457 archspec-0.2.4/archspec/json/cpu/cpuid.json
+-rw-r--r--   0        0        0     3129 2024-02-17 07:44:40.246457 archspec-0.2.4/archspec/json/cpu/cpuid_schema.json
+-rw-r--r--   0        0        0    81332 2024-03-19 06:53:55.122972 archspec-0.2.4/archspec/json/cpu/microarchitectures.json
+-rw-r--r--   0        0        0     2955 2024-02-15 14:48:47.181584 archspec-0.2.4/archspec/json/cpu/microarchitectures_schema.json
+-rw-r--r--   0        0        0      116 2021-09-03 15:23:36.888990 archspec-0.2.4/archspec/json/tests/targets/bgq-rhel6-power7
+-rw-r--r--   0        0        0      534 2021-10-22 10:17:21.472678 archspec-0.2.4/archspec/json/tests/targets/darwin-bigsur-m1
+-rw-r--r--   0        0        0      553 2024-02-14 21:23:18.209438 archspec-0.2.4/archspec/json/tests/targets/darwin-mojave-haswell
+-rw-r--r--   0        0        0     2356 2021-09-03 15:23:36.888990 archspec-0.2.4/archspec/json/tests/targets/darwin-mojave-ivybridge
+-rw-r--r--   0        0        0      598 2024-02-14 21:23:21.929404 archspec-0.2.4/archspec/json/tests/targets/darwin-mojave-skylake
+-rw-r--r--   0        0        0     3307 2022-06-06 17:01:35.566636 archspec-0.2.4/archspec/json/tests/targets/darwin-monterey-m1
+-rw-r--r--   0        0        0     3307 2022-10-20 11:44:43.351413 archspec-0.2.4/archspec/json/tests/targets/darwin-monterey-m2
+-rw-r--r--   0        0        0      221 2022-10-20 07:05:46.605297 archspec-0.2.4/archspec/json/tests/targets/linux-amazon-cortex_a72
+-rw-r--r--   0        0        0      276 2022-10-20 07:05:46.605297 archspec-0.2.4/archspec/json/tests/targets/linux-amazon-neoverse_n1
+-rw-r--r--   0        0        0      361 2022-10-20 07:05:46.605297 archspec-0.2.4/archspec/json/tests/targets/linux-amazon-neoverse_v1
+-rw-r--r--   0        0        0     1519 2023-11-06 16:40:45.253781 archspec-0.2.4/archspec/json/tests/targets/linux-amazon2-sapphirerapids
+-rw-r--r--   0        0        0      363 2022-06-06 17:01:35.566636 archspec-0.2.4/archspec/json/tests/targets/linux-asahi-m1
+-rw-r--r--   0        0        0      381 2022-10-20 11:44:43.351413 archspec-0.2.4/archspec/json/tests/targets/linux-asahi-m2
+-rw-r--r--   0        0        0     1408 2021-09-03 15:23:36.888990 archspec-0.2.4/archspec/json/tests/targets/linux-centos7-cascadelake
+-rw-r--r--   0        0        0      111 2021-09-03 15:23:36.888990 archspec-0.2.4/archspec/json/tests/targets/linux-centos7-power8le
+-rw-r--r--   0        0        0      238 2021-09-03 15:23:36.888990 archspec-0.2.4/archspec/json/tests/targets/linux-centos7-thunderx2
+-rw-r--r--   0        0        0     1411 2021-09-03 15:23:36.888990 archspec-0.2.4/archspec/json/tests/targets/linux-rhel6-piledriver
+-rw-r--r--   0        0        0     1187 2021-09-03 15:23:36.888990 archspec-0.2.4/archspec/json/tests/targets/linux-rhel7-broadwell
+-rw-r--r--   0        0        0     1095 2021-09-03 15:23:36.888990 archspec-0.2.4/archspec/json/tests/targets/linux-rhel7-haswell
+-rw-r--r--   0        0        0     1009 2021-09-03 15:23:36.888990 archspec-0.2.4/archspec/json/tests/targets/linux-rhel7-ivybridge
+-rw-r--r--   0        0        0     1286 2021-09-03 15:23:36.888990 archspec-0.2.4/archspec/json/tests/targets/linux-rhel7-skylake_avx512
+-rw-r--r--   0        0        0     1172 2021-10-22 10:17:21.472678 archspec-0.2.4/archspec/json/tests/targets/linux-rhel7-x86_64_v3
+-rw-r--r--   0        0        0     1319 2021-09-03 15:23:36.888990 archspec-0.2.4/archspec/json/tests/targets/linux-rhel7-zen
+-rw-r--r--   0        0        0      351 2024-03-19 06:53:55.122972 archspec-0.2.4/archspec/json/tests/targets/linux-rhel8-neoverse_v1
+-rw-r--r--   0        0        0      135 2023-11-06 16:40:45.253781 archspec-0.2.4/archspec/json/tests/targets/linux-rhel8-power9
+-rw-r--r--   0        0        0      444 2024-03-18 14:45:09.987004 archspec-0.2.4/archspec/json/tests/targets/linux-rhel9-neoverse_v2
+-rw-r--r--   0        0        0      256 2023-11-06 16:40:45.253781 archspec-0.2.4/archspec/json/tests/targets/linux-rocky8-a64fx
+-rw-r--r--   0        0        0     1750 2023-11-06 16:40:45.253781 archspec-0.2.4/archspec/json/tests/targets/linux-rocky8.5-zen4
+-rw-r--r--   0        0        0     1111 2021-09-03 15:23:36.888990 archspec-0.2.4/archspec/json/tests/targets/linux-scientific7-k10
+-rw-r--r--   0        0        0     1149 2021-09-03 15:23:36.888990 archspec-0.2.4/archspec/json/tests/targets/linux-scientific7-piledriver
+-rw-r--r--   0        0        0     1201 2021-09-03 15:23:36.888990 archspec-0.2.4/archspec/json/tests/targets/linux-scientificfermi6-bulldozer
+-rw-r--r--   0        0        0     1099 2021-09-03 15:23:36.888990 archspec-0.2.4/archspec/json/tests/targets/linux-scientificfermi6-piledriver
+-rw-r--r--   0        0        0      124 2021-10-22 10:17:21.472678 archspec-0.2.4/archspec/json/tests/targets/linux-sifive-u74mc
+-rw-r--r--   0        0        0     1190 2021-09-03 15:23:36.888990 archspec-0.2.4/archspec/json/tests/targets/linux-ubuntu18.04-broadwell
+-rw-r--r--   0        0        0     1531 2021-10-22 10:17:21.472678 archspec-0.2.4/archspec/json/tests/targets/linux-ubuntu20.04-zen3
+-rw-r--r--   0        0        0      458 2023-11-06 16:40:45.253781 archspec-0.2.4/archspec/json/tests/targets/linux-ubuntu22.04-neoverse_v2
+-rw-r--r--   0        0        0       83 2023-11-06 16:40:45.253781 archspec-0.2.4/archspec/json/tests/targets/linux-unknown-power10
+-rw-r--r--   0        0        0     2187 2023-11-06 16:40:45.257781 archspec-0.2.4/archspec/json/tests/targets/linux-unknown-sapphirerapids
+-rw-r--r--   0        0        0      395 2024-03-11 05:17:09.396309 archspec-0.2.4/archspec/json/tests/targets/windows-cpuid-broadwell
+-rw-r--r--   0        0        0      432 2024-03-11 05:17:09.396309 archspec-0.2.4/archspec/json/tests/targets/windows-cpuid-icelake
+-rw-r--r--   0        0        0       52 2024-02-15 22:06:34.808307 archspec-0.2.4/archspec/vendor/cpuid/.git
+-rw-r--r--   0        0        0       12 2024-02-15 22:06:34.856307 archspec-0.2.4/archspec/vendor/cpuid/.gitignore
+-rw-r--r--   0        0        0     1079 2024-02-15 22:06:34.856307 archspec-0.2.4/archspec/vendor/cpuid/LICENSE
+-rw-r--r--   0        0        0     2400 2024-02-15 22:06:34.856307 archspec-0.2.4/archspec/vendor/cpuid/README.md
+-rw-r--r--   0        0        0     6037 2024-02-17 07:41:48.471224 archspec-0.2.4/archspec/vendor/cpuid/cpuid.py
+-rw-r--r--   0        0        0     1855 2024-02-15 22:09:02.081631 archspec-0.2.4/archspec/vendor/cpuid/example.py
+-rw-r--r--   0        0        0     2119 2024-05-04 13:38:32.138207 archspec-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      200 2021-09-03 15:23:36.193003 archspec-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0     1678 2024-02-26 10:17:51.649680 archspec-0.2.4/tests/conftest.py
+-rw-r--r--   0        0        0      393 2024-05-04 13:38:32.138207 archspec-0.2.4/tests/test_archspec.py
+-rw-r--r--   0        0        0     1217 2024-02-26 10:17:51.649680 archspec-0.2.4/tests/test_cli.py
+-rw-r--r--   0        0        0    18450 2024-05-04 13:16:20.869021 archspec-0.2.4/tests/test_cpu.py
+-rw-r--r--   0        0        0     4375 1970-01-01 00:00:00.000000 archspec-0.2.4/PKG-INFO
```

### Comparing `archspec-0.2.3/LICENSE-APACHE` & `archspec-0.2.4/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/LICENSE-MIT` & `archspec-0.2.4/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/README.md` & `archspec-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/cli.py` & `archspec-0.2.4/archspec/cli.py`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/cpu/__init__.py` & `archspec-0.2.4/archspec/cpu/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # Copyright 2019-2020 Lawrence Livermore National Security, LLC and other
 # Archspec Project Developers. See the top-level COPYRIGHT file for details.
 #
 # SPDX-License-Identifier: (Apache-2.0 OR MIT)
 """The "cpu" package permits to query and compare different
 CPU microarchitectures.
 """
-from .detect import host
+from .detect import brand_string, host
 from .microarchitecture import (
     TARGETS,
+    InvalidCompilerVersion,
     Microarchitecture,
     UnsupportedMicroarchitecture,
     generic_microarchitecture,
     version_components,
 )
 
 __all__ = [
+    "brand_string",
+    "host",
+    "TARGETS",
+    "InvalidCompilerVersion",
     "Microarchitecture",
     "UnsupportedMicroarchitecture",
-    "TARGETS",
     "generic_microarchitecture",
-    "host",
     "version_components",
 ]
```

### Comparing `archspec-0.2.3/archspec/cpu/alias.py` & `archspec-0.2.4/archspec/cpu/alias.py`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/cpu/detect.py` & `archspec-0.2.4/archspec/cpu/detect.py`

 * *Files 7% similar despite different names*

```diff
@@ -151,14 +151,39 @@
 
         return result
 
     def _is_bit_set(self, register: int, bit: int) -> bool:
         mask = 1 << bit
         return register & mask > 0
 
+    def brand_string(self) -> Optional[str]:
+        """Returns the brand string, if available."""
+        if self.highest_extension_support < 0x80000004:
+            return None
+
+        r1 = self.cpuid.registers_for(eax=0x80000002, ecx=0)
+        r2 = self.cpuid.registers_for(eax=0x80000003, ecx=0)
+        r3 = self.cpuid.registers_for(eax=0x80000004, ecx=0)
+        result = struct.pack(
+            "IIIIIIIIIIII",
+            r1.eax,
+            r1.ebx,
+            r1.ecx,
+            r1.edx,
+            r2.eax,
+            r2.ebx,
+            r2.ecx,
+            r2.edx,
+            r3.eax,
+            r3.ebx,
+            r3.ecx,
+            r3.edx,
+        ).decode("utf-8")
+        return result.strip("\x00")
+
 
 @detection(operating_system="Windows")
 def cpuid_info():
     """Returns a partial Microarchitecture, obtained from running the cpuid instruction"""
     architecture = _machine()
     if architecture == X86_64:
         data = CpuidInfoCollector()
@@ -170,16 +195,16 @@
 def _check_output(args, env):
     with subprocess.Popen(args, stdout=subprocess.PIPE, env=env) as proc:
         output = proc.communicate()[0]
     return str(output.decode("utf-8"))
 
 
 WINDOWS_MAPPING = {
-    "AMD64": "x86_64",
-    "ARM64": "aarch64",
+    "AMD64": X86_64,
+    "ARM64": AARCH64,
 }
 
 
 def _machine():
     """Return the machine architecture we are on"""
     operating_system = platform.system()
 
@@ -405,7 +430,20 @@
 @compatibility_check(architecture_family=RISCV64)
 def compatibility_check_for_riscv64(info, target):
     """Compatibility check for riscv64 architectures."""
     arch_root = TARGETS[RISCV64]
     return (target == arch_root or arch_root in target.ancestors) and (
         target.name == info.name or target.vendor == "generic"
     )
+
+
+def brand_string() -> Optional[str]:
+    """Returns the brand string of the host, if detected, or None."""
+    if platform.system() == "Darwin":
+        return _check_output(
+            ["sysctl", "-n", "machdep.cpu.brand_string"], env=_ensure_bin_usrbin_in_path()
+        ).strip()
+
+    if host().family == X86_64:
+        return CpuidInfoCollector().brand_string()
+
+    return None
```

### Comparing `archspec-0.2.3/archspec/cpu/microarchitecture.py` & `archspec-0.2.4/archspec/cpu/microarchitecture.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,22 +204,29 @@
             generation=data.get("generation", 0),
         )
 
     def optimization_flags(self, compiler, version):
         """Returns a string containing the optimization flags that needs
         to be used to produce code optimized for this micro-architecture.
 
+        The version is expected to be a string of dot separated digits.
+
         If there is no information on the compiler passed as argument the
         function returns an empty string. If it is known that the compiler
         version we want to use does not support this architecture the function
         raises an exception.
 
         Args:
             compiler (str): name of the compiler to be used
             version (str): version of the compiler to be used
+
+        Raises:
+            UnsupportedMicroarchitecture: if the requested compiler does not support
+                this micro-architecture.
+            ValueError: if the version doesn't match the expected format
         """
         # If we don't have information on compiler at all return an empty string
         if compiler not in self.family.compilers:
             return ""
 
         # If we have information but it stops before this
         # microarchitecture, fall back to the best known target
@@ -228,14 +235,22 @@
             msg = (
                 "'{0}' compiler is known to optimize up to the '{1}'"
                 " microarchitecture in the '{2}' architecture family"
             )
             msg = msg.format(compiler, best_target, best_target.family)
             raise UnsupportedMicroarchitecture(msg)
 
+        # Check that the version matches the expected format
+        if not re.match(r"^(?:\d+\.)*\d+$", version):
+            msg = (
+                "invalid format for the compiler version argument. "
+                "Only dot separated digits are allowed."
+            )
+            raise InvalidCompilerVersion(msg)
+
         # If we have information on this compiler we need to check the
         # version being used
         compiler_info = self.compilers[compiler]
 
         def satisfies_constraint(entry, version):
             min_version, max_version = entry["versions"].split(":")
 
@@ -288,15 +303,15 @@
 
 def generic_microarchitecture(name):
     """Returns a generic micro-architecture with no vendor and no features.
 
     Args:
         name (str): name of the micro-architecture
     """
-    return Microarchitecture(name, parents=[], vendor="generic", features=[], compilers={})
+    return Microarchitecture(name, parents=[], vendor="generic", features=set(), compilers={})
 
 
 def version_components(version):
     """Decomposes the version passed as input in version number and
     suffix and returns them.
 
     If the version number or the suffix are not present, an empty
@@ -363,11 +378,19 @@
     return known_targets
 
 
 #: Dictionary of known micro-architectures
 TARGETS = LazyDictionary(_known_microarchitectures)
 
 
-class UnsupportedMicroarchitecture(ValueError):
+class ArchspecError(Exception):
+    """Base class for errors within archspec"""
+
+
+class UnsupportedMicroarchitecture(ArchspecError, ValueError):
     """Raised if a compiler version does not support optimization for a given
     micro-architecture.
     """
+
+
+class InvalidCompilerVersion(ArchspecError, ValueError):
+    """Raised when an invalid format is used for compiler versions in archspec."""
```

### Comparing `archspec-0.2.3/archspec/cpu/schema.py` & `archspec-0.2.4/archspec/cpu/schema.py`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/COPYRIGHT` & `archspec-0.2.4/archspec/json/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/LICENSE-APACHE` & `archspec-0.2.4/archspec/json/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/LICENSE-MIT` & `archspec-0.2.4/archspec/json/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/NOTICE` & `archspec-0.2.4/NOTICE`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/README.md` & `archspec-0.2.4/archspec/json/README.md`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/cpu/cpuid.json` & `archspec-0.2.4/archspec/json/cpu/cpuid.json`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/cpu/cpuid_schema.json` & `archspec-0.2.4/archspec/json/cpu/cpuid_schema.json`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/cpu/microarchitectures.json` & `archspec-0.2.4/archspec/json/cpu/microarchitectures.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999813363195221%*

 * *Differences: {"'microarchitectures'": "{'neoverse_v1': {'features': {delete: [30, 29]}}, 'neoverse_v2': "*

 * *                         "{'features': {delete: [46, 31, 30]}}}"}*

```diff
@@ -1755,16 +1755,14 @@
                 "sve",
                 "asimdfhm",
                 "dit",
                 "uscat",
                 "ilrcpc",
                 "flagm",
                 "ssbs",
-                "paca",
-                "pacg",
                 "dcpodp",
                 "svei8mm",
                 "svebf16",
                 "i8mm",
                 "bf16",
                 "dgh",
                 "rng"
@@ -1870,31 +1868,28 @@
                 "asimdfhm",
                 "dit",
                 "uscat",
                 "ilrcpc",
                 "flagm",
                 "ssbs",
                 "sb",
-                "paca",
-                "pacg",
                 "dcpodp",
                 "sve2",
                 "sveaes",
                 "svepmull",
                 "svebitperm",
                 "svesha3",
                 "svesm4",
                 "flagm2",
                 "frint",
                 "svei8mm",
                 "svebf16",
                 "i8mm",
                 "bf16",
-                "dgh",
-                "bti"
+                "dgh"
             ],
             "from": [
                 "neoverse_n1",
                 "armv9.0a"
             ],
             "vendor": "ARM"
         },
```

### Comparing `archspec-0.2.3/archspec/json/cpu/microarchitectures_schema.json` & `archspec-0.2.4/archspec/json/cpu/microarchitectures_schema.json`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/tests/targets/darwin-bigsur-m1` & `archspec-0.2.4/archspec/json/tests/targets/darwin-bigsur-m1`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/tests/targets/darwin-mojave-haswell` & `archspec-0.2.4/archspec/json/tests/targets/darwin-mojave-haswell`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/tests/targets/darwin-mojave-ivybridge` & `archspec-0.2.4/archspec/json/tests/targets/darwin-mojave-ivybridge`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/tests/targets/darwin-mojave-skylake` & `archspec-0.2.4/archspec/json/tests/targets/darwin-mojave-skylake`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/tests/targets/darwin-monterey-m1` & `archspec-0.2.4/archspec/json/tests/targets/darwin-monterey-m1`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/tests/targets/darwin-monterey-m2` & `archspec-0.2.4/archspec/json/tests/targets/darwin-monterey-m2`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/tests/targets/linux-amazon2-sapphirerapids` & `archspec-0.2.4/archspec/json/tests/targets/linux-amazon2-sapphirerapids`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/tests/targets/linux-centos7-cascadelake` & `archspec-0.2.4/archspec/json/tests/targets/linux-centos7-cascadelake`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/tests/targets/linux-rhel6-piledriver` & `archspec-0.2.4/archspec/json/tests/targets/linux-rhel6-piledriver`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/tests/targets/linux-rhel7-broadwell` & `archspec-0.2.4/archspec/json/tests/targets/linux-rhel7-broadwell`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/tests/targets/linux-rhel7-haswell` & `archspec-0.2.4/archspec/json/tests/targets/linux-rhel7-haswell`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/tests/targets/linux-rhel7-ivybridge` & `archspec-0.2.4/archspec/json/tests/targets/linux-rhel7-ivybridge`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/tests/targets/linux-rhel7-skylake_avx512` & `archspec-0.2.4/archspec/json/tests/targets/linux-rhel7-skylake_avx512`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/tests/targets/linux-rhel7-x86_64_v3` & `archspec-0.2.4/archspec/json/tests/targets/linux-rhel7-x86_64_v3`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/tests/targets/linux-rhel7-zen` & `archspec-0.2.4/archspec/json/tests/targets/linux-rhel7-zen`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/tests/targets/linux-rocky8.5-zen4` & `archspec-0.2.4/archspec/json/tests/targets/linux-rocky8.5-zen4`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/tests/targets/linux-scientific7-k10` & `archspec-0.2.4/archspec/json/tests/targets/linux-scientific7-k10`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/tests/targets/linux-scientific7-piledriver` & `archspec-0.2.4/archspec/json/tests/targets/linux-scientific7-piledriver`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/tests/targets/linux-scientificfermi6-bulldozer` & `archspec-0.2.4/archspec/json/tests/targets/linux-scientificfermi6-bulldozer`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/tests/targets/linux-scientificfermi6-piledriver` & `archspec-0.2.4/archspec/json/tests/targets/linux-scientificfermi6-piledriver`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/tests/targets/linux-ubuntu18.04-broadwell` & `archspec-0.2.4/archspec/json/tests/targets/linux-ubuntu18.04-broadwell`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/tests/targets/linux-ubuntu20.04-zen3` & `archspec-0.2.4/archspec/json/tests/targets/linux-ubuntu20.04-zen3`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/json/tests/targets/linux-unknown-sapphirerapids` & `archspec-0.2.4/archspec/json/tests/targets/linux-unknown-sapphirerapids`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/vendor/cpuid/LICENSE` & `archspec-0.2.4/archspec/vendor/cpuid/LICENSE`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/vendor/cpuid/README.md` & `archspec-0.2.4/archspec/vendor/cpuid/README.md`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/vendor/cpuid/cpuid.py` & `archspec-0.2.4/archspec/vendor/cpuid/cpuid.py`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/archspec/vendor/cpuid/example.py` & `archspec-0.2.4/archspec/vendor/cpuid/example.py`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/pyproject.toml` & `archspec-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "archspec"
-version = "0.2.3"
+version = "0.2.4"
 description = "A library to query system architecture"
 license = "Apache-2.0 OR MIT"
 authors = ["archspec developers <maintainers@spack.io>"]
 maintainers = [
     "Greg Becker <maintainers@spack.io>",
     "Massimiliano Culpo <massimiliano.culpo@gmail.com>",
     "Todd Gamblin <maintainers@spack.io>",
```

### Comparing `archspec-0.2.3/tests/conftest.py` & `archspec-0.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/tests/test_cli.py` & `archspec-0.2.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `archspec-0.2.3/tests/test_cpu.py` & `archspec-0.2.4/tests/test_cpu.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,16 +54,18 @@
         "darwin-monterey-m2",
         "linux-rocky8-a64fx",
         "linux-amazon2-sapphirerapids",
         "linux-unknown-sapphirerapids",
         "linux-rhel8-power9",
         "linux-unknown-power10",
         "linux-ubuntu22.04-neoverse_v2",
+        "linux-rhel9-neoverse_v2",
         "windows-cpuid-broadwell",
         "windows-cpuid-icelake",
+        "linux-rhel8-neoverse_v1",
     ]
 )
 def expected_target(request, monkeypatch):
     cpu = archspec.cpu
     platform, operating_system, target = request.param.split("-")
 
     # This is the default to use for tests on Darwin, since it will match
@@ -71,70 +73,105 @@
     # (i.e. Python for x86_64 running on top of Rosetta)
     architecture_family = "x86_64" if platform == "darwin" else archspec.cpu.TARGETS[target].family
     if platform == "windows":
         architecture_family = "AMD64" if architecture_family == "x86_64" else "ARM64"
 
     monkeypatch.setattr(cpu.detect.platform, "machine", lambda: str(architecture_family))
 
-    test_dir = os.path.dirname(__file__)
-    target_dir = os.path.join(test_dir, "..", "archspec", "json", "tests", "targets")
+    target_dir = targets_directory()
     # Monkeypatch for linux
     if platform in ("linux", "bgq"):
         monkeypatch.setattr(cpu.detect.platform, "system", lambda: "Linux")
 
         @contextlib.contextmanager
         def _open(not_used_arg):
             filename = os.path.join(target_dir, request.param)
             with open(filename) as f:
                 yield f
 
         monkeypatch.setattr(cpu.detect, "open", _open, raising=False)
 
     elif platform == "darwin":
         monkeypatch.setattr(cpu.detect.platform, "system", lambda: "Darwin")
-
         filename = os.path.join(target_dir, request.param)
-        info = {}
-        with open(filename) as f:
-            for line in f:
-                key, value = line.split(":")
-                info[key.strip()] = value.strip()
-
-        def _check_output(args, env):
-            current_key = args[-1]
-            return info[current_key]
-
-        monkeypatch.setattr(cpu.detect, "_check_output", _check_output)
+        monkeypatch.setattr(cpu.detect, "_check_output", mock_check_output(filename))
 
     elif platform == "windows":
         monkeypatch.setattr(cpu.detect.platform, "system", lambda: "Windows")
         filename = os.path.join(target_dir, request.param)
+        monkeypatch.setattr(cpu.detect, "CPUID", mock_CpuidInfoCollector(filename))
+
+    return archspec.cpu.TARGETS[target]
 
-        class MockRegisters(NamedTuple):
-            eax: int
-            ebx: int
-            ecx: int
-            edx: int
-
-        class MockCPUID:
-            def __init__(self):
-                self.data = {}
-                with open(filename) as f:
-                    reader = csv.reader(f)
-                    for row in reader:
-                        key = int(row[0]), int(row[1])
-                        values = tuple(int(x) for x in row[2:])
-                        self.data[key] = MockRegisters(*values)
 
-            def registers_for(self, eax, ecx):
-                return self.data.get((eax, ecx), MockRegisters(0, 0, 0, 0))
+def targets_directory():
+    test_dir = os.path.dirname(__file__)
+    target_dir = os.path.join(test_dir, "..", "archspec", "json", "tests", "targets")
+    return target_dir
 
-        monkeypatch.setattr(cpu.detect, "CPUID", MockCPUID)
 
-    return archspec.cpu.TARGETS[target]
+@pytest.fixture(
+    params=[
+        ("darwin-mojave-ivybridge", "Intel(R) Core(TM) i5-3230M CPU @ 2.60GHz"),
+        ("darwin-mojave-haswell", "Intel(R) Core(TM) i7-4980HQ CPU @ 2.80GHz"),
+        ("darwin-mojave-skylake", "Intel(R) Core(TM) i7-6700K CPU @ 4.00GHz"),
+        ("darwin-monterey-m1", "Apple M1 Pro"),
+        ("darwin-monterey-m2", "Apple M2"),
+        ("windows-cpuid-broadwell", "Intel(R) Core(TM) i7-5500U CPU @ 2.40GHz"),
+        ("windows-cpuid-icelake", "11th Gen Intel(R) Core(TM) i7-1185G7 @ 3.00GHz"),
+    ]
+)
+def expected_brand_string(request, monkeypatch):
+    test_file, expected_result = request.param
+    filename = os.path.join(targets_directory(), test_file)
+    if "darwin" in test_file:
+        monkeypatch.setattr(archspec.cpu.detect.platform, "system", lambda: "Darwin")
+        monkeypatch.setattr(archspec.cpu.detect, "_check_output", mock_check_output(filename))
+    elif "cpuid" in test_file:
+        monkeypatch.setattr(archspec.cpu.detect, "host", lambda: archspec.cpu.TARGETS["x86_64"])
+        monkeypatch.setattr(archspec.cpu.detect.platform, "system", lambda: "Windows")
+        monkeypatch.setattr(archspec.cpu.detect, "CPUID", mock_CpuidInfoCollector(filename))
+    return expected_result
+
+
+def mock_check_output(filename):
+    info = {}
+    with open(filename) as f:
+        for line in f:
+            key, value = line.split(":")
+            info[key.strip()] = value.strip()
+
+    def _check_output(args, env):
+        current_key = args[-1]
+        return info[current_key]
+
+    return _check_output
+
+
+def mock_CpuidInfoCollector(filename):
+    class MockRegisters(NamedTuple):
+        eax: int
+        ebx: int
+        ecx: int
+        edx: int
+
+    class MockCPUID:
+        def __init__(self):
+            self.data = {}
+            with open(filename) as f:
+                reader = csv.reader(f)
+                for row in reader:
+                    key = int(row[0]), int(row[1])
+                    values = tuple(int(x) for x in row[2:])
+                    self.data[key] = MockRegisters(*values)
+
+        def registers_for(self, eax, ecx):
+            return self.data.get((eax, ecx), MockRegisters(0, 0, 0, 0))
+
+    return MockCPUID
 
 
 @pytest.fixture(params=[x for x in archspec.cpu.TARGETS])
 def supported_target(request):
     return request.param
 
 
@@ -466,7 +503,30 @@
     """Tests that we can supply only one extension file in a custom directory, and that reading
     any other JSON file will not give errors.
     """
     monkeypatch.setenv("ARCHSPEC_EXTENSION_CPU_DIR", str(extension_file.parent))
     reset_global_state()
     assert "pentium2.5" in archspec.cpu.TARGETS
     assert "flags" in archspec.cpu.schema.CPUID_JSON
+
+
+def test_brand_string(expected_brand_string):
+    assert archspec.cpu.detect.brand_string() == expected_brand_string
+
+
+@pytest.mark.parametrize(
+    "version_str",
+    [
+        "13.2.0.debug",
+        "optimized",
+    ],
+)
+def test_error_message_unknown_compiler_version(version_str):
+    """Tests that passing a version to Microarchitecture.optimization_flags with a wrong format,
+    raises a comprehensible error message.
+    """
+    t = archspec.cpu.TARGETS["icelake"]
+    with pytest.raises(
+        archspec.cpu.InvalidCompilerVersion,
+        match="invalid format for the compiler version argument",
+    ):
+        t.optimization_flags("gcc", version_str)
```

### Comparing `archspec-0.2.3/PKG-INFO` & `archspec-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archspec
-Version: 0.2.3
+Version: 0.2.4
 Summary: A library to query system architecture
 Home-page: https://github.com/archspec/archspec
 License: Apache-2.0 OR MIT
 Author: archspec developers
 Author-email: maintainers@spack.io
 Maintainer: Greg Becker
 Maintainer-email: maintainers@spack.io
```

