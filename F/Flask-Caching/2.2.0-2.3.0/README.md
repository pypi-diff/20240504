# Comparing `tmp/flask_caching-2.2.0.tar.gz` & `tmp/flask_caching-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_caching-2.2.0.tar", last modified: Sat Apr 27 16:05:14 2024, max compression
+gzip compressed data, was "flask_caching-2.3.0.tar", last modified: Sat May  4 13:43:36 2024, max compression
```

## Comparing `flask_caching-2.2.0.tar` & `flask_caching-2.3.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-04-27 16:05:14.224943 flask_caching-2.2.0/
--rw-r--r--   0 gfvante    (501) staff       (20)     3119 2023-01-12 15:56:37.000000 flask_caching-2.2.0/LICENSE
--rw-r--r--   0 gfvante    (501) staff       (20)      260 2023-01-12 15:56:37.000000 flask_caching-2.2.0/MANIFEST.in
--rw-r--r--   0 gfvante    (501) staff       (20)     2207 2024-04-27 16:05:14.224868 flask_caching-2.2.0/PKG-INFO
--rw-r--r--   0 gfvante    (501) staff       (20)     1062 2023-01-12 15:56:37.000000 flask_caching-2.2.0/README.rst
-drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-04-27 16:05:14.219149 flask_caching-2.2.0/docs/
--rw-r--r--   0 gfvante    (501) staff       (20)     7634 2023-01-12 15:56:37.000000 flask_caching-2.2.0/docs/Makefile
-drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-04-27 16:05:14.219339 flask_caching-2.2.0/docs/_static/
--rw-r--r--   0 gfvante    (501) staff       (20)    14917 2023-01-12 15:56:37.000000 flask_caching-2.2.0/docs/_static/flask-cache.png
-drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-04-27 16:05:14.219550 flask_caching-2.2.0/docs/_templates/
--rw-r--r--   0 gfvante    (501) staff       (20)      210 2023-01-12 15:56:37.000000 flask_caching-2.2.0/docs/_templates/sidebarintro.html
--rw-r--r--   0 gfvante    (501) staff       (20)      697 2023-01-12 15:56:37.000000 flask_caching-2.2.0/docs/api.rst
--rw-r--r--   0 gfvante    (501) staff       (20)       28 2023-01-12 15:56:37.000000 flask_caching-2.2.0/docs/changelog.rst
--rw-r--r--   0 gfvante    (501) staff       (20)    10603 2023-10-08 13:54:02.000000 flask_caching-2.2.0/docs/conf.py
--rw-r--r--   0 gfvante    (501) staff       (20)    26370 2024-04-27 15:47:35.000000 flask_caching-2.2.0/docs/index.rst
--rw-r--r--   0 gfvante    (501) staff       (20)       67 2023-01-12 15:56:37.000000 flask_caching-2.2.0/docs/license.rst
--rw-r--r--   0 gfvante    (501) staff       (20)     7465 2023-01-12 15:56:37.000000 flask_caching-2.2.0/docs/make.bat
--rw-r--r--   0 gfvante    (501) staff       (20)     2075 2024-04-27 16:05:14.225510 flask_caching-2.2.0/setup.cfg
--rwxr-xr-x   0 gfvante    (501) staff       (20)      204 2023-10-07 22:16:15.000000 flask_caching-2.2.0/setup.py
-drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-04-27 16:05:14.215939 flask_caching-2.2.0/src/
-drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-04-27 16:05:14.224593 flask_caching-2.2.0/src/Flask_Caching.egg-info/
--rw-r--r--   0 gfvante    (501) staff       (20)     2207 2024-04-27 16:05:14.000000 flask_caching-2.2.0/src/Flask_Caching.egg-info/PKG-INFO
--rw-r--r--   0 gfvante    (501) staff       (20)     1197 2024-04-27 16:05:14.000000 flask_caching-2.2.0/src/Flask_Caching.egg-info/SOURCES.txt
--rw-r--r--   0 gfvante    (501) staff       (20)        1 2024-04-27 16:05:14.000000 flask_caching-2.2.0/src/Flask_Caching.egg-info/dependency_links.txt
--rw-r--r--   0 gfvante    (501) staff       (20)       30 2024-04-27 16:05:14.000000 flask_caching-2.2.0/src/Flask_Caching.egg-info/requires.txt
--rw-r--r--   0 gfvante    (501) staff       (20)       14 2024-04-27 16:05:14.000000 flask_caching-2.2.0/src/Flask_Caching.egg-info/top_level.txt
-drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-04-27 16:05:14.220889 flask_caching-2.2.0/src/flask_caching/
--rw-r--r--   0 gfvante    (501) staff       (20)    41299 2024-04-27 15:58:21.000000 flask_caching-2.2.0/src/flask_caching/__init__.py
-drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-04-27 16:05:14.222134 flask_caching-2.2.0/src/flask_caching/backends/
--rw-r--r--   0 gfvante    (501) staff       (20)     2215 2024-04-27 15:19:34.000000 flask_caching-2.2.0/src/flask_caching/backends/__init__.py
--rw-r--r--   0 gfvante    (501) staff       (20)     1501 2024-04-27 15:19:34.000000 flask_caching-2.2.0/src/flask_caching/backends/base.py
--rw-r--r--   0 gfvante    (501) staff       (20)     2680 2024-04-27 15:19:34.000000 flask_caching-2.2.0/src/flask_caching/backends/filesystemcache.py
--rw-r--r--   0 gfvante    (501) staff       (20)     7634 2024-04-27 15:19:34.000000 flask_caching-2.2.0/src/flask_caching/backends/memcache.py
--rw-r--r--   0 gfvante    (501) staff       (20)      626 2024-04-27 15:19:34.000000 flask_caching-2.2.0/src/flask_caching/backends/nullcache.py
--rw-r--r--   0 gfvante    (501) staff       (20)     9344 2024-04-27 15:47:35.000000 flask_caching-2.2.0/src/flask_caching/backends/rediscache.py
--rw-r--r--   0 gfvante    (501) staff       (20)     2066 2024-04-27 15:19:34.000000 flask_caching-2.2.0/src/flask_caching/backends/simplecache.py
--rw-r--r--   0 gfvante    (501) staff       (20)      455 2024-04-27 15:19:34.000000 flask_caching-2.2.0/src/flask_caching/backends/uwsgicache.py
-drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-04-27 16:05:14.222745 flask_caching-2.2.0/src/flask_caching/contrib/
--rw-r--r--   0 gfvante    (501) staff       (20)        0 2023-01-12 15:56:37.000000 flask_caching-2.2.0/src/flask_caching/contrib/__init__.py
--rw-r--r--   0 gfvante    (501) staff       (20)     7527 2023-01-12 15:56:37.000000 flask_caching-2.2.0/src/flask_caching/contrib/googlecloudstoragecache.py
--rw-r--r--   0 gfvante    (501) staff       (20)     2296 2024-04-27 15:19:34.000000 flask_caching-2.2.0/src/flask_caching/contrib/uwsgicache.py
--rw-r--r--   0 gfvante    (501) staff       (20)     2920 2024-04-27 15:19:34.000000 flask_caching-2.2.0/src/flask_caching/jinja2ext.py
--rw-r--r--   0 gfvante    (501) staff       (20)        0 2023-01-12 15:56:37.000000 flask_caching-2.2.0/src/flask_caching/py.typed
--rw-r--r--   0 gfvante    (501) staff       (20)     3238 2023-10-07 22:16:15.000000 flask_caching-2.2.0/src/flask_caching/utils.py
-drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-04-27 16:05:14.224396 flask_caching-2.2.0/tests/
--rw-r--r--   0 gfvante    (501) staff       (20)     2298 2023-01-12 15:56:37.000000 flask_caching-2.2.0/tests/conftest.py
--rw-r--r--   0 gfvante    (501) staff       (20)     7894 2024-04-27 15:47:35.000000 flask_caching-2.2.0/tests/test_backend_cache.py
--rw-r--r--   0 gfvante    (501) staff       (20)     3840 2023-01-12 15:56:37.000000 flask_caching-2.2.0/tests/test_basic_app.py
--rw-r--r--   0 gfvante    (501) staff       (20)     9536 2023-01-12 15:56:37.000000 flask_caching-2.2.0/tests/test_cache.py
--rw-r--r--   0 gfvante    (501) staff       (20)     1329 2023-01-12 15:56:37.000000 flask_caching-2.2.0/tests/test_init.py
--rw-r--r--   0 gfvante    (501) staff       (20)    23087 2024-04-27 15:47:35.000000 flask_caching-2.2.0/tests/test_memoize.py
--rw-r--r--   0 gfvante    (501) staff       (20)      242 2023-01-12 15:56:37.000000 flask_caching-2.2.0/tests/test_template.html
--rw-r--r--   0 gfvante    (501) staff       (20)     1940 2023-01-12 15:56:37.000000 flask_caching-2.2.0/tests/test_templates.py
--rw-r--r--   0 gfvante    (501) staff       (20)    16728 2024-04-27 15:19:34.000000 flask_caching-2.2.0/tests/test_view.py
--rw-r--r--   0 gfvante    (501) staff       (20)      555 2024-04-27 15:19:34.000000 flask_caching-2.2.0/tox.ini
+drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-05-04 13:43:36.322308 flask_caching-2.3.0/
+-rw-r--r--   0 gfvante    (501) staff       (20)     3119 2023-01-12 15:56:37.000000 flask_caching-2.3.0/LICENSE
+-rw-r--r--   0 gfvante    (501) staff       (20)      260 2023-01-12 15:56:37.000000 flask_caching-2.3.0/MANIFEST.in
+-rw-r--r--   0 gfvante    (501) staff       (20)     2207 2024-05-04 13:43:36.322244 flask_caching-2.3.0/PKG-INFO
+-rw-r--r--   0 gfvante    (501) staff       (20)     1062 2023-01-12 15:56:37.000000 flask_caching-2.3.0/README.rst
+drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-05-04 13:43:36.317394 flask_caching-2.3.0/docs/
+-rw-r--r--   0 gfvante    (501) staff       (20)     7634 2023-01-12 15:56:37.000000 flask_caching-2.3.0/docs/Makefile
+drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-05-04 13:43:36.317587 flask_caching-2.3.0/docs/_static/
+-rw-r--r--   0 gfvante    (501) staff       (20)    14917 2023-01-12 15:56:37.000000 flask_caching-2.3.0/docs/_static/flask-cache.png
+drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-05-04 13:43:36.317809 flask_caching-2.3.0/docs/_templates/
+-rw-r--r--   0 gfvante    (501) staff       (20)      210 2023-01-12 15:56:37.000000 flask_caching-2.3.0/docs/_templates/sidebarintro.html
+-rw-r--r--   0 gfvante    (501) staff       (20)      697 2023-01-12 15:56:37.000000 flask_caching-2.3.0/docs/api.rst
+-rw-r--r--   0 gfvante    (501) staff       (20)       28 2023-01-12 15:56:37.000000 flask_caching-2.3.0/docs/changelog.rst
+-rw-r--r--   0 gfvante    (501) staff       (20)    10603 2023-10-08 13:54:02.000000 flask_caching-2.3.0/docs/conf.py
+-rw-r--r--   0 gfvante    (501) staff       (20)    26370 2024-05-04 13:23:04.000000 flask_caching-2.3.0/docs/index.rst
+-rw-r--r--   0 gfvante    (501) staff       (20)       67 2023-01-12 15:56:37.000000 flask_caching-2.3.0/docs/license.rst
+-rw-r--r--   0 gfvante    (501) staff       (20)     7465 2023-01-12 15:56:37.000000 flask_caching-2.3.0/docs/make.bat
+-rw-r--r--   0 gfvante    (501) staff       (20)     2075 2024-05-04 13:43:36.322732 flask_caching-2.3.0/setup.cfg
+-rwxr-xr-x   0 gfvante    (501) staff       (20)      204 2023-10-07 22:16:15.000000 flask_caching-2.3.0/setup.py
+drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-05-04 13:43:36.314577 flask_caching-2.3.0/src/
+drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-05-04 13:43:36.322021 flask_caching-2.3.0/src/Flask_Caching.egg-info/
+-rw-r--r--   0 gfvante    (501) staff       (20)     2207 2024-05-04 13:43:36.000000 flask_caching-2.3.0/src/Flask_Caching.egg-info/PKG-INFO
+-rw-r--r--   0 gfvante    (501) staff       (20)     1197 2024-05-04 13:43:36.000000 flask_caching-2.3.0/src/Flask_Caching.egg-info/SOURCES.txt
+-rw-r--r--   0 gfvante    (501) staff       (20)        1 2024-05-04 13:43:36.000000 flask_caching-2.3.0/src/Flask_Caching.egg-info/dependency_links.txt
+-rw-r--r--   0 gfvante    (501) staff       (20)       30 2024-05-04 13:43:36.000000 flask_caching-2.3.0/src/Flask_Caching.egg-info/requires.txt
+-rw-r--r--   0 gfvante    (501) staff       (20)       14 2024-05-04 13:43:36.000000 flask_caching-2.3.0/src/Flask_Caching.egg-info/top_level.txt
+drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-05-04 13:43:36.318971 flask_caching-2.3.0/src/flask_caching/
+-rw-r--r--   0 gfvante    (501) staff       (20)    41968 2024-05-04 13:38:03.000000 flask_caching-2.3.0/src/flask_caching/__init__.py
+drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-05-04 13:43:36.320113 flask_caching-2.3.0/src/flask_caching/backends/
+-rw-r--r--   0 gfvante    (501) staff       (20)     2215 2024-05-04 13:23:04.000000 flask_caching-2.3.0/src/flask_caching/backends/__init__.py
+-rw-r--r--   0 gfvante    (501) staff       (20)     1501 2024-05-04 13:23:04.000000 flask_caching-2.3.0/src/flask_caching/backends/base.py
+-rw-r--r--   0 gfvante    (501) staff       (20)     2680 2024-05-04 13:23:04.000000 flask_caching-2.3.0/src/flask_caching/backends/filesystemcache.py
+-rw-r--r--   0 gfvante    (501) staff       (20)     7634 2024-05-04 13:23:04.000000 flask_caching-2.3.0/src/flask_caching/backends/memcache.py
+-rw-r--r--   0 gfvante    (501) staff       (20)      626 2024-05-04 13:23:04.000000 flask_caching-2.3.0/src/flask_caching/backends/nullcache.py
+-rw-r--r--   0 gfvante    (501) staff       (20)     9344 2024-05-04 13:23:04.000000 flask_caching-2.3.0/src/flask_caching/backends/rediscache.py
+-rw-r--r--   0 gfvante    (501) staff       (20)     2066 2024-05-04 13:23:04.000000 flask_caching-2.3.0/src/flask_caching/backends/simplecache.py
+-rw-r--r--   0 gfvante    (501) staff       (20)      455 2024-05-04 13:23:04.000000 flask_caching-2.3.0/src/flask_caching/backends/uwsgicache.py
+drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-05-04 13:43:36.320485 flask_caching-2.3.0/src/flask_caching/contrib/
+-rw-r--r--   0 gfvante    (501) staff       (20)        0 2023-01-12 15:56:37.000000 flask_caching-2.3.0/src/flask_caching/contrib/__init__.py
+-rw-r--r--   0 gfvante    (501) staff       (20)     7527 2023-01-12 15:56:37.000000 flask_caching-2.3.0/src/flask_caching/contrib/googlecloudstoragecache.py
+-rw-r--r--   0 gfvante    (501) staff       (20)     2296 2024-05-04 13:23:04.000000 flask_caching-2.3.0/src/flask_caching/contrib/uwsgicache.py
+-rw-r--r--   0 gfvante    (501) staff       (20)     2920 2024-05-04 13:23:04.000000 flask_caching-2.3.0/src/flask_caching/jinja2ext.py
+-rw-r--r--   0 gfvante    (501) staff       (20)        0 2023-01-12 15:56:37.000000 flask_caching-2.3.0/src/flask_caching/py.typed
+-rw-r--r--   0 gfvante    (501) staff       (20)     3238 2023-10-07 22:16:15.000000 flask_caching-2.3.0/src/flask_caching/utils.py
+drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-05-04 13:43:36.321654 flask_caching-2.3.0/tests/
+-rw-r--r--   0 gfvante    (501) staff       (20)     2298 2023-01-12 15:56:37.000000 flask_caching-2.3.0/tests/conftest.py
+-rw-r--r--   0 gfvante    (501) staff       (20)     7894 2024-05-04 13:23:04.000000 flask_caching-2.3.0/tests/test_backend_cache.py
+-rw-r--r--   0 gfvante    (501) staff       (20)     3840 2023-01-12 15:56:37.000000 flask_caching-2.3.0/tests/test_basic_app.py
+-rw-r--r--   0 gfvante    (501) staff       (20)     9536 2023-01-12 15:56:37.000000 flask_caching-2.3.0/tests/test_cache.py
+-rw-r--r--   0 gfvante    (501) staff       (20)     1329 2023-01-12 15:56:37.000000 flask_caching-2.3.0/tests/test_init.py
+-rw-r--r--   0 gfvante    (501) staff       (20)    23087 2024-05-04 13:23:04.000000 flask_caching-2.3.0/tests/test_memoize.py
+-rw-r--r--   0 gfvante    (501) staff       (20)      242 2023-01-12 15:56:37.000000 flask_caching-2.3.0/tests/test_template.html
+-rw-r--r--   0 gfvante    (501) staff       (20)     1940 2023-01-12 15:56:37.000000 flask_caching-2.3.0/tests/test_templates.py
+-rw-r--r--   0 gfvante    (501) staff       (20)    17149 2024-05-04 13:36:03.000000 flask_caching-2.3.0/tests/test_view.py
+-rw-r--r--   0 gfvante    (501) staff       (20)      555 2024-05-04 13:23:04.000000 flask_caching-2.3.0/tox.ini
```

### Comparing `flask_caching-2.2.0/LICENSE` & `flask_caching-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_caching-2.2.0/PKG-INFO` & `flask_caching-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Caching
-Version: 2.2.0
+Version: 2.3.0
 Summary: Adds caching support to Flask applications.
 Home-page: https://github.com/pallets-eco/flask-caching
 Author: Peter Justin
 Author-email: peter.justin@outlook.com
 Maintainer: Pallets
 Maintainer-email: contact@palletsprojects.com
 License: BSD
