# Comparing `tmp/glue_utils-0.2.1rc4.tar.gz` & `tmp/glue_utils-0.2.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glue_utils-0.2.1rc4.tar", max compression
+gzip compressed data, was "glue_utils-0.2.2b0.tar", max compression
```

## Comparing `glue_utils-0.2.1rc4.tar` & `glue_utils-0.2.2b0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2024-03-06 15:16:48.910706 glue_utils-0.2.1rc4/LICENSE
--rw-r--r--   0        0        0     1138 2024-03-07 09:36:58.526889 glue_utils-0.2.1rc4/README.md
--rw-r--r--   0        0        0     3315 2024-05-03 11:12:53.179892 glue_utils-0.2.1rc4/pyproject.toml
--rw-r--r--   0        0        0       99 2024-05-03 11:12:59.063439 glue_utils-0.2.1rc4/src/glue_utils/__init__.py
--rw-r--r--   0        0        0       68 2024-05-03 09:05:30.885798 glue_utils-0.2.1rc4/src/glue_utils/glueetl/__init__.py
--rw-r--r--   0        0        0     3114 2024-05-03 11:12:21.569002 glue_utils-0.2.1rc4/src/glue_utils/glueetl/job.py
--rw-r--r--   0        0        0      794 2024-05-03 09:02:47.986701 glue_utils-0.2.1rc4/src/glue_utils/options.py
--rw-r--r--   0        0        0        0 2024-05-03 09:02:47.986990 glue_utils-0.2.1rc4/src/glue_utils/py.typed
--rw-r--r--   0        0        0     2204 1970-01-01 00:00:00.000000 glue_utils-0.2.1rc4/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-03-06 15:16:48.910706 glue_utils-0.2.2b0/LICENSE
+-rw-r--r--   0        0        0     1138 2024-03-07 09:36:58.526889 glue_utils-0.2.2b0/README.md
+-rw-r--r--   0        0        0     3298 2024-05-04 14:01:12.346140 glue_utils-0.2.2b0/pyproject.toml
+-rw-r--r--   0        0        0       98 2024-05-04 14:01:24.443348 glue_utils-0.2.2b0/src/glue_utils/__init__.py
+-rw-r--r--   0        0        0       68 2024-05-03 09:05:30.885798 glue_utils-0.2.2b0/src/glue_utils/glueetl/__init__.py
+-rw-r--r--   0        0        0     3126 2024-05-04 13:59:47.431646 glue_utils-0.2.2b0/src/glue_utils/glueetl/job.py
+-rw-r--r--   0        0        0      830 2024-05-04 13:59:47.431943 glue_utils-0.2.2b0/src/glue_utils/options.py
+-rw-r--r--   0        0        0        0 2024-05-03 09:02:47.986990 glue_utils-0.2.2b0/src/glue_utils/py.typed
+-rw-r--r--   0        0        0     2252 1970-01-01 00:00:00.000000 glue_utils-0.2.2b0/PKG-INFO
```

### Comparing `glue_utils-0.2.1rc4/LICENSE` & `glue_utils-0.2.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `glue_utils-0.2.1rc4/README.md` & `glue_utils-0.2.2b0/README.md`

 * *Files identical despite different names*

### Comparing `glue_utils-0.2.1rc4/pyproject.toml` & `glue_utils-0.2.2b0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glue-utils"
-version = "0.2.1rc4"
+version = "0.2.2b0"
 # Uncomment this when dependabot has finally been updated to it is 
 # supported by dependabot.
 # package-mode = true
 description = "Reusable utilities for working with Glue PySpark jobs"
 authors = ["Noel Llevares <dashmug@gmail.com>"]
 license = "MIT"
 readme = "README.md"
@@ -26,22 +26,22 @@
     "spark",
     "etl",
     "data",
     "data-engineering",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 
 [tool.poetry.group.dev.dependencies]
 pytest-randomly = "^3.15.0"
 pytest-cov = "^5.0.0"
-ruff = "^0.4.2"
 mypy = "^1.10.0"
 pytest = "^8.2.0"
+ruff = "^0.4.3"
 
 [tool.poetry.group.local.dependencies]
 # The "local" dependency group refers to dependencies that already 
 # exist in AWS Glue's runtime. We don't need to install these in the
 # container. We only need them for local (non-container) development to 
 # aid the IDE in providing code completion and type checking.
 # 
@@ -55,42 +55,42 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 line-length = 88
 output-format = "full"
 respect-gitignore = true
-target-version = "py310"
+target-version = "py39"
 
 [tool.ruff.lint]
 select = ["ALL"]
 ignore = [
     "D203",
     "D213",
     # Conflicts with ruff format
     "COM812",
     "ISC001",
     # missing-type-self
     "ANN101",
     # missing-type-cls
     "ANN102",
 ]
