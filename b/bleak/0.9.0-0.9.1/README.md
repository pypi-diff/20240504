# Comparing `tmp/bleak-0.9.0.tar.gz` & `tmp/bleak-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bleak-0.9.0.tar", last modified: Tue Oct 20 21:32:21 2020, max compression
+gzip compressed data, was "dist/bleak-0.9.1.tar", last modified: Thu Oct 22 09:14:40 2020, max compression
```

## Comparing `bleak-0.9.0.tar` & `bleak-0.9.1.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-20 21:32:21.154277 bleak-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (116)      169 2020-10-20 21:32:11.000000 bleak-0.9.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (116)    13490 2020-10-20 21:32:11.000000 bleak-0.9.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (116)     3249 2020-10-20 21:32:11.000000 bleak-0.9.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1072 2020-10-20 21:32:11.000000 bleak-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      359 2020-10-20 21:32:11.000000 bleak-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)    20653 2020-10-20 21:32:21.154277 bleak-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2568 2020-10-20 21:32:11.000000 bleak-0.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-20 21:32:21.146277 bleak-0.9.0/bleak/
--rw-r--r--   0 runner    (1001) docker     (116)     3578 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       47 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-20 21:32:21.146277 bleak-0.9.0/bleak/backends/
--rw-r--r--   0 runner    (1001) docker     (116)      106 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    67669 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/_manufacturers.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-20 21:32:21.150277 bleak-0.9.0/bleak/backends/bluezdbus/
--rw-r--r--   0 runner    (1001) docker     (116)      948 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/bluezdbus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2911 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/bluezdbus/characteristic.py
--rw-r--r--   0 runner    (1001) docker     (116)    34590 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/bluezdbus/client.py
--rw-r--r--   0 runner    (1001) docker     (116)      625 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/bluezdbus/defs.py
--rw-r--r--   0 runner    (1001) docker     (116)     1357 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/bluezdbus/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (116)     7286 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/bluezdbus/discovery.py
--rw-r--r--   0 runner    (1001) docker     (116)    10568 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/bluezdbus/scanner.py
--rw-r--r--   0 runner    (1001) docker     (116)     1166 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/bluezdbus/service.py
--rw-r--r--   0 runner    (1001) docker     (116)     1579 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/bluezdbus/signals.py
--rw-r--r--   0 runner    (1001) docker     (116)     3362 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/bluezdbus/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     2395 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/characteristic.py
--rw-r--r--   0 runner    (1001) docker     (116)     8051 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/client.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-20 21:32:21.150277 bleak-0.9.0/bleak/backends/corebluetooth/
--rw-r--r--   0 runner    (1001) docker     (116)    11850 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/corebluetooth/CentralManagerDelegate.py
--rw-r--r--   0 runner    (1001) docker     (116)    14988 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/corebluetooth/PeripheralDelegate.py
--rw-r--r--   0 runner    (1001) docker     (116)      148 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/corebluetooth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3944 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/corebluetooth/characteristic.py
--rw-r--r--   0 runner    (1001) docker     (116)    16970 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/corebluetooth/client.py
--rw-r--r--   0 runner    (1001) docker     (116)     1450 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/corebluetooth/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (116)     4534 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/corebluetooth/device.py
--rw-r--r--   0 runner    (1001) docker     (116)     1149 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/corebluetooth/discovery.py
--rw-r--r--   0 runner    (1001) docker     (116)     5642 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/corebluetooth/scanner.py
--rw-r--r--   0 runner    (1001) docker     (116)     1142 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/corebluetooth/service.py
--rw-r--r--   0 runner    (1001) docker     (116)     1533 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/corebluetooth/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     4181 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (116)     2858 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/device.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-20 21:32:21.150277 bleak-0.9.0/bleak/backends/dotnet/
--rw-r--r--   0 runner    (1001) docker     (116)     8704 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/dotnet/BleakUWPBridge.dll
--rw-r--r--   0 runner    (1001) docker     (116)      340 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/dotnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3675 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/dotnet/characteristic.py
--rw-r--r--   0 runner    (1001) docker     (116)    34611 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/dotnet/client.py
--rw-r--r--   0 runner    (1001) docker     (116)     1287 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/dotnet/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (116)     9189 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/dotnet/discovery.py
--rw-r--r--   0 runner    (1001) docker     (116)    10223 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/dotnet/scanner.py
--rw-r--r--   0 runner    (1001) docker     (116)     1182 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/dotnet/service.py
--rw-r--r--   0 runner    (1001) docker     (116)     3376 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/dotnet/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     3522 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/scanner.py
--rw-r--r--   0 runner    (1001) docker     (116)     6118 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/backends/service.py
--rw-r--r--   0 runner    (1001) docker     (116)     3285 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/exc.py
--rw-r--r--   0 runner    (1001) docker     (116)      630 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)    33540 2020-10-20 21:32:11.000000 bleak-0.9.0/bleak/uuids.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-20 21:32:21.146277 bleak-0.9.0/bleak.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    20653 2020-10-20 21:32:20.000000 bleak-0.9.0/bleak.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2116 2020-10-20 21:32:21.000000 bleak-0.9.0/bleak.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-20 21:32:20.000000 bleak-0.9.0/bleak.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       44 2020-10-20 21:32:20.000000 bleak-0.9.0/bleak.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      185 2020-10-20 21:32:20.000000 bleak-0.9.0/bleak.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        6 2020-10-20 21:32:20.000000 bleak-0.9.0/bleak.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-20 21:32:21.154277 bleak-0.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (116)     6758 2020-10-20 21:32:11.000000 bleak-0.9.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)     1444 2020-10-20 21:32:11.000000 bleak-0.9.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (116)       28 2020-10-20 21:32:11.000000 bleak-0.9.0/docs/authors.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-20 21:32:21.154277 bleak-0.9.0/docs/backends/
--rw-r--r--   0 runner    (1001) docker     (116)      448 2020-10-20 21:32:11.000000 bleak-0.9.0/docs/backends/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1080 2020-10-20 21:32:11.000000 bleak-0.9.0/docs/backends/linux.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1240 2020-10-20 21:32:11.000000 bleak-0.9.0/docs/backends/macos.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1044 2020-10-20 21:32:11.000000 bleak-0.9.0/docs/backends/windows.rst
--rwxr-xr-x   0 runner    (1001) docker     (116)     8860 2020-10-20 21:32:11.000000 bleak-0.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)       33 2020-10-20 21:32:11.000000 bleak-0.9.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (116)       30 2020-10-20 21:32:11.000000 bleak-0.9.0/docs/history.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-20 21:32:21.154277 bleak-0.9.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (116)    45371 2020-10-20 21:32:11.000000 bleak-0.9.0/docs/images/win-10-start-cmd-as-admin.png
--rw-r--r--   0 runner    (1001) docker     (116)     1776 2020-10-20 21:32:11.000000 bleak-0.9.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1144 2020-10-20 21:32:11.000000 bleak-0.9.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (116)     6457 2020-10-20 21:32:11.000000 bleak-0.9.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (116)     4293 2020-10-20 21:32:11.000000 bleak-0.9.0/docs/scanning.rst
--rw-r--r--   0 runner    (1001) docker     (116)     4466 2020-10-20 21:32:11.000000 bleak-0.9.0/docs/troubleshooting.rst
--rw-r--r--   0 runner    (1001) docker     (116)     2112 2020-10-20 21:32:11.000000 bleak-0.9.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (116)      307 2020-10-20 21:32:21.154277 bleak-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     3539 2020-10-20 21:32:11.000000 bleak-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-20 21:32:21.154277 bleak-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (116)       60 2020-10-20 21:32:11.000000 bleak-0.9.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      973 2020-10-20 21:32:11.000000 bleak-0.9.0/tests/test_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-22 09:14:40.544852 bleak-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (116)      238 2020-10-22 09:14:30.000000 bleak-0.9.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (116)    14269 2020-10-22 09:14:30.000000 bleak-0.9.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     3396 2020-10-22 09:14:30.000000 bleak-0.9.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1072 2020-10-22 09:14:30.000000 bleak-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      359 2020-10-22 09:14:30.000000 bleak-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)    21664 2020-10-22 09:14:40.544852 bleak-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2568 2020-10-22 09:14:30.000000 bleak-0.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-22 09:14:40.536852 bleak-0.9.1/bleak/
+-rw-r--r--   0 runner    (1001) docker     (116)     3578 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)       47 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-22 09:14:40.536852 bleak-0.9.1/bleak/backends/
+-rw-r--r--   0 runner    (1001) docker     (116)      106 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    67669 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/_manufacturers.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-22 09:14:40.540852 bleak-0.9.1/bleak/backends/bluezdbus/
+-rw-r--r--   0 runner    (1001) docker     (116)      948 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/bluezdbus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2911 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/bluezdbus/characteristic.py
+-rw-r--r--   0 runner    (1001) docker     (116)    34766 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/bluezdbus/client.py
+-rw-r--r--   0 runner    (1001) docker     (116)      625 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/bluezdbus/defs.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1357 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/bluezdbus/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7286 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/bluezdbus/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10568 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/bluezdbus/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1166 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/bluezdbus/service.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1579 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/bluezdbus/signals.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3362 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/bluezdbus/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2395 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/characteristic.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8051 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/client.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-22 09:14:40.540852 bleak-0.9.1/bleak/backends/corebluetooth/
+-rw-r--r--   0 runner    (1001) docker     (116)    11784 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/corebluetooth/CentralManagerDelegate.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14988 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/corebluetooth/PeripheralDelegate.py
+-rw-r--r--   0 runner    (1001) docker     (116)      148 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/corebluetooth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3944 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/corebluetooth/characteristic.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16932 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/corebluetooth/client.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1450 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/corebluetooth/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4511 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/corebluetooth/device.py
+-rw-r--r--   0 runner    (1001) docker     (116)      952 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/corebluetooth/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5508 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/corebluetooth/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1142 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/corebluetooth/service.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1533 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/corebluetooth/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4181 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2858 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/device.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-22 09:14:40.540852 bleak-0.9.1/bleak/backends/dotnet/
+-rw-r--r--   0 runner    (1001) docker     (116)     8704 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/dotnet/BleakUWPBridge.dll
+-rw-r--r--   0 runner    (1001) docker     (116)      340 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/dotnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3675 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/dotnet/characteristic.py
+-rw-r--r--   0 runner    (1001) docker     (116)    34611 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/dotnet/client.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1287 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/dotnet/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9189 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/dotnet/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10223 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/dotnet/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1182 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/dotnet/service.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3376 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/dotnet/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3522 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6118 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/backends/service.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3285 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/exc.py
+-rw-r--r--   0 runner    (1001) docker     (116)      630 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)    33540 2020-10-22 09:14:30.000000 bleak-0.9.1/bleak/uuids.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-22 09:14:40.536852 bleak-0.9.1/bleak.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)    21664 2020-10-22 09:14:39.000000 bleak-0.9.1/bleak.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2116 2020-10-22 09:14:40.000000 bleak-0.9.1/bleak.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-22 09:14:39.000000 bleak-0.9.1/bleak.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       44 2020-10-22 09:14:39.000000 bleak-0.9.1/bleak.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      185 2020-10-22 09:14:39.000000 bleak-0.9.1/bleak.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        6 2020-10-22 09:14:39.000000 bleak-0.9.1/bleak.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-22 09:14:40.544852 bleak-0.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (116)     6758 2020-10-22 09:14:30.000000 bleak-0.9.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (116)     1444 2020-10-22 09:14:30.000000 bleak-0.9.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (116)       28 2020-10-22 09:14:30.000000 bleak-0.9.1/docs/authors.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-22 09:14:40.544852 bleak-0.9.1/docs/backends/
+-rw-r--r--   0 runner    (1001) docker     (116)      448 2020-10-22 09:14:30.000000 bleak-0.9.1/docs/backends/index.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1080 2020-10-22 09:14:30.000000 bleak-0.9.1/docs/backends/linux.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1240 2020-10-22 09:14:30.000000 bleak-0.9.1/docs/backends/macos.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1044 2020-10-22 09:14:30.000000 bleak-0.9.1/docs/backends/windows.rst
+-rwxr-xr-x   0 runner    (1001) docker     (116)     8860 2020-10-22 09:14:30.000000 bleak-0.9.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (116)       33 2020-10-22 09:14:30.000000 bleak-0.9.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (116)       30 2020-10-22 09:14:30.000000 bleak-0.9.1/docs/history.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-22 09:14:40.544852 bleak-0.9.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (116)    45371 2020-10-22 09:14:30.000000 bleak-0.9.1/docs/images/win-10-start-cmd-as-admin.png
+-rw-r--r--   0 runner    (1001) docker     (116)     1776 2020-10-22 09:14:30.000000 bleak-0.9.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1144 2020-10-22 09:14:30.000000 bleak-0.9.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     6457 2020-10-22 09:14:30.000000 bleak-0.9.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (116)     4293 2020-10-22 09:14:30.000000 bleak-0.9.1/docs/scanning.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     4466 2020-10-22 09:14:30.000000 bleak-0.9.1/docs/troubleshooting.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     2112 2020-10-22 09:14:30.000000 bleak-0.9.1/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      307 2020-10-22 09:14:40.544852 bleak-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     3539 2020-10-22 09:14:30.000000 bleak-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-22 09:14:40.544852 bleak-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)       60 2020-10-22 09:14:30.000000 bleak-0.9.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      973 2020-10-22 09:14:30.000000 bleak-0.9.1/tests/test_imports.py
```

### Comparing `bleak-0.9.0/CHANGELOG.rst` & `bleak-0.9.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,42 @@
 =========
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog <https://keepachangelog.com/en/1.0.0/>`_,
 and this project adheres to `Semantic Versioning <https://semver.org/spec/v2.0.0.html>`_.
 
