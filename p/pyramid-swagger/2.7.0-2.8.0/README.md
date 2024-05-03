# Comparing `tmp/pyramid_swagger-2.7.0.tar.gz` & `tmp/pyramid_swagger-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyramid_swagger-2.7.0.tar", last modified: Tue May  7 14:20:30 2019, max compression
+gzip compressed data, was "pyramid_swagger-2.8.0.tar", last modified: Fri May  3 23:10:01 2024, max compression
```

## Comparing `pyramid_swagger-2.7.0.tar` & `pyramid_swagger-2.8.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 maci     (537078489) AD\Domain Users (1954207199)        0 2019-05-07 14:20:30.000000 pyramid_swagger-2.7.0/
--rw-r--r--   0 maci     (537078489) AD\Domain Users (1954207199)      141 2019-02-11 18:59:11.000000 pyramid_swagger-2.7.0/MANIFEST.in
--rw-r--r--   0 maci     (537078489) AD\Domain Users (1954207199)     3759 2019-05-07 14:20:30.000000 pyramid_swagger-2.7.0/PKG-INFO
--rw-r--r--   0 maci     (537078489) AD\Domain Users (1954207199)     2519 2019-05-05 22:14:35.000000 pyramid_swagger-2.7.0/README.rst
-drwxr-xr-x   0 maci     (537078489) AD\Domain Users (1954207199)        0 2019-05-07 14:20:29.000000 pyramid_swagger-2.7.0/pyramid_swagger/
--rw-r--r--   0 maci     (537078489) AD\Domain Users (1954207199)      582 2019-05-07 14:17:50.000000 pyramid_swagger-2.7.0/pyramid_swagger/__about__.py
--rw-r--r--   0 maci     (537078489) AD\Domain Users (1954207199)     2137 2019-05-05 22:47:23.000000 pyramid_swagger-2.7.0/pyramid_swagger/__init__.py
--rw-r--r--   0 maci     (537078489) AD\Domain Users (1954207199)    10264 2019-05-05 22:47:23.000000 pyramid_swagger-2.7.0/pyramid_swagger/api.py
--rw-r--r--   0 maci     (537078489) AD\Domain Users (1954207199)     1267 2019-05-05 22:47:23.000000 pyramid_swagger-2.7.0/pyramid_swagger/exceptions.py
--rw-r--r--   0 maci     (537078489) AD\Domain Users (1954207199)     9324 2019-05-06 08:46:17.000000 pyramid_swagger-2.7.0/pyramid_swagger/ingest.py
--rw-r--r--   0 maci     (537078489) AD\Domain Users (1954207199)     9177 2019-05-06 08:46:17.000000 pyramid_swagger-2.7.0/pyramid_swagger/load_schema.py
--rw-r--r--   0 maci     (537078489) AD\Domain Users (1954207199)     2981 2019-05-05 22:47:23.000000 pyramid_swagger-2.7.0/pyramid_swagger/model.py
--rw-r--r--   0 maci     (537078489) AD\Domain Users (1954207199)     1886 2019-05-05 22:47:23.000000 pyramid_swagger-2.7.0/pyramid_swagger/renderer.py
--rw-r--r--   0 maci     (537078489) AD\Domain Users (1954207199)     1309 2019-05-05 22:47:23.000000 pyramid_swagger-2.7.0/pyramid_swagger/spec.py
--rw-r--r--   0 maci     (537078489) AD\Domain Users (1954207199)    21413 2019-05-05 23:21:44.000000 pyramid_swagger-2.7.0/pyramid_swagger/tween.py
-drwxr-xr-x   0 maci     (537078489) AD\Domain Users (1954207199)        0 2019-05-07 14:20:30.000000 pyramid_swagger-2.7.0/pyramid_swagger.egg-info/
--rw-r--r--   0 maci     (537078489) AD\Domain Users (1954207199)     3759 2019-05-07 14:20:29.000000 pyramid_swagger-2.7.0/pyramid_swagger.egg-info/PKG-INFO
--rw-r--r--   0 maci     (537078489) AD\Domain Users (1954207199)      504 2019-05-07 14:20:29.000000 pyramid_swagger-2.7.0/pyramid_swagger.egg-info/SOURCES.txt
--rw-r--r--   0 maci     (537078489) AD\Domain Users (1954207199)        1 2019-05-07 14:20:29.000000 pyramid_swagger-2.7.0/pyramid_swagger.egg-info/dependency_links.txt
--rw-r--r--   0 maci     (537078489) AD\Domain Users (1954207199)       50 2019-05-07 14:20:29.000000 pyramid_swagger-2.7.0/pyramid_swagger.egg-info/requires.txt
--rw-r--r--   0 maci     (537078489) AD\Domain Users (1954207199)       16 2019-05-07 14:20:29.000000 pyramid_swagger-2.7.0/pyramid_swagger.egg-info/top_level.txt
--rw-r--r--   0 maci     (537078489) AD\Domain Users (1954207199)      106 2019-05-07 14:20:30.000000 pyramid_swagger-2.7.0/setup.cfg
--rw-r--r--   0 maci     (537078489) AD\Domain Users (1954207199)     1352 2019-05-05 22:47:23.000000 pyramid_swagger-2.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:01.299472 pyramid_swagger-2.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-03 23:09:59.000000 pyramid_swagger-2.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-03 23:09:59.000000 pyramid_swagger-2.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-03 23:10:01.299472 pyramid_swagger-2.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-03 23:09:59.000000 pyramid_swagger-2.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:01.299472 pyramid_swagger-2.8.0/pyramid_swagger/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-03 23:09:59.000000 pyramid_swagger-2.8.0/pyramid_swagger/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-03 23:09:59.000000 pyramid_swagger-2.8.0/pyramid_swagger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-05-03 23:09:59.000000 pyramid_swagger-2.8.0/pyramid_swagger/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-03 23:09:59.000000 pyramid_swagger-2.8.0/pyramid_swagger/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-05-03 23:09:59.000000 pyramid_swagger-2.8.0/pyramid_swagger/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9635 2024-05-03 23:09:59.000000 pyramid_swagger-2.8.0/pyramid_swagger/load_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-03 23:09:59.000000 pyramid_swagger-2.8.0/pyramid_swagger/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-03 23:09:59.000000 pyramid_swagger-2.8.0/pyramid_swagger/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-03 23:09:59.000000 pyramid_swagger-2.8.0/pyramid_swagger/spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21771 2024-05-03 23:09:59.000000 pyramid_swagger-2.8.0/pyramid_swagger/tween.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:10:01.299472 pyramid_swagger-2.8.0/pyramid_swagger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-03 23:10:01.000000 pyramid_swagger-2.8.0/pyramid_swagger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-03 23:10:01.000000 pyramid_swagger-2.8.0/pyramid_swagger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 23:10:01.000000 pyramid_swagger-2.8.0/pyramid_swagger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-03 23:10:01.000000 pyramid_swagger-2.8.0/pyramid_swagger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 23:10:01.000000 pyramid_swagger-2.8.0/pyramid_swagger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-03 23:10:01.299472 pyramid_swagger-2.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-03 23:09:59.000000 pyramid_swagger-2.8.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyramid_swagger-2.7.0/PKG-INFO` & `pyramid_swagger-2.8.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,87 +1,85 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyramid_swagger
-Version: 2.7.0
+Version: 2.8.0
 Summary: Swagger tools for use in pyramid webapps
 Home-page: https://github.com/striglia/pyramid_swagger
 Author: Scott Triglia
 Author-email: scott.triglia@gmail.com
 License: BSD 3-clause
