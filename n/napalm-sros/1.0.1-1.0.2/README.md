# Comparing `tmp/napalm-sros-1.0.1.tar.gz` & `tmp/napalm_sros-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napalm-sros-1.0.1.tar", last modified: Fri Oct 27 17:08:40 2023, max compression
+gzip compressed data, was "napalm_sros-1.0.2.tar", last modified: Sat May  4 05:16:04 2024, max compression
```

## Comparing `napalm-sros-1.0.1.tar` & `napalm_sros-1.0.2.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxrwxr-x   0 jeroen    (1000) jeroen    (1000)        0 2023-10-27 17:08:40.661958 napalm-sros-1.0.1/
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      120 2023-05-26 15:13:45.000000 napalm-sros-1.0.1/AUTHORS
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)    11357 2023-05-26 15:13:45.000000 napalm-sros-1.0.1/LICENSE
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      110 2023-05-26 15:13:45.000000 napalm-sros-1.0.1/MANIFEST.in
--rw-r--r--   0 jeroen    (1000) jeroen    (1000)     3597 2023-10-27 17:08:40.661958 napalm-sros-1.0.1/PKG-INFO
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)     2102 2023-05-26 15:13:45.000000 napalm-sros-1.0.1/README.md
-drwxrwxr-x   0 jeroen    (1000) jeroen    (1000)        0 2023-10-27 17:08:40.657958 napalm-sros-1.0.1/napalm_sros/
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      737 2023-05-26 15:13:45.000000 napalm-sros-1.0.1/napalm_sros/__init__.py
-drwxrwxr-x   0 jeroen    (1000) jeroen    (1000)        0 2023-10-27 17:08:40.657958 napalm-sros-1.0.1/napalm_sros/api/
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      827 2023-06-01 21:38:46.000000 napalm-sros-1.0.1/napalm_sros/api/__init__.py
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)     5714 2023-06-26 21:39:04.000000 napalm-sros-1.0.1/napalm_sros/api/get_bgp_neighbors.py
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)     7346 2023-06-26 21:39:04.000000 napalm-sros-1.0.1/napalm_sros/api/get_bgp_neighbors_detail.py
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)     2472 2023-05-26 15:13:45.000000 napalm-sros-1.0.1/napalm_sros/api/util.py
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)    22297 2023-06-26 21:39:04.000000 napalm-sros-1.0.1/napalm_sros/nc_filters.py
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)   159221 2023-10-21 18:31:32.000000 napalm-sros-1.0.1/napalm_sros/sros.py
-drwxrwxr-x   0 jeroen    (1000) jeroen    (1000)        0 2023-10-27 17:08:40.661958 napalm-sros-1.0.1/napalm_sros/templates/
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)        0 2023-10-27 17:07:50.000000 napalm-sros-1.0.1/napalm_sros/templates/__init__.py
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)       60 2023-05-26 15:13:45.000000 napalm-sros-1.0.1/napalm_sros/templates/set_hostname.j2
-drwxrwxr-x   0 jeroen    (1000) jeroen    (1000)        0 2023-10-27 17:08:40.661958 napalm-sros-1.0.1/napalm_sros/utils/
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)       28 2023-05-26 15:13:45.000000 napalm-sros-1.0.1/napalm_sros/utils/__init__.py
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)     1551 2023-05-26 15:13:45.000000 napalm-sros-1.0.1/napalm_sros/utils/parse_output_to_dict.py
-drwxrwxr-x   0 jeroen    (1000) jeroen    (1000)        0 2023-10-27 17:08:40.661958 napalm-sros-1.0.1/napalm_sros/utils/textfsm_templates/
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)        0 2023-10-27 17:07:50.000000 napalm-sros-1.0.1/napalm_sros/utils/textfsm_templates/__init__.py
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      478 2023-05-26 15:13:45.000000 napalm-sros-1.0.1/napalm_sros/utils/textfsm_templates/nokia_sros_show_service_fdb_mac.tpl
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      408 2023-05-26 15:13:45.000000 napalm-sros-1.0.1/napalm_sros/utils/utils.py
-drwxrwxr-x   0 jeroen    (1000) jeroen    (1000)        0 2023-10-27 17:08:40.657958 napalm-sros-1.0.1/napalm_sros.egg-info/
--rw-r--r--   0 jeroen    (1000) jeroen    (1000)     3597 2023-10-27 17:08:40.000000 napalm-sros-1.0.1/napalm_sros.egg-info/PKG-INFO
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      756 2023-10-27 17:08:40.000000 napalm-sros-1.0.1/napalm_sros.egg-info/SOURCES.txt
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)        1 2023-10-27 17:08:40.000000 napalm-sros-1.0.1/napalm_sros.egg-info/dependency_links.txt
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      184 2023-10-27 17:08:40.000000 napalm-sros-1.0.1/napalm_sros.egg-info/requires.txt
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)       12 2023-10-27 17:08:40.000000 napalm-sros-1.0.1/napalm_sros.egg-info/top_level.txt
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)     1184 2023-10-27 17:07:50.000000 napalm-sros-1.0.1/pyproject.toml
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      163 2023-10-27 16:19:48.000000 napalm-sros-1.0.1/requirements.txt
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      438 2023-10-27 17:08:40.661958 napalm-sros-1.0.1/setup.cfg
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)     1321 2023-10-27 17:07:50.000000 napalm-sros-1.0.1/setup.py
+drwxrwxr-x   0 jeroen    (1000) jeroen    (1000)        0 2024-05-04 05:16:04.202287 napalm_sros-1.0.2/
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      120 2023-05-26 15:13:45.000000 napalm_sros-1.0.2/AUTHORS
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)    11357 2023-05-26 15:13:45.000000 napalm_sros-1.0.2/LICENSE
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      110 2023-05-26 15:13:45.000000 napalm_sros-1.0.2/MANIFEST.in
+-rw-r--r--   0 jeroen    (1000) jeroen    (1000)     3609 2024-05-04 05:16:04.202287 napalm_sros-1.0.2/PKG-INFO
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)     2113 2024-05-04 04:56:36.000000 napalm_sros-1.0.2/README.md
+drwxrwxr-x   0 jeroen    (1000) jeroen    (1000)        0 2024-05-04 05:16:04.198287 napalm_sros-1.0.2/napalm_sros/
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      737 2023-05-26 15:13:45.000000 napalm_sros-1.0.2/napalm_sros/__init__.py
+drwxrwxr-x   0 jeroen    (1000) jeroen    (1000)        0 2024-05-04 05:16:04.198287 napalm_sros-1.0.2/napalm_sros/api/
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      827 2023-06-01 21:38:46.000000 napalm_sros-1.0.2/napalm_sros/api/__init__.py
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)     5714 2023-06-26 21:39:04.000000 napalm_sros-1.0.2/napalm_sros/api/get_bgp_neighbors.py
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)     7346 2023-06-26 21:39:04.000000 napalm_sros-1.0.2/napalm_sros/api/get_bgp_neighbors_detail.py
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)     2472 2023-05-26 15:13:45.000000 napalm_sros-1.0.2/napalm_sros/api/util.py
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)    22297 2023-06-26 21:39:04.000000 napalm_sros-1.0.2/napalm_sros/nc_filters.py
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)   159243 2024-05-04 05:05:54.000000 napalm_sros-1.0.2/napalm_sros/sros.py
+drwxrwxr-x   0 jeroen    (1000) jeroen    (1000)        0 2024-05-04 05:16:04.198287 napalm_sros-1.0.2/napalm_sros/templates/
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)        0 2023-12-06 16:07:19.000000 napalm_sros-1.0.2/napalm_sros/templates/__init__.py
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)       60 2023-05-26 15:13:45.000000 napalm_sros-1.0.2/napalm_sros/templates/set_hostname.j2
+drwxrwxr-x   0 jeroen    (1000) jeroen    (1000)        0 2024-05-04 05:16:04.198287 napalm_sros-1.0.2/napalm_sros/utils/
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)       28 2023-05-26 15:13:45.000000 napalm_sros-1.0.2/napalm_sros/utils/__init__.py
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)     1551 2023-05-26 15:13:45.000000 napalm_sros-1.0.2/napalm_sros/utils/parse_output_to_dict.py
+drwxrwxr-x   0 jeroen    (1000) jeroen    (1000)        0 2024-05-04 05:16:04.198287 napalm_sros-1.0.2/napalm_sros/utils/textfsm_templates/
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)        0 2023-12-06 16:07:19.000000 napalm_sros-1.0.2/napalm_sros/utils/textfsm_templates/__init__.py
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      478 2023-05-26 15:13:45.000000 napalm_sros-1.0.2/napalm_sros/utils/textfsm_templates/nokia_sros_show_service_fdb_mac.tpl
+drwxrwxr-x   0 jeroen    (1000) jeroen    (1000)        0 2024-05-04 05:16:04.202287 napalm_sros-1.0.2/napalm_sros.egg-info/
+-rw-r--r--   0 jeroen    (1000) jeroen    (1000)     3609 2024-05-04 05:16:04.000000 napalm_sros-1.0.2/napalm_sros.egg-info/PKG-INFO
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      729 2024-05-04 05:16:04.000000 napalm_sros-1.0.2/napalm_sros.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)        1 2024-05-04 05:16:04.000000 napalm_sros-1.0.2/napalm_sros.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      184 2024-05-04 05:16:04.000000 napalm_sros-1.0.2/napalm_sros.egg-info/requires.txt
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)       12 2024-05-04 05:16:04.000000 napalm_sros-1.0.2/napalm_sros.egg-info/top_level.txt
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)     1185 2024-05-04 05:09:55.000000 napalm_sros-1.0.2/pyproject.toml
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      163 2024-05-04 04:56:33.000000 napalm_sros-1.0.2/requirements.txt
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      438 2024-05-04 05:16:04.202287 napalm_sros-1.0.2/setup.cfg
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)     1322 2024-05-04 05:08:49.000000 napalm_sros-1.0.2/setup.py
```

### Comparing `napalm-sros-1.0.1/LICENSE` & `napalm_sros-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napalm-sros-1.0.1/PKG-INFO` & `napalm_sros-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: napalm-sros
-Version: 1.0.1
+Version: 1.0.2
 Summary: Network Automation and Programmability Abstraction Layer driver for Nokia SR OS
 Home-page: https://github.com/napalm-automation/napalm-sros
 Author: Nokia
 Author-email: Ashna Shah <ashna.shah@nokia.com>, Roman Dodin <roman.dodin@nokia.com>, Patryk Szulczewski <patryk.szulczewski@nokia.com>, Jeroen van Bemmel <jeroen.van_bemmel@nokia.com>
 Project-URL: Homepage, https://github.com/napalm-automation-community/napalm-sros
 Project-URL: Bug Tracker, https://github.com/napalm-automation-community/napalm-sros/issues
 Classifier: Topic :: System :: Networking
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Natural Language :: English
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: napalm>=4.0.0
 Requires-Dist: pytest>=7.0.1
 Requires-Dist: setuptools>=47.3.1
 Requires-Dist: pip>=21.3.1
 Requires-Dist: textfsm
 Requires-Dist: paramiko>=2.11.0
 Requires-Dist: lxml>=4.9.1