+
+`0.9.1`_ (2020-10-22)
+---------------------
+
+Added
+~~~~~
+
+* Added new attribute ``_device_info`` on ``BleakClientBlueZDBus``. Merges #347.
+* Added Pull Request Template.
+
+Changed
+~~~~~~~
+
+* Updated instructions on how to contribute, file issues and make PRs.
+* Updated ``AUTHORS.rst`` file with development team.
+
+Fixed
+~~~~~
+
+* Fix well-known services not converted to UUIDs in ``BLEDevice.metadata`` in
+  CoreBluetooth backend. Fixes #342.
+* Fix advertising data replaced instead of merged in scanner in CoreBluetooth
+  backend. Merged #343.
+* Fix CBCentralManager not properly waited for during initialization in some
+  cases.
+* Fix AttributeError in CoreBluetooth when using BLEDeviceCoreBluetooth object.
+
+
 `0.9.0`_ (2020-10-20)
 ---------------------
 
 Added
 ~~~~~
 
 * Timeout for BlueZ backend connect call to avoid potential infinite hanging. Merged #306.
@@ -343,15 +371,16 @@
 
 0.1.0 (2017-10-23)
 ------------------
 
 * Bleak created.
 
 
-.. _Unreleased: https://github.com/hbldh/bleak/compare/v0.9.0...develop
+.. _Unreleased: https://github.com/hbldh/bleak/compare/v0.9.1...develop
+.. _0.9.1: https://github.com/hbldh/bleak/compare/v0.9.1...v0.9.0
 .. _0.9.0: https://github.com/hbldh/bleak/compare/v0.9.0...v0.8.0
 .. _0.8.0: https://github.com/hbldh/bleak/compare/v0.8.0...v0.7.1
 .. _0.7.1: https://github.com/hbldh/bleak/compare/v0.7.1...v0.7.0
 .. _0.7.0: https://github.com/hbldh/bleak/compare/v0.7.0...v0.6.4
 .. _0.6.4: https://github.com/hbldh/bleak/compare/v0.6.3...v0.6.4
 .. _0.6.3: https://github.com/hbldh/bleak/compare/v0.6.2...v0.6.3
 .. _0.6.2: https://github.com/hbldh/bleak/compare/v0.6.1...v0.6.2
