# Comparing `tmp/Flask-Cors-4.0.0a0.tar.gz` & `tmp/flask_cors-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-Cors-4.0.0a0.tar", last modified: Mon Jun 26 01:19:10 2023, max compression
+gzip compressed data, was "flask_cors-4.0.1.tar", last modified: Sat May  4 19:49:36 2024, max compression
```

## Comparing `Flask-Cors-4.0.0a0.tar` & `flask_cors-4.0.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:19:10.163316 Flask-Cors-4.0.0a0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:19:10.163316 Flask-Cors-4.0.0a0/Flask_Cors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-26 01:19:10.000000 Flask-Cors-4.0.0a0/Flask_Cors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-26 01:19:10.000000 Flask-Cors-4.0.0a0/Flask_Cors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 01:19:10.000000 Flask-Cors-4.0.0a0/Flask_Cors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 01:19:10.000000 Flask-Cors-4.0.0a0/Flask_Cors.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 01:19:10.000000 Flask-Cors-4.0.0a0/Flask_Cors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 01:19:10.000000 Flask-Cors-4.0.0a0/Flask_Cors.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-26 01:19:10.167316 Flask-Cors-4.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:19:10.163316 Flask-Cors-4.0.0a0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:19:10.163316 Flask-Cors-4.0.0a0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/examples/app_based_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/examples/blueprints_based_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/examples/view_based_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:19:10.163316 Flask-Cors-4.0.0a0/flask_cors/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/flask_cors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14063 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/flask_cors/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/flask_cors/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/flask_cors/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/flask_cors/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-26 01:19:10.167316 Flask-Cors-4.0.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:19:10.163316 Flask-Cors-4.0.0a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/base_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:19:10.163316 Flask-Cors-4.0.0a0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/core/helper_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/core/test_override_headers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:19:10.163316 Flask-Cors-4.0.0a0/tests/decorator/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/decorator/test_allow_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/decorator/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/decorator/test_duplicate_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/decorator/test_exception_interception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/decorator/test_expose_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/decorator/test_max_age.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/decorator/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/decorator/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/decorator/test_origins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/decorator/test_vary_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/decorator/test_w3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:19:10.163316 Flask-Cors-4.0.0a0/tests/extension/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13982 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/extension/test_app_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:49:36.194678 flask_cors-4.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:49:36.194678 flask_cors-4.0.1/Flask_Cors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-04 19:49:36.000000 flask_cors-4.0.1/Flask_Cors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-04 19:49:36.000000 flask_cors-4.0.1/Flask_Cors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 19:49:36.000000 flask_cors-4.0.1/Flask_Cors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 19:49:36.000000 flask_cors-4.0.1/Flask_Cors.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 19:49:36.000000 flask_cors-4.0.1/Flask_Cors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 19:49:36.000000 flask_cors-4.0.1/Flask_Cors.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-04 19:49:31.000000 flask_cors-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-04 19:49:31.000000 flask_cors-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-04 19:49:36.194678 flask_cors-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-04 19:49:31.000000 flask_cors-4.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:49:36.190678 flask_cors-4.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-05-04 19:49:31.000000 flask_cors-4.0.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-04 19:49:31.000000 flask_cors-4.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-05-04 19:49:31.000000 flask_cors-4.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-05-04 19:49:31.000000 flask_cors-4.0.1/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-04 19:49:31.000000 flask_cors-4.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-04 19:49:31.000000 flask_cors-4.0.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:49:36.190678 flask_cors-4.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-04 19:49:31.000000 flask_cors-4.0.1/examples/app_based_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-04 19:49:31.000000 flask_cors-4.0.1/examples/blueprints_based_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-04 19:49:31.000000 flask_cors-4.0.1/examples/view_based_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:49:36.190678 flask_cors-4.0.1/flask_cors/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-04 19:49:31.000000 flask_cors-4.0.1/flask_cors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14063 2024-05-04 19:49:31.000000 flask_cors-4.0.1/flask_cors/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-04 19:49:31.000000 flask_cors-4.0.1/flask_cors/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7857 2024-05-04 19:49:31.000000 flask_cors-4.0.1/flask_cors/extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-04 19:49:31.000000 flask_cors-4.0.1/flask_cors/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 19:49:31.000000 flask_cors-4.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-04 19:49:36.194678 flask_cors-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-04 19:49:31.000000 flask_cors-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:49:36.190678 flask_cors-4.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-04 19:49:31.000000 flask_cors-4.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-04 19:49:31.000000 flask_cors-4.0.1/tests/base_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:49:36.190678 flask_cors-4.0.1/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-04 19:49:31.000000 flask_cors-4.0.1/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-04 19:49:31.000000 flask_cors-4.0.1/tests/core/helper_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-04 19:49:31.000000 flask_cors-4.0.1/tests/core/test_override_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:49:36.194678 flask_cors-4.0.1/tests/decorator/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-04 19:49:31.000000 flask_cors-4.0.1/tests/decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-04 19:49:31.000000 flask_cors-4.0.1/tests/decorator/test_allow_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-04 19:49:31.000000 flask_cors-4.0.1/tests/decorator/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-04 19:49:31.000000 flask_cors-4.0.1/tests/decorator/test_duplicate_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7911 2024-05-04 19:49:31.000000 flask_cors-4.0.1/tests/decorator/test_exception_interception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-04 19:49:31.000000 flask_cors-4.0.1/tests/decorator/test_expose_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-04 19:49:31.000000 flask_cors-4.0.1/tests/decorator/test_max_age.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-04 19:49:31.000000 flask_cors-4.0.1/tests/decorator/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-04 19:49:31.000000 flask_cors-4.0.1/tests/decorator/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8069 2024-05-04 19:49:31.000000 flask_cors-4.0.1/tests/decorator/test_origins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-04 19:49:31.000000 flask_cors-4.0.1/tests/decorator/test_vary_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-04 19:49:31.000000 flask_cors-4.0.1/tests/decorator/test_w3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 19:49:36.194678 flask_cors-4.0.1/tests/extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-04 19:49:31.000000 flask_cors-4.0.1/tests/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13982 2024-05-04 19:49:31.000000 flask_cors-4.0.1/tests/extension/test_app_extension.py
```

### Comparing `Flask-Cors-4.0.0a0/Flask_Cors.egg-info/PKG-INFO` & `flask_cors-4.0.1/Flask_Cors.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Cors
-Version: 4.0.0a0
+Version: 4.0.1
 Summary: A Flask extension adding a decorator for CORS support
 Home-page: https://github.com/corydolphin/flask-cors
 Author: Cory Dolphin
 Author-email: corydolphin@gmail.com
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
@@ -12,54 +12,56 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
+Requires-Dist: Flask>=0.9
 
 Flask-CORS
 ==========
 
 |Build Status| |Latest Version| |Supported Python versions|
 |License|
 
 A Flask extension for handling Cross Origin Resource Sharing (CORS), making cross-origin AJAX possible.
 