-Requires-Dist: ncclient>=0.6.13
+Requires-Dist: ncclient>=0.6.15
 Requires-Dist: xmltodict>=0.12.0
 Requires-Dist: dictdiffer>=0.9.0
 Requires-Dist: datetime>=4.7
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: ruff; extra == "tests"
 
@@ -50,17 +50,17 @@
 2) The main files included for Nokia SR OS driver are:
      3) napalm_sros/sros.py: Overridden NAPALM methods to get the expected output from SR OS
      4) napalm_sros/nc_filters.py: Filters defined to get data from SR OS using a NETCONF connection
 5) Mapping of various parameters of NAPALM output to Nokia SR OS can be found in this [Mapping Document](https://github.com/napalm-automation-community/napalm-sros/blob/master/Summary_of_Methods.pdf)
 6) For testing, please refer to [Test Document](https://github.com/napalm-automation-community/napalm-sros/blob/master/README_TEST.md)
 
 #### **Components Version**
-1) Python - 3.6
+1) Python - 3.8 or higher
 2) ncclient >= 0.6.13
 3) paramiko >= 2.11.0
-4) NAPALM >= 3.4.1
+4) NAPALM >= 4.0.0
 
 ##### **Note**
-This version of the driver leverages Nokia’s defined YANG models for configuration and state trees for the SROS platform. While SROS also support limited configuration and state retrieval using openconfig standard models, the NAPALM driver does not support configuration or state retrieval of openconfig data models.
+This version of the driver leverages Nokia’s defined YANG models for configuration and state trees for the SROS platform. While SROS also supports limited configuration and state retrieval using openconfig standard models, the NAPALM driver does not support configuration or state retrieval of openconfig data models.
 
 #### License
 This project is licensed under the Apache-2.0 license - see the [LICENSE](LICENSE) file.
