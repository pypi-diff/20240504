# Comparing `tmp/pyshotgrid-2.0.0.tar.gz` & `tmp/pyshotgrid-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyshotgrid-2.0.0.tar", last modified: Sun Mar  3 14:42:55 2024, max compression
+gzip compressed data, was "pyshotgrid-2.0.2.tar", last modified: Sat May  4 20:47:17 2024, max compression
```

## Comparing `pyshotgrid-2.0.0.tar` & `pyshotgrid-2.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 14:42:55.688011 pyshotgrid-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-03 14:42:50.000000 pyshotgrid-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-03 14:42:50.000000 pyshotgrid-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-03-03 14:42:55.688011 pyshotgrid-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-03-03 14:42:50.000000 pyshotgrid-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 14:42:55.684011 pyshotgrid-2.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-03-03 14:42:50.000000 pyshotgrid-2.0.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 14:42:55.684011 pyshotgrid-2.0.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)   157270 2024-03-03 14:42:50.000000 pyshotgrid-2.0.0/docs/images/default_entity_overview_4k.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-03-03 14:42:50.000000 pyshotgrid-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-03 14:42:55.688011 pyshotgrid-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 14:42:55.684011 pyshotgrid-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 14:42:55.684011 pyshotgrid-2.0.0/src/pyshotgrid/
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-03-03 14:42:50.000000 pyshotgrid-2.0.0/src/pyshotgrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    58928 2024-03-03 14:42:50.000000 pyshotgrid-2.0.0/src/pyshotgrid/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    20138 2024-03-03 14:42:50.000000 pyshotgrid-2.0.0/src/pyshotgrid/sg_default_entities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 14:42:55.684011 pyshotgrid-2.0.0/src/pyshotgrid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-03-03 14:42:55.000000 pyshotgrid-2.0.0/src/pyshotgrid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-03 14:42:55.000000 pyshotgrid-2.0.0/src/pyshotgrid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 14:42:55.000000 pyshotgrid-2.0.0/src/pyshotgrid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-03 14:42:55.000000 pyshotgrid-2.0.0/src/pyshotgrid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-03 14:42:55.000000 pyshotgrid-2.0.0/src/pyshotgrid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:47:17.692384 pyshotgrid-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-04 20:47:12.000000 pyshotgrid-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-04 20:47:12.000000 pyshotgrid-2.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10033 2024-05-04 20:47:17.692384 pyshotgrid-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9052 2024-05-04 20:47:12.000000 pyshotgrid-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:47:17.688384 pyshotgrid-2.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7185 2024-05-04 20:47:12.000000 pyshotgrid-2.0.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:47:17.688384 pyshotgrid-2.0.2/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   157270 2024-05-04 20:47:12.000000 pyshotgrid-2.0.2/docs/images/default_entity_overview_4k.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-04 20:47:12.000000 pyshotgrid-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 20:47:17.692384 pyshotgrid-2.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:47:17.688384 pyshotgrid-2.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:47:17.688384 pyshotgrid-2.0.2/src/pyshotgrid/
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-04 20:47:12.000000 pyshotgrid-2.0.2/src/pyshotgrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59138 2024-05-04 20:47:12.000000 pyshotgrid-2.0.2/src/pyshotgrid/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20138 2024-05-04 20:47:12.000000 pyshotgrid-2.0.2/src/pyshotgrid/sg_default_entities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:47:17.692384 pyshotgrid-2.0.2/src/pyshotgrid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10033 2024-05-04 20:47:17.000000 pyshotgrid-2.0.2/src/pyshotgrid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-04 20:47:17.000000 pyshotgrid-2.0.2/src/pyshotgrid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 20:47:17.000000 pyshotgrid-2.0.2/src/pyshotgrid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-04 20:47:17.000000 pyshotgrid-2.0.2/src/pyshotgrid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 20:47:17.000000 pyshotgrid-2.0.2/src/pyshotgrid.egg-info/top_level.txt
```

### Comparing `pyshotgrid-2.0.0/LICENSE` & `pyshotgrid-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyshotgrid-2.0.0/PKG-INFO` & `pyshotgrid-2.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyshotgrid
-Version: 2.0.0
+Version: 2.0.2
 Summary: A pythonic and object oriented way to talk to Autodesk ShotGrid.
 Author-email: Fabian Geisler <info@fasbue.com>
 License: MIT
 Project-URL: Homepage, https://github.com/fabiangeisler/pyshotgrid
 Project-URL: Documentation, https://fabiangeisler.github.io/pyshotgrid
 Project-URL: Bug Tracker, https://github.com/fabiangeisler/pyshotgrid/issues
 Keywords: shotgrid
