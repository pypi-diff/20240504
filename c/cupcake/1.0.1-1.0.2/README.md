# Comparing `tmp/cupcake-1.0.1.tar.gz` & `tmp/cupcake-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cupcake-1.0.1.tar", max compression
+gzip compressed data, was "cupcake-1.0.2.tar", max compression
```

## Comparing `cupcake-1.0.1.tar` & `cupcake-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      761 2023-03-01 17:58:55.790012 cupcake-1.0.1/LICENSE
--rw-r--r--   0        0        0      576 2024-05-01 00:22:02.738062 cupcake-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       73 2023-03-13 22:19:09.065654 cupcake-1.0.1/src/cupcake/__init__.py
--rw-r--r--   0        0        0     3965 2024-02-28 04:41:46.514999 cupcake-1.0.1/src/cupcake/cascade.py
--rw-r--r--   0        0        0    10078 2024-02-22 06:16:05.800878 cupcake-1.0.1/src/cupcake/confee.py
--rw-r--r--   0        0        0     1027 2024-01-11 04:42:54.793235 cupcake-1.0.1/src/cupcake/data/cmake_names.py
--rw-r--r--   0        0        0       58 2024-03-30 22:14:37.710534 cupcake-1.0.1/src/cupcake/data/new/.gitignore
--rw-r--r--   0        0        0     1031 2024-04-30 21:17:59.470632 cupcake-1.0.1/src/cupcake/data/new/CMakeLists.txt
--rw-r--r--   0        0        0     2477 2024-04-29 20:21:28.383431 cupcake-1.0.1/src/cupcake/data/new/conanfile.py
--rw-r--r--   0        0        0      438 2024-03-19 14:45:33.698677 cupcake-1.0.1/src/cupcake/data/new/include/{{name}}/{{name}}.hpp
--rw-r--r--   0        0        0      103 2024-03-19 14:16:34.798335 cupcake-1.0.1/src/cupcake/data/new/src/lib{{name}}.cpp
--rw-r--r--   0        0        0      227 2024-03-19 14:16:51.427197 cupcake-1.0.1/src/cupcake/data/new/src/{{name}}.cpp
--rw-r--r--   0        0        0      470 2024-02-01 17:18:45.120789 cupcake-1.0.1/src/cupcake/data/new/tests/CMakeLists.txt
--rw-r--r--   0        0        0      203 2024-03-19 13:09:50.402090 cupcake-1.0.1/src/cupcake/data/new/tests/{{name}}.cpp
--rw-r--r--   0        0        0      177 2023-03-01 15:12:58.048397 cupcake-1.0.1/src/cupcake/data/query/CMakeLists.txt
--rw-r--r--   0        0        0     1758 2024-02-06 16:16:50.206575 cupcake-1.0.1/src/cupcake/expression.py
--rw-r--r--   0        0        0      227 2024-02-04 01:50:29.311228 cupcake-1.0.1/src/cupcake/functional.py
--rw-r--r--   0        0        0    53272 2024-05-01 00:10:40.111456 cupcake-1.0.1/src/cupcake/main.py
--rw-r--r--   0        0        0     1053 2024-04-26 23:12:40.126982 cupcake-1.0.1/src/cupcake/transformations.py
--rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 cupcake-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      761 2023-03-01 17:58:55.790012 cupcake-1.0.2/LICENSE
+-rw-r--r--   0        0        0      594 2024-05-04 21:06:45.174223 cupcake-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-03-13 22:19:09.065654 cupcake-1.0.2/src/cupcake/__init__.py
+-rw-r--r--   0        0        0     3965 2024-02-28 04:41:46.514999 cupcake-1.0.2/src/cupcake/cascade.py
+-rw-r--r--   0        0        0    10078 2024-02-22 06:16:05.800878 cupcake-1.0.2/src/cupcake/confee.py
+-rw-r--r--   0        0        0     1027 2024-01-11 04:42:54.793235 cupcake-1.0.2/src/cupcake/data/cmake_names.py
+-rw-r--r--   0        0        0       58 2024-03-30 22:14:37.710534 cupcake-1.0.2/src/cupcake/data/new/.gitignore
+-rw-r--r--   0        0        0     1031 2024-04-30 21:17:59.470632 cupcake-1.0.2/src/cupcake/data/new/CMakeLists.txt
+-rw-r--r--   0        0        0     2477 2024-04-29 20:21:28.383431 cupcake-1.0.2/src/cupcake/data/new/conanfile.py
+-rw-r--r--   0        0        0      438 2024-03-19 14:45:33.698677 cupcake-1.0.2/src/cupcake/data/new/include/{{name}}/{{name}}.hpp
+-rw-r--r--   0        0        0      103 2024-03-19 14:16:34.798335 cupcake-1.0.2/src/cupcake/data/new/src/lib{{name}}.cpp
+-rw-r--r--   0        0        0      227 2024-03-19 14:16:51.427197 cupcake-1.0.2/src/cupcake/data/new/src/{{name}}.cpp
+-rw-r--r--   0        0        0      470 2024-02-01 17:18:45.120789 cupcake-1.0.2/src/cupcake/data/new/tests/CMakeLists.txt
+-rw-r--r--   0        0        0      203 2024-03-19 13:09:50.402090 cupcake-1.0.2/src/cupcake/data/new/tests/{{name}}.cpp
+-rw-r--r--   0        0        0      177 2023-03-01 15:12:58.048397 cupcake-1.0.2/src/cupcake/data/query/CMakeLists.txt
+-rw-r--r--   0        0        0     1758 2024-02-06 16:16:50.206575 cupcake-1.0.2/src/cupcake/expression.py
+-rw-r--r--   0        0        0      227 2024-02-04 01:50:29.311228 cupcake-1.0.2/src/cupcake/functional.py
+-rw-r--r--   0        0        0    55263 2024-05-04 21:06:05.660247 cupcake-1.0.2/src/cupcake/main.py
+-rw-r--r--   0        0        0     1053 2024-04-26 23:12:40.126982 cupcake-1.0.2/src/cupcake/transformations.py
+-rw-r--r--   0        0        0      579 1970-01-01 00:00:00.000000 cupcake-1.0.2/PKG-INFO
```

### Comparing `cupcake-1.0.1/LICENSE` & `cupcake-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cupcake-1.0.1/pyproject.toml` & `cupcake-1.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "cupcake"
-version = "1.0.1"
+version = "1.0.2"
 description = "Make C++ a piece of cake."
 authors = ["John Freeman <jfreeman08@gmail.com>"]
 packages = [{include = "cupcake", from = "src"}]
 
 [tool.poetry.scripts]
 cupcake = 'cupcake.main:main'
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = "^8.0.4"
 click-option-group = "^0.5.3"
 tomlkit = "^0.10.1"
 jinja2 = "^3.1.1"
