# Comparing `tmp/citric-1.0.1a1.tar.gz` & `tmp/citric-1.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Wed May  1 17:46:34 2024, max compression
+gzip compressed data, last modified: Sat May  4 03:21:31 2024, max compression
```

## Comparing `citric-1.0.1a1.tar` & `citric-1.0.1a2.tar`

### file list

```diff
@@ -1,140 +1,140 @@
--rw-r--r--   0        0        0     1081 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changie.yaml
--rw-r--r--   0        0        0       85 2024-05-01 17:46:34.000000 citric-1.0.1a1/.flake8
--rw-r--r--   0        0        0       36 2024-05-01 17:46:34.000000 citric-1.0.1a1/.gitattributes
--rw-r--r--   0        0        0     1699 2024-05-01 17:46:34.000000 citric-1.0.1a1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      290 2024-05-01 17:46:34.000000 citric-1.0.1a1/.readthedocs.yaml
--rw-r--r--   0        0        0       54 2024-05-01 17:46:34.000000 citric-1.0.1a1/.sonarcloud.properties
--rw-r--r--   0        0        0    10546 2024-05-01 17:46:34.000000 citric-1.0.1a1/CHANGELOG.md
--rw-r--r--   0        0        0      337 2024-05-01 17:46:34.000000 citric-1.0.1a1/CITATION.cff
--rw-r--r--   0        0        0     5225 2024-05-01 17:46:34.000000 citric-1.0.1a1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      837 2024-05-01 17:46:34.000000 citric-1.0.1a1/SECURITY.md
--rw-r--r--   0        0        0      247 2024-05-01 17:46:34.000000 citric-1.0.1a1/codecov.yml
--rw-r--r--   0        0        0      889 2024-05-01 17:46:34.000000 citric-1.0.1a1/docker-compose.mysql.yml
--rw-r--r--   0        0        0      323 2024-05-01 17:46:34.000000 citric-1.0.1a1/docker-compose.ref.yml
--rw-r--r--   0        0        0     1701 2024-05-01 17:46:34.000000 citric-1.0.1a1/docker-compose.yml
--rw-r--r--   0        0        0     4847 2024-05-01 17:46:34.000000 citric-1.0.1a1/noxfile.py
--rw-r--r--   0        0        0      491 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.0.1.md
--rw-r--r--   0        0        0     1152 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.0.10.md
--rw-r--r--   0        0        0      246 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.0.11.md
--rw-r--r--   0        0        0      132 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.0.12.md
--rw-r--r--   0        0        0      135 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.0.13.md
--rw-r--r--   0        0        0      129 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.0.14.md
--rw-r--r--   0        0        0      157 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.0.2.md
--rw-r--r--   0        0        0      126 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.0.3.md
--rw-r--r--   0        0        0      186 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.0.4.md
--rw-r--r--   0        0        0      245 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.0.5.md
--rw-r--r--   0        0        0      114 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.0.6.md
--rw-r--r--   0        0        0      141 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.0.7.md
--rw-r--r--   0        0        0      224 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.0.8.md
--rw-r--r--   0        0        0      314 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.0.9.md
--rw-r--r--   0        0        0      132 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.1.0.md
--rw-r--r--   0        0        0      669 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.10.0.md
--rw-r--r--   0        0        0      269 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.2.0.md
--rw-r--r--   0        0        0      129 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.3.0.md
--rw-r--r--   0        0        0      506 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.4.0.md
--rw-r--r--   0        0        0      142 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.4.1.md
--rw-r--r--   0        0        0      251 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.4.2.md
--rw-r--r--   0        0        0      167 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.4.3.md
--rw-r--r--   0        0        0      295 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.4.4.md
--rw-r--r--   0        0        0      152 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.4.5.md
--rw-r--r--   0        0        0      227 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.5.0.md
--rw-r--r--   0        0        0      364 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.6.0.md
--rw-r--r--   0        0        0      260 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.7.0.md
--rw-r--r--   0        0        0      141 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.7.1-b1.md
--rw-r--r--   0        0        0      141 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.7.1-b2.md
--rw-r--r--   0        0        0      231 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.7.1-b3.md
--rw-r--r--   0        0        0      136 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.7.1.md
--rw-r--r--   0        0        0      151 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.7.2.md
--rw-r--r--   0        0        0      756 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.8.0.md
--rw-r--r--   0        0        0      590 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/0.9.0.md
--rw-r--r--   0        0        0      672 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/1.0.0.md
--rw-r--r--   0        0        0      304 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/header.tpl.md
--rw-r--r--   0        0        0        0 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/unreleased/.gitkeep
--rw-r--r--   0        0        0      142 2024-05-01 17:46:34.000000 citric-1.0.1a1/.changes/unreleased/Fixed-20240222-213639.yaml
--rw-r--r--   0        0        0     2399 2024-05-01 17:46:34.000000 citric-1.0.1a1/.circleci/config.yml
--rw-r--r--   0        0        0      138 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0     1326 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/dependabot.yml
--rw-r--r--   0        0        0     1007 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/pull_request_template.md
--rw-r--r--   0        0        0       59 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/semantic.yml
--rw-r--r--   0        0        0     2154 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/ISSUE_TEMPLATE/BUG.yml
--rw-r--r--   0        0        0       27 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1013 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/ISSUE_TEMPLATE/feature.yml
--rw-r--r--   0        0        0     1044 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/actions/install-tools/action.yml
--rw-r--r--   0        0        0        0 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/badges/.gitkeep
--rw-r--r--   0        0        0     1295 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/workflows/api-changes.yml
--rw-r--r--   0        0        0     2121 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/workflows/build.yml
--rw-r--r--   0        0        0       68 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/workflows/constraints.txt
--rw-r--r--   0        0        0     3461 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/workflows/gen-release-pr.yml
--rw-r--r--   0        0        0      319 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/workflows/pr-preview-links.yml
--rw-r--r--   0        0        0     2891 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/workflows/scorecard.yml
--rw-r--r--   0        0        0    10275 2024-05-01 17:46:34.000000 citric-1.0.1a1/.github/workflows/tests.yml
--rw-r--r--   0        0        0      267 2024-05-01 17:46:34.000000 citric-1.0.1a1/code_samples/auth_plugin.py
--rw-r--r--   0        0        0      336 2024-05-01 17:46:34.000000 citric-1.0.1a1/code_samples/context_manager.py
--rw-r--r--   0        0        0      563 2024-05-01 17:46:34.000000 citric-1.0.1a1/code_samples/custom_requests_session.py
--rw-r--r--   0        0        0      626 2024-05-01 17:46:34.000000 citric-1.0.1a1/code_samples/duckdb_sql.py
--rw-r--r--   0        0        0      573 2024-05-01 17:46:34.000000 citric-1.0.1a1/code_samples/get_surveys.py
--rw-r--r--   0        0        0      583 2024-05-01 17:46:34.000000 citric-1.0.1a1/code_samples/pandas_df.py
--rw-r--r--   0        0        0      517 2024-05-01 17:46:34.000000 citric-1.0.1a1/code_samples/requests_session_attributes.py
--rw-r--r--   0        0        0      159 2024-05-01 17:46:34.000000 citric-1.0.1a1/code_samples/ruff.toml
--rw-r--r--   0        0        0      521 2024-05-01 17:46:34.000000 citric-1.0.1a1/code_samples/session_attr.py
--rw-r--r--   0        0        0      561 2024-05-01 17:46:34.000000 citric-1.0.1a1/code_samples/upload_s3.py
--rw-r--r--   0        0        0       33 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/changelog.md
--rw-r--r--   0        0        0   106926 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/code.png
--rw-r--r--   0        0        0     6110 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/conf.py
--rw-r--r--   0        0        0       54 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/googled10b55fb460af091.html
--rw-r--r--   0        0        0     2876 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/how-to.md
--rw-r--r--   0        0        0     2571 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/index.md
--rw-r--r--   0        0        0       41 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/license.rst
--rw-r--r--   0        0        0     2080 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/requirements.txt
--rw-r--r--   0        0        0      740 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/rest_coverage.md
--rw-r--r--   0        0        0    11121 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/rpc_coverage.md
--rw-r--r--   0        0        0        0 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/_ext/__init__.py
--rw-r--r--   0        0        0     2521 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/_ext/limesurvey_future.py
--rw-r--r--   0        0        0       42 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/contributing/code-of-conduct.md
--rw-r--r--   0        0        0     2418 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/contributing/docker.md
--rw-r--r--   0        0        0      299 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/contributing/docs.md
--rw-r--r--   0        0        0     1244 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/contributing/environment.md
--rw-r--r--   0        0        0     1472 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/contributing/getting-started.md
--rw-r--r--   0        0        0      822 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/contributing/release.md
--rw-r--r--   0        0        0      626 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/contributing/testing.md
--rw-r--r--   0        0        0      881 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/contributing/unreleased-features.md
--rw-r--r--   0        0        0       19 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/notebooks/.gitignore
--rw-r--r--   0        0        0    18574 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/notebooks/duckdb.ipynb
--rw-r--r--   0        0        0     6352 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/notebooks/import_s3.ipynb
--rw-r--r--   0        0        0    10331 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/notebooks/pandas_sqlite.ipynb
--rw-r--r--   0        0        0     5862 2024-05-01 17:46:34.000000 citric-1.0.1a1/docs/notebooks/parse_files.ipynb
--rw-r--r--   0        0        0     6976 2024-05-01 17:46:34.000000 citric-1.0.1a1/examples/free_text.lsq
--rw-r--r--   0        0        0    11072 2024-05-01 17:46:34.000000 citric-1.0.1a1/examples/group.lsg
--rw-r--r--   0        0        0    24464 2024-05-01 17:46:34.000000 citric-1.0.1a1/examples/limesurvey_survey_432535.lss
--rw-r--r--   0        0        0    25801 2024-05-01 17:46:34.000000 citric-1.0.1a1/examples/survey.lss
--rw-r--r--   0        0        0     1824 2024-05-01 17:46:34.000000 citric-1.0.1a1/scripts/docker_tags.py
--rw-r--r--   0        0        0      299 2024-05-01 17:46:34.000000 citric-1.0.1a1/src/citric/__init__.py
--rw-r--r--   0        0        0     2450 2024-05-01 17:46:34.000000 citric-1.0.1a1/src/citric/_compat.py
--rw-r--r--   0        0        0    50489 2024-05-01 17:46:34.000000 citric-1.0.1a1/src/citric/client.py
--rw-r--r--   0        0        0     2373 2024-05-01 17:46:34.000000 citric-1.0.1a1/src/citric/enums.py
--rw-r--r--   0        0        0     1192 2024-05-01 17:46:34.000000 citric-1.0.1a1/src/citric/exceptions.py
--rw-r--r--   0        0        0     1123 2024-05-01 17:46:34.000000 citric-1.0.1a1/src/citric/method.py
--rw-r--r--   0        0        0     1183 2024-05-01 17:46:34.000000 citric-1.0.1a1/src/citric/objects.py
--rw-r--r--   0        0        0        0 2024-05-01 17:46:34.000000 citric-1.0.1a1/src/citric/py.typed
--rw-r--r--   0        0        0     7152 2024-05-01 17:46:34.000000 citric-1.0.1a1/src/citric/session.py
--rw-r--r--   0        0        0    12698 2024-05-01 17:46:34.000000 citric-1.0.1a1/src/citric/types.py
--rw-r--r--   0        0        0      128 2024-05-01 17:46:34.000000 citric-1.0.1a1/src/citric/_rest/__init__.py
--rw-r--r--   0        0        0     5258 2024-05-01 17:46:34.000000 citric-1.0.1a1/src/citric/_rest/client.py
--rw-r--r--   0        0        0       72 2024-05-01 17:46:34.000000 citric-1.0.1a1/tests/__init__.py
--rw-r--r--   0        0        0     7664 2024-05-01 17:46:34.000000 citric-1.0.1a1/tests/conftest.py
--rw-r--r--   0        0        0      498 2024-05-01 17:46:34.000000 citric-1.0.1a1/tests/fixtures.py
--rw-r--r--   0        0        0    17380 2024-05-01 17:46:34.000000 citric-1.0.1a1/tests/test_client.py
--rw-r--r--   0        0        0     1034 2024-05-01 17:46:34.000000 citric-1.0.1a1/tests/test_compat.py
--rw-r--r--   0        0        0     5348 2024-05-01 17:46:34.000000 citric-1.0.1a1/tests/test_rest.py
--rw-r--r--   0        0        0     5380 2024-05-01 17:46:34.000000 citric-1.0.1a1/tests/test_rpc.py
--rw-r--r--   0        0        0       38 2024-05-01 17:46:34.000000 citric-1.0.1a1/tests/integration/__init__.py
--rw-r--r--   0        0        0     1762 2024-05-01 17:46:34.000000 citric-1.0.1a1/tests/integration/conftest.py
--rw-r--r--   0        0        0     2231 2024-05-01 17:46:34.000000 citric-1.0.1a1/tests/integration/test_rest_client.py
--rw-r--r--   0        0        0    27436 2024-05-01 17:46:34.000000 citric-1.0.1a1/tests/integration/test_rpc_client.py
--rw-r--r--   0        0        0     1393 2024-05-01 17:46:34.000000 citric-1.0.1a1/tests/resources/config.php
--rw-r--r--   0        0        0     1950 2024-05-01 17:46:34.000000 citric-1.0.1a1/.gitignore
--rw-r--r--   0        0        0      131 2024-05-01 17:46:34.000000 citric-1.0.1a1/AUTHORS.md
--rw-r--r--   0        0        0     1083 2024-05-01 17:46:34.000000 citric-1.0.1a1/LICENSE
--rw-r--r--   0        0        0     5453 2024-05-01 17:46:34.000000 citric-1.0.1a1/README.md
--rw-r--r--   0        0        0     8059 2024-05-01 17:46:34.000000 citric-1.0.1a1/pyproject.toml
--rw-r--r--   0        0        0    11802 2024-05-01 17:46:34.000000 citric-1.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changie.yaml
+-rw-r--r--   0        0        0       85 2024-05-04 03:21:31.000000 citric-1.0.1a2/.flake8
+-rw-r--r--   0        0        0       36 2024-05-04 03:21:31.000000 citric-1.0.1a2/.gitattributes
+-rw-r--r--   0        0        0     1699 2024-05-04 03:21:31.000000 citric-1.0.1a2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      290 2024-05-04 03:21:31.000000 citric-1.0.1a2/.readthedocs.yaml
+-rw-r--r--   0        0        0       54 2024-05-04 03:21:31.000000 citric-1.0.1a2/.sonarcloud.properties
+-rw-r--r--   0        0        0    10546 2024-05-04 03:21:31.000000 citric-1.0.1a2/CHANGELOG.md
+-rw-r--r--   0        0        0      337 2024-05-04 03:21:31.000000 citric-1.0.1a2/CITATION.cff
+-rw-r--r--   0        0        0     5225 2024-05-04 03:21:31.000000 citric-1.0.1a2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      837 2024-05-04 03:21:31.000000 citric-1.0.1a2/SECURITY.md
+-rw-r--r--   0        0        0      247 2024-05-04 03:21:31.000000 citric-1.0.1a2/codecov.yml
+-rw-r--r--   0        0        0      889 2024-05-04 03:21:31.000000 citric-1.0.1a2/docker-compose.mysql.yml
+-rw-r--r--   0        0        0      323 2024-05-04 03:21:31.000000 citric-1.0.1a2/docker-compose.ref.yml
+-rw-r--r--   0        0        0     1701 2024-05-04 03:21:31.000000 citric-1.0.1a2/docker-compose.yml
+-rw-r--r--   0        0        0     4847 2024-05-04 03:21:31.000000 citric-1.0.1a2/noxfile.py
+-rw-r--r--   0        0        0      491 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.0.1.md
+-rw-r--r--   0        0        0     1152 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.0.10.md
+-rw-r--r--   0        0        0      246 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.0.11.md
+-rw-r--r--   0        0        0      132 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.0.12.md
+-rw-r--r--   0        0        0      135 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.0.13.md
+-rw-r--r--   0        0        0      129 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.0.14.md
+-rw-r--r--   0        0        0      157 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.0.2.md
+-rw-r--r--   0        0        0      126 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.0.3.md
+-rw-r--r--   0        0        0      186 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.0.4.md
+-rw-r--r--   0        0        0      245 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.0.5.md
+-rw-r--r--   0        0        0      114 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.0.6.md
+-rw-r--r--   0        0        0      141 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.0.7.md
+-rw-r--r--   0        0        0      224 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.0.8.md
+-rw-r--r--   0        0        0      314 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.0.9.md
+-rw-r--r--   0        0        0      132 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.1.0.md
+-rw-r--r--   0        0        0      669 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.10.0.md
+-rw-r--r--   0        0        0      269 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.2.0.md
+-rw-r--r--   0        0        0      129 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.3.0.md
+-rw-r--r--   0        0        0      506 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.4.0.md
+-rw-r--r--   0        0        0      142 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.4.1.md
+-rw-r--r--   0        0        0      251 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.4.2.md
+-rw-r--r--   0        0        0      167 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.4.3.md
+-rw-r--r--   0        0        0      295 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.4.4.md
+-rw-r--r--   0        0        0      152 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.4.5.md
+-rw-r--r--   0        0        0      227 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.5.0.md
+-rw-r--r--   0        0        0      364 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.6.0.md
+-rw-r--r--   0        0        0      260 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.7.0.md
+-rw-r--r--   0        0        0      141 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.7.1-b1.md
+-rw-r--r--   0        0        0      141 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.7.1-b2.md
+-rw-r--r--   0        0        0      231 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.7.1-b3.md
+-rw-r--r--   0        0        0      136 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.7.1.md
+-rw-r--r--   0        0        0      151 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.7.2.md
+-rw-r--r--   0        0        0      756 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.8.0.md
+-rw-r--r--   0        0        0      590 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/0.9.0.md
+-rw-r--r--   0        0        0      672 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/1.0.0.md
+-rw-r--r--   0        0        0      304 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/header.tpl.md
+-rw-r--r--   0        0        0        0 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/unreleased/.gitkeep
+-rw-r--r--   0        0        0      142 2024-05-04 03:21:31.000000 citric-1.0.1a2/.changes/unreleased/Fixed-20240222-213639.yaml
+-rw-r--r--   0        0        0     2399 2024-05-04 03:21:31.000000 citric-1.0.1a2/.circleci/config.yml
+-rw-r--r--   0        0        0      138 2024-05-04 03:21:31.000000 citric-1.0.1a2/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1326 2024-05-04 03:21:31.000000 citric-1.0.1a2/.github/dependabot.yml
+-rw-r--r--   0        0        0     1007 2024-05-04 03:21:31.000000 citric-1.0.1a2/.github/pull_request_template.md
+-rw-r--r--   0        0        0       59 2024-05-04 03:21:31.000000 citric-1.0.1a2/.github/semantic.yml
+-rw-r--r--   0        0        0     2154 2024-05-04 03:21:31.000000 citric-1.0.1a2/.github/ISSUE_TEMPLATE/BUG.yml
+-rw-r--r--   0        0        0       27 2024-05-04 03:21:31.000000 citric-1.0.1a2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1013 2024-05-04 03:21:31.000000 citric-1.0.1a2/.github/ISSUE_TEMPLATE/feature.yml
+-rw-r--r--   0        0        0     1044 2024-05-04 03:21:31.000000 citric-1.0.1a2/.github/actions/install-tools/action.yml
+-rw-r--r--   0        0        0        0 2024-05-04 03:21:31.000000 citric-1.0.1a2/.github/badges/.gitkeep
+-rw-r--r--   0        0        0     1295 2024-05-04 03:21:31.000000 citric-1.0.1a2/.github/workflows/api-changes.yml
+-rw-r--r--   0        0        0     2214 2024-05-04 03:21:31.000000 citric-1.0.1a2/.github/workflows/build.yml
+-rw-r--r--   0        0        0       68 2024-05-04 03:21:31.000000 citric-1.0.1a2/.github/workflows/constraints.txt
+-rw-r--r--   0        0        0     3461 2024-05-04 03:21:31.000000 citric-1.0.1a2/.github/workflows/gen-release-pr.yml
+-rw-r--r--   0        0        0      319 2024-05-04 03:21:31.000000 citric-1.0.1a2/.github/workflows/pr-preview-links.yml
+-rw-r--r--   0        0        0     2891 2024-05-04 03:21:31.000000 citric-1.0.1a2/.github/workflows/scorecard.yml
+-rw-r--r--   0        0        0    10275 2024-05-04 03:21:31.000000 citric-1.0.1a2/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      267 2024-05-04 03:21:31.000000 citric-1.0.1a2/code_samples/auth_plugin.py
+-rw-r--r--   0        0        0      336 2024-05-04 03:21:31.000000 citric-1.0.1a2/code_samples/context_manager.py
+-rw-r--r--   0        0        0      563 2024-05-04 03:21:31.000000 citric-1.0.1a2/code_samples/custom_requests_session.py
+-rw-r--r--   0        0        0      626 2024-05-04 03:21:31.000000 citric-1.0.1a2/code_samples/duckdb_sql.py
+-rw-r--r--   0        0        0      573 2024-05-04 03:21:31.000000 citric-1.0.1a2/code_samples/get_surveys.py
+-rw-r--r--   0        0        0      583 2024-05-04 03:21:31.000000 citric-1.0.1a2/code_samples/pandas_df.py
+-rw-r--r--   0        0        0      517 2024-05-04 03:21:31.000000 citric-1.0.1a2/code_samples/requests_session_attributes.py
+-rw-r--r--   0        0        0      159 2024-05-04 03:21:31.000000 citric-1.0.1a2/code_samples/ruff.toml
+-rw-r--r--   0        0        0      521 2024-05-04 03:21:31.000000 citric-1.0.1a2/code_samples/session_attr.py
+-rw-r--r--   0        0        0      561 2024-05-04 03:21:31.000000 citric-1.0.1a2/code_samples/upload_s3.py
+-rw-r--r--   0        0        0       33 2024-05-04 03:21:31.000000 citric-1.0.1a2/docs/changelog.md
+-rw-r--r--   0        0        0   106926 2024-05-04 03:21:31.000000 citric-1.0.1a2/docs/code.png
+-rw-r--r--   0        0        0     6110 2024-05-04 03:21:31.000000 citric-1.0.1a2/docs/conf.py
+-rw-r--r--   0        0        0       54 2024-05-04 03:21:31.000000 citric-1.0.1a2/docs/googled10b55fb460af091.html
+-rw-r--r--   0        0        0     2876 2024-05-04 03:21:31.000000 citric-1.0.1a2/docs/how-to.md
+-rw-r--r--   0        0        0     2571 2024-05-04 03:21:31.000000 citric-1.0.1a2/docs/index.md
+-rw-r--r--   0        0        0       41 2024-05-04 03:21:31.000000 citric-1.0.1a2/docs/license.rst
+-rw-r--r--   0        0        0     2080 2024-05-04 03:21:31.000000 citric-1.0.1a2/docs/requirements.txt
+-rw-r--r--   0        0        0      740 2024-05-04 03:21:31.000000 citric-1.0.1a2/docs/rest_coverage.md
+-rw-r--r--   0        0        0    11121 2024-05-04 03:21:31.000000 citric-1.0.1a2/docs/rpc_coverage.md
+-rw-r--r--   0        0        0        0 2024-05-04 03:21:31.000000 citric-1.0.1a2/docs/_ext/__init__.py
+-rw-r--r--   0        0        0     2521 2024-05-04 03:21:31.000000 citric-1.0.1a2/docs/_ext/limesurvey_future.py
+-rw-r--r--   0        0        0       42 2024-05-04 03:21:31.000000 citric-1.0.1a2/docs/contributing/code-of-conduct.md
+-rw-r--r--   0        0        0     2418 2024-05-04 03:21:31.000000 citric-1.0.1a2/docs/contributing/docker.md
+-rw-r--r--   0        0        0      299 2024-05-04 03:21:31.000000 citric-1.0.1a2/docs/contributing/docs.md
+-rw-r--r--   0        0        0     1244 2024-05-04 03:21:31.000000 citric-1.0.1a2/docs/contributing/environment.md
+-rw-r--r--   0        0        0     1472 2024-05-04 03:21:31.000000 citric-1.0.1a2/docs/contributing/getting-started.md
+-rw-r--r--   0        0        0      822 2024-05-04 03:21:31.000000 citric-1.0.1a2/docs/contributing/release.md
+-rw-r--r--   0        0        0      626 2024-05-04 03:21:31.000000 citric-1.0.1a2/docs/contributing/testing.md
+-rw-r--r--   0        0        0      881 2024-05-04 03:21:31.000000 citric-1.0.1a2/docs/contributing/unreleased-features.md
+-rw-r--r--   0        0        0       19 2024-05-04 03:21:31.000000 citric-1.0.1a2/docs/notebooks/.gitignore
+-rw-r--r--   0        0        0    18574 2024-05-04 03:21:31.000000 citric-1.0.1a2/docs/notebooks/duckdb.ipynb
+-rw-r--r--   0        0        0     6352 2024-05-04 03:21:31.000000 citric-1.0.1a2/docs/notebooks/import_s3.ipynb
+-rw-r--r--   0        0        0    10331 2024-05-04 03:21:31.000000 citric-1.0.1a2/docs/notebooks/pandas_sqlite.ipynb
+-rw-r--r--   0        0        0     5862 2024-05-04 03:21:31.000000 citric-1.0.1a2/docs/notebooks/parse_files.ipynb
+-rw-r--r--   0        0        0     6976 2024-05-04 03:21:31.000000 citric-1.0.1a2/examples/free_text.lsq
+-rw-r--r--   0        0        0    11072 2024-05-04 03:21:31.000000 citric-1.0.1a2/examples/group.lsg
+-rw-r--r--   0        0        0    24464 2024-05-04 03:21:31.000000 citric-1.0.1a2/examples/limesurvey_survey_432535.lss
+-rw-r--r--   0        0        0    25801 2024-05-04 03:21:31.000000 citric-1.0.1a2/examples/survey.lss
+-rw-r--r--   0        0        0     1824 2024-05-04 03:21:31.000000 citric-1.0.1a2/scripts/docker_tags.py
+-rw-r--r--   0        0        0      299 2024-05-04 03:21:31.000000 citric-1.0.1a2/src/citric/__init__.py
+-rw-r--r--   0        0        0     2450 2024-05-04 03:21:31.000000 citric-1.0.1a2/src/citric/_compat.py
+-rw-r--r--   0        0        0    50489 2024-05-04 03:21:31.000000 citric-1.0.1a2/src/citric/client.py
+-rw-r--r--   0        0        0     2373 2024-05-04 03:21:31.000000 citric-1.0.1a2/src/citric/enums.py
+-rw-r--r--   0        0        0     1192 2024-05-04 03:21:31.000000 citric-1.0.1a2/src/citric/exceptions.py
+-rw-r--r--   0        0        0     1123 2024-05-04 03:21:31.000000 citric-1.0.1a2/src/citric/method.py
+-rw-r--r--   0        0        0     1183 2024-05-04 03:21:31.000000 citric-1.0.1a2/src/citric/objects.py
+-rw-r--r--   0        0        0        0 2024-05-04 03:21:31.000000 citric-1.0.1a2/src/citric/py.typed
+-rw-r--r--   0        0        0     7152 2024-05-04 03:21:31.000000 citric-1.0.1a2/src/citric/session.py
+-rw-r--r--   0        0        0    12698 2024-05-04 03:21:31.000000 citric-1.0.1a2/src/citric/types.py
+-rw-r--r--   0        0        0      128 2024-05-04 03:21:31.000000 citric-1.0.1a2/src/citric/_rest/__init__.py
+-rw-r--r--   0        0        0     5258 2024-05-04 03:21:31.000000 citric-1.0.1a2/src/citric/_rest/client.py
+-rw-r--r--   0        0        0       72 2024-05-04 03:21:31.000000 citric-1.0.1a2/tests/__init__.py
+-rw-r--r--   0        0        0     7664 2024-05-04 03:21:31.000000 citric-1.0.1a2/tests/conftest.py
+-rw-r--r--   0        0        0      498 2024-05-04 03:21:31.000000 citric-1.0.1a2/tests/fixtures.py
+-rw-r--r--   0        0        0    17380 2024-05-04 03:21:31.000000 citric-1.0.1a2/tests/test_client.py
+-rw-r--r--   0        0        0     1034 2024-05-04 03:21:31.000000 citric-1.0.1a2/tests/test_compat.py
+-rw-r--r--   0        0        0     5348 2024-05-04 03:21:31.000000 citric-1.0.1a2/tests/test_rest.py
+-rw-r--r--   0        0        0     5380 2024-05-04 03:21:31.000000 citric-1.0.1a2/tests/test_rpc.py
+-rw-r--r--   0        0        0       38 2024-05-04 03:21:31.000000 citric-1.0.1a2/tests/integration/__init__.py
+-rw-r--r--   0        0        0     1762 2024-05-04 03:21:31.000000 citric-1.0.1a2/tests/integration/conftest.py
+-rw-r--r--   0        0        0     2231 2024-05-04 03:21:31.000000 citric-1.0.1a2/tests/integration/test_rest_client.py
+-rw-r--r--   0        0        0    27436 2024-05-04 03:21:31.000000 citric-1.0.1a2/tests/integration/test_rpc_client.py
+-rw-r--r--   0        0        0     1393 2024-05-04 03:21:31.000000 citric-1.0.1a2/tests/resources/config.php
+-rw-r--r--   0        0        0     1950 2024-05-04 03:21:31.000000 citric-1.0.1a2/.gitignore
+-rw-r--r--   0        0        0      131 2024-05-04 03:21:31.000000 citric-1.0.1a2/AUTHORS.md
+-rw-r--r--   0        0        0     1083 2024-05-04 03:21:31.000000 citric-1.0.1a2/LICENSE
+-rw-r--r--   0        0        0     5453 2024-05-04 03:21:31.000000 citric-1.0.1a2/README.md
+-rw-r--r--   0        0        0     8059 2024-05-04 03:21:31.000000 citric-1.0.1a2/pyproject.toml
+-rw-r--r--   0        0        0    11802 2024-05-04 03:21:31.000000 citric-1.0.1a2/PKG-INFO
```

### Comparing `citric-1.0.1a1/.changie.yaml` & `citric-1.0.1a2/.changie.yaml`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/.pre-commit-config.yaml` & `citric-1.0.1a2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/CHANGELOG.md` & `citric-1.0.1a2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/CODE_OF_CONDUCT.md` & `citric-1.0.1a2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/SECURITY.md` & `citric-1.0.1a2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/docker-compose.mysql.yml` & `citric-1.0.1a2/docker-compose.mysql.yml`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/docker-compose.yml` & `citric-1.0.1a2/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/noxfile.py` & `citric-1.0.1a2/noxfile.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/.changes/0.0.10.md` & `citric-1.0.1a2/.changes/0.0.10.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/.changes/0.10.0.md` & `citric-1.0.1a2/.changes/0.10.0.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/.changes/0.8.0.md` & `citric-1.0.1a2/.changes/0.8.0.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/.changes/0.9.0.md` & `citric-1.0.1a2/.changes/0.9.0.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/.changes/1.0.0.md` & `citric-1.0.1a2/.changes/1.0.0.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/.circleci/config.yml` & `citric-1.0.1a2/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/.github/dependabot.yml` & `citric-1.0.1a2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/.github/pull_request_template.md` & `citric-1.0.1a2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/.github/ISSUE_TEMPLATE/BUG.yml` & `citric-1.0.1a2/.github/ISSUE_TEMPLATE/BUG.yml`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/.github/ISSUE_TEMPLATE/feature.yml` & `citric-1.0.1a2/.github/ISSUE_TEMPLATE/feature.yml`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/.github/actions/install-tools/action.yml` & `citric-1.0.1a2/.github/actions/install-tools/action.yml`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/.github/workflows/api-changes.yml` & `citric-1.0.1a2/.github/workflows/api-changes.yml`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/.github/workflows/build.yml` & `citric-1.0.1a2/.github/workflows/build.yml`

 * *Files 9% similar despite different names*

```diff
@@ -47,26 +47,26 @@
   # Move this up when PyPI supports signing
   sign:
     name: Sign the distribution package
     if: startsWith(github.ref, 'refs/tags/') || github.event_name == 'workflow_dispatch'
     runs-on: ubuntu-latest
     needs: [build]
     permissions:
-      contents: write # IMPORTANT: mandatory for making GitHub Releases
-      id-token: write # IMPORTANT: mandatory for sigstore
+      contents: write     # IMPORTANT: mandatory for making GitHub Releases
+      id-token: write     # IMPORTANT: mandatory for attestations
+      attestations: write # IMPORTANT: mandatory for attestations
 
     steps:
       - uses: actions/download-artifact@65a9edc5881444af0b9093a5e628f2fe47ea3b2e
         with:
           name: Packages
           path: dist
-      - uses: sigstore/gh-action-sigstore-python@61f6a500bbfdd9a2a339cf033e5421951fbc1cd2
+      - uses: actions/attest-build-provenance@eab7f69317b589ac05272d67712fdd10ab3d4d1d
+        id: attest
         with:
-          inputs: >-
-            ./dist/*.tar.gz
-            ./dist/*.whl
+          subject-path: "./dist/citric*"
       - uses: svenstaro/upload-release-action@04733e069f2d7f7f0b4aebc4fbdbce8613b03ccd
         with:
-          file: dist/**
+          file: ${{ steps.attest.outputs.bundle-path }}
           tag: ${{ github.event.inputs.tag || github.ref }}
           overwrite: false
           file_glob: true
```

### Comparing `citric-1.0.1a1/.github/workflows/gen-release-pr.yml` & `citric-1.0.1a2/.github/workflows/gen-release-pr.yml`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/.github/workflows/scorecard.yml` & `citric-1.0.1a2/.github/workflows/scorecard.yml`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/.github/workflows/tests.yml` & `citric-1.0.1a2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/code_samples/custom_requests_session.py` & `citric-1.0.1a2/code_samples/custom_requests_session.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/code_samples/duckdb_sql.py` & `citric-1.0.1a2/code_samples/duckdb_sql.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/code_samples/get_surveys.py` & `citric-1.0.1a2/code_samples/get_surveys.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/code_samples/pandas_df.py` & `citric-1.0.1a2/code_samples/pandas_df.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/code_samples/requests_session_attributes.py` & `citric-1.0.1a2/code_samples/requests_session_attributes.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/code_samples/session_attr.py` & `citric-1.0.1a2/code_samples/session_attr.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/code_samples/upload_s3.py` & `citric-1.0.1a2/code_samples/upload_s3.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/docs/code.png` & `citric-1.0.1a2/docs/code.png`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/docs/conf.py` & `citric-1.0.1a2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/docs/how-to.md` & `citric-1.0.1a2/docs/how-to.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/docs/index.md` & `citric-1.0.1a2/docs/index.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/docs/requirements.txt` & `citric-1.0.1a2/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/docs/rest_coverage.md` & `citric-1.0.1a2/docs/rest_coverage.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/docs/rpc_coverage.md` & `citric-1.0.1a2/docs/rpc_coverage.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/docs/_ext/limesurvey_future.py` & `citric-1.0.1a2/docs/_ext/limesurvey_future.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/docs/contributing/docker.md` & `citric-1.0.1a2/docs/contributing/docker.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/docs/contributing/environment.md` & `citric-1.0.1a2/docs/contributing/environment.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/docs/contributing/getting-started.md` & `citric-1.0.1a2/docs/contributing/getting-started.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/docs/contributing/release.md` & `citric-1.0.1a2/docs/contributing/release.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/docs/contributing/testing.md` & `citric-1.0.1a2/docs/contributing/testing.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/docs/contributing/unreleased-features.md` & `citric-1.0.1a2/docs/contributing/unreleased-features.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/docs/notebooks/duckdb.ipynb` & `citric-1.0.1a2/docs/notebooks/duckdb.ipynb`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/docs/notebooks/import_s3.ipynb` & `citric-1.0.1a2/docs/notebooks/import_s3.ipynb`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/docs/notebooks/pandas_sqlite.ipynb` & `citric-1.0.1a2/docs/notebooks/pandas_sqlite.ipynb`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/docs/notebooks/parse_files.ipynb` & `citric-1.0.1a2/docs/notebooks/parse_files.ipynb`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/examples/free_text.lsq` & `citric-1.0.1a2/examples/free_text.lsq`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/examples/group.lsg` & `citric-1.0.1a2/examples/group.lsg`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/examples/limesurvey_survey_432535.lss` & `citric-1.0.1a2/examples/limesurvey_survey_432535.lss`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/examples/survey.lss` & `citric-1.0.1a2/examples/survey.lss`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/scripts/docker_tags.py` & `citric-1.0.1a2/scripts/docker_tags.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/src/citric/_compat.py` & `citric-1.0.1a2/src/citric/_compat.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/src/citric/client.py` & `citric-1.0.1a2/src/citric/client.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/src/citric/enums.py` & `citric-1.0.1a2/src/citric/enums.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/src/citric/exceptions.py` & `citric-1.0.1a2/src/citric/exceptions.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/src/citric/method.py` & `citric-1.0.1a2/src/citric/method.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/src/citric/objects.py` & `citric-1.0.1a2/src/citric/objects.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/src/citric/session.py` & `citric-1.0.1a2/src/citric/session.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/src/citric/types.py` & `citric-1.0.1a2/src/citric/types.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/src/citric/_rest/client.py` & `citric-1.0.1a2/src/citric/_rest/client.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/tests/conftest.py` & `citric-1.0.1a2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/tests/test_client.py` & `citric-1.0.1a2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/tests/test_compat.py` & `citric-1.0.1a2/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/tests/test_rest.py` & `citric-1.0.1a2/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/tests/test_rpc.py` & `citric-1.0.1a2/tests/test_rpc.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/tests/integration/conftest.py` & `citric-1.0.1a2/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/tests/integration/test_rest_client.py` & `citric-1.0.1a2/tests/integration/test_rest_client.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/tests/integration/test_rpc_client.py` & `citric-1.0.1a2/tests/integration/test_rpc_client.py`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/tests/resources/config.php` & `citric-1.0.1a2/tests/resources/config.php`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/.gitignore` & `citric-1.0.1a2/.gitignore`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/LICENSE` & `citric-1.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/README.md` & `citric-1.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/pyproject.toml` & `citric-1.0.1a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `citric-1.0.1a1/PKG-INFO` & `citric-1.0.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: citric
-Version: 1.0.1a1
+Version: 1.0.1a2
 Summary: A client to the LimeSurvey Remote Control API 2, written in modern Python.
 Project-URL: Documentation, https://citric.readthedocs.io
 Project-URL: Homepage, https://github.com/edgarrmondragon/citric
 Project-URL: Issue Tracker, https://github.com/edgarrmondragon/citric/issues
 Project-URL: Repository, https://github.com/edgarrmondragon/citric
 Author-email: Edgar Ramírez-Mondragón <edgarrm358@gmail.com>
 Maintainer-email: Edgar Ramírez-Mondragón <edgarrm358@gmail.com>
```