-This package has a simple philosophy: when you want to enable CORS, you wish to enable it for all use cases on a domain. 
-This means no mucking around with different allowed headers, methods, etc. 
+This package has a simple philosophy: when you want to enable CORS, you wish to enable it for all use cases on a domain.
+This means no mucking around with different allowed headers, methods, etc.
 
-By default, submission of cookies across domains is disabled due to the security implications. 
+By default, submission of cookies across domains is disabled due to the security implications.
 Please see the documentation for how to enable credential'ed requests, and please make sure you add some sort of `CSRF <http://en.wikipedia.org/wiki/Cross-site_request_forgery>`__ protection before doing so!
 
 Installation
 ------------
 
 Install the extension with using pip, or easy\_install.
 
 .. code:: bash
 
     $ pip install -U flask-cors
 
 Usage
 -----
 
-This package exposes a Flask extension which by default enables CORS support on all routes, for all origins and methods. 
-It allows parameterization of all CORS headers on a per-resource level. 
+This package exposes a Flask extension which by default enables CORS support on all routes, for all origins and methods.
+It allows parameterization of all CORS headers on a per-resource level.
 The package also contains a decorator, for those who prefer this approach.
 
 Simple Usage
 ~~~~~~~~~~~~
 
-In the simplest case, initialize the Flask-Cors extension with default arguments in order to allow CORS for all domains on all routes. 
+In the simplest case, initialize the Flask-Cors extension with default arguments in order to allow CORS for all domains on all routes.
 See the full list of options in the `documentation <https://flask-cors.corydolphin.com/en/latest/api.html#extension>`__.
 
 .. code:: python
 
 
     from flask import Flask
     from flask_cors import CORS
