# Comparing `tmp/mlforge-0.1.3a0.tar.gz` & `tmp/mlforge-0.1.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlforge-0.1.3a0.tar", last modified: Mon Apr 29 07:52:35 2024, max compression
+gzip compressed data, was "mlforge-0.1.4a0.tar", last modified: Sat May  4 09:43:21 2024, max compression
```

## Comparing `mlforge-0.1.3a0.tar` & `mlforge-0.1.4a0.tar`

### file list

```diff
@@ -1,28 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:52:35.464708 mlforge-0.1.3a0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-29 07:52:35.464708 mlforge-0.1.3a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:52:35.460708 mlforge-0.1.3a0/mlforge/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/mlforge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/mlforge/logconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    34254 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/mlforge/mlforge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/mlforge/progbar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:52:35.464708 mlforge-0.1.3a0/mlforge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-29 07:52:35.000000 mlforge-0.1.3a0/mlforge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-29 07:52:35.000000 mlforge-0.1.3a0/mlforge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 07:52:35.000000 mlforge-0.1.3a0/mlforge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 07:52:35.000000 mlforge-0.1.3a0/mlforge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 07:52:35.464708 mlforge-0.1.3a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:52:35.464708 mlforge-0.1.3a0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/tests/test_add_stages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/tests/test_build_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/tests/test_callable_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/tests/test_from_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/tests/test_from_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/tests/test_get_method_signature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/tests/test_get_step_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/tests/test_parse_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/tests/test_pbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-29 07:52:29.000000 mlforge-0.1.3a0/tests/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:43:21.941566 mlforge-0.1.4a0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-05-04 09:43:21.941566 mlforge-0.1.4a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6133 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:43:21.941566 mlforge-0.1.4a0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/examples/example1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/examples/example2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/examples/example3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/examples/example4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/examples/example5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/examples/sample_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:43:21.941566 mlforge-0.1.4a0/mlforge/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/mlforge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/mlforge/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/mlforge/logconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34441 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/mlforge/mlforge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/mlforge/progbar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:43:21.941566 mlforge-0.1.4a0/mlforge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-05-04 09:43:21.000000 mlforge-0.1.4a0/mlforge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-04 09:43:21.000000 mlforge-0.1.4a0/mlforge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 09:43:21.000000 mlforge-0.1.4a0/mlforge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-04 09:43:21.000000 mlforge-0.1.4a0/mlforge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 09:43:21.941566 mlforge-0.1.4a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-04 09:43:15.000000 mlforge-0.1.4a0/setup.py
```

### Comparing `mlforge-0.1.3a0/LICENSE.txt` & `mlforge-0.1.4a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mlforge-0.1.3a0/PKG-INFO` & `mlforge-0.1.4a0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,12 @@
-Metadata-Version: 2.1
-Name: mlforge
-Version: 0.1.3a0
-Summary: A package to design and run sequential ML pipelines
-Home-page: https://github.com/renero/mlforge
-Author: J. Renero
-Author-email: jesus.renero@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 MLForge
 =======
 
+|build-status| |coverage| |wheel| |documentation|
+
 **MLForge** is a simple package to write simple pipelines of calls (to
 methods, classes, …). You can access the documentation at
 `ReadTheDocs <https://mlforge.readthedocs.io/en/latest/>`__
 
 It surges from the need to execute several things in a row, and to be
 able to easily add or remove steps in the pipeline.
 
@@ -206,7 +194,24 @@
 -----
 
 -  Add a way to add a step at a specific position
 -  Add a way to remove a step
 -  Add a way to replace a step
 -  Add a way to add a step before or after another step
 -  And many other things…