```

### Comparing `flask_caching-2.2.0/README.rst` & `flask_caching-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `flask_caching-2.2.0/docs/Makefile` & `flask_caching-2.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `flask_caching-2.2.0/docs/_static/flask-cache.png` & `flask_caching-2.3.0/docs/_static/flask-cache.png`

 * *Files identical despite different names*

### Comparing `flask_caching-2.2.0/docs/api.rst` & `flask_caching-2.3.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `flask_caching-2.2.0/docs/conf.py` & `flask_caching-2.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `flask_caching-2.2.0/docs/index.rst` & `flask_caching-2.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `flask_caching-2.2.0/docs/make.bat` & `flask_caching-2.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `flask_caching-2.2.0/setup.cfg` & `flask_caching-2.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `flask_caching-2.2.0/src/Flask_Caching.egg-info/PKG-INFO` & `flask_caching-2.3.0/src/Flask_Caching.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Caching
-Version: 2.2.0
+Version: 2.3.0
 Summary: Adds caching support to Flask applications.
 Home-page: https://github.com/pallets-eco/flask-caching
 Author: Peter Justin
 Author-email: peter.justin@outlook.com
 Maintainer: Pallets
 Maintainer-email: contact@palletsprojects.com
 License: BSD
```

### Comparing `flask_caching-2.2.0/src/Flask_Caching.egg-info/SOURCES.txt` & `flask_caching-2.3.0/src/Flask_Caching.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flask_caching-2.2.0/src/flask_caching/__init__.py` & `flask_caching-2.3.0/src/flask_caching/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from flask_caching.utils import function_namespace
 from flask_caching.utils import get_arg_default
 from flask_caching.utils import get_arg_names
 from flask_caching.utils import get_id
 from flask_caching.utils import make_template_fragment_key  # noqa: F401
 from flask_caching.utils import wants_args
 