@@ -70,31 +72,31 @@
     @app.route("/")
     def helloWorld():
       return "Hello, cross-origin-world!"
 
 Resource specific CORS
 ^^^^^^^^^^^^^^^^^^^^^^
 
-Alternatively, you can specify CORS options on a resource and origin level of granularity by passing a dictionary as the `resources` option, mapping paths to a set of options. 
+Alternatively, you can specify CORS options on a resource and origin level of granularity by passing a dictionary as the `resources` option, mapping paths to a set of options.
 See the full list of options in the `documentation <https://flask-cors.corydolphin.com/en/latest/api.html#extension>`__.
 
 .. code:: python
 
     app = Flask(__name__)
     cors = CORS(app, resources={r"/api/*": {"origins": "*"}})
 
     @app.route("/api/v1/users")
     def list_users():
       return "user example"
 
 Route specific CORS via decorator
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-This extension also exposes a simple decorator to decorate flask routes with. 
-Simply add ``@cross_origin()`` below a call to Flask's ``@app.route(..)`` to allow CORS on a given route. 
+This extension also exposes a simple decorator to decorate flask routes with.
+Simply add ``@cross_origin()`` below a call to Flask's ``@app.route(..)`` to allow CORS on a given route.
 See the full list of options in the `decorator documentation <https://flask-cors.corydolphin.com/en/latest/api.html#decorator>`__.
 
 .. code:: python
 
     @app.route("/")
     @cross_origin()
     def helloWorld():
@@ -114,33 +116,33 @@
 
     logging.getLogger('flask_cors').level = logging.DEBUG
 
 
 Tests
 -----
 
-A simple set of tests is included in ``test/``. 
+A simple set of tests is included in ``test/``.
 To run, install nose, and simply invoke ``nosetests`` or ``python setup.py test`` to exercise the tests.
 
 If nosetests does not work for you, due to it no longer working with newer python versions.
 You can use pytest to run the tests instead.
 
 Contributing
 ------------
 
-Questions, comments or improvements? 
-Please create an issue on `Github <https://github.com/corydolphin/flask-cors>`__, tweet at `@corydolphin <https://twitter.com/corydolphin>`__ or send me an email. 
+Questions, comments or improvements?
+Please create an issue on `Github <https://github.com/corydolphin/flask-cors>`__, tweet at `@corydolphin <https://twitter.com/corydolphin>`__ or send me an email.
 I do my best to include every contribution proposed in any way that I can.
 
 Credits
 -------
 
 This Flask extension is based upon the `Decorator for the HTTP Access Control <https://web.archive.org/web/20190128010149/http://flask.pocoo.org/snippets/56/>`__ written by Armin Ronacher.
 
-.. |Build Status| image:: https://api.travis-ci.org/corydolphin/flask-cors.svg?branch=master
+.. |Build Status| image:: https://github.com/corydolphin/flask-cors/actions/workflows/unittests.yaml/badge.svg
    :target: https://travis-ci.org/corydolphin/flask-cors
 .. |Latest Version| image:: https://img.shields.io/pypi/v/Flask-Cors.svg
    :target: https://pypi.python.org/pypi/Flask-Cors/
 .. |Supported Python versions| image:: https://img.shields.io/pypi/pyversions/Flask-Cors.svg
    :target: https://img.shields.io/pypi/pyversions/Flask-Cors.svg
 .. |License| image:: http://img.shields.io/:license-mit-blue.svg
    :target: https://pypi.python.org/pypi/Flask-Cors/