```

### Comparing `bleak-0.9.0/CONTRIBUTING.rst` & `bleak-0.9.1/CONTRIBUTING.rst`

 * *Files 10% similar despite different names*

```diff
@@ -94,17 +94,18 @@
 7. Submit a pull request through the GitHub website.
 
 Pull Request Guidelines
 -----------------------
 
 Before you submit a pull request, check that it meets these guidelines:
 
-1. The pull request should include tests.
-2. If the pull request adds functionality, the docs should be updated. Put
-   your new functionality into a function with a docstring, and add the
-   feature to the list in README.rst.
+1. If the pull request adds functionality, the docs should be updated.
+2. Modify the ``CHANGELOG.rst``, describing your changes as is specified by the
+   guidelines in that document.
 3. The pull request should work for Python 3.6+ on the following platforms:
     - Windows 10, version 16299 (Fall Creators Update) and greater
     - Linux distributions with BlueZ >= 5.43
     - OS X / macOS >= 10.11
-4. Feel free to add your name to the ``AUTHORS.rst`` in the root of the project!
-
+4. Squash all your commits on your PR branch, if the commits are not solving
+   different problems and you are committing them in the same PR. In that case,
+   consider making several PRs instead.
+5. Feel free to add your name as a contributor to the ``AUTHORS.rst`` file!
```

### Comparing `bleak-0.9.0/LICENSE` & `bleak-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/PKG-INFO` & `bleak-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bleak
-Version: 0.9.0
+Version: 0.9.1
 Summary: Bluetooth Low Energy platform Agnostic Klient
 Home-page: https://github.com/hbldh/bleak
 Author: Henrik Blidh
 Author-email: henrik.blidh@nedomkull.com
 License: MIT
 Description: 
         =====
