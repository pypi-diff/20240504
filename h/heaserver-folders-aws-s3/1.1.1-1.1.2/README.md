# Comparing `tmp/heaserver-folders-aws-s3-1.1.1.tar.gz` & `tmp/heaserver_folders_aws_s3-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-folders-aws-s3-1.1.1.tar", last modified: Tue Apr  9 21:48:31 2024, max compression
+gzip compressed data, was "heaserver_folders_aws_s3-1.1.2.tar", last modified: Fri May  3 23:14:25 2024, max compression
```

## Comparing `heaserver-folders-aws-s3-1.1.1.tar` & `heaserver_folders_aws_s3-1.1.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 21:48:31.088485 heaserver-folders-aws-s3-1.1.1/
--rw-rw-rw-   0        0        0      261 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.1.1/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.1/.gitignore
--rw-rw-rw-   0        0        0     1664 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.1/Dockerfile
--rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.1.1/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6559 2024-04-09 21:48:31.087484 heaserver-folders-aws-s3-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5317 2024-04-09 21:43:10.000000 heaserver-folders-aws-s3-1.1.1/README.md
--rw-rw-rw-   0        0        0     1777 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.1/RELEASING.md
--rw-rw-rw-   0        0        0      658 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.1/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-04-09 21:48:31.018487 heaserver-folders-aws-s3-1.1.1/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-04-09 21:48:31.019485 heaserver-folders-aws-s3-1.1.1/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-09 21:48:31.052486 heaserver-folders-aws-s3-1.1.1/integrationtests/heaserver/folderawss3integrationtest/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.1.1/integrationtests/heaserver/folderawss3integrationtest/__init__.py
--rw-rw-rw-   0        0        0    38201 2024-04-09 03:39:38.000000 heaserver-folders-aws-s3-1.1.1/integrationtests/heaserver/folderawss3integrationtest/folderawss3testcase.py
--rw-rw-rw-   0        0        0    40185 2024-04-09 03:40:08.000000 heaserver-folders-aws-s3-1.1.1/integrationtests/heaserver/folderawss3integrationtest/projectawss3testcase.py
--rw-rw-rw-   0        0        0    30533 2024-04-09 05:12:41.000000 heaserver-folders-aws-s3-1.1.1/integrationtests/heaserver/folderawss3integrationtest/test_all.py
--rw-rw-rw-   0        0        0      111 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.1/pytest.ini
--rw-rw-rw-   0        0        0      261 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.1/requirements_dev.txt
--rw-rw-rw-   0        0        0    14460 2024-03-22 02:50:09.000000 heaserver-folders-aws-s3-1.1.1/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-04-09 21:48:31.088485 heaserver-folders-aws-s3-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2473 2024-04-09 21:47:53.000000 heaserver-folders-aws-s3-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 21:48:31.021485 heaserver-folders-aws-s3-1.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-09 21:48:31.020484 heaserver-folders-aws-s3-1.1.1/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-09 21:48:31.063486 heaserver-folders-aws-s3-1.1.1/src/heaserver/folderawss3/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.1.1/src/heaserver/folderawss3/__init__.py
--rw-rw-rw-   0        0        0   154476 2024-04-09 05:22:55.000000 heaserver-folders-aws-s3-1.1.1/src/heaserver/folderawss3/projectservice.py
--rw-rw-rw-   0        0        0   157027 2024-04-09 05:22:16.000000 heaserver-folders-aws-s3-1.1.1/src/heaserver/folderawss3/service.py
--rw-rw-rw-   0        0        0     8385 2024-03-22 02:50:09.000000 heaserver-folders-aws-s3-1.1.1/src/heaserver/folderawss3/util.py
-drwxrwxrwx   0        0        0        0 2024-04-09 21:48:31.064487 heaserver-folders-aws-s3-1.1.1/src/heaserver/folderawss3/wstl/
--rw-rw-rw-   0        0        0    33204 2024-04-09 03:55:24.000000 heaserver-folders-aws-s3-1.1.1/src/heaserver/folderawss3/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-04-09 21:48:31.085484 heaserver-folders-aws-s3-1.1.1/src/heaserver_folders_aws_s3.egg-info/
--rw-rw-rw-   0        0        0     6559 2024-04-09 21:48:30.000000 heaserver-folders-aws-s3-1.1.1/src/heaserver_folders_aws_s3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1196 2024-04-09 21:48:31.000000 heaserver-folders-aws-s3-1.1.1/src/heaserver_folders_aws_s3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 21:48:30.000000 heaserver-folders-aws-s3-1.1.1/src/heaserver_folders_aws_s3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-04-09 21:48:30.000000 heaserver-folders-aws-s3-1.1.1/src/heaserver_folders_aws_s3.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-04-09 21:48:30.000000 heaserver-folders-aws-s3-1.1.1/src/heaserver_folders_aws_s3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-09 21:48:30.000000 heaserver-folders-aws-s3-1.1.1/src/heaserver_folders_aws_s3.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-09 21:48:31.022484 heaserver-folders-aws-s3-1.1.1/tests/
-drwxrwxrwx   0        0        0        0 2024-04-09 21:48:31.023487 heaserver-folders-aws-s3-1.1.1/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-09 21:48:31.081485 heaserver-folders-aws-s3-1.1.1/tests/heaserver/folderawss3test/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.1.1/tests/heaserver/folderawss3test/__init__.py
--rw-rw-rw-   0        0        0    37459 2024-04-09 02:51:46.000000 heaserver-folders-aws-s3-1.1.1/tests/heaserver/folderawss3test/folderawss3testcase.py
--rw-rw-rw-   0        0        0    38816 2024-04-09 02:52:38.000000 heaserver-folders-aws-s3-1.1.1/tests/heaserver/folderawss3test/projectawss3testcase.py
--rw-rw-rw-   0        0        0     2608 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.1/tests/heaserver/folderawss3test/test_all.py
-drwxrwxrwx   0        0        0        0 2024-04-09 21:48:31.083484 heaserver-folders-aws-s3-1.1.1/tests/heaserver/folderawss3test/wstl/
--rw-rw-rw-   0        0        0    14496 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.1/tests/heaserver/folderawss3test/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-05-03 23:14:25.065788 heaserver_folders_aws_s3-1.1.2/
+-rw-rw-rw-   0        0        0      261 2022-03-11 01:28:25.000000 heaserver_folders_aws_s3-1.1.2/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-18 20:10:59.000000 heaserver_folders_aws_s3-1.1.2/.gitignore
+-rw-rw-rw-   0        0        0     1664 2023-12-18 20:10:59.000000 heaserver_folders_aws_s3-1.1.2/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:25.000000 heaserver_folders_aws_s3-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 20:10:59.000000 heaserver_folders_aws_s3-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6616 2024-05-03 23:14:25.064788 heaserver_folders_aws_s3-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5374 2024-05-03 23:13:31.000000 heaserver_folders_aws_s3-1.1.2/README.md
+-rw-rw-rw-   0        0        0     1777 2023-12-18 20:10:59.000000 heaserver_folders_aws_s3-1.1.2/RELEASING.md
+-rw-rw-rw-   0        0        0      658 2023-12-18 20:10:59.000000 heaserver_folders_aws_s3-1.1.2/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-05-03 23:14:25.007238 heaserver_folders_aws_s3-1.1.2/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-05-03 23:14:25.008238 heaserver_folders_aws_s3-1.1.2/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-03 23:14:25.034238 heaserver_folders_aws_s3-1.1.2/integrationtests/heaserver/folderawss3integrationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:25.000000 heaserver_folders_aws_s3-1.1.2/integrationtests/heaserver/folderawss3integrationtest/__init__.py
+-rw-rw-rw-   0        0        0    38201 2024-04-09 21:50:01.000000 heaserver_folders_aws_s3-1.1.2/integrationtests/heaserver/folderawss3integrationtest/folderawss3testcase.py
+-rw-rw-rw-   0        0        0    40185 2024-04-09 21:50:01.000000 heaserver_folders_aws_s3-1.1.2/integrationtests/heaserver/folderawss3integrationtest/projectawss3testcase.py
+-rw-rw-rw-   0        0        0    30533 2024-04-09 21:50:01.000000 heaserver_folders_aws_s3-1.1.2/integrationtests/heaserver/folderawss3integrationtest/test_all.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 20:10:59.000000 heaserver_folders_aws_s3-1.1.2/pytest.ini
+-rw-rw-rw-   0        0        0      261 2023-12-18 20:10:59.000000 heaserver_folders_aws_s3-1.1.2/requirements_dev.txt
+-rw-rw-rw-   0        0        0    14460 2024-03-22 02:50:09.000000 heaserver_folders_aws_s3-1.1.2/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-05-03 23:14:25.065788 heaserver_folders_aws_s3-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2473 2024-05-03 23:13:31.000000 heaserver_folders_aws_s3-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:14:25.010237 heaserver_folders_aws_s3-1.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-03 23:14:25.009238 heaserver_folders_aws_s3-1.1.2/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-03 23:14:25.042791 heaserver_folders_aws_s3-1.1.2/src/heaserver/folderawss3/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:25.000000 heaserver_folders_aws_s3-1.1.2/src/heaserver/folderawss3/__init__.py
+-rw-rw-rw-   0        0        0   154476 2024-04-09 21:50:01.000000 heaserver_folders_aws_s3-1.1.2/src/heaserver/folderawss3/projectservice.py
+-rw-rw-rw-   0        0        0   157027 2024-04-09 21:50:01.000000 heaserver_folders_aws_s3-1.1.2/src/heaserver/folderawss3/service.py
+-rw-rw-rw-   0        0        0     8385 2024-03-22 02:50:09.000000 heaserver_folders_aws_s3-1.1.2/src/heaserver/folderawss3/util.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:14:25.043789 heaserver_folders_aws_s3-1.1.2/src/heaserver/folderawss3/wstl/
+-rw-rw-rw-   0        0        0    33204 2024-04-09 21:50:01.000000 heaserver_folders_aws_s3-1.1.2/src/heaserver/folderawss3/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-05-03 23:14:25.063788 heaserver_folders_aws_s3-1.1.2/src/heaserver_folders_aws_s3.egg-info/
+-rw-rw-rw-   0        0        0     6616 2024-05-03 23:14:24.000000 heaserver_folders_aws_s3-1.1.2/src/heaserver_folders_aws_s3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1196 2024-05-03 23:14:25.000000 heaserver_folders_aws_s3-1.1.2/src/heaserver_folders_aws_s3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 23:14:24.000000 heaserver_folders_aws_s3-1.1.2/src/heaserver_folders_aws_s3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-03 23:14:24.000000 heaserver_folders_aws_s3-1.1.2/src/heaserver_folders_aws_s3.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-05-03 23:14:24.000000 heaserver_folders_aws_s3-1.1.2/src/heaserver_folders_aws_s3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-03 23:14:24.000000 heaserver_folders_aws_s3-1.1.2/src/heaserver_folders_aws_s3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 23:14:25.010237 heaserver_folders_aws_s3-1.1.2/tests/
+drwxrwxrwx   0        0        0        0 2024-05-03 23:14:25.011237 heaserver_folders_aws_s3-1.1.2/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-03 23:14:25.060788 heaserver_folders_aws_s3-1.1.2/tests/heaserver/folderawss3test/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:25.000000 heaserver_folders_aws_s3-1.1.2/tests/heaserver/folderawss3test/__init__.py
+-rw-rw-rw-   0        0        0    37459 2024-04-09 21:50:01.000000 heaserver_folders_aws_s3-1.1.2/tests/heaserver/folderawss3test/folderawss3testcase.py
+-rw-rw-rw-   0        0        0    38816 2024-04-09 21:50:01.000000 heaserver_folders_aws_s3-1.1.2/tests/heaserver/folderawss3test/projectawss3testcase.py
+-rw-rw-rw-   0        0        0     2608 2023-12-18 20:10:59.000000 heaserver_folders_aws_s3-1.1.2/tests/heaserver/folderawss3test/test_all.py
+drwxrwxrwx   0        0        0        0 2024-05-03 23:14:25.061788 heaserver_folders_aws_s3-1.1.2/tests/heaserver/folderawss3test/wstl/
+-rw-rw-rw-   0        0        0    14496 2023-12-18 20:10:59.000000 heaserver_folders_aws_s3-1.1.2/tests/heaserver/folderawss3test/wstl/all.json
```

### Comparing `heaserver-folders-aws-s3-1.1.1/Dockerfile` & `heaserver_folders_aws_s3-1.1.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.1.1/LICENSE` & `heaserver_folders_aws_s3-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.1.1/PKG-INFO` & `heaserver_folders_aws_s3-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-folders-aws-s3
-Version: 1.1.1
+Version: 1.1.2
 Summary: The HEA AWS S3 bucket folder service.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -20,22 +20,25 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.4.0