-Description: :PyPI: https://pypi.python.org/pypi/pyramid_swagger
-        :Documentation: http://pyramid-swagger.readthedocs.org/en/latest/
-        :Source: https://github.com/striglia/pyramid_swagger
-        :License: Copyright © 2014 Scott Triglia under the `BSD 3-clause <http://opensource.org/licenses/BSD-3-Clause>`_
-        :Build status:
-            .. image:: https://travis-ci.org/striglia/pyramid_swagger.png?branch=master
-                :target: https://travis-ci.org/striglia/pyramid_swagger?branch=master
-                :alt: Travis CI
-            .. image:: https://ci.appveyor.com/api/projects/status/ufmlmpwy1vj3yjgk/branch/master?svg=true
-                :target: https://ci.appveyor.com/project/striglia/pyramid-swagger
-                :alt: Appveyor (Windows CI)
-        :Current coverage on master:
-            .. image:: https://coveralls.io/repos/striglia/pyramid_swagger/badge.png
-                :target: https://coveralls.io/r/striglia/pyramid_swagger
-        :Persistent chat for questions:
-            .. image:: https://badges.gitter.im/Join%20Chat.svg
-                :alt: Join the chat at https://gitter.im/striglia/pyramid_swagger
-                :target: https://gitter.im/striglia/pyramid_swagger?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
-        
-        
-        pyramid_swagger
-        ===============
-        
-        This project offers convenient tools for using Swagger to define and validate
-        your interfaces in a Pyramid webapp.
-        
-        Full documentation is available at http://pyramid-swagger.readthedocs.org/.
-        
-        
-        How to contribute
-        -----------------
-        
-        #. Fork this repository on Github: https://help.github.com/articles/fork-a-repo/
-        #. Clone your forked repository: https://help.github.com/articles/cloning-a-repository/
-        #. Make a feature branch for your changes:
-        
-            ::
-        
-                git remote add upstream https://github.com/striglia/pyramid_swagger.git
-                git fetch upstream
-                git checkout upstream/master -b my-feature-branch
-        
-        #. Create and activate the virtual environment, this will provide you with all the
-           libraries and tools necessary for pyramid_swagger development:
-        
-            ::
-        
-                make
-                source .activate.sh
-        
-        #. Make sure the test suite works before you start:
-        
-            ::
-        
-                tox -e py27    # Note: use py35 for Python 3.5, see tox.ini for possible values
-        
-        #. Commit patches: http://gitref.org/basic/
-        #. Push to github: ``git pull && git push origin``
-        #. Send a pull request: https://help.github.com/articles/creating-a-pull-request/
-        
-        
-        Running a single test
-        *********************
-        
-        Make sure you have activated the virtual environment (see above).
-        
-        ::
-        
-            py.test -vvv tests/tween_test.py::test_response_properties
-        
 Keywords: pyramid swagger validation
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE
+
+:PyPI: https://pypi.python.org/pypi/pyramid_swagger
+:Documentation: http://pyramid-swagger.readthedocs.org/en/latest/
+:Source: https://github.com/striglia/pyramid_swagger
+:License: Copyright © 2014 Scott Triglia under the `BSD 3-clause <http://opensource.org/licenses/BSD-3-Clause>`_
+:Build status:
+    .. image:: https://travis-ci.org/striglia/pyramid_swagger.png?branch=master
+        :target: https://travis-ci.org/striglia/pyramid_swagger?branch=master
+        :alt: Travis CI
+    .. image:: https://ci.appveyor.com/api/projects/status/ufmlmpwy1vj3yjgk/branch/master?svg=true
+        :target: https://ci.appveyor.com/project/striglia/pyramid-swagger
+        :alt: Appveyor (Windows CI)
+:Current coverage on master:
+    .. image:: https://coveralls.io/repos/striglia/pyramid_swagger/badge.png
+        :target: https://coveralls.io/r/striglia/pyramid_swagger
+:Persistent chat for questions:
+    .. image:: https://badges.gitter.im/Join%20Chat.svg
+        :alt: Join the chat at https://gitter.im/striglia/pyramid_swagger
+        :target: https://gitter.im/striglia/pyramid_swagger?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
+
+
+pyramid_swagger
+===============
+
+This project offers convenient tools for using Swagger to define and validate
+your interfaces in a Pyramid webapp.
+
+Full documentation is available at http://pyramid-swagger.readthedocs.org/.
+
+
+How to contribute
+-----------------
+
+#. Fork this repository on Github: https://help.github.com/articles/fork-a-repo/
+#. Clone your forked repository: https://help.github.com/articles/cloning-a-repository/
+#. Make a feature branch for your changes:
+
+    ::
+
+        git remote add upstream https://github.com/Yelp/pyramid_swagger.git
+        git fetch upstream
+        git checkout upstream/master -b my-feature-branch
+
+#. Create and activate the virtual environment, this will provide you with all the
+   libraries and tools necessary for pyramid_swagger development:
+
+    ::
+
+        make
+        source .activate.sh
+
+#. Make sure the test suite works before you start:
+
+    ::
+
+        tox -e py38    # Note: use py310 for Python 3.10, see tox.ini for possible values
+
+#. Commit patches: http://gitref.org/basic/
+#. Push to github: ``git pull && git push origin``
+#. Send a pull request: https://help.github.com/articles/creating-a-pull-request/
+
+
+Running a single test
+*********************
+
+Make sure you have activated the virtual environment (see above).
+
+::
+
+    py.test -vvv tests/tween_test.py::test_response_properties
```

### Comparing `pyramid_swagger-2.7.0/README.rst` & `pyramid_swagger-2.8.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 #. Fork this repository on Github: https://help.github.com/articles/fork-a-repo/
 #. Clone your forked repository: https://help.github.com/articles/cloning-a-repository/
 #. Make a feature branch for your changes:
 
     ::
 
