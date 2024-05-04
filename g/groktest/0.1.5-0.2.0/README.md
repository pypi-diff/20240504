# Comparing `tmp/groktest-0.1.5.tar.gz` & `tmp/groktest-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groktest-0.1.5.tar", last modified: Sat Dec  9 18:05:27 2023, max compression
+gzip compressed data, was "groktest-0.2.0.tar", last modified: Sat May  4 18:40:03 2024, max compression
```

## Comparing `groktest-0.1.5.tar` & `groktest-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxr-x   0 garrett   (1000) garrett   (1000)        0 2023-12-09 18:05:27.722459 groktest-0.1.5/
--rw-rw-r--   0 garrett   (1000) garrett   (1000)    11358 2023-08-16 19:33:04.000000 groktest-0.1.5/LICENSE
--rw-r--r--   0 garrett   (1000) garrett   (1000)     5902 2023-12-09 18:05:27.722459 groktest-0.1.5/PKG-INFO
--rw-rw-r--   0 garrett   (1000) garrett   (1000)     5370 2023-08-20 20:45:54.000000 groktest-0.1.5/README.md
-drwxrwxr-x   0 garrett   (1000) garrett   (1000)        0 2023-12-09 18:05:27.722459 groktest-0.1.5/groktest/
--rw-rw-r--   0 garrett   (1000) garrett   (1000)    41058 2023-12-09 18:04:01.000000 groktest-0.1.5/groktest/__init__.py
--rw-rw-r--   0 garrett   (1000) garrett   (1000)     5931 2023-12-08 15:28:19.000000 groktest-0.1.5/groktest/__main__.py
--rw-rw-r--   0 garrett   (1000) garrett   (1000)    35153 2023-08-19 17:41:28.000000 groktest-0.1.5/groktest/_vendor_parse.py
-drwxrwxr-x   0 garrett   (1000) garrett   (1000)        0 2023-12-09 18:05:27.722459 groktest-0.1.5/groktest/_vendor_tomli/
--rw-rw-r--   0 garrett   (1000) garrett   (1000)      396 2023-08-21 00:19:44.000000 groktest-0.1.5/groktest/_vendor_tomli/__init__.py
--rw-rw-r--   0 garrett   (1000) garrett   (1000)    22633 2023-08-21 00:20:32.000000 groktest-0.1.5/groktest/_vendor_tomli/_parser.py
--rw-rw-r--   0 garrett   (1000) garrett   (1000)     2943 2023-08-21 00:19:44.000000 groktest-0.1.5/groktest/_vendor_tomli/_re.py
--rw-rw-r--   0 garrett   (1000) garrett   (1000)      254 2023-08-21 00:19:44.000000 groktest-0.1.5/groktest/_vendor_tomli/_types.py
--rw-rw-r--   0 garrett   (1000) garrett   (1000)       26 2023-08-21 00:19:44.000000 groktest-0.1.5/groktest/_vendor_tomli/py.typed
--rw-rw-r--   0 garrett   (1000) garrett   (1000)     6321 2023-09-07 23:45:22.000000 groktest-0.1.5/groktest/nushell.py
--rw-rw-r--   0 garrett   (1000) garrett   (1000)    14189 2023-12-09 17:27:34.000000 groktest-0.1.5/groktest/python.py
-drwxrwxr-x   0 garrett   (1000) garrett   (1000)        0 2023-12-09 18:05:27.722459 groktest-0.1.5/groktest.egg-info/
--rw-r--r--   0 garrett   (1000) garrett   (1000)     5902 2023-12-09 18:05:27.000000 groktest-0.1.5/groktest.egg-info/PKG-INFO
--rw-rw-r--   0 garrett   (1000) garrett   (1000)      466 2023-12-09 18:05:27.000000 groktest-0.1.5/groktest.egg-info/SOURCES.txt
--rw-rw-r--   0 garrett   (1000) garrett   (1000)        1 2023-12-09 18:05:27.000000 groktest-0.1.5/groktest.egg-info/dependency_links.txt
--rw-rw-r--   0 garrett   (1000) garrett   (1000)       52 2023-12-09 18:05:27.000000 groktest-0.1.5/groktest.egg-info/entry_points.txt
--rw-rw-r--   0 garrett   (1000) garrett   (1000)        9 2023-12-09 18:05:27.000000 groktest-0.1.5/groktest.egg-info/top_level.txt
--rw-rw-r--   0 garrett   (1000) garrett   (1000)      931 2023-12-09 18:03:46.000000 groktest-0.1.5/pyproject.toml
--rw-rw-r--   0 garrett   (1000) garrett   (1000)       38 2023-12-09 18:05:27.722459 groktest-0.1.5/setup.cfg
+drwxrwxr-x   0 garrett   (1000) garrett   (1000)        0 2024-05-04 18:40:03.063159 groktest-0.2.0/
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)    11358 2023-08-16 19:33:04.000000 groktest-0.2.0/LICENSE
+-rw-r--r--   0 garrett   (1000) garrett   (1000)     5925 2024-05-04 18:40:03.063159 groktest-0.2.0/PKG-INFO
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     5371 2024-05-02 20:50:08.000000 groktest-0.2.0/README.md
+drwxrwxr-x   0 garrett   (1000) garrett   (1000)        0 2024-05-04 18:40:03.063159 groktest-0.2.0/groktest/
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)    45386 2024-05-03 23:30:21.000000 groktest-0.2.0/groktest/__init__.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)    12077 2024-05-03 23:49:11.000000 groktest-0.2.0/groktest/__main__.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)      472 2024-05-02 16:26:30.000000 groktest-0.2.0/groktest/_test_util.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)    35153 2023-08-19 17:41:28.000000 groktest-0.2.0/groktest/_vendor_parse.py
+drwxrwxr-x   0 garrett   (1000) garrett   (1000)        0 2024-05-04 18:40:03.063159 groktest-0.2.0/groktest/_vendor_tomli/
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)      396 2023-08-21 00:19:44.000000 groktest-0.2.0/groktest/_vendor_tomli/__init__.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)    22658 2024-05-02 20:19:20.000000 groktest-0.2.0/groktest/_vendor_tomli/_parser.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     2956 2024-05-02 20:19:09.000000 groktest-0.2.0/groktest/_vendor_tomli/_re.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)      254 2023-08-21 00:19:44.000000 groktest-0.2.0/groktest/_vendor_tomli/_types.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)       26 2023-08-21 00:19:44.000000 groktest-0.2.0/groktest/_vendor_tomli/py.typed
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)     6327 2024-05-02 20:18:57.000000 groktest-0.2.0/groktest/nushell.py
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)    16056 2024-05-03 23:20:12.000000 groktest-0.2.0/groktest/python.py
+drwxrwxr-x   0 garrett   (1000) garrett   (1000)        0 2024-05-04 18:40:03.063159 groktest-0.2.0/groktest.egg-info/
+-rw-r--r--   0 garrett   (1000) garrett   (1000)     5925 2024-05-04 18:40:03.000000 groktest-0.2.0/groktest.egg-info/PKG-INFO
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)      520 2024-05-04 18:40:03.000000 groktest-0.2.0/groktest.egg-info/SOURCES.txt
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)        1 2024-05-04 18:40:03.000000 groktest-0.2.0/groktest.egg-info/dependency_links.txt
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)       52 2024-05-04 18:40:03.000000 groktest-0.2.0/groktest.egg-info/entry_points.txt
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)        7 2024-05-04 18:40:03.000000 groktest-0.2.0/groktest.egg-info/requires.txt
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)        9 2024-05-04 18:40:03.000000 groktest-0.2.0/groktest.egg-info/top_level.txt
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)      955 2024-05-03 14:00:59.000000 groktest-0.2.0/pyproject.toml
+-rw-rw-r--   0 garrett   (1000) garrett   (1000)       38 2024-05-04 18:40:03.063159 groktest-0.2.0/setup.cfg
```

### Comparing `groktest-0.1.5/LICENSE` & `groktest-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `groktest-0.1.5/PKG-INFO` & `groktest-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: groktest
-Version: 0.1.5
+Version: 0.2.0
 Summary: Literate testing framework based on Python doctest
 Author-email: Garrett Smith <garrett@placeon.earth>
 Project-URL: Homepage, https://github.com/gar1t/groktest
 Project-URL: Bug Tracker, https://github.com/gar1t/groktest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyyaml
 
 ---
 test-type: doctest
 ---
 
 # Groktest
 
@@ -41,31 +42,31 @@
 - Test options do not require a `doctest:` prefix
 - Front-matter in test files may be used to configure a test suite
 
 ### Why?
 
 Python's `doctest` paved the way for computational documents like
 Jupyter Notebooks, R Markdown, and Quarto. It was one of the first of
-its kind. We owe a debt of grattutude to Tim Peters for the original
+its kind. We owe a debt of gratitude to Tim Peters for the original
 work and to Jim Fulton for advancing its use.
 
 The rationale for `doctest` is that examples provide a high-signal,
 low-noise representation of developer intent.
 
 - Tests are framed within comments (rather than using comments), which
   encourages a narrative mode of testing
 - Examples are often easier to understand (grok) than a series of
   assertions
 - Example output can replace a large number of explicit assertions,
-  providing more test coverage with fewer expresions
+  providing more test coverage with fewer expressions
 
 `doctest` however presents some key problems.
 
 - Result comparison can use an ellipsis `...` to match any output; while
-  the match is geedy, it can match invalid output and mast errors
+  the match is greedy, it can match invalid output and mast errors
 - The framework is Python specific and difficult to apply to cases
   outside Python
 - Pattern matching is limited to a single 'match all' pattern
 - Output from tests cannot be captured for use in subsequent tests
 
 Groktest addresses these issues while maintaining the original `doctest`
 value proposition.
```

