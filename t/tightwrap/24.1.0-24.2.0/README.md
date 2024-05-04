# Comparing `tmp/tightwrap-24.1.0.tar.gz` & `tmp/tightwrap-24.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Jan  9 20:08:01 2024, max compression
+gzip compressed data, last modified: Sat May  4 12:43:10 2024, max compression
```

## Comparing `tightwrap-24.1.0.tar` & `tightwrap-24.2.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0      182 2024-01-09 20:08:01.000000 tightwrap-24.1.0/Justfile
--rw-r--r--   0        0        0    37967 2024-01-09 20:08:01.000000 tightwrap-24.1.0/pdm.lock
--rw-r--r--   0        0        0      752 2024-01-09 20:08:01.000000 tightwrap-24.1.0/tox.ini
--rw-r--r--   0        0        0     3195 2024-01-09 20:08:01.000000 tightwrap-24.1.0/.github/workflows/main.yml
--rw-r--r--   0        0        0     1577 2024-01-09 20:08:01.000000 tightwrap-24.1.0/.github/workflows/pypi-package.yml
--rw-r--r--   0        0        0      812 2024-01-09 20:08:01.000000 tightwrap-24.1.0/src/tightwrap/__init__.py
--rw-r--r--   0        0        0        0 2024-01-09 20:08:01.000000 tightwrap-24.1.0/src/tightwrap/py.typed
--rw-r--r--   0        0        0        0 2024-01-09 20:08:01.000000 tightwrap-24.1.0/tests/__init__.py
--rw-r--r--   0        0        0      321 2024-01-09 20:08:01.000000 tightwrap-24.1.0/tests/test_typing.yml
--rw-r--r--   0        0        0      929 2024-01-09 20:08:01.000000 tightwrap-24.1.0/tests/test_wraps.py
--rw-r--r--   0        0        0     3104 2024-01-09 20:08:01.000000 tightwrap-24.1.0/.gitignore
--rw-r--r--   0        0        0     9160 2024-01-09 20:08:01.000000 tightwrap-24.1.0/LICENSE
--rw-r--r--   0        0        0     2429 2024-01-09 20:08:01.000000 tightwrap-24.1.0/README.md
--rw-r--r--   0        0        0      717 2024-01-09 20:08:01.000000 tightwrap-24.1.0/pyproject.toml
--rw-r--r--   0        0        0     2675 2024-01-09 20:08:01.000000 tightwrap-24.1.0/PKG-INFO
+-rw-r--r--   0        0        0      182 2024-05-04 12:43:10.000000 tightwrap-24.2.0/Justfile
+-rw-r--r--   0        0        0    37967 2024-05-04 12:43:10.000000 tightwrap-24.2.0/pdm.lock
+-rw-r--r--   0        0        0      792 2024-05-04 12:43:10.000000 tightwrap-24.2.0/tox.ini
+-rw-r--r--   0        0        0     3253 2024-05-04 12:43:10.000000 tightwrap-24.2.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1577 2024-05-04 12:43:10.000000 tightwrap-24.2.0/.github/workflows/pypi-package.yml
+-rw-r--r--   0        0        0     1577 2024-05-04 12:43:10.000000 tightwrap-24.2.0/src/tightwrap/__init__.py
+-rw-r--r--   0        0        0     2654 2024-05-04 12:43:10.000000 tightwrap-24.2.0/src/tightwrap/_backported.py
+-rw-r--r--   0        0        0        0 2024-05-04 12:43:10.000000 tightwrap-24.2.0/src/tightwrap/py.typed
+-rw-r--r--   0        0        0        0 2024-05-04 12:43:10.000000 tightwrap-24.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      321 2024-05-04 12:43:10.000000 tightwrap-24.2.0/tests/test_typing.yml
+-rw-r--r--   0        0        0     1093 2024-05-04 12:43:10.000000 tightwrap-24.2.0/tests/test_wraps.py
+-rw-r--r--   0        0        0     3104 2024-05-04 12:43:10.000000 tightwrap-24.2.0/.gitignore
+-rw-r--r--   0        0        0     9160 2024-05-04 12:43:10.000000 tightwrap-24.2.0/LICENSE
+-rw-r--r--   0        0        0     2615 2024-05-04 12:43:10.000000 tightwrap-24.2.0/README.md
+-rw-r--r--   0        0        0     1232 2024-05-04 12:43:10.000000 tightwrap-24.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3392 2024-05-04 12:43:10.000000 tightwrap-24.2.0/PKG-INFO
```

### Comparing `tightwrap-24.1.0/pdm.lock` & `tightwrap-24.2.0/pdm.lock`

 * *Files identical despite different names*

### Comparing `tightwrap-24.1.0/tox.ini` & `tightwrap-24.2.0/tox.ini`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # Keep docs in sync with docs env and .readthedocs.yml.
 [gh-actions]
 python =
+    3.8: py38
+    3.9: py39
     3.10: py310
     3.11: py311
     3.12: py312, lint
 
 [tox]
-envlist = py310, py311, py312, lint
+envlist = py38, py39, py310, py311, py312, lint
 isolated_build = True
 
 [testenv:lint]
 basepython = python3.12
 allowlist_externals =
     just
     pdm
```