```

### Comparing `napalm-sros-1.0.1/README.md` & `napalm_sros-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 2) The main files included for Nokia SR OS driver are:
      3) napalm_sros/sros.py: Overridden NAPALM methods to get the expected output from SR OS
      4) napalm_sros/nc_filters.py: Filters defined to get data from SR OS using a NETCONF connection
 5) Mapping of various parameters of NAPALM output to Nokia SR OS can be found in this [Mapping Document](https://github.com/napalm-automation-community/napalm-sros/blob/master/Summary_of_Methods.pdf)
 6) For testing, please refer to [Test Document](https://github.com/napalm-automation-community/napalm-sros/blob/master/README_TEST.md)
 
 #### **Components Version**
-1) Python - 3.6
+1) Python - 3.8 or higher
 2) ncclient >= 0.6.13
 3) paramiko >= 2.11.0
-4) NAPALM >= 3.4.1
+4) NAPALM >= 4.0.0
 
 ##### **Note**
-This version of the driver leverages Nokia’s defined YANG models for configuration and state trees for the SROS platform. While SROS also support limited configuration and state retrieval using openconfig standard models, the NAPALM driver does not support configuration or state retrieval of openconfig data models.
+This version of the driver leverages Nokia’s defined YANG models for configuration and state trees for the SROS platform. While SROS also supports limited configuration and state retrieval using openconfig standard models, the NAPALM driver does not support configuration or state retrieval of openconfig data models.
 
 #### License
 This project is licensed under the Apache-2.0 license - see the [LICENSE](LICENSE) file.
