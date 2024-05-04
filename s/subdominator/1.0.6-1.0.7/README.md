# Comparing `tmp/subdominator-1.0.6.tar.gz` & `tmp/subdominator-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subdominator-1.0.6.tar", last modified: Sat Jan 13 06:57:11 2024, max compression
+gzip compressed data, was "subdominator-1.0.7.tar", last modified: Sat May  4 08:56:02 2024, max compression
```

## Comparing `subdominator-1.0.6.tar` & `subdominator-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,177 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 06:57:11.567859 subdominator-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-01-13 06:57:03.000000 subdominator-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-01-13 06:57:11.563859 subdominator-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10556 2024-01-13 06:57:03.000000 subdominator-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-13 06:57:11.567859 subdominator-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-01-13 06:57:03.000000 subdominator-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 06:57:11.563859 subdominator-1.0.6/subdominator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 06:57:03.000000 subdominator-1.0.6/subdominator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    95863 2024-01-13 06:57:03.000000 subdominator-1.0.6/subdominator/subdominator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 06:57:11.563859 subdominator-1.0.6/subdominator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-01-13 06:57:11.000000 subdominator-1.0.6/subdominator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-13 06:57:11.000000 subdominator-1.0.6/subdominator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-13 06:57:11.000000 subdominator-1.0.6/subdominator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-13 06:57:11.000000 subdominator-1.0.6/subdominator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-01-13 06:57:11.000000 subdominator-1.0.6/subdominator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-13 06:57:11.000000 subdominator-1.0.6/subdominator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.767939 subdominator-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-04 08:55:55.000000 subdominator-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22347 2024-05-04 08:56:02.763939 subdominator-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21735 2024-05-04 08:55:55.000000 subdominator-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 08:56:02.767939 subdominator-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-04 08:55:55.000000 subdominator-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.743939 subdominator-1.0.7/subdominator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.747939 subdominator-1.0.7/subdominator/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.747939 subdominator-1.0.7/subdominator/modules/banner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/banner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/banner/banner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.747939 subdominator-1.0.7/subdominator/modules/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.747939 subdominator-1.0.7/subdominator/modules/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.747939 subdominator-1.0.7/subdominator/modules/enumerates/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.747939 subdominator-1.0.7/subdominator/modules/enumerates/abuseipdb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/abuseipdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/abuseipdb/abuseipdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.747939 subdominator-1.0.7/subdominator/modules/enumerates/alienvault/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/alienvault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/alienvault/alienvault.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.747939 subdominator-1.0.7/subdominator/modules/enumerates/anubis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/anubis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/anubis/anubis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.747939 subdominator-1.0.7/subdominator/modules/enumerates/bevigil/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/bevigil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/bevigil/bevigil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.751939 subdominator-1.0.7/subdominator/modules/enumerates/binaryedge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/binaryedge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/binaryedge/binaryedge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.751939 subdominator-1.0.7/subdominator/modules/enumerates/bufferover/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/bufferover/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/bufferover/bufferover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.751939 subdominator-1.0.7/subdominator/modules/enumerates/censys/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/censys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/censys/censys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.751939 subdominator-1.0.7/subdominator/modules/enumerates/certspotter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/certspotter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5648 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/certspotter/certspotter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.751939 subdominator-1.0.7/subdominator/modules/enumerates/chaos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/chaos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/chaos/chaos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.751939 subdominator-1.0.7/subdominator/modules/enumerates/columbusapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/columbusapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/columbusapi/columbusapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.751939 subdominator-1.0.7/subdominator/modules/enumerates/crtsh/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/crtsh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/crtsh/crtsh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.751939 subdominator-1.0.7/subdominator/modules/enumerates/digitorus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/digitorus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/digitorus/digitorus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.751939 subdominator-1.0.7/subdominator/modules/enumerates/dnsdumpster/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/dnsdumpster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/dnsdumpster/dnsdumpster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.751939 subdominator-1.0.7/subdominator/modules/enumerates/dnsrepo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/dnsrepo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/dnsrepo/dnsrepo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.751939 subdominator-1.0.7/subdominator/modules/enumerates/facebook/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/facebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/facebook/facebook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.751939 subdominator-1.0.7/subdominator/modules/enumerates/fullhunt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/fullhunt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5116 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/fullhunt/fullhunt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.755939 subdominator-1.0.7/subdominator/modules/enumerates/google/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/google/google.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.755939 subdominator-1.0.7/subdominator/modules/enumerates/hackertarget/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/hackertarget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/hackertarget/hackertarget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.755939 subdominator-1.0.7/subdominator/modules/enumerates/huntermap/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/huntermap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/huntermap/huntermap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.755939 subdominator-1.0.7/subdominator/modules/enumerates/intelx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/intelx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/intelx/intelx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.755939 subdominator-1.0.7/subdominator/modules/enumerates/leakix/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/leakix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/leakix/leakix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.755939 subdominator-1.0.7/subdominator/modules/enumerates/netlas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/netlas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/netlas/netlas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.755939 subdominator-1.0.7/subdominator/modules/enumerates/quake/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/quake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/quake/quake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.755939 subdominator-1.0.7/subdominator/modules/enumerates/rapidapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/rapidapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/rapidapi/rapidapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.755939 subdominator-1.0.7/subdominator/modules/enumerates/rapiddns/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/rapiddns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/rapiddns/rapiddns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.755939 subdominator-1.0.7/subdominator/modules/enumerates/rapidfinder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/rapidfinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/rapidfinder/rapidfinder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.755939 subdominator-1.0.7/subdominator/modules/enumerates/rapidscan/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/rapidscan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/rapidscan/rapidscan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.759939 subdominator-1.0.7/subdominator/modules/enumerates/redhuntlabs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/redhuntlabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/redhuntlabs/redhuntlabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.759939 subdominator-1.0.7/subdominator/modules/enumerates/securitytrails/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/securitytrails/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/securitytrails/securitytrails.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.759939 subdominator-1.0.7/subdominator/modules/enumerates/shodan/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/shodan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/shodan/shodan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.759939 subdominator-1.0.7/subdominator/modules/enumerates/shodanx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/shodanx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/shodanx/shodanx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.759939 subdominator-1.0.7/subdominator/modules/enumerates/shrewdeye/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/shrewdeye/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/shrewdeye/shrewdeye.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.759939 subdominator-1.0.7/subdominator/modules/enumerates/sitedossier/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/sitedossier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/sitedossier/sitedossier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.759939 subdominator-1.0.7/subdominator/modules/enumerates/subdomaincenter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/subdomaincenter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/subdomaincenter/subdomaincenter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.759939 subdominator-1.0.7/subdominator/modules/enumerates/urlscan/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/urlscan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/urlscan/urlscan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.759939 subdominator-1.0.7/subdominator/modules/enumerates/virustotal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/virustotal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/virustotal/virustotal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.759939 subdominator-1.0.7/subdominator/modules/enumerates/waybackarchive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/waybackarchive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/waybackarchive/waybackarchive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.759939 subdominator-1.0.7/subdominator/modules/enumerates/whoisxml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/whoisxml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/whoisxml/whoisxml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.759939 subdominator-1.0.7/subdominator/modules/enumerates/zoomeyeapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/zoomeyeapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/enumerates/zoomeyeapi/zoomeyeapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.763939 subdominator-1.0.7/subdominator/modules/extract/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/extract/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.763939 subdominator-1.0.7/subdominator/modules/file/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/file/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13974 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.763939 subdominator-1.0.7/subdominator/modules/help/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/help/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/help/help.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.763939 subdominator-1.0.7/subdominator/modules/notify/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/notify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/notify/notify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.763939 subdominator-1.0.7/subdominator/modules/save/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/save/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/save/save.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.763939 subdominator-1.0.7/subdominator/modules/source/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/source/source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.763939 subdominator-1.0.7/subdominator/modules/update/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/update/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.763939 subdominator-1.0.7/subdominator/modules/username/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/username/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/username/username.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.763939 subdominator-1.0.7/subdominator/modules/verify/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/verify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/verify/verify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.763939 subdominator-1.0.7/subdominator/modules/version/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/modules/version/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-04 08:55:55.000000 subdominator-1.0.7/subdominator/subdominator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:56:02.763939 subdominator-1.0.7/subdominator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22347 2024-05-04 08:56:02.000000 subdominator-1.0.7/subdominator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-05-04 08:56:02.000000 subdominator-1.0.7/subdominator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 08:56:02.000000 subdominator-1.0.7/subdominator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-04 08:56:02.000000 subdominator-1.0.7/subdominator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-04 08:56:02.000000 subdominator-1.0.7/subdominator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-04 08:56:02.000000 subdominator-1.0.7/subdominator.egg-info/top_level.txt
```

### Comparing `subdominator-1.0.6/LICENSE` & `subdominator-1.0.7/LICENSE`

 * *Files identical despite different names*