-        git remote add upstream https://github.com/striglia/pyramid_swagger.git
+        git remote add upstream https://github.com/Yelp/pyramid_swagger.git
         git fetch upstream
         git checkout upstream/master -b my-feature-branch
 
 #. Create and activate the virtual environment, this will provide you with all the
    libraries and tools necessary for pyramid_swagger development:
 
     ::
@@ -48,15 +48,15 @@
         make
         source .activate.sh
 
 #. Make sure the test suite works before you start:
 
     ::
 
-        tox -e py27    # Note: use py35 for Python 3.5, see tox.ini for possible values
+        tox -e py38    # Note: use py310 for Python 3.10, see tox.ini for possible values
 
 #. Commit patches: http://gitref.org/basic/
 #. Push to github: ``git pull && git push origin``
 #. Send a pull request: https://help.github.com/articles/creating-a-pull-request/
 
 
 Running a single test
```

### Comparing `pyramid_swagger-2.7.0/pyramid_swagger/__about__.py` & `pyramid_swagger-2.8.0/pyramid_swagger/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,14 @@
     "__email__", "__license__", "__copyright__",
 ]
 
 __title__ = "pyramid_swagger"
 __summary__ = "Swagger tools for use in pyramid webapps"
 __uri__ = "https://github.com/striglia/pyramid_swagger"
 
