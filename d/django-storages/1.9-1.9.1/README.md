# Comparing `tmp/django-storages-1.9.tar.gz` & `tmp/django-storages-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-storages-1.9.tar", last modified: Mon Feb  3 07:27:27 2020, max compression
+gzip compressed data, was "dist/django-storages-1.9.1.tar", last modified: Tue Feb  4 06:44:13 2020, max compression
```

## Comparing `django-storages-1.9.tar` & `django-storages-1.9.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2020-02-03 07:27:27.000000 django-storages-1.9/
--rw-r--r--   0 josh       (501) staff       (20)     1585 2020-02-02 22:26:59.000000 django-storages-1.9/AUTHORS
--rw-r--r--   0 josh       (501) staff       (20)    38031 2020-02-03 07:25:34.000000 django-storages-1.9/CHANGELOG.rst
--rw-r--r--   0 josh       (501) staff       (20)     1532 2019-09-09 04:46:10.000000 django-storages-1.9/LICENSE
--rw-r--r--   0 josh       (501) staff       (20)      133 2018-10-02 03:27:46.000000 django-storages-1.9/MANIFEST.in
--rw-r--r--   0 josh       (501) staff       (20)    49484 2020-02-03 07:27:27.000000 django-storages-1.9/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)     3339 2020-01-20 00:01:11.000000 django-storages-1.9/README.rst
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2020-02-03 07:27:27.000000 django-storages-1.9/django_storages.egg-info/
--rw-r--r--   0 josh       (501) staff       (20)    49484 2020-02-03 07:27:27.000000 django-storages-1.9/django_storages.egg-info/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)     1249 2020-02-03 07:27:27.000000 django-storages-1.9/django_storages.egg-info/SOURCES.txt
--rw-r--r--   0 josh       (501) staff       (20)        1 2020-02-03 07:27:27.000000 django-storages-1.9/django_storages.egg-info/dependency_links.txt
--rw-r--r--   0 josh       (501) staff       (20)        1 2020-02-03 07:27:27.000000 django-storages-1.9/django_storages.egg-info/not-zip-safe
--rw-r--r--   0 josh       (501) staff       (20)      188 2020-02-03 07:27:27.000000 django-storages-1.9/django_storages.egg-info/requires.txt
--rw-r--r--   0 josh       (501) staff       (20)        9 2020-02-03 07:27:27.000000 django-storages-1.9/django_storages.egg-info/top_level.txt
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2020-02-03 07:27:27.000000 django-storages-1.9/docs/
--rw-r--r--   0 josh       (501) staff       (20)     4626 2017-11-24 19:18:18.000000 django-storages-1.9/docs/Makefile
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2020-02-03 07:27:27.000000 django-storages-1.9/docs/backends/
--rw-r--r--   0 josh       (501) staff       (20)    11377 2020-02-03 07:25:31.000000 django-storages-1.9/docs/backends/amazon-S3.rst
--rw-r--r--   0 josh       (501) staff       (20)     6190 2020-02-02 22:26:59.000000 django-storages-1.9/docs/backends/apache_libcloud.rst
--rw-r--r--   0 josh       (501) staff       (20)     5251 2020-02-02 22:26:59.000000 django-storages-1.9/docs/backends/azure.rst
--rw-r--r--   0 josh       (501) staff       (20)      507 2020-02-02 22:26:59.000000 django-storages-1.9/docs/backends/digital-ocean-spaces.rst
--rw-r--r--   0 josh       (501) staff       (20)     1035 2019-09-09 04:46:10.000000 django-storages-1.9/docs/backends/dropbox.rst
--rw-r--r--   0 josh       (501) staff       (20)      715 2019-09-09 04:46:10.000000 django-storages-1.9/docs/backends/ftp.rst
--rw-r--r--   0 josh       (501) staff       (20)     9569 2020-02-03 07:25:31.000000 django-storages-1.9/docs/backends/gcloud.rst
--rw-r--r--   0 josh       (501) staff       (20)     2313 2019-09-09 04:46:10.000000 django-storages-1.9/docs/backends/sftp.rst
--rw-r--r--   0 josh       (501) staff       (20)     8337 2018-10-02 03:27:49.000000 django-storages-1.9/docs/conf.py
--rw-r--r--   0 josh       (501) staff       (20)      938 2018-10-02 03:27:46.000000 django-storages-1.9/docs/index.rst
--rw-r--r--   0 josh       (501) staff       (20)     4529 2017-11-24 19:18:18.000000 django-storages-1.9/docs/make.bat
--rw-r--r--   0 josh       (501) staff       (20)      308 2020-02-03 07:27:27.000000 django-storages-1.9/setup.cfg
--rw-r--r--   0 josh       (501) staff       (20)     1877 2020-02-02 23:22:10.000000 django-storages-1.9/setup.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2020-02-03 07:27:27.000000 django-storages-1.9/storages/
--rw-r--r--   0 josh       (501) staff       (20)       20 2020-02-03 07:25:34.000000 django-storages-1.9/storages/__init__.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2020-02-03 07:27:27.000000 django-storages-1.9/storages/backends/
--rw-r--r--   0 josh       (501) staff       (20)        0 2017-11-24 19:18:18.000000 django-storages-1.9/storages/backends/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)     7422 2020-02-02 22:26:59.000000 django-storages-1.9/storages/backends/apache_libcloud.py
--rw-r--r--   0 josh       (501) staff       (20)    11963 2020-02-02 22:26:59.000000 django-storages-1.9/storages/backends/azure_storage.py
--rw-r--r--   0 josh       (501) staff       (20)     5335 2020-02-03 06:50:22.000000 django-storages-1.9/storages/backends/dropbox.py
--rw-r--r--   0 josh       (501) staff       (20)     9907 2020-02-02 22:26:59.000000 django-storages-1.9/storages/backends/ftp.py
--rw-r--r--   0 josh       (501) staff       (20)    10775 2020-02-03 07:25:31.000000 django-storages-1.9/storages/backends/gcloud.py
--rw-r--r--   0 josh       (501) staff       (20)    29275 2020-02-03 07:25:31.000000 django-storages-1.9/storages/backends/s3boto3.py
--rw-r--r--   0 josh       (501) staff       (20)     7878 2020-02-02 22:26:59.000000 django-storages-1.9/storages/backends/sftpstorage.py
--rw-r--r--   0 josh       (501) staff       (20)     3700 2020-02-02 22:26:59.000000 django-storages-1.9/storages/utils.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2020-02-03 07:27:27.000000 django-storages-1.9/tests/
--rw-r--r--   0 josh       (501) staff       (20)        0 2017-11-24 19:18:18.000000 django-storages-1.9/tests/__init__.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2020-02-03 07:27:27.000000 django-storages-1.9/tests/integration/
--rw-r--r--   0 josh       (501) staff       (20)       24 2018-10-02 03:27:46.000000 django-storages-1.9/tests/integration/__init__.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2020-02-03 07:27:27.000000 django-storages-1.9/tests/integration/migrations/
--rw-r--r--   0 josh       (501) staff       (20)      509 2019-09-08 06:14:27.000000 django-storages-1.9/tests/integration/migrations/0001_initial.py
--rw-r--r--   0 josh       (501) staff       (20)        0 2018-10-02 03:27:46.000000 django-storages-1.9/tests/integration/migrations/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)      152 2019-09-08 06:14:27.000000 django-storages-1.9/tests/integration/models.py
--rw-r--r--   0 josh       (501) staff       (20)      507 2020-02-02 22:26:59.000000 django-storages-1.9/tests/integration/settings.py
--rw-r--r--   0 josh       (501) staff       (20)    11062 2019-09-10 06:18:51.000000 django-storages-1.9/tests/integration/test_azure.py
--rw-r--r--   0 josh       (501) staff       (20)      184 2019-09-08 06:14:27.000000 django-storages-1.9/tests/settings.py
--rw-r--r--   0 josh       (501) staff       (20)    16770 2020-02-02 22:26:59.000000 django-storages-1.9/tests/test_azure.py
--rw-r--r--   0 josh       (501) staff       (20)     6790 2020-02-02 22:26:59.000000 django-storages-1.9/tests/test_dropbox.py
--rw-r--r--   0 josh       (501) staff       (20)     9067 2019-09-08 06:14:27.000000 django-storages-1.9/tests/test_ftp.py
--rw-r--r--   0 josh       (501) staff       (20)    17520 2020-02-03 07:25:31.000000 django-storages-1.9/tests/test_gcloud.py
--rw-r--r--   0 josh       (501) staff       (20)    24778 2020-02-03 07:25:31.000000 django-storages-1.9/tests/test_s3boto3.py
--rw-r--r--   0 josh       (501) staff       (20)     6674 2019-09-08 06:14:27.000000 django-storages-1.9/tests/test_sftp.py
--rw-r--r--   0 josh       (501) staff       (20)     4663 2019-09-08 06:14:27.000000 django-storages-1.9/tests/test_utils.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2020-02-04 06:44:13.000000 django-storages-1.9.1/
+-rw-r--r--   0 josh       (501) staff       (20)     1613 2020-02-03 07:46:04.000000 django-storages-1.9.1/AUTHORS
+-rw-r--r--   0 josh       (501) staff       (20)    38269 2020-02-04 06:43:22.000000 django-storages-1.9.1/CHANGELOG.rst
+-rw-r--r--   0 josh       (501) staff       (20)     1532 2019-09-09 04:46:10.000000 django-storages-1.9.1/LICENSE
+-rw-r--r--   0 josh       (501) staff       (20)      133 2018-10-02 03:27:46.000000 django-storages-1.9.1/MANIFEST.in
+-rw-r--r--   0 josh       (501) staff       (20)    50486 2020-02-04 06:44:13.000000 django-storages-1.9.1/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)     3909 2020-02-03 07:41:07.000000 django-storages-1.9.1/README.rst
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2020-02-04 06:44:13.000000 django-storages-1.9.1/django_storages.egg-info/
+-rw-r--r--   0 josh       (501) staff       (20)    50486 2020-02-04 06:44:13.000000 django-storages-1.9.1/django_storages.egg-info/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)     1249 2020-02-04 06:44:13.000000 django-storages-1.9.1/django_storages.egg-info/SOURCES.txt
+-rw-r--r--   0 josh       (501) staff       (20)        1 2020-02-04 06:44:13.000000 django-storages-1.9.1/django_storages.egg-info/dependency_links.txt
+-rw-r--r--   0 josh       (501) staff       (20)        1 2020-02-04 06:44:13.000000 django-storages-1.9.1/django_storages.egg-info/not-zip-safe
+-rw-r--r--   0 josh       (501) staff       (20)      188 2020-02-04 06:44:13.000000 django-storages-1.9.1/django_storages.egg-info/requires.txt
+-rw-r--r--   0 josh       (501) staff       (20)        9 2020-02-04 06:44:13.000000 django-storages-1.9.1/django_storages.egg-info/top_level.txt
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2020-02-04 06:44:13.000000 django-storages-1.9.1/docs/
+-rw-r--r--   0 josh       (501) staff       (20)     4626 2017-11-24 19:18:18.000000 django-storages-1.9.1/docs/Makefile
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2020-02-04 06:44:13.000000 django-storages-1.9.1/docs/backends/
+-rw-r--r--   0 josh       (501) staff       (20)    15574 2020-02-03 07:45:14.000000 django-storages-1.9.1/docs/backends/amazon-S3.rst
+-rw-r--r--   0 josh       (501) staff       (20)     6190 2020-02-02 22:26:59.000000 django-storages-1.9.1/docs/backends/apache_libcloud.rst
+-rw-r--r--   0 josh       (501) staff       (20)     5251 2020-02-02 22:26:59.000000 django-storages-1.9.1/docs/backends/azure.rst
+-rw-r--r--   0 josh       (501) staff       (20)      507 2020-02-02 22:26:59.000000 django-storages-1.9.1/docs/backends/digital-ocean-spaces.rst
+-rw-r--r--   0 josh       (501) staff       (20)     1035 2019-09-09 04:46:10.000000 django-storages-1.9.1/docs/backends/dropbox.rst
+-rw-r--r--   0 josh       (501) staff       (20)      715 2019-09-09 04:46:10.000000 django-storages-1.9.1/docs/backends/ftp.rst
+-rw-r--r--   0 josh       (501) staff       (20)     9569 2020-02-03 07:25:31.000000 django-storages-1.9.1/docs/backends/gcloud.rst
+-rw-r--r--   0 josh       (501) staff       (20)     2313 2019-09-09 04:46:10.000000 django-storages-1.9.1/docs/backends/sftp.rst
+-rw-r--r--   0 josh       (501) staff       (20)     8337 2018-10-02 03:27:49.000000 django-storages-1.9.1/docs/conf.py
+-rw-r--r--   0 josh       (501) staff       (20)      938 2018-10-02 03:27:46.000000 django-storages-1.9.1/docs/index.rst
+-rw-r--r--   0 josh       (501) staff       (20)     4529 2017-11-24 19:18:18.000000 django-storages-1.9.1/docs/make.bat
+-rw-r--r--   0 josh       (501) staff       (20)      308 2020-02-04 06:44:13.000000 django-storages-1.9.1/setup.cfg
+-rw-r--r--   0 josh       (501) staff       (20)     1877 2020-02-02 23:22:10.000000 django-storages-1.9.1/setup.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2020-02-04 06:44:13.000000 django-storages-1.9.1/storages/
+-rw-r--r--   0 josh       (501) staff       (20)       22 2020-02-04 06:43:22.000000 django-storages-1.9.1/storages/__init__.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2020-02-04 06:44:13.000000 django-storages-1.9.1/storages/backends/
+-rw-r--r--   0 josh       (501) staff       (20)        0 2017-11-24 19:18:18.000000 django-storages-1.9.1/storages/backends/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)     7422 2020-02-02 22:26:59.000000 django-storages-1.9.1/storages/backends/apache_libcloud.py
+-rw-r--r--   0 josh       (501) staff       (20)    11963 2020-02-02 22:26:59.000000 django-storages-1.9.1/storages/backends/azure_storage.py
+-rw-r--r--   0 josh       (501) staff       (20)     5335 2020-02-03 06:50:22.000000 django-storages-1.9.1/storages/backends/dropbox.py
+-rw-r--r--   0 josh       (501) staff       (20)     9907 2020-02-02 22:26:59.000000 django-storages-1.9.1/storages/backends/ftp.py
+-rw-r--r--   0 josh       (501) staff       (20)    10775 2020-02-03 07:25:31.000000 django-storages-1.9.1/storages/backends/gcloud.py
+-rw-r--r--   0 josh       (501) staff       (20)    29297 2020-02-04 06:43:19.000000 django-storages-1.9.1/storages/backends/s3boto3.py
+-rw-r--r--   0 josh       (501) staff       (20)     7878 2020-02-02 22:26:59.000000 django-storages-1.9.1/storages/backends/sftpstorage.py
+-rw-r--r--   0 josh       (501) staff       (20)     3700 2020-02-02 22:26:59.000000 django-storages-1.9.1/storages/utils.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2020-02-04 06:44:13.000000 django-storages-1.9.1/tests/
+-rw-r--r--   0 josh       (501) staff       (20)        0 2017-11-24 19:18:18.000000 django-storages-1.9.1/tests/__init__.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2020-02-04 06:44:13.000000 django-storages-1.9.1/tests/integration/
+-rw-r--r--   0 josh       (501) staff       (20)       24 2018-10-02 03:27:46.000000 django-storages-1.9.1/tests/integration/__init__.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2020-02-04 06:44:13.000000 django-storages-1.9.1/tests/integration/migrations/
+-rw-r--r--   0 josh       (501) staff       (20)      509 2019-09-08 06:14:27.000000 django-storages-1.9.1/tests/integration/migrations/0001_initial.py
+-rw-r--r--   0 josh       (501) staff       (20)        0 2018-10-02 03:27:46.000000 django-storages-1.9.1/tests/integration/migrations/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)      152 2019-09-08 06:14:27.000000 django-storages-1.9.1/tests/integration/models.py
+-rw-r--r--   0 josh       (501) staff       (20)      507 2020-02-02 22:26:59.000000 django-storages-1.9.1/tests/integration/settings.py
+-rw-r--r--   0 josh       (501) staff       (20)    11062 2019-09-10 06:18:51.000000 django-storages-1.9.1/tests/integration/test_azure.py
+-rw-r--r--   0 josh       (501) staff       (20)      184 2019-09-08 06:14:27.000000 django-storages-1.9.1/tests/settings.py
+-rw-r--r--   0 josh       (501) staff       (20)    16770 2020-02-02 22:26:59.000000 django-storages-1.9.1/tests/test_azure.py
+-rw-r--r--   0 josh       (501) staff       (20)     6790 2020-02-02 22:26:59.000000 django-storages-1.9.1/tests/test_dropbox.py
+-rw-r--r--   0 josh       (501) staff       (20)     9067 2019-09-08 06:14:27.000000 django-storages-1.9.1/tests/test_ftp.py
+-rw-r--r--   0 josh       (501) staff       (20)    17520 2020-02-03 07:25:31.000000 django-storages-1.9.1/tests/test_gcloud.py
+-rw-r--r--   0 josh       (501) staff       (20)    24778 2020-02-04 06:29:19.000000 django-storages-1.9.1/tests/test_s3boto3.py
+-rw-r--r--   0 josh       (501) staff       (20)     6674 2019-09-08 06:14:27.000000 django-storages-1.9.1/tests/test_sftp.py
+-rw-r--r--   0 josh       (501) staff       (20)     4663 2019-09-08 06:14:27.000000 django-storages-1.9.1/tests/test_utils.py
```

### Comparing `django-storages-1.9/AUTHORS` & `django-storages-1.9.1/AUTHORS`

 * *Files 6% similar despite different names*

```diff
@@ -35,12 +35,12 @@
     * Scott White (Google Cloud updates)
     * Alex Watt (Google Cloud Storage patch)
     * Jumpei Yoshimura (S3 docs)
     * Jon Dufresne
     * Rodrigo Gadea (Dropbox fixes)
     * Martey Dodoo
     * Chris Rink