```

### Comparing `napalm-sros-1.0.1/napalm_sros/__init__.py` & `napalm_sros-1.0.2/napalm_sros/__init__.py`

 * *Files identical despite different names*

### Comparing `napalm-sros-1.0.1/napalm_sros/api/__init__.py` & `napalm_sros-1.0.2/napalm_sros/api/__init__.py`

 * *Files identical despite different names*

### Comparing `napalm-sros-1.0.1/napalm_sros/api/get_bgp_neighbors.py` & `napalm_sros-1.0.2/napalm_sros/api/get_bgp_neighbors.py`

 * *Files identical despite different names*

### Comparing `napalm-sros-1.0.1/napalm_sros/api/get_bgp_neighbors_detail.py` & `napalm_sros-1.0.2/napalm_sros/api/get_bgp_neighbors_detail.py`

 * *Files identical despite different names*

### Comparing `napalm-sros-1.0.1/napalm_sros/api/util.py` & `napalm_sros-1.0.2/napalm_sros/api/util.py`

 * *Files identical despite different names*

### Comparing `napalm-sros-1.0.1/napalm_sros/nc_filters.py` & `napalm_sros-1.0.2/napalm_sros/nc_filters.py`

 * *Files identical despite different names*

### Comparing `napalm-sros-1.0.1/napalm_sros/sros.py` & `napalm_sros-1.0.2/napalm_sros/sros.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 """
 Napalm driver for SROS.
 """
 # import standard library
 import json
 import time
 import re
-import logging
 import datetime
 import traceback
 import xmltodict
 from dictdiffer import diff
 import paramiko
 
 # import NAPALM libraries
@@ -37,14 +36,16 @@
 
 from napalm.base import NetworkDriver
 from napalm.base.exceptions import (
     ConnectionException,
     SessionLockedException,
     MergeConfigException,
     ReplaceConfigException,
+    CommitError,
+    CommandErrorException,
 )
 from napalm.base.helpers import convert, ip, as_number
 import napalm.base.constants as C
 
 # import third party libraries
 from ncclient import manager
 from ncclient.xml_ import to_ele, to_xml