```

### Comparing `Flask-Cors-4.0.0a0/Flask_Cors.egg-info/SOURCES.txt` & `flask_cors-4.0.1/Flask_Cors.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0a0/LICENSE` & `flask_cors-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0a0/PKG-INFO` & `flask_cors-4.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Cors
-Version: 4.0.0a0
+Version: 4.0.1
 Summary: A Flask extension adding a decorator for CORS support
 Home-page: https://github.com/corydolphin/flask-cors
 Author: Cory Dolphin
 Author-email: corydolphin@gmail.com
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
@@ -12,54 +12,56 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
+Requires-Dist: Flask>=0.9
 
 Flask-CORS
 ==========
 
 |Build Status| |Latest Version| |Supported Python versions|
 |License|
 
 A Flask extension for handling Cross Origin Resource Sharing (CORS), making cross-origin AJAX possible.
 
-This package has a simple philosophy: when you want to enable CORS, you wish to enable it for all use cases on a domain. 
-This means no mucking around with different allowed headers, methods, etc. 
+This package has a simple philosophy: when you want to enable CORS, you wish to enable it for all use cases on a domain.
+This means no mucking around with different allowed headers, methods, etc.
 
-By default, submission of cookies across domains is disabled due to the security implications. 
+By default, submission of cookies across domains is disabled due to the security implications.
 Please see the documentation for how to enable credential'ed requests, and please make sure you add some sort of `CSRF <http://en.wikipedia.org/wiki/Cross-site_request_forgery>`__ protection before doing so!
 
 Installation
 ------------
 
 Install the extension with using pip, or easy\_install.
 
 .. code:: bash
 
     $ pip install -U flask-cors
 
 Usage
 -----
 
-This package exposes a Flask extension which by default enables CORS support on all routes, for all origins and methods. 
-It allows parameterization of all CORS headers on a per-resource level. 
+This package exposes a Flask extension which by default enables CORS support on all routes, for all origins and methods.
+It allows parameterization of all CORS headers on a per-resource level.
 The package also contains a decorator, for those who prefer this approach.
 
 Simple Usage
 ~~~~~~~~~~~~
 
-In the simplest case, initialize the Flask-Cors extension with default arguments in order to allow CORS for all domains on all routes. 
+In the simplest case, initialize the Flask-Cors extension with default arguments in order to allow CORS for all domains on all routes.
 See the full list of options in the `documentation <https://flask-cors.corydolphin.com/en/latest/api.html#extension>`__.
 
 .. code:: python
 
 
     from flask import Flask
     from flask_cors import CORS
@@ -70,31 +72,31 @@
     @app.route("/")
     def helloWorld():
       return "Hello, cross-origin-world!"
 
 Resource specific CORS
 ^^^^^^^^^^^^^^^^^^^^^^
 
-Alternatively, you can specify CORS options on a resource and origin level of granularity by passing a dictionary as the `resources` option, mapping paths to a set of options. 
+Alternatively, you can specify CORS options on a resource and origin level of granularity by passing a dictionary as the `resources` option, mapping paths to a set of options.
 See the full list of options in the `documentation <https://flask-cors.corydolphin.com/en/latest/api.html#extension>`__.
 
 .. code:: python
 
     app = Flask(__name__)
     cors = CORS(app, resources={r"/api/*": {"origins": "*"}})
 
     @app.route("/api/v1/users")
     def list_users():
       return "user example"
 
 Route specific CORS via decorator
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-This extension also exposes a simple decorator to decorate flask routes with. 
-Simply add ``@cross_origin()`` below a call to Flask's ``@app.route(..)`` to allow CORS on a given route. 
+This extension also exposes a simple decorator to decorate flask routes with.
+Simply add ``@cross_origin()`` below a call to Flask's ``@app.route(..)`` to allow CORS on a given route.
 See the full list of options in the `decorator documentation <https://flask-cors.corydolphin.com/en/latest/api.html#decorator>`__.
 
 .. code:: python
 
     @app.route("/")
     @cross_origin()
     def helloWorld():
