# Comparing `tmp/proboscis_async_events-0.1.2.tar.gz` & `tmp/proboscis_async_events-0.1.3.tar.gz`

## Comparing `proboscis_async_events-0.1.2.tar` & `proboscis_async_events-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,19 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.2/.python-version
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.2/requirements-dev.lock
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.2/requirements.lock
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.2/.idea/.gitignore
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.2/.idea/misc.xml
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.2/.idea/workspace.xml
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.2/src/proboscis_async_events/__init__.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.2/src/proboscis_async_events/messaging.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.2/.gitignore
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.2/README.md
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/.python-version
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/requirements-dev.lock
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/requirements.lock
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/.idea/.gitignore
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/.idea/misc.xml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/.idea/modules.xml
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/.idea/proboscis-async-events.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/.idea/vcs.xml
+-rw-r--r--   0        0        0     3921 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/.idea/workspace.xml
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/.idea/codeStyles/Project.xml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/src/proboscis_async_events/__init__.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/src/proboscis_async_events/messaging.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/test/test_messaging.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/.gitignore
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/README.md
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.3/PKG-INFO
```

### Comparing `proboscis_async_events-0.1.2/pyproject.toml` & `proboscis_async_events-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [project]
 name = "proboscis-async-events"
-version = "0.1.2"
+version = "0.1.3"
 description = "Add your description here"
 authors = [
     { name = "proboscis", email = "nameissoap@gmail.com" }
 ]
 dependencies = [
     "pampy>=0.3.0",
+    "pytest>=8.2.0",
 ]
 readme = "README.md"
 requires-python = ">= 3.10"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
```

