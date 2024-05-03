# Comparing `tmp/heaserver-buckets-1.1.1.tar.gz` & `tmp/heaserver_buckets-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-buckets-1.1.1.tar", last modified: Tue Apr  9 21:34:32 2024, max compression
+gzip compressed data, was "heaserver_buckets-1.1.2.tar", last modified: Fri May  3 23:38:21 2024, max compression
```

## Comparing `heaserver-buckets-1.1.1.tar` & `heaserver_buckets-1.1.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 21:34:32.827100 heaserver-buckets-1.1.1/
--rw-rw-rw-   0        0        0      261 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.1/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.1/.gitignore
--rw-rw-rw-   0        0        0     1515 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.1/Dockerfile
--rw-rw-rw-   0        0        0    11625 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.1/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5107 2024-04-09 21:34:32.826100 heaserver-buckets-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3766 2024-04-09 21:29:16.000000 heaserver-buckets-1.1.1/README.md
--rw-rw-rw-   0        0        0     1737 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.1/RELEASING.md
--rw-rw-rw-   0        0        0      470 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.1/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-04-09 21:34:32.719101 heaserver-buckets-1.1.1/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-04-09 21:34:32.720101 heaserver-buckets-1.1.1/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-09 21:34:32.778099 heaserver-buckets-1.1.1/integrationtests/heaserver/bucketintegrationtest/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.1/integrationtests/heaserver/bucketintegrationtest/__init__.py
--rw-rw-rw-   0        0        0     4817 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.1/integrationtests/heaserver/bucketintegrationtest/test_all.py
--rw-rw-rw-   0        0        0    10927 2024-04-09 19:49:54.000000 heaserver-buckets-1.1.1/integrationtests/heaserver/bucketintegrationtest/testcase.py
--rw-rw-rw-   0        0        0      111 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.1/pytest.ini
--rw-rw-rw-   0        0        0      262 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.1/requirements_dev.txt
--rw-rw-rw-   0        0        0     5310 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.1/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-04-09 21:34:32.827100 heaserver-buckets-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1838 2024-04-09 21:33:58.000000 heaserver-buckets-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 21:34:32.722099 heaserver-buckets-1.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-09 21:34:32.721130 heaserver-buckets-1.1.1/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-09 21:34:32.791099 heaserver-buckets-1.1.1/src/heaserver/bucket/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.1/src/heaserver/bucket/__init__.py
--rw-rw-rw-   0        0        0    73544 2024-04-03 03:36:32.000000 heaserver-buckets-1.1.1/src/heaserver/bucket/service.py
-drwxrwxrwx   0        0        0        0 2024-04-09 21:34:32.792099 heaserver-buckets-1.1.1/src/heaserver/bucket/wstl/
--rw-rw-rw-   0        0        0    14793 2024-04-09 20:01:57.000000 heaserver-buckets-1.1.1/src/heaserver/bucket/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-04-09 21:34:32.825099 heaserver-buckets-1.1.1/src/heaserver_buckets.egg-info/
--rw-rw-rw-   0        0        0     5107 2024-04-09 21:34:32.000000 heaserver-buckets-1.1.1/src/heaserver_buckets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      829 2024-04-09 21:34:32.000000 heaserver-buckets-1.1.1/src/heaserver_buckets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 21:34:32.000000 heaserver-buckets-1.1.1/src/heaserver_buckets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-04-09 21:34:32.000000 heaserver-buckets-1.1.1/src/heaserver_buckets.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-04-09 21:34:32.000000 heaserver-buckets-1.1.1/src/heaserver_buckets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-09 21:34:32.000000 heaserver-buckets-1.1.1/src/heaserver_buckets.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-09 21:34:32.722099 heaserver-buckets-1.1.1/tests/
-drwxrwxrwx   0        0        0        0 2024-04-09 21:34:32.723132 heaserver-buckets-1.1.1/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-09 21:34:32.823099 heaserver-buckets-1.1.1/tests/heaserver/buckettest/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.1/tests/heaserver/buckettest/__init__.py
--rw-rw-rw-   0        0        0     1623 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.1/tests/heaserver/buckettest/test_all.py
--rw-rw-rw-   0        0        0     9173 2024-04-09 19:49:37.000000 heaserver-buckets-1.1.1/tests/heaserver/buckettest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:38:21.713273 heaserver_buckets-1.1.2/
+-rw-rw-rw-   0        0        0      261 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.2/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.2/.gitignore
+-rw-rw-rw-   0        0        0     1515 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.2/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5197 2024-05-03 23:38:21.711567 heaserver_buckets-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3823 2024-05-02 18:39:38.000000 heaserver_buckets-1.1.2/README.md
+-rw-rw-rw-   0        0        0     1737 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.2/RELEASING.md
+-rw-rw-rw-   0        0        0      470 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.2/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-05-03 23:38:21.601436 heaserver_buckets-1.1.2/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-05-03 23:38:21.601436 heaserver_buckets-1.1.2/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-03 23:38:21.655286 heaserver_buckets-1.1.2/integrationtests/heaserver/bucketintegrationtest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.2/integrationtests/heaserver/bucketintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0     4817 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.2/integrationtests/heaserver/bucketintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0    10927 2024-04-09 21:37:15.000000 heaserver_buckets-1.1.2/integrationtests/heaserver/bucketintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.2/pytest.ini
+-rw-rw-rw-   0        0        0      262 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.2/requirements_dev.txt
+-rw-rw-rw-   0        0        0     5310 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.2/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-05-03 23:38:21.713273 heaserver_buckets-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1858 2024-05-03 23:37:00.000000 heaserver_buckets-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:38:21.604438 heaserver_buckets-1.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-03 23:38:21.603437 heaserver_buckets-1.1.2/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-03 23:38:21.657894 heaserver_buckets-1.1.2/src/heaserver/bucket/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.2/src/heaserver/bucket/__init__.py
+-rw-rw-rw-   0        0        0    73544 2024-04-03 03:36:32.000000 heaserver_buckets-1.1.2/src/heaserver/bucket/service.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:38:21.659989 heaserver_buckets-1.1.2/src/heaserver/bucket/wstl/
+-rw-rw-rw-   0        0        0    14793 2024-04-09 21:37:15.000000 heaserver_buckets-1.1.2/src/heaserver/bucket/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-05-03 23:38:21.709990 heaserver_buckets-1.1.2/src/heaserver_buckets.egg-info/
+-rw-rw-rw-   0        0        0     5197 2024-05-03 23:38:21.000000 heaserver_buckets-1.1.2/src/heaserver_buckets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      829 2024-05-03 23:38:21.000000 heaserver_buckets-1.1.2/src/heaserver_buckets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 23:38:21.000000 heaserver_buckets-1.1.2/src/heaserver_buckets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-05-03 23:38:21.000000 heaserver_buckets-1.1.2/src/heaserver_buckets.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2024-05-03 23:38:21.000000 heaserver_buckets-1.1.2/src/heaserver_buckets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-03 23:38:21.000000 heaserver_buckets-1.1.2/src/heaserver_buckets.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 23:38:21.605437 heaserver_buckets-1.1.2/tests/
+drwxrwxrwx   0        0        0        0 2024-05-03 23:38:21.605437 heaserver_buckets-1.1.2/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-03 23:38:21.708364 heaserver_buckets-1.1.2/tests/heaserver/buckettest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.2/tests/heaserver/buckettest/__init__.py
+-rw-rw-rw-   0        0        0     1623 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.2/tests/heaserver/buckettest/test_all.py
+-rw-rw-rw-   0        0        0     9173 2024-04-09 21:37:15.000000 heaserver_buckets-1.1.2/tests/heaserver/buckettest/testcase.py
```

### Comparing `heaserver-buckets-1.1.1/Dockerfile` & `heaserver_buckets-1.1.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.1.1/LICENSE` & `heaserver_buckets-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.1.1/PKG-INFO` & `heaserver_buckets-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-buckets
-Version: 1.1.1
+Version: 1.1.2
 Summary: a service for managing buckets and their data within the cloud
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-buckets,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,26 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.4.0
+Requires-Dist: heaserver~=1.5.2
+Requires-Dist: heaobject~=1.5.1
 
 # HEA Server Buckets Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Buckets Microservice is a service for managing buckets and their data within the cloud.
 
