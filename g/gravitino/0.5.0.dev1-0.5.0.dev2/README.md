# Comparing `tmp/gravitino-0.5.0.dev1.tar.gz` & `tmp/gravitino-0.5.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitino-0.5.0.dev1.tar", last modified: Fri May  3 12:38:07 2024, max compression
+gzip compressed data, was "gravitino-0.5.0.dev2.tar", last modified: Sat May  4 01:20:16 2024, max compression
```

## Comparing `gravitino-0.5.0.dev1.tar` & `gravitino-0.5.0.dev2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-03 12:38:07.696108 gravitino-0.5.0.dev1/
--rw-r--r--   0 xun        (501) staff       (20)     3714 2024-05-03 12:38:07.695973 gravitino-0.5.0.dev1/PKG-INFO
--rw-r--r--   0 xun        (501) staff       (20)     3424 2024-05-03 12:21:44.000000 gravitino-0.5.0.dev1/README.md
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-03 12:38:07.695020 gravitino-0.5.0.dev1/gravitino/
--rw-r--r--   0 xun        (501) staff       (20)      244 2024-04-08 10:35:22.000000 gravitino-0.5.0.dev1/gravitino/__init__.py
--rw-r--r--   0 xun        (501) staff       (20)      119 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev1/gravitino/constants.py
--rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev1/gravitino/exceptions.py
--rw-r--r--   0 xun        (501) staff       (20)     4404 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev1/gravitino/gravitino_client.py
--rw-r--r--   0 xun        (501) staff       (20)     9035 2024-05-01 10:39:47.000000 gravitino-0.5.0.dev1/gravitino/name_identifier.py
--rw-r--r--   0 xun        (501) staff       (20)     7608 2024-05-01 10:39:47.000000 gravitino-0.5.0.dev1/gravitino/namespace.py
--rw-r--r--   0 xun        (501) staff       (20)     2430 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev1/gravitino/service.py
--rw-r--r--   0 xun        (501) staff       (20)      318 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev1/gravitino/typing.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-03 12:38:07.695605 gravitino-0.5.0.dev1/gravitino.egg-info/
--rw-r--r--   0 xun        (501) staff       (20)     3714 2024-05-03 12:38:07.000000 gravitino-0.5.0.dev1/gravitino.egg-info/PKG-INFO
--rw-r--r--   0 xun        (501) staff       (20)      405 2024-05-03 12:38:07.000000 gravitino-0.5.0.dev1/gravitino.egg-info/SOURCES.txt
--rw-r--r--   0 xun        (501) staff       (20)        1 2024-05-03 12:38:07.000000 gravitino-0.5.0.dev1/gravitino.egg-info/dependency_links.txt
--rw-r--r--   0 xun        (501) staff       (20)       62 2024-05-03 12:38:07.000000 gravitino-0.5.0.dev1/gravitino.egg-info/requires.txt
--rw-r--r--   0 xun        (501) staff       (20)       10 2024-05-03 12:38:07.000000 gravitino-0.5.0.dev1/gravitino.egg-info/top_level.txt
--rw-r--r--   0 xun        (501) staff       (20)       38 2024-05-03 12:38:07.696157 gravitino-0.5.0.dev1/setup.cfg
--rw-r--r--   0 xun        (501) staff       (20)      654 2024-05-03 12:26:51.000000 gravitino-0.5.0.dev1/setup.py
-drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-03 12:38:07.695759 gravitino-0.5.0.dev1/tests/
--rw-r--r--   0 xun        (501) staff       (20)     2175 2024-04-13 14:55:38.000000 gravitino-0.5.0.dev1/tests/test_gravitino_client.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 01:20:16.578039 gravitino-0.5.0.dev2/
+-rw-r--r--   0 xun        (501) staff       (20)     3714 2024-05-04 01:20:16.577917 gravitino-0.5.0.dev2/PKG-INFO
+-rw-r--r--   0 xun        (501) staff       (20)     3424 2024-05-03 12:21:44.000000 gravitino-0.5.0.dev2/README.md
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 01:20:16.576876 gravitino-0.5.0.dev2/gravitino/
+-rw-r--r--   0 xun        (501) staff       (20)      244 2024-04-08 10:35:22.000000 gravitino-0.5.0.dev2/gravitino/__init__.py
+-rw-r--r--   0 xun        (501) staff       (20)      119 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev2/gravitino/constants.py
+-rw-r--r--   0 xun        (501) staff       (20)      105 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev2/gravitino/exceptions.py
+-rw-r--r--   0 xun        (501) staff       (20)     4404 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev2/gravitino/gravitino_client.py
+-rw-r--r--   0 xun        (501) staff       (20)     9035 2024-05-01 10:39:47.000000 gravitino-0.5.0.dev2/gravitino/name_identifier.py
+-rw-r--r--   0 xun        (501) staff       (20)     7608 2024-05-01 10:39:47.000000 gravitino-0.5.0.dev2/gravitino/namespace.py
+-rw-r--r--   0 xun        (501) staff       (20)     2430 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev2/gravitino/service.py
+-rw-r--r--   0 xun        (501) staff       (20)      318 2024-04-02 06:05:04.000000 gravitino-0.5.0.dev2/gravitino/typing.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 01:20:16.577484 gravitino-0.5.0.dev2/gravitino.egg-info/
+-rw-r--r--   0 xun        (501) staff       (20)     3714 2024-05-04 01:20:16.000000 gravitino-0.5.0.dev2/gravitino.egg-info/PKG-INFO
+-rw-r--r--   0 xun        (501) staff       (20)      405 2024-05-04 01:20:16.000000 gravitino-0.5.0.dev2/gravitino.egg-info/SOURCES.txt
+-rw-r--r--   0 xun        (501) staff       (20)        1 2024-05-04 01:20:16.000000 gravitino-0.5.0.dev2/gravitino.egg-info/dependency_links.txt
+-rw-r--r--   0 xun        (501) staff       (20)       62 2024-05-04 01:20:16.000000 gravitino-0.5.0.dev2/gravitino.egg-info/requires.txt
+-rw-r--r--   0 xun        (501) staff       (20)       10 2024-05-04 01:20:16.000000 gravitino-0.5.0.dev2/gravitino.egg-info/top_level.txt
+-rw-r--r--   0 xun        (501) staff       (20)       38 2024-05-04 01:20:16.578091 gravitino-0.5.0.dev2/setup.cfg
+-rw-r--r--   0 xun        (501) staff       (20)      722 2024-05-04 01:20:02.000000 gravitino-0.5.0.dev2/setup.py
+drwxr-xr-x   0 xun        (501) staff       (20)        0 2024-05-04 01:20:16.577623 gravitino-0.5.0.dev2/tests/
+-rw-r--r--   0 xun        (501) staff       (20)     2175 2024-04-13 14:55:38.000000 gravitino-0.5.0.dev2/tests/test_gravitino_client.py
```

### Comparing `gravitino-0.5.0.dev1/PKG-INFO` & `gravitino-0.5.0.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gravitino
-Version: 0.5.0.dev1
+Version: 0.5.0.dev2
 Summary: Python lib/client for Gravitino
 Home-page: https://github.com/datastrato/gravitino
 Author: datastrato
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `gravitino-0.5.0.dev1/README.md` & `gravitino-0.5.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev1/gravitino/gravitino_client.py` & `gravitino-0.5.0.dev2/gravitino/gravitino_client.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev1/gravitino/name_identifier.py` & `gravitino-0.5.0.dev2/gravitino/name_identifier.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev1/gravitino/namespace.py` & `gravitino-0.5.0.dev2/gravitino/namespace.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev1/gravitino/service.py` & `gravitino-0.5.0.dev2/gravitino/service.py`

 * *Files identical despite different names*

### Comparing `gravitino-0.5.0.dev1/gravitino.egg-info/PKG-INFO` & `gravitino-0.5.0.dev2/gravitino.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gravitino
-Version: 0.5.0.dev1
+Version: 0.5.0.dev2
 Summary: Python lib/client for Gravitino
 Home-page: https://github.com/datastrato/gravitino
 Author: datastrato
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `gravitino-0.5.0.dev1/setup.py` & `gravitino-0.5.0.dev2/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 
 from setuptools import find_packages, setup
 
 
 setup(
     name="gravitino",
     description="Python lib/client for Gravitino",
-    version="0.5.0.dev1",
+    version="0.5.0.dev2",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/datastrato/gravitino",
     author="datastrato",
     python_requires=">=3.8",
     packages=find_packages(include=["gravitino", ".*"]),
+    include_package_data=True,
+    package_data={"": ["assets/*"]},
     install_requires=open("requirements.txt").read(),
     extras_require={
         "dev": open("requirements-dev.txt").read(),
     },
 )
```

### Comparing `gravitino-0.5.0.dev1/tests/test_gravitino_client.py` & `gravitino-0.5.0.dev2/tests/test_gravitino_client.py`

 * *Files identical despite different names*