+
+
+.. |build-status| image:: https://github.com/renero/mlforge/actions/workflows/python-test.yml/badge.svg
+    :target: https://github.com/renero/mlforge/actions/workflows/python-test.yml
+    :alt: Tests Status
+
+.. |coverage| image:: https://codecov.io/gh/renero/mlforge/graph/badge.svg?token=HRZAE9GS0I
+    :target: https://codecov.io/gh/renero/mlforge
+    :alt: Code Coverage
+
+.. |wheel| image:: https://github.com/renero/mlforge/actions/workflows/python-publish.yml/badge.svg
+    :target: https://pypi.org/project/mlforge/
+    :alt: PyPi Publish Status
+
+.. |documentation| image:: https://readthedocs.org/projects/mlforge/badge/?version=latest
+    :target: https://mlforge.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
```

### Comparing `mlforge-0.1.3a0/mlforge/logconfig.py` & `mlforge-0.1.4a0/mlforge/logconfig.py`

 * *Files identical despite different names*

### Comparing `mlforge-0.1.3a0/mlforge/mlforge.py` & `mlforge-0.1.4a0/mlforge/mlforge.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 """
 
 Pipeline class to define and run several execution steps.
 @author: Jesús Renero
 
 """
+
+# pylint: disable=E1101:no-member, W0201:attribute-defined-outside-init, W0511:fixme
+# pylint: disable=C0103:invalid-name, R0902:too-many-instance-attributes
+# pylint: disable=C0116:missing-function-docstring, C0115:missing-class-docstring
+# pylint: disable=R0913:too-many-arguments, R0903:too-few-public-methods
+# pylint: disable=R0914:too-many-locals, R0915:too-many-statements
+# pylint: disable=W0106:expression-not-assigned, R1702:too-many-branches
+# pylint: disable=W0212:protected-access
+
 import importlib
 import inspect
 import logging
 import time
 import types
 import typing
 from dataclasses import asdict, dataclass
@@ -19,22 +28,14 @@
 from rich import print as rp
 from rich.columns import Columns
 from rich.table import Table
 
 from mlforge.logconfig import LogConfig
 from mlforge.progbar import ProgBar
 
-# pylint: disable=E1101:no-member, W0201:attribute-defined-outside-init, W0511:fixme
-# pylint: disable=C0103:invalid-name, R0902:too-many-instance-attributes
-# pylint: disable=C0116:missing-function-docstring, C0115:missing-class-docstring
-# pylint: disable=R0913:too-many-arguments, R0903:too-few-public-methods
-# pylint: disable=R0914:too-many-locals, R0915:too-many-statements
-# pylint: disable=W0106:expression-not-assigned, R1702:too-many-branches
-# pylint: disable=W0212:protected-access
-
 
 @dataclass
 class Stage:
     _num: int = None
     _id: str = None
     attribute_name: str = None
     method_name: str = None
@@ -67,14 +68,16 @@
         Name of the logger.
     log_level: str
         Level of the logger.
     log_fname: str
         Name of the log file.
     prog_bar: bool
         Flag indicating whether to display the progress bar.
+    description: str
+        Description of the pipeline to be displayed by the progbar.
     subtask: bool
         Indicates whether to show a secondary progress bar to show the progress of
         each stage. This flag requires that each method in the pipeline will call
         the `ProgBar` object to update the progress bar.
     verbose: bool
         Flag indicating whether to display verbose output.
     silent: bool
@@ -84,28 +87,30 @@
     def __init__(
             self,
             host: type = None,
             log_name: str = None,
             log_level: str = "info",
             log_fname: str = None,
             prog_bar: bool = True,
+            description: str = None,
             subtask: bool = False,
             verbose: bool = False,
             silent: bool = False):
 
         # First thing is knowing who is calling the pipeline.
         caller = inspect.stack()[1]
         self.caller_module = caller.frame.f_globals['__name__']
         self.caller_filename = caller[0].f_code.co_filename
         self.caller_filename = self.caller_filename.split('/')[-1]
 
         self.host = host
         self.pipeline = []
         self.verbose = verbose
         self.prog_bar = prog_bar
+        self.description = description
         self.subtask = subtask
         self.silent = silent
         self.attributes_ = {}
         self.objects_ = {'host': self.host}
         self.pbar = None
         self.run_ = False
 