@@ -114,33 +116,33 @@
 
     logging.getLogger('flask_cors').level = logging.DEBUG
 
 
 Tests
 -----
 
-A simple set of tests is included in ``test/``. 
+A simple set of tests is included in ``test/``.
 To run, install nose, and simply invoke ``nosetests`` or ``python setup.py test`` to exercise the tests.
 
 If nosetests does not work for you, due to it no longer working with newer python versions.
 You can use pytest to run the tests instead.
 
 Contributing
 ------------
 
-Questions, comments or improvements? 
-Please create an issue on `Github <https://github.com/corydolphin/flask-cors>`__, tweet at `@corydolphin <https://twitter.com/corydolphin>`__ or send me an email. 
+Questions, comments or improvements?
+Please create an issue on `Github <https://github.com/corydolphin/flask-cors>`__, tweet at `@corydolphin <https://twitter.com/corydolphin>`__ or send me an email.
 I do my best to include every contribution proposed in any way that I can.
 
 Credits
 -------
 
 This Flask extension is based upon the `Decorator for the HTTP Access Control <https://web.archive.org/web/20190128010149/http://flask.pocoo.org/snippets/56/>`__ written by Armin Ronacher.
 
-.. |Build Status| image:: https://api.travis-ci.org/corydolphin/flask-cors.svg?branch=master
+.. |Build Status| image:: https://github.com/corydolphin/flask-cors/actions/workflows/unittests.yaml/badge.svg
    :target: https://travis-ci.org/corydolphin/flask-cors
 .. |Latest Version| image:: https://img.shields.io/pypi/v/Flask-Cors.svg
    :target: https://pypi.python.org/pypi/Flask-Cors/
 .. |Supported Python versions| image:: https://img.shields.io/pypi/pyversions/Flask-Cors.svg
    :target: https://img.shields.io/pypi/pyversions/Flask-Cors.svg
 .. |License| image:: http://img.shields.io/:license-mit-blue.svg
    :target: https://pypi.python.org/pypi/Flask-Cors/
```

### Comparing `Flask-Cors-4.0.0a0/README.rst` & `flask_cors-4.0.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,40 +2,40 @@
 ==========
 
 |Build Status| |Latest Version| |Supported Python versions|
 |License|
 
 A Flask extension for handling Cross Origin Resource Sharing (CORS), making cross-origin AJAX possible.
 
-This package has a simple philosophy: when you want to enable CORS, you wish to enable it for all use cases on a domain. 
-This means no mucking around with different allowed headers, methods, etc. 
+This package has a simple philosophy: when you want to enable CORS, you wish to enable it for all use cases on a domain.
+This means no mucking around with different allowed headers, methods, etc.
 
-By default, submission of cookies across domains is disabled due to the security implications. 
+By default, submission of cookies across domains is disabled due to the security implications.
 Please see the documentation for how to enable credential'ed requests, and please make sure you add some sort of `CSRF <http://en.wikipedia.org/wiki/Cross-site_request_forgery>`__ protection before doing so!
 
 Installation
 ------------
 
 Install the extension with using pip, or easy\_install.
 
 .. code:: bash
 
     $ pip install -U flask-cors
 
 Usage
 -----
 
-This package exposes a Flask extension which by default enables CORS support on all routes, for all origins and methods. 
-It allows parameterization of all CORS headers on a per-resource level. 
+This package exposes a Flask extension which by default enables CORS support on all routes, for all origins and methods.
+It allows parameterization of all CORS headers on a per-resource level.
 The package also contains a decorator, for those who prefer this approach.
 
 Simple Usage
 ~~~~~~~~~~~~
 
