# Comparing `tmp/silverback-0.4.0.tar.gz` & `tmp/silverback-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silverback-0.4.0.tar", last modified: Thu May  2 23:12:00 2024, max compression
+gzip compressed data, was "silverback-0.4.1.tar", last modified: Sat May  4 17:42:22 2024, max compression
```

## Comparing `silverback-0.4.0.tar` & `silverback-0.4.1.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:12:00.967940 silverback-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:12:00.959941 silverback-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:12:00.959941 silverback-0.4.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-02 23:11:00.000000 silverback-0.4.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-02 23:11:00.000000 silverback-0.4.0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-02 23:11:00.000000 silverback-0.4.0/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-02 23:11:00.000000 silverback-0.4.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-02 23:11:00.000000 silverback-0.4.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:12:00.959941 silverback-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-02 23:11:00.000000 silverback-0.4.0/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-02 23:11:00.000000 silverback-0.4.0/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-02 23:11:00.000000 silverback-0.4.0/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-02 23:11:00.000000 silverback-0.4.0/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-02 23:11:00.000000 silverback-0.4.0/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-02 23:11:00.000000 silverback-0.4.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-02 23:11:00.000000 silverback-0.4.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-02 23:11:00.000000 silverback-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-02 23:11:00.000000 silverback-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-02 23:11:00.000000 silverback-0.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-02 23:11:00.000000 silverback-0.4.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-02 23:11:00.000000 silverback-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-02 23:12:00.967940 silverback-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-02 23:11:00.000000 silverback-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-02 23:11:00.000000 silverback-0.4.0/build_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:12:00.959941 silverback-0.4.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:12:00.963940 silverback-0.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/_static/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:12:00.963940 silverback-0.4.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/_templates/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:12:00.963940 silverback-0.4.0/docs/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/commands/run.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/logo.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:12:00.963940 silverback-0.4.0/docs/methoddocs/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/methoddocs/application.md
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/methoddocs/exceptions.md
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/methoddocs/middlewares.md
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/methoddocs/runner.md
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/methoddocs/subscriptions.md
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/methoddocs/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:12:00.963940 silverback-0.4.0/docs/userguides/
--rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/userguides/development.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 23:11:00.000000 silverback-0.4.0/docs/userguides/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-02 23:11:00.000000 silverback-0.4.0/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-02 23:11:00.000000 silverback-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-02 23:12:00.967940 silverback-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-02 23:11:00.000000 silverback-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:12:00.963940 silverback-0.4.0/silverback/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-02 23:11:00.000000 silverback-0.4.0/silverback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-02 23:11:00.000000 silverback-0.4.0/silverback/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-02 23:11:00.000000 silverback-0.4.0/silverback/_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9712 2024-05-02 23:11:00.000000 silverback-0.4.0/silverback/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-02 23:11:00.000000 silverback-0.4.0/silverback/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-05-02 23:11:00.000000 silverback-0.4.0/silverback/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 23:11:00.000000 silverback-0.4.0/silverback/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-05-02 23:11:00.000000 silverback-0.4.0/silverback/recorder.py
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-05-02 23:11:00.000000 silverback-0.4.0/silverback/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-02 23:11:00.000000 silverback-0.4.0/silverback/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-02 23:11:00.000000 silverback-0.4.0/silverback/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-02 23:11:00.000000 silverback-0.4.0/silverback/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-02 23:11:00.000000 silverback-0.4.0/silverback/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-02 23:11:00.000000 silverback-0.4.0/silverback/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-02 23:12:00.000000 silverback-0.4.0/silverback/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:12:00.967940 silverback-0.4.0/silverback.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-02 23:12:00.000000 silverback-0.4.0/silverback.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-02 23:12:00.000000 silverback-0.4.0/silverback.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 23:12:00.000000 silverback-0.4.0/silverback.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-02 23:12:00.000000 silverback-0.4.0/silverback.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 23:12:00.000000 silverback-0.4.0/silverback.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-02 23:12:00.000000 silverback-0.4.0/silverback.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-02 23:12:00.000000 silverback-0.4.0/silverback.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 23:12:00.967940 silverback-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 23:11:00.000000 silverback-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-02 23:11:00.000000 silverback-0.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-02 23:11:00.000000 silverback-0.4.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:42:22.986196 silverback-0.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:42:22.978196 silverback-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:42:22.978196 silverback-0.4.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-04 17:41:26.000000 silverback-0.4.1/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-04 17:41:26.000000 silverback-0.4.1/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-04 17:41:26.000000 silverback-0.4.1/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-04 17:41:26.000000 silverback-0.4.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-04 17:41:26.000000 silverback-0.4.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:42:22.982196 silverback-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-04 17:41:26.000000 silverback-0.4.1/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-04 17:41:26.000000 silverback-0.4.1/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-04 17:41:26.000000 silverback-0.4.1/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-04 17:41:26.000000 silverback-0.4.1/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-04 17:41:26.000000 silverback-0.4.1/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-04 17:41:26.000000 silverback-0.4.1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-04 17:41:26.000000 silverback-0.4.1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-04 17:41:26.000000 silverback-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-04 17:41:26.000000 silverback-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-04 17:41:26.000000 silverback-0.4.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-04 17:41:26.000000 silverback-0.4.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-04 17:41:26.000000 silverback-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-04 17:42:22.986196 silverback-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-04 17:41:26.000000 silverback-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-04 17:41:26.000000 silverback-0.4.1/build_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:42:22.982196 silverback-0.4.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:42:22.982196 silverback-0.4.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/_static/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:42:22.982196 silverback-0.4.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/_templates/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:42:22.982196 silverback-0.4.1/docs/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/commands/run.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/logo.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:42:22.982196 silverback-0.4.1/docs/methoddocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/methoddocs/application.md
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/methoddocs/exceptions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/methoddocs/middlewares.md
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/methoddocs/runner.md
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/methoddocs/subscriptions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/methoddocs/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:42:22.982196 silverback-0.4.1/docs/userguides/
+-rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/userguides/development.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-04 17:41:26.000000 silverback-0.4.1/docs/userguides/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-04 17:41:26.000000 silverback-0.4.1/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-04 17:41:26.000000 silverback-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-04 17:42:22.986196 silverback-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-04 17:41:26.000000 silverback-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:42:22.986196 silverback-0.4.1/silverback/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-04 17:41:26.000000 silverback-0.4.1/silverback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-04 17:41:26.000000 silverback-0.4.1/silverback/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-04 17:41:26.000000 silverback-0.4.1/silverback/_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9712 2024-05-04 17:41:26.000000 silverback-0.4.1/silverback/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-04 17:41:26.000000 silverback-0.4.1/silverback/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-05-04 17:41:26.000000 silverback-0.4.1/silverback/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:41:26.000000 silverback-0.4.1/silverback/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-04 17:41:26.000000 silverback-0.4.1/silverback/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-05-04 17:41:26.000000 silverback-0.4.1/silverback/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-04 17:41:26.000000 silverback-0.4.1/silverback/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-04 17:41:26.000000 silverback-0.4.1/silverback/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-04 17:41:26.000000 silverback-0.4.1/silverback/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-04 17:41:26.000000 silverback-0.4.1/silverback/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-04 17:41:26.000000 silverback-0.4.1/silverback/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-04 17:42:22.000000 silverback-0.4.1/silverback/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:42:22.986196 silverback-0.4.1/silverback.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-04 17:42:22.000000 silverback-0.4.1/silverback.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-04 17:42:22.000000 silverback-0.4.1/silverback.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 17:42:22.000000 silverback-0.4.1/silverback.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-04 17:42:22.000000 silverback-0.4.1/silverback.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 17:42:22.000000 silverback-0.4.1/silverback.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-04 17:42:22.000000 silverback-0.4.1/silverback.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 17:42:22.000000 silverback-0.4.1/silverback.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 17:42:22.986196 silverback-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 17:41:26.000000 silverback-0.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-04 17:41:26.000000 silverback-0.4.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-04 17:41:26.000000 silverback-0.4.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-04 17:41:26.000000 silverback-0.4.1/tests/test_types.py
```

### Comparing `silverback-0.4.0/.github/ISSUE_TEMPLATE/bug.md` & `silverback-0.4.1/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/.github/ISSUE_TEMPLATE/feature.md` & `silverback-0.4.1/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/.github/ISSUE_TEMPLATE/work-item.md` & `silverback-0.4.1/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/.github/release-drafter.yml` & `silverback-0.4.1/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/.github/workflows/codeql.yaml` & `silverback-0.4.1/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/.github/workflows/commitlint.yaml` & `silverback-0.4.1/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/.github/workflows/docs.yaml` & `silverback-0.4.1/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/.github/workflows/prtitle.yaml` & `silverback-0.4.1/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/.github/workflows/publish.yaml` & `silverback-0.4.1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/.github/workflows/test.yaml` & `silverback-0.4.1/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/.gitignore` & `silverback-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/.pre-commit-config.yaml` & `silverback-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/CONTRIBUTING.md` & `silverback-0.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/Dockerfile` & `silverback-0.4.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/LICENSE` & `silverback-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/PKG-INFO` & `silverback-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silverback
-Version: 0.4.0
+Version: 0.4.1
 Summary: Ape SDK for the Silverback platform
 Home-page: https://github.com/ApeWorX/silverback
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `silverback-0.4.0/README.md` & `silverback-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/build_docs.py` & `silverback-0.4.1/build_docs.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/docs/_static/custom.css` & `silverback-0.4.1/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/docs/_static/custom.js` & `silverback-0.4.1/docs/_static/custom.js`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/docs/_templates/layout.html` & `silverback-0.4.1/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/docs/conf.py` & `silverback-0.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/docs/favicon.ico` & `silverback-0.4.1/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/docs/logo.gif` & `silverback-0.4.1/docs/logo.gif`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/docs/userguides/development.md` & `silverback-0.4.1/docs/userguides/development.md`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/example.py` & `silverback-0.4.1/example.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/pyproject.toml` & `silverback-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/setup.py` & `silverback-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/silverback/_cli.py` & `silverback-0.4.1/silverback/_cli.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/silverback/_importer.py` & `silverback-0.4.1/silverback/_importer.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/silverback/application.py` & `silverback-0.4.1/silverback/application.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/silverback/exceptions.py` & `silverback-0.4.1/silverback/exceptions.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/silverback/middlewares.py` & `silverback-0.4.1/silverback/middlewares.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/silverback/recorder.py` & `silverback-0.4.1/silverback/recorder.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,23 +3,15 @@
 from typing import Any, Iterator
 
 from ape.logging import get_logger
 from pydantic import BaseModel, Field
 from taskiq import TaskiqResult
 from typing_extensions import Self  # Introduced 3.11
 