-
+    * Shaung Cheng (S3 docs)
 
 
 Extra thanks to Marty for adding this in Django,
 you can buy his very interesting book (Pro Django).
```

### Comparing `django-storages-1.9/CHANGELOG.rst` & `django-storages-1.9.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 django-storages CHANGELOG
 =========================
 
+1.9.1 (2020-02-03)
+******************
+
+S3
+--
+
+- Fix reading files with ``S3Boto3StorageFile`` (`#831`_, `#833`_)
+
+.. _#831: https://github.com/jschneier/django-storages/issues/831
+.. _#833: https://github.com/jschneier/django-storages/pull/833
+
 1.9 (2020-02-02)
-***********************
+****************
 
 General
 -------
 
 - **Breaking**: The long deprecated S3 backend based on ``boto`` has been removed. (`#825`_)
 - Test against and support Python 3.8 (`#810`_)
```

### Comparing `django-storages-1.9/LICENSE` & `django-storages-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-storages-1.9/PKG-INFO` & `django-storages-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-storages
-Version: 1.9
+Version: 1.9.1
 Summary: Support for many storage backends in Django
 Home-page: https://github.com/jschneier/django-storages
 Author: Josh Schneier
 Author-email: josh.schneier@gmail.com
 License: BSD-3-Clause
 Description: .. image:: https://raw.githubusercontent.com/jschneier/django-storages/master/docs/logos/horizontal.png
             :alt: Django-Storages