@@ -52,19 +53,19 @@
 # import local modules
 from napalm_sros.utils.parse_output_to_dict import parse_with_textfsm
 from napalm_sros.nc_filters import GET_ARP_TABLE,GET_BGP_CONFIG,GET_ENVIRONMENT, \
      GET_FACTS,GET_INTERFACES,GET_INTERFACES_COUNTERS,GET_INTERFACES_IP, \
      GET_IPV6_NEIGHBORS_TABLE,GET_LLDP_NEIGHBORS,GET_LLDP_NEIGHBORS_DETAIL, \
      GET_NETWORK_INSTANCES,GET_NTP_PEERS,GET_NTP_SERVERS,GET_OPTICS, \
      GET_PROBES_CONFIG,GET_ROUTE_TO,GET_SNMP_INFORMATION,GET_USERS
-from napalm_sros.utils.utils import init_logging
 
 from .api import get_bgp_neighbors, get_bgp_neighbors_detail
+import logging
 
-log = init_logging()
+log = logging.getLogger(__file__)
 
 class NokiaSROSDriver(NetworkDriver):
     """Napalm driver for Skeleton."""
 
     def __init__(self, hostname, username, password, timeout=60, optional_args=None):
         """Constructor."""
         self.manager = None
@@ -291,22 +292,22 @@
                 if isinstance(xpath_result, type(xml_tree)):
                     if xpath_result.text is not None:
                         value = xpath_result.text.strip()
                 else:
                     value = xpath_result
             else:
                 if xpath_applied == "":