@@ -104,14 +104,42 @@
         =========
         
         All notable changes to this project will be documented in this file.
         
         The format is based on `Keep a Changelog <https://keepachangelog.com/en/1.0.0/>`_,
         and this project adheres to `Semantic Versioning <https://semver.org/spec/v2.0.0.html>`_.
         
+        
+        `0.9.1`_ (2020-10-22)
+        ---------------------
+        
+        Added
+        ~~~~~
+        
+        * Added new attribute ``_device_info`` on ``BleakClientBlueZDBus``. Merges #347.
+        * Added Pull Request Template.
+        
+        Changed
+        ~~~~~~~
+        
+        * Updated instructions on how to contribute, file issues and make PRs.
+        * Updated ``AUTHORS.rst`` file with development team.
+        
+        Fixed
+        ~~~~~
+        
+        * Fix well-known services not converted to UUIDs in ``BLEDevice.metadata`` in
+          CoreBluetooth backend. Fixes #342.
+        * Fix advertising data replaced instead of merged in scanner in CoreBluetooth
+          backend. Merged #343.
+        * Fix CBCentralManager not properly waited for during initialization in some
+          cases.
+        * Fix AttributeError in CoreBluetooth when using BLEDeviceCoreBluetooth object.
+        
+        
         `0.9.0`_ (2020-10-20)
         ---------------------
         
         Added
         ~~~~~
         
         * Timeout for BlueZ backend connect call to avoid potential infinite hanging. Merged #306.
@@ -444,15 +472,16 @@
         
         0.1.0 (2017-10-23)
         ------------------
         
         * Bleak created.
         
         
-        .. _Unreleased: https://github.com/hbldh/bleak/compare/v0.9.0...develop
+        .. _Unreleased: https://github.com/hbldh/bleak/compare/v0.9.1...develop
+        .. _0.9.1: https://github.com/hbldh/bleak/compare/v0.9.1...v0.9.0
         .. _0.9.0: https://github.com/hbldh/bleak/compare/v0.9.0...v0.8.0
         .. _0.8.0: https://github.com/hbldh/bleak/compare/v0.8.0...v0.7.1
         .. _0.7.1: https://github.com/hbldh/bleak/compare/v0.7.1...v0.7.0
         .. _0.7.0: https://github.com/hbldh/bleak/compare/v0.7.0...v0.6.4
         .. _0.6.4: https://github.com/hbldh/bleak/compare/v0.6.3...v0.6.4
         .. _0.6.3: https://github.com/hbldh/bleak/compare/v0.6.2...v0.6.3
         .. _0.6.2: https://github.com/hbldh/bleak/compare/v0.6.1...v0.6.2
```

### Comparing `bleak-0.9.0/README.rst` & `bleak-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/__init__.py` & `bleak-0.9.1/bleak/__init__.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/backends/_manufacturers.py` & `bleak-0.9.1/bleak/backends/_manufacturers.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/backends/bluezdbus/__init__.py` & `bleak-0.9.1/bleak/backends/bluezdbus/__init__.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/backends/bluezdbus/characteristic.py` & `bleak-0.9.1/bleak/backends/bluezdbus/characteristic.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/backends/bluezdbus/client.py` & `bleak-0.9.1/bleak/backends/bluezdbus/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,16 +50,18 @@
     def __init__(self, address_or_ble_device: Union[BLEDevice, str], **kwargs):
         super(BleakClientBlueZDBus, self).__init__(address_or_ble_device, **kwargs)
         self.device = kwargs.get("device") if kwargs.get("device") else "hci0"
 
         # Backend specific, TXDBus objects and data
         if isinstance(address_or_ble_device, BLEDevice):
             self._device_path = address_or_ble_device.details["path"]