@@ -66,14 +66,27 @@
         About
         =====
         django-storages is a project to provide a variety of storage backends in a single library.
         
         This library is usually compatible with the currently supported versions of
         Django. Check the Trove classifiers in setup.py to be sure.
         
+        django-storages is backed in part by `Tidelift`_. Check them out for all of your enterprise open source
+        software commerical support needs.
+        
+        .. _Tidelift: https://tidelift.com/subscription/pkg/pypi-django-storages?utm_source=pypi-django-storages&utm_medium=referral&utm_campaign=enterprise&utm_term=repo
+        
+        Security
+        ========
+        
+        To report a security vulnerability, please use the `Tidelift security contact`_. Tidelift will coordinate the
+        fix and disclosure. Please **do not** post a public issue on the tracker.
+        
+        .. _Tidelift security contact: https://tidelift.com/security
+        
         History
         =======
         This repo began as a fork of the original library under the package name of django-storages-redux and
         became the official successor (releasing under django-storages on PyPI) in February of 2016.
         
         Found a Bug? Something Unsupported?
         ===================================
@@ -102,16 +115,27 @@
         #. Bug me until I can merge your pull request. Also, don't forget to add
            yourself to ``AUTHORS``.
         
         
         django-storages CHANGELOG
         =========================
         
+        1.9.1 (2020-02-03)
+        ******************
+        
+        S3
+        --
+        
+        - Fix reading files with ``S3Boto3StorageFile`` (`#831`_, `#833`_)
+        
+        .. _#831: https://github.com/jschneier/django-storages/issues/831
+        .. _#833: https://github.com/jschneier/django-storages/pull/833
+        
         1.9 (2020-02-02)