-__version__ = "2.7.0"
+__version__ = "2.8.0"
 
 __author__ = "Scott Triglia"
 __email__ = "scott.triglia@gmail.com"
 
 __license__ = "BSD 3-clause"
 __copyright__ = "Copyright 2014 Scott Triglia"
```

### Comparing `pyramid_swagger-2.7.0/pyramid_swagger/__init__.py` & `pyramid_swagger-2.8.0/pyramid_swagger/__init__.py`

 * *Files identical despite different names*

### Comparing `pyramid_swagger-2.7.0/pyramid_swagger/api.py` & `pyramid_swagger-2.8.0/pyramid_swagger/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,15 +229,15 @@
 class YamlRendererFactory(object):
     def __init__(self, info):
         pass
 
     def __call__(self, value, system):
         response = system['request'].response
         response.headers['Content-Type'] = 'application/x-yaml; charset=UTF-8'
-        return yaml.dump(value).encode('utf-8')
+        return yaml.safe_dump(value).encode('utf-8')
 
 
 def build_swagger_20_swagger_schema_views(config):
     settings = config.registry.settings
     if settings.get('pyramid_swagger.dereference_served_schema'):
         views = _build_dereferenced_swagger_20_schema_views(config)
     else:
```

### Comparing `pyramid_swagger-2.7.0/pyramid_swagger/exceptions.py` & `pyramid_swagger-2.8.0/pyramid_swagger/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,22 +3,29 @@
 
 import sys
 
 import six
 from pyramid.httpexceptions import HTTPBadRequest
 from pyramid.httpexceptions import HTTPInternalServerError
 from pyramid.httpexceptions import HTTPNotFound
+from pyramid.httpexceptions import HTTPUnauthorized
 
 
 class RequestValidationError(HTTPBadRequest):
     def __init__(self, *args, **kwargs):
         self.child = kwargs.pop('child', None)
         super(RequestValidationError, self).__init__(*args, **kwargs)
 
 
+class RequestAuthenticationError(HTTPUnauthorized):
+    def __init__(self, *args, **kwargs):
+        self.child = kwargs.pop('child', None)
+        super(RequestAuthenticationError, self).__init__(*args, **kwargs)
+
+
 class PathNotFoundError(HTTPNotFound):
     def __init__(self, *args, **kwargs):
         self.child = kwargs.pop('child', None)
         super(PathNotFoundError, self).__init__(*args, **kwargs)
 
 
 class ResponseValidationError(HTTPInternalServerError):
