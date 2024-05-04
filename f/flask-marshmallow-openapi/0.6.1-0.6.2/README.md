# Comparing `tmp/flask-marshmallow-openapi-0.6.1.tar.gz` & `tmp/flask_marshmallow_openapi-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-marshmallow-openapi-0.6.1.tar", last modified: Tue Nov 21 07:01:59 2023, max compression
+gzip compressed data, was "flask_marshmallow_openapi-0.6.2.tar", last modified: Sat May  4 08:16:52 2024, max compression
```

## Comparing `flask-marshmallow-openapi-0.6.1.tar` & `flask_marshmallow_openapi-0.6.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 07:01:59.464349 flask-marshmallow-openapi-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      709 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      838 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2023-11-21 07:01:59.464349 flask-marshmallow-openapi-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-21 07:01:59.464349 flask-marshmallow-openapi-0.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 07:01:59.448348 flask-marshmallow-openapi-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 07:01:59.452349 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 07:01:59.452349 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/decorators/decorate_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/decorators/decorate_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/decorators/decorate_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4411 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/decorators/decorate_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/decorators/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5889 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/flask_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)    15470 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/schemas_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/securities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 07:01:59.452349 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/static/
--rw-r--r--   0 runner    (1001) docker     (127)     8215 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/static/redoc_favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 07:01:59.460348 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/static/swagger_ui/
--rw-r--r--   0 runner    (1001) docker     (127)      665 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)      628 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/static/swagger_ui/index.css
--rw-r--r--   0 runner    (1001) docker     (127)      734 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/static/swagger_ui/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html
--rw-r--r--   0 runner    (1001) docker     (127)      539 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js
--rw-r--r--   0 runner    (1001) docker     (127)  1045708 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)   368781 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js
--rw-r--r--   0 runner    (1001) docker     (127)  1045498 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)   322863 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js
--rw-r--r--   0 runner    (1001) docker     (127)   145206 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css
--rw-r--r--   0 runner    (1001) docker     (127)   256702 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/static_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 07:01:59.460348 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/templates/changelog.html.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/templates/re_doc.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2023-11-21 07:01:48.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 07:01:59.460348 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2023-11-21 07:01:59.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2023-11-21 07:01:59.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 07:01:59.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 07:01:59.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      479 2023-11-21 07:01:59.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-11-21 07:01:59.000000 flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:16:52.076809 flask_marshmallow_openapi-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-04 08:16:52.076809 flask_marshmallow_openapi-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 08:16:52.076809 flask_marshmallow_openapi-0.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:16:52.060808 flask_marshmallow_openapi-0.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:16:52.064808 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:16:52.064808 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/decorators/decorate_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/decorators/decorate_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/decorators/decorate_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/decorators/decorate_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/decorators/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5889 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/flask_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16024 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/schemas_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/securities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:16:52.064808 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/redoc_favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:16:52.072808 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/index.css
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js
+-rw-r--r--   0 runner    (1001) docker     (127)  1045708 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)   368781 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js
+-rw-r--r--   0 runner    (1001) docker     (127)  1045498 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)   322863 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js
+-rw-r--r--   0 runner    (1001) docker     (127)   145206 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css
+-rw-r--r--   0 runner    (1001) docker     (127)   256702 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:16:52.072808 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/templates/changelog.html.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/templates/re_doc.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-04 08:16:47.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:16:52.072808 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-04 08:16:52.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-04 08:16:52.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 08:16:52.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 08:16:51.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-04 08:16:52.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-04 08:16:52.000000 flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi.egg-info/top_level.txt
```

### Comparing `flask-marshmallow-openapi-0.6.1/.gitignore` & `flask_marshmallow_openapi-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.6.1/LICENSE` & `flask_marshmallow_openapi-0.6.2/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 tadams42
+Copyright (c) 2023, 2024 tadams42
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `flask-marshmallow-openapi-0.6.1/MANIFEST.in` & `flask_marshmallow_openapi-0.6.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.6.1/PKG-INFO` & `flask_marshmallow_openapi-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-marshmallow-openapi
-Version: 0.6.1
+Version: 0.6.2
 Summary: Flask + marshmallow + OpenAPI
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/flask-marshmallow-openapi
 Keywords: OpenAPI SwaggerUI ReDoc
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: apispec[marshmallow,yaml]
-Requires-Dist: flask>=2.3.0
+Requires-Dist: flask>=2.0.1
 Requires-Dist: inflection
 Requires-Dist: marshmallow>=3.18.0
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: wrapt
 Requires-Dist: openapi-pydantic-models>=1.0.1
 Provides-Extra: dev
```

### Comparing `flask-marshmallow-openapi-0.6.1/README.md` & `flask_marshmallow_openapi-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.6.1/pyproject.toml` & `flask_marshmallow_openapi-0.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 65", "wheel"]
 
 
 [project]
 name = "flask-marshmallow-openapi"