@@ -33,15 +33,16 @@
 [![coverage](https://img.shields.io/badge/%20coverage-99%25-%231674b1?style=flat&color=darkgreen)](https://github.com/fabiangeisler/pyshotgrid/actions/workflows/Tests.yml)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 
 `pyshotgrid` is a python package that gives you a pythonic and
-object oriented way to talk to [Autodesk ShotGrid](https://www.autodesk.com/products/shotgrid/overview).
+object oriented way to talk to [Autodesk Flow Production Tracking](https://www.autodesk.com/products/flow-production-tracking/overview)
+(formally known as ShotGrid).
 
 # Quickstart
 
 Install `pyshotgrid` via pip:
 
 ```shell
 pip install pyshotgrid
@@ -155,15 +156,15 @@
 ## I have some custom entity setup in ShotGrid. Can this be reflected in `pyshotgrid`?
 Yes, it can! By default `pyshotgrid` returns any entity as [SGEntity][SGEntity] to provide
 a minimum of functionality in all cases. However you can write your own class
 that inherits from [SGEntity][SGEntity] and register that to `pyshotgrid`. After that,
 `pyshotgrid` will use your custom entity whenever you ask for it. With this method
 you can even overwrite default classes that ship with `pyshotgrid`.
 
-## Why is does `pyshotgrid` not support Python 3.7? [shotgun_api3][shotgun_api3] has support for it.
+## Why does `pyshotgrid` not support Python 3.7? [shotgun_api3][shotgun_api3] has support for it.
 A couple of reasons:
 - [Python 3.7 reached EOL](https://devguide.python.org/versions/) and is no longer maintained.
 - Python 3.7 is soon off the [VFX Reference Platform](https://vfxplatform.com/).
 - The hidden goal of this project is to create a python library that uses the latest
   innovations in the Python world.
   In a nutshell I want to create the simplest setup that gives you:
   - automatic publishing to PyPI
@@ -180,14 +181,18 @@
   keep up the compatibility.
 
 ## Is this an official project from Autodesk?
 No, just a brainchild from me, [Fabian Geisler](https://github.com/fabiangeisler).
 I am a Pipeline Developer based in Berlin.
 Feel free to follow me on GitHub. :)
 
+## How will the rebranding from "ShotGrid" to "Flow Production Tracking" affect this project?
+There will be no code-breaking name changes and `pyshotgrid` will not be rebranded.
+Only docs and docstrings will use the new name.
+
 # Credits
 
 This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and
 the [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage) project template
 (but was heavily modified in the meantime).
 
 [SGEntity]: https://fabiangeisler.github.io/pyshotgrid/modules/core.html#pyshotgrid.core.SGEntity
```

### Comparing `pyshotgrid-2.0.0/README.md` & `pyshotgrid-2.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 [![coverage](https://img.shields.io/badge/%20coverage-99%25-%231674b1?style=flat&color=darkgreen)](https://github.com/fabiangeisler/pyshotgrid/actions/workflows/Tests.yml)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 
 `pyshotgrid` is a python package that gives you a pythonic and
-object oriented way to talk to [Autodesk ShotGrid](https://www.autodesk.com/products/shotgrid/overview).
+object oriented way to talk to [Autodesk Flow Production Tracking](https://www.autodesk.com/products/flow-production-tracking/overview)
+(formally known as ShotGrid).
 
 # Quickstart
 
 Install `pyshotgrid` via pip:
 
 ```shell
 pip install pyshotgrid
@@ -131,15 +132,15 @@
 ## I have some custom entity setup in ShotGrid. Can this be reflected in `pyshotgrid`?
 Yes, it can! By default `pyshotgrid` returns any entity as [SGEntity][SGEntity] to provide
 a minimum of functionality in all cases. However you can write your own class
 that inherits from [SGEntity][SGEntity] and register that to `pyshotgrid`. After that,
 `pyshotgrid` will use your custom entity whenever you ask for it. With this method
 you can even overwrite default classes that ship with `pyshotgrid`.
 
-## Why is does `pyshotgrid` not support Python 3.7? [shotgun_api3][shotgun_api3] has support for it.
+## Why does `pyshotgrid` not support Python 3.7? [shotgun_api3][shotgun_api3] has support for it.
 A couple of reasons:
 - [Python 3.7 reached EOL](https://devguide.python.org/versions/) and is no longer maintained.
 - Python 3.7 is soon off the [VFX Reference Platform](https://vfxplatform.com/).
 - The hidden goal of this project is to create a python library that uses the latest
   innovations in the Python world.
   In a nutshell I want to create the simplest setup that gives you:
   - automatic publishing to PyPI
@@ -156,14 +157,18 @@
   keep up the compatibility.
 
 ## Is this an official project from Autodesk?
 No, just a brainchild from me, [Fabian Geisler](https://github.com/fabiangeisler).
 I am a Pipeline Developer based in Berlin.
 Feel free to follow me on GitHub. :)
 
+## How will the rebranding from "ShotGrid" to "Flow Production Tracking" affect this project?
+There will be no code-breaking name changes and `pyshotgrid` will not be rebranded.
+Only docs and docstrings will use the new name.
+
 # Credits
 
 This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and
 the [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage) project template
 (but was heavily modified in the meantime).
 
 [SGEntity]: https://fabiangeisler.github.io/pyshotgrid/modules/core.html#pyshotgrid.core.SGEntity
```

### Comparing `pyshotgrid-2.0.0/docs/conf.py` & `pyshotgrid-2.0.2/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -184,15 +184,18 @@
     ),
 ]
 
 # -- Options for links to external documentation ------------------------
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
-    "shotgun_api3": ("https://developer.shotgridsoftware.com/python-api/", None),
+    # For some odd reason we need to use "http" and not "https"
+    # for the intersphinx setup of the shotgun_api3. With "https" we run into an SSL
+    # certificate error.
+    "shotgun_api3": ("http://developer.shotgridsoftware.com/python-api/", None),
 }
 
 
 # -- Options for autodoc generation ------------------------
 
 autodoc_default_options = {
     "members": True,
```

### Comparing `pyshotgrid-2.0.0/docs/images/default_entity_overview_4k.jpg` & `pyshotgrid-2.0.2/docs/images/default_entity_overview_4k.jpg`

 * *Files identical despite different names*

### Comparing `pyshotgrid-2.0.0/pyproject.toml` & `pyshotgrid-2.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools_scm]
+
 [project]
 name = "pyshotgrid"
 authors = [
   { name="Fabian Geisler", email="info@fasbue.com" },
 ]
 description = "A pythonic and object oriented way to talk to Autodesk ShotGrid."
 dependencies = ["shotgun-api3>=3.4.0"]
@@ -80,15 +82,15 @@
     "shotgun_api3.*",
     "tank_vendor.*",
 ]
 ignore_missing_imports = true
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "2.0.0"
+version = "2.0.2"
 tag_format = "v$version"
 update_changelog_on_bump = true
 annotated_tag = true
 version_files = [
     "src/pyshotgrid/__init__.py:VERSION",
 ]
```

### Comparing `pyshotgrid-2.0.0/src/pyshotgrid/__init__.py` & `pyshotgrid-2.0.2/src/pyshotgrid/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     new_entity,  # noqa: F401
     new_site,  # noqa: F401
     register_pysg_class,
     register_sg_site_class,  # noqa: F401
 )
 
 #: The pyshotgrid version number as string
-VERSION = "2.0.0"
+VERSION = "2.0.2"
 
 # Register default pysg plugins
 register_pysg_class(sde.SGProject)
 register_pysg_class(sde.SGShot)
 register_pysg_class(sde.SGAsset)
 register_pysg_class(sde.SGTask)
 register_pysg_class(sde.SGPublishedFile)
```

### Comparing `pyshotgrid-2.0.0/src/pyshotgrid/core.py` & `pyshotgrid-2.0.2/src/pyshotgrid/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,31 @@
 import http.cookiejar
 import os
 import sys
 import urllib.parse
 import urllib.request
 from typing import Any, Optional, Type, Union
 
+__SG_CLASSES = []
+try:
+    import tank_vendor
+    import tank_vendor.shotgun_api3 as shotgun_api3
+    import tank_vendor.shotgun_api3.lib.mockgun
+
+    __SG_CLASSES += [tank_vendor.shotgun_api3.Shotgun, tank_vendor.shotgun_api3.lib.mockgun.Shotgun]
+except ImportError:
+    pass
+
 try:
     import shotgun_api3
+    import shotgun_api3.lib.mockgun
+
+    __SG_CLASSES += [shotgun_api3.Shotgun, shotgun_api3.lib.mockgun.Shotgun]
 except ImportError:
-    import tank_vendor.shotgun_api3 as shotgun_api3
+    pass
 
 
 class SGEntity:
     """
     An instance of this class represents a single entity in ShotGrid.
 
     .. Note::
@@ -525,15 +538,15 @@
         sg_versions = self._sg.find(
             "Version",
             sg_filter,
             ["entity", "created_at"],
         )
 
         # Sort one more time by name.
-        sg_versions.sort(key=lambda pub: pub["entity"]["id"])
+        sg_versions.sort(key=lambda pub: (pub["entity"] or {}).get("id", 10000000000))
         # sort them by date and than by version_number which sorts the latest publish to the
         # last position.
         sg_versions.sort(key=lambda pub: pub["created_at"], reverse=True)
 
         if latest:
             tmp_list = []
             last_entity: dict[str, Any] = {}
@@ -1366,20 +1379,19 @@
         # shotgun_api3 and tk-core are installed at the same time.
         # In this case there are 4 different Shotgun classes that could
         # work with pyshotgrid:
         #   - shotgun_api3.Shotgun
         #   - shotgun_api3.lib.mockgun.Shotgun
         #   - tank_vendor.shotgun_api3.Shotgun
         #   - tank_vendor.shotgun_api3.lib.mockgun.Shotgun
-        # pyshotgrid will load either shotgun_api3 or tk-core (tank_vendor.shotgun_api3)
-        # and therefore we cannot use "isinstance" here ,since the user might
-        # pass in a Shotgun class from the other library. We just check
-        # if the passed in object is a instance of a class named "Shotgun".
-        if args[0].__class__.__name__ == "Shotgun":
-            sg = args[0]
+        # These are collected during import on top of the file and are now compared against.
+        for sg_class in __SG_CLASSES:
+            if isinstance(args[0], sg_class):
+                sg = args[0]
+                break
         else:
             sg = shotgun_api3.Shotgun(*args)
     else:
         sg = shotgun_api3.Shotgun(**kwargs)
     return __SG_SITE_CLASS(sg)
```

### Comparing `pyshotgrid-2.0.0/src/pyshotgrid/sg_default_entities.py` & `pyshotgrid-2.0.2/src/pyshotgrid/sg_default_entities.py`

 * *Files identical despite different names*

### Comparing `pyshotgrid-2.0.0/src/pyshotgrid.egg-info/PKG-INFO` & `pyshotgrid-2.0.2/src/pyshotgrid.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyshotgrid
-Version: 2.0.0
+Version: 2.0.2
 Summary: A pythonic and object oriented way to talk to Autodesk ShotGrid.
 Author-email: Fabian Geisler <info@fasbue.com>
 License: MIT
 Project-URL: Homepage, https://github.com/fabiangeisler/pyshotgrid
 Project-URL: Documentation, https://fabiangeisler.github.io/pyshotgrid
 Project-URL: Bug Tracker, https://github.com/fabiangeisler/pyshotgrid/issues
 Keywords: shotgrid
@@ -33,15 +33,16 @@
 [![coverage](https://img.shields.io/badge/%20coverage-99%25-%231674b1?style=flat&color=darkgreen)](https://github.com/fabiangeisler/pyshotgrid/actions/workflows/Tests.yml)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 
 `pyshotgrid` is a python package that gives you a pythonic and
-object oriented way to talk to [Autodesk ShotGrid](https://www.autodesk.com/products/shotgrid/overview).
+object oriented way to talk to [Autodesk Flow Production Tracking](https://www.autodesk.com/products/flow-production-tracking/overview)
+(formally known as ShotGrid).
 
 # Quickstart
 
 Install `pyshotgrid` via pip:
 
 ```shell
 pip install pyshotgrid
@@ -155,15 +156,15 @@
 ## I have some custom entity setup in ShotGrid. Can this be reflected in `pyshotgrid`?
 Yes, it can! By default `pyshotgrid` returns any entity as [SGEntity][SGEntity] to provide
 a minimum of functionality in all cases. However you can write your own class
 that inherits from [SGEntity][SGEntity] and register that to `pyshotgrid`. After that,
 `pyshotgrid` will use your custom entity whenever you ask for it. With this method
 you can even overwrite default classes that ship with `pyshotgrid`.
 
-## Why is does `pyshotgrid` not support Python 3.7? [shotgun_api3][shotgun_api3] has support for it.
+## Why does `pyshotgrid` not support Python 3.7? [shotgun_api3][shotgun_api3] has support for it.
 A couple of reasons:
 - [Python 3.7 reached EOL](https://devguide.python.org/versions/) and is no longer maintained.
 - Python 3.7 is soon off the [VFX Reference Platform](https://vfxplatform.com/).
 - The hidden goal of this project is to create a python library that uses the latest
   innovations in the Python world.
   In a nutshell I want to create the simplest setup that gives you:
   - automatic publishing to PyPI
@@ -180,14 +181,18 @@
   keep up the compatibility.
 
 ## Is this an official project from Autodesk?
 No, just a brainchild from me, [Fabian Geisler](https://github.com/fabiangeisler).
 I am a Pipeline Developer based in Berlin.
 Feel free to follow me on GitHub. :)
 
+## How will the rebranding from "ShotGrid" to "Flow Production Tracking" affect this project?
+There will be no code-breaking name changes and `pyshotgrid` will not be rebranded.
+Only docs and docstrings will use the new name.
+
 # Credits
 
 This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and
 the [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage) project template
 (but was heavily modified in the meantime).
 
 [SGEntity]: https://fabiangeisler.github.io/pyshotgrid/modules/core.html#pyshotgrid.core.SGEntity
```