+            self._device_info = address_or_ble_device.details.get("props")
         else:
             self._device_path = None
+            self._device_info = None
         self._bus = None
         self._reactor = None
         self._rules = {}
         self._subscriptions = list()
 
         # This maps DBus paths of GATT Characteristics to their BLE handles.
         self._char_path_to_handle = {}
@@ -88,14 +90,15 @@
         timeout = kwargs.get("timeout", self._timeout)
         if self._device_path is None:
             device = await BleakScannerBlueZDBus.find_device_by_address(
                 self.address, timeout=timeout, device=self.device
             )
 
             if device:
+                self._device_info = device.details.get("props")
                 self._device_path = device.details["path"]
             else:
                 raise BleakError(
                     "Device with address {0} was not found.".format(self.address)
                 )
 
         loop = asyncio.get_event_loop()
```

### Comparing `bleak-0.9.0/bleak/backends/bluezdbus/defs.py` & `bleak-0.9.1/bleak/backends/bluezdbus/defs.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/backends/bluezdbus/descriptor.py` & `bleak-0.9.1/bleak/backends/bluezdbus/descriptor.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/backends/bluezdbus/discovery.py` & `bleak-0.9.1/bleak/backends/bluezdbus/discovery.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/backends/bluezdbus/scanner.py` & `bleak-0.9.1/bleak/backends/bluezdbus/scanner.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/backends/bluezdbus/service.py` & `bleak-0.9.1/bleak/backends/bluezdbus/service.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/backends/bluezdbus/signals.py` & `bleak-0.9.1/bleak/backends/bluezdbus/signals.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/backends/bluezdbus/utils.py` & `bleak-0.9.1/bleak/backends/bluezdbus/utils.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/backends/characteristic.py` & `bleak-0.9.1/bleak/backends/characteristic.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/backends/client.py` & `bleak-0.9.1/bleak/backends/client.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/backends/corebluetooth/CentralManagerDelegate.py` & `bleak-0.9.1/bleak/backends/corebluetooth/CentralManagerDelegate.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 Created on June, 25 2019 by kevincar <kevincarrolldavis@gmail.com>
 
 """
 
 import asyncio
 import logging
 import platform
+import threading
 from enum import Enum
 from typing import List
 
 import objc
 from CoreBluetooth import (
     CBManagerStateUnknown,
     CBManagerStateResetting,
@@ -31,14 +32,15 @@
     NSNumber,
     NSError,
 )
 from libdispatch import dispatch_queue_create, DISPATCH_QUEUE_SERIAL
 
 from bleak.backends.corebluetooth.PeripheralDelegate import PeripheralDelegate
 from bleak.backends.corebluetooth.device import BLEDeviceCoreBluetooth
+from bleak.exc import BleakError
 
 logger = logging.getLogger(__name__)
 CBCentralManagerDelegate = objc.protocolNamed("CBCentralManagerDelegate")
 
 try:
     _mac_version = list(map(int, platform.mac_ver()[0].split(".")))
     _IS_PRE_10_13 = _mac_version[0] == 10 and _mac_version[1] < 13
@@ -66,44 +68,43 @@
             return None
 
         self.event_loop = asyncio.get_event_loop()
         self.connected_peripheral_delegate = None
         self.connected_peripheral = None
         self._connection_state = CMDConnectionState.DISCONNECTED
 
-        self.powered_on_event = asyncio.Event()
         self.devices = {}
 
         self.callbacks = {}
         self.disconnected_callback = None
         self._connection_state_changed = asyncio.Event()
 
+        self._did_update_state_event = threading.Event()
         self.central_manager = CBCentralManager.alloc().initWithDelegate_queue_(
             self, dispatch_queue_create(b"bleak.corebluetooth", DISPATCH_QUEUE_SERIAL)
         )
 
+        # according to CoreBluetooth docs, it is not valid to call CBCentral
+        # methods until the centralManagerDidUpdateState_() delegate method
+        # is called and the current state is CBManagerStatePoweredOn.
+        # It doesn't take long for the callback to occur, so we should be able
+        # to do a blocking wait here without anyone complaining.
+        self._did_update_state_event.wait(1)
+        if self.central_manager.state() != CBManagerStatePoweredOn:
+            raise BleakError("Bluetooth device is turned off")
+
         return self
 
     # User defined functions
 
     @property
     def isConnected(self) -> bool:
         return self._connection_state == CMDConnectionState.CONNECTED
 
     @objc.python_method
-    async def wait_for_powered_on(self, timeout: float):
-        """
-        Waits for state to be CBManagerStatePoweredOn. This must be done before
-        attempting to do anything else.
-
-        Throws asyncio.TimeoutError if power on is not detected before timeout.
-        """
-        await asyncio.wait_for(self.powered_on_event.wait(), timeout)
-
-    @objc.python_method
     def start_scan(self, scan_options):
         # remove old
         self.devices = {}
         service_uuids = []
         if "service_uuids" in scan_options:
             service_uuids_str = scan_options["service_uuids"]
             service_uuids = NSArray.alloc().initWithArray_(
@@ -170,40 +171,30 @@
         while self._connection_state == CMDConnectionState.PENDING:
             await asyncio.sleep(0)
 
         return self._connection_state == CMDConnectionState.DISCONNECTED
 
     # Protocol Functions
 
-    @objc.python_method
-    def did_update_state(self, centralManager):
+    def centralManagerDidUpdateState_(self, centralManager):
+        logger.debug("centralManagerDidUpdateState_")
         if centralManager.state() == CBManagerStateUnknown:
             logger.debug("Cannot detect bluetooth device")
         elif centralManager.state() == CBManagerStateResetting:
             logger.debug("Bluetooth is resetting")
         elif centralManager.state() == CBManagerStateUnsupported:
             logger.debug("Bluetooth is unsupported")
         elif centralManager.state() == CBManagerStateUnauthorized:
             logger.debug("Bluetooth is unauthorized")
         elif centralManager.state() == CBManagerStatePoweredOff:
             logger.debug("Bluetooth powered off")
         elif centralManager.state() == CBManagerStatePoweredOn:
             logger.debug("Bluetooth powered on")
 
-        if centralManager.state() == CBManagerStatePoweredOn:
-            self.powered_on_event.set()
-        else:
-            self.powered_on_event.clear()
-
-    def centralManagerDidUpdateState_(self, centralManager):
-        logger.debug("centralManagerDidUpdateState_")
-        self.event_loop.call_soon_threadsafe(
-            self.did_update_state,
-            centralManager,
-        )
+        self._did_update_state_event.set()
 
     @objc.python_method
     def did_discover_peripheral(
         self,
         central: CBCentralManager,
         peripheral: CBPeripheral,
         advertisementData: NSDictionary,
@@ -230,15 +221,15 @@
             # It could be the device did not have a name previously but now it does.
             if peripheral.name():
                 device.name = peripheral.name()
         else:
             address = uuid_string
             name = peripheral.name() or None
             details = peripheral
-            device = BLEDeviceCoreBluetooth(address, name, details)
+            device = BLEDeviceCoreBluetooth(address, name, details, delegate=self)
             self.devices[uuid_string] = device
 
         device._rssi = float(RSSI)
         device._update(advertisementData)
 
         for callback in self.callbacks.values():
             if callback:
```

### Comparing `bleak-0.9.0/bleak/backends/corebluetooth/PeripheralDelegate.py` & `bleak-0.9.1/bleak/backends/corebluetooth/PeripheralDelegate.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/backends/corebluetooth/characteristic.py` & `bleak-0.9.1/bleak/backends/corebluetooth/characteristic.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/backends/corebluetooth/client.py` & `bleak-0.9.1/bleak/backends/corebluetooth/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,17 +44,15 @@
     """
 
     def __init__(self, address_or_ble_device: Union[BLEDevice, str], **kwargs):
         super(BleakClientCoreBluetooth, self).__init__(address_or_ble_device, **kwargs)
 
         if isinstance(address_or_ble_device, BLEDevice):
             self._device_info = address_or_ble_device.details