-from .types import (
-    Datapoint,
-    ScalarDatapoint,
-    ScalarType,
-    SilverbackID,
-    UTCTimestamp,
-    iso_format,
-    utc_now,
-)
+from .types import Datapoints, SilverbackID, UTCTimestamp, iso_format, utc_now
 
 logger = get_logger(__name__)
 
 
 class TaskResult(BaseModel):
     # NOTE: Model must eventually serialize using PyArrow/Parquet for long-term storage
 
@@ -31,47 +23,25 @@
     # NOTE: intended to use default when creating a model with this type
     completed: UTCTimestamp = Field(default_factory=utc_now)
 
     # System Metrics here (must default to None in case they are missing)
     block_number: int | None = None
 
     # Custom user metrics here
-    metrics: dict[str, Datapoint] = {}
+    metrics: Datapoints
 
     @classmethod
-    def _extract_custom_metrics(cls, result: Any, task_name: str) -> dict[str, Datapoint]:
-        if isinstance(result, Datapoint):  # type: ignore[arg-type,misc]
-            return {"result": result}
+    def _extract_custom_metrics(cls, return_value: Any, task_name: str) -> Datapoints:
+        if return_value is None:
+            return Datapoints(root={})
 
-        elif isinstance(result, ScalarType):  # type: ignore[arg-type,misc]
-            return {"result": ScalarDatapoint(data=result)}
+        elif not isinstance(return_value, dict):
+            return_value = {"return_value": return_value}
 
