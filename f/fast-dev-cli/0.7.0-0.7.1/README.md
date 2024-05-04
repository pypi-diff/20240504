# Comparing `tmp/fast_dev_cli-0.7.0.tar.gz` & `tmp/fast_dev_cli-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_dev_cli-0.7.0.tar", max compression
+gzip compressed data, was "fast_dev_cli-0.7.1.tar", max compression
```

## Comparing `fast_dev_cli-0.7.0.tar` & `fast_dev_cli-0.7.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2024-03-06 06:08:37.265617 fast_dev_cli-0.7.0/LICENSE
--rw-r--r--   0        0        0     1755 2024-04-07 08:42:22.439293 fast_dev_cli-0.7.0/README.md
--rw-r--r--   0        0        0       76 2024-03-06 06:08:37.265993 fast_dev_cli-0.7.0/fast_dev_cli/__init__.py
--rw-r--r--   0        0        0       28 2024-03-06 06:08:37.266125 fast_dev_cli-0.7.0/fast_dev_cli/__main__.py
--rw-r--r--   0        0        0    20260 2024-04-18 04:13:37.056185 fast_dev_cli-0.7.0/fast_dev_cli/cli.py
--rw-r--r--   0        0        0        0 2024-03-06 06:08:37.266469 fast_dev_cli-0.7.0/fast_dev_cli/py.typed
--rw-r--r--   0        0        0     1225 2024-04-18 04:09:13.720129 fast_dev_cli-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2457 1970-01-01 00:00:00.000000 fast_dev_cli-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-03-06 06:08:37.265617 fast_dev_cli-0.7.1/LICENSE
+-rw-r--r--   0        0        0     2109 2024-04-30 08:17:16.702283 fast_dev_cli-0.7.1/README.md
+-rw-r--r--   0        0        0      392 2024-04-30 13:31:19.454648 fast_dev_cli-0.7.1/fast_dev_cli/__init__.py
+-rw-r--r--   0        0        0       28 2024-03-06 06:08:37.266125 fast_dev_cli-0.7.1/fast_dev_cli/__main__.py
+-rw-r--r--   0        0        0    20742 2024-04-30 13:35:34.884923 fast_dev_cli-0.7.1/fast_dev_cli/cli.py
+-rw-r--r--   0        0        0        0 2024-03-06 06:08:37.266469 fast_dev_cli-0.7.1/fast_dev_cli/py.typed
+-rw-r--r--   0        0        0     1407 2024-05-01 04:45:50.351656 fast_dev_cli-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     3014 1970-01-01 00:00:00.000000 fast_dev_cli-0.7.1/PKG-INFO
```

### Comparing `fast_dev_cli-0.7.0/LICENSE` & `fast_dev_cli-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_dev_cli-0.7.0/README.md` & `fast_dev_cli-0.7.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,20 @@
 </a>
 <a href="https://github.com/waketzheng/fast-dev-cli/actions?query=workflow:ci" target="_blank">
     <img src="https://github.com/waketzheng/fast-dev-cli/workflows/ci/badge.svg" alt="GithubActionResult">
 </a>
 <a href="https://coveralls.io/github/waketzheng/fast-dev-cli?branch=main" target="_blank">
     <img src="https://coveralls.io/repos/github/waketzheng/fast-dev-cli/badge.svg?branch=main" alt="Coverage Status">
 </a>