+Requires-Dist: heaserver~=1.5.2
 
 # HEA Server AWS S3 Bucket Folders Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/),
 Salt Lake City, UT
 
 The HEA Server AWS S3 Bucket Folders Microservice manages folders in AWS S3 buckets.
 
+## Version 1.1.2
+* Fixed new folder form submission.
+
 ## Version 1.1.1
 * Display type display name in properties card, and return the type display name from GET calls.
 
 ## Version 1.1.0
 * Pass folder and project permissions back to clients.
 
 ## Version 1.0.13
```

### Comparing `heaserver-folders-aws-s3-1.1.1/README.md` & `heaserver_folders_aws_s3-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # HEA Server AWS S3 Bucket Folders Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/),
 Salt Lake City, UT
 
 The HEA Server AWS S3 Bucket Folders Microservice manages folders in AWS S3 buckets.
 
+## Version 1.1.2
+* Fixed new folder form submission.
+
 ## Version 1.1.1
 * Display type display name in properties card, and return the type display name from GET calls.
 
 ## Version 1.1.0
 * Pass folder and project permissions back to clients.
 
 ## Version 1.0.13
```

### Comparing `heaserver-folders-aws-s3-1.1.1/RELEASING.md` & `heaserver_folders_aws_s3-1.1.2/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.1.1/docker-entrypoint.sh` & `heaserver_folders_aws_s3-1.1.2/docker-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.1.1/integrationtests/heaserver/folderawss3integrationtest/folderawss3testcase.py` & `heaserver_folders_aws_s3-1.1.2/integrationtests/heaserver/folderawss3integrationtest/folderawss3testcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.1.1/integrationtests/heaserver/folderawss3integrationtest/projectawss3testcase.py` & `heaserver_folders_aws_s3-1.1.2/integrationtests/heaserver/folderawss3integrationtest/projectawss3testcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.1.1/integrationtests/heaserver/folderawss3integrationtest/test_all.py` & `heaserver_folders_aws_s3-1.1.2/integrationtests/heaserver/folderawss3integrationtest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.1.1/run-swaggerui.py` & `heaserver_folders_aws_s3-1.1.2/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.1.1/setup.py` & `heaserver_folders_aws_s3-1.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(name='heaserver-folders-aws-s3',
-                 version='1.1.1',
+                 version='1.1.2',
                  description='The HEA AWS S3 bucket folder service.',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  url='https://risr.hci.utah.edu',
                  author='Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT',
                  author_email='Andrew.Post@hci.utah.edu',
                  python_requires='>=3.10',
                  package_dir={'': 'src'},
                  packages=['heaserver.folderawss3'],
                  package_data={'heaserver.folderawss3': ['wstl/*.json']},
                  install_requires=[
-                     'heaserver~=1.4.0'
+                     'heaserver~=1.5.2'
                  ],
                  classifiers=[
                      'Development Status :: 5 - Production/Stable',
                      'Intended Audience :: Developers',
                      'Intended Audience :: Science/Research',
                      'License :: OSI Approved :: Apache Software License',
                      'Framework :: AsyncIO',
```

### Comparing `heaserver-folders-aws-s3-1.1.1/src/heaserver/folderawss3/projectservice.py` & `heaserver_folders_aws_s3-1.1.2/src/heaserver/folderawss3/projectservice.py`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.1.1/src/heaserver/folderawss3/service.py` & `heaserver_folders_aws_s3-1.1.2/src/heaserver/folderawss3/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.1.1/src/heaserver/folderawss3/util.py` & `heaserver_folders_aws_s3-1.1.2/src/heaserver/folderawss3/util.py`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.1.1/src/heaserver/folderawss3/wstl/all.json` & `heaserver_folders_aws_s3-1.1.2/src/heaserver/folderawss3/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.1.1/src/heaserver_folders_aws_s3.egg-info/PKG-INFO` & `heaserver_folders_aws_s3-1.1.2/src/heaserver_folders_aws_s3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-folders-aws-s3
-Version: 1.1.1
+Version: 1.1.2
 Summary: The HEA AWS S3 bucket folder service.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -20,22 +20,25 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.4.0
+Requires-Dist: heaserver~=1.5.2
 
 # HEA Server AWS S3 Bucket Folders Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/),
 Salt Lake City, UT
 
 The HEA Server AWS S3 Bucket Folders Microservice manages folders in AWS S3 buckets.
 
+## Version 1.1.2
+* Fixed new folder form submission.
+
 ## Version 1.1.1
 * Display type display name in properties card, and return the type display name from GET calls.
 
 ## Version 1.1.0
 * Pass folder and project permissions back to clients.
 
 ## Version 1.0.13
```

### Comparing `heaserver-folders-aws-s3-1.1.1/src/heaserver_folders_aws_s3.egg-info/SOURCES.txt` & `heaserver_folders_aws_s3-1.1.2/src/heaserver_folders_aws_s3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.1.1/tests/heaserver/folderawss3test/folderawss3testcase.py` & `heaserver_folders_aws_s3-1.1.2/tests/heaserver/folderawss3test/folderawss3testcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.1.1/tests/heaserver/folderawss3test/projectawss3testcase.py` & `heaserver_folders_aws_s3-1.1.2/tests/heaserver/folderawss3test/projectawss3testcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.1.1/tests/heaserver/folderawss3test/test_all.py` & `heaserver_folders_aws_s3-1.1.2/tests/heaserver/folderawss3test/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.1.1/tests/heaserver/folderawss3test/wstl/all.json` & `heaserver_folders_aws_s3-1.1.2/tests/heaserver/folderawss3test/wstl/all.json`

 * *Files identical despite different names*