-        elif result is None:
-            return {}
-
-        elif not isinstance(result, dict):
-            logger.warning(f"Cannot handle return type of '{task_name}': '{type(result)}'.")
-            return {}
-
-        converted_result = {}
-
-        for metric_name, metric_value in result.items():
-            if isinstance(metric_value, Datapoint):  # type: ignore[arg-type,misc]
-                converted_result[metric_name] = metric_value
-
-            elif isinstance(metric_value, ScalarType):  # type: ignore[arg-type,misc]
-                converted_result[metric_name] = ScalarDatapoint(data=metric_value)
-
-            else:
-                logger.warning(
-                    f"Cannot handle type of metric '{task_name}.{metric_name}':"
-                    f" '{type(metric_value)}'."
-                )
-
-        return converted_result
+        return Datapoints(root=return_value)
 
     @classmethod
     def _extract_system_metrics(cls, labels: dict) -> dict:
         metrics = {}
 
         if block_number := labels.get("block_number"):
             metrics["block_number"] = int(block_number)
```

### Comparing `silverback-0.4.0/silverback/runner.py` & `silverback-0.4.1/silverback/runner.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/silverback/settings.py` & `silverback-0.4.1/silverback/settings.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/silverback/state.py` & `silverback-0.4.1/silverback/state.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/silverback/subscriptions.py` & `silverback-0.4.1/silverback/subscriptions.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/silverback/types.py` & `silverback-0.4.1/silverback/types.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from datetime import datetime, timezone
 from decimal import Decimal
 from enum import Enum  # NOTE: `enum.StrEnum` only in Python 3.11+
 from typing import Literal
 