-In the simplest case, initialize the Flask-Cors extension with default arguments in order to allow CORS for all domains on all routes. 
+In the simplest case, initialize the Flask-Cors extension with default arguments in order to allow CORS for all domains on all routes.
 See the full list of options in the `documentation <https://flask-cors.corydolphin.com/en/latest/api.html#extension>`__.
 
 .. code:: python
 
 
     from flask import Flask
     from flask_cors import CORS
@@ -46,31 +46,31 @@
     @app.route("/")
     def helloWorld():
       return "Hello, cross-origin-world!"
 
 Resource specific CORS
 ^^^^^^^^^^^^^^^^^^^^^^
 
-Alternatively, you can specify CORS options on a resource and origin level of granularity by passing a dictionary as the `resources` option, mapping paths to a set of options. 
+Alternatively, you can specify CORS options on a resource and origin level of granularity by passing a dictionary as the `resources` option, mapping paths to a set of options.
 See the full list of options in the `documentation <https://flask-cors.corydolphin.com/en/latest/api.html#extension>`__.
 
 .. code:: python
 
     app = Flask(__name__)
     cors = CORS(app, resources={r"/api/*": {"origins": "*"}})
 
     @app.route("/api/v1/users")
     def list_users():
       return "user example"
 
 Route specific CORS via decorator
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-This extension also exposes a simple decorator to decorate flask routes with. 
-Simply add ``@cross_origin()`` below a call to Flask's ``@app.route(..)`` to allow CORS on a given route. 
+This extension also exposes a simple decorator to decorate flask routes with.
+Simply add ``@cross_origin()`` below a call to Flask's ``@app.route(..)`` to allow CORS on a given route.
 See the full list of options in the `decorator documentation <https://flask-cors.corydolphin.com/en/latest/api.html#decorator>`__.
 
 .. code:: python
 
     @app.route("/")
     @cross_origin()
     def helloWorld():
@@ -90,33 +90,33 @@
 
     logging.getLogger('flask_cors').level = logging.DEBUG
 
 
 Tests
 -----
 
-A simple set of tests is included in ``test/``. 
+A simple set of tests is included in ``test/``.
 To run, install nose, and simply invoke ``nosetests`` or ``python setup.py test`` to exercise the tests.
 
 If nosetests does not work for you, due to it no longer working with newer python versions.
 You can use pytest to run the tests instead.
 
 Contributing
 ------------
 
-Questions, comments or improvements? 
-Please create an issue on `Github <https://github.com/corydolphin/flask-cors>`__, tweet at `@corydolphin <https://twitter.com/corydolphin>`__ or send me an email. 
+Questions, comments or improvements?
+Please create an issue on `Github <https://github.com/corydolphin/flask-cors>`__, tweet at `@corydolphin <https://twitter.com/corydolphin>`__ or send me an email.
 I do my best to include every contribution proposed in any way that I can.
 
 Credits
 -------
 
 This Flask extension is based upon the `Decorator for the HTTP Access Control <https://web.archive.org/web/20190128010149/http://flask.pocoo.org/snippets/56/>`__ written by Armin Ronacher.
 
-.. |Build Status| image:: https://api.travis-ci.org/corydolphin/flask-cors.svg?branch=master
+.. |Build Status| image:: https://github.com/corydolphin/flask-cors/actions/workflows/unittests.yaml/badge.svg
    :target: https://travis-ci.org/corydolphin/flask-cors
 .. |Latest Version| image:: https://img.shields.io/pypi/v/Flask-Cors.svg
    :target: https://pypi.python.org/pypi/Flask-Cors/
 .. |Supported Python versions| image:: https://img.shields.io/pypi/pyversions/Flask-Cors.svg
    :target: https://img.shields.io/pypi/pyversions/Flask-Cors.svg
 .. |License| image:: http://img.shields.io/:license-mit-blue.svg
    :target: https://pypi.python.org/pypi/Flask-Cors/
