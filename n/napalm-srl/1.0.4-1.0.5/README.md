# Comparing `tmp/napalm-srl-1.0.4.tar.gz` & `tmp/napalm_srl-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napalm-srl-1.0.4.tar", last modified: Fri Dec 15 15:54:34 2023, max compression
+gzip compressed data, was "napalm_srl-1.0.5.tar", last modified: Sat May  4 04:42:24 2024, max compression
```

## Comparing `napalm-srl-1.0.4.tar` & `napalm_srl-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 jeroen    (1000) jeroen    (1000)        0 2023-12-15 15:54:34.847934 napalm-srl-1.0.4/
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      304 2023-05-26 15:22:56.000000 napalm-srl-1.0.4/AUTHORS
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)    11357 2023-05-18 14:35:14.000000 napalm-srl-1.0.4/LICENSE
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)       54 2023-05-26 15:22:56.000000 napalm-srl-1.0.4/MANIFEST.in
--rw-r--r--   0 jeroen    (1000) jeroen    (1000)     4531 2023-12-15 15:54:34.847934 napalm-srl-1.0.4/PKG-INFO
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)     3165 2023-09-19 14:03:03.000000 napalm-srl-1.0.4/README.md
-drwxrwxr-x   0 jeroen    (1000) jeroen    (1000)        0 2023-12-15 15:54:34.847934 napalm-srl-1.0.4/napalm_srl/
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      732 2023-05-18 14:35:14.000000 napalm-srl-1.0.4/napalm_srl/__init__.py
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)    81400 2023-05-18 14:35:14.000000 napalm-srl-1.0.4/napalm_srl/gnmi_pb2.py
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)     9806 2023-05-18 14:35:14.000000 napalm-srl-1.0.4/napalm_srl/jsondiff.py
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)   138089 2023-12-15 15:49:30.000000 napalm-srl-1.0.4/napalm_srl/srl.py
-drwxrwxr-x   0 jeroen    (1000) jeroen    (1000)        0 2023-12-15 15:54:34.847934 napalm-srl-1.0.4/napalm_srl.egg-info/
--rw-r--r--   0 jeroen    (1000) jeroen    (1000)     4531 2023-12-15 15:54:34.000000 napalm-srl-1.0.4/napalm_srl.egg-info/PKG-INFO
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      365 2023-12-15 15:54:34.000000 napalm-srl-1.0.4/napalm_srl.egg-info/SOURCES.txt
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)        1 2023-12-15 15:54:34.000000 napalm-srl-1.0.4/napalm_srl.egg-info/dependency_links.txt
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      141 2023-12-15 15:54:34.000000 napalm-srl-1.0.4/napalm_srl.egg-info/requires.txt
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)       11 2023-12-15 15:54:34.000000 napalm-srl-1.0.4/napalm_srl.egg-info/top_level.txt
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)     1067 2023-12-15 15:51:12.000000 napalm-srl-1.0.4/pyproject.toml
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      125 2023-05-18 14:35:14.000000 napalm-srl-1.0.4/requirements-dev.txt
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      244 2023-09-15 03:14:44.000000 napalm-srl-1.0.4/requirements.txt
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      493 2023-12-15 15:54:34.847934 napalm-srl-1.0.4/setup.cfg
--rw-rw-r--   0 jeroen    (1000) jeroen    (1000)     1229 2023-12-15 15:51:26.000000 napalm-srl-1.0.4/setup.py
+drwxrwxr-x   0 jeroen    (1000) jeroen    (1000)        0 2024-05-04 04:42:24.007902 napalm_srl-1.0.5/
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      304 2023-05-26 15:22:56.000000 napalm_srl-1.0.5/AUTHORS
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)    11357 2023-05-18 14:35:14.000000 napalm_srl-1.0.5/LICENSE
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)       54 2023-05-26 15:22:56.000000 napalm_srl-1.0.5/MANIFEST.in
+-rw-r--r--   0 jeroen    (1000) jeroen    (1000)     4532 2024-05-04 04:42:24.007902 napalm_srl-1.0.5/PKG-INFO
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)     3165 2023-09-19 14:03:03.000000 napalm_srl-1.0.5/README.md
+drwxrwxr-x   0 jeroen    (1000) jeroen    (1000)        0 2024-05-04 04:42:24.003902 napalm_srl-1.0.5/napalm_srl/
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      732 2023-05-18 14:35:14.000000 napalm_srl-1.0.5/napalm_srl/__init__.py
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)    81400 2023-05-18 14:35:14.000000 napalm_srl-1.0.5/napalm_srl/gnmi_pb2.py
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)     9806 2023-05-18 14:35:14.000000 napalm_srl-1.0.5/napalm_srl/jsondiff.py
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)   138261 2024-05-04 04:23:55.000000 napalm_srl-1.0.5/napalm_srl/srl.py
+drwxrwxr-x   0 jeroen    (1000) jeroen    (1000)        0 2024-05-04 04:42:24.007902 napalm_srl-1.0.5/napalm_srl.egg-info/
+-rw-r--r--   0 jeroen    (1000) jeroen    (1000)     4532 2024-05-04 04:42:23.000000 napalm_srl-1.0.5/napalm_srl.egg-info/PKG-INFO
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      365 2024-05-04 04:42:23.000000 napalm_srl-1.0.5/napalm_srl.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)        1 2024-05-04 04:42:23.000000 napalm_srl-1.0.5/napalm_srl.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      141 2024-05-04 04:42:23.000000 napalm_srl-1.0.5/napalm_srl.egg-info/requires.txt
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)       11 2024-05-04 04:42:23.000000 napalm_srl-1.0.5/napalm_srl.egg-info/top_level.txt
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)     1068 2024-05-04 04:25:33.000000 napalm_srl-1.0.5/pyproject.toml
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      125 2023-05-18 14:35:14.000000 napalm_srl-1.0.5/requirements-dev.txt
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      244 2023-09-15 03:14:44.000000 napalm_srl-1.0.5/requirements.txt
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)      493 2024-05-04 04:42:24.007902 napalm_srl-1.0.5/setup.cfg
+-rw-rw-r--   0 jeroen    (1000) jeroen    (1000)     1230 2024-05-04 04:25:15.000000 napalm_srl-1.0.5/setup.py
```

### Comparing `napalm-srl-1.0.4/LICENSE` & `napalm_srl-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `napalm-srl-1.0.4/PKG-INFO` & `napalm_srl-1.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: napalm-srl
-Version: 1.0.4
+Version: 1.0.5
 Summary: Network Automation and Programmability Abstraction Layer driver for Nokia SR Linux
 Home-page: https://github.com/napalm-automation-community/napalm-srlinux
 Author: Jose Valente
 Author-email: Jose Valente <jose.valente@nokia.com>, Jeroen van Bemmel <jeroen.van_bemmel@nokia.com>
 Project-URL: Homepage, https://github.com/napalm-automation-community/napalm-srlinux
 Project-URL: Bug Tracker, https://github.com/napalm-automation-community/napalm-srlinux/issues
 Classifier: Topic :: System :: Networking
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Natural Language :: English
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: napalm>=2.0.0
 Requires-Dist: pip>=20.1.1
 Requires-Dist: pytest>=5.4.3
 Requires-Dist: setuptools>=47.3.1
```