-                    logging.error(
+                    log.error(
                         "Unable to find the specified-text-element/XML path: %s in  \
                             the XML tree provided. Total Items in XML tree: %d "
                         % (path, xpath_length)
                     )
         except Exception as e:  # in case of any exception, returns default
             print("Error while finding text in xml: {}".format(e))
-            logging.error("Error while finding text in xml: %s" % traceback.format_exc())
+            log.error("Error while finding text in xml: %s" % traceback.format_exc())
             value = default
         return str(value)
 
     def is_alive(self):
         """
         Returns a flag with the connection state. Depends on the nature of API used by each driver.
         The state does not reflect only on the connection status (when SSH), it must also take into
@@ -319,15 +320,15 @@
             if self.conn is not None and self.conn_ssh is not None:
                 is_alive_dict.update({"is_alive": True})
             else:
                 is_alive_dict.update({"is_alive": False})
             return is_alive_dict
         except Exception as e:  # in case of any exception, returns default
             print("Error occurred in is_alive method: {}".format(e))
-            logging.error("Error occurred in is_alive: %s" % traceback.format_exc())
+            log.error("Error occurred in is_alive: %s" % traceback.format_exc())
 
     def discard_config(self):
         """
         Discards the configuration loaded into the candidate.
         """
         if self.fmt == "xml":
             self.conn.discard_changes()
@@ -341,22 +342,21 @@
         Commits the changes requested by the method load_replace_candidate or load_merge_candidate.
         """
         if self.fmt == "text":
             buff = self._perform_cli_commands(["commit"], True)
             # If error while performing commit, return the error
             error = ""
             for item in buff.split("\n"):
-                if self.cmd_line_pattern_re.search(item):
-                    continue
                 if any(match.search(item) for match in self.terminal_stderr_re):
                     row = item.strip()
                     row_list = row.split(": ")
                     error += row_list[2]
             if error:
-                print("Error while commit: ", error)
+                log.error(f"Error during commit: {error}")
+                raise CommitError(error)
         elif self.fmt == "xml":
             self.conn.commit()
             if not self.lock_disable and not self.session_config_lock:
                 self._unlock_config()
 
     def rollback(self):
         """
@@ -371,16 +371,16 @@
                 if "MINOR: CLI #2069" in item:
                     continue
                 elif any(match.search(item) for match in self.terminal_stderr_re):
                     row = item.strip()
                     row_list = row.split(": ")
                     error += row_list[2]
                 if error:
-                    print("Error while rollback: ", error)
-                    break
+                    log.error(f"Error during rollback: {error}")
+                    raise CommandErrorException(error)
 
     def compare_config(self):
         """
         :return: A string showing the difference between the running configuration and the candidate
         configuration. The running_config is loaded automatically just before doing the comparison
         so there is no need for you to do it.
         """
@@ -547,14 +547,15 @@
             configuration.insert(0, "edit-config exclusive")
             configuration.insert(1, "delete configure")
             buff = self._perform_cli_commands(configuration, False)
             # error checking
             if buff is not None:
                 for item in buff.split("\n"):
                     if any(match.search(item) for match in self.terminal_stderr_re):
+                        log.error( f"Replace issue: {item}" )
                         raise ReplaceConfigException("Replace issue: %s", item)
             else:
                 raise ReplaceConfigException("Timeout during load_replace_candidate")
 
     def get_facts(self):
         """
             Returns a dictionary containing the following information:
@@ -1100,14 +1101,15 @@
             log.error("Error in method get network instances : %s", traceback.format_exc())
 
     def get_config(
         self,
         retrieve="all",
         full=False,
         sanitized=False,
+        format="text",
     ):
         """
             Return the configuration of a device.
             Parameters:
                 retrieve (string) – Which configuration type you want to populate, default is all of
                 them.
                 The rest will be set to “”.
@@ -1123,15 +1125,15 @@
                 If the device doesn't differentiate between running and startup configuration this
                 will an empty string
             Return type:
             The object returned is a dictionary with a key for each configuration store
         """
         try:
             configuration = {"running": "", "candidate": "", "startup": ""}
-            if self.sros_get_format == "cli" and (sanitized is True or sanitized is False):
+            if self.sros_get_format == "cli" or format == "cli":
                 # Getting output in MD-CLI format
                 # retrieving config using md-cli
                 cmd_running = "admin show configuration | no-more"
                 cmd_candidate = ["edit-config read-only", "info | no-more", "quit-config"]
 
                 # helper method
                 def _update_buff(buff):
@@ -1185,15 +1187,15 @@
                     buff_candidate = self._perform_cli_commands(cmd_candidate, True)
                     configuration["running"] = _update_buff(buff_running)
                     configuration["startup"] = _update_buff(buff_running)
                     configuration["candidate"] = _update_buff(buff_candidate)
                     return configuration
 
             # returning the config in xml format
-            elif self.sros_get_format == "xml" and (sanitized is True or sanitized is False):
+            elif self.sros_get_format == "xml" or format == "xml":
                 config_data_running_xml = ""
                 if retrieve == "running" or retrieve == "all":
                     config_data_running = to_ele(
                         self.conn.get_config(source="running").data_xml
                     )
                     config_data_running_xml = to_xml(
                         config_data_running.xpath(
```

### Comparing `napalm-sros-1.0.1/napalm_sros/utils/parse_output_to_dict.py` & `napalm_sros-1.0.2/napalm_sros/utils/parse_output_to_dict.py`

 * *Files identical despite different names*

### Comparing `napalm-sros-1.0.1/napalm_sros.egg-info/PKG-INFO` & `napalm_sros-1.0.2/napalm_sros.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: napalm-sros
-Version: 1.0.1
+Version: 1.0.2
 Summary: Network Automation and Programmability Abstraction Layer driver for Nokia SR OS
 Home-page: https://github.com/napalm-automation/napalm-sros
 Author: Nokia
 Author-email: Ashna Shah <ashna.shah@nokia.com>, Roman Dodin <roman.dodin@nokia.com>, Patryk Szulczewski <patryk.szulczewski@nokia.com>, Jeroen van Bemmel <jeroen.van_bemmel@nokia.com>
 Project-URL: Homepage, https://github.com/napalm-automation-community/napalm-sros
 Project-URL: Bug Tracker, https://github.com/napalm-automation-community/napalm-sros/issues
 Classifier: Topic :: System :: Networking
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Natural Language :: English
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: napalm>=4.0.0
 Requires-Dist: pytest>=7.0.1
 Requires-Dist: setuptools>=47.3.1
 Requires-Dist: pip>=21.3.1
 Requires-Dist: textfsm
 Requires-Dist: paramiko>=2.11.0
 Requires-Dist: lxml>=4.9.1
-Requires-Dist: ncclient>=0.6.13
+Requires-Dist: ncclient>=0.6.15
 Requires-Dist: xmltodict>=0.12.0
 Requires-Dist: dictdiffer>=0.9.0
 Requires-Dist: datetime>=4.7
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: ruff; extra == "tests"
 
@@ -50,17 +50,17 @@
 2) The main files included for Nokia SR OS driver are:
      3) napalm_sros/sros.py: Overridden NAPALM methods to get the expected output from SR OS
      4) napalm_sros/nc_filters.py: Filters defined to get data from SR OS using a NETCONF connection
 5) Mapping of various parameters of NAPALM output to Nokia SR OS can be found in this [Mapping Document](https://github.com/napalm-automation-community/napalm-sros/blob/master/Summary_of_Methods.pdf)
 6) For testing, please refer to [Test Document](https://github.com/napalm-automation-community/napalm-sros/blob/master/README_TEST.md)
 
 #### **Components Version**
-1) Python - 3.6
+1) Python - 3.8 or higher
 2) ncclient >= 0.6.13
 3) paramiko >= 2.11.0