```

### Comparing `Flask-Cors-4.0.0a0/docs/Makefile` & `flask_cors-4.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0a0/docs/api.rst` & `flask_cors-4.0.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0a0/docs/conf.py` & `flask_cors-4.0.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,8 +251,8 @@
 #texinfo_domain_indices = True
 
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
 #texinfo_show_urls = 'footnote'
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {'http://docs.python.org/': None}
+intersphinx_mapping = {'py': ('http://docs.python.org/', None)}
```

### Comparing `Flask-Cors-4.0.0a0/docs/configuration.rst` & `flask_cors-4.0.1/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0a0/examples/app_based_example.py` & `flask_cors-4.0.1/examples/app_based_example.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0a0/examples/blueprints_based_example.py` & `flask_cors-4.0.1/examples/blueprints_based_example.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0a0/examples/view_based_example.py` & `flask_cors-4.0.1/examples/view_based_example.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0a0/flask_cors/__init__.py` & `flask_cors-4.0.1/flask_cors/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0a0/flask_cors/core.py` & `flask_cors-4.0.1/flask_cors/core.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0a0/flask_cors/decorator.py` & `flask_cors-4.0.1/flask_cors/decorator.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0a0/flask_cors/extension.py` & `flask_cors-4.0.1/flask_cors/extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,17 +66,19 @@
     :type resources: dict, iterable or string
 
     :param origins:
         The origin, or list of origins to allow requests from.
         The origin(s) may be regular expressions, case-sensitive strings,
         or else an asterisk.
 
-        :note: origins must include the schema and the port (if not port 80),
-        e.g.,
-        `CORS(app, origins=["http://localhost:8000", "https://example.com"])`.
+        ..  note::
+
+            origins must include the schema and the port (if not port 80),
+            e.g.,
+            `CORS(app, origins=["http://localhost:8000", "https://example.com"])`.
 
         Default : '*'
     :type origins: list, string or regex
 
     :param methods:
         The method or list of methods which the allowed origins are allowed to
         access for non-simple requests.
@@ -156,15 +158,15 @@
         # the app's configuration, the constructor, the kwargs to init_app, and
         # finally the options specified in the resources dictionary.
         resources = [
                      (pattern, get_cors_options(app, options, opts))
                      for (pattern, opts) in resources
                     ]
 
-        # Create a human readable form of these resources by converting the compiled
+        # Create a human-readable form of these resources by converting the compiled
         # regular expressions into strings.
         resources_human = {get_regexp_pattern(pattern): opts for (pattern,opts) in resources}
         LOG.debug("Configuring CORS with resources: %s", resources_human)
 
         cors_after_request = make_after_request_function(resources)
         app.after_request(cors_after_request)
 
@@ -187,15 +189,15 @@
         # If CORS headers are set in a view decorator, pass
         if resp.headers is not None and resp.headers.get(ACL_ORIGIN):
             LOG.debug('CORS have been already evaluated, skipping')
             return resp
         normalized_path = unquote_plus(request.path)
         for res_regex, res_options in resources:
             if try_match(normalized_path, res_regex):
-                LOG.debug("Request to '%s' matches CORS resource '%s'. Using options: %s",
+                LOG.debug("Request to '%r' matches CORS resource '%s'. Using options: %s",
                       request.path, get_regexp_pattern(res_regex), res_options)
                 set_cors_headers(resp, res_options)
                 break
         else:
             LOG.debug('No CORS rule matches')
         return resp
     return cors_after_request
```

### Comparing `Flask-Cors-4.0.0a0/setup.py` & `flask_cors-4.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,13 +43,14 @@
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
         'Topic :: Software Development :: Libraries :: Python Modules'
     ]
 )
```

### Comparing `Flask-Cors-4.0.0a0/tests/base_test.py` & `flask_cors-4.0.1/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0a0/tests/core/helper_tests.py` & `flask_cors-4.0.1/tests/core/helper_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 
 class InternalsTestCase(unittest.TestCase):
     def test_try_match(self):
         self.assertFalse(try_match('www.com/foo', 'www.com/fo'))
         self.assertTrue(try_match('www.com/foo', 'www.com/fo*'))
 
     def test_flexible_str_str(self):