### Comparing `napalm-srl-1.0.4/README.md` & `napalm_srl-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `napalm-srl-1.0.4/napalm_srl/__init__.py` & `napalm_srl-1.0.5/napalm_srl/__init__.py`

 * *Files identical despite different names*

### Comparing `napalm-srl-1.0.4/napalm_srl/gnmi_pb2.py` & `napalm_srl-1.0.5/napalm_srl/gnmi_pb2.py`

 * *Files identical despite different names*

### Comparing `napalm-srl-1.0.4/napalm_srl/jsondiff.py` & `napalm_srl-1.0.5/napalm_srl/jsondiff.py`

 * *Files identical despite different names*

### Comparing `napalm-srl-1.0.4/napalm_srl/srl.py` & `napalm_srl-1.0.5/napalm_srl/srl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1671,15 +1671,21 @@
     #         return {
     #             "running": "",
     #             "candidate": "",
     #             "startup": ""
     #         }
 
 
-    def get_config(self, retrieve='all', full=False, sanitized=False):
+    def get_config(
+        self,
+        retrieve: str = "all",
+        full: bool = False,
+        sanitized: bool = False,
+        format: str = "text",    # This driver supports 'cli' for CLI, else default 'json'
+    ):
         """
         :param retrieve: Which configuration type you want to populate, default is all of them. The rest will be set to “”.
         :param full:Retrieve all the configuration. For instance, on ios, “sh run all”.
         :param sanitized:Remove secret data. Default: False.
         :return:Return the configuration of a device.
         """
         try:
@@ -1687,15 +1693,15 @@
                 # Only 'running' or 'all' is supported for get_config
                 return {
                     "running": "",
                     "candidate": "",
                     "startup": ""
                 }
 
-            if self.running_format == 'cli':
+            if self.running_format == 'cli' or format == 'cli':
                 if sanitized:
                     raise NotImplementedError(
                         "sanitized=True is not implemented with CLI format")
                 output = self.device._jsonrpcRunCli(["info flat"])
                 running_config = self._return_result(output)
             else:
                 running = self.device._gnmiGet("", {"/"}, "CONFIG")
```

### Comparing `napalm-srl-1.0.4/napalm_srl.egg-info/PKG-INFO` & `napalm_srl-1.0.5/napalm_srl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: napalm-srl
-Version: 1.0.4
+Version: 1.0.5
 Summary: Network Automation and Programmability Abstraction Layer driver for Nokia SR Linux
 Home-page: https://github.com/napalm-automation-community/napalm-srlinux
 Author: Jose Valente
 Author-email: Jose Valente <jose.valente@nokia.com>, Jeroen van Bemmel <jeroen.van_bemmel@nokia.com>
 Project-URL: Homepage, https://github.com/napalm-automation-community/napalm-srlinux
 Project-URL: Bug Tracker, https://github.com/napalm-automation-community/napalm-srlinux/issues
 Classifier: Topic :: System :: Networking
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Natural Language :: English
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: napalm>=2.0.0
 Requires-Dist: pip>=20.1.1
 Requires-Dist: pytest>=5.4.3
 Requires-Dist: setuptools>=47.3.1
```

### Comparing `napalm-srl-1.0.4/pyproject.toml` & `napalm_srl-1.0.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools>=56.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "napalm-srl"
-version="1.0.4"
+version="1.0.5"
 description="Network Automation and Programmability Abstraction Layer driver for Nokia SR Linux"
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
   { name="Jose Valente", email="jose.valente@nokia.com" },
   { name="Jeroen van Bemmel", email="jeroen.van_bemmel@nokia.com" },
 ]
```

### Comparing `napalm-srl-1.0.4/setup.py` & `napalm_srl-1.0.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 from setuptools import setup, find_packages
 with open("requirements.txt", "r") as file:
     reqs = [req for req in file.read().splitlines() if (len(req) > 0 and not req.startswith("#"))]
 __author__ = 'Jose Valente <jose.valente@nokia.com>'
 
 setup(
     name="napalm-srl",
-    version="1.0.4",
+    version="1.0.5",
     packages=find_packages(),
     author="Jose Valente",
     author_email="jose.valente@nokia.com",
     description="Network Automation and Programmability Abstraction Layer with Multivendor support",
     classifiers=[
         'Topic :: Utilities',
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Natural Language :: English",
         'Operating System :: POSIX :: Linux',
         'Operating System :: MacOS',
     ],
     url="https://github.com/napalm-automation-community/napalm-srlinux",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     include_package_data=True,
     install_requires=reqs,
 )
```