### Comparing `tightwrap-24.1.0/.github/workflows/main.yml` & `tightwrap-24.2.0/.github/workflows/main.yml`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 jobs:
   tests:
     name: "Python ${{ matrix.python-version }}"
     runs-on: "ubuntu-latest"
 
     strategy:
       matrix:
-        python-version: ["3.10", "3.11", "3.12"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
     steps:
       - uses: "actions/checkout@v3"
 
       - uses: "actions/setup-python@v4"
         with:
           python-version: "${{ matrix.python-version }}"
@@ -80,14 +80,15 @@
         uses: "actions/upload-artifact@v3"
         with:
           name: "html-report"
           path: "htmlcov"
         if: always()
 
       - name: "Make badge"
+        if: github.ref == 'refs/heads/main'
         uses: "schneegans/dynamic-badges-action@v1.4.0"
         with:
           # GIST_TOKEN is a GitHub personal access token with scope "gist".
           auth: ${{ secrets.GIST_TOKEN }}
           gistID: 090e3ce4d18dd18bb1323538d6de8ffd
           filename: covbadge.json
           label: Coverage
```

### Comparing `tightwrap-24.1.0/.github/workflows/pypi-package.yml` & `tightwrap-24.2.0/.github/workflows/pypi-package.yml`

 * *Files identical despite different names*

### Comparing `tightwrap-24.1.0/tests/test_wraps.py` & `tightwrap-24.2.0/tests/test_wraps.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 from __future__ import annotations
 
-from inspect import signature
 from typing import Any, Callable
 
+from tightwrap import _get_resolved_signature  # pyright: ignore[reportPrivateUsage]
 from tightwrap import wraps
 
 
 def test_wraps() -> None:
     """Wraps works."""
 
     def wrapped(a: int) -> int:
         return a + 1
 
     @wraps(wrapped)
     def wrapper(a: int) -> int:
         return wrapped(a)
 
     assert wrapper(3) == 4
-    assert signature(wrapped) == signature(wrapper)
+    assert _get_resolved_signature(wrapped) == _get_resolved_signature(wrapper)
 
     _: Callable[[int], int] = wrapper
 
 
 def test_wraps_different_return() -> None:
     def wrapped(a: int) -> int:
         return a + 1
 
     @wraps(wrapped)
     def wrapper(*args: Any, **kwargs: Any) -> str:
         return str(wrapped(*args, **kwargs))
 
+    wrapped_signature = _get_resolved_signature(wrapped)
+    wrapper_signature = _get_resolved_signature(wrapper)
+
     assert wrapper(3) == "4"
-    assert signature(wrapped, eval_str=True).parameters == signature(wrapper).parameters
-    assert signature(wrapper).return_annotation is str
-    assert signature(wrapped, eval_str=True).return_annotation is int
+    assert wrapped_signature.parameters == wrapper_signature.parameters
+    assert wrapper_signature.return_annotation is str
+    assert wrapped_signature.return_annotation is int
 
     _: Callable[[int], str] = wrapper
```

### Comparing `tightwrap-24.1.0/.gitignore` & `tightwrap-24.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tightwrap-24.1.0/LICENSE` & `tightwrap-24.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tightwrap-24.1.0/README.md` & `tightwrap-24.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # tightwrap
 
 [![PyPI](https://img.shields.io/pypi/v/tightwrap.svg)](https://pypi.python.org/pypi/tightwrap)
 [![Build](https://github.com/Tinche/tightwrap/workflows/CI/badge.svg)](https://github.com/Tinche/tightwrap/actions?workflow=CI)
 [![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/Tinche/090e3ce4d18dd18bb1323538d6de8ffd/raw/covbadge.json)](https://github.com/Tinche/tightwrap/actions/workflows/main.yml)
-[![Supported Python versions](https://img.shields.io/pypi/pyversions/tightwrap.svg)](https://github.com/Tinche/tightwrap)
+[![Supported Python Versions](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2FTinche%2Ftightwrap%2Fmain%2Fpyproject.toml)](https://github.com/Tinche/tightwrap/blob/main/pyproject.toml)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 _tightwrap_ (pronounced _typed wrap_) is a drop-in replacement for [`functools.wraps`](https://docs.python.org/3/library/functools.html#functools.wraps) that works with static typing.
 _tightwrap_ is very small, so if you don't want to add a dependency to it just [vendor this file](https://github.com/Tinche/tightwrap/blob/main/src/tightwrap/__init__.py).
 
 `functools.wraps` is very commonly used to adapt runtime function signatures when wrapping functions, but it doesn't work well with static typing tools.
 `tightwrap.wraps` has the same interface and you should use it instead:
@@ -47,10 +47,14 @@
 reveal_type(wrapping)  # Revealed type is "def (*args: Any, **kwargs: Any) -> builtins.int"
 
 wrapping("a string")  # No type error, blows up at runtime.
 ```
 
 ## Changelog
 
+### 24.2.0 (2024-05-04)
+
+- Add support for Python 3.8 and 3.9.
+
 ### 24.1.0 (2024-01-09)
 
 - Initial version.
```

### Comparing `tightwrap-24.1.0/PKG-INFO` & `tightwrap-24.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,33 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: tightwrap
-Version: 24.1.0
+Version: 24.2.0
 Summary: A typed `functools.wraps`.
 Author-email: Tin Tvrtković <tinchester@gmail.com>
 License: Apache2
 License-File: LICENSE
-Requires-Python: >=3.10
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
+Requires-Dist: typing-extensions>=4.0.0; python_version <= '3.10'
 Description-Content-Type: text/markdown
 
 # tightwrap
 
 [![PyPI](https://img.shields.io/pypi/v/tightwrap.svg)](https://pypi.python.org/pypi/tightwrap)
 [![Build](https://github.com/Tinche/tightwrap/workflows/CI/badge.svg)](https://github.com/Tinche/tightwrap/actions?workflow=CI)
 [![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/Tinche/090e3ce4d18dd18bb1323538d6de8ffd/raw/covbadge.json)](https://github.com/Tinche/tightwrap/actions/workflows/main.yml)
-[![Supported Python versions](https://img.shields.io/pypi/pyversions/tightwrap.svg)](https://github.com/Tinche/tightwrap)
+[![Supported Python Versions](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2FTinche%2Ftightwrap%2Fmain%2Fpyproject.toml)](https://github.com/Tinche/tightwrap/blob/main/pyproject.toml)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 _tightwrap_ (pronounced _typed wrap_) is a drop-in replacement for [`functools.wraps`](https://docs.python.org/3/library/functools.html#functools.wraps) that works with static typing.
 _tightwrap_ is very small, so if you don't want to add a dependency to it just [vendor this file](https://github.com/Tinche/tightwrap/blob/main/src/tightwrap/__init__.py).
 
 `functools.wraps` is very commonly used to adapt runtime function signatures when wrapping functions, but it doesn't work well with static typing tools.
 `tightwrap.wraps` has the same interface and you should use it instead:
@@ -57,10 +67,14 @@
 reveal_type(wrapping)  # Revealed type is "def (*args: Any, **kwargs: Any) -> builtins.int"
 
 wrapping("a string")  # No type error, blows up at runtime.
 ```
 
 ## Changelog
 
+### 24.2.0 (2024-05-04)
+
+- Add support for Python 3.8 and 3.9.
+
 ### 24.1.0 (2024-01-09)
 
 - Initial version.
```