```

### Comparing `pyramid_swagger-2.7.0/pyramid_swagger/ingest.py` & `pyramid_swagger-2.8.0/pyramid_swagger/ingest.py`

 * *Files identical despite different names*

### Comparing `pyramid_swagger-2.7.0/pyramid_swagger/load_schema.py` & `pyramid_swagger-2.8.0/pyramid_swagger/load_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 Module to load swagger specs and build efficient data structures for querying
 them during request validation.
 """
 from __future__ import absolute_import
 from __future__ import unicode_literals
 
 from collections import namedtuple
+from copy import deepcopy
 
+import jsonschema
 import simplejson
 from jsonschema import RefResolver
 from jsonschema import validators
 from jsonschema.exceptions import ValidationError
 from jsonschema.validators import Draft3Validator
 from jsonschema.validators import Draft4Validator
+from six import iteritems
 
 from pyramid_swagger.model import partial_path_match
 
 
 EXTENDED_TYPES = {
     'number': (float,),
     'float': (float,),
@@ -191,17 +194,26 @@
 
     def __init__(self, schema, validator):
         self.schema = schema
         self.validator = validator
 
     @classmethod
     def from_schema(cls, schema, resolver, validator_class):
+        type_checker = deepcopy(validator_class.TYPE_CHECKER)
+        type_checker.redefine_many({
+            type_name: lambda checker, value: all(check(value) for check in checks)
+            for type_name, checks in iteritems(EXTENDED_TYPES)
+        })
+        extended_validator_class = jsonschema.validators.extend(
+            validator_class,
+            type_checker=type_checker,
+        )
         return cls(
             schema,
-            validator_class(schema, resolver=resolver, types=EXTENDED_TYPES))
+            extended_validator_class(schema, resolver=resolver))
 
     def validate(self, values):
         """Validate a :class:`dict` of values. If `self.schema` is falsy this
         is a noop.
         """
         if not self.schema or (values is None and not self.schema.get('required', False)):
             return
@@ -258,15 +270,15 @@
 def extract_validatable_type(type_name, models):
     """Returns a jsonschema-compatible typename from the Swagger type.
 
     This is necessary because for our Swagger specs to be compatible with
     swagger-ui, they must not use a $ref to internal models.
 
     :returns: A key-value that jsonschema can validate. Key will be either
-        'type' or '$ref' as is approriate.
+        'type' or '$ref' as is appropriate.
     :rtype: dict
     """
     if type_name in models:
         return {'$ref': type_name}
     else:
         return {'type': type_name}
```

### Comparing `pyramid_swagger-2.7.0/pyramid_swagger/model.py` & `pyramid_swagger-2.8.0/pyramid_swagger/model.py`

 * *Files identical despite different names*

### Comparing `pyramid_swagger-2.7.0/pyramid_swagger/renderer.py` & `pyramid_swagger-2.8.0/pyramid_swagger/renderer.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,18 +31,15 @@
                 op=request.operation,
             )
             return marshal_schema_object(
                 swagger_spec=request.registry.settings['pyramid_swagger.schema20'],
                 schema_object_spec=response_spec['schema'],
                 value=response_object,
             )
-        except MatchingResponseNotFound:
-            # Response specs not found
-            return response_object
-        except SwaggerMappingError:
+        except (MatchingResponseNotFound, SwaggerMappingError, KeyError):
             # marshaling process failed
             return response_object
 
     def _render(self, external_renderer, value, system):
         value = self._marshal_object(system['request'], value)
         return external_renderer(value, system)
```

### Comparing `pyramid_swagger-2.7.0/pyramid_swagger/spec.py` & `pyramid_swagger-2.8.0/pyramid_swagger/spec.py`

 * *Files identical despite different names*

### Comparing `pyramid_swagger-2.7.0/pyramid_swagger/tween.py` & `pyramid_swagger-2.8.0/pyramid_swagger/tween.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,26 +8,29 @@
 import sys
 from collections import namedtuple
 from contextlib import contextmanager
 
 import bravado_core
 import jsonschema.exceptions
 import simplejson
+import six
 from bravado_core.exception import SwaggerMappingError
-from bravado_core.formatter import SwaggerFormat  # noqa
+from bravado_core.exception import SwaggerSecurityValidationError
+from bravado_core.formatter import SwaggerFormat  # noqa: F401
 from bravado_core.operation import Operation
 from bravado_core.request import IncomingRequest
 from bravado_core.request import unmarshal_request
 from bravado_core.response import get_response_spec
 from bravado_core.response import OutgoingResponse
 from pyramid.interfaces import IRoutesMapper
 from pyramid.settings import asbool
 from pyramid.settings import aslist
 
 from pyramid_swagger.exceptions import PathNotFoundError
+from pyramid_swagger.exceptions import RequestAuthenticationError
 from pyramid_swagger.exceptions import RequestValidationError
 from pyramid_swagger.exceptions import ResponseValidationError
 from pyramid_swagger.model import PathNotMatchedError
 
 
 log = logging.getLogger(__name__)
 
@@ -470,16 +473,18 @@
 
 def validation_error(exc_class):
     def decorator(f):
         @functools.wraps(f)
         def _validate(*args, **kwargs):
             try:
                 return f(*args, **kwargs)
-            except (jsonschema.exceptions.ValidationError,
-                    SwaggerMappingError) as exc:
+            except (
+                jsonschema.exceptions.ValidationError,
+                SwaggerMappingError,
+            ) as exc:
                 # This will alter our stack trace slightly, but Pyramid knows
                 # how to render it. And the real value is in the message
                 # anyway.
                 e = exc_class(str(exc), child=exc)
                 e._traceback = sys.exc_info()[2]
                 raise e
 
@@ -576,16 +581,20 @@
     """
     Delegate handling the Swagger concerns of the request to bravado-core.
     Post-invocation, the Swagger request parameters are available as a dict
     named `swagger_data` on the Pyramid request.
 
     :type request: :class:`pyramid.request.Request`
     :type op: :class:`bravado_core.operation.Operation`
