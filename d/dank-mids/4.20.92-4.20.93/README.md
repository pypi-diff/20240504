# Comparing `tmp/dank_mids-4.20.92.tar.gz` & `tmp/dank_mids-4.20.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dank_mids-4.20.92.tar", last modified: Tue Apr 30 10:14:18 2024, max compression
+gzip compressed data, was "dank_mids-4.20.93.tar", last modified: Fri May  3 23:28:53 2024, max compression
```

## Comparing `dank_mids-4.20.92.tar` & `dank_mids-4.20.93.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:18.149071 dank_mids-4.20.92/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:18.137071 dank_mids-4.20.92/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:18.141071 dank_mids-4.20.92/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-30 10:14:06.000000 dank_mids-4.20.92/.github/workflows/deploy-docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-30 10:14:06.000000 dank_mids-4.20.92/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-30 10:14:06.000000 dank_mids-4.20.92/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-30 10:14:06.000000 dank_mids-4.20.92/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-30 10:14:06.000000 dank_mids-4.20.92/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-30 10:14:06.000000 dank_mids-4.20.92/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-30 10:14:18.149071 dank_mids-4.20.92/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-30 10:14:06.000000 dank_mids-4.20.92/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:18.141071 dank_mids-4.20.92/dank_mids/
--rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/ENVIRONMENT_VARIABLES.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/_batch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:18.145071 dank_mids-4.20.92/dank_mids/_debugging/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/_debugging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/_debugging/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/_debugging/failures.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/_demo_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/_envs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)    41591 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/_uid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:18.145071 dank_mids-4.20.92/dank_mids/brownie_patch/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/brownie_patch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/brownie_patch/_abi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/brownie_patch/_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/brownie_patch/call.py
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/brownie_patch/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/brownie_patch/overloaded.py
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/brownie_patch/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12236 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:18.145071 dank_mids-4.20.92/dank_mids/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/helpers/_codec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/helpers/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/helpers/_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/semaphore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/semaphores.py
--rw-r--r--   0 runner    (1001) docker     (127)     9291 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     8729 2024-04-30 10:14:06.000000 dank_mids-4.20.92/dank_mids/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:18.149071 dank_mids-4.20.92/dank_mids.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-30 10:14:18.000000 dank_mids-4.20.92/dank_mids.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-30 10:14:18.000000 dank_mids-4.20.92/dank_mids.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 10:14:18.000000 dank_mids-4.20.92/dank_mids.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-30 10:14:18.000000 dank_mids-4.20.92/dank_mids.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 10:14:18.000000 dank_mids-4.20.92/dank_mids.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:18.145071 dank_mids-4.20.92/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:18.137071 dank_mids-4.20.92/docs/_build/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:18.137071 dank_mids-4.20.92/docs/_build/html/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:18.149071 dank_mids-4.20.92/docs/_build/html/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    11230 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/_build/html/_static/alabaster.css
--rw-r--r--   0 runner    (1001) docker     (127)    15059 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/_build/html/_static/basic.css
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/_build/html/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/_build/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/_build/html/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/_build/html/_static/language_data.js
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/_build/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/_build/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/_build/html/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (127)    18215 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-30 10:14:06.000000 dank_mids-4.20.92/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:18.149071 dank_mids-4.20.92/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-30 10:14:06.000000 dank_mids-4.20.92/examples/dank_brownie_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 10:14:06.000000 dank_mids-4.20.92/license
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-30 10:14:06.000000 dank_mids-4.20.92/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-30 10:14:06.000000 dank_mids-4.20.92/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-30 10:14:06.000000 dank_mids-4.20.92/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-30 10:14:18.149071 dank_mids-4.20.92/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-30 10:14:06.000000 dank_mids-4.20.92/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:18.149071 dank_mids-4.20.92/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 10:14:06.000000 dank_mids-4.20.92/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-30 10:14:06.000000 dank_mids-4.20.92/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    16155 2024-04-30 10:14:06.000000 dank_mids-4.20.92/tests/test_brownie_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-30 10:14:06.000000 dank_mids-4.20.92/tests/test_dank_mids.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-30 10:14:06.000000 dank_mids-4.20.92/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:28:53.283865 dank_mids-4.20.93/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:28:53.271865 dank_mids-4.20.93/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:28:53.275865 dank_mids-4.20.93/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-03 23:28:42.000000 dank_mids-4.20.93/.github/workflows/deploy-docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-03 23:28:42.000000 dank_mids-4.20.93/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-03 23:28:42.000000 dank_mids-4.20.93/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-03 23:28:42.000000 dank_mids-4.20.93/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-03 23:28:42.000000 dank_mids-4.20.93/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-03 23:28:42.000000 dank_mids-4.20.93/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-03 23:28:53.283865 dank_mids-4.20.93/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-03 23:28:42.000000 dank_mids-4.20.93/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:28:53.279865 dank_mids-4.20.93/dank_mids/
+-rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/ENVIRONMENT_VARIABLES.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/_batch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:28:53.279865 dank_mids-4.20.93/dank_mids/_debugging/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/_debugging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/_debugging/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/_debugging/failures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/_demo_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/_envs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44253 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/_uid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:28:53.279865 dank_mids-4.20.93/dank_mids/brownie_patch/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/brownie_patch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/brownie_patch/_abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/brownie_patch/_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/brownie_patch/call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/brownie_patch/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/brownie_patch/overloaded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/brownie_patch/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12986 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:28:53.279865 dank_mids-4.20.93/dank_mids/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/helpers/_codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/helpers/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8124 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/helpers/_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/semaphores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9348 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8838 2024-05-03 23:28:42.000000 dank_mids-4.20.93/dank_mids/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:28:53.283865 dank_mids-4.20.93/dank_mids.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-03 23:28:53.000000 dank_mids-4.20.93/dank_mids.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-03 23:28:53.000000 dank_mids-4.20.93/dank_mids.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 23:28:53.000000 dank_mids-4.20.93/dank_mids.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-03 23:28:53.000000 dank_mids-4.20.93/dank_mids.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 23:28:53.000000 dank_mids-4.20.93/dank_mids.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:28:53.279865 dank_mids-4.20.93/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-03 23:28:42.000000 dank_mids-4.20.93/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:28:53.275865 dank_mids-4.20.93/docs/_build/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:28:53.275865 dank_mids-4.20.93/docs/_build/html/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:28:53.283865 dank_mids-4.20.93/docs/_build/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    11230 2024-05-03 23:28:42.000000 dank_mids-4.20.93/docs/_build/html/_static/alabaster.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15059 2024-05-03 23:28:42.000000 dank_mids-4.20.93/docs/_build/html/_static/basic.css
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-03 23:28:42.000000 dank_mids-4.20.93/docs/_build/html/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-05-03 23:28:42.000000 dank_mids-4.20.93/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-03 23:28:42.000000 dank_mids-4.20.93/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-03 23:28:42.000000 dank_mids-4.20.93/docs/_build/html/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-05-03 23:28:42.000000 dank_mids-4.20.93/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-03 23:28:42.000000 dank_mids-4.20.93/docs/_build/html/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-03 23:28:42.000000 dank_mids-4.20.93/docs/_build/html/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-05-03 23:28:42.000000 dank_mids-4.20.93/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18215 2024-05-03 23:28:42.000000 dank_mids-4.20.93/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-03 23:28:42.000000 dank_mids-4.20.93/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-03 23:28:42.000000 dank_mids-4.20.93/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-03 23:28:42.000000 dank_mids-4.20.93/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-03 23:28:42.000000 dank_mids-4.20.93/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:28:53.283865 dank_mids-4.20.93/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-03 23:28:42.000000 dank_mids-4.20.93/examples/dank_brownie_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-03 23:28:42.000000 dank_mids-4.20.93/license
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-03 23:28:42.000000 dank_mids-4.20.93/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-03 23:28:42.000000 dank_mids-4.20.93/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-03 23:28:42.000000 dank_mids-4.20.93/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-03 23:28:53.283865 dank_mids-4.20.93/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-03 23:28:42.000000 dank_mids-4.20.93/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 23:28:53.283865 dank_mids-4.20.93/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 23:28:42.000000 dank_mids-4.20.93/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-03 23:28:42.000000 dank_mids-4.20.93/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16155 2024-05-03 23:28:42.000000 dank_mids-4.20.93/tests/test_brownie_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-05-03 23:28:42.000000 dank_mids-4.20.93/tests/test_dank_mids.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-03 23:28:42.000000 dank_mids-4.20.93/tests/test_examples.py
```

### Comparing `dank_mids-4.20.92/.github/workflows/deploy-docs.yaml` & `dank_mids-4.20.93/.github/workflows/deploy-docs.yaml`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.92/.github/workflows/mypy.yaml` & `dank_mids-4.20.93/.github/workflows/mypy.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -19,11 +19,11 @@
       uses: actions/setup-python@v2
       with:
         python-version: "3.9"
 
     - name: Install MyPy
       run: |
         python -m pip install --upgrade pip
-        pip install mypy types-requests
+        pip install mypy types-requests types-aiofiles
 
     - name: Run MyPy
       run: mypy ./dank_mids --pretty --ignore-missing-imports --show-error-codes --show-error-context --no-warn-no-return
```

### Comparing `dank_mids-4.20.92/.github/workflows/pytest.yaml` & `dank_mids-4.20.93/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.92/.github/workflows/release.yaml` & `dank_mids-4.20.93/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.92/PKG-INFO` & `dank_mids-4.20.93/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dank_mids
-Version: 4.20.92
+Version: 4.20.93
 Summary: Multicall batching middleware for asynchronous scripts using web3.py
 Home-page: https://github.com/BobTheBuidler/dank_mids
 Author: BobTheBuidler
 Author-email: bobthebuidlerdefi@gmail.com
 License: MIT
 Requires-Dist: aiofiles
 Requires-Dist: eth_retry<0.2,>=0.1.15
```

### Comparing `dank_mids-4.20.92/README.md` & `dank_mids-4.20.93/README.md`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.92/dank_mids/ENVIRONMENT_VARIABLES.py` & `dank_mids-4.20.93/dank_mids/ENVIRONMENT_VARIABLES.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-# type: ignore [attr-defined]
+# mypy: disable-error-code="attr-defined,dict-item"
 import logging
+from typing import Dict
 
 import a_sync
 import typed_envs
 from a_sync import AsyncProcessPoolExecutor
 
 from dank_mids import _envs
 from dank_mids._mode import OperationMode
@@ -65,15 +66,15 @@
 # NOTE: COLLECT_STATS is implemented
 COLLECT_STATS = _envs.create_env("COLLECT_STATS", bool, default=EXPORT_STATS, verbose=not EXPORT_STATS)
 
 # You probably don't need to use this unless you know you need to
 STUCK_CALL_TIMEOUT = _envs.create_env("STUCK_CALL_TIMEOUT", int, default=60*60*2)
 
 # Method-specific Semaphores
-method_semaphores = {
+method_semaphores: Dict[str, a_sync.Semaphore] = {
     "eth_call": _envs.create_env("ETH_CALL_SEMAPHORE", BlockSemaphore, default=BROWNIE_CALL_SEMAPHORE._value, string_converter=int, verbose=False),
     "eth_getBlock": _envs.create_env("ETH_GETBLOCK_SEMAPHORE", a_sync.Semaphore, default=1_000, string_converter=int, verbose=False),
     "eth_getLogs": _envs.create_env("ETH_GETLOGS_SEMAPHORE", a_sync.Semaphore, default=64, string_converter=int, verbose=False),
     "eth_getTransaction": _envs.create_env("ETH_GETTRANSACTION_SEMAPHORE", a_sync.Semaphore, default=1_000, string_converter=int, verbose=False),
     "eth_getCode": _envs.create_env("ETH_GETCODE_SEMAPHORE", a_sync.Semaphore, default=5_000, string_converter=int, verbose=False),
 }
```

### Comparing `dank_mids-4.20.92/dank_mids/__init__.py` & `dank_mids-4.20.93/dank_mids/__init__.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.92/dank_mids/_batch.py` & `dank_mids-4.20.93/dank_mids/_batch.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 
 import asyncio
 import logging
-from typing import TYPE_CHECKING, Any, Generator, List
+from typing import TYPE_CHECKING, Any, Awaitable, Generator, List, Union
 
 from dank_mids._exceptions import DankMidsInternalError
-from dank_mids._requests import JSONRPCBatch, RPCRequest, _Batch
-from dank_mids.types import Multicalls
+from dank_mids._requests import _Batch, JSONRPCBatch, Multicall, RPCRequest
+from dank_mids.types import Multicalls, RawResponse
 
 if TYPE_CHECKING:
     from dank_mids.controller import DankMiddlewareController
 
 MIN_SIZE = 1  # TODO: Play with this
 CHECK = MIN_SIZE - 1
 
 logger = logging.getLogger(__name__)
 
 class DankBatch:
     __slots__ = 'controller', 'multicalls', 'rpc_calls', '_started'
     """ A batch of jsonrpc batches. This is pretty much deprecated and needs to be refactored away."""
-    def __init__(self, controller: "DankMiddlewareController", multicalls: Multicalls, rpc_calls: List[RPCRequest]):
+    def __init__(self, controller: "DankMiddlewareController", multicalls: Multicalls, rpc_calls: List[Union[Multicall, RPCRequest]]):
         self.controller = controller
         self.multicalls = multicalls
         self.rpc_calls = rpc_calls
         self._started = False
     
     def __await__(self) -> Generator[Any, None, Any]:
         self.start()