-version = "0.6.1"
+version = "0.6.2"
 description = "Flask + marshmallow + OpenAPI"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
@@ -19,15 +19,15 @@
     "Programming Language :: Python :: 3 :: Only",
 ]
 keywords = ["OpenAPI SwaggerUI ReDoc"]
 license = { text = "MIT" }
 authors = [{ name = "Tomislav Adamic", email = "tomislav.adamic@gmail.com" }]
 dependencies = [
     "apispec[yaml,marshmallow]",
-    "flask >= 2.3.0",
+    "flask >= 2.0.1",
     "inflection",
     "marshmallow >= 3.18.0",
     "pyyaml",
     "requests",
     "wrapt",
     "openapi-pydantic-models >= 1.0.1",
 ]
```

### Comparing `flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/decorators/decorate_delete.py` & `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/decorators/decorate_delete.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/decorators/decorate_get.py` & `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/decorators/decorate_get.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/decorators/decorate_patch.py` & `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/decorators/decorate_patch.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/decorators/decorate_post.py` & `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/decorators/decorate_post.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/decorators/helpers.py` & `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/decorators/helpers.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/flask_paths.py` & `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/flask_paths.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/middleware.py` & `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/middleware.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import json
 import os
 from dataclasses import dataclass
-from pathlib import Path
 from typing import Callable
 
 import apispec
 import flask
 import requests
 from apispec.exceptions import DuplicateComponentNameError
 from apispec.ext.marshmallow import MarshmallowPlugin
 from openapi_pydantic_models import OperationObject
 
 from .flask_paths import FlaskPathsManager
 from .schemas_registry import SchemasRegistry
 from .static_collector import StaticResourcesCollector
 
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from pathlib import Path
+
 _MINIMAL_SPEC = {"title": "Some API", "openapi_version": "3.0.2", "version": "v1"}
 
 _DEFAULT_SECURITIES = {
     "components": {
         "securitySchemes": {
             "access_token": {
                 "scheme": "bearer",
@@ -223,25 +227,36 @@
             https://apispec.readthedocs.io/en/latest/using_plugins.html#custom-fields
         """
         self._attribute_functions.append(f)
 
     def init_app(self, app: flask.Flask):
         self._add_own_endpoints()
 
-        full_url_prefix = (
-            Path(self.config.mounted_at or "/") / f"./{self.blueprint.url_prefix}"
+        # Try making safe URL path from whatever input we get via self.config and
+        # self.blueprint. This is still not absolutely foolproof and will give dubious
+        # results for ie ("/v1//docs", "/foobar") => "/v1//docs/foobar". urllib.parse
+        # doesn't help here since it also doesn't try to correct invalid or dubious
+        # input.
+        full_url_prefix = "/" + "/".join(
+            [
+                _.strip("/\\")
+                for _ in [
+                    f"/{self.config.mounted_at or '/'}/",
+                    f"/{self.blueprint.url_prefix}",
+                ]
+            ]
         )
 
         with app.test_request_context():
             SchemasRegistry.find_all_schemas(self.config.app_package_name)
             self._init_apispec()
             self._collect_shema_docs()
             self._collect_endpoints_docs(app)
 
-        app.register_blueprint(self.blueprint, url_prefix=str(full_url_prefix))
+        app.register_blueprint(self.blueprint, url_prefix=full_url_prefix)
 
         if not hasattr(app, "extensions"):
             app.extensions = {}
         app.extensions["open_api"] = self
 
     def _collect_endpoints_docs(self, app):
         for converted_path, operations in FlaskPathsManager(
```

### Comparing `flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/schemas_registry.py` & `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/schemas_registry.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/static/redoc_favicon.png` & `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/redoc_favicon.png`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png` & `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png` & `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/static/swagger_ui/index.html` & `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/index.html`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html` & `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js` & `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js` & `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js` & `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js` & `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js` & `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css` & `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js` & `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/static_collector.py` & `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/static_collector.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/templates/changelog.html.jinja2` & `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/templates/changelog.html.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/templates/re_doc.jinja2` & `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/templates/re_doc.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2` & `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi.egg-info/PKG-INFO` & `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-marshmallow-openapi
-Version: 0.6.1
+Version: 0.6.2
 Summary: Flask + marshmallow + OpenAPI
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/flask-marshmallow-openapi
 Keywords: OpenAPI SwaggerUI ReDoc
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: apispec[marshmallow,yaml]
-Requires-Dist: flask>=2.3.0
+Requires-Dist: flask>=2.0.1
 Requires-Dist: inflection
 Requires-Dist: marshmallow>=3.18.0
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: wrapt
 Requires-Dist: openapi-pydantic-models>=1.0.1
 Provides-Extra: dev
```

### Comparing `flask-marshmallow-openapi-0.6.1/src/flask_marshmallow_openapi.egg-info/SOURCES.txt` & `flask_marshmallow_openapi-0.6.2/src/flask_marshmallow_openapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