-exclude = ["snapshots", ".venv"]
+exclude = [".venv"]
 # # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
 [tool.ruff.lint.mccabe]
 max-complexity = 5
 
 [tool.ruff.lint.per-file-ignores]
 "test/**" = ["S101", "ANN", "ARG001", "ARG002", "PLR2004", "PT", "PD", "D"]
 
 [tool.mypy]
 files = "**/*.py"
-python_version = "3.10"
+python_version = "3.9"
 show_error_codes = true
 pretty = true
 strict = true
 ignore_missing_imports = true
 implicit_reexport = true
 explicit_package_bases = true
```

### Comparing `glue_utils-0.2.1rc4/src/glue_utils/glueetl/job.py` & `glue_utils-0.2.2b0/src/glue_utils/glueetl/job.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,57 @@
 """Module providing the GlueETLJob class for handling Glue ETL jobs."""
 
+from __future__ import annotations
+
 import sys
-from collections.abc import Generator
 from contextlib import contextmanager
 from dataclasses import fields
-from typing import Generic, cast, overload
+from typing import TYPE_CHECKING, Generic, cast, overload
 
 from awsglue.context import GlueContext
 from awsglue.job import Job
 from awsglue.utils import getResolvedOptions
 from pyspark import SparkConf, SparkContext
-from pyspark.sql import SparkSession
 from typing_extensions import TypeVar
 
 from glue_utils import BaseOptions
 
+if TYPE_CHECKING:
+    from collections.abc import Generator
+
+    from pyspark.sql import SparkSession
+
 T = TypeVar("T", bound=BaseOptions, default=BaseOptions)
 
 
 class GlueETLJob(Generic[T]):
     """Class that handles the boilerplate setup for Glue ETL jobs."""
 
     name: str
     options: T
     sc: SparkContext
     spark: SparkSession
     glue_context: GlueContext
 
     @overload
     def __init__(
-        self: "GlueETLJob[BaseOptions]",
+        self: GlueETLJob[BaseOptions],
     ) -> None: ...
 
     @overload
     def __init__(
-        self: "GlueETLJob[T]",
+        self: GlueETLJob[T],
         *,
         options_cls: type[T],
     ) -> None: ...
 
     def __init__(
         self,
         *,
-        options_cls: type[T] | type[BaseOptions] = BaseOptions,
+        options_cls: type[T | BaseOptions] = BaseOptions,
     ) -> None:
         """Initialize the GlueETLJob.
 
         Parameters
         ----------
         options_cls, optional
             Has to be a subclass of BaseOptions, by default BaseOptions
@@ -64,15 +69,14 @@
         job_options = getResolvedOptions(sys.argv, params)
 
         self.options = cast(T, options_cls.from_resolved_options(job_options))
 
         self.name = job_options.get("JOB_NAME", "glueetl-job")
 
         self.sc = self.create_spark_context()
-        self.sc.setLogLevel("DEBUG")
         self.glue_context = self.create_glue_context()
         self.spark = self.glue_context.spark_session
 
         self._job = Job(self.glue_context)
         self._job.init(self.name, job_options)
 
     def create_spark_context(self) -> SparkContext:
@@ -85,15 +89,15 @@
         return SparkContext.getOrCreate(spark_conf)
 
     def create_glue_context(self) -> GlueContext:
         """Create a GlueContext.
 
         Override this method to customize the GlueContext creation.
         """
-        return GlueContext(self.create_spark_context())
+        return GlueContext(self.sc)
 
     @contextmanager
     def managed_glue_context(
         self,
         *,
         commit: bool = True,
     ) -> Generator[GlueContext, None, None]:
```

### Comparing `glue_utils-0.2.1rc4/src/glue_utils/options.py` & `glue_utils-0.2.2b0/src/glue_utils/options.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Module for conveniently parsing options resolved from command-line arguments."""
 
+from __future__ import annotations
+
 from dataclasses import dataclass, fields
 from typing import Any
 
 from typing_extensions import Self
 
 
 @dataclass(frozen=True)
```

### Comparing `glue_utils-0.2.1rc4/PKG-INFO` & `glue_utils-0.2.2b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: glue-utils
-Version: 0.2.1rc4
+Version: 0.2.2b0
 Summary: Reusable utilities for working with Glue PySpark jobs
 Home-page: https://github.com/dashmug/glue-utils
 License: MIT
 Keywords: aws,glue,pyspark,spark,etl,data,data-engineering
 Author: Noel Llevares
 Author-email: dashmug@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Documentation, https://github.com/dashmug/glue-utils/wiki
 Project-URL: Repository, https://github.com/dashmug/glue-utils/issues
```

