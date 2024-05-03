# Comparing `tmp/haondt_charon-1.0.3.tar.gz` & `tmp/haondt_charon-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haondt_charon-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "haondt_charon-1.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `haondt_charon-1.0.3.tar` & `haondt_charon-1.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       39 2024-04-28 02:50:20.846986 haondt_charon-1.0.3/.gitignore
--rw-r--r--   0        0        0      169 2024-04-27 13:55:39.003551 haondt_charon-1.0.3/.gitlab-ci.yml
--rw-r--r--   0        0        0      196 2024-04-28 03:00:11.413730 haondt_charon-1.0.3/Dockerfile
--rw-r--r--   0        0        0     1081 2024-04-28 02:50:20.850987 haondt_charon-1.0.3/LICENSE
--rw-r--r--   0        0        0     5697 2024-04-29 01:14:55.084319 haondt_charon-1.0.3/README.md
--rw-r--r--   0        0        0     1054 2024-04-27 13:55:39.003551 haondt_charon-1.0.3/charon.yml
--rw-r--r--   0        0        0        0 2024-04-29 01:15:15.784595 haondt_charon-1.0.3/charon/__init__.py
--rw-r--r--   0        0        0     1395 2024-04-28 02:50:20.850987 haondt_charon-1.0.3/charon/__main__.py
--rw-r--r--   0        0        0       45 2024-04-28 02:50:20.850987 haondt_charon-1.0.3/charon/destinations/__init__.py
--rw-r--r--   0        0        0     1794 2024-04-28 02:50:20.850987 haondt_charon-1.0.3/charon/destinations/gcp_bucket.py
--rw-r--r--   0        0        0     1164 2024-04-28 02:50:20.850987 haondt_charon-1.0.3/charon/destinations/local.py
--rw-r--r--   0        0        0       50 2024-04-28 02:50:20.850987 haondt_charon-1.0.3/charon/requirements.txt
--rw-r--r--   0        0        0     2532 2024-04-28 02:50:20.850987 haondt_charon-1.0.3/charon/scheduling.py
--rw-r--r--   0        0        0     2369 2024-04-28 02:50:20.850987 haondt_charon-1.0.3/charon/shared.py
--rw-r--r--   0        0        0      107 2024-04-28 02:50:20.850987 haondt_charon-1.0.3/charon/sources/__init__.py
--rw-r--r--   0        0        0     2145 2024-04-28 02:50:20.850987 haondt_charon-1.0.3/charon/sources/http.py
--rw-r--r--   0        0        0     2010 2024-04-28 02:50:20.850987 haondt_charon-1.0.3/charon/sources/lib.py
--rw-r--r--   0        0        0     1350 2024-04-28 02:50:20.850987 haondt_charon-1.0.3/charon/sources/local.py
--rw-r--r--   0        0        0     1312 2024-04-28 02:50:20.850987 haondt_charon-1.0.3/charon/styx.py
--rw-r--r--   0        0        0      314 2024-04-27 14:17:35.041418 haondt_charon-1.0.3/docker-compose.yml
--rw-r--r--   0        0        0      465 2024-04-28 13:17:35.863272 haondt_charon-1.0.3/pipeline.yml
--rw-r--r--   0        0        0      742 2024-04-29 01:15:16.188600 haondt_charon-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      493 2024-04-28 02:50:20.850987 haondt_charon-1.0.3/tests/charon.test.yml
--rwxr-xr-x   0        0        0      561 2024-04-28 02:50:20.854987 haondt_charon-1.0.3/tests/test.sh
--rwxr-xr-x   0        0        0      787 2024-04-28 02:50:20.854987 haondt_charon-1.0.3/tests/test2.sh
--rw-r--r--   0        0        0     6242 1970-01-01 00:00:00.000000 haondt_charon-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/.gitignore
+-rw-r--r--   0        0        0      169 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/.gitlab-ci.yml
+-rw-r--r--   0        0        0      206 2024-05-03 22:30:54.865617 haondt_charon-1.0.4/Dockerfile
+-rw-r--r--   0        0        0     1081 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/LICENSE
+-rw-r--r--   0        0        0     5755 2024-05-03 22:30:54.865617 haondt_charon-1.0.4/README.md
+-rw-r--r--   0        0        0     1054 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/charon.yml
+-rw-r--r--   0        0        0        0 2024-05-03 22:30:54.933617 haondt_charon-1.0.4/charon/__init__.py
+-rw-r--r--   0        0        0     1395 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/charon/__main__.py
+-rw-r--r--   0        0        0       45 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/charon/destinations/__init__.py
+-rw-r--r--   0        0        0     1794 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/charon/destinations/gcp_bucket.py
+-rw-r--r--   0        0        0     1164 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/charon/destinations/local.py
+-rw-r--r--   0        0        0       50 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/charon/requirements.txt
+-rw-r--r--   0        0        0     2532 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/charon/scheduling.py
+-rw-r--r--   0        0        0     2369 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/charon/shared.py
+-rw-r--r--   0        0        0      107 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/charon/sources/__init__.py
+-rw-r--r--   0        0        0     2145 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/charon/sources/http.py
+-rw-r--r--   0        0        0     2010 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/charon/sources/lib.py
+-rw-r--r--   0        0        0     1350 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/charon/sources/local.py
+-rw-r--r--   0        0        0     1312 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/charon/styx.py
+-rw-r--r--   0        0        0      314 2024-04-29 01:45:23.302231 haondt_charon-1.0.4/docker-compose.yml
+-rw-r--r--   0        0        0      468 2024-05-03 22:30:54.865617 haondt_charon-1.0.4/pipeline.yml
+-rw-r--r--   0        0        0      742 2024-05-03 22:30:55.501625 haondt_charon-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      493 2024-04-29 01:45:23.306231 haondt_charon-1.0.4/tests/charon.test.yml
+-rwxr-xr-x   0        0        0      561 2024-04-29 01:45:23.306231 haondt_charon-1.0.4/tests/test.sh
+-rwxr-xr-x   0        0        0      787 2024-04-29 01:45:23.310231 haondt_charon-1.0.4/tests/test2.sh
+-rw-r--r--   0        0        0     6300 1970-01-01 00:00:00.000000 haondt_charon-1.0.4/PKG-INFO
```

### Comparing `haondt_charon-1.0.3/LICENSE` & `haondt_charon-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.3/README.md` & `haondt_charon-1.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 - [tests](#tests)
 
 # installation
 
 charon can be installed as a docker image
 
 ```bash
+# from docker hub
+docker pull haumea/charon
+# from gitlab
 docker pull registry.gitlab.com/haondt/cicd/registry/charon:latest
 ```
 
 see `docker-compose.yml` for a sample docker compose setup.
 
 charon can also be installed as a python package
```

### Comparing `haondt_charon-1.0.3/charon.yml` & `haondt_charon-1.0.4/charon.yml`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.3/charon/__main__.py` & `haondt_charon-1.0.4/charon/__main__.py`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.3/charon/destinations/gcp_bucket.py` & `haondt_charon-1.0.4/charon/destinations/gcp_bucket.py`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.3/charon/destinations/local.py` & `haondt_charon-1.0.4/charon/destinations/local.py`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.3/charon/scheduling.py` & `haondt_charon-1.0.4/charon/scheduling.py`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.3/charon/shared.py` & `haondt_charon-1.0.4/charon/shared.py`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.3/charon/sources/http.py` & `haondt_charon-1.0.4/charon/sources/http.py`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.3/charon/sources/lib.py` & `haondt_charon-1.0.4/charon/sources/lib.py`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.3/charon/sources/local.py` & `haondt_charon-1.0.4/charon/sources/local.py`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.3/charon/styx.py` & `haondt_charon-1.0.4/charon/styx.py`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.3/pyproject.toml` & `haondt_charon-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [ "flit_core >=3.2,<4",]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "haondt_charon"
 classifiers = [ "License :: OSI Approved :: MIT License",]
 description = "charon is a utility for backing up data from one location to another at regular intervals."
-version = "1.0.3"
+version = "1.0.4"
 readme = "README.md"
 keywords = [ "backup", "recovery",]
 dependencies = [ "croniter>=2.0.5", "PyYAML>=6.0.1", "cryptography>=42.0.5", "google-cloud-storage>=2.16.0",]
 [[project.authors]]
 name = "haondt"
 
 [project.license]
```

### Comparing `haondt_charon-1.0.3/tests/test.sh` & `haondt_charon-1.0.4/tests/test.sh`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.3/tests/test2.sh` & `haondt_charon-1.0.4/tests/test2.sh`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.3/PKG-INFO` & `haondt_charon-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haondt_charon
-Version: 1.0.3
+Version: 1.0.4
 Summary: charon is a utility for backing up data from one location to another at regular intervals.
 Keywords: backup,recovery
 Author: haondt
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: croniter>=2.0.5
 Requires-Dist: PyYAML>=6.0.1
@@ -29,14 +29,17 @@
 - [tests](#tests)
 
 # installation
 
 charon can be installed as a docker image
 
 ```bash
+# from docker hub
+docker pull haumea/charon
+# from gitlab
 docker pull registry.gitlab.com/haondt/cicd/registry/charon:latest
 ```
 
 see `docker-compose.yml` for a sample docker compose setup.
 
 charon can also be installed as a python package
```

