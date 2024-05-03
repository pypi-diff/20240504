# Comparing `tmp/heaserver_accounts-1.1.1.tar.gz` & `tmp/heaserver_accounts-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver_accounts-1.1.1.tar", last modified: Thu May  2 20:42:09 2024, max compression
+gzip compressed data, was "heaserver_accounts-1.1.2.tar", last modified: Fri May  3 22:19:11 2024, max compression
```

## Comparing `heaserver_accounts-1.1.1.tar` & `heaserver_accounts-1.1.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 20:42:09.814577 heaserver_accounts-1.1.1/
--rw-rw-rw-   0        0        0      261 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.1/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.1/.gitignore
--rw-rw-rw-   0        0        0     1624 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.1/Dockerfile
--rw-rw-rw-   0        0        0    11625 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.1/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5973 2024-05-02 20:42:09.813521 heaserver_accounts-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4665 2024-05-02 20:08:33.000000 heaserver_accounts-1.1.1/README.md
--rw-rw-rw-   0        0        0     1878 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.1/RELEASING.md
--rw-rw-rw-   0        0        0      441 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.1/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-05-02 20:42:09.620346 heaserver_accounts-1.1.1/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-05-02 20:42:09.620346 heaserver_accounts-1.1.1/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-02 20:42:09.750656 heaserver_accounts-1.1.1/integrationtests/heaserver/accountintegrationtest/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.1/integrationtests/heaserver/accountintegrationtest/__init__.py
--rw-rw-rw-   0        0        0      481 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.1/integrationtests/heaserver/accountintegrationtest/test_all.py
--rw-rw-rw-   0        0        0     7797 2024-04-09 21:25:34.000000 heaserver_accounts-1.1.1/integrationtests/heaserver/accountintegrationtest/testcase.py
--rw-rw-rw-   0        0        0      111 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.1/pytest.ini
--rw-rw-rw-   0        0        0      262 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.1/requirements_dev.txt
--rw-rw-rw-   0        0        0     4294 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.1/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-05-02 20:42:09.815101 heaserver_accounts-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1825 2024-05-02 20:40:26.000000 heaserver_accounts-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-02 20:42:09.623341 heaserver_accounts-1.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-02 20:42:09.622339 heaserver_accounts-1.1.1/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-02 20:42:09.754325 heaserver_accounts-1.1.1/src/heaserver/account/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.1/src/heaserver/account/__init__.py
--rw-rw-rw-   0        0        0    47097 2024-05-02 20:39:51.000000 heaserver_accounts-1.1.1/src/heaserver/account/service.py
-drwxrwxrwx   0        0        0        0 2024-05-02 20:42:09.755951 heaserver_accounts-1.1.1/src/heaserver/account/wstl/
--rw-rw-rw-   0        0        0    11957 2024-05-02 20:08:33.000000 heaserver_accounts-1.1.1/src/heaserver/account/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-05-02 20:42:09.811946 heaserver_accounts-1.1.1/src/heaserver_accounts.egg-info/
--rw-rw-rw-   0        0        0     5973 2024-05-02 20:42:09.000000 heaserver_accounts-1.1.1/src/heaserver_accounts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      844 2024-05-02 20:42:09.000000 heaserver_accounts-1.1.1/src/heaserver_accounts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 20:42:09.000000 heaserver_accounts-1.1.1/src/heaserver_accounts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-05-02 20:42:09.000000 heaserver_accounts-1.1.1/src/heaserver_accounts.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-05-02 20:42:09.000000 heaserver_accounts-1.1.1/src/heaserver_accounts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-02 20:42:09.000000 heaserver_accounts-1.1.1/src/heaserver_accounts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-02 20:42:09.624339 heaserver_accounts-1.1.1/tests/
-drwxrwxrwx   0        0        0        0 2024-05-02 20:42:09.624339 heaserver_accounts-1.1.1/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-02 20:42:09.809834 heaserver_accounts-1.1.1/tests/heaserver/accounttest/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.1/tests/heaserver/accounttest/__init__.py
--rw-rw-rw-   0        0        0     7626 2024-04-09 21:25:34.000000 heaserver_accounts-1.1.1/tests/heaserver/accounttest/test_all.py
--rw-rw-rw-   0        0        0     5462 2024-05-02 20:39:51.000000 heaserver_accounts-1.1.1/tests/heaserver/accounttest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-05-03 22:19:11.086614 heaserver_accounts-1.1.2/
+-rw-rw-rw-   0        0        0      261 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.2/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.2/.gitignore
+-rw-rw-rw-   0        0        0     1624 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.2/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6020 2024-05-03 22:19:11.084508 heaserver_accounts-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4712 2024-05-03 22:17:46.000000 heaserver_accounts-1.1.2/README.md
+-rw-rw-rw-   0        0        0     1878 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.2/RELEASING.md
+-rw-rw-rw-   0        0        0      441 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.2/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-05-03 22:19:10.982010 heaserver_accounts-1.1.2/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-05-03 22:19:10.983043 heaserver_accounts-1.1.2/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-03 22:19:11.032118 heaserver_accounts-1.1.2/integrationtests/heaserver/accountintegrationtest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.2/integrationtests/heaserver/accountintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0      481 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.2/integrationtests/heaserver/accountintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0     7797 2024-04-09 21:25:34.000000 heaserver_accounts-1.1.2/integrationtests/heaserver/accountintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.2/pytest.ini
+-rw-rw-rw-   0        0        0      262 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.2/requirements_dev.txt
+-rw-rw-rw-   0        0        0     4294 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.2/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-05-03 22:19:11.087148 heaserver_accounts-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1825 2024-05-03 22:18:16.000000 heaserver_accounts-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 22:19:10.985011 heaserver_accounts-1.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-03 22:19:10.984012 heaserver_accounts-1.1.2/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-03 22:19:11.035812 heaserver_accounts-1.1.2/src/heaserver/account/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.2/src/heaserver/account/__init__.py
+-rw-rw-rw-   0        0        0    47097 2024-05-03 22:13:10.000000 heaserver_accounts-1.1.2/src/heaserver/account/service.py
+drwxrwxrwx   0        0        0        0 2024-05-03 22:19:11.037389 heaserver_accounts-1.1.2/src/heaserver/account/wstl/
+-rw-rw-rw-   0        0        0    11957 2024-05-03 03:06:58.000000 heaserver_accounts-1.1.2/src/heaserver/account/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-05-03 22:19:11.083287 heaserver_accounts-1.1.2/src/heaserver_accounts.egg-info/
+-rw-rw-rw-   0        0        0     6020 2024-05-03 22:19:10.000000 heaserver_accounts-1.1.2/src/heaserver_accounts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      844 2024-05-03 22:19:10.000000 heaserver_accounts-1.1.2/src/heaserver_accounts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 22:19:10.000000 heaserver_accounts-1.1.2/src/heaserver_accounts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-05-03 22:19:10.000000 heaserver_accounts-1.1.2/src/heaserver_accounts.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-05-03 22:19:10.000000 heaserver_accounts-1.1.2/src/heaserver_accounts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-03 22:19:10.000000 heaserver_accounts-1.1.2/src/heaserver_accounts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-03 22:19:10.986010 heaserver_accounts-1.1.2/tests/
+drwxrwxrwx   0        0        0        0 2024-05-03 22:19:10.986010 heaserver_accounts-1.1.2/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-03 22:19:11.081221 heaserver_accounts-1.1.2/tests/heaserver/accounttest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.2/tests/heaserver/accounttest/__init__.py
+-rw-rw-rw-   0        0        0     7626 2024-04-09 21:25:34.000000 heaserver_accounts-1.1.2/tests/heaserver/accounttest/test_all.py
+-rw-rw-rw-   0        0        0     5462 2024-05-03 22:13:10.000000 heaserver_accounts-1.1.2/tests/heaserver/accounttest/testcase.py
```

### Comparing `heaserver_accounts-1.1.1/Dockerfile` & `heaserver_accounts-1.1.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver_accounts-1.1.1/LICENSE` & `heaserver_accounts-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver_accounts-1.1.1/PKG-INFO` & `heaserver_accounts-1.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-accounts
-Version: 1.1.1
+Version: 1.1.2
 Summary: Manages account information
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-accounts,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,25 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.5.1
+Requires-Dist: heaserver~=1.5.2
 
 # HEA Server AWS Accounts Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server AWS Accounts Microservice is It manages the AWS account information details.
 