+psutil = "^5.9.8"
 
 [tool.poetry.group.dev.dependencies]
 shush = "^0.3.2"
 pytest = "^7.0.1"
 pytest-cov = "^4.1.0"
 pytest-xdist = "^3.2.1"
```

### Comparing `cupcake-1.0.1/src/cupcake/cascade.py` & `cupcake-1.0.2/src/cupcake/cascade.py`

 * *Files identical despite different names*

### Comparing `cupcake-1.0.1/src/cupcake/confee.py` & `cupcake-1.0.2/src/cupcake/confee.py`

 * *Files identical despite different names*

### Comparing `cupcake-1.0.1/src/cupcake/data/cmake_names.py` & `cupcake-1.0.2/src/cupcake/data/cmake_names.py`

 * *Files identical despite different names*

### Comparing `cupcake-1.0.1/src/cupcake/data/new/CMakeLists.txt` & `cupcake-1.0.2/src/cupcake/data/new/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cupcake-1.0.1/src/cupcake/data/new/conanfile.py` & `cupcake-1.0.2/src/cupcake/data/new/conanfile.py`

 * *Files identical despite different names*

### Comparing `cupcake-1.0.1/src/cupcake/expression.py` & `cupcake-1.0.2/src/cupcake/expression.py`

 * *Files identical despite different names*

### Comparing `cupcake-1.0.1/src/cupcake/main.py` & `cupcake-1.0.2/src/cupcake/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,27 +8,73 @@
 import itertools
 import jinja2
 import json
 import locale
 import operator
 import os
 import pathlib
+import psutil
 import re
 import shlex
 import shutil
 import subprocess
 import sys
 import tempfile
 import time
 import typing as t
 import urllib.parse
 
 from cupcake import cascade, confee, transformations
 from cupcake.expression import subject, contains
 
+_DEFAULT_JOBS = psutil.cpu_count()
+
+thresholds = [
+    (60 * 60 * 24, 'day'),
+    (60 * 60, 'hour'),
+    (60, 'minute'),
+    (1, 'second'),
+]
+
+fractions = [
+    'seconds',
+    'milliseconds',
+    'microseconds',
+    'nanoseconds',
+]
+
+def hrd(d: float) -> str:
+    """
+    Convert a machine-readable duration into a human-readable one.
+
+    Given a duration calculated by subtracting two results of a time method,
+    e.g. `time.perf_counter()`, return a friendly string like "1.23 seconds".
+    """
+    i = 0
+    while i < 3 and thresholds[i][0] > d:
+        i += 1
+    # If we are not dipping into fractional seconds, then use this formula.
+    if i < 3:
+        (d1, u1) = thresholds[i]
+        q1, r1 = divmod(d, d1)
+        if q1 > 1:
+            u1 += 's'
+        (d2, u2) =  thresholds[i+1]
+        q2, r2 = divmod(r1, d2)
+        if q2 > 1:
+            u2 += 's'
+        return f'{int(q1)} {u1}, {int(q2)} {u2}'
+    # We want 3 significant digits.
+    i = 0
+    while d < 1:
+        i += 1
+        d *= 1000
+    u = fractions[i]
+    return f'{d:.3} {u}'
+
 def run(command, *args, **kwargs):
     # TODO: Print this in a special color if writing to terminal.
     print(' '.join(shlex.quote(str(arg)) for arg in command), flush=True)
     proc = subprocess.run(command, *args, **kwargs)
     if proc.returncode != 0:
         raise SystemExit(proc.returncode)
     return proc