-__version__ = "2.2.0"
+__version__ = "2.3.0"
 
 logger = logging.getLogger(__name__)
 
 SUPPORTED_HASH_FUNCTIONS = [
     hashlib.sha1,
     hashlib.sha224,
     hashlib.sha256,
@@ -247,14 +247,15 @@
         forced_update: Optional[Callable] = None,
         response_filter: Optional[Callable] = None,
         query_string: bool = False,
         hash_method: Callable = hashlib.md5,
         cache_none: bool = False,
         make_cache_key: Optional[Callable] = None,
         source_check: Optional[bool] = None,
+        response_hit_indication: Optional[bool] = False,
     ) -> Callable:
         """Decorator. Use this to cache a function. By default the cache key
         is `view/request.path`. You are able to use this decorator with any
         function by changing the `key_prefix`. If the token `%s` is located
         within the `key_prefix` then it will replace that with `request.path`
 
         Example::
@@ -347,14 +348,18 @@
                              If True, include the function's source code in the
                              hash to avoid using cached values when the source
                              code has changed and the input values remain the
                              same. This ensures that the cache_key will be
                              formed with the function's source code hash in
                              addition to other parameters that may be included
                              in the formation of the key.
+
+        :param response_hit_indication: Default False.
+                             If True, it will add to response header field 'hit_cache'
+                             if used cache.
         """
 
         def decorator(f):
             @functools.wraps(f)
             def decorated_function(*args, **kwargs):
                 #: Bypass the cache entirely.
                 if self._bypass_cache(unless, f, *args, **kwargs):