### Comparing `groktest-0.1.5/README.md` & `groktest-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,31 +27,31 @@
 - Test options do not require a `doctest:` prefix
 - Front-matter in test files may be used to configure a test suite
 
 ### Why?
 
 Python's `doctest` paved the way for computational documents like
 Jupyter Notebooks, R Markdown, and Quarto. It was one of the first of
-its kind. We owe a debt of grattutude to Tim Peters for the original
+its kind. We owe a debt of gratitude to Tim Peters for the original
 work and to Jim Fulton for advancing its use.
 
 The rationale for `doctest` is that examples provide a high-signal,
 low-noise representation of developer intent.
 
 - Tests are framed within comments (rather than using comments), which
   encourages a narrative mode of testing
 - Examples are often easier to understand (grok) than a series of
   assertions
 - Example output can replace a large number of explicit assertions,
-  providing more test coverage with fewer expresions
+  providing more test coverage with fewer expressions
 
 `doctest` however presents some key problems.
 
 - Result comparison can use an ellipsis `...` to match any output; while
-  the match is geedy, it can match invalid output and mast errors
+  the match is greedy, it can match invalid output and mast errors
 - The framework is Python specific and difficult to apply to cases
   outside Python
 - Pattern matching is limited to a single 'match all' pattern
 - Output from tests cannot be captured for use in subsequent tests
 
 Groktest addresses these issues while maintaining the original `doctest`
 value proposition.
```

### Comparing `groktest-0.1.5/groktest/__init__.py` & `groktest-0.2.0/groktest/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from typing import *
 from types import ModuleType
 
-import configparser
 import copy
 import difflib
 import doctest
 import importlib
 import importlib.util
 import inspect
 import io
 import json
 import logging
 import os
 import re
 import sys
 import tokenize
 
+import yaml
+
 from . import _vendor_parse as parselib
 from . import _vendor_tomli as toml
 
 __all__ = [
     "__version__",
     "DEFAULT_SPEC",
     "PYTHON_SPEC",
@@ -33,33 +34,44 @@
     "ParseTypeFunctions",
     "ParseTypes",
     "ProjectDecodeError",
     "RunnerState",
     "Runtime",
     "RuntimeNotSupported",
     "SPECS",
+    "Skip",
     "Test",
     "TestMatch",
     "TestMatcher",
     "TestResult",
     "TestSpec",
     "TestTypeNotSupported",
     "init_runner_state",
     "match_test_output",
+    "matcher",
+    "parse_match",
     "parse_tests",
     "start_runtime",
     "test_file",
 ]
 
-__version__ = "0.1.5"  # Sync with pyproject.toml
-
+__version__ = "0.2.0"  # Sync with pyproject.toml
 
 log = logging.getLogger("groktest")
 
 
+class Skip(RuntimeError):
+    def __init__(self):
+        super().__init__("skip")
+
+
+class Panic(Exception):
+    pass
+
+
 class Error(Exception):
     pass
 
 
 class TestTypeNotSupported(Error):
     pass
 
@@ -82,14 +94,34 @@
 
 ParseTypes = Dict[str, str]
 
 ParseTypeFunction = Callable[[str], Any]
 
 ParseTypeFunctions = Dict[str, ParseTypeFunction]
 
+TransformFunction = Callable[[str, str], tuple[str, str]]
+
+OptionFunction = Callable[[Any, TestOptions, "Test"], Optional[TransformFunction]]
+
+OptionFunctions = dict[str, OptionFunction]
+
+
+class TestSummary:
+    def __init__(self):
+        self.failed: list[Test] = []
+        self.tested: list[Test] = []
+        self.skipped: list[Test] = []
+
+    def __repr__(self):
+        return (
+            f"<TestSummary failed={len(self.failed)}"
+            f" tested={len(self.tested)}"
+            f" skipped={len(self.skipped)}>"
+        )
+
 
 class TestSpec:
     def __init__(
         self,
         runtime: str,
         ps1: str,
         ps2: str,
@@ -109,40 +141,14 @@
             re.MULTILINE | re.VERBOSE,
         )
         self.blankline = blankline
         self.wildcard = wildcard
         self.option_candidates = option_candidates
 
 