-        ***********************
+        ****************
         
         General
         -------
         
         - **Breaking**: The long deprecated S3 backend based on ``boto`` has been removed. (`#825`_)
         - Test against and support Python 3.8 (`#810`_)
         
@@ -866,13 +890,13 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
-Provides-Extra: libcloud
-Provides-Extra: google
 Provides-Extra: azure
 Provides-Extra: dropbox
+Provides-Extra: libcloud
 Provides-Extra: boto3
 Provides-Extra: sftp
+Provides-Extra: google
```

### Comparing `django-storages-1.9/README.rst` & `django-storages-1.9.1/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -58,14 +58,27 @@
 About
 =====
 django-storages is a project to provide a variety of storage backends in a single library.
 
 This library is usually compatible with the currently supported versions of
 Django. Check the Trove classifiers in setup.py to be sure.
 
+django-storages is backed in part by `Tidelift`_. Check them out for all of your enterprise open source
+software commerical support needs.
+
+.. _Tidelift: https://tidelift.com/subscription/pkg/pypi-django-storages?utm_source=pypi-django-storages&utm_medium=referral&utm_campaign=enterprise&utm_term=repo
+
+Security
+========
+
+To report a security vulnerability, please use the `Tidelift security contact`_. Tidelift will coordinate the
+fix and disclosure. Please **do not** post a public issue on the tracker.
+
+.. _Tidelift security contact: https://tidelift.com/security
+
 History
 =======
 This repo began as a fork of the original library under the package name of django-storages-redux and
 became the official successor (releasing under django-storages on PyPI) in February of 2016.
 
 Found a Bug? Something Unsupported?
 ===================================