@@ -431,14 +477,16 @@
             args = ['-G', generator, *args]
         args = [*args, source_dir]
         env = os.environ | env
         run([self.CMAKE, *args], cwd=build_dir, env=env)
 
 TEST_TEMPLATE_ = """
 '{{ ctest }}' --test-dir '{{ cmakeDir }}'
+{% if verbosity > 0 %} --verbose {% endif %}
+{% if jobs > 1 %} --parallel {{ jobs }} {% endif %}
 {% if multiConfig %} --build-config {{ flavor }} {% endif %}
 {% if regex %} --tests-regex {{ regex }} {% endif %}
 """
 
 # We want commands to call dependencies,
 # and want them to be able to pass options.
 # That means dependent command must accept all the options of all its
@@ -601,36 +649,35 @@
         if path.is_file():
             m.update(path.read_bytes())
         for name, value in copts.items():
             m.update(name.encode())
             m.update(value.encode())
         id = m.hexdigest()
         old_flavors = state_.conan.flavors([])
-        new_flavors = list({*config_.flavors([]), flavor_})
-        diff_flavors = [f for f in new_flavors if f not in old_flavors]
         conan_dir = build_dir_ / 'conan'
-        if state_.conan:
-            if state_.conan.id() == id:
-                if not diff_flavors:
-                    return state_.conan
-            else:
-                shutil.rmtree(conan_dir, ignore_errors=True)
-                diff_flavors = new_flavors
+        if state_.conan.id(None) == id:
+            if flavor_ in old_flavors:
+                return state_.conan
+        else:
+            shutil.rmtree(conan_dir, ignore_errors=True)
+            old_flavors = []
+        new_flavors = list({*config_.flavors([]), flavor_})
+        added_flavors = [f for f in new_flavors if f not in old_flavors]
         conan_dir.mkdir(parents=True, exist_ok=True)
         command = [
             CONAN.command, 'install', source_dir_, '--build', 'missing',
             '--output-folder', conan_dir,
             '--profile:build', profile, '--profile:host', profile,
         ]
         for name, value in copts.items():
             command.extend(['--options', f'{name}={value}'])
-        for flavor in diff_flavors:
+        for flavor in added_flavors:
             with (log_dir_ / 'conan').open('wb') as stream:
                 tee(
-                    [*command, '--settings', f'build_type={FLAVORS[flavor_]}'],
+                    [*command, '--settings', f'build_type={FLAVORS[flavor]}'],
                     stream=stream,
                     cwd=conan_dir,
                 )
         state_.conan.id = id
         state_.conan.flavors = new_flavors
         # TODO: Find layout. How?
         toolchain = conan_dir / 'conan_toolchain.cmake'
@@ -772,16 +819,17 @@
         else:
             sflavors = [flavor_]
 
         cmake_dir = build_dir_ / 'cmake'
         if not multiConfig:
             cmake_dir /= flavor_
 
-        if not keep:
-            shutil.rmtree(cmake_dir, ignore_errors=True)
+        # We must remove at least the cache file.
+        removee = (cmake_dir / 'CMakeCache.txt') if keep else cmake_dir
+        shutil.rmtree(removee, ignore_errors=True)
         cmake_dir.mkdir(parents=True, exist_ok=True)
         # CMake complains if any of these variables are unused,
         # but it is impossible to predict which will be unused.
         # Don't sweat it.
         cmake_args = {}
         cmake_args['CMAKE_EXPORT_COMPILE_COMMANDS'] = 'ON'
         cmake_args['CMAKE_POLICY_DEFAULT_CMP0091'] = 'NEW'
@@ -817,29 +865,54 @@
     @cascade.value()
     def cmake_dir_(self, build_dir_, flavor_, cmake):
         build_dir_ /= 'cmake'
         if not cmake.multiConfig():
             build_dir_ /= flavor_
         return build_dir_
 
-    @cascade.command()
+    @cascade.value()
     @cascade.option(
-        '--jobs', '-j', type=int, help='Maximum number of simultaneous jobs.',
+        '--jobs', '--parallel', '-j',
+        is_flag=False, flag_value=_DEFAULT_JOBS, default=_DEFAULT_JOBS,
+        help='Maximum number of simultaneous jobs.',
     )