@@ -228,15 +233,15 @@
             In the case of a tuple, the value returned by the function or the fit
             method of the class will be assigned to the attribute of the host object.
             In the case of a function or method name, the value returned by the
             function or the fit method of the class will not be assigned to any
             attribute of the host object.
         """
         assert self.pipeline, "Pipeline is empty. No steps to run."
-        self._pbar_create()
+        self._pbar_create(name=self.description)
         self._m(f"RUN pipeline with {len(self.pipeline)} steps")
 
         self.logger.info('Pipeline execution started')
         for stage in self.pipeline:
             self._m(f"  > Step #{stage._num:>03d}({stage._id})\n"
                     f"    > attribute_name: {stage.attribute_name}\n"
                     f"    > method_name: {stage.method_name}\n"
```

### Comparing `mlforge-0.1.3a0/mlforge/progbar.py` & `mlforge-0.1.4a0/mlforge/progbar.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,26 +42,31 @@
     Implements a progress bar for the mlforge package.
     """
 
     def __init__(self, name: str = None, num_steps: int = None, subtask: bool = False):
         self.num_steps = num_steps
         self.sub_task = subtask
         self.progress = Progress(
+            TextColumn("[progress.description]{task.description:<20s}"),
+            TextColumn("•"),
             TextColumn("[progress.percentage]{task.percentage:>3.0f}%"),
             BarColumn(),
             MofNCompleteColumn(),
             TextColumn("•"),
             TimeElapsedColumn(),
             TextColumn("•"),
             TimeRemainingColumn(),
         )
-        pb_name = name if name else "Progress..."
+        pb_name = name if name else "Progress"
+        pb_name = pb_name[:20]+'.' if len(pb_name) > 20 else pb_name
+        if len(pb_name) < 20:
+            pb_name = pb_name + "." * (20 - len(pb_name))
         self.main_task = self.progress.add_task(pb_name, total=num_steps)
         if self.sub_task:
-            self.sub_task = self.progress.add_task('subtask', start=False)
+            self.sub_task = self.progress.add_task(" ↳ Subtask(s)", start=False)
 
     def start_subtask(self, num_steps: int):
         """
         Starts a subtask with the specified number of steps.
 
         Args:
             num_steps (int): The total number of steps in the subtask.
```

### Comparing `mlforge-0.1.3a0/mlforge.egg-info/PKG-INFO` & `mlforge-0.1.4a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: mlforge
-Version: 0.1.3a0
+Version: 0.1.4a0
 Summary: A package to design and run sequential ML pipelines
 Home-page: https://github.com/renero/mlforge
 Author: J. Renero
 Author-email: jesus.renero@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 MLForge
 =======
 
+|build-status| |coverage| |wheel| |documentation|
+
 **MLForge** is a simple package to write simple pipelines of calls (to
 methods, classes, …). You can access the documentation at
 `ReadTheDocs <https://mlforge.readthedocs.io/en/latest/>`__
 
 It surges from the need to execute several things in a row, and to be
 able to easily add or remove steps in the pipeline.
 
@@ -206,7 +208,24 @@
 -----
 
 -  Add a way to add a step at a specific position
 -  Add a way to remove a step
 -  Add a way to replace a step
 -  Add a way to add a step before or after another step
 -  And many other things…
+
+
+.. |build-status| image:: https://github.com/renero/mlforge/actions/workflows/python-test.yml/badge.svg
+    :target: https://github.com/renero/mlforge/actions/workflows/python-test.yml
+    :alt: Tests Status
+
+.. |coverage| image:: https://codecov.io/gh/renero/mlforge/graph/badge.svg?token=HRZAE9GS0I
+    :target: https://codecov.io/gh/renero/mlforge
+    :alt: Code Coverage
+
+.. |wheel| image:: https://github.com/renero/mlforge/actions/workflows/python-publish.yml/badge.svg
+    :target: https://pypi.org/project/mlforge/
+    :alt: PyPi Publish Status
+
+.. |documentation| image:: https://readthedocs.org/projects/mlforge/badge/?version=latest
+    :target: https://mlforge.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
```