```

### Comparing `django-storages-1.9/django_storages.egg-info/PKG-INFO` & `django-storages-1.9.1/django_storages.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-storages
-Version: 1.9
+Version: 1.9.1
 Summary: Support for many storage backends in Django
 Home-page: https://github.com/jschneier/django-storages
 Author: Josh Schneier
 Author-email: josh.schneier@gmail.com
 License: BSD-3-Clause
 Description: .. image:: https://raw.githubusercontent.com/jschneier/django-storages/master/docs/logos/horizontal.png
             :alt: Django-Storages
@@ -66,14 +66,27 @@
         About
         =====
         django-storages is a project to provide a variety of storage backends in a single library.
         
         This library is usually compatible with the currently supported versions of
         Django. Check the Trove classifiers in setup.py to be sure.
         
+        django-storages is backed in part by `Tidelift`_. Check them out for all of your enterprise open source
+        software commerical support needs.
+        
+        .. _Tidelift: https://tidelift.com/subscription/pkg/pypi-django-storages?utm_source=pypi-django-storages&utm_medium=referral&utm_campaign=enterprise&utm_term=repo
+        
+        Security
+        ========
+        
+        To report a security vulnerability, please use the `Tidelift security contact`_. Tidelift will coordinate the
+        fix and disclosure. Please **do not** post a public issue on the tracker.
+        
+        .. _Tidelift security contact: https://tidelift.com/security
+        
         History
         =======
         This repo began as a fork of the original library under the package name of django-storages-redux and
         became the official successor (releasing under django-storages on PyPI) in February of 2016.
         
         Found a Bug? Something Unsupported?
         ===================================