-from pydantic import BaseModel, Field
+from ape.logging import get_logger
+from pydantic import BaseModel, Field, RootModel, ValidationError, model_validator
 from pydantic.functional_serializers import PlainSerializer
 from typing_extensions import Annotated
 
+logger = get_logger(__name__)
+
 
 class TaskType(str, Enum):
     STARTUP = "startup"
     NEW_BLOCKS = "block"
     EVENT_LOG = "event"
     SHUTDOWN = "shutdown"
 
@@ -43,18 +46,61 @@
     type: str  # discriminator
 
 
 # NOTE: Maximum supported parquet integer type: https://parquet.apache.org/docs/file-format/types
 Int96 = Annotated[int, Field(ge=-(2**95), le=2**95 - 1)]
 # NOTE: only these types of data are implicitly converted e.g. `{"something": 1, "else": 0.001}`
 ScalarType = bool | Int96 | float | Decimal
+# NOTE: Interesting side effect is that `int` outside the INT96 range parse as `Decimal`
+#       This is okay, preferable actually, because it means we can store ints outside that range
 
 
 class ScalarDatapoint(_BaseDatapoint):
     type: Literal["scalar"] = "scalar"
     data: ScalarType
 
 
-# NOTE: Other datapoint types must be explicitly used
+# NOTE: Other datapoint types must be explicitly defined as subclasses of `_BaseDatapoint`
+#       Users will have to import and use these directly
 
-# TODO: Other datapoint types added to union here...
+# NOTE: Other datapoint types must be added to this union
 Datapoint = ScalarDatapoint
+
+
+class Datapoints(RootModel):
+    root: dict[str, Datapoint]
+
+    @model_validator(mode="before")
+    def parse_datapoints(cls, datapoints: dict) -> dict:
+        names_to_remove: dict[str, ValidationError] = {}
+        # Automatically convert raw scalar types
+        for name in datapoints:
+            if not isinstance(datapoints[name], Datapoint):
+                try:
+                    datapoints[name] = ScalarDatapoint(data=datapoints[name])
+                except ValidationError as e:
+                    names_to_remove[name] = e
+
+        # Prune and raise a warning about unconverted datapoints
+        for name in names_to_remove:
+            data = datapoints.pop(name)
+            logger.warning(
+                f"Cannot convert datapoint '{name}' of type '{type(data)}': {names_to_remove[name]}"
+            )
+
+        return datapoints
+
+    # Add dict methods
+    def get(self, key: str, default: Datapoint | None = None) -> Datapoint | None:
+        if key in self:
+            return self[key]
+
+        return default
+
+    def __iter__(self):
+        return iter(self.root)
+
+    def __getitem__(self, item):
+        return self.root[item]
+
+    def items(self):
+        return self.root.items()
```

### Comparing `silverback-0.4.0/silverback/utils.py` & `silverback-0.4.1/silverback/utils.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.0/silverback.egg-info/PKG-INFO` & `silverback-0.4.1/silverback.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silverback
-Version: 0.4.0
+Version: 0.4.1
 Summary: Ape SDK for the Silverback platform
 Home-page: https://github.com/ApeWorX/silverback
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `silverback-0.4.0/silverback.egg-info/SOURCES.txt` & `silverback-0.4.1/silverback.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -57,8 +57,9 @@
 silverback.egg-info/dependency_links.txt
 silverback.egg-info/entry_points.txt
 silverback.egg-info/not-zip-safe
 silverback.egg-info/requires.txt
 silverback.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
-tests/test_cli.py
+tests/test_cli.py
+tests/test_types.py
```

### Comparing `silverback-0.4.0/silverback.egg-info/requires.txt` & `silverback-0.4.1/silverback.egg-info/requires.txt`

 * *Files identical despite different names*