+<a href="https://github.com/astral-sh/ruff" target="_blank">
+    <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json" alt="Ruff">
+</a>
+<a href="https://github.com/python/mypy" target="_blank">
+    <img src="https://img.shields.io/badge/mypy-100%25-green.svg" alt="Mypy Coverage">
+</a>
 </p>
 
 ---
 
 **Source Code**: <a href="https://github.com/waketzheng/fast-dev-cli" target="_blank">https://github.com/waketzheng/fast-dev-cli</a>
 
 ## Requirements
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
                                  [FastDevCli]
                   TToooollkkiitt ffoorr ppyytthhoonn ccooddee lliinntt//tteesstt//bbuummpp ......
    _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_G_i_t_h_u_b_A_c_t_i_o_n_R_e_s_u_l_t_]_[_C_o_v_e_r_a_g_e
-                                    _S_t_a_t_u_s_]
+                         _S_t_a_t_u_s_]_[_R_u_f_f_]_[_M_y_p_y_ _C_o_v_e_r_a_g_e_]
 --- **Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_w_a_k_e_t_z_h_e_n_g_/_f_a_s_t_-_d_e_v_-_c_l_i ## Requirements
 Python 3.11+ ## Installation
 ```console $ pip install "fast-dev-cli[all]" ---> 100% Successfully installed
 fast-dev-cli isort black ruff mypy typer bumpversion pytest coverage ```
 ## Usage - Lint py code: ```bash fast lint /path/to/file-or-directory ``` -
 Check only ```bash fast check ``` - Bump up version in pyproject.toml ```bash
 fast bump ``` - Run unittest and report coverage ```bash fast test ``` - Export
```

### Comparing `fast_dev_cli-0.7.0/fast_dev_cli/cli.py` & `fast_dev_cli-0.7.1/fast_dev_cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 import importlib.metadata
 import os
 import re
 import subprocess
 import sys
-from enum import StrEnum
 from functools import cached_property
 from pathlib import Path
 from subprocess import CompletedProcess
-from typing import Self, Type
+from typing import Type
+
+if sys.version_info >= (3, 11):
+    from enum import StrEnum
+    from typing import Self
+else:  # pragma: no cover
+    from strenum import StrEnum  # type:ignore[no-redef,assignment]
+    from typing_extensions import Self
+
 
 __version__ = importlib.metadata.version(Path(__file__).parent.name)
 
 
 def parse_files(args: list[str] | tuple[str, ...]) -> list[str]:
     return [i for i in args if not i.startswith("-")]
 
@@ -376,16 +383,17 @@
         cls: Type[Self], toml_text: str | None = None
     ) -> tuple[list[str], list[str], list[list[str]], str]:
         if toml_text is None:
             toml_text = cls.load_toml_text()
         main_title = "[tool.poetry.dependencies]"
         text = toml_text.split(main_title)[-1]
         dev_flag = "--group dev"
-        if (dev_title := cls.DevFlag.new.value) not in text:
-            dev_title = cls.DevFlag.old.value  # For poetry<=1.2
+        new_flag, old_flag = cls.DevFlag.new, cls.DevFlag.old
+        if (dev_title := getattr(new_flag, "value", new_flag)) not in text:
+            dev_title = getattr(old_flag, "value", old_flag)  # For poetry<=1.2
             dev_flag = "--dev"
         others: list[list[str]] = []
         try:
             main_toml, dev_toml = text.split(dev_title)
         except ValueError:
             dev_toml = ""
             main_toml = text
@@ -592,20 +600,23 @@
 def _should_run_test_script(path: Path) -> bool:
     return path.exists()
 
 
 @cli.command()
 def test(
     dry: bool = Option(False, "--dry", help="Only print, not really run shell command"),
+    ignore_script: bool = Option(False, "--ignore-script", "-i"),
 ) -> None:
     """Run unittest by pytest and report coverage"""
     cwd = Path.cwd()
     root = Project.get_work_dir(cwd=cwd, allow_cwd=True)
     test_script = root / "scripts" / "test.sh"
-    if _should_run_test_script(test_script):
+    if not isinstance(ignore_script, bool):
+        ignore_script = getattr(ignore_script, "default", False)
+    if not ignore_script and _should_run_test_script(test_script):
         cmd = f"sh {test_script.relative_to(root)}"
         if cwd != root:
             cmd = f"cd {root} && " + cmd
     else:
         cmd = 'coverage run -m pytest -s && coverage report --omit="tests/*" -m'
         if not is_venv() or not check_call("coverage --version"):
             sep = " && "
```

### Comparing `fast_dev_cli-0.7.0/pyproject.toml` & `fast_dev_cli-0.7.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,53 +1,50 @@
 [tool.poetry]
 name = "fast-dev-cli"