@@ -102,16 +115,27 @@
         #. Bug me until I can merge your pull request. Also, don't forget to add
            yourself to ``AUTHORS``.
         
         
         django-storages CHANGELOG
         =========================
         
+        1.9.1 (2020-02-03)
+        ******************
+        
+        S3
+        --
+        
+        - Fix reading files with ``S3Boto3StorageFile`` (`#831`_, `#833`_)
+        
+        .. _#831: https://github.com/jschneier/django-storages/issues/831
+        .. _#833: https://github.com/jschneier/django-storages/pull/833
+        
         1.9 (2020-02-02)
-        ***********************
+        ****************
         
         General
         -------
         
         - **Breaking**: The long deprecated S3 backend based on ``boto`` has been removed. (`#825`_)
         - Test against and support Python 3.8 (`#810`_)
         
@@ -866,13 +890,13 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
-Provides-Extra: libcloud
-Provides-Extra: google
 Provides-Extra: azure
 Provides-Extra: dropbox
+Provides-Extra: libcloud
 Provides-Extra: boto3
 Provides-Extra: sftp
+Provides-Extra: google
```

### Comparing `django-storages-1.9/django_storages.egg-info/SOURCES.txt` & `django-storages-1.9.1/django_storages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-storages-1.9/docs/Makefile` & `django-storages-1.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-storages-1.9/docs/backends/amazon-S3.rst` & `django-storages-1.9.1/docs/backends/amazon-S3.rst`

 * *Files 21% similar despite different names*

```diff
@@ -244,14 +244,121 @@
     'storage contents'
     >>> file.close()
 
     >>> default_storage.delete('storage_test')
     >>> default_storage.exists('storage_test')
     False
 