+## Version 1.1.2
+* Fixed new folder form submission.
+
 ## Version 1.1.1
 * Display type display name in properties card, and return the type display name from GET calls.
 
 ## Version 1.1.0
 * Fixed support for uploading to a bucket.
 * Pass desktop object permissions back to clients.
```

### Comparing `heaserver-buckets-1.1.1/README.md` & `heaserver_buckets-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # HEA Server Buckets Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Buckets Microservice is a service for managing buckets and their data within the cloud.
 
+## Version 1.1.2
+* Fixed new folder form submission.
+
 ## Version 1.1.1
 * Display type display name in properties card, and return the type display name from GET calls.
 
 ## Version 1.1.0
 * Fixed support for uploading to a bucket.
 * Pass desktop object permissions back to clients.
```

### Comparing `heaserver-buckets-1.1.1/RELEASING.md` & `heaserver_buckets-1.1.2/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.1.1/integrationtests/heaserver/bucketintegrationtest/test_all.py` & `heaserver_buckets-1.1.2/integrationtests/heaserver/bucketintegrationtest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.1.1/integrationtests/heaserver/bucketintegrationtest/testcase.py` & `heaserver_buckets-1.1.2/integrationtests/heaserver/bucketintegrationtest/testcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.1.1/run-swaggerui.py` & `heaserver_buckets-1.1.2/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.1.1/setup.py` & `heaserver_buckets-1.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-buckets',
-    version='1.1.1',
+    version='1.1.2',
     description="a service for managing buckets and their data within the cloud",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.bucket'],
     package_data={'heaserver.bucket': ['wstl/*.json']},