+    :raises: RequestValidationError, RequestAuthenticationError
     """
-    request_data = unmarshal_request(request, op)
+    try:
+        request_data = unmarshal_request(request, op)
+    except SwaggerSecurityValidationError as e:
+        six.raise_from(RequestAuthenticationError(e), e)
     return request_data
 
 
 @validation_error(ResponseValidationError)
 def swaggerize_response(response, op):
     """
     Delegate handling the Swagger concerns of the response to bravado-core.
```

### Comparing `pyramid_swagger-2.7.0/pyramid_swagger.egg-info/PKG-INFO` & `pyramid_swagger-2.8.0/pyramid_swagger.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,87 +1,85 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyramid-swagger
-Version: 2.7.0
+Version: 2.8.0
 Summary: Swagger tools for use in pyramid webapps
 Home-page: https://github.com/striglia/pyramid_swagger
 Author: Scott Triglia
 Author-email: scott.triglia@gmail.com
 License: BSD 3-clause
-Description: :PyPI: https://pypi.python.org/pypi/pyramid_swagger
-        :Documentation: http://pyramid-swagger.readthedocs.org/en/latest/
-        :Source: https://github.com/striglia/pyramid_swagger
-        :License: Copyright © 2014 Scott Triglia under the `BSD 3-clause <http://opensource.org/licenses/BSD-3-Clause>`_
-        :Build status:
-            .. image:: https://travis-ci.org/striglia/pyramid_swagger.png?branch=master
-                :target: https://travis-ci.org/striglia/pyramid_swagger?branch=master
-                :alt: Travis CI
-            .. image:: https://ci.appveyor.com/api/projects/status/ufmlmpwy1vj3yjgk/branch/master?svg=true
-                :target: https://ci.appveyor.com/project/striglia/pyramid-swagger
-                :alt: Appveyor (Windows CI)
-        :Current coverage on master:
-            .. image:: https://coveralls.io/repos/striglia/pyramid_swagger/badge.png
-                :target: https://coveralls.io/r/striglia/pyramid_swagger
-        :Persistent chat for questions:
-            .. image:: https://badges.gitter.im/Join%20Chat.svg
-                :alt: Join the chat at https://gitter.im/striglia/pyramid_swagger
-                :target: https://gitter.im/striglia/pyramid_swagger?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
-        
-        
-        pyramid_swagger
-        ===============
-        
-        This project offers convenient tools for using Swagger to define and validate
-        your interfaces in a Pyramid webapp.
-        
-        Full documentation is available at http://pyramid-swagger.readthedocs.org/.
-        
-        
-        How to contribute
-        -----------------
-        
-        #. Fork this repository on Github: https://help.github.com/articles/fork-a-repo/
-        #. Clone your forked repository: https://help.github.com/articles/cloning-a-repository/
-        #. Make a feature branch for your changes:
-        
-            ::
-        
-                git remote add upstream https://github.com/striglia/pyramid_swagger.git
-                git fetch upstream
-                git checkout upstream/master -b my-feature-branch
-        
-        #. Create and activate the virtual environment, this will provide you with all the
-           libraries and tools necessary for pyramid_swagger development:
-        
-            ::
-        
-                make
-                source .activate.sh
-        
-        #. Make sure the test suite works before you start:
-        
-            ::
-        
-                tox -e py27    # Note: use py35 for Python 3.5, see tox.ini for possible values
-        
-        #. Commit patches: http://gitref.org/basic/
-        #. Push to github: ``git pull && git push origin``
-        #. Send a pull request: https://help.github.com/articles/creating-a-pull-request/
-        
-        
-        Running a single test
-        *********************
-        
-        Make sure you have activated the virtual environment (see above).
-        
-        ::
-        
-            py.test -vvv tests/tween_test.py::test_response_properties
-        
 Keywords: pyramid swagger validation
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE
+
+:PyPI: https://pypi.python.org/pypi/pyramid_swagger
+:Documentation: http://pyramid-swagger.readthedocs.org/en/latest/
+:Source: https://github.com/striglia/pyramid_swagger
+:License: Copyright © 2014 Scott Triglia under the `BSD 3-clause <http://opensource.org/licenses/BSD-3-Clause>`_
+:Build status:
+    .. image:: https://travis-ci.org/striglia/pyramid_swagger.png?branch=master
+        :target: https://travis-ci.org/striglia/pyramid_swagger?branch=master
+        :alt: Travis CI
+    .. image:: https://ci.appveyor.com/api/projects/status/ufmlmpwy1vj3yjgk/branch/master?svg=true
+        :target: https://ci.appveyor.com/project/striglia/pyramid-swagger
+        :alt: Appveyor (Windows CI)
+:Current coverage on master:
+    .. image:: https://coveralls.io/repos/striglia/pyramid_swagger/badge.png
+        :target: https://coveralls.io/r/striglia/pyramid_swagger
+:Persistent chat for questions:
+    .. image:: https://badges.gitter.im/Join%20Chat.svg
+        :alt: Join the chat at https://gitter.im/striglia/pyramid_swagger
+        :target: https://gitter.im/striglia/pyramid_swagger?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
+
+
+pyramid_swagger
+===============
+
+This project offers convenient tools for using Swagger to define and validate
+your interfaces in a Pyramid webapp.
+
+Full documentation is available at http://pyramid-swagger.readthedocs.org/.
+
+
+How to contribute
+-----------------
+
+#. Fork this repository on Github: https://help.github.com/articles/fork-a-repo/
+#. Clone your forked repository: https://help.github.com/articles/cloning-a-repository/
+#. Make a feature branch for your changes:
+
+    ::
+
+        git remote add upstream https://github.com/Yelp/pyramid_swagger.git
+        git fetch upstream
+        git checkout upstream/master -b my-feature-branch
+
+#. Create and activate the virtual environment, this will provide you with all the
+   libraries and tools necessary for pyramid_swagger development:
+
+    ::
+
+        make
+        source .activate.sh
+
+#. Make sure the test suite works before you start:
+
+    ::
+
+        tox -e py38    # Note: use py310 for Python 3.10, see tox.ini for possible values
+
+#. Commit patches: http://gitref.org/basic/
+#. Push to github: ``git pull && git push origin``
+#. Send a pull request: https://help.github.com/articles/creating-a-pull-request/
+
+
+Running a single test
+*********************
+
+Make sure you have activated the virtual environment (see above).
+
+::
+
+    py.test -vvv tests/tween_test.py::test_response_properties
```

### Comparing `pyramid_swagger-2.7.0/setup.py` & `pyramid_swagger-2.8.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,22 +30,20 @@
 
     classifiers=[
         'Development Status :: 5 - Production/Stable',
 
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries :: Python Modules',
 
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3.3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.10',
     ],
     keywords='pyramid swagger validation',
     packages=find_packages(exclude=["contrib", "docs", "tests*"]),
     include_package_data=True,
     install_requires=[
         'bravado-core >= 4.8.4',
-        'jsonschema',
+        'jsonschema >= 3.0.0',
         'pyramid',
         'simplejson',
     ],
 )
```