-        self.assertEquals(flexible_str('Bar, Foo, Qux'), 'Bar, Foo, Qux')
+        self.assertEqual(flexible_str('Bar, Foo, Qux'), 'Bar, Foo, Qux')
 
     def test_flexible_str_set(self):
-        self.assertEquals(flexible_str({'Foo', 'Bar', 'Qux'}),
+        self.assertEqual(flexible_str({'Foo', 'Bar', 'Qux'}),
                           'Bar, Foo, Qux')
 
     def test_serialize_options(self):
         try:
             serialize_options({
                 'origins': r'*',
                 'allow_headers': True,
@@ -39,32 +39,32 @@
             self.assertFalse(True, "A Value Error should have been raised.")
         except ValueError:
             pass
 
     def test_get_allow_headers_empty(self):
         options = serialize_options({'allow_headers': r'*'})
 
-        self.assertEquals(get_allow_headers(options, ''), None)
-        self.assertEquals(get_allow_headers(options, None), None)
+        self.assertEqual(get_allow_headers(options, ''), None)
+        self.assertEqual(get_allow_headers(options, None), None)
 
     def test_get_allow_headers_matching(self):
         options = serialize_options({'allow_headers': r'*'})
 
-        self.assertEquals(get_allow_headers(options, 'X-FOO'), 'X-FOO')
-        self.assertEquals(
+        self.assertEqual(get_allow_headers(options, 'X-FOO'), 'X-FOO')
+        self.assertEqual(
             get_allow_headers(options, 'X-Foo, X-Bar'),
             'X-Bar, X-Foo'
         )
 
     def test_get_allow_headers_matching_none(self):
         options = serialize_options({'allow_headers': r'X-FLASK-.*'})
 
-        self.assertEquals(get_allow_headers(options, 'X-FLASK-CORS'),
+        self.assertEqual(get_allow_headers(options, 'X-FLASK-CORS'),
                           'X-FLASK-CORS')
-        self.assertEquals(
+        self.assertEqual(
             get_allow_headers(options, 'X-NOT-FLASK-CORS'),
             ''
         )
 
     def test_parse_resources_sorted(self):
         resources = parse_resources({
             '/foo': {'origins': 'http://foo.com'},
```

### Comparing `Flask-Cors-4.0.0a0/tests/core/test_override_headers.py` & `flask_cors-4.0.1/tests/core/test_override_headers.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0a0/tests/decorator/test_allow_headers.py` & `flask_cors-4.0.1/tests/decorator/test_allow_headers.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0a0/tests/decorator/test_credentials.py` & `flask_cors-4.0.1/tests/decorator/test_credentials.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0a0/tests/decorator/test_duplicate_headers.py` & `flask_cors-4.0.1/tests/decorator/test_duplicate_headers.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0a0/tests/decorator/test_exception_interception.py` & `flask_cors-4.0.1/tests/decorator/test_exception_interception.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0a0/tests/decorator/test_expose_headers.py` & `flask_cors-4.0.1/tests/decorator/test_expose_headers.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0a0/tests/decorator/test_max_age.py` & `flask_cors-4.0.1/tests/decorator/test_max_age.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0a0/tests/decorator/test_methods.py` & `flask_cors-4.0.1/tests/decorator/test_methods.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0a0/tests/decorator/test_options.py` & `flask_cors-4.0.1/tests/decorator/test_options.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0a0/tests/decorator/test_origins.py` & `flask_cors-4.0.1/tests/decorator/test_origins.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0a0/tests/decorator/test_vary_header.py` & `flask_cors-4.0.1/tests/decorator/test_vary_header.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0a0/tests/decorator/test_w3.py` & `flask_cors-4.0.1/tests/decorator/test_w3.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0a0/tests/extension/test_app_extension.py` & `flask_cors-4.0.1/tests/extension/test_app_extension.py`

 * *Files identical despite different names*