-            self._central_manager_delegate = address_or_ble_device.metadata.get(
-                "delegate"
-            )
+            self._central_manager_delegate = address_or_ble_device.metadata["delegate"]
         else:
             self._device_info = None
             self._central_manager_delegate = None
         self._requester = None
         self._callbacks = {}
         self._services = None
 
@@ -75,15 +73,15 @@
         if self._device_info is None:
             device = await BleakScannerCoreBluetooth.find_device_by_address(
                 self.address, timeout=timeout
             )
 
             if device:
                 self._device_info = device.details
-                self._central_manager_delegate = device.metadata.get("delegate")
+                self._central_manager_delegate = device.metadata["delegate"]
             else:
                 raise BleakError(
                     "Device with address {} was not found".format(self.address)
                 )
         # self._device_info.manager() should return a CBCentralManager
 
         manager = self._central_manager_delegate
```

### Comparing `bleak-0.9.0/bleak/backends/corebluetooth/descriptor.py` & `bleak-0.9.1/bleak/backends/corebluetooth/descriptor.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/backends/corebluetooth/device.py` & `bleak-0.9.1/bleak/backends/corebluetooth/device.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 from bleak.backends._manufacturers import MANUFACTURERS
 
 from Foundation import NSDictionary
 
-
+from bleak.backends.corebluetooth.utils import cb_uuid_to_str
 from bleak.backends.device import BLEDevice
 
 
 class BLEDeviceCoreBluetooth(BLEDevice):
     """
     A CoreBlutooth class representing a BLE server detected during
     a `discover` call.
 
     - The `details` attribute will be a CBPeripheral object.
 
-    - The `metadata` keys are more or less part of the crossplattform interface.
+    - The `metadata` keys are more or less part of the cross-platform interface.
 
     - Note: Take care not to rely on any reference to `advertisementData` and
       it's data as lower layers of the corebluetooth stack can change it. i.e.
       only valid/trusted in callback(s) or if copied.
 
     - AdvertisementData fields/keys that might be of interest:
       - kCBAdvDataAppleMfgData
@@ -31,27 +31,25 @@
       - kCBAdvDataLocalName
       - kCBAdvDataServiceUUIDs
       - kCBAdvDataManufacturerData
     """
 
     def __init__(self, *args, **kwargs):
         super(BLEDeviceCoreBluetooth, self).__init__(*args, **kwargs)