@@ -402,14 +407,24 @@
                             else:
                                 found = self.cache.has(cache_key)
                 except Exception:
                     if self.app.debug:
                         raise
                     logger.exception("Exception possibly due to cache backend.")
                     return self._call_fn(f, *args, **kwargs)
+                if found and self.app.debug:
+                    logger.info(f"Cache used for key: {cache_key}")
+                if response_hit_indication:
+
+                    def apply_caching(response):
+                        if found:
+                            response.headers["hit_cache"] = found
+                        return response
+
+                    self.app.after_request_funcs[None].append(apply_caching)
 
                 if not found:
                     rv = self._call_fn(f, *args, **kwargs)
                     if inspect.isgenerator(rv):
                         rv = [val for val in rv]
 
                     if response_filter is None or response_filter(rv):
```

### Comparing `flask_caching-2.2.0/src/flask_caching/backends/__init__.py` & `flask_caching-2.3.0/src/flask_caching/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_caching-2.2.0/src/flask_caching/backends/base.py` & `flask_caching-2.3.0/src/flask_caching/backends/base.py`

 * *Files identical despite different names*

### Comparing `flask_caching-2.2.0/src/flask_caching/backends/filesystemcache.py` & `flask_caching-2.3.0/src/flask_caching/backends/filesystemcache.py`

 * *Files identical despite different names*

### Comparing `flask_caching-2.2.0/src/flask_caching/backends/memcache.py` & `flask_caching-2.3.0/src/flask_caching/backends/memcache.py`

 * *Files identical despite different names*

### Comparing `flask_caching-2.2.0/src/flask_caching/backends/nullcache.py` & `flask_caching-2.3.0/src/flask_caching/backends/nullcache.py`

 * *Files identical despite different names*

### Comparing `flask_caching-2.2.0/src/flask_caching/backends/rediscache.py` & `flask_caching-2.3.0/src/flask_caching/backends/rediscache.py`

 * *Files identical despite different names*

### Comparing `flask_caching-2.2.0/src/flask_caching/backends/simplecache.py` & `flask_caching-2.3.0/src/flask_caching/backends/simplecache.py`

 * *Files identical despite different names*

### Comparing `flask_caching-2.2.0/src/flask_caching/contrib/googlecloudstoragecache.py` & `flask_caching-2.3.0/src/flask_caching/contrib/googlecloudstoragecache.py`

 * *Files identical despite different names*

### Comparing `flask_caching-2.2.0/src/flask_caching/contrib/uwsgicache.py` & `flask_caching-2.3.0/src/flask_caching/contrib/uwsgicache.py`

 * *Files identical despite different names*

### Comparing `flask_caching-2.2.0/src/flask_caching/jinja2ext.py` & `flask_caching-2.3.0/src/flask_caching/jinja2ext.py`

 * *Files identical despite different names*

### Comparing `flask_caching-2.2.0/src/flask_caching/utils.py` & `flask_caching-2.3.0/src/flask_caching/utils.py`

 * *Files identical despite different names*

### Comparing `flask_caching-2.2.0/tests/conftest.py` & `flask_caching-2.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flask_caching-2.2.0/tests/test_backend_cache.py` & `flask_caching-2.3.0/tests/test_backend_cache.py`

 * *Files identical despite different names*

### Comparing `flask_caching-2.2.0/tests/test_basic_app.py` & `flask_caching-2.3.0/tests/test_basic_app.py`

 * *Files identical despite different names*

### Comparing `flask_caching-2.2.0/tests/test_cache.py` & `flask_caching-2.3.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `flask_caching-2.2.0/tests/test_init.py` & `flask_caching-2.3.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `flask_caching-2.2.0/tests/test_memoize.py` & `flask_caching-2.3.0/tests/test_memoize.py`

 * *Files identical despite different names*

### Comparing `flask_caching-2.2.0/tests/test_templates.py` & `flask_caching-2.3.0/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `flask_caching-2.2.0/tests/test_view.py` & `flask_caching-2.3.0/tests/test_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -569,7 +569,21 @@
     # Make the second query...
     third_response = tc.get("/works?mock=true&offset=20&limit=15")
     third_time = third_response.get_data(as_text=True)
 
     # Now make sure the time for the first and third responses are the same
     # i.e. cached is used since cache will not check for source changes!
     assert third_time == first_time
+
+
+def test_hit_cache(app, cache):
+    @app.route("/")
+    @cache.cached(10, response_hit_indication=True)
+    def cached_view():
+        # This should override the timeout to be 2 seconds
+        return {"data": "data"}
+
+    tc = app.test_client()
+
+    assert tc.get("/").headers.get("hit_cache") is None
+    assert tc.get("/").headers.get("hit_cache") == "True"
+    assert tc.get("/").headers.get("hit_cache") == "True"
```

### Comparing `flask_caching-2.2.0/tox.ini` & `flask_caching-2.3.0/tox.ini`

 * *Files identical despite different names*