@@ -40,15 +40,15 @@
         for mcall in self.multicalls.values():
             mcall.start(self, cleanup=False)
         for call in self.rpc_calls:
             call.start(self)
         self._started = True
     
     @property
-    def coroutines(self) -> Generator["_Batch", None, None]:
+    def coroutines(self) -> Generator[Union["_Batch", Awaitable[RawResponse]], None, None]:
         # Combine multicalls into one or more jsonrpc batches
 
         # Create empty batch
         working_batch = JSONRPCBatch(self.controller)
 
         check_len = min(CHECK, self.controller.batcher.step)
         # Go thru the multicalls and add calls to the batch
@@ -69,10 +69,10 @@
                 yield working_batch
                 working_batch = JSONRPCBatch(self.controller)
             working_batch.append(rpc_calls_to_batch.pop(), skip_check=True)
         if working_batch:
             if working_batch.is_single_multicall:
                 yield working_batch[0]  # type: ignore [misc]
             elif len(working_batch) == 1:
-                yield working_batch[0].make_request()
+                yield working_batch[0].make_request()  # type: ignore [union-attr]
             else:
                 yield working_batch
```

### Comparing `dank_mids-4.20.92/dank_mids/_debugging/_base.py` & `dank_mids-4.20.93/dank_mids/_debugging/_base.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.92/dank_mids/_debugging/failures.py` & `dank_mids-4.20.93/dank_mids/_debugging/failures.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.92/dank_mids/_exceptions.py` & `dank_mids-4.20.93/dank_mids/_exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,11 +42,11 @@
         super().__init__(exc.request_info, exc.history, status=exc.status, message=exc.message, headers=exc.headers)
         self.args = (*self.args, request)
         self._exception = exc
 
 internal_err_types = Union[AttributeError, TypeError, UnboundLocalError, NotImplementedError, RuntimeError, SyntaxError]
 
 class DankMidsInternalError(Exception):
-    def __init__(self, e: internal_err_types) -> None:
+    def __init__(self, e: Union[ValueError, internal_err_types]) -> None:
         logger.warning(f"unhandled exception inside dank mids internals: {e}", exc_info=True)
         self._original_exception = e
         super().__init__(e.__repr__())
```

### Comparing `dank_mids-4.20.92/dank_mids/_mode.py` & `dank_mids-4.20.93/dank_mids/_mode.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.92/dank_mids/_requests.py` & `dank_mids-4.20.93/dank_mids/_requests.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,30 +3,29 @@
 import asyncio
 import logging
 import time
 import weakref
 from collections import defaultdict
 from concurrent.futures.process import BrokenProcessPool
 from contextlib import suppress
-from functools import cached_property, lru_cache, partial
+from functools import cached_property, lru_cache
 from typing import (TYPE_CHECKING, Any, DefaultDict, Dict, Generator, Generic,
-                    Iterable, Iterator, List, NoReturn, Optional, Tuple,
-                    TypeVar, Union)
+                    Iterable, Iterator, List, Optional, Tuple, TypeVar, Union,
+                    overload)
 
 import a_sync
 import eth_retry
-import msgspec
 from a_sync import AsyncProcessPoolExecutor, PruningThreadPoolExecutor
 from aiohttp.client_exceptions import ClientResponseError
 from eth_abi import abi, decoding
 from eth_typing import ChecksumAddress
 from eth_utils import function_signature_to_4byte_selector
 from hexbytes import HexBytes
-from typing_extensions import Self
 from web3.types import RPCEndpoint, RPCResponse