-version = "0.7.0"
+version = "0.7.1"
 description = ""
 authors = ["Waket Zheng <waketzheng@gmail.com>"]
 readme = "README.md"
 packages = [{include = "fast_dev_cli"}]
 
 [tool.poetry.dependencies]
-python = "^3.11"
-click = ">=7.1.1"
-ruff = {version = ">=0.3", optional = true}
-mypy = {version = ">=1.5.0", optional = true}
+python = "^3.10"
+click = ">=7.1.1"  # Many package depends on click, so only limit min version
+strenum = {version = ">=0.4.15", python = "<3.11"}
+type-extensions = {version = ">=0.1.2", python = "<3.11"}
 coverage = {version = ">=6.5.0", optional = true}
+ruff = {version = "^0.4.2", optional = true}
+mypy = {version = "^1.10.0", optional = true}
 bumpversion = {version = "^0.6.0", optional = true}
-pytest = {version = "^8.1.1", optional = true}
-typer = {version = ">=0.12.0", optional = true}
+pytest = {version = "^8.2.0", optional = true}
+typer = {version = "^0.12.3", optional = true}
 
 [tool.poetry.extras]
 all = ["ruff", "typer", "mypy", "bumpversion", "pytest", "coverage"]
 
 [tool.poetry.group.dev.dependencies]
-ruff = ">=0.3"
-mypy = "*"
-pytest = "*"
-coverage = "*"
-bumpversion = "*"
-typer = {extras = ["all"], version = "*"}
-ipython = "^8.23.0"
-coveralls = "^3.3.1"
+coveralls = {version = ">=4.0.0", python = ">=3.10,<3.13"}
+coverage = ">=6.5.0"  # use >= to compare with coveralls
+typer = "^0.12.3"
+ruff = "^0.4.2"
+mypy = "^1.10.0"
+pytest = "^8.2.0"
+ipython = "^8.24.0"
+bumpversion = "^0.6.0"
 pytest-mock = "^3.14.0"
+type-extensions = "^0.1.2"
+strenum = "^0.4.15"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-fast = "fast_dev_cli:cli"
-
-[tool.ruff]
-target-version = "py311"
+fast = "fast_dev_cli:cli.cli"
 
 [tool.mypy]
 pretty = true
 ignore_missing_imports = true
 check_untyped_defs = true
 
-[[tool.mypy.overrides]]
-module = ["tests.*"]
-check_untyped_defs = false
-
 [tool.ruff.lint.per-file-ignores]
 "test_*.py" = ["E501"]
```

### Comparing `fast_dev_cli-0.7.0/PKG-INFO` & `fast_dev_cli-0.7.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: fast-dev-cli
-Version: 0.7.0
+Version: 0.7.1
 Summary: 
 Author: Waket Zheng
 Author-email: waketzheng@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: all
 Requires-Dist: bumpversion (>=0.6.0,<0.7.0) ; extra == "all"
 Requires-Dist: click (>=7.1.1)
 Requires-Dist: coverage (>=6.5.0) ; extra == "all"
-Requires-Dist: mypy (>=1.5.0) ; extra == "all"
-Requires-Dist: pytest (>=8.1.1,<9.0.0) ; extra == "all"
-Requires-Dist: ruff (>=0.3) ; extra == "all"
-Requires-Dist: typer (>=0.12.0) ; extra == "all"
+Requires-Dist: mypy (>=1.10.0,<2.0.0) ; extra == "all"
+Requires-Dist: pytest (>=8.2.0,<9.0.0) ; extra == "all"
+Requires-Dist: ruff (>=0.4.2,<0.5.0) ; extra == "all"
+Requires-Dist: strenum (>=0.4.15) ; python_version < "3.11"
+Requires-Dist: type-extensions (>=0.1.2) ; python_version < "3.11"
+Requires-Dist: typer (>=0.12.3,<0.13.0) ; extra == "all"
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://fastdevcli.waketzheng.top/img/logo-margin/logo-teal.png" alt="FastDevCli">
 </p>
 <p align="center">
     <em>Toolkit for python code lint/test/bump ...</em>