+
+Overriding the default Storage class
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+You can override the default Storage class and create your custom storage backend. Below provides some examples and common use cases to help you get started. This section assumes you have your AWS credentials configured, e.g. ``AWS_ACCESS_KEY_ID`` and ``AWS_SECRET_ACCESS_KEY``.
+
+To create a storage class using a specific bucket::
+
+    from storages.backends.s3boto3 import S3Boto3Storage
+
+    class MediaStorage(S3Boto3Storage):
+        bucket_name = 'my-media-bucket'
+
+
+Assume that you store the above class ``MediaStorage`` in a file called ``custom_storage.py`` in the project directory tree like below::
+
+    | (your django project root directory)
+    | ├── manage.py
+    | ├── my_django_app
+    | │   ├── custom_storage.py
+    | │   └── ...
+    | ├── ...
+
+You can now use your custom storage class for default file storage in Django settings like below::
+
+    DEFAULT_FILE_STORAGE = 'my_django_app.custom_storage.MediaStorage'
+
+Or you may want to upload files to the bucket in some view that accepts file upload request::
+
+    import os
+
+    from django.views import View
+    from django.http import JsonResponse
+
+    from django_backend.custom_storages import MediaStorage
+
+    class FileUploadView(View):
+        def post(self, requests, **kwargs):
+            file_obj = requests.FILES.get('file', '')
+
+            # do your validation here e.g. file size/type check
+
+            # organize a path for the file in bucket
+            file_directory_within_bucket = 'user_uplaod_files/{username}'.format(username=requests.user)
+
+            # synthesize a full file path; note that we included the filename
+            file_path_within_bucket = os.path.join(
+                file_directory_within_bucket,
+                file_obj.name
+            )
+
+            media_storage = MediaStorage()
+
+            if not media_storage.exists(file_path_within_bucket): # avoid overwriting existing file
+                media_storage.save(file_path_within_bucket, file_obj)
+                file_url = media_storage.url(file_path_within_bucket)
+
+                return JsonResponse({
+                    'message': 'OK',
+                    'fileUrl': file_url,
+                })
+            else:
+                return JsonResponse({
+                    'message': 'Error: file {filename} already exists at {file_directory} in bucket {bucket_name}'.format(
+                        filename=file_obj.name,
+                        file_directory=file_directory_within_bucket,
+                        bucket_name=media_storage.bucket_name
+                    ),
+                }, status=400)
+
+A side note is that if you have ``AWS_S3_CUSTOM_DOMAIN`` setup in your ``settings.py``, by default the storage class will always use ``AWS_S3_CUSTOM_DOMAIN`` to generate url.
+
+If your ``AWS_S3_CUSTOM_DOMAIN`` is pointing to a different bucket than your custom storage class, the ``.url()`` function will give you the wrong url. In such case, you will have to configure your storage class and explicitly specifiy ``custom_domain`` as below::
+
+    class MediaStorage(S3Boto3Storage):
+        bucket_name = 'my-media-bucket'
+        custom_domain = '{}.s3.amazonaws.com'.format(bucket_name)
+
+You can also decide to config your custom storage class to store files under a specific directory within the bucket::
+
+    class MediaStorage(S3Boto3Storage):
+        bucket_name = 'my-app-bucket'
+        location = 'media' # store files under directory `media/` in bucket `my-app-bucket`
+
+This is especially useful when you want to have multiple storage classes share the same bucket::
+
+    class MediaStorage(S3Boto3Storage):
+        bucket_name = 'my-app-bucket'
+        location = 'media'
+
+    class StaticStorage(S3Boto3Storage):
+        bucket_name = 'my-app-bucket'
+        location = 'static'
+
+So your bucket file can be organized like as below::
+
+    | my-app-bucket
+    | ├── media
+    | │   ├── user_video.mp4
+    | │   ├── user_file.pdf
+    | │   └── ...
+    | ├── static
+    | │   ├── app.js
+    | │   ├── app.css
+    | │   └── ...
+
+
 Model
 -----
 
 An object without a file has limited functionality::
     from django.db import models
 
     class MyModel(models.Model):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-storages-1.9/docs/backends/apache_libcloud.rst` & `django-storages-1.9.1/docs/backends/apache_libcloud.rst`

 * *Files identical despite different names*

### Comparing `django-storages-1.9/docs/backends/azure.rst` & `django-storages-1.9.1/docs/backends/azure.rst`

 * *Files identical despite different names*

### Comparing `django-storages-1.9/docs/backends/dropbox.rst` & `django-storages-1.9.1/docs/backends/dropbox.rst`

 * *Files identical despite different names*

### Comparing `django-storages-1.9/docs/backends/ftp.rst` & `django-storages-1.9.1/docs/backends/ftp.rst`

 * *Files identical despite different names*

### Comparing `django-storages-1.9/docs/backends/gcloud.rst` & `django-storages-1.9.1/docs/backends/gcloud.rst`

 * *Files identical despite different names*

### Comparing `django-storages-1.9/docs/backends/sftp.rst` & `django-storages-1.9.1/docs/backends/sftp.rst`

 * *Files identical despite different names*

### Comparing `django-storages-1.9/docs/conf.py` & `django-storages-1.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-storages-1.9/docs/index.rst` & `django-storages-1.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-storages-1.9/docs/make.bat` & `django-storages-1.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-storages-1.9/setup.py` & `django-storages-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `django-storages-1.9/storages/backends/apache_libcloud.py` & `django-storages-1.9.1/storages/backends/apache_libcloud.py`

 * *Files identical despite different names*