-        self.metadata = {}
         self._rssi = kwargs.get("rssi")
 
     def _update(self, advertisementData: NSDictionary):
         self._update_uuids(advertisementData)
         self._update_manufacturer(advertisementData)
 
     def _update_uuids(self, advertisementData: NSDictionary):
         cbuuids = advertisementData.get("kCBAdvDataServiceUUIDs", [])
         if not cbuuids:
             return
-        # converting to lower case to match other platforms
-        chuuids = [str(u).lower() for u in cbuuids]
+        chuuids = [cb_uuid_to_str(u) for u in cbuuids]
         if "uuids" in self.metadata:
             for uuid in chuuids:
                 if not uuid in self.metadata["uuids"]:
                     self.metadata["uuids"].append(uuid)
         else:
             self.metadata["uuids"] = chuuids
```

### Comparing `bleak-0.9.0/bleak/backends/corebluetooth/discovery.py` & `bleak-0.9.1/bleak/backends/corebluetooth/discovery.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,35 +3,28 @@
 
 macOS
 
 Created on 2019-06-24 by kevincar <kevincarrolldavis@gmail.com>
 
 """
 
-import asyncio
 from typing import List
 
 from bleak.backends.corebluetooth.CentralManagerDelegate import CentralManagerDelegate
 from bleak.backends.device import BLEDevice
-from bleak.exc import BleakError
 
 
 async def discover(timeout: float = 5.0, **kwargs) -> List[BLEDevice]:
     """Perform a Bluetooth LE Scan.
 
     Args:
         timeout (float): duration of scanning period
 
     """
     manager = CentralManagerDelegate.alloc().init()
-    try:
-        await manager.wait_for_powered_on(0.1)
-    except asyncio.TimeoutError:
-        raise BleakError("Bluetooth device is turned off")
-
     scan_options = {"timeout": timeout}
 
     await manager.scanForPeripherals_(scan_options)
 
     # CoreBluetooth doesn't explicitly use Bluetooth addresses to identify peripheral
     # devices because private devices may obscure their Bluetooth addresses. To cope
     # with this, CoreBluetooth utilizes UUIDs for each peripheral. We'll use
```

### Comparing `bleak-0.9.0/bleak/backends/corebluetooth/scanner.py` & `bleak-0.9.1/bleak/backends/corebluetooth/scanner.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 import asyncio
 import pathlib
 import uuid
 from typing import Callable, Any, Union, List
 
 from bleak.backends.corebluetooth.CentralManagerDelegate import CentralManagerDelegate
+from bleak.backends.corebluetooth.utils import cb_uuid_to_str
 from bleak.backends.device import BLEDevice
-from bleak.exc import BleakError
 from bleak.backends.scanner import BaseBleakScanner
 
 
 logger = logging.getLogger(__name__)
 _here = pathlib.Path(__file__).parent
 
 
@@ -35,23 +35,19 @@
         super(BleakScannerCoreBluetooth, self).__init__(**kwargs)
         self._callback = None
         self._identifiers = None
         self._manager = CentralManagerDelegate.alloc().init()
         self._timeout = kwargs.get("timeout", 5.0)
 
     async def start(self):
-        try:
-            await self._manager.wait_for_powered_on(0.1)
-        except asyncio.TimeoutError:
-            raise BleakError("Bluetooth device is turned off")
-
         self._identifiers = {}
 
         def callback(p, a, r):
-            self._identifiers[p.identifier()] = a
+            # update identifiers for scanned device
+            self._identifiers.setdefault(p.identifier(), {}).update(a)
             if self._callback:
                 self._callback(p, a, r)
 
         self._manager.callbacks[id(self)] = callback
         self._manager.start_scan({})
 
     async def stop(self):
@@ -97,16 +93,15 @@
                 manufacturer_id = int.from_bytes(
                     manufacturer_binary_data[0:2], byteorder="little"
                 )
                 manufacturer_value = bytes(manufacturer_binary_data[2:])
                 manufacturer_data = {manufacturer_id: manufacturer_value}
 
             uuids = [
-                # converting to lower case to match other platforms
-                str(u).lower()
+                cb_uuid_to_str(u)
                 for u in advertisementData.get("kCBAdvDataServiceUUIDs", [])
             ]
 
             found.append(
                 BLEDevice(
                     address,
                     name,
```

### Comparing `bleak-0.9.0/bleak/backends/corebluetooth/service.py` & `bleak-0.9.1/bleak/backends/corebluetooth/service.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/backends/corebluetooth/utils.py` & `bleak-0.9.1/bleak/backends/corebluetooth/utils.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/backends/descriptor.py` & `bleak-0.9.1/bleak/backends/descriptor.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/backends/device.py` & `bleak-0.9.1/bleak/backends/device.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/backends/dotnet/BleakUWPBridge.dll` & `bleak-0.9.1/bleak/backends/dotnet/BleakUWPBridge.dll`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/backends/dotnet/characteristic.py` & `bleak-0.9.1/bleak/backends/dotnet/characteristic.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/backends/dotnet/client.py` & `bleak-0.9.1/bleak/backends/dotnet/client.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/backends/dotnet/descriptor.py` & `bleak-0.9.1/bleak/backends/dotnet/descriptor.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/backends/dotnet/discovery.py` & `bleak-0.9.1/bleak/backends/dotnet/discovery.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/backends/dotnet/scanner.py` & `bleak-0.9.1/bleak/backends/dotnet/scanner.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/backends/dotnet/service.py` & `bleak-0.9.1/bleak/backends/dotnet/service.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/backends/dotnet/utils.py` & `bleak-0.9.1/bleak/backends/dotnet/utils.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/backends/scanner.py` & `bleak-0.9.1/bleak/backends/scanner.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/backends/service.py` & `bleak-0.9.1/bleak/backends/service.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/exc.py` & `bleak-0.9.1/bleak/exc.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/utils.py` & `bleak-0.9.1/bleak/utils.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak/uuids.py` & `bleak-0.9.1/bleak/uuids.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/bleak.egg-info/PKG-INFO` & `bleak-0.9.1/bleak.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bleak
-Version: 0.9.0
+Version: 0.9.1
 Summary: Bluetooth Low Energy platform Agnostic Klient
 Home-page: https://github.com/hbldh/bleak
 Author: Henrik Blidh
 Author-email: henrik.blidh@nedomkull.com
 License: MIT
 Description: 
         =====
@@ -104,14 +104,42 @@
         =========
         
         All notable changes to this project will be documented in this file.
         
         The format is based on `Keep a Changelog <https://keepachangelog.com/en/1.0.0/>`_,
         and this project adheres to `Semantic Versioning <https://semver.org/spec/v2.0.0.html>`_.
         
+        
+        `0.9.1`_ (2020-10-22)
+        ---------------------
+        
+        Added
+        ~~~~~
+        
+        * Added new attribute ``_device_info`` on ``BleakClientBlueZDBus``. Merges #347.
+        * Added Pull Request Template.
+        
+        Changed
+        ~~~~~~~
+        
+        * Updated instructions on how to contribute, file issues and make PRs.
+        * Updated ``AUTHORS.rst`` file with development team.
+        
+        Fixed
+        ~~~~~
+        
+        * Fix well-known services not converted to UUIDs in ``BLEDevice.metadata`` in
+          CoreBluetooth backend. Fixes #342.
+        * Fix advertising data replaced instead of merged in scanner in CoreBluetooth
+          backend. Merged #343.
+        * Fix CBCentralManager not properly waited for during initialization in some
+          cases.
+        * Fix AttributeError in CoreBluetooth when using BLEDeviceCoreBluetooth object.
+        
+        
         `0.9.0`_ (2020-10-20)
         ---------------------
         
         Added
         ~~~~~
         
         * Timeout for BlueZ backend connect call to avoid potential infinite hanging. Merged #306.
@@ -444,15 +472,16 @@
         
         0.1.0 (2017-10-23)
         ------------------
         
         * Bleak created.
         
         
-        .. _Unreleased: https://github.com/hbldh/bleak/compare/v0.9.0...develop
+        .. _Unreleased: https://github.com/hbldh/bleak/compare/v0.9.1...develop
+        .. _0.9.1: https://github.com/hbldh/bleak/compare/v0.9.1...v0.9.0
         .. _0.9.0: https://github.com/hbldh/bleak/compare/v0.9.0...v0.8.0
         .. _0.8.0: https://github.com/hbldh/bleak/compare/v0.8.0...v0.7.1
         .. _0.7.1: https://github.com/hbldh/bleak/compare/v0.7.1...v0.7.0
         .. _0.7.0: https://github.com/hbldh/bleak/compare/v0.7.0...v0.6.4
         .. _0.6.4: https://github.com/hbldh/bleak/compare/v0.6.3...v0.6.4
         .. _0.6.3: https://github.com/hbldh/bleak/compare/v0.6.2...v0.6.3
         .. _0.6.2: https://github.com/hbldh/bleak/compare/v0.6.1...v0.6.2
```

### Comparing `bleak-0.9.0/bleak.egg-info/SOURCES.txt` & `bleak-0.9.1/bleak.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/docs/Makefile` & `bleak-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/docs/api.rst` & `bleak-0.9.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/docs/backends/linux.rst` & `bleak-0.9.1/docs/backends/linux.rst`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/docs/backends/macos.rst` & `bleak-0.9.1/docs/backends/macos.rst`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/docs/backends/windows.rst` & `bleak-0.9.1/docs/backends/windows.rst`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/docs/conf.py` & `bleak-0.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/docs/images/win-10-start-cmd-as-admin.png` & `bleak-0.9.1/docs/images/win-10-start-cmd-as-admin.png`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/docs/index.rst` & `bleak-0.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/docs/installation.rst` & `bleak-0.9.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/docs/make.bat` & `bleak-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/docs/scanning.rst` & `bleak-0.9.1/docs/scanning.rst`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/docs/troubleshooting.rst` & `bleak-0.9.1/docs/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/docs/usage.rst` & `bleak-0.9.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/setup.py` & `bleak-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `bleak-0.9.0/tests/test_imports.py` & `bleak-0.9.1/tests/test_imports.py`

 * *Files identical despite different names*