@@ -33,14 +36,20 @@
 </a>
 <a href="https://github.com/waketzheng/fast-dev-cli/actions?query=workflow:ci" target="_blank">
     <img src="https://github.com/waketzheng/fast-dev-cli/workflows/ci/badge.svg" alt="GithubActionResult">
 </a>
 <a href="https://coveralls.io/github/waketzheng/fast-dev-cli?branch=main" target="_blank">
     <img src="https://coveralls.io/repos/github/waketzheng/fast-dev-cli/badge.svg?branch=main" alt="Coverage Status">
 </a>
+<a href="https://github.com/astral-sh/ruff" target="_blank">
+    <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json" alt="Ruff">
+</a>
+<a href="https://github.com/python/mypy" target="_blank">
+    <img src="https://img.shields.io/badge/mypy-100%25-green.svg" alt="Mypy Coverage">
+</a>
 </p>
 
 ---
 
 **Source Code**: <a href="https://github.com/waketzheng/fast-dev-cli" target="_blank">https://github.com/waketzheng/fast-dev-cli</a>
 
 ## Requirements
```

#### html2text {}

```diff
@@ -1,21 +1,23 @@
-Metadata-Version: 2.1 Name: fast-dev-cli Version: 0.7.0 Summary: Author: Waket
-Zheng Author-email: waketzheng@gmail.com Requires-Python: >=3.11,<4.0
+Metadata-Version: 2.1 Name: fast-dev-cli Version: 0.7.1 Summary: Author: Waket
+Zheng Author-email: waketzheng@gmail.com Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Provides-Extra: all Requires-Dist: bumpversion (>=0.6.0,<0.7.0) ; extra ==
-"all" Requires-Dist: click (>=7.1.1) Requires-Dist: coverage (>=6.5.0) ; extra
-== "all" Requires-Dist: mypy (>=1.5.0) ; extra == "all" Requires-Dist: pytest
-(>=8.1.1,<9.0.0) ; extra == "all" Requires-Dist: ruff (>=0.3) ; extra == "all"
-Requires-Dist: typer (>=0.12.0) ; extra == "all" Description-Content-Type:
-text/markdown
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Provides-Extra: all
+Requires-Dist: bumpversion (>=0.6.0,<0.7.0) ; extra == "all" Requires-Dist:
+click (>=7.1.1) Requires-Dist: coverage (>=6.5.0) ; extra == "all" Requires-
+Dist: mypy (>=1.10.0,<2.0.0) ; extra == "all" Requires-Dist: pytest
+(>=8.2.0,<9.0.0) ; extra == "all" Requires-Dist: ruff (>=0.4.2,<0.5.0) ; extra
+== "all" Requires-Dist: strenum (>=0.4.15) ; python_version < "3.11" Requires-
+Dist: type-extensions (>=0.1.2) ; python_version < "3.11" Requires-Dist: typer
+(>=0.12.3,<0.13.0) ; extra == "all" Description-Content-Type: text/markdown
                                  [FastDevCli]
                   TToooollkkiitt ffoorr ppyytthhoonn ccooddee lliinntt//tteesstt//bbuummpp ......
    _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_G_i_t_h_u_b_A_c_t_i_o_n_R_e_s_u_l_t_]_[_C_o_v_e_r_a_g_e
-                                    _S_t_a_t_u_s_]
+                         _S_t_a_t_u_s_]_[_R_u_f_f_]_[_M_y_p_y_ _C_o_v_e_r_a_g_e_]
 --- **Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_w_a_k_e_t_z_h_e_n_g_/_f_a_s_t_-_d_e_v_-_c_l_i ## Requirements
 Python 3.11+ ## Installation
 ```console $ pip install "fast-dev-cli[all]" ---> 100% Successfully installed
 fast-dev-cli isort black ruff mypy typer bumpversion pytest coverage ```
 ## Usage - Lint py code: ```bash fast lint /path/to/file-or-directory ``` -
 Check only ```bash fast check ``` - Bump up version in pyproject.toml ```bash
 fast bump ``` - Run unittest and report coverage ```bash fast test ``` - Export
```