+    def jobs_(self, config_, jobs):
+        return confee.resolve(jobs, config_.jobs, _DEFAULT_JOBS)
+
+    @cascade.value()
+    @cascade.option('--verbose', '-v', count=True, help='Increment verbosity.')
+    @cascade.option('--quiet', '-q', count=True, help='Decrement verbosity.')
+    def verbosity_(self, config_, verbose, quiet):
+        verbosity = min(max(verbose - quiet, 0), 3)
+        return confee.resolve(verbosity, config_.verbosity, 0)
+
+    @cascade.command()
     @cascade.argument('target', required=False)
-    def build(self, config_, CMAKE, build_dir_, log_dir_, cmake_dir_, flavor_, cmake, jobs, target):
+    def build(
+        self,
+        config_,
+        CMAKE,
+        build_dir_,
+        log_dir_,
+        cmake_dir_,
+        flavor_,
+        jobs_,
+        verbosity_,
+        cmake,
+        target,
+    ):
         """Build the selected flavor."""
-        jobs = confee.resolve(jobs, config_.jobs, None)
         confee.write(config_)
-        command = [CMAKE, '--build', cmake_dir_, '--verbose']
+        command = [CMAKE, '--build', cmake_dir_]
+        if verbosity_ > 0:
+            command.append('--verbose')
+        if jobs_ > 1:
+            command.extend(['--parallel', str(jobs_)])
         if cmake.multiConfig():
             command.extend(['--config', FLAVORS[flavor_]])
-        command.append('--parallel')
-        if jobs is not None:
-            command.append(str(jobs))
         if target is not None:
             command.extend(['--target', target])
         with (log_dir_ / 'build').open('wb') as stream:
             tee(command, stream=stream)
         return cmake
 
     @cascade.command()
@@ -870,24 +943,38 @@
             FLAVORS[flavor_],
             '--prefix',
             prefix_,
         ])
 
     @cascade.command()
     @cascade.argument('regex', required=False)
-    def test(self, config_, CTEST, log_dir_, cmake_dir_, flavor_, cmake, regex):
+    def test(
+        self,
+        config_,
+        CTEST,
+        log_dir_,
+        cmake_dir_,
+        flavor_,
+        jobs_,
+        verbosity_,
+        cmake,
+        regex,
+    ):
         """Test the selected flavor."""
+        confee.write(config_)
         template = confee.resolve(None, config_.scripts.test, TEST_TEMPLATE_)
         template = jinja2.Template(template)
         context = {
             'ctest': CTEST,
             'cmakeDir': cmake_dir_,
             'multiConfig': cmake.multiConfig(),
             'flavor': FLAVORS[flavor_],
             'regex': regex,
+            'jobs': jobs_,
+            'verbosity': verbosity_,
         }
         command = shlex.split(template.render(**context))
         env = os.environ.copy()
         env['CTEST_OUTPUT_ON_FAILURE'] = 'ON'
         with (log_dir_ / 'test').open('wb') as stream:
             tee(command, stream=stream, env=env)
 
@@ -902,15 +989,15 @@
         jenv.filters['pascal'] = pascal
         jenv.filters['snake'] = snake
         return jenv
 
     @cascade.command()
     @cascade.argument('path', required=False, default='.')
     @cascade.option(
-        '--version', help='Version of requirement cupcake.cmake@github/thejohnfreeman.', default='1.0.0',
+        '--version', help='Version of requirement cupcake.cmake@github/thejohnfreeman.', default='1.0.2',
     )
     @cascade.option(
         '--special/--general', help='Whether to enable special commands.', default=True,
     )
     @cascade.option(
         '--library/--no-library', help='Whether to export a library.', default=True,
     )
@@ -1500,9 +1587,8 @@
 def main():
     start = time.time()
     try:
         Cupcake()
     finally:
         duration = time.time() - start # in seconds
         if duration > 1:
-            # TODO: Print human-friendly representation.
-            print(f'{duration:.3}s')
+            print(hrd(duration))
```

### Comparing `cupcake-1.0.1/src/cupcake/transformations.py` & `cupcake-1.0.2/src/cupcake/transformations.py`

 * *Files identical despite different names*

### Comparing `cupcake-1.0.1/PKG-INFO` & `cupcake-1.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: cupcake
-Version: 1.0.1
+Version: 1.0.2
 Summary: Make C++ a piece of cake.
 Author: John Freeman
 Author-email: jfreeman08@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.0.4,<9.0.0)
 Requires-Dist: click-option-group (>=0.5.3,<0.6.0)
 Requires-Dist: jinja2 (>=3.1.1,<4.0.0)
+Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Requires-Dist: tomlkit (>=0.10.1,<0.11.0)
```