### Comparing `django-storages-1.9/storages/backends/azure_storage.py` & `django-storages-1.9.1/storages/backends/azure_storage.py`

 * *Files identical despite different names*

### Comparing `django-storages-1.9/storages/backends/dropbox.py` & `django-storages-1.9.1/storages/backends/dropbox.py`

 * *Files identical despite different names*

### Comparing `django-storages-1.9/storages/backends/ftp.py` & `django-storages-1.9.1/storages/backends/ftp.py`

 * *Files identical despite different names*

### Comparing `django-storages-1.9/storages/backends/gcloud.py` & `django-storages-1.9.1/storages/backends/gcloud.py`

 * *Files identical despite different names*

### Comparing `django-storages-1.9/storages/backends/s3boto3.py` & `django-storages-1.9.1/storages/backends/s3boto3.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
             parts = [{'ETag': part.e_tag, 'PartNumber': part.part_number}
                      for part in self._multipart.parts.all()]
             self._multipart.complete(
                 MultipartUpload={'Parts': parts})
         else:
             if self._multipart is not None:
                 self._multipart.abort()
-            if self._raw_bytes_written == 0:
+            if 'w' in self._mode and self._raw_bytes_written == 0:
                 self._create_empty_on_close()
         if self._file is not None:
             self._file.close()
             self._file = None
 
 
 @deconstructible
```

### Comparing `django-storages-1.9/storages/backends/sftpstorage.py` & `django-storages-1.9.1/storages/backends/sftpstorage.py`

 * *Files identical despite different names*

### Comparing `django-storages-1.9/storages/utils.py` & `django-storages-1.9.1/storages/utils.py`

 * *Files identical despite different names*

### Comparing `django-storages-1.9/tests/integration/test_azure.py` & `django-storages-1.9.1/tests/integration/test_azure.py`

 * *Files identical despite different names*

### Comparing `django-storages-1.9/tests/test_azure.py` & `django-storages-1.9.1/tests/test_azure.py`

 * *Files identical despite different names*

### Comparing `django-storages-1.9/tests/test_dropbox.py` & `django-storages-1.9.1/tests/test_dropbox.py`

 * *Files identical despite different names*

### Comparing `django-storages-1.9/tests/test_ftp.py` & `django-storages-1.9.1/tests/test_ftp.py`

 * *Files identical despite different names*

### Comparing `django-storages-1.9/tests/test_gcloud.py` & `django-storages-1.9.1/tests/test_gcloud.py`

 * *Files identical despite different names*

### Comparing `django-storages-1.9/tests/test_s3boto3.py` & `django-storages-1.9.1/tests/test_s3boto3.py`

 * *Files identical despite different names*

### Comparing `django-storages-1.9/tests/test_sftp.py` & `django-storages-1.9.1/tests/test_sftp.py`

 * *Files identical despite different names*

### Comparing `django-storages-1.9/tests/test_utils.py` & `django-storages-1.9.1/tests/test_utils.py`

 * *Files identical despite different names*