+## Version 1.1.2
+* Fixed crash regression.
+
 ## Version 1.1.1
 * Fixed new bucket form submission.
 
 ## Version 1.1.0
 * Removed the PUT and DELETE account calls because neither works.
 
 ## Version 1.0.8
```

### Comparing `heaserver_accounts-1.1.1/README.md` & `heaserver_accounts-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # HEA Server AWS Accounts Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server AWS Accounts Microservice is It manages the AWS account information details.
 
+## Version 1.1.2
+* Fixed crash regression.
+
 ## Version 1.1.1
 * Fixed new bucket form submission.
 
 ## Version 1.1.0
 * Removed the PUT and DELETE account calls because neither works.
 
 ## Version 1.0.8
```

### Comparing `heaserver_accounts-1.1.1/RELEASING.md` & `heaserver_accounts-1.1.2/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver_accounts-1.1.1/integrationtests/heaserver/accountintegrationtest/testcase.py` & `heaserver_accounts-1.1.2/integrationtests/heaserver/accountintegrationtest/testcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_accounts-1.1.1/run-swaggerui.py` & `heaserver_accounts-1.1.2/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver_accounts-1.1.1/setup.py` & `heaserver_accounts-1.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-accounts',
-    version='1.1.1',
+    version='1.1.2',
     description="Manages account information",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.account'],
     package_data={'heaserver.account': ['wstl/*.json']},
     install_requires=[
-        'heaserver~=1.5.1'
+        'heaserver~=1.5.2'
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
```

### Comparing `heaserver_accounts-1.1.1/src/heaserver/account/service.py` & `heaserver_accounts-1.1.2/src/heaserver/account/service.py`

 * *Files identical despite different names*

### Comparing `heaserver_accounts-1.1.1/src/heaserver/account/wstl/all.json` & `heaserver_accounts-1.1.2/src/heaserver/account/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver_accounts-1.1.1/src/heaserver_accounts.egg-info/PKG-INFO` & `heaserver_accounts-1.1.2/src/heaserver_accounts.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-accounts
-Version: 1.1.1
+Version: 1.1.2
 Summary: Manages account information
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-accounts,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,25 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.5.1
+Requires-Dist: heaserver~=1.5.2
 
 # HEA Server AWS Accounts Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server AWS Accounts Microservice is It manages the AWS account information details.
 
+## Version 1.1.2
+* Fixed crash regression.
+
 ## Version 1.1.1
 * Fixed new bucket form submission.
 
 ## Version 1.1.0
 * Removed the PUT and DELETE account calls because neither works.
 
 ## Version 1.0.8
```

### Comparing `heaserver_accounts-1.1.1/src/heaserver_accounts.egg-info/SOURCES.txt` & `heaserver_accounts-1.1.2/src/heaserver_accounts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver_accounts-1.1.1/tests/heaserver/accounttest/test_all.py` & `heaserver_accounts-1.1.2/tests/heaserver/accounttest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver_accounts-1.1.1/tests/heaserver/accounttest/testcase.py` & `heaserver_accounts-1.1.2/tests/heaserver/accounttest/testcase.py`

 * *Files identical despite different names*