-4) NAPALM >= 3.4.1
+4) NAPALM >= 4.0.0
 
 ##### **Note**
-This version of the driver leverages Nokia’s defined YANG models for configuration and state trees for the SROS platform. While SROS also support limited configuration and state retrieval using openconfig standard models, the NAPALM driver does not support configuration or state retrieval of openconfig data models.
+This version of the driver leverages Nokia’s defined YANG models for configuration and state trees for the SROS platform. While SROS also supports limited configuration and state retrieval using openconfig standard models, the NAPALM driver does not support configuration or state retrieval of openconfig data models.
 
 #### License
 This project is licensed under the Apache-2.0 license - see the [LICENSE](LICENSE) file.
```

### Comparing `napalm-sros-1.0.1/napalm_sros.egg-info/SOURCES.txt` & `napalm_sros-1.0.2/napalm_sros.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,10 +18,9 @@
 napalm_sros/api/get_bgp_neighbors.py
 napalm_sros/api/get_bgp_neighbors_detail.py
 napalm_sros/api/util.py
 napalm_sros/templates/__init__.py
 napalm_sros/templates/set_hostname.j2
 napalm_sros/utils/__init__.py
 napalm_sros/utils/parse_output_to_dict.py
-napalm_sros/utils/utils.py
 napalm_sros/utils/textfsm_templates/__init__.py
 napalm_sros/utils/textfsm_templates/nokia_sros_show_service_fdb_mac.tpl
```

### Comparing `napalm-sros-1.0.1/pyproject.toml` & `napalm_sros-1.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools>=56.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "napalm-sros"
-version="1.0.1"
+version="1.0.2"
 description="Network Automation and Programmability Abstraction Layer driver for Nokia SR OS"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dynamic = [ "dependencies" ]
 classifiers = [
     "Topic :: System :: Networking",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Natural Language :: English",
 ]
 
 authors = [
   { name="Ashna Shah", email="ashna.shah@nokia.com" },
   { name="Roman Dodin", email="roman.dodin@nokia.com" },
   { name="Patryk Szulczewski", email="patryk.szulczewski@nokia.com" },
```

### Comparing `napalm-sros-1.0.1/setup.py` & `napalm_sros-1.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,28 +4,28 @@
     reqs = [r for r in fs.read().splitlines() if (len(r) > 0 and not r.startswith("#"))]
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="napalm-sros",
-    version="1.0.1",
+    version="1.0.2",
     packages=find_packages(),
     package_data={"napalm_sros.templates": ["*.js"], "napalm_sros.utils.textfsm_templates": ["*.tpl"]},
     author="Nokia",
     author_email="",
     description="Network Automation and Programmability Abstraction Layer with Multivendor support",
     classifiers=[
         "Topic :: Utilities",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Natural Language :: English",
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: Apache Software License",
     ],
     url="https://github.com/napalm-automation/napalm-sros",
     include_package_data=True,
     install_requires=reqs,
```