-    install_requires=['heaserver~=1.4.0'],
+    install_requires=['heaserver~=1.5.2', 'heaobject~=1.5.1'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
         'Environment :: Web Environment',
```

### Comparing `heaserver-buckets-1.1.1/src/heaserver/bucket/service.py` & `heaserver_buckets-1.1.2/src/heaserver/bucket/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.1.1/src/heaserver/bucket/wstl/all.json` & `heaserver_buckets-1.1.2/src/heaserver/bucket/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.1.1/src/heaserver_buckets.egg-info/PKG-INFO` & `heaserver_buckets-1.1.2/src/heaserver_buckets.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-buckets
-Version: 1.1.1
+Version: 1.1.2
 Summary: a service for managing buckets and their data within the cloud
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-buckets,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,26 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.4.0
+Requires-Dist: heaserver~=1.5.2
+Requires-Dist: heaobject~=1.5.1
 
 # HEA Server Buckets Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Buckets Microservice is a service for managing buckets and their data within the cloud.
 
+## Version 1.1.2
+* Fixed new folder form submission.
+
 ## Version 1.1.1
 * Display type display name in properties card, and return the type display name from GET calls.
 
 ## Version 1.1.0
 * Fixed support for uploading to a bucket.
 * Pass desktop object permissions back to clients.
```

### Comparing `heaserver-buckets-1.1.1/src/heaserver_buckets.egg-info/SOURCES.txt` & `heaserver_buckets-1.1.2/src/heaserver_buckets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.1.1/tests/heaserver/buckettest/test_all.py` & `heaserver_buckets-1.1.2/tests/heaserver/buckettest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.1.1/tests/heaserver/buckettest/testcase.py` & `heaserver_buckets-1.1.2/tests/heaserver/buckettest/testcase.py`

 * *Files identical despite different names*