-TestOptions = Dict[str, Any]
-
-
-class TestMatch:
-    def __init__(
-        self,
-        match: bool,
-        vars: Optional[Dict[str, Any]] = None,
-        reason: Optional[Any] = None,
-    ):
-        self.match = match
-        self.vars = vars
-        self.reason = reason
-
-
-TestMatcher = Callable[
-    [
-        str,
-        str,
-        Optional[TestOptions],
-        Optional[TestConfig],
-    ],
-    TestMatch,
-]
-
-
 class Test:
     def __init__(
         self,
         expr: str,
         expected: str,
         filename: str,
         line: int,
@@ -151,14 +157,19 @@
         self.expr = expr
         self.expected = expected
         self.filename = filename
         self.line = line
         self.options = options
 
 
+class TestProxy(Test):
+    def __init__(self, filename: str):
+        super().__init__("", "", filename, 0, {})
+
+
 class TestResult:
     def __init__(self, code: int, output: str, short_error: Optional[str] = None):
         self.code = code
         self.output = output
         self.short_error = short_error
 
 
@@ -187,42 +198,84 @@
         self.runtime = runtime
         self.stop_timeout = stop_timeout
 
     def __enter__(self):
         return self
 
     def __exit__(self, *exc: Any):
-        if self.stop_timeout is not None:
-            self.runtime.stop(self.stop_timeout)
-        else:
-            self.runtime.stop()
+        try:
+            _stop_runtime(self.runtime, self.stop_timeout)
+        except Exception as e:
+            if log.getEffectiveLevel() <= logging.DEBUG:
+                log.exception("Stopping runtime")
+            log.error("Error stopping runtime: %s", e)
+
+
+def _stop_runtime(runtime: Runtime, timeout: Optional[int]):
+    if timeout is not None:
+        runtime.stop(timeout)
+    else:
+        runtime.stop()
+
+
+Printer = Callable[[str], None]
 
 
 class RunnerState:
     def __init__(
         self,
         tests: List[Test],
         runtime: Runtime,
         spec: TestSpec,
         config: TestConfig,
         filename: str,
+        print_output: Optional[Printer] = None,
+        parse_functions: Optional[ParseTypeFunctions] = None,
+        option_functions: Optional[OptionFunctions] = None,
     ):
         self.tests = tests
         self.runtime = runtime
         self.spec = spec
         self.filename = filename
         self.config = config
-        self.results: Dict[str, Any] = {"failed": 0, "tested": 0, "skipped": 0}
+        self.summary = TestSummary()
         self.skip_rest = False
+        self.print_output = print_output or print
+        self.parse_functions = parse_functions or {}
+        self.option_functions = option_functions or {}
 
 
 class DocTestRunnerState:
     def __init__(self, filename: str, config: TestConfig):
         self.filename = filename
         self.config = config
+        self.results = TestSummary()
+
+
+class TestMatch:
+    def __init__(
+        self,
+        match: bool,
+        vars: Optional[Dict[str, Any]] = None,
+        reason: Optional[Any] = None,
+    ):
+        self.match = match
+        self.vars = vars
+        self.reason = reason
+
+
+TestMatcher = Callable[
+    [
+        str,
+        str,
+        Optional[TestOptions],
+        Optional[RunnerState],
+    ],
+    TestMatch,
+]
 
 
 DEFAULT_TEST_PATTERN = r"""
 # Credit: Tim Peters, et al. Python doctest.py
 # Test expression: PS1 line followed by zero or more PS2 lines
 (?P<expr>
     (?:^(?P<indent> [ ]*) {ps1} .*)   # PS1 line
@@ -297,31 +350,39 @@
 RUNTIME = {
     "doctest": "groktest.doctest.DoctestRuntime",
     "python": "groktest.python.PythonRuntime",
     "nushell": "groktest.nushell.NuShellRuntime",
 }
 
 
-def init_runner_state(filename: str, project_config: Optional[ProjectConfig] = None):
+def init_runner_state(
+    filename: str,
+    project_config: Optional[ProjectConfig] = None,
+    print_output: Optional[Printer] = None,
+):
     filename = os.path.abspath(filename)
     contents = _read_file(filename)
     fm = _parse_front_matter(contents, filename)
     spec = _spec_for_front_matter(fm, filename)
     test_config = _test_config(fm, project_config, filename)
-    log.debug("test config: %s", test_config)
+    log.debug("Test config: %s", test_config)
     if spec is DOCTEST_MARKER:
         return DocTestRunnerState(filename, test_config)
     runtime = start_runtime(spec.runtime, test_config)
     tests = parse_tests(contents, spec, filename)
-    return RunnerState(tests, runtime, spec, test_config, filename)
-
-
-def init_test_runner_state(spec: TestSpec, filename: Optional[str] = None):
-    runtime = start_runtime(spec.runtime)
-    return RunnerState([], runtime, spec, {}, filename or "<test>")
+    return RunnerState(
+        tests,
+        runtime,
+        spec,
+        test_config,
+        filename,
+        print_output or print,
+        _parse_type_functions(test_config),
+        _option_functions(test_config),
+    )
 
 
 def _read_file(filename: str):
     bytes = open(filename, "rb").read()
     return _norm_line_endings(bytes).decode()
 
 
@@ -339,113 +400,88 @@
 
     If PyYaml is installed, it's used to parse front matter. As this
     library has no external dependencies, if PyYaml is not installed, a
     parsing hack is used in attempt to parse front matter as YAML. In
     this case, front matter configuration is limited to simple key value
     pairs using `<key>: <value>` syntax.
     """
-    data = _parsed_front_matter(s, filename) or _empty_front_matter(filename)
-    data["__src__"] = filename
-    return data
+    return cast(
+        FrontMatter,
+        {
+            **_parsed_front_matter(s, filename),
+            "__src__": filename,
+        },
+    )
 
 
 def _parsed_front_matter(s: str, filename: str):
     m = _FRONT_MATTER_P.match(s)
     if not m:
-        return None
-    fm = m.group(1)
-    return (
-        _try_parse_json(fm, filename)
-        or _try_parse_toml(fm, filename)
-        or _try_parse_full_yaml(fm, filename)
-        or _try_parse_simplified_yaml(fm, filename)
-    )
+        log.debug("No front matter for %s", filename)
+        return cast(FrontMatter, {})
+    s = m.group(1)
+    try:
+        data = _try_parsers([_parse_json, _parse_toml, _parse_yaml], s, filename)
+    except ValueError as e:
+        log.warning(
+            "Unable to parse front matter in %s - verify valid JSON, TOML, or YAML",
+            filename,
+        )
+        return cast(FrontMatter, {})
+    else:
+        if isinstance(data, str):
+            log.warning(
+                "Unable to parse front matter in %s - verify valid JSON, TOML, or YAML",
+                filename,
+            )
+            return cast(FrontMatter, {})
+        if not isinstance(data, dict):
+            log.warning(
+                "Invalid front matter in %s, expected mapping but got %s",
+                filename,
+                type(data).__name__,
+            )
+            return cast(FrontMatter, {})
+    return cast(FrontMatter, data)
+
+
+Parser = Callable[[str, str], FrontMatter]
 
 
-def _empty_front_matter(filename: str):
-    log.debug("Missing or unparsable front matter for %s", filename)
-    return cast(FrontMatter, {})
+def _try_parsers(parsers: list[Parser], s: str, filename: str):
+    for p in parsers:
+        try:
+            return p(s, filename)
+        except ValueError:
+            pass
+    raise ValueError()
 
 
-def _try_parse_json(s: str, filename: str, raise_error: bool = False):
+def _parse_json(s: str, filename: str):
     try:
-        data = json.loads(s)
+        return json.loads(s)
     except Exception as e:
-        if raise_error:
-            raise
-        log.debug("ERROR parsing JSON for %s: %s", filename, e)
-        return None
-    else:
-        log.debug("Parsed JSON for %s: %r", filename, data)
-        return cast(FrontMatter, data)
+        log.debug("Could not parse JSON front matter for %s: %s", filename, e)
+        raise ValueError(e) from None
 
 
-def _try_parse_toml(s: str, filename: str, raise_error: bool = False):
+def _parse_toml(s: str, filename: str):
     try:
-        data = toml.loads(s)
+        return toml.loads(s)
     except toml.TOMLDecodeError as e:
-        if raise_error:
-            raise
-        log.debug("ERROR parsing TOML front matter for %s: %s", filename, e)
-        return None
-    else:
-        log.debug("Parsed TOML front matter for %s: %r", filename, data)
-        return cast(FrontMatter, data)
+        log.debug("Could not parse TOML front matter for %s: %s", filename, e)
+        raise ValueError(e) from None
 
 
-def _try_parse_full_yaml(s: str, filename: str, raise_error: bool = False):
+def _parse_yaml(s: str, filename: str):
     try:
-        import yaml  # type: ignore
-    except ImportError:
-        if raise_error:
-            raise
-        log.debug("yaml module not available, skipping full YAML for %s", filename)
-        return None
-    try:
-        data = yaml.safe_load(s)
+        return yaml.safe_load(s)
     except Exception as e:
-        if raise_error:
-            raise
-        log.debug("ERROR parsing YAML front matter for %s: %s", filename, e)
-        return None
-    else:
-        log.debug("Parsed YAML front matter  for %s: %r", filename, data)
-        if not isinstance(data, dict):
-            log.warning(
-                "Unsupported front-matter in %s: expected mapping, got %s",
-                filename,
-                type(data).__name__,
-            )
-            return None
-        return cast(FrontMatter, data)
-
-
-def _try_parse_simplified_yaml(s: str, filename: str, raise_error: bool = False):
-    parser = configparser.ConfigParser()
-    try:
-        parser.read_string("[__anonymous__]\n" + s)
-    except configparser.Error as e:
-        if raise_error:
-            raise
-        log.debug("ERROR parsing simplified YAML for %s: %s", filename, e)
-        return None
-    else:
-        data = _simplified_yaml_for_ini(parser)
-        log.debug("Parsed simplified YAML front matter for %s: %r", filename, data)
-        return cast(FrontMatter, data)
-
-
-def _simplified_yaml_for_ini(parser: configparser.ConfigParser):
-    parsed = {
-        section: dict(
-            {key: _simplified_yaml_val(val) for key, val in parser[section].items()}
-        )
-        for section in parser
-    }
-    return parsed.get("__anonymous__", {})
+        log.debug("Could not parse YAML front matter for %s: %s", filename, e)
+        raise ValueError(e) from None
 
 
 def _simplified_yaml_val(s: str):
     if s[:1] + s[-1:] in ("\"\"", "''"):
         return s[1:-1]
     s_lower = s.lower()
     if s_lower in ("true", "yes", "on"):
@@ -607,15 +643,17 @@
 
 
 def _test_config(
     test_fm: FrontMatter,
     project_config: Optional[ProjectConfig],
     filename: str,
 ):
-    project_config = project_config or _try_test_file_project_config(filename) or {}
+    project_config = project_config or {}
+    if "__src__" not in project_config:
+        project_config.update(_try_test_file_project_config(filename) or {})
     return _merge_test_config(project_config, test_fm)
 
 
 def _merge_test_config(project_config: TestConfig, test_fm: FrontMatter) -> TestConfig:
     test_config = front_matter_to_config(test_fm)
     # Start with project taking precedence over test config
     merged = {
@@ -627,23 +665,26 @@
     _merge_append_list(["python", "init"], test_config, merged)
     _merge_items(["parse", "types"], test_config, merged)
     _merge_append_list(["__src__"], test_config, merged)
     return merged
 
 
 def front_matter_to_config(fm: FrontMatter) -> TestConfig:
+    src = fm.get("__src__")
     try:
-        return fm["tool"]["groktest"]
+        config = fm["tool"]["groktest"]
     except KeyError:
-        return _mapped_front_matter_config(fm)
+        config = _mapped_front_matter_config(fm)
+    return {**config, **({"__src__": src} if src else {})}
 
 
 FRONT_MATTER_TO_CONFIG = {
     "parse-types": ["parse", "types"],
     "parse-functions": ["parse", "functions"],
+    "option-functions": ["option", "functions"],
     "python-init": ["python", "init"],
     "test-options": ["options"],
     "nushell-init": ["nushell", "init"],
 }
 
 
 def _mapped_front_matter_config(fm: FrontMatter) -> TestConfig:
@@ -748,81 +789,250 @@
         modname, classname = import_spec.rsplit(".", 1)
         mod = importlib.import_module(modname)
         rt = cast(Runtime, getattr(mod, classname)())
         rt.start(config)
         return rt
 
 
-def test_file(filename: str, config: Optional[ProjectConfig] = None):
-    state = init_runner_state(filename, config)
+def _parse_type_functions(config: TestConfig) -> ParseTypeFunctions:
+    return {
+        **_module_parse_type_functions(config),
+        **_regex_parse_type_functions(config),
+    }
+
+
+def _module_parse_type_functions(config: TestConfig) -> ParseTypeFunctions:
+    try:
+        spec = config["parse"]["functions"]
+    except KeyError:
+        return {}
+    else:
+        spec = _coerce_list(spec)
+        module_path = _config_src_path(config)
+        return dict(_iter_named_functions(spec, module_path, "parse_", "type_name"))
+
+
+def _config_src_path(config: TestConfig):
+    config_src: List[str] = _coerce_list(config["__src__"])
+    return [os.path.dirname(path) for path in config_src]
+
+
+def _iter_named_functions(
+    modules: List[Any],
+    module_path: List[str],
+    function_prefix: str,
+    name_attr: str,
+) -> Generator[Tuple[str, Callable[..., Any]], None, None]:
+    for module_name in modules:
+        log.debug("Loading parse functions from %s", module_name)
+        module = _try_load_module(module_name, module_path)
+        if not module:
+            continue
+        for f in _iter_module_functions(module, function_prefix):
+            function_name = _function_name(f, name_attr, function_prefix)
+            log.debug("Registering function %s as '%s' type", f.__name__, function_name)
+            yield function_name, f
+
+
+def _try_load_module(spec: str, path: List[str]):
+    if not isinstance(spec, str):
+        log.warning("Invalid value for functions %r, expected a string", spec)
+        return None
+    _ensure_sys_path_for_doc_tests(path)
+    try:
+        return importlib.import_module(spec)
+    except Exception as e:
+        if log.getEffectiveLevel() <= logging.DEBUG:
+            log.exception("Loading module %r", spec)
+        else:
+            log.warning("Error loading functions from %r: %r", spec, e)
+        return None
+
+
+def _ensure_sys_path_for_doc_tests(doctest_path: List[str]):
+    # Add in reverse order as doctest path goes from more specific (test
+    # file path) to less specific (project path)
+    for p in reversed(doctest_path):
+        if p not in sys.path:
+            sys.path.append(p)
+
+
+def _function_name(f: Callable[[str], Any], name_attr: str, prefix: str):
+    try:
+        return getattr(f, name_attr)
+    except AttributeError:
+        name = f.__name__
+        assert name.startswith(prefix)
+        return name[len(prefix) :]
+
+
+def _iter_module_functions(
+    module: ModuleType,
+    function_prefix: str,
+) -> Generator[ParseTypeFunction, None, None]:
+    for name in _exported_names(module, function_prefix):
+        x = getattr(module, name)
+        if _is_function(x):
+            yield x
+
+
+def _exported_names(module: ModuleType, prefix: str):
+    all = getattr(module, "__all__", [])
+    if isinstance(all, str):
+        all = all.split()
+    return [name for name in (all or dir(module)) if name.startswith(prefix)]
+
+
+def _is_function(x: Any):
+    # Simple sniff-test for callable with at least one arg
+    try:
+        sig = inspect.signature(x)
+    except TypeError:
+        return False
+    else:
+        return len(sig.parameters) >= 1
+
+
+def _regex_parse_type_functions(config: TestConfig) -> ParseTypeFunctions:
+    try:
+        types = config["parse"]["types"]
+    except KeyError:
+        return {}
+    else:
+        return {
+            type_name: _parselib_regex_converter(pattern)
+            for type_name, pattern in types.items()
+        }
+
+
+def _parselib_regex_converter(pattern: str):
+    def f(s: str):
+        return s
+
+    f.pattern = pattern
+    return f
+
+
+def _option_functions(config: TestConfig) -> OptionFunctions:
+    try:
+        spec = config["option"]["functions"]
+    except KeyError:
+        return {}
+    else:
+        spec = _coerce_list(spec)
+        module_path = _config_src_path(config)
+        return dict(_iter_named_functions(spec, module_path, "option_", "option_name"))
+
+
+def test_file(
+    filename: str,
+    config: Optional[ProjectConfig] = None,
+    print_output: Optional[Printer] = None,
+):
+    state = init_runner_state(filename, config, print_output)
     if isinstance(state, DocTestRunnerState):
-        return _doctest_file(state.filename, state.config)
+        _doctest_file(state)
+        return state.results
     assert isinstance(state, RunnerState)
     assert state.runtime.is_available
     state.runtime.init_for_tests(state.config)
     _apply_skip_for_solo(state.tests)
     with RuntimeScope(state.runtime):
         for test in state.tests:
-            test_options = _test_options(test, state.config, state.spec)
+            test_options = _test_options(test, state)
             _apply_skip_rest(test_options, state)
-            if _skip_test(test_options, state):
+            if _skip_test(test, test_options, state):
                 _handle_test_skipped(test, state)
             else:
                 run_test(test, test_options, state)
-        return state.results
+        return state.summary
 
 
 def run_test(test: Test, options: TestOptions, state: RunnerState):
     try:
         result = state.runtime.exec_test_expr(test, options)
-    except RuntimeError:
-        raise
     except Exception as e:
-        raise RuntimeError(e)
-    else:
-        _handle_test_result(result, test, options, state)
+        if log.getEffectiveLevel() <= logging.DEBUG:
+            log.exception("")
+        log.error("Unhandled error running test at %s:%s: %s", test.filename, test.line, e)
+        raise Panic()
+    _handle_test_result(result, test, options, state)
 
 
 def _apply_skip_for_solo(tests: List[Test]):
     solo_tests = [test for test in tests if test.options.get("solo")]
     if not solo_tests:
         return
     for test in tests:
         test.options["skip"] = test not in solo_tests
 
 
 def _apply_skip_rest(options: TestOptions, state: RunnerState):
     state.skip_rest = _option_value("skiprest", options, state.skip_rest)
 
 
-def _skip_test(options: TestOptions, state: RunnerState):
-    val = _option_value("skip", options, state.skip_rest)
-    if isinstance(val, str):
-        return bool(os.getenv(val))
-    return val
+def _skip_test(test: Test, options: TestOptions, state: RunnerState):
+    val = _option_value("skip", options, None)
+    if val is None:
+        val = _try_option_function_skip(test, options, state)
+    elif isinstance(val, str):
+        val = bool(os.getenv(val))
+    return val if val is not None else state.skip_rest
+
+
+def _try_option_function_skip(test: Test, options: TestOptions, state: RunnerState):
+    for name, f in state.option_functions.items():
+        val = options.get(name)
+        if val is None:
+            continue
+        try:
+            _apply_option_args(f, val, options, test)
+        except Skip:
+            return True
+        except Exception as e:
+            if e.args == ("skip",):
+                return True
+            if log.getEffectiveLevel() <= logging.DEBUG:
+                log.exception(name)
+            log.warning(
+                "Error evaluating option '%s' at %s:%i: %s",
+                name,
+                test.filename,
+                test.line,
+                e,
+            )
+    return None
+
+
+def _apply_option_args(f: Callable[..., Any], *args: Any):
+    f_arg_count = len(inspect.signature(f).parameters)
+    return f(*args[:f_arg_count])
 
 
 def _handle_test_skipped(test: Test, state: RunnerState):
-    state.results["skipped"] += 1
+    state.summary.skipped.append(test)
 
 
 def _handle_test_result(
-    result: TestResult, test: Test, options: TestOptions, state: RunnerState
+    result: TestResult,
+    test: Test,
+    options: TestOptions,
+    state: RunnerState,
 ):
-    expected = _format_match_expected(test, options, state.spec)
-    output_candidates = _match_test_output_candidates(result, test, options)
+    expected = _format_match_expected(test, options, state)
+    output_candidates = _match_test_output_candidates(result, test, options, state)
     match, match_output = _try_match_output_candidates(
         output_candidates, expected, test, state
     )
     _log_test_result_match(match, result, test, expected, match_output, state)
     if options.get("fails"):
         if match.match:
             _handle_unexpected_test_pass(test, options, state)
         else:
-            _handle_expected_test_failed(test, state)
+            _handle_expected_test_failed(test, options, state)
     elif match.match:
         _handle_test_passed(test, match, state)
     else:
         _handle_test_failed(test, match, result, options, state)
 
 
 def _log_test_result_match(
@@ -840,48 +1050,53 @@
     log.debug("  test expected:   %r", test.expected)
     log.debug("  test output [%r]: %r", result.code, result.output)
     log.debug("  used expected:   %r", used_expected)
     log.debug("  used output:     %r", used_test_output)
 
 
 def _try_match_output_candidates(
-    output_candidates: List[str], expected: str, test: Test, state: RunnerState
+    output_candidates: List[str],
+    expected: str,
+    test: Test,
+    state: RunnerState,
 ):
     assert output_candidates
     match = None
     matched_output = None
     for output in output_candidates:
-        match = match_test_output(expected, output, test, state.config, state.spec)
+        match = match_test_output(expected, output, test, state)
         matched_output = output
         if match.match:
             break
     assert match
     assert matched_output is not None
     return match, matched_output
 
 
 def _handle_unexpected_test_pass(test: Test, options: TestOptions, state: RunnerState):
-    _print_failed_test_sep(options)
-    print(f"File \"{test.filename}\", line {test.line}")
-    print("Failed example:")
-    _print_test_expr(test.expr)
-    print("Expected test to fail but passed")
-    state.results["failed"] += 1
-    state.results["tested"] += 1
+    _print_failed_test_sep(options, state)
+    state.print_output(f"File \"{test.filename}\", line {test.line}")
+    state.print_output("Failed example:")
+    _print_test_expr(test.expr, state)
+    state.print_output("Expected test to fail but passed")
+    state.summary.failed.append(test)
+    state.summary.tested.append(test)
 
 
-def _handle_expected_test_failed(test: Test, state: RunnerState):
-    state.results["tested"] += 1
+def _handle_expected_test_failed(test: Test, options: TestOptions, state: RunnerState):
+    # This case is not a failure - it's expected
+    state.summary.tested.append(test)
 
 
-def _format_match_expected(test: Test, options: TestOptions, spec: TestSpec):
+def _format_match_expected(test: Test, options: TestOptions, state: RunnerState):
     expected = _append_lf_for_non_empty(test.expected)
-    expected = _maybe_remove_blankline_markers(expected, options, spec)
+    expected = _maybe_remove_blankline_markers(expected, options, state.spec)
     expected = _maybe_normalize_whitespace(expected, options)
     expected = _maybe_normalize_paths(expected, options)
+    expected = _apply_option_functions(expected, test, options, state)
     return expected
 
 
 def _append_lf_for_non_empty(s: str):
     return s + '\n' if s else s
 
 
@@ -914,26 +1129,78 @@
 
 def _maybe_normalize_paths(s: str, options: TestOptions):
     if not _option_value("paths", options, False):
         return s
     return s.replace("\\\\", "\\").replace("\\", "/")
 
 
-def _match_test_output_candidates(result: TestResult, test: Test, options: TestOptions):
-    output = _format_test_output(result.output, options)
+def _apply_option_functions(
+    s: str,
+    test: Test,
+    options: TestOptions,
+    state: RunnerState,
+):
+    for name, f in state.option_functions.items():
+        val = options.get(name)
+        if val is None:
+            continue
+        f = _apply_option_args_no_raise(f, val, options, test)
+        if not f:
+            continue
+        log.debug("Applying option '%s' to string:\n%s", name, s)
+        try:
+            s = f(s)
+        except Exception as e:
+            if log.getEffectiveLevel() <= logging.DEBUG:
+                log.exception(name)
+            log.warning(
+                "Error evaluating option '%s' at %s:%i: %s",
+                name,
+                test.filename,
+                test.line,
+                e,
+            )
+        else:
+            log.debug("After option '%s':\n%s", name, s)
+
+    return s
+
+
+def _apply_option_args_no_raise(f: Callable[..., Any], *args: Any):
+    f_arg_count = len(inspect.signature(f).parameters)
+    try:
+        return f(*args[:f_arg_count])
+    except Exception:
+        log.exception(str([f, *args]))
+        return None
+
+
+def _match_test_output_candidates(
+    result: TestResult,
+    test: Test,
+    options: TestOptions,
+    state: RunnerState,
+):
+    output = _format_test_output(result.output, test, options, state)
     short_error = _maybe_short_error(result, options)
     if short_error:
-        return [output, _format_test_output(short_error, options)]
+        return [output, _format_test_output(short_error, test, options, state)]
     return [output]
 
 
-def _format_test_output(output: str, options: TestOptions):
+def _format_test_output(
+    output: str,
+    test: Test,
+    options: TestOptions,
+    state: RunnerState,
+):
     output = _truncate_empty_line_spaces(output)
     output = _maybe_normalize_whitespace(output, options)
     output = _maybe_normalize_paths(output, options)
+    output = _apply_option_functions(output, test, options, state)
     return output
 
 
 def _maybe_short_error(result: TestResult, options: TestOptions):
     if result.short_error and not _option_value("error-detail", options, False):
         return result.short_error
     return None
@@ -943,36 +1210,36 @@
     return re.sub(r"(?m)^[^\S\n]+$", "", s)
 
 
 def match_test_output(
     expected: str,
     test_output: str,
     test: Test,
-    config: TestConfig,
-    spec: TestSpec,
+    state: RunnerState,
 ):
-    options = _test_options(test, config, spec)
-    return matcher(options)(expected, test_output, options, config)
+    test_options = _test_options(test, state)
+    return matcher(test_options)(expected, test_output, test_options, state)
 
 
-def _test_options(test: Test, config: TestConfig, spec: TestSpec):
+def _test_options(test: Test, state: RunnerState):
     options = {
-        **_parse_config_options(config, test.filename),
+        **_test_options_for_config(state.config, test.filename),
         **test.options,
     }
-    _maybe_apply_spec_wildcard(spec, options)
+    _maybe_apply_spec_wildcard(state.spec, options)
     return cast(TestOptions, options)
 
 
-def _parse_config_options(config: TestConfig, filename: str):
-    parsed: TestOptions = {}
+def _test_options_for_config(config: TestConfig, filename: str):
     options = config.get("options")
     if not options:
-        return parsed
-    for part in _coerce_list(options):
+        return cast(TestOptions, {})
+    parsed: TestOptions = {}
+    # Visible options in reverse order as left-most takes priority
+    for part in reversed(_coerce_list(options)):
         if not isinstance(part, str):
             log.warning("Invalid option %r in %s: expected string", part, filename)
             continue
         parsed.update(_decode_options(part))
     return parsed
 
 
@@ -1005,20 +1272,19 @@
     return str_match
 
 
 def parse_match(
     expected: str,
     test_output: str,
     options: Optional[TestOptions] = None,
-    config: Optional[TestConfig] = None,
+    state: Optional[RunnerState] = None,
 ):
     options = options or {}
-    config = config or {}
     case_sensitive = _option_value("case", options, True)
-    extra_types = _parselib_types(config)
+    extra_types = state.parse_functions if state else {}
     try:
         m = parselib.parse(
             expected,
             test_output,
             extra_types,
             evaluate_result=True,
             case_sensitive=case_sensitive,
@@ -1038,140 +1304,19 @@
         return default
     else:
         if val is None:
             return default
         return val
 
 
-def _parselib_types(config: TestConfig) -> ParseTypeFunctions:
-    return {
-        **_parselib_module_types(config),
-        **_parselib_regex_types(config),
-    }
-
-
-def _parselib_module_types(config: TestConfig) -> ParseTypeFunctions:
-    try:
-        functions_spec = config["parse"]["functions"]
-    except KeyError:
-        return {}
-    else:
-        functions_spec = _coerce_list(functions_spec)
-        path = _config_src_path(config)
-        return dict(_iter_parse_functions(functions_spec, path))
-
-
-def _config_src_path(config: TestConfig):
-    config_src: List[str] = _coerce_list(config["__src__"])
-    return [os.path.dirname(path) for path in config_src]
-
-
-def _iter_parse_functions(
-    specs: List[Any],
-    path: List[str],
-) -> Generator[Tuple[str, ParseTypeFunction], None, None]:
-    for spec in specs:
-        log.debug("Loading parse functions from %s", spec)
-        module = _try_load_module(spec, path)
-        if not module:
-            continue
-        found = 0
-        for f in _iter_module_parse_functions(module):
-            found += 1
-            type_name = _parse_type_name(f)
-            log.debug("Registering function %s as '%s' type", f.__name__, type_name)
-            yield type_name, f
-        if not found:
-            log.debug("No parse functions found in %s", spec)
-
-
-def _try_load_module(spec: str, path: List[str]):
-    if not isinstance(spec, str):
-        log.warning("Invalid value for type-functions %r, expected a string", spec)
-        return None
-    _ensure_sys_path_for_doc_tests(path)
-    try:
-        return importlib.import_module(spec)
-    except Exception as e:
-        if log.getEffectiveLevel() <= logging.DEBUG:
-            log.exception("Loading module %r", spec)
-        else:
-            log.warning("Error loading parse functions from %r: %r", spec, e)
-        return None
-
-
-def _ensure_sys_path_for_doc_tests(doctest_path: List[str]):
-    # Add in reverse order as doctest path goes from more specific (test
-    # file path) to less specific (project path)
-    for p in reversed(doctest_path):
-        if p not in sys.path:
-            sys.path.append(p)
-
-
-def _parse_type_name(f: Callable[[str], Any]):
-    try:
-        return getattr(f, "type_name")
-    except AttributeError:
-        name = f.__name__
-        assert name.startswith("parse_")
-        return name[6:]
-
-
-def _iter_module_parse_functions(
-    module: ModuleType,
-) -> Generator[ParseTypeFunction, None, None]:
-    for name in _module_parse_names(module):
-        x = getattr(module, name)
-
-        if _is_parse_function(x):
-            yield x
-
-
-def _module_parse_names(module: ModuleType):
-    all = getattr(module, "__all__", [])
-    if isinstance(all, str):
-        all = all.split()
-    return [name for name in (all or dir(module)) if name.startswith("parse_")]
-
-
-def _is_parse_function(x: Any):
-    # Simple sniff test for callable with at least one arg
-    try:
-        sig = inspect.signature(x)
-    except TypeError:
-        return False
-    else:
-        return len(sig.parameters) >= 1
-
-
-def _parselib_regex_types(config: TestConfig) -> ParseTypeFunctions:
-    try:
-        types = config["parse"]["types"]
-    except KeyError:
-        return {}
-    else:
-        return {
-            type_name: _parselib_regex_converter(pattern)
-            for type_name, pattern in types.items()
-        }
-
-
-def _parselib_regex_converter(pattern: str):
-    def f(s: str):
-        return s
-
-    f.pattern = pattern
-    return f
-
-
 def str_match(
     expected: str,
     test_output: str,
     options: Optional[TestOptions] = None,
-    config: Optional[TestConfig] = None,
+    state: Optional[RunnerState] = None,
 ):
     options = options or {}
     expected, test_output = _apply_transform_options(expected, test_output, options)
     wildcard = options.get("wildcard")
     if wildcard:
         return _wildcard_match(expected, test_output, wildcard, options)
     return _default_str_match(expected, test_output, options)
@@ -1240,74 +1385,78 @@
     options: Optional[TestOptions] = None,
 ):
     return TestMatch(True) if test_output == expected else TestMatch(False)
 
 
 def _handle_test_passed(test: Test, match: TestMatch, state: RunnerState):
     state.runtime.handle_test_match(match)
-    state.results["tested"] += 1
+    state.summary.tested.append(test)
 
 
 def _handle_test_failed(
     test: Test,
     match: TestMatch,
     result: TestResult,
     options: TestOptions,
     state: RunnerState,
 ):
-    _print_failed_test_sep(options)
-    _print_failed_test(test, match, result, options, state.spec)
-    state.results["failed"] += 1
-    state.results["tested"] += 1
+    _print_failed_test_sep(options, state)
+    _print_failed_test(test, match, result, options, state)
+    state.summary.failed.append(test)
+    state.summary.tested.append(test)
+    if state.config.get("fail-fast"):
+        state.skip_rest = True
 
 
-def _print_failed_test_sep(options: TestOptions):
+def _print_failed_test_sep(options: TestOptions, state: RunnerState):
     sep = _option_value("sep", options, True)
     if sep is True:
-        print("**********************************************************************")
+        state.print_output("*" * 70)
     elif sep:
-        print(sep)
+        state.print_output(sep)
 
 
 def _print_failed_test(
     test: Test,
     match: TestMatch,
     result: TestResult,
     options: TestOptions,
-    spec: TestSpec,
+    state: RunnerState,
 ):
-    print(f"File \"{test.filename}\", line {test.line}")
-    print("Failed example:")
-    _print_test_expr(test.expr)
+    state.print_output(f"File \"{test.filename}\", line {test.line}")
+    state.print_output("Failed example:")
+    _print_test_expr(test.expr, state)
     if test.expected and options.get("diff"):
-        _print_test_result_diff(test, result, options, spec)
+        _print_test_result_diff(test, result, options, state)
     else:
-        _print_test_expected(test)
-        _print_test_result_output(result, options, spec)
+        _print_test_expected(test, state)
+        _print_test_result_output(result, options, state)
     if match.reason:
-        print(f"Reason:")
-        _print_mismatch_reason(match.reason, test)
+        state.print_output(f"Reason:")
+        _print_mismatch_reason(match.reason, test, state)
 
 
-def _print_test_expr(expr: str):
+def _print_test_expr(expr: str, state: RunnerState):
     expr = expr.strip()
     for line in expr.split("\n"):
-        print("    " + line)
+        state.print_output("    " + line)
 
 
 def _print_test_result_diff(
     test: Test,
     result: TestResult,
     options: TestOptions,
-    spec: TestSpec,
+    state: RunnerState,
 ):
-    expected_lines, output_lines = _format_lines_for_diff(test, result, options, spec)
-    print("Differences between expected and actual:")
+    expected_lines, output_lines = _format_lines_for_diff(
+        test, result, options, state.spec
+    )
+    state.print_output("Differences between expected and actual:")
     for line in _diff_lines(expected_lines, output_lines):
-        print("   " + line)
+        state.print_output("   " + line)
 
 
 def _format_lines_for_diff(
     test: Test, result: TestResult, options: TestOptions, spec: TestSpec
 ):
     expected = test.expected
     output = _format_test_result_output(result.output, options, spec)
@@ -1317,36 +1466,40 @@
 def _diff_lines(a: List[str], b: List[str]):
     diff = difflib.unified_diff(a, b, n=2)
     diff_no_header = list(diff)[2:]
     for line in diff_no_header:
         yield line.rstrip()
 
 
-def _print_test_expected(test: Test):
+def _print_test_expected(test: Test, state: RunnerState):
     if test.expected:
-        print("Expected:")
+        state.print_output("Expected:")
         expected = _format_test_result_expected(test.expected)
         for line in expected.split("\n"):
-            print("    " + line)
+            state.print_output("    " + line)
     else:
-        print("Expected nothing")
+        state.print_output("Expected nothing")
 
 
 def _format_test_result_expected(expected: str):
     return expected.strip()
 
 
-def _print_test_result_output(result: TestResult, options: TestOptions, spec: TestSpec):
+def _print_test_result_output(
+    result: TestResult,
+    options: TestOptions,
+    state: RunnerState,
+):
     if result.output:
-        print("Got:")
-        output = _format_test_result_output(result.output, options, spec)
+        state.print_output("Got:")
+        output = _format_test_result_output(result.output, options, state.spec)
         for line in output.split("\n"):
-            print("    " + line)
+            state.print_output("    " + line)
     else:
-        print("Got nothing")
+        state.print_output("Got nothing")
 
 
 def _format_test_result_output(output: str, options: TestOptions, spec: TestSpec):
     blankline = _blankline_marker(options, spec)
     if blankline:
         output = _insert_blankline_markers(output, blankline)
     return _strip_trailing_lf(output)
@@ -1356,42 +1509,46 @@
     return re.sub(r"(?m)^[ ]*(?=\n)", marker, s)
 
 
 def _strip_trailing_lf(s: str):
     return s[:-1] if s[-1:] == "\n" else s
 
 
-def _print_mismatch_reason(reason: Any, test: Test):
+def _print_mismatch_reason(reason: Any, test: Test, state: RunnerState):
     msg = str(reason)
     # Try format spec error message
     m = re.match(r"format spec '(.+?)' not recognized", msg)
     if m:
         type = m.group(1)
         line = _find_parse_type_line(type, test.expected)
         line_msg = f" on line {line}" if line is not None else ""
-        print(f"    Unsupported parse type '{type}'{line_msg}")
+        state.print_output(f"    Unsupported parse type '{type}'{line_msg}")
     else:
-        print(f"    {msg}")
+        state.print_output(f"    {msg}")
 
 
 def _find_parse_type_line(type: str, s: str):
     m = re.search(rf"{{\s*(?:[^\s:]+)?\s*:\s*{re.escape(type)}\s*?}}", s)
     if m:
         return s[: m.start()].count("\n") + 1
     return None
 
 
-def _doctest_file(filename: str, config: TestConfig):
+def _doctest_file(state: DocTestRunnerState):
     failed, tested = doctest.testfile(
-        filename,
+        state.filename,
         module_relative=False,
-        optionflags=_doctest_options(config),
-        extraglobs=_doctest_globals(config),
+        optionflags=_doctest_options(state.config),
     )
-    return {"failed": failed, "tested": tested}
+    test = TestProxy(state.filename)
+    if failed:
+        assert tested, state.filename
+        state.results.failed.append(test)
+    if tested:
+        state.results.tested.append(test)
 
 
 def _doctest_options(config: TestConfig):
     opts = config.get("options")
     if not opts:
         return 0
     opts = " ".join(_coerce_list(opts))
@@ -1412,52 +1569,44 @@
         enabled, opt = opt[0] == "+", opt[1:]
         try:
             yield getattr(doctest, opt.upper()), enabled
         except AttributeError:
             pass
 
 
-def _doctest_globals(config: Any):
-    from pprint import pprint as pprint0
-
-    def pprint(s: str, **kw: Any):
-        kw = dict(width=72, **kw)
-        pprint0(s, **kw)
-
-    return {
-        "pprint": pprint,
-    }
-
-
 def load_project_config(filename: str):
     try:
         data = _load_toml(filename)
     except toml.TOMLDecodeError as e:
         raise ProjectDecodeError(e, filename) from None
     else:
-        return _project_config_for_data(data) if data else None
+        return _project_config_for_data(data)
 
 
 def _load_toml(filename: str):
     try:
         f = open(filename, "rb")
     except FileNotFoundError:
         raise
     with f:
         try:
             data = toml.load(f)
         except toml.TOMLDecodeError:
             raise
         else:
-            log.debug("Using project config in %s", filename)
+            if not isinstance(data, dict):
+                raise SystemExit(
+                    f"Unexpected config in {filename}: expected "
+                    f"mapping but got {type(data).__name__}"
+                )
             data["__src__"] = filename
             return data
 
 
 def _project_config_for_data(data: Dict[str, Any]):
     try:
         groktest_data = data["tool"]["groktest"]
     except KeyError:
-        return None
+        return cast(ProjectConfig, {})
     else:
         groktest_data["__src__"] = data["__src__"]
         return cast(ProjectConfig, groktest_data)
```

### Comparing `groktest-0.1.5/groktest/_vendor_parse.py` & `groktest-0.2.0/groktest/_vendor_parse.py`

 * *Files identical despite different names*

### Comparing `groktest-0.1.5/groktest/_vendor_tomli/_parser.py` & `groktest-0.2.0/groktest/_vendor_tomli/_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Licensed to PSF under a Contributor Agreement.
 
 from __future__ import annotations
 
 from collections.abc import Iterable
 import string
 from types import MappingProxyType
-from typing import Any, BinaryIO, NamedTuple
+from typing import Any, BinaryIO, NamedTuple, Optional
 
 from ._re import (
     RE_DATETIME,
     RE_LOCALTIME,
     RE_NUMBER,
     match_to_datetime,
     match_to_localtime,
@@ -258,15 +258,15 @@
             pos += 1
         raise suffixed_err(src, pos, f"Found invalid character {src[pos]!r}")
     return new_pos
 
 
 def skip_comment(src: str, pos: Pos) -> Pos:
     try:
-        char: str | None = src[pos]
+        char: Optional[str] = src[pos]
     except IndexError:
         char = None
     if char == "#":
         return skip_until(
             src, pos + 1, "\n", error_on=ILLEGAL_COMMENT_CHARS, error_on_eof=False
         )
     return pos
@@ -355,15 +355,15 @@
 
 
 def parse_key_value_pair(
     src: str, pos: Pos, parse_float: ParseFloat
 ) -> tuple[Pos, Key, Any]:
     pos, key = parse_key(src, pos)
     try:
-        char: str | None = src[pos]
+        char: Optional[str] = src[pos]
     except IndexError:
         char = None
     if char != "=":
         raise suffixed_err(src, pos, "Expected '=' after a key in a key/value pair")
     pos += 1
     pos = skip_chars(src, pos, TOML_WS)
     pos, value = parse_value(src, pos, parse_float)
@@ -372,29 +372,29 @@
 
 def parse_key(src: str, pos: Pos) -> tuple[Pos, Key]:
     pos, key_part = parse_key_part(src, pos)
     key: Key = (key_part,)
     pos = skip_chars(src, pos, TOML_WS)
     while True:
         try:
-            char: str | None = src[pos]
+            char: Optional[str] = src[pos]
         except IndexError:
             char = None
         if char != ".":
             return pos, key
         pos += 1
         pos = skip_chars(src, pos, TOML_WS)
         pos, key_part = parse_key_part(src, pos)
         key += (key_part,)
         pos = skip_chars(src, pos, TOML_WS)
 
 
 def parse_key_part(src: str, pos: Pos) -> tuple[Pos, str]:
     try:
-        char: str | None = src[pos]
+        char: Optional[str] = src[pos]
     except IndexError:
         char = None
     if char in BARE_KEY_CHARS:
         start_pos = pos
         pos = skip_chars(src, pos, BARE_KEY_CHARS)
         return pos, src[start_pos:pos]
     if char == "'":
@@ -581,15 +581,15 @@
         pos += 1
 
 
 def parse_value(  # noqa: C901
     src: str, pos: Pos, parse_float: ParseFloat
 ) -> tuple[Pos, Any]:
     try:
-        char: str | None = src[pos]
+        char: Optional[str] = src[pos]
     except IndexError:
         char = None
 
     # IMPORTANT: order conditions based on speed of checking and likelihood
 
     # Basic strings
     if char == '"':
```

### Comparing `groktest-0.1.5/groktest/_vendor_tomli/_re.py` & `groktest-0.2.0/groktest/_vendor_tomli/_re.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Licensed to PSF under a Contributor Agreement.
 
 from __future__ import annotations
 
 from datetime import date, datetime, time, timedelta, timezone, tzinfo
 from functools import lru_cache
 import re
-from typing import Any
+from typing import Any, Optional
 
 from ._types import ParseFloat
 
 # E.g.
 # - 00:32:00.999999
 # - 00:32:00
 _TIME_RE_STR = r"([01][0-9]|2[0-3]):([0-5][0-9]):([0-5][0-9])(?:\.([0-9]{1,6})[0-9]*)?"
@@ -70,15 +70,15 @@
     ) = match.groups()
     year, month, day = int(year_str), int(month_str), int(day_str)
     if hour_str is None:
         return date(year, month, day)
     hour, minute, sec = int(hour_str), int(minute_str), int(sec_str)
     micros = int(micros_str.ljust(6, "0")) if micros_str else 0
     if offset_sign_str:
-        tz: tzinfo | None = cached_tz(
+        tz: Optional[tzinfo] = cached_tz(
             offset_hour_str, offset_minute_str, offset_sign_str
         )
     elif zulu_time:
         tz = timezone.utc
     else:  # local date-time
         tz = None
     return datetime(year, month, day, hour, minute, sec, micros, tzinfo=tz)
```

### Comparing `groktest-0.1.5/groktest/nushell.py` & `groktest-0.2.0/groktest/nushell.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 class NuShellRuntime(Runtime):
     _state: Optional[State] = None
 
     def start(self, config: Optional[TestConfig] = None):
         self._state = _init_state()
 
-    def init_for_tests(self, config: TestConfig | None = None) -> None:
+    def init_for_tests(self, config: Optional[TestConfig] = None) -> None:
         assert self._state is not None
         self._state.vars.clear()
         self._state.cwd = None
         self._state.config = config
 
     def exec_test_expr(self, test: Test, options: TestOptions):
         assert self._state
@@ -198,31 +198,34 @@
     {_cd_command(state)}
     print (
         {test.expr}
     )
     $env.PWD
     """
 
+
 def _init_commands(state: State):
     if not state.config:
         return ""
     try:
         return state.config["nushell"]["init"]
     except KeyError:
         return ""
 
+
 def _source_vars_command(state: State):
     return f"source {state.vars_nu_filename}"
 
 
 def _cd_command(state: State):
     if not state.cwd:
         return ""
     return f"cd `{state.cwd}`"
 
+
 def _log_command(cmd: List[str], cwd: str, env: Dict[str, str]):
     if log.getEffectiveLevel() > logging.DEBUG:
         return
     log.debug("Running Nu command:")
     log.debug(textwrap.indent(f"cmd: {cmd}", "  "))
     log.debug(textwrap.indent(f"cwd: {cwd}", "  "))
     log.debug(textwrap.indent(f"env: {env}", "  "))
```

### Comparing `groktest-0.1.5/groktest/python.py` & `groktest-0.2.0/groktest/python.py`

 * *Files 14% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 class PythonRuntime(Runtime):
     _p: Optional[subprocess.Popen[str]] = None
 
     def start(self, config: Optional[TestConfig] = None):
         self._p = _open_proc()
 
-    def init_for_tests(self, config: TestConfig | None = None) -> None:
+    def init_for_tests(self, config: Optional[TestConfig] = None) -> None:
         if config:
             _init_for_tests(config, _check_proc(self._p))
 
     def exec_test_expr(self, test: Test, options: TestOptions):
         return _exec_test_expr(test, options, _check_proc(self._p))
 
     def handle_test_match(self, match: TestMatch):
@@ -111,16 +111,20 @@
     assert p.stdin
     assert p.stdout
     return p.stdin, p.stdout
 
 
 def _close_proc(p: Popen[str], timeout: int):
     assert p.stdin
-    p.stdin.write("\n")
-    p.stdin.flush()
+    try:
+        p.stdin.write("\n")
+        p.stdin.flush()
+    except OSError as e:
+        if e.errno != 22:  # stream closed
+            raise
     try:
         p.wait(timeout)
     except subprocess.TimeoutExpired:
         p.send_signal(_sigkill())
 
 
 def _sigkill():
@@ -187,48 +191,76 @@
             "options": options,
         }
     )
     _write_req(req, out)
 
 
 def _read_test_result(input: IO[str]):
-    resp = json.loads(input.readline())
-    return TestResult(resp["code"], resp["output"], resp.get("short-error"))
+    resp_raw = input.readline()
+    if not resp_raw:
+        return TestResult(-9, "", "")
+    try:
+        resp = json.loads(resp_raw)
+    except json.JSONDecodeError as e:
+        return TestResult(-9, "", f"Invalid resp from runtime server: {resp_raw}")
+    else:
+        return TestResult(resp["code"], resp["output"], resp.get("short-error"))
 
 
 def _update_vars(vars: Dict[str, Any], proc: Popen[str]):
     stdin, stdout = _proc_streams(proc)
     _write_vars_req(vars, stdin)
     _read_ack(stdout)
 
 
 def _write_vars_req(vars: Dict[str, Any], out: IO[str]):
     req = json.dumps({"type": "vars", "vars": vars})
     _write_req(req, out)
 
 
+def _parse_args():
+    import argparse
+
+    p = argparse.ArgumentParser()
+    p.add_argument("--debug", action="store_true")
+    return p.parse_args()
+
+
+def _init_logging():
+    logging.basicConfig(
+        level=logging.DEBUG if args.debug else logging.WARNING,
+        format="%(levelname)s: [%(name)s] %(message)s",
+    )
+    globals()["log"] = logging.getLogger("groktest.python")
+
+
 def _main_loop():
     globals = {}
     while True:
         line = _readline()
         if not line:
             break
         req = _decode_request(line)
         if isinstance(req, TestReq):
-            _handle_test(req, globals)
+            _handle_test_req(req, globals)
         elif isinstance(req, VarsReq):
-            _handle_vars(req, globals)
+            _handle_vars_req(req, globals)
         elif isinstance(req, InitReq):
-            _handle_init(req, globals)
+            _handle_init_req(req, globals)
         else:
             assert False, req
 
 
 def _readline():
-    return sys.stdin.readline().rstrip()
+    try:
+        return sys.stdin.readline().rstrip()
+    except OSError as e:
+        if e.errno != 22:  # stream closed
+            raise
+        return ""
 
 
 def _decode_request(line: str):
     data = json.loads(line)
     if data["type"] == "test":
         return TestReq(
             expr=data["expr"],
@@ -240,17 +272,17 @@
         return VarsReq(data["vars"])
     elif data["type"] == "init":
         return InitReq(data["expr"])
     else:
         assert False, data
 
 
-def _handle_test(test: TestReq, globals: Dict[str, Any]):
+def _handle_test_req(test: TestReq, globals: Dict[str, Any]):
     _log_test(test)
-    with _StdOutCapture() as out:
+    with _StdOutCapture(test.options) as out:
         try:
             _exec_test(test, globals)
         except:
             exc_info = sys.exc_info()
         else:
             exc_info = None
     _handle_test_result(out.getvalue(), exc_info, test)
@@ -274,37 +306,76 @@
     log.debug("Test result:")
     log.debug(textwrap.indent(output, "  "))
     if exc_info and log.getEffectiveLevel() <= logging.DEBUG:
         log.debug("%s", _format_exc_info(exc_info))
 
 
 class _StdOutCapture(io.StringIO):
-    _real_stdout = None
+    _stdout_save = None
+    _stderr_save = None
+    _log_handlers_save = None
+
+    def __init__(self, options: TestOptions):
+        super().__init__()
+        self._capture_stderr = options.get("stderr")
 
     def __enter__(self):
-        assert not self._real_stdout
-        self._real_stdout = sys.stdout
+        assert self._stdout_save is None
+        assert self._stderr_save is None
+        assert self._log_handlers_save is None
+        self._stdout_save = sys.stdout
         sys.stdout = self
+        if self._capture_stderr:
+            self._stderr_save = sys.stderr
+            sys.stderr = self
+            self._log_handlers_save = _set_log_handlers(self)
         return self
 
     def __exit__(self, *exc: Any):
-        assert self._real_stdout
-        sys.stdout = self._real_stdout
-        self._real_stdout = None
+        assert self._stdout_save is not None
+        sys.stdout = self._stdout_save
+        self._stdout_save = None
+        if self._stderr_save:
+            assert self._stderr_save is not None
+            sys.stderr = self._stderr_save
+            self._stderr_save = None
+            assert self._log_handlers_save is not None
+            _restore_log_handlers(self._log_handlers_save)
+
+
+def _set_log_handlers(stream: IO[str]):
+    handlers: list[tuple[logging.Logger, list[logging.Handler]]] = []
+    cur = log
+    while cur:
+        handlers.append((cur, cur.handlers))
+        cur.handlers = [
+            logging.StreamHandler(stream) if hasattr(h, "stream") else h
+            for h in cur.handlers
+        ]
+        cur = cur.parent
+    return handlers
+
+
+def _restore_log_handlers(
+    log_handlers: list[tuple[logging.Logger, list[logging.Handler]]]
+):
+    for logger, handlers in log_handlers:
+        logger.handlers = handlers
 
 
 def _exec_test(test: TestReq, globals: Dict[str, Any]):
     _apply_test_globals_effect(test, globals)
     code = _compile_test_expr(test)
     try:
         result = eval(code, globals)
     except AssertionError as e:
         _maybe_apply_code_vars(e, code, globals)
         raise
-    _maybe_pretty_print_result(result, test.options)
+    else:
+        _maybe_pretty_print_result(result, test.options)
 
 
 def _maybe_apply_code_vars(e: AssertionError, code: CodeType, globals: Dict[str, Any]):
     if not e.args:
         e.args = (_code_vars(code, globals),)
 
 
@@ -485,25 +556,25 @@
 
 def _writeline(line: str):
     sys.stdout.write(line)
     sys.stdout.write("\n")
     sys.stdout.flush()
 
 
-def _handle_vars(vars: VarsReq, globals: Dict[str, Any]):
+def _handle_vars_req(vars: VarsReq, globals: Dict[str, Any]):
     _log_vars(vars)
     globals.update(vars.vars)
     _writeline(_encode_ack())
 
 
 def _log_vars(vars: VarsReq):
     log.debug("Updating variables: %r", vars.vars)
 
 
-def _handle_init(init: InitReq, globals: Dict[str, Any]):
+def _handle_init_req(init: InitReq, globals: Dict[str, Any]):
     _log_init(init)
     globals.clear()
     try:
         exec(init.expr, globals)
     except Exception as e:
         log.exception("Error initializing Python runtime")
     _writeline(_encode_ack())
@@ -515,21 +586,10 @@
 
 
 def _encode_ack():
     return json.dumps("ack")
 
 
 if __name__ == "__main__":
-    import argparse
-
-    p = argparse.ArgumentParser()
-    p.add_argument("--debug", action="store_true")
-    args = p.parse_args()
-
-    logging.basicConfig(
-        level=logging.DEBUG if args.debug else logging.WARNING,
-        format="%(levelname)s: [%(name)s] %(message)s",
-    )
-
-    globals()["log"] = logging.getLogger("groktest.python")
-
+    args = _parse_args()
+    _init_logging()
     _main_loop()
```

### Comparing `groktest-0.1.5/groktest.egg-info/PKG-INFO` & `groktest-0.2.0/groktest.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: groktest
-Version: 0.1.5
+Version: 0.2.0
 Summary: Literate testing framework based on Python doctest
 Author-email: Garrett Smith <garrett@placeon.earth>
 Project-URL: Homepage, https://github.com/gar1t/groktest
 Project-URL: Bug Tracker, https://github.com/gar1t/groktest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyyaml
 
 ---
 test-type: doctest
 ---
 
 # Groktest
 
@@ -41,31 +42,31 @@
 - Test options do not require a `doctest:` prefix
 - Front-matter in test files may be used to configure a test suite
 
 ### Why?
 
 Python's `doctest` paved the way for computational documents like
 Jupyter Notebooks, R Markdown, and Quarto. It was one of the first of
-its kind. We owe a debt of grattutude to Tim Peters for the original
+its kind. We owe a debt of gratitude to Tim Peters for the original
 work and to Jim Fulton for advancing its use.
 
 The rationale for `doctest` is that examples provide a high-signal,
 low-noise representation of developer intent.
 
 - Tests are framed within comments (rather than using comments), which
   encourages a narrative mode of testing
 - Examples are often easier to understand (grok) than a series of
   assertions
 - Example output can replace a large number of explicit assertions,
-  providing more test coverage with fewer expresions
+  providing more test coverage with fewer expressions
 
 `doctest` however presents some key problems.
 
 - Result comparison can use an ellipsis `...` to match any output; while
-  the match is geedy, it can match invalid output and mast errors
+  the match is greedy, it can match invalid output and mast errors
 - The framework is Python specific and difficult to apply to cases
   outside Python
 - Pattern matching is limited to a single 'match all' pattern
 - Output from tests cannot be captured for use in subsequent tests
 
 Groktest addresses these issues while maintaining the original `doctest`
 value proposition.
```

### Comparing `groktest-0.1.5/pyproject.toml` & `groktest-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 [project]
 
 name = "groktest"
-version = "0.1.5"  # Sync with groktest.__init__
+version = "0.2.0"  # Sync with groktest.__init__
 authors = [
   { name="Garrett Smith", email="garrett@placeon.earth" },
 ]
 description = "Literate testing framework based on Python doctest"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "pyyaml",
+]
 
 [project.scripts]
 
 groktest = "groktest.__main__:main"
 
 [project.urls]
 
@@ -34,15 +37,14 @@
   "README.md",
   "docs/*.md",
   "examples/*.md"
 ]
 
 exclude = [
   "docs/yaml.md",
-  "examples/unknown-format.md"
+  "examples/unknown-format.md",
+  "examples/fail-fast.md",
 ]
 
 python.init = """
-from groktest import load_project_config
-from os import path
-import re
+from groktest._test_util import *
 """
```