+from web3.types import RPCError as _RPCError
 
 from dank_mids import ENVIRONMENT_VARIABLES as ENVS
 from dank_mids import _debugging, constants, stats
 from dank_mids._demo_mode import demo_logger
 from dank_mids._exceptions import (BadResponse, DankMidsClientResponseError,
                                    DankMidsInternalError, EmptyBatch,
                                    ExceedsMaxBatchSize, PayloadTooLarge,
@@ -35,21 +34,25 @@
 from dank_mids.helpers import _codec, _session
 from dank_mids.helpers._helpers import set_done
 from dank_mids.types import (BatchId, BlockId, JSONRPCBatchResponse,
                              JsonrpcParams, PartialRequest, PartialResponse,
                              RawResponse, Request, Response)
 
 if TYPE_CHECKING:
+    from dank_mids._batch import DankBatch
     from dank_mids.controller import (DankMiddlewareController,
                                       _MulticallContract)
 
 
 logger = logging.getLogger(__name__)
 
-_Response = TypeVar("_Response", Response, List[Response], RPCResponse, List[RPCResponse])
+_Response = TypeVar("_Response", Response, List[Response], RPCResponse, List[RPCResponse], RawResponse)
+
+class RPCError(_RPCError, total=False):
+    dankmids_added_context: Dict[str, Any]
 
 class _RequestEvent(a_sync.Event):
     def __init__(self, owner: "_RequestMeta") -> None:
         super().__init__(debug_daemon_interval=300)
         self._owner = weakref.proxy(owner)
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} object at {hex(id(self))} [{'set' if self.is_set() else 'unset'}, waiter:{self._owner}>"
@@ -61,37 +64,42 @@
             self._loop.call_soon_threadsafe(super().set)
 
 class _RequestMeta(Generic[_Response], metaclass=abc.ABCMeta):
     __slots__ = 'controller', 'uid', '_response', '_done', '_start', '_batch', '__weakref__'
     controller: "DankMiddlewareController"
     def __init__(self) -> None:
         self.uid = self.controller.call_uid.next
-        self._response: Optional[_Response] = None
+        self._response: Union[_Response, RPCResponse, Exception, None] = None
         self._done = _RequestEvent(self)
         self._start = time.time()
     
-    def __await__(self) -> Generator[Any, None, Optional[_Response]]:
+    def __await__(self) -> Generator[Any, None, _Response]:
         return self.get_response().__await__()
     
     @abc.abstractmethod
     def __len__(self) -> int:
         pass
 
     @property
     def response(self) -> _Response:
         if not self._done.is_set():
             raise ResponseNotReady(self)
         return self._response
 
     @abc.abstractmethod
-    async def get_response(self) -> Optional[_Response]:
+    async def get_response(self) -> _Response:
+        pass
+    
+    @abc.abstractmethod
+    def start(self, batch: Union["_Batch", "DankBatch", None] = None) -> None:
         pass
 
     async def _debug_daemon(self) -> None:
-        while not self._done.is_set():
+        # NOTE: _resonse works for RPCRequst and eth_call, _done works for _Batch classes
+        while self and self._response is None and not self._done.is_set():
             await asyncio.sleep(60)
             if not self._done.is_set():
                 logger.debug(f"{self} has not received data after {time.time() - self._start}s")
             
 
 ### Single requests:
 
@@ -99,24 +107,23 @@
 
 @lru_cache(maxsize=None)
 def _should_batch_method(method: str) -> bool:
     return all(bypass not in method for bypass in BYPASS_METHODS)
 
 class RPCRequest(_RequestMeta[RawResponse]):
     __slots__ = 'method', 'params', 'should_batch', '_started', '_retry', '_daemon'
-    dict_responses = set()
-    str_responses = set()
-
-    _types = set()
-
     def __init__(self, controller: "DankMiddlewareController", method: RPCEndpoint, params: Any, retry: bool = False):
-        self.controller = weakref.proxy(controller)
+        self.controller = controller
+        """The DankMiddlewareController that created this request."""
         self.method = method
+        """The rpc method for this request."""
         self.params = params
+        """The parameters to send with this request, if any."""
         self.should_batch = _should_batch_method(method)
+        """Returns `True` if this request should be batched with others into a jsonrpc batch request, `False` if it should be sent as an individual request."""
         self._started = False
         self._retry = retry
         super().__init__()
 
         with self.controller.pools_closed_lock:
             if isinstance(self, eth_call) and self.multicall_compatible:
                 self.controller.pending_eth_calls[self.block].append(self)
@@ -127,39 +134,39 @@
             self._daemon = asyncio.create_task(self._debug_daemon())
     
     def __eq__(self, __o: object) -> bool:
         return self.uid == __o.uid if isinstance(__o, self.__class__) else False 
     
     def __len__(self) -> int:
         # we dont need to consider this for v small batch sizes
-        if ENVS.MAX_JSONRPC_BATCH_SIZE > 50:
+        if ENVS.MAX_JSONRPC_BATCH_SIZE > 50:  # type: ignore [operator]
             # NOTE: These are totally arbitrary
             if self.method == "eth_getTransactionReceipt":
                 return 10
             elif any(m in self.method for m in ["eth_getCode" "eth_getBlockBy", "eth_getTransaction"]):
                 return 6
         return 1
     
     def __repr__(self) -> str:
-        return f"<{self.__class__.__name__} uid={self.uid} method={self.method}>"
+        return f"<{self.__class__.__name__} uid={self.uid} method={self.method} params={self.params}>"
 
     @property
     def request(self) -> Union[Request, PartialRequest]:
         return self.controller.request_type(method=self.method, params=self.params, id=self.uid)
     
-    def start(self, batch: "_Batch") -> None:
+    def start(self, batch: Union["_Batch", "DankBatch"]) -> None:  # type: ignore [override]
         self._started = True
         self._batch = batch
 
     @set_done
-    async def get_response(self) -> RPCResponse:
+    async def get_response(self) -> RPCResponse:  # type: ignore [override]
         if not self.should_batch:
             logger.debug(f"bypassed, method is {self.method}")
             try:
-                await asyncio.wait_for(self.make_request(), timeout=ENVS.STUCK_CALL_TIMEOUT)
+                await asyncio.wait_for(self.make_request(), timeout=ENVS.STUCK_CALL_TIMEOUT)  # type: ignore [arg-type]
             except asyncio.TimeoutError:
                 return await self.create_duplicate()
             return self.response.decode(partial=True).to_dict(self.method)
         
         if self._started and not self._batch._started:
             # NOTE: If we're already started, we filled a batch. Let's await it now so we can send something to the node.
             await self._batch
@@ -169,36 +176,37 @@
         if not self._started:
             try:
                 await asyncio.wait_for(
                     # If this timeout fails, we go nuclear and destroy the batch.
                     # Any calls that already succeeded will have already completed on the client side.
                     # Any calls that have not yet completed with results will be recreated, rebatched (potentially bringing better results?), and retried
                     self.controller.execute_batch(),
-                    timeout=ENVS.STUCK_CALL_TIMEOUT,
+                    timeout=ENVS.STUCK_CALL_TIMEOUT,  # type: ignore [arg-type]
                 )
             except asyncio.TimeoutError:
                 return await self.create_duplicate()
         
         try:
-            await asyncio.wait_for(self._done.wait(), timeout=ENVS.STUCK_CALL_TIMEOUT)
+            await asyncio.wait_for(self._done.wait(), timeout=ENVS.STUCK_CALL_TIMEOUT)  # type: ignore [arg-type]
         except asyncio.TimeoutError:
             return await self.create_duplicate()
 
         # JIT json decoding
         if isinstance(self.response, RawResponse):
             response = self.response.decode(partial=True).to_dict(self.method)
-            if 'error' in response:
-                if response['error']['message'].lower() in ['invalid request', 'parse error']:
+            error: Optional[RPCError]
+            if error := response.get('error'):  # type: ignore [assignment]
+                if error['message'].lower() in ['invalid request', 'parse error']:
                     if self.controller._time_of_request_type_change == 0:
                         self.controller.request_type = Request
                         self.controller._time_of_request_type_change = time.time()
                     if time.time() - self.controller._time_of_request_type_change <= 600:
                         logger.debug("your node says the partial request was invalid but its okay, we can use the full jsonrpc spec instead")
                         return await self.controller(self.method, self.params)
-                response['error']['dankmids_added_context'] = self.request.to_dict()
+                error['dankmids_added_context'] = self.request.to_dict()
                 # I'm 99.99999% sure that any errd call has no result and we only get this field from mscspec object defs
                 # But I'll check it anyway to be safe
                 if result := response.pop('result', None):
                     response['result'] = result
                 logger.debug("error response for %s: %s", self, response)
             return response
     
@@ -227,23 +235,23 @@
         `Exception` type data comes from failed calls
         """
         
         # New handler
         if isinstance(data, RawResponse):
             self._response = data
         elif isinstance(data, BadResponse):
-            if data.response.error.message.lower() in ['invalid request', 'parse error']:
+            if data.response.error.message.lower() in ['invalid request', 'parse error']:  # type: ignore [union-attr]
                 if self.controller._time_of_request_type_change == 0:
                     self.controller.request_type = Request
                     self.controller._time_of_request_type_change = int(time.time())
                 if time.time() - self.controller._time_of_request_type_change <= 600:
                     logger.debug("your node says the partial request was invalid but its okay, we can use the full jsonrpc spec instead")
                     self._response = await self.create_duplicate()
                     return
-            error = data.response.error.to_dict()
+            error = data.response.error.to_dict()  # type: ignore [union-attr]
             error['dankmids_added_context'] = self.request.to_dict()
             self._response = {"error": error}
             logger.debug("%s _response set to rpc error response %s", self, self._response)
         elif isinstance(data, Exception):
             logger.debug("%s _response set to Exception %s", self, data)
             self._response = data
         # From multicalls
@@ -258,26 +266,25 @@
         self._started = True
         self._response = await self.controller.make_request(self.method, self.params, request_id=self.uid)
         return self._response
     
     @property
     def semaphore(self) -> a_sync.Semaphore:
         # NOTE: We cannot cache this property so the semaphore control pattern in the `duplicate` fn will work as intended
-        semaphore = self.controller.method_semaphores[self.method]
         if self.method == 'eth_call':
-            semaphore = semaphore[self.params[1]]
-        return semaphore
+            return self.controller.eth_call_semaphores[self.params[1]]
+        return self.controller.method_semaphores[self.method]  # type: ignore [return-value]
     
     async def create_duplicate(self) -> RPCResponse: # Not actually self, but for typing purposes it is.
         # We need to make room since the stalled call is still holding the semaphore
         self.semaphore.release()
         # We need to check the semaphore again to ensure we have the right context manager, soon but not right away.
         # Creating the task before awaiting the new call ensures the new call will grab the semaphore immediately
         # and then the task will try to acquire at the very next event loop _run_once cycle
-        logger.warning(f"call {self.uid} got stuck, we're creating a new one")
+        logger.warning("%s got stuck, we're creating a new one", self)
         retval = await self.controller(self.method, self.params)
         await self.semaphore.acquire()
         return retval
 
 
 INDIVIDUAL_CALL_REVERT_STRINGS = {
     "invalid opcode",
@@ -298,27 +305,34 @@
     """Returns True if this particular `BadResponse` indicates that the node we are using requires the full request spec. Dank mids will detect this and changeover automagically."""
 
 
 class eth_call(RPCRequest):
     __slots__ = 'block'
     def __init__(self, controller: "DankMiddlewareController", params: Any, retry: bool = False) -> None:
         """ Adds a call to the DankMiddlewareContoller's `pending_eth_calls`. """
-        self.block = params[1]
+        self.block: BlockId = params[1]
+        """The block height at which the contract will be called."""
         super().__init__(controller, "eth_call", params)  # type: ignore
     
+    def __repr__(self) -> str:
+        return f"<{self.__class__.__name__} uid={self.uid} params={self.params}>"
+    
     @property
     def calldata(self) -> HexBytes:
+        """The calldata for the call."""
         return HexBytes(self.params[0]['data'])
     
     @property
     def multicall_compatible(self) -> bool:
+        """True if this contract is multicall compatible, False if not."""
         return self.target not in self.controller.no_multicall
 
     @property
-    def target(self) -> str:
+    def target(self) -> ChecksumAddress:
+        """The contract address for the call."""
         return self.params[0]["to"]
 
     async def spoof_response(self, data: Union[bytes, Exception, RawResponse]) -> None:  # type: ignore
         """ Sets and returns a spoof rpc response for this BatchedCall instance using data provided by the worker. """
 
         # NOTE: If `type(data)` is `bytes`, it is a result from a multicall. If not, `data` comes from a jsonrpc batch.
         # If this if clause is True, it means the call reverted inside of a multicall but returned a result, without causing the multicall to revert.
@@ -338,46 +352,53 @@
                 data = e
         # The above revert catching logic fails to account for pre-decoding RawResponse objects.
         await super().spoof_response(data)
     
     @property
     def semaphore(self) -> a_sync.Semaphore:
         # NOTE: We cannot cache this property so the semaphore control pattern in the `duplicate` fn will work as intended
-        return self.controller.method_semaphores['eth_call'][self.block]
+        return self.controller.eth_call_semaphores[self.block]
     
     
 
 ### Batch requests:
 
-_Request = TypeVar("_Request")
-
-class _Batch(_RequestMeta[List[RPCResponse]], Iterable[_Request]):
-    _fut = None
-    __slots__ = 'calls', '_lock', '_daemon'
-    calls: List[_Request]
+_Request = TypeVar("_Request", bound=_RequestMeta)
 
+class _Batch(_RequestMeta[List[_Response]], Iterable[_Request]):
+    __slots__ = '_calls', '_lock', '_daemon'
+    _calls: List["weakref.ref[_Request]"]
     def __init__(self, controller: "DankMiddlewareController", calls: Iterable[_Request]):
-        self.controller = weakref.proxy(controller)
-        self.calls = [weakref.proxy(call, callback=self._remove) for call in calls]
+        self.controller = controller
+        self._calls = [weakref.ref(call) for call in calls]
         self._lock = _AlertingRLock(name=self.__class__.__name__)
         super().__init__()
     
     def __bool__(self) -> bool:
         return bool(self.calls)
     
-    def __getitem__(self, ix: int) -> _Request:
+    @overload
+    def __getitem__(self, ix: int) -> _Request:...
+    @overload
+    def __getitem__(self, ix: slice) -> List[_Request]:...
+    def __getitem__(self, ix: Union[int, slice]) -> Union[_Request, List[_Request]]:
         return self.calls[ix]
 
     def __iter__(self) -> Iterator[_Request]:
         return iter(self.calls)
     
     def __len__(self) -> int:
         return len(self.calls)
     
     @property
+    def calls(self) -> List[_Request]:
+        "Returns a list of calls. Creates a temporary strong reference to each call in the batch, if it still exists."
+        return [call for ref in self._calls if (call := ref())]
+
+    @property
     def halfpoint(self) -> int:
         return len(self) // 2
     
     @property
     def bisected(self) -> Generator[List[_Request], None, None]:
         yield self.chunk0
         yield self.chunk1
@@ -385,36 +406,39 @@
     @property
     def chunk0(self) -> List[_Request]:
         return self.calls[:self.halfpoint]
     
     @property
     def chunk1(self) -> List[_Request]:
         return self.calls[self.halfpoint:]
+
+    @property
+    def is_full(self) -> bool:
+        raise NotImplementedError(type(self).__name__)
     
     def append(self, call: _Request, skip_check: bool = False) -> None:
         with self._lock:
-            self.calls.append(call)
+            self._calls.append(weakref.ref(call))
             #self._len += 1
             if not skip_check:
                 if self.is_full:
                     self.start()
                 elif self.controller.queue_is_full:
                     self.controller.early_start()
     
     def extend(self, calls: Iterable[_Request], skip_check: bool = False) -> None:
         with self._lock:
-            self.calls.extend(calls)
-            #self._len += len(calls)
+            self._calls.extend(weakref.ref(call) for call in calls)
             if not skip_check:
                 if self.is_full:
                     self.start()
                 elif self.controller.queue_is_full:
                     self.controller.early_start()
 
-    def start(self, batch: Optional["_Batch"] = None, cleanup=True) -> None:
+    def start(self, batch: Optional[Union["_Batch", "DankBatch"]] = None, cleanup=True) -> None:
         if logger.isEnabledFor(logging.DEBUG):
             self._daemon = asyncio.create_task(self._debug_daemon())
         with self._lock:
             for call in self.calls:
                 call.start(batch or self)
             if cleanup:
                 self._post_future_cleanup()
@@ -429,41 +453,38 @@
             logger.debug('Dank too loud. Bisecting batch and retrying.')
         elif isinstance(e, BadResponse) and (_needs_full_request_spec(e) or _is_call_revert(e)):
             pass
         elif "429" not in f"{e}":
             logger.warning(f"unexpected {e.__class__.__name__}: {e}")
         return len(self) > 1
       
-    def _remove(self, proxy: weakref.CallableProxyType) -> None:
-        try:
-            self.calls.remove(proxy)
-        except ValueError:
-            pass
+    def _post_future_cleanup(self) -> None:
+        raise NotImplementedError
 
 mcall_encoder = abi.default_codec._registry.get_encoder("(bool,(address,bytes)[])")
 mcall_decoder = abi.default_codec._registry.get_decoder("(uint256,uint256,(bool,bytes)[])")
 
 def mcall_encode(data: List[Tuple[bool, bytes]]) -> bytes:
     return mcall_encoder([False, data])
 
-def mcall_decode(data: PartialResponse) -> List[Tuple[bool, bytes]]:        
+def mcall_decode(data: PartialResponse) -> Union[List[Tuple[bool, bytes]], Exception]:        
     try:
-        # NOTE: We need to safely bring any Exceptions back out of the ProcessPool
-        data = data.decode_result("eth_call")[2:]
-        data = bytes.fromhex(data)
-        return mcall_decoder(decoding.ContextFramesBytesIO(data))[2]
+        decoded = data.decode_result("eth_call")[2:]  # type: ignore [arg-type]
+        decoded = bytes.fromhex(decoded)
+        return mcall_decoder(decoding.ContextFramesBytesIO(decoded))[2]
     except Exception as e:
+        # NOTE: We need to safely bring any Exceptions back out of the ProcessPool
         try:
             # We do this goofy thing since we can't `return Exc() from e`
             raise e.__class__(*e.args, data.decode_result() if isinstance(data, PartialResponse) else data) from e
         except Exception as new_e:
             return new_e
     
 
-class Multicall(_Batch[eth_call]):
+class Multicall(_Batch[RPCResponse, eth_call]):
     __slots__ = 'bid', '_started', '__dict__'  # We need to specify __dict__ for the cached properties to work
     method = "eth_call"
     fourbyte = function_signature_to_4byte_selector("tryBlockAndAggregate(bool,(address,bytes)[])")    
 
     def __init__(self, controller: "DankMiddlewareController", calls: List[eth_call] = [], bid: Optional[BatchId] = None):
         # sourcery skip: default-mutable-arg
         super().__init__(controller, calls)
@@ -475,57 +496,59 @@
     
     @cached_property
     def block(self) -> BlockId:
         return self.calls[0].block
     
     @property
     def calldata(self) -> str:
-        return (self.fourbyte + mcall_encode([[call.target, call.calldata] for call in self.calls])).hex()
+        return (self.fourbyte + mcall_encode([[call.target, call.calldata] for call in self.calls])).hex()  # type: ignore [misc]
     
     @property
     def target(self) -> ChecksumAddress:
         return self.mcall.address
     
     @cached_property
     def mcall(self) -> "_MulticallContract":
         return self.controller._select_mcall_target_for_block(self.block)
     
     @property
     def params(self) -> JsonrpcParams:
         params = [{'to': self.target, 'data': f'0x{self.calldata}'}, self.block]
         if self.needs_override_code and not self.controller.state_override_not_supported:
             params.append({self.target: {'code': self.mcall.bytecode}})
-        return params
+        return params  # type: ignore [return-value]
     
     @property
     def request(self) -> Union[Request, PartialRequest]:
         return self.controller.request_type(method=self.method, params=self.params, id=self.uid)
     
     @property
     def is_full(self) -> bool:
         return len(self) >= self.controller.batcher.step
 
     @property
     def needs_override_code(self) -> bool:
         return self.mcall.needs_override_code_for_block(self.block)
         
-    async def get_response(self) -> None:
+    async def get_response(self) -> None:  # type: ignore [override]
         if self._started:
             logger.error(f'{self} early exit')
             return
         self._started = True
         if (l := len(self)) == 1:
             return await self._exec_single_call()
         #elif l < 50: # TODO play with later
         #    return await JSONRPCBatch(self.controller, self.calls)
         rid = self.controller.request_uid.next
         demo_logger.info(f'request {rid} for multicall {self.bid} starting')  # type: ignore
         try:
-            await self.spoof_response(await self.controller.make_request(self.method, self.params, request_id=self.uid))
-        except internal_err_types.__args__ as e:
+            # create a strong ref to all calls we will execute so they cant get gced mid execution and mess up response ordering
+            calls = self.calls
+            await self.spoof_response(await self.controller.make_request(self.method, self.params, request_id=self.uid), calls)
+        except internal_err_types.__args__ as e:  # type: ignore [attr-defined]
             raise e if 'invalid argument' in str(e) else DankMidsInternalError(e) from e
         except ClientResponseError as e:
             if e.message == "Payload Too Large":
                 logger.info("Payload too large. response headers: %s", e.headers)
                 self.controller.reduce_multicall_size(len(self))
                 _debugging.failures.record(self.controller.chain_id, e, type(self).__name__, self.uid, len(self), self.request.data)
             else:
@@ -547,30 +570,33 @@
             e.args[0]["dankmids_note"] = "You're not using an archive node, and you need one for the application you are attempting to run."
             return False
         elif super().should_retry(e):
             return True
         return len(self) > 1
     
     @set_done
-    async def spoof_response(self, data: Union[RawResponse, Exception]) -> None:
+    async def spoof_response(self, data: Union[RawResponse, Exception], calls: Optional[List[eth_call]] = None) -> None:
+        # NOTE: we pass in the calls to create a strong reference so when we zip up the results everything gets to the right place
+        if calls is None:
+            calls = self.calls
         # This happens if an Exception takes place during a singular Multicall request.
         if isinstance(data, Exception):
             logger.debug("%s had Exception %s", self, data)
             logger.debug("propagating the %s to all %s's calls", data.__class__.__name__, self)
-            await asyncio.gather(*[call.spoof_response(data) for call in self.calls])
+            await asyncio.gather(*[call.spoof_response(data) for call in calls])
         # A `RawResponse` represents either a successful or a failed response, stored as pre-decoded bytes.
         # It was either received as a response to a single rpc call or as a part of a batch response.
         elif isinstance(data, RawResponse):
             response = data.decode(partial=True)
             if response.error:
                 logger.debug("%s received an 'error' response from the rpc: %s", self, response.exception)
                 # NOTE: We raise the exception which will be caught, call will be broken up and retried
                 raise response.exception
             logger.debug("%s received valid bytes from the rpc", self)
-            await asyncio.gather(*(call.spoof_response(data) for call, (_, data) in zip(self.calls, await self.decode(response))))
+            await asyncio.gather(*(call.spoof_response(data) for call, (_, data) in zip(calls, await self.decode(response))))
         else:
             raise NotImplementedError(f"type {type(data)} not supported.", data)
     
     async def decode(self, data: PartialResponse) -> List[Tuple[bool, bytes]]:
         start = time.time()
         if ENVS.OPERATION_MODE.infura:  # type: ignore [attr-defined]
             retval = mcall_decode(data)
@@ -580,15 +606,15 @@
                     self[100]
                 retval = await ENVS.MULTICALL_DECODER_PROCESSES.run(mcall_decode, data)  # type: ignore [attr-defined]
             except IndexError:
                 retval = mcall_decode(data)
             except BrokenProcessPool:
                 # TODO: Move this somewhere else
                 logger.critical("Oh fuck, you broke the %s while decoding %s", ENVS.MULTICALL_DECODER_PROCESSES, data)  # type: ignore [attr-defined]
-                ENVS.MULTICALL_DECODER_PROCESSES = AsyncProcessPoolExecutor(ENVS.MULTICALL_DECODER_PROCESSES._max_workers)  # type: ignore [attr-defined]
+                ENVS.MULTICALL_DECODER_PROCESSES = AsyncProcessPoolExecutor(ENVS.MULTICALL_DECODER_PROCESSES._max_workers)  # type: ignore [attr-defined,assignment]
                 retval = mcall_decode(data)
         stats.log_duration(f"multicall decoding for {len(self)} calls", start)
         # Raise any Exceptions that may have come out of the process pool.
         if isinstance(retval, Exception):
             raise retval.__class__(*retval.args, self.request.to_dict(), f"response: {data.to_dict()}", f"error: {data.error.to_dict() if data.error else None}")
         return retval
     
@@ -615,15 +641,15 @@
     def _post_future_cleanup(self) -> None:
         with suppress(KeyError):
             with self.controller.pools_closed_lock:
                 # This will have already taken place in a full json batch of multicalls
                 self.controller.pending_eth_calls.pop(self.block)
 
 
-class JSONRPCBatch(_Batch[Union[Multicall, RPCRequest]]):
+class JSONRPCBatch(_Batch[RPCResponse, Union[Multicall, RPCRequest]]):
     __slots__ = 'jid', '_started'
     def __init__(
         self,
         controller: "DankMiddlewareController",
         calls: List[Union[Multicall, RPCRequest]] = [], 
         jid: Optional[BatchId] = None
     ) -> None:  # sourcery skip: default-mutable-arg
@@ -632,72 +658,72 @@
         self._started = False
 
     def __repr__(self) -> str:
         return f"<JSONRPCBatch jid={self.jid} len={len(self)}>"
     
     @property
     def data(self) -> bytes:
-        if not self.calls:
+        if not self:
             raise EmptyBatch(f"batch {self.uid} is empty and should not be processed.")
         try:
-            return _codec.encode([call.request for call in self.calls])
+            return _codec.encode([call.request for call in self])
         except TypeError:
             # If we can't encode one of the calls, lets figure out which one and pass some useful info downstream
-            for call in self.calls:
+            for call in self:
                 try:
                     _codec.encode(call.request)
                 except TypeError as e:
                     raise TypeError(e, call.request) from None
             raise
     
     @property
     def is_multicalls_only(self) -> bool:
         with self._lock:
-            return all(isinstance(call, Multicall) for call in self.calls)
+            return all(isinstance(call, Multicall) for call in self)
 
     @property
     def is_single_multicall(self) -> bool:
         with self._lock:
             return len(self) == 1 and self.is_multicalls_only
 
     @property
     def method_counts(self) -> Dict[RPCEndpoint, int]:
         counts: DefaultDict[RPCEndpoint, int] = defaultdict(int)
         with self._lock:
-            for call in self.calls:
+            for call in self:
                 if isinstance(call, Multicall):
                     counts["eth_call[multicall]"] += len(call)  # type: ignore
                 else:
                     counts[call.method] += 1
             return dict(counts)
     
     @property
     def total_calls(self) -> int:
         with self._lock:
-            return sum(len(call) for call in self.calls)
+            return sum(len(call) for call in self)
 
     @property
     def is_full(self) -> bool:
         with self._lock:
-            return self.total_calls >= self.controller.batcher.step or len(self) >= ENVS.MAX_JSONRPC_BATCH_SIZE  # type: ignore [attr-defined]
+            return self.total_calls >= self.controller.batcher.step or len(self) >= ENVS.MAX_JSONRPC_BATCH_SIZE  # type: ignore [attr-defined,operator]
 
-    async def get_response(self) -> None:
+    async def get_response(self) -> None:  # type: ignore [override]
         if self._started:
             logger.warning(f"{self} exiting early. This shouldn't really happen bro")
             return
         self._started = True
         rid = self.controller.request_uid.next
         if ENVS.DEMO_MODE:  # type: ignore [attr-defined]
             # When demo mode is disabled, we can save some CPU time by skipping this sum
-            demo_logger.info(f'request {rid} for jsonrpc batch {self.jid} ({sum(len(batch) for batch in self.calls)} calls) starting')  # type: ignore
+            demo_logger.info(f'request {rid} for jsonrpc batch {self.jid} ({sum(len(batch) for batch in self)} calls) starting')  # type: ignore
         try:
             # NOTE: We do this inline so we never have to allocate the response to memory
-            await self.spoof_response(await self.post())
+            await self.spoof_response(*await self.post())
         # I want to see these asap when working on the lib.
-        except internal_err_types.__args__ as e:
+        except internal_err_types.__args__ as e:  # type: ignore [attr-defined]
             raise e if 'invalid argument' in str(e) else DankMidsInternalError(e) from e
         except EmptyBatch as e:
             logger.warning("These EmptyBatch exceptions shouldn't actually happen and this except clause can probably be removed soon.")
         except ExceedsMaxBatchSize as e:
             logger.warning("exceeded max batch size for your node")
             self.controller.set_batch_size_limit(e.limit)
             await self.bisect_and_retry(e)
@@ -711,28 +737,32 @@
             stats.log_errd_batch(self)
             if self.should_retry(e):
                 await self.bisect_and_retry(e)
             # NOTE: `self.should_retry(e)` can only return False here if the json batch is comprised of just one rpc request that is not a multicall.
             #       I include this elif clause as a failsafe. This is rare and should not impact performance.
             elif not self.is_single_multicall:
                 # Just to force my IDE to resolve types correctly
-                calls : List[RPCRequest] = self.calls
+                calls : List[RPCRequest] = self.calls # type: ignore [assignment]
                 logger.debug("%s had exception %s, aborting and setting Exception as call._response", self, e)
                 # NOTE: This means an exception occurred during the post request
                 # AND that the json batch is made of just one rpc request that is not a multicall.
                 logger.info('does this ever actually run? pretty sure a single-multicall json batch is not possible. can I delete this?')
                 await asyncio.gather(*[call.spoof_response(e) for call in calls])
             else:
                 raise NotImplementedError('and you may ask yourself, well, how did I get here?')
         demo_logger.info(f'request {rid} for jsonrpc batch {self.jid} complete')  # type: ignore
     
     @eth_retry.auto_retry
-    async def post(self) -> List[RawResponse]:
+    async def post(self) -> Tuple[List[RawResponse], List[Union[Multicall, RPCRequest]]]:
         "this function raises `BadResponse` if a successful 'error' response was received from the rpc"
         try:
+            # we need strong refs so the results all get to the right place
+            calls = self.calls
+            # for the multicalls too
+            mcall_calls_strong_refs = [call.calls for call in filter(lambda x: isinstance(x, Multicall), calls)]  # type: ignore [union-attr]
             response: JSONRPCBatchResponse = await _session.post(self.controller.endpoint, data=self.data, loads=_codec.decode_jsonrpc_batch)
         except ClientResponseError as e:
             if e.message == "Payload Too Large":
                 logger.warning("Payload Too Large")
                 logger.warning("This is what was too large: %s", self.method_counts)
                 self.adjust_batch_size()
             elif 'broken pipe' in str(e).lower():
@@ -746,24 +776,24 @@
                 logger.warning("This is what broke the pipe: %s", self.method_counts)
             if ENVS.DEBUG:  # type: ignore [attr-defined]
                 _debugging.failures.record(self.controller.chain_id, e, type(self).__name__, self.uid, len(self), self.data)
             raise e
         # NOTE: A successful response will be a list of `RawResponse` objects.
         #       A single `PartialResponse` implies an error.
         if isinstance(response, list):
-            return response
+            return response, calls
         # Oops, we failed.
-        if response.error.message.lower() in ['invalid request', 'parse error']:
+        if response.error.message.lower() in ['invalid request', 'parse error']:  # type: ignore [union-attr]
             # NOT SURE IF THIS ACTUALLY RUNS, CAN WE RECEIVE THIS TYPE RESPONSE FOR A JSON BATCH?
             if self.controller._time_of_request_type_change == 0:
                 self.controller.request_type = Request
                 self.controller._time_of_request_type_change = time.time()
             if time.time() - self.controller._time_of_request_type_change <= 600:
                 logger.debug("your node says the partial request was invalid but its okay, we can use the full jsonrpc spec instead")
-        elif response.error.message == "batch limit exceeded":
+        elif response.error.message == "batch limit exceeded":  # type: ignore [union-attr]
             self.adjust_batch_size()
             
         if ENVS.DEBUG:
             _debugging.failures.record(self.controller.chain_id, response.exception, type(self).__name__, self.uid, len(self), self.data)
         raise response.exception
     
     def should_retry(self, e: Exception) -> bool:
@@ -773,27 +803,25 @@
             logger.debug('No state available for one of the blocks queried. Bisecting batch and retrying.')
             return True
         elif super().should_retry(e):
             return True
         return self.is_single_multicall
     
     @set_done
-    async def spoof_response(self, response: List[RawResponse]) -> None:
+    async def spoof_response(self, response: List[RawResponse], calls: List[RPCRequest]) -> None:
         # This means we got results. That doesn't mean they're good, but we got 'em.
         
         if self.controller._sort_calls:
             # NOTE: these providers don't always return batch results in the correct ordering
             # NOTE: is it maybe because they 
-            calls = sorted(self.calls, key=lambda call: call.uid)
+            calls = sorted(calls, key=lambda call: call.uid)
             for i, (call, raw) in enumerate(zip(calls, response)):
                 # TODO: make sure this doesn't ever raise and then delete it
                 decoded = raw.decode()
                 assert call.uid == decoded.id, (i, call, decoded, response, [[call.uid for call in calls], [raw.decode() for raw in response]])
-        else:
-            calls = self.calls
             
         for r in await asyncio.gather(*[call.spoof_response(raw) for call, raw in zip(calls, response)], return_exceptions=True):
             # NOTE: By doing this with the exceptions we allow any successful calls to get their results sooner
             #       without being interrupted by the first exc in the gather and having to wait for the bisect and retry process
             # TODO: stop retrying ones that succeed, that's wasteful
             if isinstance(r, Exception):
                 raise r
@@ -830,17 +858,15 @@
             self.controller.reduce_batch_size(len(self))
             stats.logger.devhint(
                 "We still need some better logic for catching these errors and using them to better optimize the batching process"
             )
 
     def _post_future_cleanup(self) -> None:
         with self.controller.pools_closed_lock:
-            # a hacky way to get the real controller obj from the weak reference proxy
-            controller = self.controller.__repr__.__self__
-            self.controller.pending_rpc_calls = JSONRPCBatch(controller)
+            self.controller.pending_rpc_calls = JSONRPCBatch(self.controller)
 
 def _log_exception(e: Exception) -> bool:
     # NOTE: These errors are expected during normal use and are not indicative of any problem(s). No need to log them.
     # TODO: Better filter what we choose to log here
     dont_need_to_see_errs = constants.RETRY_ERRS + ['out of gas', 'non_empty_data', 'exceeding --rpc.returndata.limit', "'code': 429", 'payload too large']
     
     dont_need_to_see_errs += [
@@ -850,11 +876,11 @@
         *INDIVIDUAL_CALL_REVERT_STRINGS
     ]
 
     
     
     stre = str(e).lower()
     if any(err in stre for err in dont_need_to_see_errs):
-        return ENVS.DEBUG  # type: ignore [attr-defined]
+        return ENVS.DEBUG  # type: ignore [attr-defined,return-value]
     logger.warning("The following exception is being logged for informational purposes and does not indicate failure:")
     logger.warning(e, exc_info=True)
-    return ENVS.DEBUG  # type: ignore [attr-defined]
+    return ENVS.DEBUG  # type: ignore [attr-defined,return-value]
```

### Comparing `dank_mids-4.20.92/dank_mids/_uid.py` & `dank_mids-4.20.93/dank_mids/_uid.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     def next(self) -> int:
         """ Returns the next unique id. """
         with self.lock:
             new: int = self._value + 1
             self._value = new
             return new
 
-class _AlertingRLock(threading._RLock):
+class _AlertingRLock(threading._RLock):  # type: ignore [misc]
     def __init__(self, name: str) -> None:
         super().__init__()
         self.name = name
-    def acquire(self, blocking: bool = True, timeout: int = -1) -> bool:
+    def acquire(self, blocking: bool = True, timeout: int = -1) -> bool:  # type: ignore [override]
         acquired = super().acquire(blocking=False, timeout=5)
         if not acquired:
             logger.warning("wtf?! %s with name %s is locked!", self, self.name)
             super().acquire(blocking=blocking, timeout=timeout)
```

### Comparing `dank_mids-4.20.92/dank_mids/brownie_patch/__init__.py` & `dank_mids-4.20.93/dank_mids/brownie_patch/__init__.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.92/dank_mids/brownie_patch/_method.py` & `dank_mids-4.20.93/dank_mids/brownie_patch/_method.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import functools
 from decimal import Decimal
 from typing import Any, Awaitable, Callable, Dict, Generic, Iterable, List, Optional, TypeVar
 
 from brownie.typing import AccountsType
 from brownie.convert.datatypes import EthAddress
 from eth_abi.exceptions import InsufficientDataBytes
-from web3 import Web3
+from hexbytes.main import BytesLike
 
 from dank_mids import ENVIRONMENT_VARIABLES as ENVS
 from dank_mids.brownie_patch._abi import FunctionABI
-from dank_mids.helpers._helpers import _make_hashable
+from dank_mids.helpers._helpers import DankWeb3, _make_hashable
 
 _EVMType = TypeVar("_EVMType")
 
 class _DankMethodMixin(Generic[_EVMType]):
     _address: EthAddress
     _abi: FunctionABI
     """A mixin class that gives brownie objects async support and reduces memory usage"""
@@ -32,32 +32,40 @@
         return await asyncio.gather(*[self.coroutine(arg, block_identifier=block_identifier, decimals=decimals) for arg in args])
     @property
     def abi(self) -> dict:
         return self._abi.abi
     @property
     def signature(self) -> str:
         return self._abi.signature
+    async def coroutine(  # type: ignore [empty-body]
+        self, 
+        *args: Any, 
+        block_identifier: Optional[int] = None, 
+        decimals: Optional[int] = None,
+        override: Optional[Dict[str, str]] = None,
+    ) -> _EVMType:
+        raise NotImplementedError
     @property
     def _input_sig(self) -> str:
         return self._abi.input_sig
     @functools.cached_property
     def _len_inputs(self) -> int:
         return len(self.abi['inputs'])
     @functools.cached_property
     def _skip_decoder_proc_pool(self) -> bool:
         from dank_mids.brownie_patch.call import _skip_proc_pool
         return self._address in _skip_proc_pool
     @functools.cached_property
-    def _web3(cls) -> Web3:
+    def _web3(cls) -> DankWeb3:
         from dank_mids import web3
         return web3
     @functools.cached_property
-    def _prep_request_data(self) -> Callable[..., Awaitable[bytes]]:
+    def _prep_request_data(self) -> Callable[..., Awaitable[BytesLike]]:
         from dank_mids.brownie_patch import call
-        if ENVS.OPERATION_MODE.application or self._len_inputs:
+        if ENVS.OPERATION_MODE.application or self._len_inputs:  # type: ignore [attr-defined]
             return call.encode
         else:
             return call._request_data_no_args
 
 class _DankMethod(_DankMethodMixin):
     __slots__ = "_address", "_abi", "_name", "_owner", "natspec", "_encode_input", "_decode_output"
     def __init__(
@@ -93,16 +101,16 @@
             - decimals (optional): if provided, the output will be `result / 10 ** decimals`
         
         Returns:
             - Whatever the node sends back as the output for this contract method.
         """
         if override:
             raise ValueError("Cannot use state override with `coroutine`.")
-        async with ENVS.BROWNIE_ENCODER_SEMAPHORE[block_identifier]:  # type: ignore [attr-defined]
+        async with ENVS.BROWNIE_ENCODER_SEMAPHORE[block_identifier]:  # type: ignore [attr-defined,index]
             data = await self._encode_input(self, self._len_inputs, self._prep_request_data, *args)
-            async with ENVS.BROWNIE_CALL_SEMAPHORE[block_identifier]:  # type: ignore [attr-defined]
+            async with ENVS.BROWNIE_CALL_SEMAPHORE[block_identifier]:  # type: ignore [attr-defined,index]
                 output = await self._web3.eth.call({"to": self._address, "data": data}, block_identifier)
         try:
             decoded = await self._decode_output(self, output)
         except InsufficientDataBytes as e:
             raise InsufficientDataBytes(str(e), self, self._address, output) from e
         return decoded if decimals is None else decoded / 10 ** Decimal(decimals)
```

### Comparing `dank_mids-4.20.92/dank_mids/brownie_patch/call.py` & `dank_mids-4.20.93/dank_mids/brownie_patch/call.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,89 +4,91 @@
 from concurrent.futures.process import BrokenProcessPool
 from decimal import Decimal
 from pickle import PicklingError
 from types import MethodType
 from typing import Any, Dict, Optional, Tuple, Union
 
 import eth_abi
-import eth_retry
 from a_sync import AsyncProcessPoolExecutor
 from brownie import chain
 from brownie.convert.normalize import format_input, format_output
 from brownie.convert.utils import get_type_strings
 from brownie.exceptions import VirtualMachineError
 from brownie.network.contract import Contract, ContractCall
 from brownie.project.compiler.solidity import SOLIDITY_ERROR_CODES
 from eth_abi.exceptions import InsufficientDataBytes
+from eth_typing import HexStr
 from eth_utils import to_checksum_address
 from hexbytes import HexBytes
+from hexbytes.main import BytesLike
 from multicall.constants import MULTICALL2_ADDRESSES
-from web3 import Web3
+from web3.types import BlockIdentifier
 
 from dank_mids import ENVIRONMENT_VARIABLES as ENVS
 from dank_mids.brownie_patch.types import ContractMethod
 from dank_mids.exceptions import Revert
+from dank_mids.helpers._helpers import DankWeb3
 
 logger = logging.getLogger(__name__)
 encode = lambda self, *args: ENVS.BROWNIE_ENCODER_PROCESSES.run(__encode_input, self.abi, self.signature, *args)  # type: ignore [attr-defined]
 decode = lambda self, data: ENVS.BROWNIE_DECODER_PROCESSES.run(__decode_output, data, self.abi)  # type: ignore [attr-defined]
 
-def _patch_call(call: ContractCall, w3: Web3) -> None:
+def _patch_call(call: ContractCall, w3: DankWeb3) -> None:
     call._skip_decoder_proc_pool = call._address in _skip_proc_pool
     call.coroutine = MethodType(_get_coroutine_fn(w3, len(call.abi['inputs'])), call)
     call.__await__ = MethodType(_call_no_args, call)
     
 @functools.lru_cache
-def _get_coroutine_fn(w3: Web3, len_inputs: int):
+def _get_coroutine_fn(w3: DankWeb3, len_inputs: int):
     if ENVS.OPERATION_MODE.application or len_inputs:  # type: ignore [attr-defined]
         get_request_data = encode
     else:
-        get_request_data = _request_data_no_args
+        get_request_data = _request_data_no_args  # type: ignore [assignment]
     
     async def coroutine(
         self: ContractCall,
         *args: Tuple[Any,...],
-        block_identifier: Optional[Union[int, str, bytes]] = None,
+        block_identifier: Optional[BlockIdentifier] = None,
         decimals: Optional[int] = None,
         override: Optional[Dict[str, str]] = None
     ) -> Any:
         if override:
             raise ValueError("Cannot use state override with `coroutine`.")
-        async with ENVS.BROWNIE_ENCODER_SEMAPHORE[block_identifier]:  # type: ignore [attr-defined]
+        async with ENVS.BROWNIE_ENCODER_SEMAPHORE[block_identifier]:  # type: ignore [attr-defined, index]
             data = await encode_input(self, len_inputs, get_request_data, *args)
-            async with ENVS.BROWNIE_CALL_SEMAPHORE[block_identifier]:  # type: ignore [attr-defined]
+            async with ENVS.BROWNIE_CALL_SEMAPHORE[block_identifier]:  # type: ignore [attr-defined, index]
                 output = await w3.eth.call({"to": self._address, "data": data}, block_identifier)
         try:
             decoded = await decode_output(self, output)
         except InsufficientDataBytes as e:
             raise InsufficientDataBytes(str(e), self, self._address, output) from e
         
         return decoded if decimals is None else decoded / 10 ** Decimal(decimals)
 
     return coroutine
 
 def _call_no_args(self: ContractMethod):
     """Asynchronously call `self` with no arguments at the latest block."""
     return self.coroutine().__await__()
 
-async def encode_input(call: ContractCall, len_inputs, get_request_data, *args) -> bytes:
+async def encode_input(call: ContractCall, len_inputs, get_request_data, *args) -> HexStr:
     if any(isinstance(arg, Contract) for arg in args) or any(hasattr(arg, "__contains__") for arg in args): # We will just assume containers contain a Contract object until we have a better way to handle this
         # We can't unpickle these because of the added `coroutine` method.
         data = __encode_input(call.abi, call.signature, *args)
     else:
         try: # We're better off sending these to the subprocess so they don't clog up the event loop.
             data = await get_request_data(call, *args)
         except (AttributeError, TypeError):
             # These occur when we have issues pickling an object, but that's fine, we can do it sync.
             data = __encode_input(call.abi, call.signature, *args)
         # TODO: move this somewhere else
         except BrokenProcessPool:
             logger.critical("Oh fuck, you broke the %s while decoding %s with abi %s", ENVS.BROWNIE_ENCODER_PROCESSES, data, call.abi)  # type: ignore [attr-defined]
             # Let's fix that right up
-            ENVS.BROWNIE_ENCODER_PROCESSES = AsyncProcessPoolExecutor(ENVS.BROWNIE_ENCODER_PROCESSES._max_workers)  # type: ignore [attr-defined]
+            ENVS.BROWNIE_ENCODER_PROCESSES = AsyncProcessPoolExecutor(ENVS.BROWNIE_ENCODER_PROCESSES._max_workers)  # type: ignore [attr-defined,assignment]
             data = __encode_input(call.abi, call.signature, *args) if len_inputs else call.signature
         except PicklingError:  # But if that fails, don't worry. I got you.
             data = __encode_input(call.abi, call.signature, *args) if len_inputs else call.signature
     # We have to do it like this so we don't break the process pool.
     if isinstance(data, Exception):
         raise data
     return data
@@ -101,36 +103,36 @@
         else:
             try:
                 decoded = await decode(call, data)
             # TODO: move this somewhere else
             except BrokenProcessPool:
                 # Let's fix that right up
                 logger.critical("Oh fuck, you broke the %s while decoding %s with abi %s", ENVS.BROWNIE_DECODER_PROCESSES, data, call.abi)  # type: ignore [attr-defined]
-                ENVS.BROWNIE_DECODER_PROCESSES = AsyncProcessPoolExecutor(ENVS.BROWNIE_DECODER_PROCESSES._max_workers)  # type: ignore [attr-defined]
+                ENVS.BROWNIE_DECODER_PROCESSES = AsyncProcessPoolExecutor(ENVS.BROWNIE_DECODER_PROCESSES._max_workers)  # type: ignore [attr-defined, assignment]
                 decoded = __decode_output(data, call.abi)
         # We have to do it like this so we don't break the process pool.
         if isinstance(decoded, Exception):
             raise decoded
         return decoded
     except AttributeError as e: 
         # NOTE: Not sure why this happens as we set the attr while patching the call but w/e, this works for now
         if not str(e).endswith(" object has no attribute '_skip_decoder_proc_pool'"):
             raise e
         logger.debug("DEBUG ME BRO: %s", e)
         call._skip_decoder_proc_pool = call._address in _skip_proc_pool
         return await decode_output(call, data)
 
-async def _request_data_no_args(call: ContractCall) -> str:
+async def _request_data_no_args(call: ContractCall) -> HexStr:
     return call.signature
 
 # These methods were renamed in eth-abi 4.0.0
 __eth_abi_encode = eth_abi.encode if hasattr(eth_abi, 'encode') else eth_abi.encode_abi
 __eth_abi_decode = eth_abi.decode if hasattr(eth_abi, 'decode') else eth_abi.decode_abi
 
-def __encode_input(abi: Dict[str, Any], signature: str, *args: Tuple[Any,...]) -> str:
+def __encode_input(abi: Dict[str, Any], signature: str, *args: Tuple[Any,...]) -> Union[HexStr, Exception]:
     try:
         data = format_input(abi, args)
         types_list = get_type_strings(abi["inputs"])
         return signature + __eth_abi_encode(types_list, data).hex()
     except Exception as e:
         return e
 
@@ -142,26 +144,26 @@
         break
     except Exception as e:
         if "429" not in str(e):
             raise e
 if multicall2 := MULTICALL2_ADDRESSES.get(chainid, None):
     _skip_proc_pool.add(to_checksum_address(multicall2))
     
-def __decode_output(hexstr: str, abi: Dict[str, Any]) -> Any:
+def __decode_output(hexstr: BytesLike, abi: Dict[str, Any]) -> Any:
     try:
         types_list = get_type_strings(abi["outputs"])
         result = __eth_abi_decode(types_list, HexBytes(hexstr))
         result = format_output(abi, result)
         if len(result) == 1:
             result = result[0]
         return result
     except Exception as e:
         return e
 
-def __validate_output(abi: Dict[str, Any], hexstr: str):
+def __validate_output(abi: Dict[str, Any], hexstr: BytesLike):
     try:
         selector = HexBytes(hexstr)[:4].hex()
         if selector == "0x08c379a0":
             revert_str = eth_abi.decode_abi(["string"], HexBytes(hexstr)[4:])[0]
             raise Revert(f"Call reverted: {revert_str}")
         elif selector == "0x4e487b71":
             error_code = int(HexBytes(hexstr)[4:].hex(), 16)
```

### Comparing `dank_mids-4.20.92/dank_mids/brownie_patch/contract.py` & `dank_mids-4.20.93/dank_mids/brownie_patch/contract.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,16 @@
                                       build_function_signature)
 from brownie.typing import AccountsType
 from web3 import Web3
 
 from dank_mids.brownie_patch.call import _patch_call
 from dank_mids.brownie_patch.overloaded import _patch_overloaded_method
 from dank_mids.brownie_patch.types import ContractMethod, DankContractMethod, DankOverloadedMethod, _get_method_object
-
+from dank_mids.helpers._helpers import DankWeb3
+    
 
 EventName = NewType("EventName", str)
 LogTopic = NewType("LogTopic", str)
 Method = NewType("Method", str)
 Signature = NewType("Signature", str)
 
 class Contract(brownie.Contract):
@@ -93,30 +94,30 @@
             elif overloaded is True:
                 overloaded = DankOverloadedMethod(self.address, full_name, self._owner)
             overloaded._add_fn(abi, natspec)
         return overloaded  # type: ignore [return-value]
 
     
 @overload
-def patch_contract(contract: Contract, w3: Optional[Web3] = None) -> Contract:...
+def patch_contract(contract: Contract, w3: Optional[DankWeb3] = None) -> Contract:...
 @overload
-def patch_contract(contract: Union[brownie.Contract, str], w3: Optional[Web3] = None) -> brownie.Contract:...
-def patch_contract(contract: Union[Contract, brownie.Contract, str], w3: Optional[Web3] = None) -> Union[Contract, brownie.Contract]:
+def patch_contract(contract: Union[brownie.Contract, str], w3: Optional[DankWeb3] = None) -> brownie.Contract:...
+def patch_contract(contract: Union[Contract, brownie.Contract, str], w3: Optional[DankWeb3] = None) -> Union[Contract, brownie.Contract]:
     """returns a patched version of `contract` with async and call batchings functionalities"""
     if not isinstance(contract, brownie.Contract):
         contract = brownie.Contract(contract)
     if w3 is None and brownie.network.is_connected():
         from dank_mids import dank_web3 as w3
     if w3 is None:
         raise RuntimeError("You must make sure either brownie is connected or you pass in a Web3 instance.")
     for k, v in contract.__dict__.items():
         _patch_if_method(v, w3)
     return contract
 
-def _patch_if_method(method: ContractMethod, w3: Web3) -> None:
+def _patch_if_method(method: ContractMethod, w3: DankWeb3) -> None:
     if isinstance(method, (ContractCall, ContractTx)):
         _patch_call(method, w3)
     elif isinstance(method, OverloadedMethod):
         _patch_overloaded_method(method, w3)
 
 class _ContractMethodPlaceholder:
     """A sentinel object that indicates a Contract does have a member by a specific name."""
```

### Comparing `dank_mids-4.20.92/dank_mids/brownie_patch/overloaded.py` & `dank_mids-4.20.93/dank_mids/brownie_patch/overloaded.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from types import MethodType
 from typing import Any, Dict, Optional, Tuple, Union
 
 from brownie import Contract
 from brownie.network.contract import ContractCall, ContractTx, OverloadedMethod
 from dank_mids.brownie_patch.call import _get_coroutine_fn, _skip_proc_pool
 from dank_mids.brownie_patch.types import ContractMethod
-from web3 import Web3
+from dank_mids.helpers._helpers import DankWeb3
 
 
-def _patch_overloaded_method(call: OverloadedMethod, w3: Web3) -> None:
+def _patch_overloaded_method(call: OverloadedMethod, w3: DankWeb3) -> None:
     # sourcery skip: avoid-builtin-shadow
     @functools.wraps(call)
     async def coroutine(
         self: Contract,
         *args: Tuple[Any,...],
         block_identifier: Optional[Union[int, str, bytes]] = None,
         decimals: Optional[int] = None,
```

### Comparing `dank_mids-4.20.92/dank_mids/brownie_patch/types.py` & `dank_mids-4.20.93/dank_mids/brownie_patch/types.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.92/dank_mids/constants.py` & `dank_mids-4.20.93/dank_mids/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-
+# mypy: disable-error-code="attr-defined, dict-item"
+from typing import Dict
 
 import multicall
+from eth_typing import BlockNumber
 from multicall.constants import Network
 
 TOO_MUCH_DATA_ERRS = ["Payload Too Large", "content length too large", "request entity too large", "batch limit exceeded"]
 RETRY_ERRS = ["connection reset by peer", "server disconnected", "execution aborted (timeout =", "batch limit exceeded", "request timed out"]
 
 GAS_LIMIT = multicall.constants.GAS_LIMIT
 MULTICALL2_OVERRIDE_CODE = multicall.constants.MULTICALL2_BYTECODE
 try:
     MULTICALL3_OVERRIDE_CODE = multicall.constants.MULTICALL3_BYTECODE
 except AttributeError:
     MULTICALL3_OVERRIDE_CODE = multicall.constants.MULTICALL2_BYTECODE
 
-MULTICALL2_DEPLOY_BLOCKS = {
+MULTICALL2_DEPLOY_BLOCKS: Dict[Network, BlockNumber] = {
     Network.Mainnet: 12336033,
     Network.Fantom: 16572242,
     Network.Arbitrum: 821923,
     Network.Optimism: 722566,
 }
 
-MULTICALL3_DEPLOY_BLOCKS = {
+MULTICALL3_DEPLOY_BLOCKS: Dict[Network, BlockNumber] = {
     Network.Mainnet: 14353601,
     Network.Fantom: 33001987,
     Network.Arbitrum: 7654707,
     Network.Optimism: 4286263,
     Network.Base: 5022,
 }
```

### Comparing `dank_mids-4.20.92/dank_mids/controller.py` & `dank_mids-4.20.93/dank_mids/controller.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 
 import logging
 from collections import defaultdict
 from contextlib import suppress
 from functools import lru_cache
-from importlib.metadata import version
-from typing import Any, DefaultDict, List, Literal, Optional
+from typing import Any, DefaultDict, List, Literal, Optional, Set, Union
 
 import eth_retry
+from eth_typing import BlockNumber, ChecksumAddress
 from eth_utils import to_checksum_address
 from msgspec import Struct
 from multicall.constants import MULTICALL2_ADDRESSES, MULTICALL_ADDRESSES
 from multicall.multicall import NotSoBrightBatcher
 from web3 import Web3
 from web3.providers import HTTPProvider
 from web3.providers.async_base import AsyncBaseProvider
@@ -20,15 +20,15 @@
 from dank_mids import _debugging, constants
 from dank_mids._batch import DankBatch
 from dank_mids._demo_mode import demo_logger
 from dank_mids._exceptions import DankMidsInternalError
 from dank_mids._requests import JSONRPCBatch, Multicall, RPCRequest, eth_call
 from dank_mids._uid import UIDGenerator, _AlertingRLock
 from dank_mids.helpers import _codec, _helpers, _session
-from dank_mids.semaphores import _MethodQueues, _MethodSemaphores
+from dank_mids.semaphores import _MethodQueues, _MethodSemaphores, BlockSemaphore
 from dank_mids.types import (BlockId, ChainId, PartialRequest, RawResponse,
                              Request)
 
 try:
     from multicall.constants import MULTICALL3_ADDRESSES
 except ImportError:
     MULTICALL3_ADDRESSES = {}
@@ -48,36 +48,36 @@
     return sync_w3
 
 
 class DankMiddlewareController:
     def __init__(self, w3: Web3) -> None:
         logger.info('Dank Middleware initializing... Strap on your rocket boots...')
         self.w3: Web3 = w3
-        w3_version = version("web3")
-        w3_version_major = int(w3_version.split(".")[0])
-        if w3_version_major >= 6:
+        if _helpers.w3_version_major >= 6:
             from web3.middleware import async_attrdict_middleware
             try:
                 self.w3.middleware_onion.add(async_attrdict_middleware)
             except ValueError as e:
                 if str(e) != "You can't add the same un-named instance twice":
-                    raise e
+                    raise
                 # NOTE: the web3 instance already has the middleware
         self.sync_w3 = _sync_w3_from_async(w3)
 
         self.chain_id = self.sync_w3.eth.chain_id
         # NOTE: We need this mutable for node types that require the full jsonrpc spec
         self.request_type = Request if ENVS.USE_FULL_REQUEST else PartialRequest
-        self._time_of_request_type_change = 0
-        self.state_override_not_supported: bool = ENVS.GANACHE_FORK or self.chain_id == 100  # Gnosis Chain does not support state override.
+        self._time_of_request_type_change: Union[int, float] = 0
 
-        self.endpoint = self.w3.provider.endpoint_uri
+        # NOTE: Ganache does not support state override. Neither does Gnosis Chain.
+        self.state_override_not_supported: bool = ENVS.GANACHE_FORK or self.chain_id == 100  # type: ignore [assignment]
+
+        self.endpoint = self.w3.provider.endpoint_uri  # type: ignore [attr-defined]
 
         self._sort_calls = "tenderly" in self.endpoint or "chainstack" in self.endpoint
-        if "tenderly" in self.endpoint and ENVS.MAX_JSONRPC_BATCH_SIZE > 10:
+        if "tenderly" in self.endpoint and ENVS.MAX_JSONRPC_BATCH_SIZE > 10:  # type: ignore [operator]
             logger.info("max jsonrpc batch size for tenderly is 10, overriding existing max")
             self.set_batch_size_limit(10)
             
         self._instance: int = sum(len(_instances) for _instances in instances.values())
         instances[self.chain_id].append(self)  # type: ignore
 
         multicall = MULTICALL_ADDRESSES.get(self.chain_id)
@@ -96,59 +96,68 @@
         self.mc3 = _MulticallContract(
             address = to_checksum_address(multicall3), 
             # TODO: copypasta deploy block dict
             deploy_block = constants.MULTICALL3_DEPLOY_BLOCKS.get(self.chain_id),
             bytecode = constants.MULTICALL3_OVERRIDE_CODE,
         ) if multicall3 else None
                     
-        self.no_multicall = set()
+        self.no_multicall: Set[ChecksumAddress] = set()
         if multicall:
             self.no_multicall.add(to_checksum_address(multicall))
         if self.mc2:
             self.no_multicall.add(self.mc2.address)
         if self.mc3:
             self.no_multicall.add(self.mc3.address)
         
-        self.eth_call_semaphores = _MethodSemaphores(self)["eth_call"]  # TODO: refactor this out
+        self.method_semaphores = _MethodSemaphores(self)  # TODO: refactor this out
+        self.eth_call_semaphores: BlockSemaphore = self.method_semaphores["eth_call"]  # type: ignore [assignment]
         # semaphores soon to be deprecated for smart queue
         self.method_queues = _MethodQueues(self)
         self.batcher = NotSoBrightBatcher()
-        self.batcher.step = ENVS.MAX_MULTICALL_SIZE
+        self.batcher.step = ENVS.MAX_MULTICALL_SIZE  # type: ignore [attr-defined]
 
         self.call_uid = UIDGenerator()
         self.multicall_uid: UIDGenerator = UIDGenerator()
         self.request_uid: UIDGenerator = UIDGenerator()
         self.jsonrpc_batch_uid: UIDGenerator = UIDGenerator()
         self.pools_closed_lock = _AlertingRLock(name='pools closed')
 
         self.pending_eth_calls: DefaultDict[BlockId, Multicall] = defaultdict(lambda: Multicall(self))
         self.pending_rpc_calls = JSONRPCBatch(self)
     
     def __repr__(self) -> str:
         return f"<DankMiddlewareController instance={self._instance} chain={self.chain_id} endpoint={self.endpoint}>"
 
     async def __call__(self, method: RPCEndpoint, params: Any) -> RPCResponse:
-        with suppress(KeyError):
-            # some methods go thru a SmartProcessingQueue, we try this first
-            try:
-                queue = self.method_queues[method]
-                return await queue(self, method, params)
-            except TypeError as e:
-                if "unhashable type" in str(e):
-                    return await queue(self, method, _helpers._make_hashable(params))
-                raise e
-            
+        
         # eth_call go thru a specialized Semaphore and other methods pass thru unblocked
-        logger.debug(f'making {self.request_type.__name__} {method} with params {params}')
-        if method != "eth_call":
-            return await RPCRequest(self, method, params)
-        async with self.eth_call_semaphores[params[1]]:
-            if params[0]["to"] not in self.no_multicall:
+        if method == "eth_call":
+            async with self.eth_call_semaphores[params[1]]:
+                # create a strong ref to the call that will be held until the caller completes or is cancelled
+                logger.debug(f'making {self.request_type.__name__} {method} with params {params}')
+                if params[0]["to"] in self.no_multicall:
+                    return await RPCRequest(self, method, params)
                 return await eth_call(self, params)
+
+        # some methods go thru a SmartProcessingQueue, we check those next
+        queue = self.method_queues[method]
+        logger.debug(f'making {self.request_type.__name__} {method} with params {params}')
+
+        # no queue, we can make the request normally
+        if queue is None:
             return await RPCRequest(self, method, params)
+        
+        # queue found, queue up the call and await the future
+        try:
+            # NOTE: is this a strong enough ref? 
+            return await queue(self, method, params)
+        except TypeError as e:
+            if "unhashable type" not in str(e):
+                raise e
+        return await queue(self, method, _helpers._make_hashable(params))
     
     @eth_retry.auto_retry
     async def make_request(self, method: str, params: List[Any], request_id: Optional[int] = None) -> RawResponse:
         request = self.request_type(method=method, params=params, id=request_id or self.call_uid.next)
         try:
             return await _session.post(self.endpoint, data=request, loads=_codec.decode_raw)
         except Exception as e:
@@ -168,15 +177,15 @@
         await batch
         demo_logger.info(f'{batch} done')
 
     @property
     def queue_is_full(self) -> bool:
         with self.pools_closed_lock:
             if ENVS.OPERATION_MODE.infura:  # type: ignore [attr-defined]
-                return sum(len(call) for call in self.pending_rpc_calls) >= ENVS.MAX_JSONRPC_BATCH_SIZE  # type: ignore [attr-defined]
+                return sum(len(call) for call in self.pending_rpc_calls) >= ENVS.MAX_JSONRPC_BATCH_SIZE  # type: ignore [attr-defined,operator]
             eth_calls = sum(len(calls) for calls in self.pending_eth_calls.values())
             other_calls = sum(len(call) for call in self.pending_rpc_calls)
             return eth_calls + other_calls >= self.batcher.step
     
     def early_start(self):
         """Used to start all queued calls when we have enough for a full batch"""
         with self.pools_closed_lock:
@@ -184,23 +193,23 @@
             self.pending_eth_calls.clear()
             self.pending_rpc_calls.start()
     
     def reduce_multicall_size(self, num_calls: int) -> None:
         self._reduce_chunk_size(num_calls, "multicall")
     
     def reduce_batch_size(self, num_calls: int) -> None:
-        self._reduce_chunk_size(num_calls, "jsonrpc batch")
+        self._reduce_chunk_size(num_calls, "batch")
     
-    def _reduce_chunk_size(self, num_calls: int, chunk_name: Literal["multicall", "jsonrpc"]) -> None:
+    def _reduce_chunk_size(self, num_calls: int, chunk_name: Literal["multicall", "batch"]) -> None:
         new_chunk_size = round(num_calls * 0.99) if num_calls >= 100 else num_calls - 1
         if new_chunk_size < 30:
             logger.warning(f"your {chunk_name} batch size is really low, did you have some connection issue earlier? You might want to restart your script. {chunk_name} chunk size will not be further lowered.")
             return
         # NOTE: We need the 2nd check because one of the other calls in a batch might have already reduced the chunk size
-        if chunk_name == "jsonrpc batch":
+        if chunk_name == "batch":
             self.set_batch_size_limit(new_chunk_size)
             logger.info("The failed batch had %s calls", num_calls)
             return
         elif chunk_name == "multicall":
             self.set_multicall_size_limit(new_chunk_size)
             logger.info("The failed multicall had %s calls", num_calls)
             return
@@ -212,38 +221,38 @@
             self.batcher.step = new_limit
             logger.warning("multicall size limit reduced from %s to %s", existing_limit, new_limit)
         else:
             logger.info("new multicall size limit %s is not lower than existing limit %s", new_limit, existing_limit)
             
     def set_batch_size_limit(self, new_limit: int) -> None:
         existing_limit = ENVS.MAX_JSONRPC_BATCH_SIZE  # type: ignore [attr-defined]
-        if new_limit < existing_limit:
-            ENVS.MAX_JSONRPC_BATCH_SIZE = new_limit  # type: ignore [attr-defined]
+        if new_limit < existing_limit:  # type: ignore [operator]
+            ENVS.MAX_JSONRPC_BATCH_SIZE = new_limit  # type: ignore [attr-defined,assignment]
             logger.warning("jsonrpc batch size limit reduced from %s to %s", existing_limit, new_limit)
         else:
-            logger.info("new jsonrpc batch size limit %s is not lower than existing limit %s", new_limit, int(existing_limit))
+            logger.info("new jsonrpc batch size limit %s is not lower than existing limit %s", new_limit, int(existing_limit))  # type: ignore [call-overload]
     
     @lru_cache(maxsize=1024)
     def _select_mcall_target_for_block(self, block) -> "_MulticallContract":
         if block == 'latest':
-            return self.mc3 if self.mc3 else self.mc2
+            return self.mc3 if self.mc3 else self.mc2  # type: ignore [return-value]
         if self.mc3 and not self.mc3.needs_override_code_for_block(block):
             return self.mc3
         if self.mc2:
             # We don't care if mc2 needs override code, mc2 override code is shorter
             return self.mc2
-        return self.mc3
+        return self.mc3  # type: ignore [return-value]
 
 class _MulticallContract(Struct):
-    address: str
-    deploy_block: Optional[int]
+    address: ChecksumAddress
+    deploy_block: Optional[BlockNumber]
     bytecode: str
     
     @lru_cache(maxsize=1024)
-    def needs_override_code_for_block(self, block: BlockId) -> bool:
+    def needs_override_code_for_block(self, block: BlockNumber) -> bool:
         if block == 'latest':
             return False
         if self.deploy_block is None:
             return True
         if isinstance(block, str):
             block = int(block, 16)
         return block < self.deploy_block
```

### Comparing `dank_mids-4.20.92/dank_mids/helpers/_codec.py` & `dank_mids-4.20.93/dank_mids/helpers/_codec.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.92/dank_mids/helpers/_helpers.py` & `dank_mids-4.20.93/dank_mids/helpers/_helpers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 
 import asyncio
 from functools import wraps
+from importlib.metadata import version
 from typing import (TYPE_CHECKING, Any, Awaitable, Callable, Coroutine,
                     Iterable, List, Literal, Optional, TypeVar)
 
 from async_lru import alru_cache
+from eth_typing import BlockNumber
 from eth_utils.curried import (apply_formatter_if, apply_formatters_to_dict,
                                apply_key_map, is_null)
 from eth_utils.toolz import assoc, complement, compose, merge
 from hexbytes import HexBytes
 from multicall.utils import get_async_w3
-from typing_extensions import ParamSpec
+from typing_extensions import Concatenate, ParamSpec
 from web3 import Web3
 from web3.datastructures import AttributeDict
 from web3._utils.rpc_abi import RPC
 from web3.eth import AsyncEth
 from web3.providers.async_base import AsyncBaseProvider
 from web3.providers.base import BaseProvider
 from web3.types import Formatters, FormattersDict, RPCEndpoint, RPCResponse
 
 from dank_mids.types import AsyncMiddleware
 
 if TYPE_CHECKING:
-    from dank_mids._requests import RPCRequest
+    from dank_mids._requests import _Request
 
 dank_w3s: List[Web3] = []
+sync_w3s: List[Web3] = []
 
 T = TypeVar("T")
 P = ParamSpec("P")
 
+w3_version_major = int(version("web3").split(".")[0])
+
 class DankEth(AsyncEth):
     @alru_cache(ttl=0)
-    async def get_block_number(self) -> int:
-        return await super().get_block_number()
+    async def get_block_number(self) -> BlockNumber:  # type: ignore [override]
+        block = await super().get_block_number()  # type: ignore [misc]
+        return block
     
 class DankWeb3:
     """This is just a helper for type checkers. Your object will just be a modified ``web3.Web3`` object."""
     eth: DankEth
 
 def setup_dank_w3(async_w3: Web3) -> DankWeb3:
     """ Injects Dank Middleware into an async Web3 instance. """
@@ -50,24 +56,40 @@
         dank_w3s.append(async_w3)
     async_w3.eth = DankEth(async_w3)
     return async_w3
 
 def setup_dank_w3_from_sync(sync_w3: Web3) -> DankWeb3:
     """ Creates a new async Web3 instance from `w3.provider.endpoint_uri` and injects it with Dank Middleware. """
     assert not sync_w3.eth.is_async and isinstance(sync_w3.provider, BaseProvider)
+    if sync_w3 not in sync_w3s:
+        if w3_version_major >= 6:
+            from web3.middleware import attrdict_middleware
+            try:
+                sync_w3.middleware_onion.add(attrdict_middleware)
+            except ValueError as e:
+                if str(e) != "You can't add the same un-named instance twice":
+                    raise e
+        if w3_version_major >= 7:
+            # we need to make sure our sync w3 instance is compatible with poa chains
+            from web3.middleware.proof_of_authority import ExtraDataToPOAMiddleware
+            sync_w3.middleware_onion.inject(ExtraDataToPOAMiddleware, layer=0)
+        elif w3_version_major >= 6:
+            from web3.middleware import geth_poa_middleware
+            sync_w3.middleware_onion.inject(geth_poa_middleware, layer=0)
+        sync_w3s.append(sync_w3)
     return setup_dank_w3(get_async_w3(sync_w3))
 
 async def await_all(futs: Iterable[Awaitable]) -> None:
     for fut in asyncio.as_completed([*futs]):
         await fut
         del fut
 
-def set_done(fn: Callable[P, Awaitable[T]]):
+def set_done(fn: Callable[Concatenate["_Request", P], Awaitable[T]]) -> Callable[Concatenate["_Request", P], Awaitable[T]]:
 	@wraps(fn)
-	async def set_done_wrap(self: "RPCRequest", *args: P.args, **kwargs: P.kwargs) -> T:
+	async def set_done_wrap(self: "_Request", *args: P.args, **kwargs: P.kwargs) -> T:
 		retval = await fn(self, *args, **kwargs)
 		self._done.set()
 		return retval
 	return set_done_wrap
 
 # Everything below is in web3.py now, but dank_mids currently needs a version that predates them.
```

### Comparing `dank_mids-4.20.92/dank_mids/helpers/_session.py` & `dank_mids-4.20.93/dank_mids/helpers/_session.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from random import random
 from typing import Any, Callable, List, Optional, overload
 
 import msgspec
 from aiohttp import ClientSession as DefaultClientSession
 from aiohttp import ClientTimeout, TCPConnector
 from aiohttp.client_exceptions import ClientResponseError
-from aiohttp.typedefs import JSONDecoder
+from aiohttp.typedefs import DEFAULT_JSON_DECODER, JSONDecoder
 from aiolimiter import AsyncLimiter
 from async_lru import alru_cache
 
 from dank_mids import ENVIRONMENT_VARIABLES
 from dank_mids.helpers import _codec
 from dank_mids.types import JSONRPCBatchResponse, PartialRequest, RawResponse
 
@@ -54,62 +54,62 @@
         + 'and Pantheon. In the case of Cloudflare, a second HTTP status code 1XXX error message will be\n'
         + 'included to provide a more accurate description of the problem. For Pantheon, HTTP status code\n'
         + '530 Site Frozen indicates that a site has been restricted due to inactivity.\n'
         + 'Learn more at https://http.dev/530')
     def __new__(cls, value, phrase, description=''):
         obj = int.__new__(cls, value)
         obj._value_ = value
-        obj.phrase = phrase
-        obj.description = description
+        obj.phrase = phrase  # type: ignore [attr-defined]
+        obj.description = description  # type: ignore [attr-defined]
         return obj
 
 # Then, combine the standard HTTPStatus enum and the custom extension to get the full custom HTTPStatus enum we need.
-HTTPStatusExtended = IntEnum('HTTPStatusExtended', [(i.name, i.value) for i in chain(http.HTTPStatus, _HTTPStatusExtension)])
+HTTPStatusExtended = IntEnum('HTTPStatusExtended', [(i.name, i.value) for i in chain(http.HTTPStatus, _HTTPStatusExtension)])  # type: ignore [misc]
 
 RETRY_FOR_CODES = {
     HTTPStatusExtended.BAD_GATEWAY,  # type: ignore [attr-defined]
     HTTPStatusExtended.WEB_SERVER_IS_RETURNING_AN_UNKNOWN_ERROR,  # type: ignore [attr-defined]
     HTTPStatusExtended.CLOUDFLARE_CONNECTION_TIMEOUT,  # type: ignore [attr-defined]
     HTTPStatusExtended.CLOUDFLARE_TIMEOUT,  # type: ignore [attr-defined]
 }
 
 limiter = AsyncLimiter(5, 0.1)  # 50 requests/second
 
 @overload
 async def post(endpoint: str, *args, loads: Callable[[Any], RawResponse], **kwargs) -> RawResponse:...
 @overload
 async def post(endpoint: str, *args, loads: Callable[[Any], JSONRPCBatchResponse], **kwargs) -> JSONRPCBatchResponse:...
-async def post(endpoint: str, *args, loads: Optional[JSONDecoder] = None, **kwargs) -> Any:
+async def post(endpoint: str, *args, loads: JSONDecoder = DEFAULT_JSON_DECODER, **kwargs) -> Any:
     """Returns decoded json data from `endpoint`"""
     session = await get_session()
     return await session.post(endpoint, *args, loads=loads, **kwargs)
 
 async def get_session() -> "ClientSession":
     return await _get_session_for_thread(get_ident())
 
 class ClientSession(DefaultClientSession):
-    async def post(self, endpoint: str, *args, loads: Optional[JSONDecoder] = None, _retry_after: int = 1, **kwargs) -> bytes:  # type: ignore [override]
+    async def post(self, endpoint: str, *args, loads: JSONDecoder = DEFAULT_JSON_DECODER, _retry_after: float = 1, **kwargs) -> bytes:  # type: ignore [override]
         # Process input arguments.
         if isinstance(kwargs.get('data'), PartialRequest):
             logger.debug("making request for %s", kwargs['data'])
             kwargs['data'] = _codec.encode(kwargs['data'])
-        logger.debug("making request with (args, kwargs): (%s %s)", tuple(endpoint, *args), kwargs)
+        logger.debug("making request to %s with (args, kwargs): (%s %s)", endpoint, args, kwargs)
 
         # Try the request until success or 5 failures.
         tried = 0
         while True:
             try:
                 async with limiter:
                     async with super().post(endpoint, *args, **kwargs) as response:
-                        response = await response.json(loads=loads, content_type=None)
-                        logger.debug("received response %s", response)
-                        return response
+                        response_data = await response.json(loads=loads, content_type=None)
+                        logger.debug("received response %s", response_data)
+                        return response_data
             except ClientResponseError as ce:
-                if ce.status == HTTPStatusExtended.TOO_MANY_REQUESTS:
-                    try_after = float(ce.headers.get("Retry-After", _retry_after * 1.5))
+                if ce.status == HTTPStatusExtended.TOO_MANY_REQUESTS:  # type: ignore [attr-defined]
+                    try_after = float(ce.headers.get("Retry-After", _retry_after * 1.5))  # type: ignore [union-attr]
                     if self not in _limited:
                         _limited.append(self)
                         logger.info("You're being rate limited by your node provider")
                         logger.info("Its all good, dank_mids has this handled, but you might get results slower than you'd like")
                     logger.info(f"rate limited: retrying after {try_after}s")
                     await asyncio.sleep(try_after)
                     if try_after > 30:
@@ -135,10 +135,11 @@
     Most everything should be run in main thread though.
     """
     return ClientSession(
         connector = TCPConnector(limit=32),
         headers = {'content-type': 'application/json'}, 
         timeout = ClientTimeout(ENVIRONMENT_VARIABLES.AIOHTTP_TIMEOUT),  # type: ignore [arg-type, attr-defined]
         raise_for_status = True,
+        read_bufsize=2**20,  # 1mb
     )
 
 _limited: List[ClientSession] = []
```

### Comparing `dank_mids-4.20.92/dank_mids/middleware.py` & `dank_mids-4.20.93/dank_mids/middleware.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.92/dank_mids/semaphores.py` & `dank_mids-4.20.93/dank_mids/semaphores.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 class _BlockSemaphoreContextManager(_PrioritySemaphoreContextManager):
     _priority_name = "block"
     def __init__(self, parent: "BlockSemaphore", priority: Union[int, float, Decimal], name: Optional[str] = None) -> None:
         if not isinstance(priority, (int, float, Decimal)):
             raise TypeError(priority)
         super().__init__(parent, priority, name)
     
-class BlockSemaphore(_AbstractPrioritySemaphore[str, _BlockSemaphoreContextManager]):
-    _context_manager_class = _BlockSemaphoreContextManager
-    _top_priority = -1
-    def __getitem__(self, block: Union[int, str, Literal["latest", None]]) -> "_BlockSemaphoreContextManager":
-        return super().__getitem__(
-            block if isinstance(block, int)
-            else int(block.hex(), 16) if isinstance(block, bytes)
+class BlockSemaphore(_AbstractPrioritySemaphore[str, _BlockSemaphoreContextManager]):  # type: ignore [type-var]
+    _context_manager_class = _BlockSemaphoreContextManager  # type: ignore [assignment]
+    _top_priority: int = -1  # type: ignore [assignment]
+    def __getitem__(self, block: Union[int, str, Literal["latest", None]]) -> "_BlockSemaphoreContextManager":  # type: ignore [override]
+        return super().__getitem__(  # type: ignore [return-value]
+            block if isinstance(block, int)  # type: ignore [index]
+            else int(block.hex(), 16) if isinstance(block, bytes)  # type: ignore [union-attr]
             else int(block, 16) if isinstance(block, str) and "0x" in block
             else block if block not in [None, 'latest']  # NOTE: We do this to generate an err if an unsuitable value was provided
             else self._top_priority
-        )
+        )  # type: ignore [index]
 
 
 class _MethodSemaphores:
     def __init__(self, controller: "DankMiddlewareController") -> None:
         # TODO: refactor this out, just use BlockSemaphore for eth_call and SmartProcessingQueue to limit other methods
         from dank_mids import ENVIRONMENT_VARIABLES
         self.controller = controller
@@ -56,12 +56,12 @@
         self.method_queues = {
             method: a_sync.SmartProcessingQueue(RPCRequest, num_workers=sem._value, name=f"{method} {controller}")
             for method, sem in ENVIRONMENT_VARIABLES.method_semaphores.items()
             if method != "eth_call"
         }
         self.keys = self.method_queues.keys()
     @functools.lru_cache(maxsize=None)
-    def __getitem__(self, method: RPCEndpoint) -> a_sync.SmartProcessingQueue:
+    def __getitem__(self, method: RPCEndpoint) -> Optional[a_sync.SmartProcessingQueue]:
         try:
             return next(self.method_queues[key] for key in self.keys if key in method)
         except StopIteration:
-            raise KeyError(method) from None
+            return None
```

### Comparing `dank_mids-4.20.92/dank_mids/stats.py` & `dank_mids-4.20.93/dank_mids/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from dank_mids import ENVIRONMENT_VARIABLES as ENVS
 
 if TYPE_CHECKING:
     from dank_mids._requests import JSONRPCBatch
     from dank_mids.types import Request
 
-_LogLevel = Union[int, str]
+_LogLevel = int
 
 # New logging levels:
 # DEBUG=10, INFO=20, 
 STATS = 13
 DEVHINT = 15
 
 COLLECT_STATS: bool = False  # TODO: enable this
@@ -93,18 +93,18 @@
         """If `self.isEnabledFor(level)` is True, will call `callable` with your args and log the output."""
         if self.isEnabledFor(level):
             return self._log_nocheck(level, callable(*callable_args), (), **logging_kwargs)
     
     # Daemon
 
     def _ensure_daemon(self) -> None:
-        if (ENVS.COLLECT_STATS or self.enabled) and self._daemon is None:  # type: ignore [attr-defined]
+        if (ENVS.COLLECT_STATS or self.enabled) and self._daemon is None:  # type: ignore [attr-defined,has-type]
             self._daemon = asyncio.create_task(self._stats_daemon())
         elif self._daemon.done():
-            raise self._daemon.exception()
+            raise self._daemon.exception()  # type: ignore [misc]
         
     async def _stats_daemon(self) -> None:
         start = time()
         time_since_notified = 0
         while True:
             await asyncio.sleep(0)
             now = time()
@@ -143,20 +143,20 @@
 
 
 _Times = Deque[float]
 
 class _Collector:
     def __init__(self):
         """Handles the collection and computation of stats-related data."""
-        self.errd_batches = deque(maxlen=500)
+        self.errd_batches: Deque["JSONRPCBatch"] = deque(maxlen=500)
         self.durations: DefaultDict[str, _Times] = defaultdict(lambda: deque(maxlen=50_000))
         self.types: Set[Type] = set()
         self.event_loop_times: _Times = deque(maxlen=50_000)
         # not implemented
-        self.validation_errors: DefaultDict[RPCEndpoint, Deque["Request"]] = defaultdict(lambda: deque(maxlen=100))
+        self.validation_errors: DefaultDict[RPCEndpoint, Deque[msgspec.ValidationError]] = defaultdict(lambda: deque(maxlen=100))
 
     @property
     def avg_loop_time(self) -> float:
         return sum(collector.event_loop_times) / len(collector.event_loop_times)
     @property
     def count_active_brownie_calls(self) -> int:
         return ENVS.BROWNIE_CALL_SEMAPHORE.default_value - ENVS.BROWNIE_CALL_SEMAPHORE.semaphore._value  # type: ignore [attr-defined]
```

### Comparing `dank_mids-4.20.92/dank_mids/types.py` & `dank_mids-4.20.93/dank_mids/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import re
 from time import time
 from typing import (TYPE_CHECKING, Any, Callable, Coroutine, DefaultDict, Dict,
-                    List, Literal, NewType, Optional, Set, TypedDict, TypeVar,
-                    Union, overload)
+                    List, Literal, NewType, Optional, Set, Tuple, TypedDict, 
+                    TypeVar, Union, overload)
 
 import msgspec
 from eth_typing import ChecksumAddress
 from web3.datastructures import AttributeDict
 from web3.types import RPCEndpoint, RPCResponse
 
 from dank_mids import constants, stats
@@ -91,15 +91,14 @@
 decoder_logger = logging.getLogger('dank_mids.decoder')
 
 class PartialResponse(_DictStruct):
     result: msgspec.Raw = None  # type: ignore
     "If the rpc response contains a 'result' field, it is set here"
     error: Optional[Error] = None
     "If the rpc response contains an 'error' field, it is set here"
-
     @property
     def exception(self) -> Exception:
         "If the rpc response contains an 'error' field, returns a specialized exception for the specified rpc error."
         if self.error is None:
             raise AttributeError(f"{self} did not error.")
         return (
             PayloadTooLarge(self) if self.payload_too_large
@@ -108,29 +107,29 @@
             else BadResponse(self)
         )
     
     @property
     def payload_too_large(self) -> bool:
         return any(err in self.error.message for err in constants.TOO_MUCH_DATA_ERRS)  # type: ignore [union-attr]
         
-    def to_dict(self, method: Optional[RPCEndpoint] = None) -> Dict[str, Any]:
+    def to_dict(self, method: Optional[RPCEndpoint] = None) -> RPCResponse:  # type: ignore [override]
         """Returns a complete dictionary representation of this response ``Struct``."""
-        data = {}
+        data: RPCResponse = {}
         for field in self.__struct_fields__:
             attr = getattr(self, field)
             if attr is None:
                 continue
             if field == "result":
                 attr = self.decode_result(method=method, _caller=self)
             if isinstance(attr, _DictStruct):
                 attr = attr.to_dict()
-            data[field] = AttributeDict(attr) if isinstance(attr, dict) and field != "error" else attr
+            data[field] = AttributeDict(attr) if isinstance(attr, dict) and field != "error" else attr  # type: ignore [literal-required]
         return data
 
-    def decode_result(self, method: Optional[RPCEndpoint] = None, _caller = None) -> Any:
+    def decode_result(self, method: Optional[RPCEndpoint] = None, _caller = None) -> Union[str, AttributeDict]:
         # NOTE: These must be added to the `RETURN_TYPES` constant above manually
         if method and (typ := RETURN_TYPES.get(method)):
             if method in ["eth_call", "eth_blockNumber", "eth_getCode", "eth_getBlockByNumber", "eth_getTransactionReceipt", "eth_getTransactionCount", "eth_getBalance", "eth_chainId", "erigon_getHeaderByNumber"]:
                 return msgspec.json.decode(self.result, type=typ)
             try:
                 start = time()
                 decoded = msgspec.json.decode(self.result, type=typ)
@@ -179,15 +178,15 @@
     """
     def __init__(self, raw: msgspec.Raw) -> None:
         self._raw = raw
         """The `msgspec.Raw` object wrapped by this wrapper."""
     @overload
     def decode(self, partial: Literal[True]) -> PartialResponse:...
     @overload
-    def decode(self, partial: Literal[False]) -> Response:...
+    def decode(self, partial: Literal[False] = False) -> Response:...
     def decode(self, partial: bool = False) -> Union[Response, PartialResponse]:
         """Decode the wrapped `msgspec.Raw` object into a `Response` or a `PartialResponse`."""
         return msgspec.json.decode(self._raw, type=PartialResponse if partial else Response)
 
 JSONRPCBatchRequest = List[Request]
 # NOTE: A PartialResponse result implies a failure response from the rpc.
 JSONRPCBatchResponse = Union[List[RawResponse], PartialResponse]
```

### Comparing `dank_mids-4.20.92/dank_mids.egg-info/PKG-INFO` & `dank_mids-4.20.93/dank_mids.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dank_mids
-Version: 4.20.92
+Version: 4.20.93
 Summary: Multicall batching middleware for asynchronous scripts using web3.py
 Home-page: https://github.com/BobTheBuidler/dank_mids
 Author: BobTheBuidler
 Author-email: bobthebuidlerdefi@gmail.com
 License: MIT
 Requires-Dist: aiofiles
 Requires-Dist: eth_retry<0.2,>=0.1.15
```

### Comparing `dank_mids-4.20.92/dank_mids.egg-info/SOURCES.txt` & `dank_mids-4.20.93/dank_mids.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.92/docs/Makefile` & `dank_mids-4.20.93/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.92/docs/_build/html/_static/alabaster.css` & `dank_mids-4.20.93/docs/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.92/docs/_build/html/_static/basic.css` & `dank_mids-4.20.93/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.92/docs/_build/html/_static/doctools.js` & `dank_mids-4.20.93/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.92/docs/_build/html/_static/language_data.js` & `dank_mids-4.20.93/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.92/docs/_build/html/_static/pygments.css` & `dank_mids-4.20.93/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.92/docs/_build/html/_static/searchtools.js` & `dank_mids-4.20.93/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.92/docs/_build/html/_static/sphinx_highlight.js` & `dank_mids-4.20.93/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.92/docs/conf.py` & `dank_mids-4.20.93/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.92/docs/make.bat` & `dank_mids-4.20.93/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.92/examples/dank_brownie_example.py` & `dank_mids-4.20.93/examples/dank_brownie_example.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.92/license` & `dank_mids-4.20.93/license`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.92/setup.py` & `dank_mids-4.20.93/setup.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.92/tests/test_brownie_patch.py` & `dank_mids-4.20.93/tests/test_brownie_patch.py`

 * *Files identical despite different names*

### Comparing `dank_mids-4.20.92/tests/test_dank_mids.py` & `dank_mids-4.20.93/tests/test_dank_mids.py`

 * *Files identical despite different names*

