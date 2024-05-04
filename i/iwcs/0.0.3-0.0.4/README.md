# Comparing `tmp/iwcs-0.0.3.tar.gz` & `tmp/iwcs-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iwcs-0.0.3.tar", last modified: Wed Apr 17 15:52:48 2024, max compression
+gzip compressed data, was "iwcs-0.0.4.tar", last modified: Sat May  4 14:16:04 2024, max compression
```

## Comparing `iwcs-0.0.3.tar` & `iwcs-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:52:48.369680 iwcs-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-17 15:52:45.000000 iwcs-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-17 15:52:48.369680 iwcs-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-17 15:52:45.000000 iwcs-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:52:48.365680 iwcs-0.0.3/iwcs/
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-17 15:52:45.000000 iwcs-0.0.3/iwcs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:52:48.369680 iwcs-0.0.3/iwcs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-17 15:52:48.000000 iwcs-0.0.3/iwcs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-17 15:52:48.000000 iwcs-0.0.3/iwcs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 15:52:48.000000 iwcs-0.0.3/iwcs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-17 15:52:48.000000 iwcs-0.0.3/iwcs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 15:52:48.369680 iwcs-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-17 15:52:45.000000 iwcs-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:16:04.333445 iwcs-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-04 14:16:00.000000 iwcs-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-04 14:16:04.333445 iwcs-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-04 14:16:00.000000 iwcs-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:16:04.333445 iwcs-0.0.4/iwcs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-04 14:16:00.000000 iwcs-0.0.4/iwcs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 14:16:04.333445 iwcs-0.0.4/iwcs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-04 14:16:04.000000 iwcs-0.0.4/iwcs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-04 14:16:04.000000 iwcs-0.0.4/iwcs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 14:16:04.000000 iwcs-0.0.4/iwcs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-04 14:16:04.000000 iwcs-0.0.4/iwcs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 14:16:04.333445 iwcs-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-04 14:16:00.000000 iwcs-0.0.4/setup.py
```

### Comparing `iwcs-0.0.3/LICENSE` & `iwcs-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iwcs-0.0.3/PKG-INFO` & `iwcs-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iwcs
-Version: 0.0.3
+Version: 0.0.4
 Summary: iw client stats, get connected wireless client connection statistics
 Home-page: https://github.com/manbehindthemadness/iwcs
 Author: Manbehindthemadness
 Author-email: manbehindthemadness@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iwcs-0.0.3/README.md` & `iwcs-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `iwcs-0.0.3/iwcs/__init__.py` & `iwcs-0.0.4/iwcs/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 import subprocess
 from pathlib import Path
 
-
 if not Path('/sbin/iw').is_file():
     raise FileNotFoundError('command `iw` not found, please run `sudo apt-get install iw`')
 
 
 def mac(mac_address: str, interface: str = 'wlan0') -> dict:
     """
     Gather the information in relation to a single sensor by MAC address.
     """
     client_info_dict = dict()
     try:
         client_info_output = subprocess.check_output(
-            ["/sbin/iw", "dev", interface, "station", "get", mac_address]
+            ["/sbin/iw", "dev", interface, "station", "get", mac_address],
+            stderr=subprocess.DEVNULL,  # Silence stderr
         ).decode(
             "utf-8")
         client_info_lines = client_info_output.split("\n")
         client_info_dict = {}
-        for line in client_info_lines:
-            if ":" in line:
-                key, value = line.split(":", 1)
-                client_info_dict[key.strip()] = value.strip()
+        if client_info_lines[0]:
+            for line in client_info_lines:
+                if ":" in line:
+                    key, value = line.split(":", 1)
+                    client_info_dict[key.strip()] = value.strip()
     except subprocess.CalledProcessError:
         print(f'client {mac_address} not found on interface {interface}')
     return client_info_dict
 
 
 def info(interface: str = 'wlan0') -> dict:
     """
     This will grab the connection stats of the clients connected to the specified interface.
 
     returns: {'<MAC ADDRESS>': {'inactive time': <value>, 'rx bytes': <value>, ...}}
     """
-    mac_addresses_output = subprocess.check_output(["/sbin/iw", "dev", interface, "station", "dump"]).decode("utf-8")
+    mac_addresses_output = subprocess.check_output(["/sbin/iw", "dev", interface, "station", "dump"],
+                                                   stderr=subprocess.DEVNULL).decode("utf-8")
     mac_addresses_list = [line.split()[1] for line in mac_addresses_output.split("\n") if "Station" in line]
     clients_info = {}
     for mac_address in mac_addresses_list:
         client_info_dict = mac(mac_address, interface)
         clients_info[mac_address] = client_info_dict
     return clients_info
```

### Comparing `iwcs-0.0.3/iwcs.egg-info/PKG-INFO` & `iwcs-0.0.4/iwcs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iwcs
-Version: 0.0.3
+Version: 0.0.4
 Summary: iw client stats, get connected wireless client connection statistics
 Home-page: https://github.com/manbehindthemadness/iwcs
 Author: Manbehindthemadness
 Author-email: manbehindthemadness@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `iwcs-0.0.3/setup.py` & `iwcs-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name='iwcs',
-    version='0.0.3',
+    version='0.0.4',
     packages=find_packages(),
     install_requires=[],
     entry_points={
         'console_scripts': [
         ],
     },
     author='Manbehindthemadness',
```

